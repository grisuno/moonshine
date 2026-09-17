# Subsystem: reliability

## core/reliability/fuzz-bin-tokenizer.cpp
- Layer: utility
- Doc: libFuzzer harness for the binary tokenizer.  The in-memory BinTokenizer constructor parses an untrusted byte blob (a tok
- Language: cpp
- Symbols:
  - `text` (function, line 25) `const std::string text(data, data + text_size);`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`

## core/reliability/fuzz-resampler.cpp
- Layer: utility
- Doc: libFuzzer harness for the audio resampler.  The input is split into two float sample rates followed by float PCM samples
- Language: cpp
- Symbols:
  - `sane_rate` (function, line 17) `float sane_rate(float rate)`
  - `audio` (function, line 45) `std::vector<float> audio(num_samples);`
  - `0` (variable, line 32) `extern "C" int LLVMFuzzerTestOneInput(const uint8_t *data, size_t size) { // Layout: [4 bytes input rate][4 bytes output rate][float samples...]. if (size < 8) { return 0;`
- Depends on: `core/resampler.h`

## core/reliability/fuzz-string-utils.cpp
- Layer: utility
- Doc: libFuzzer harness for the string utilities.  Feeds arbitrary bytes through the trimming, splitting, path, and typed-pars
- Language: cpp
- Symbols:
  - `input` (function, line 15) `const std::string input(data, data + size);`
- Depends on: `core/moonshine-utils/string-utils.h`

## core/reliability/fuzz-tensor-view.cpp
- Layer: presentation
- Doc: libFuzzer harness for MoonshineTensorView construction.  The shape/dtype/data constructor forwards to moonshine_tensor_f
- Language: cpp
- Symbols:
  - `Reader` (struct, line 21)
  - `next_u8` (function, line 26) `uint8_t next_u8()`
  - `next_i64` (function, line 28) `int64_t next_i64()`
  - `source` (function, line 82) `std::vector<uint8_t> source(element_count * 8, 0);`
- Depends on: `core/ort-utils/moonshine-tensor-view.h`

## core/reliability/fuzz-wav-pcm.cpp
- Layer: utility
- Doc: libFuzzer harness for the WAV/RIFF parsers.  Both readers take a file path, so we write the fuzz input to a temporary fi
- Language: cpp
- Depends on: `core/cpp-annote/src/wav_pcm_float32.h`, `core/moonshine-utils/debug-utils.h`
