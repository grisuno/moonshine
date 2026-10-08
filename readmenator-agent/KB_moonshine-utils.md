# Subsystem: moonshine-utils

## core/moonshine-utils/debug-utils-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `return_on_error_test` (function, line 10) `int return_on_error_test()`
  - `return_on_false_test` (function, line 15) `int return_on_false_test()`
  - `return_on_null_test` (function, line 20) `int return_on_null_test()`
  - `return_on_not_equal_test` (function, line 25) `int return_on_not_equal_test()`
  - `TEST_CASE` (function, line 31) `TEST_CASE("debug-utils")`
  - `SUBCASE` (function, line 32) `SUBCASE("LOG")`
  - `SUBCASE` (function, line 36) `SUBCASE("RETURN_ON_ERROR")`
  - `SUBCASE` (function, line 37) `SUBCASE("RETURN_ON_FALSE")`
  - `SUBCASE` (function, line 38) `SUBCASE("RETURN_ON_NULL")`
  - `SUBCASE` (function, line 39) `SUBCASE("RETURN_ON_NOT_EQUAL")`
  - `SUBCASE` (function, line 40) `SUBCASE("TIMER")`
  - `SUBCASE` (function, line 45) `SUBCASE("DEBUG_CALLOC")`
  - `SUBCASE` (function, line 51) `SUBCASE("TRACE")`
  - `SUBCASE` (function, line 55) `SUBCASE("LOG_VARS")`
  - `SUBCASE` (function, line 76) `SUBCASE("load_file_into_memory")`
  - `SUBCASE` (function, line 87) `SUBCASE("save_memory_to_file")`
  - `SUBCASE` (function, line 100) `SUBCASE("load_wav_data_beckett")`
  - `SUBCASE` (function, line 114) `SUBCASE("load_wav_data_two_cities")`
  - `SUBCASE` (function, line 128) `SUBCASE("save_wav_data")`
  - `read_data` (function, line 93) `std::vector<uint8_t> read_data(data.size());`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 6) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-utils/debug-utils.h`

## core/moonshine-utils/debug-utils.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `log_backtrace` (function, line 16) `void log_backtrace()`
  - `load_wav_data` (function, line 52) `bool load_wav_data(const char *path, float **out_float_data,
                   size_t *out_num_s...`
  - `save_wav_data` (function, line 197) `bool save_wav_data(const char *path, const float *audio_data,
                   size_t num_sampl...`
  - `float_vector_stats_to_string` (function, line 250) `std::string float_vector_stats_to_string(const std::vector<float> &vector)`
  - `load_file_into_memory` (function, line 269) `std::vector<uint8_t> load_file_into_memory(const std::string &path)`
  - `save_memory_to_file` (function, line 290) `void save_memory_to_file(const std::string &path,
                         const std::vector<uint...`
  - `audio_int16` (function, line 205) `std::vector<int16_t> audio_int16(num_samples);`
  - `data` (function, line 277) `std::vector<uint8_t> data(size);`
- Depends on: `core/moonshine-utils/debug-utils.h`

## core/moonshine-utils/debug-utils.h
- Doc: debug_calloc: define DEBUG_CALLOC(size, count) \
- Layer: utility
- Language: h
- Symbols:
  - `_moonshine_filename_without_path` (function, line 15) `static inline const char *_moonshine_filename_without_path(const char *path)`
  - `debug_calloc` (function, line 139) `debug_calloc(size, count, FILENAME_ONLY, __LINE__, __FUNCTION__)

static inline void *debug_callo...`
  - `debug_free` (function, line 156) `static inline void debug_free(void *voidMemPtr, const char *file, int line,
                     ...`
  - `debug_alloc_get_size` (function, line 176) `static inline size_t debug_alloc_get_size(void *voidMemPtr)`
  - `gate` (function, line 268) `template <typename T>
T gate(T value, T min, T max)`
  - `log_backtrace` (function, line 253) `void log_backtrace();`
  - `load_wav_data` (function, line 255) `bool load_wav_data(const char *path, float **out_float_data, size_t *out_num_samples, int32_t *out_sample_rate =...`
  - `save_wav_data` (function, line 258) `bool save_wav_data(const char *path, const float *audio_data, size_t num_samples, uint32_t sample_rate = 16000);`
  - `load_file_into_memory` (function, line 263) `std::vector<uint8_t> load_file_into_memory(const std::string &path);`
  - `save_memory_to_file` (function, line 264) `void save_memory_to_file(const std::string &path, const std::vector<uint8_t> &data);`
  - `UTILS_H` (macro, line 2) `#define UTILS_H`
  - `FILENAME_ONLY` (macro, line 23) `#define FILENAME_ONLY`
  - `LOGF` (macro, line 27) `#define LOGF(format, ...)`
  - `LOGF` (macro, line 33) `#define LOGF(format, ...)`
  - `LOG` (macro, line 43) `#define LOG(x)`
  - `LOG_IF` (macro, line 45) `#define LOG_IF(condition, x)`
  - `LOGF_IF` (macro, line 50) `#define LOGF_IF(condition, format, ...)`
  - `RETURN_ON_ERROR` (macro, line 55) `#define RETURN_ON_ERROR(error)`
  - `RETURN_ON_FALSE` (macro, line 63) `#define RETURN_ON_FALSE(expr)`
  - `RETURN_ON_NULL` (macro, line 71) `#define RETURN_ON_NULL(ptr)`
  - `RETURN_ON_NOT_EQUAL` (macro, line 79) `#define RETURN_ON_NOT_EQUAL(expr1, expr2)`
  - `RETURN_ON_FILE_DOES_NOT_EXIST` (macro, line 87) `#define RETURN_ON_FILE_DOES_NOT_EXIST(path)`
  - `ENABLE_TIMER` (macro, line 95) `#define ENABLE_TIMER`
  - `TIMER_START` (macro, line 99) `#define TIMER_START(x)`
  - `TIMER_END` (macro, line 102) `#define TIMER_END(x)`
  - `TIMER_START_IF` (macro, line 111) `#define TIMER_START_IF(condition, x)`
  - `TIMER_END_IF` (macro, line 114) `#define TIMER_END_IF(condition, x)`
  - `TIMER_START` (macro, line 119) `#define TIMER_START(x)`
  - `TIMER_END` (macro, line 120) `#define TIMER_END(x)`
  - `TIMER_START_IF` (macro, line 121) `#define TIMER_START_IF(condition, x)`
  - `TIMER_END_IF` (macro, line 122) `#define TIMER_END_IF(condition, x)`
  - `DEBUG_ALLOC_MAGIC` (macro, line 132) `#define DEBUG_ALLOC_MAGIC`
  - `DEBUG_ALLOC_ALIGNMENT` (macro, line 134) `#define DEBUG_ALLOC_ALIGNMENT`
  - `DEBUG_ALLOC_LOG_MIN_SIZE` (macro, line 136) `#define DEBUG_ALLOC_LOG_MIN_SIZE`
  - `DEBUG_CALLOC` (macro, line 138) `#define DEBUG_CALLOC(size, count)`
  - `DEBUG_FREE` (macro, line 154) `#define DEBUG_FREE(ptr)`
  - `DEBUG_CALLOC` (macro, line 195) `#define DEBUG_CALLOC(size, count)`
  - `DEBUG_FREE` (macro, line 196) `#define DEBUG_FREE(ptr)`
  - `TRACE` (macro, line 200) `#define TRACE()`
  - `THROW_WITH_LOG` (macro, line 205) `#define THROW_WITH_LOG(message)`
  - `LOG_INT` (macro, line 213) `#define LOG_INT(x)`
  - `LOG_INT64` (macro, line 214) `#define LOG_INT64(x)`
  - `LOG_UINT64` (macro, line 215) `#define LOG_UINT64(x)`
  - `LOG_LONG` (macro, line 216) `#define LOG_LONG(x)`
  - `LOG_SIZET` (macro, line 217) `#define LOG_SIZET(x)`
  - `LOG_PTR` (macro, line 218) `#define LOG_PTR(x)`
  - `LOG_VECTOR` (macro, line 219) `#define LOG_VECTOR(x)`
  - `LOG_FLOAT` (macro, line 232) `#define LOG_FLOAT(x)`
  - `LOG_STRING` (macro, line 233) `#define LOG_STRING(x)`
  - `LOG_BOOL` (macro, line 234) `#define LOG_BOOL(x)`
  - `LOG_BYTES` (macro, line 235) `#define LOG_BYTES(x, size)`
  - `LOG_STRUCT_BYTES` (macro, line 251) `#define LOG_STRUCT_BYTES(x)`
- Imported by: `core/bin-tokenizer/bin-tokenizer-test.cpp`, `core/bin-tokenizer/bin-tokenizer.cpp`, `core/gemma-embedding-model.cpp`, `core/moonshine-c-api-test.cpp`, `core/moonshine-c-api.cpp`, `core/moonshine-download-smoke.cpp`, `core/moonshine-model.cpp`, `core/moonshine-streaming-model.cpp`, `core/moonshine-tts/src/lang-specific/korean.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/moonshine-tts.cpp`, `core/moonshine-tts/src/piper-tts.cpp`, `core/moonshine-tts/src/zipvoice-tts.cpp`, `core/moonshine-utils/debug-utils-test.cpp`, `core/moonshine-utils/debug-utils.cpp`, `core/moonshine-utils/file-utils.cpp`, `core/moonshine-utils/test-utils.h`, `core/ort-utils/moonshine-ort-allocator.cpp`, `core/ort-utils/moonshine-tensor-view.cpp`, `core/ort-utils/moonshine-tensor.cpp`, `core/ort-utils/ort-utils.h`, `core/reliability/fuzz-wav-pcm.cpp`, `core/resampler-test.cpp`, `core/resampler.cpp`, `core/speaker-diarizer.cpp`, `core/spelling-model-test.cpp`, `core/spelling-model.cpp`, `core/voice-activity-detector-test.cpp`, `core/voice-activity-detector.cpp`, `core/word-alignment-test.cpp`

## core/moonshine-utils/file-utils-test.cpp
- Doc: write_file: Writes `bytes` to `path` for the read-back tests below.
- Layer: testing
- Language: cpp
- Symbols:
  - `write_file` (function, line 14) `void write_file(const char *path, const std::vector<uint8_t> &bytes)`
  - `TEST_CASE` (function, line 25) `TEST_CASE("fread_exact")`
  - `SUBCASE` (function, line 28) `SUBCASE("reads the full requested amount")`
  - `SUBCASE` (function, line 42) `SUBCASE("reads multi-byte elements and preserves values")`
  - `SUBCASE` (function, line 59) `SUBCASE("throws when fewer elements are available than requested")`
  - `SUBCASE` (function, line 72) `SUBCASE("throws on a partial trailing element")`
  - `SUBCASE` (function, line 85) `SUBCASE("throws when reading past end of file")`
  - `SUBCASE` (function, line 100) `SUBCASE("zero count is a no-op that returns count")`
  - `SUBCASE` (function, line 109) `SUBCASE("zero size is a no-op that returns count")`
  - `buffer` (function, line 34) `std::vector<uint8_t> buffer(contents.size());`
  - `contents` (function, line 44) `std::vector<uint8_t> contents(sizeof(values));`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 9) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-utils/file-utils.h`

## core/moonshine-utils/file-utils.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `fread_exact` (function, line 10) `std::size_t fread_exact(void *ptr, std::size_t size, std::size_t count,
                        s...`
- Depends on: `core/moonshine-utils/debug-utils.h`, `core/moonshine-utils/file-utils.h`

## core/moonshine-utils/file-utils.h
- Doc: Wrapper around std::fread that throws std::runtime_error unless the full requested number of...
- Layer: utility
- Language: h
- Symbols:
  - `fread_exact` (function, line 12) `std::size_t fread_exact(void *ptr, std::size_t size, std::size_t count, std::FILE *stream, const char *what = "file");`
  - `FILE_UTILS_H` (macro, line 2) `#define FILE_UTILS_H`
- Imported by: `core/benchmark.cpp`, `core/bin-tokenizer/bin-tokenizer.cpp`, `core/moonshine-utils/file-utils-test.cpp`, `core/moonshine-utils/file-utils.cpp`, `core/word-alignment-benchmark.cpp`

## core/moonshine-utils/string-utils-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 8) `TEST_CASE("string-utils")`
  - `SUBCASE` (function, line 9) `SUBCASE("replace_all")`
  - `SUBCASE` (function, line 12) `SUBCASE("trim")`
  - `SUBCASE` (function, line 13) `SUBCASE("split")`
  - `SUBCASE` (function, line 17) `SUBCASE("starts_with")`
  - `SUBCASE` (function, line 18) `SUBCASE("starts_with_invalid")`
  - `SUBCASE` (function, line 21) `SUBCASE("ends_with")`
  - `SUBCASE` (function, line 22) `SUBCASE("ends_with_invalid")`
  - `SUBCASE` (function, line 25) `SUBCASE("name_to_index")`
  - `SUBCASE` (function, line 29) `SUBCASE("append_path_component")`
  - `SUBCASE` (function, line 35) `SUBCASE("to_lowercase")`
  - `SUBCASE` (function, line 40) `SUBCASE("bool_from_string")`
  - `SUBCASE` (function, line 46) `SUBCASE("bool_from_string_invalid")`
  - `SUBCASE` (function, line 51) `SUBCASE("float_from_string")`
  - `SUBCASE` (function, line 56) `SUBCASE("float_from_string_invalid")`
  - `SUBCASE` (function, line 61) `SUBCASE("int32_from_string")`
  - `SUBCASE` (function, line 66) `SUBCASE("int32_from_string_invalid")`
  - `SUBCASE` (function, line 71) `SUBCASE("size_t_from_string")`
  - `SUBCASE` (function, line 76) `SUBCASE("size_t_from_string_invalid")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 5) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-utils/string-utils.h`

## core/moonshine-utils/string-utils.cpp
- Doc: See https://stackoverflow.com/questions/2896600/how-to-replace-all-occurrences-of-a-character-in...
- Layer: utility
- Language: cpp
- Symbols:
  - `replace_all` (function, line 9) `std::string replace_all(std::string str, const std::string &from,
                        const s...`
  - `trim` (function, line 21) `std::string trim(const std::string &str, const std::string &whitespace)`
  - `split` (function, line 31) `std::vector<std::string> split(const std::string &str,
                               const std::...`
  - `starts_with` (function, line 44) `bool starts_with(const std::string &str, const std::string &prefix)`
  - `ends_with` (function, line 49) `bool ends_with(const std::string &str, const std::string &suffix)`
  - `append_path_component` (function, line 63) `std::string append_path_component(const std::string &path,
                                  cons...`
  - `to_lowercase` (function, line 86) `std::string to_lowercase(const std::string &str)`
  - `bool_from_string` (function, line 92) `bool bool_from_string(const char *input)`
  - `bool_from_string` (function, line 99) `bool bool_from_string(const std::string &input)`
  - `float_from_string` (function, line 109) `float float_from_string(const char *input)`
  - `float_from_string` (function, line 116) `float float_from_string(const std::string &input)`
  - `int32_from_string` (function, line 127) `int32_t int32_from_string(const char *input)`
  - `int32_from_string` (function, line 134) `int32_t int32_from_string(const std::string &input)`
  - `size_t_from_string` (function, line 145) `size_t size_t_from_string(const char *input)`
  - `size_t_from_string` (function, line 152) `size_t size_t_from_string(const std::string &input)`
- Depends on: `core/moonshine-utils/string-utils.h`

## core/moonshine-utils/string-utils.h
- Layer: utility
- Language: h
- Symbols:
  - `starts_with` (function, line 17) `bool starts_with(const std::string &str, const std::string &prefix);`
  - `ends_with` (function, line 19) `bool ends_with(const std::string &str, const std::string &suffix);`
  - `bool_from_string` (function, line 29) `bool bool_from_string(const std::string &input);`
  - `float_from_string` (function, line 32) `float float_from_string(const std::string &input);`
  - `int32_from_string` (function, line 35) `int32_t int32_from_string(const std::string &input);`
  - `size_t_from_string` (function, line 38) `size_t size_t_from_string(const std::string &input);`
  - `STRING_UTILS_H` (macro, line 2) `#define STRING_UTILS_H`
- Imported by: `core/bin-tokenizer/bin-tokenizer.cpp`, `core/gemma-embedding-model.cpp`, `core/moonshine-c-api-test.cpp`, `core/moonshine-c-api.cpp`, `core/moonshine-model.cpp`, `core/moonshine-streaming-model.cpp`, `core/moonshine-tts/src/moonshine-g2p-options.cpp`, `core/moonshine-tts/src/moonshine-tts-options.cpp`, `core/moonshine-tts/src/moonshine-tts.cpp`, `core/moonshine-utils/string-utils-test.cpp`, `core/moonshine-utils/string-utils.cpp`, `core/reliability/fuzz-string-utils.cpp`

## core/moonshine-utils/test-utils.h
- Layer: testing
- Language: h
- Symbols:
  - `MOONSHINE_TEST_UTILS_H` (macro, line 2) `#define MOONSHINE_TEST_UTILS_H`
  - `REQUIRE_FILE_EXISTS` (macro, line 8) `#define REQUIRE_FILE_EXISTS(filename)`
- Depends on: `core/moonshine-utils/debug-utils.h`
