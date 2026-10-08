# Subsystem: reliability

## core/reliability/fuzz-bin-tokenizer.cpp
- Doc: libFuzzer harness for the binary tokenizer.
- Layer: utility
- Language: cpp
- Symbols:
  - `text` (function, line 25) `const std::string text(data, data + text_size);`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`

## core/reliability/fuzz-resampler.cpp
- Doc: libFuzzer harness for the audio resampler.
- Layer: utility
- Language: cpp
- Symbols:
  - `sane_rate` (function, line 17) `float sane_rate(float rate)`
  - `audio` (function, line 45) `std::vector<float> audio(num_samples);`
  - `0` (variable, line 32) `extern "C" int LLVMFuzzerTestOneInput(const uint8_t *data, size_t size) { // Layout: [4 bytes input rate][4 bytes...`
- Depends on: `core/resampler.h`

## core/reliability/fuzz-string-utils.cpp
- Doc: libFuzzer harness for the string utilities.
- Layer: utility
- Language: cpp
- Symbols:
  - `input` (function, line 15) `const std::string input(data, data + size);`
- Depends on: `core/moonshine-utils/string-utils.h`

## core/reliability/fuzz-tensor-view.cpp
- Doc: libFuzzer harness for MoonshineTensorView construction.
- Layer: presentation
- Language: cpp
- Symbols:
  - `Reader` (struct, line 21)
  - `next_u8` (function, line 26) `uint8_t next_u8()`
  - `next_i64` (function, line 28) `int64_t next_i64()`
  - `source` (function, line 82) `std::vector<uint8_t> source(element_count * 8, 0);`
- Depends on: `core/ort-utils/moonshine-tensor-view.h`

## core/reliability/fuzz-wav-pcm.cpp
- Doc: libFuzzer harness for the WAV/RIFF parsers.
- Layer: utility
- Language: cpp
- Depends on: `core/cpp-annote/src/wav_pcm_float32.h`, `core/moonshine-utils/debug-utils.h`
