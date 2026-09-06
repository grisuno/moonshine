# Subsystem: reliability

## core/reliability/fuzz-bin-tokenizer.cpp
- Layer: utility
- Doc: libFuzzer harness for the binary tokenizer.  The in-memory BinTokenizer constructor parses an untrusted byte blob (a tok
- Language: cpp

## core/reliability/fuzz-resampler.cpp
- Layer: utility
- Doc: libFuzzer harness for the audio resampler.  The input is split into two float sample rates followed by float PCM samples
- Language: cpp
- Symbols:
  - `sane_rate` (function, line 17) `float sane_rate(float rate)`

## core/reliability/fuzz-string-utils.cpp
- Layer: utility
- Doc: libFuzzer harness for the string utilities.  Feeds arbitrary bytes through the trimming, splitting, path, and typed-pars
- Language: cpp

## core/reliability/fuzz-tensor-view.cpp
- Layer: presentation
- Doc: libFuzzer harness for MoonshineTensorView construction.  The shape/dtype/data constructor forwards to moonshine_tensor_f
- Language: cpp
- Symbols:
  - `Reader` (struct, line 21)
  - `next_u8` (function, line 25) `uint8_t next_u8()`
  - `next_i64` (function, line 27) `int64_t next_i64()`

## core/reliability/fuzz-wav-pcm.cpp
- Layer: utility
- Doc: libFuzzer harness for the WAV/RIFF parsers.  Both readers take a file path, so we write the fuzz input to a temporary fi
- Language: cpp
