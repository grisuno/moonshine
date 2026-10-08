# Subsystem: micro_klatt-tts_src

## micro/klatt-tts/src/config.cc
- Doc: SetPhoneField: Apply one "<field> <value>" override to a phone.
- Layer: infrastructure
- Language: cc
- Symbols:
  - `ClassName` (function, line 14) `const char* ClassName(PhoneClass c)`
  - `SourceName` (function, line 34) `const char* SourceName(Source s)`
  - `SetPhoneField` (function, line 105) `bool SetPhoneField(Phone& p, const std::string& field, float v)`
  - `Lookup` (function, line 139) `const Phone* VoiceParams::Lookup(const std::string& ipa) const`
  - `DefaultVoiceParams` (function, line 146) `VoiceParams DefaultVoiceParams()`
  - `LoadVoiceConfig` (function, line 152) `bool LoadVoiceConfig(const std::string& path, VoiceParams& vp)`
  - `DumpVoiceConfig` (function, line 216) `bool DumpVoiceConfig(const std::string& path, const VoiceParams& vp)`
- Depends on: `micro/klatt-tts/include/tts/config.h`

## micro/klatt-tts/src/klatt.cc
- Doc: GlottalPulse: Rosenberg-style glottal flow pulse as a function of phase in [0, 1).
- Layer: utility
- Language: cc
- Symbols:
  - `GlottalPulse` (function, line 16) `inline float GlottalPulse(float phase, float open, float close)`
  - `TiltCoef` (function, line 29) `float TiltCoef(float tilt_db, float sample_rate)`
  - `SetParams` (function, line 48) `void Resonator::SetParams(float freq_hz, float bw_hz, float sample_rate)`
  - `SetBandpass` (function, line 55) `void Biquad::SetBandpass(float freq_hz, float q, float sample_rate)`
  - `SetParams` (function, line 70) `void Antiresonator::SetParams(float freq_hz, float bw_hz, float sample_rate)`
  - `KlattSynth` (function, line 82) `KlattSynth::KlattSynth(float sample_rate, const KlattParams& params)
    : sample_rate_(sample_ra...`
  - `EnsureLfShape` (function, line 94) `void KlattSynth::EnsureLfShape(float rd)`
  - `LfDeriv` (function, line 165) `inline float KlattSynth::LfDeriv(float phase) const`
  - `NextNoise` (function, line 173) `float KlattSynth::NextNoise()`
  - `RenderFrame` (function, line 181) `void KlattSynth::RenderFrame(const SynthFrame& cur, const SynthFrame& nxt,
                      ...`
  - `Render` (function, line 296) `std::vector<float> KlattSynth::Render(const std::vector<SynthFrame>& frames,
                    ...`
- Depends on: `micro/klatt-tts/include/tts/klatt.h`

## micro/klatt-tts/src/phonemes.cc
- Layer: utility
- Language: cc
- Symbols:
  - `LookupPhone` (function, line 90) `const Phone* LookupPhone(const std::string& ipa)`
  - `DefaultPhoneTable` (function, line 96) `std::vector<Phone> DefaultPhoneTable()`
- Depends on: `micro/klatt-tts/include/tts/phonemes.h`

## micro/klatt-tts/src/synth_internal.cc
- Doc: AppendStop: Expand a stop into closure -> burst -> (aspiration) sub-segments so that...
- Layer: utility
- Language: cc
- Symbols:
  - `SegFromPhone` (function, line 15) `Segment SegFromPhone(const Phone& p)`
  - `AppendStop` (function, line 38) `void AppendStop(const Phone& p, const VoiceParams& vp, int src_token,
                Segment* ou...`
  - `BuildSegments` (function, line 75) `int BuildSegments(const char* const* phones, int n_phones, const VoiceParams& vp,
               ...`
  - `BuildSegments` (function, line 176) `std::vector<Segment> BuildSegments(const std::vector<std::string>& phones,
                      ...`
  - `SmoothBidir` (function, line 190) `void SmoothBidir(float* v, size_t n, float tau_ms)`
  - `SmoothFwd` (function, line 201) `void SmoothFwd(float* v, size_t n, float tau_ms)`
  - `SmoothAsym` (function, line 209) `void SmoothAsym(float* v, size_t n, float attack_ms, float release_ms)`
  - `CountFrames` (function, line 222) `size_t CountFrames(const std::vector<Segment>& segs, float dur_scale)`
  - `FillParamTracks` (function, line 232) `void FillParamTracks(const std::vector<Segment>& segs, const VoiceParams& vp,
                   ...`
  - `FrameAt` (function, line 339) `SynthFrame FrameAt(const ParamTracks& t, size_t i)`
  - `MakeKlattParams` (function, line 358) `KlattParams MakeKlattParams(const VoiceParams& vp)`
- Depends on: `micro/klatt-tts/include/tts/phonemes.h`, `micro/klatt-tts/include/tts/synth_internal.h`

## micro/klatt-tts/src/synth_stream.cc
- Doc: SoftClip: Soft limiter: perfectly linear up to a knee (so the RMS body of the signal is...
- Layer: utility
- Language: cc
- Symbols:
  - `SoftClip` (function, line 18) `inline float SoftClip(float x)`
  - `StreamSynth` (function, line 30) `StreamSynth::StreamSynth(const VoiceParams& vp, uint8_t* arena,
                         size_t a...`
  - `ArenaBytes` (function, line 34) `uint8_t* StreamSynth::ArenaBytes(size_t count, size_t align)`
  - `ArenaFloats` (function, line 41) `float* StreamSynth::ArenaFloats(size_t count)`
  - `BeginText` (function, line 46) `int StreamSynth::BeginText(const char* text, const StreamOptions& opts,
                         ...`
  - `BeginIpa` (function, line 54) `int StreamSynth::BeginIpa(const char* ipa, const StreamOptions& opts)`
  - `BeginPhones` (function, line 60) `int StreamSynth::BeginPhones(const std::vector<std::string>& phones,
                            ...`
  - `RenderNextFrame` (function, line 125) `void StreamSynth::RenderNextFrame()`
  - `Read` (function, line 140) `int StreamSynth::Read(float* out, int max_samples)`
- Depends on: `micro/g2p/include/g2p/g2p.h`, `micro/klatt-tts/include/tts/phonemes.h`, `micro/klatt-tts/include/tts/synth_stream.h`
