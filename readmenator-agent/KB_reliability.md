# Subsystem: reliability

## core/reliability/fuzz-bin-tokenizer.cpp
- Layer: utility
- Doc: libFuzzer harness for the binary tokenizer.  The in-memory BinTokenizer constructor parses an untrusted byte blob (a tok
- Language: cpp
- Symbols:
  - `tokenizer` (function, line 21) `BinTokenizer tokenizer(data, size);`
  - `text` (function, line 25) `const std::string text(data, data + text_size);`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`

## core/reliability/fuzz-resampler.cpp
- Layer: utility
- Doc: libFuzzer harness for the audio resampler.  The input is split into two float sample rates followed by float PCM samples
- Language: cpp
- Symbols:
  - `sane_rate` (function, line 17) `float sane_rate(float rate)`
  - `memcpy` (function, line 39) `std::memcpy(&input_rate, data, sizeof(float));`
  - `audio` (function, line 45) `std::vector<float> audio(num_samples);`
  - `resample_audio` (function, line 49) `resample_audio(audio, input_rate, output_rate);`
  - `0` (variable, line 31) `extern "C" int LLVMFuzzerTestOneInput(const uint8_t *data, size_t size) { // Layout: [4 bytes input rate][4 bytes output rate][float samples...]. if (size < 8) { return 0;`
- Depends on: `core/resampler.h`

## core/reliability/fuzz-string-utils.cpp
- Layer: utility
- Doc: libFuzzer harness for the string utilities.  Feeds arbitrary bytes through the trimming, splitting, path, and typed-pars
- Language: cpp
- Symbols:
  - `input` (function, line 15) `const std::string input(data, data + size);`
  - `trim` (function, line 16) `trim(input);`
  - `to_lowercase` (function, line 18) `to_lowercase(input);`
  - `starts_with` (function, line 19) `starts_with(input, "prefix");`
  - `ends_with` (function, line 20) `ends_with(input, "suffix");`
  - `replace_all` (function, line 21) `replace_all(input, " ", "_");`
  - `split` (function, line 22) `split(input, ",");`
  - `append_path_component` (function, line 23) `append_path_component(input, input);`
  - `bool_from_string` (function, line 26) `bool_from_string(input);`
  - `float_from_string` (function, line 30) `float_from_string(input);`
  - `int32_from_string` (function, line 34) `int32_from_string(input);`
  - `size_t_from_string` (function, line 38) `size_t_from_string(input);`
- Depends on: `core/moonshine-utils/string-utils.h`

## core/reliability/fuzz-tensor-view.cpp
- Layer: presentation
- Doc: libFuzzer harness for MoonshineTensorView construction.  The shape/dtype/data constructor forwards to moonshine_tensor_f
- Language: cpp
- Symbols:
  - `Reader` (struct, line 21)
  - `next_u8` (function, line 25) `uint8_t next_u8()`
  - `next_i64` (function, line 27) `int64_t next_i64()`
  - `source` (function, line 82) `std::vector<uint8_t> source(element_count * 8, 0);`
  - `view` (function, line 83) `MoonshineTensorView view(shape, dtype, source.data(), "fuzz");`
- Depends on: `core/ort-utils/moonshine-tensor-view.h`

## core/reliability/fuzz-wav-pcm.cpp
- Layer: utility
- Doc: libFuzzer harness for the WAV/RIFF parsers.  Both readers take a file path, so we write the fuzz input to a temporary fi
- Language: cpp
- Symbols:
  - `close` (function, line 32) `close(fd);`
  - `free` (function, line 39) `free(samples);`
  - `load_wav_pcm16_mono_float32` (function, line 45) `wav_pcm::load_wav_pcm16_mono_float32(std::string(path_template), sr);`
  - `unlink` (function, line 49) `unlink(path_template);`
- Depends on: `core/cpp-annote/src/wav_pcm_float32.h`, `core/moonshine-utils/debug-utils.h`
