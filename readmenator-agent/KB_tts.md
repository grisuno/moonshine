# Subsystem: tts

## micro/klatt-tts/include/tts/config.h
- Layer: infrastructure
- Doc: Externalized, tunable voice parameters.  Every "magic number" in the synthesizer lives here so it can be overridden at r
- Language: h
- Symbols:
  - `VoiceParams` (struct, line 24)
  - `Lookup` (function, line 127) `const Phone* Lookup(const std::string& ipa) const;`
  - `DefaultVoiceParams` (function, line 132) `VoiceParams DefaultVoiceParams();`
  - `LoadVoiceConfig` (function, line 136) `bool LoadVoiceConfig(const std::string& path, VoiceParams& vp);`
  - `DumpVoiceConfig` (function, line 140) `bool DumpVoiceConfig(const std::string& path, const VoiceParams& vp);`
  - `TTS_CONFIG_H_` (macro, line 15) `#define TTS_CONFIG_H_`
- Depends on: `micro/klatt-tts/include/tts/phonemes.h`
- Imported by: `micro/klatt-tts/include/tts/synth_internal.h`, `micro/klatt-tts/include/tts/synth_stream.h`, `micro/klatt-tts/include/tts/tts.h`, `micro/klatt-tts/src/config.cc`, `micro/neural-tts/src/neural_tts.cc`

## micro/klatt-tts/include/tts/klatt.h
- Layer: utility
- Doc: Klatt-style cascade formant synthesizer (simplified).  This is the "coral" stage from the design notes: it turns a strea
- Language: h
- Symbols:
  - `SynthFrame` (struct, line 32)
  - `Resonator` (struct, line 46)
  - `KlattParams` (struct, line 62)
  - `Biquad` (struct, line 101)
  - `Antiresonator` (struct, line 120)
  - `KlattSynth` (class, line 134)
  - `Step` (function, line 51) `inline float Step(float x)`
  - `Reset` (function, line 57) `void Reset()`
  - `Step` (function, line 108) `inline float Step(float x)`
  - `Reset` (function, line 116) `void Reset()`
  - `Step` (function, line 125) `inline float Step(float x)`
  - `Reset` (function, line 131) `void Reset()`
  - `SetParams` (function, line 49) `void SetParams(float freq_hz, float bw_hz, float sample_rate);`
  - `SetBandpass` (function, line 107) `void SetBandpass(float freq_hz, float q, float sample_rate);`
  - `KlattSynth` (function, line 135) `public: KlattSynth(float sample_rate, const KlattParams& params);`
  - `Render` (function, line 141) `std::vector<float> Render(const std::vector<SynthFrame>& frames, int samples_per_frame);`
  - `RenderFrame` (function, line 150) `void RenderFrame(const SynthFrame& cur, const SynthFrame& nxt, int samples_per_frame, float* out);`
  - `NextNoise` (function, line 152) `private: float NextNoise();`
  - `EnsureLfShape` (function, line 157) `void EnsureLfShape(float rd);`
  - `LfDeriv` (function, line 160) `inline float LfDeriv(float phase) const;`
  - `TTS_KLATT_H_` (macro, line 22) `#define TTS_KLATT_H_`
- Imported by: `micro/klatt-tts/include/tts/synth_internal.h`, `micro/klatt-tts/include/tts/synth_stream.h`, `micro/klatt-tts/src/klatt.cc`

## micro/klatt-tts/include/tts/phonemes.h
- Layer: utility
- Doc: English phoneme inventory for the formant synthesizer.  Keyed by IPA (UTF-8), matching the G2P front-end output. Each en
- Language: h
- Symbols:
  - `Phone` (struct, line 45)
  - `PhoneClass` (enum, line 28)
  - `Source` (enum, line 38)
  - `LookupPhone` (function, line 72) `const Phone* LookupPhone(const std::string& ipa);`
  - `DefaultPhoneTable` (function, line 77) `std::vector<Phone> DefaultPhoneTable();`
  - `TTS_PHONEMES_H_` (macro, line 20) `#define TTS_PHONEMES_H_`
- Imported by: `micro/klatt-tts/include/tts/config.h`, `micro/klatt-tts/src/phonemes.cc`, `micro/klatt-tts/src/synth_internal.cc`, `micro/klatt-tts/src/synth_stream.cc`

## micro/klatt-tts/include/tts/synth_internal.h
- Layer: utility
- Doc: Shared internals for the batch (synth.cc) and streaming (synth_stream.cc) drivers. Factoring these out keeps the two pat
- Language: h
- Symbols:
  - `Segment` (struct, line 28)
  - `ParamTracks` (struct, line 65)
  - `SmoothBidir` (function, line 45) `void SmoothBidir(float* v, size_t n, float tau_ms);`
  - `SmoothFwd` (function, line 46) `void SmoothFwd(float* v, size_t n, float tau_ms);`
  - `SmoothAsym` (function, line 47) `void SmoothAsym(float* v, size_t n, float attack_ms, float release_ms);`
  - `BuildSegments` (function, line 51) `std::vector<Segment> BuildSegments(const std::vector<std::string>& phones, const VoiceParams& vp);`
  - `CountFrames` (function, line 60) `size_t CountFrames(const std::vector<Segment>& segs, float dur_scale);`
  - `FillParamTracks` (function, line 88) `void FillParamTracks(const std::vector<Segment>& segs, const VoiceParams& vp, float dur_scale, bool question, ParamTracks& t);`
  - `FrameAt` (function, line 92) `SynthFrame FrameAt(const ParamTracks& t, size_t i);`
  - `MakeKlattParams` (function, line 96) `KlattParams MakeKlattParams(const VoiceParams& vp);`
  - `TTS_SYNTH_INTERNAL_H_` (macro, line 9) `#define TTS_SYNTH_INTERNAL_H_`
- Depends on: `micro/klatt-tts/include/tts/config.h`, `micro/klatt-tts/include/tts/klatt.h`
- Imported by: `micro/klatt-tts/include/tts/synth_stream.h`, `micro/klatt-tts/src/synth_internal.cc`, `micro/neural-tts/src/neural_tts.cc`

## micro/klatt-tts/include/tts/synth_stream.h
- Layer: utility
- Doc: Streaming, caller-arena formant synthesizer for the RP2350 (and desktop).  Unlike the batch Synthesize() (synth.h), whic
- Language: h
- Symbols:
  - `StreamOptions` (struct, line 37)
  - `StreamStatus` (enum, line 44)
  - `StreamSynth` (class, line 51)
  - `done` (function, line 72) `bool done() const`
  - `sample_rate` (function, line 76) `int sample_rate() const`
  - `total_samples` (function, line 77) `int total_samples() const`
  - `ArenaReset` (function, line 84) `void ArenaReset()`
  - `StreamSynth` (function, line 57) `StreamSynth(const VoiceParams& vp, uint8_t* arena, size_t arena_size);`
  - `BeginText` (function, line 61) `int BeginText(const char* text, const StreamOptions& opts, const g2p::Lexicon* overrides = nullptr);`
  - `BeginIpa` (function, line 66) `int BeginIpa(const char* ipa, const StreamOptions& opts);`
  - `Read` (function, line 71) `int Read(float* out, int max_samples);`
  - `BeginPhones` (function, line 80) `private: int BeginPhones(const std::vector<std::string>& phones, const StreamOptions& opts);`
  - `ArenaFloats` (function, line 85) `float* ArenaFloats(size_t count);`
  - `ArenaBytes` (function, line 86) `uint8_t* ArenaBytes(size_t count, size_t align);`
  - `RenderNextFrame` (function, line 87) `void RenderNextFrame();`
  - `TTS_SYNTH_STREAM_H_` (macro, line 22) `#define TTS_SYNTH_STREAM_H_`
- Depends on: `micro/g2p/include/g2p/g2p_dict.h`, `micro/klatt-tts/include/tts/config.h`, `micro/klatt-tts/include/tts/klatt.h`, `micro/klatt-tts/include/tts/synth_internal.h`
- Imported by: `micro/klatt-tts/include/tts/tts.h`, `micro/klatt-tts/src/synth_stream.cc`

## micro/klatt-tts/include/tts/tts.h
- Layer: utility
- Doc: tts -- portable, dependency-free formant (Klatt-style) text-to-speech.  This is the single public header for the module.
- Language: h
- Symbols:
  - `TTS_TTS_H_` (macro, line 26) `#define TTS_TTS_H_`
- Depends on: `micro/klatt-tts/include/tts/config.h`, `micro/klatt-tts/include/tts/synth_stream.h`
- Imported by: `micro/klatt-tts/tests/tts_test.cc`
