# Subsystem: tts

## micro/klatt-tts/include/tts/config.h
- Layer: infrastructure
- Doc: Externalized, tunable voice parameters.  Every "magic number" in the synthesizer lives here so it can be overridden at r
- Language: h
- Symbols:
  - `VoiceParams` (struct, line 24)
  - `TTS_CONFIG_H_` (macro, line 15)

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
  - `TTS_KLATT_H_` (macro, line 22)

## micro/klatt-tts/include/tts/phonemes.h
- Layer: utility
- Doc: English phoneme inventory for the formant synthesizer.  Keyed by IPA (UTF-8), matching the G2P front-end output. Each en
- Language: h
- Symbols:
  - `Phone` (struct, line 45)
  - `TTS_PHONEMES_H_` (macro, line 20)

## micro/klatt-tts/include/tts/synth_internal.h
- Layer: utility
- Doc: Shared internals for the batch (synth.cc) and streaming (synth_stream.cc) drivers. Factoring these out keeps the two pat
- Language: h
- Symbols:
  - `Segment` (struct, line 28)
  - `ParamTracks` (struct, line 65)
  - `TTS_SYNTH_INTERNAL_H_` (macro, line 9)

## micro/klatt-tts/include/tts/synth_stream.h
- Layer: utility
- Doc: Streaming, caller-arena formant synthesizer for the RP2350 (and desktop).  Unlike the batch Synthesize() (synth.h), whic
- Language: h
- Symbols:
  - `StreamOptions` (struct, line 37)
  - `StreamSynth` (class, line 51)
  - `done` (function, line 72) `bool done() const`
  - `sample_rate` (function, line 76) `int sample_rate() const`
  - `total_samples` (function, line 77) `int total_samples() const`
  - `ArenaReset` (function, line 84) `void ArenaReset()`
  - `TTS_SYNTH_STREAM_H_` (macro, line 22)

## micro/klatt-tts/include/tts/tts.h
- Layer: utility
- Doc: tts -- portable, dependency-free formant (Klatt-style) text-to-speech.  This is the single public header for the module.
- Language: h
- Symbols:
  - `TTS_TTS_H_` (macro, line 26)
