# Subsystem: moonshine-utils

## core/moonshine-utils/debug-utils-test.cpp
- Layer: testing
- Doc: include "debug-utils.h"  include <cstdio> include <filesystem>  define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN include <docte
- Language: cpp
- Symbols:
  - `return_on_error_test` (function, line 10) `int return_on_error_test()`
  - `return_on_false_test` (function, line 14) `int return_on_false_test()`
  - `return_on_null_test` (function, line 19) `int return_on_null_test()`
  - `return_on_not_equal_test` (function, line 24) `int return_on_not_equal_test()`
  - `TEST_CASE` (function, line 30) `TEST_CASE("debug-utils")`
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
  - `RETURN_ON_ERROR` (function, line 11) `RETURN_ON_ERROR(1);`
  - `RETURN_ON_FALSE` (function, line 16) `RETURN_ON_FALSE(false);`
  - `RETURN_ON_NULL` (function, line 21) `RETURN_ON_NULL(nullptr);`
  - `RETURN_ON_NOT_EQUAL` (function, line 26) `RETURN_ON_NOT_EQUAL(1, 2);`
  - `LOG` (function, line 33) `LOG("Hello, world!");`
  - `CHECK` (function, line 34) `CHECK(true);`
  - `TIMER_START` (function, line 41) `TIMER_START(my_timer);`
  - `TIMER_END` (function, line 42) `TIMER_END(my_timer);`
  - `DEBUG_FREE` (function, line 48) `DEBUG_FREE(ptr);`
  - `TRACE` (function, line 52) `TRACE();`
  - `LOG_INT` (function, line 56) `LOG_INT(1);`
  - `LOG_INT64` (function, line 57) `LOG_INT64((int64_t)(1));`
  - `LOG_LONG` (function, line 58) `LOG_LONG((long)(1));`
  - `LOG_SIZET` (function, line 59) `LOG_SIZET((size_t)(1));`
  - `LOG_PTR` (function, line 60) `LOG_PTR(nullptr);`
  - `LOG_VECTOR` (function, line 62) `LOG_VECTOR(vector);`
  - `LOG_FLOAT` (function, line 63) `LOG_FLOAT(1.0f);`
  - `LOG_STRING` (function, line 66) `LOG_STRING(std::string("Hello, world!"));`
  - `LOG_BOOL` (function, line 69) `LOG_BOOL(true);`
  - `LOG_BYTES` (function, line 73) `LOG_BYTES(bytes.c_str(), bytes.size());`
  - `fwrite` (function, line 79) `std::fwrite(file_contents.c_str(), 1, file_contents.size(), file);`
  - `fclose` (function, line 80) `std::fclose(file);`
  - `remove` (function, line 85) `std::remove("test.txt");`
  - `save_memory_to_file` (function, line 89) `save_memory_to_file("test.bin", data);`
  - `REQUIRE` (function, line 90) `REQUIRE(std::filesystem::exists("test.bin"));`
  - `read_data` (function, line 93) `std::vector<uint8_t> read_data(data.size());`
  - `free` (function, line 112) `free(audio_data);`
  - `create_directory` (function, line 130) `std::filesystem::create_directory("output");`
  - `LOGF` (function, line 153) `LOGF("audio_data[%zu] = %f, read_audio_data[%zu] = %f", i, audio_data[i], i, read_audio_data[i]);`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 5) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-utils/debug-utils.h`

## core/moonshine-utils/debug-utils.cpp
- Layer: utility
- Doc: include "debug-utils.h"  include <fcntl.h>  include <algorithm> include <cmath> include <cstdio> include <cstring> inclu
- Language: cpp
- Symbols:
  - `log_backtrace` (function, line 15) `void log_backtrace()`
  - `load_wav_data` (function, line 51) `bool load_wav_data(const char *path, float **out_float_data,
                   size_t *out_num_s...`
  - `save_wav_data` (function, line 196) `bool save_wav_data(const char *path, const float *audio_data,
                   size_t num_sampl...`
  - `float_vector_stats_to_string` (function, line 249) `std::string float_vector_stats_to_string(const std::vector<float> &vector)`
  - `load_file_into_memory` (function, line 268) `std::vector<uint8_t> load_file_into_memory(const std::string &path)`
  - `save_memory_to_file` (function, line 289) `void save_memory_to_file(const std::string &path,
                         const std::vector<uint...`
  - `LOGF` (function, line 23) `LOGF("Backtrace (%d frames):", frames);`
  - `symbol_str` (function, line 27) `std::string symbol_str(symbols[i]);`
  - `__cxa_demangle` (function, line 36) `abi::__cxa_demangle(mangled_name.c_str(), nullptr, nullptr, &status);`
  - `free` (function, line 40) `std::free(demangled_name);`
  - `perror` (function, line 60) `std::perror("Failed to open WAV file");`
  - `fclose` (function, line 68) `std::fclose(file);`
  - `fprintf` (function, line 69) `std::fprintf(stderr, "Not a RIFF file\n");`
  - `fseek` (function, line 74) `std::fseek(file, 4, SEEK_CUR);`
  - `audio_int16` (function, line 204) `std::vector<int16_t> audio_int16(num_samples);`
  - `fwrite` (function, line 213) `std::fwrite(riff_header, 1, 4, file);`
  - `accumulate` (function, line 258) `std::accumulate(vector.begin(), vector.end(), 0.0f) / vector.size();`
  - `THROW_WITH_LOG` (function, line 272) `THROW_WITH_LOG(("Failed to open file: '" + path + "'").c_str());`
  - `data` (function, line 277) `std::vector<uint8_t> data(size);`
- Depends on: `core/moonshine-utils/debug-utils.h`

## core/moonshine-utils/debug-utils.h
- Layer: utility
- Doc: ifndef UTILS_H define UTILS_H  include <cinttypes> include <cstring> include <sstream> include <string> include <thread>
- Language: h
- Symbols:
  - `_moonshine_filename_without_path` (function, line 14) `static inline const char *_moonshine_filename_without_path(const char *path)`
  - `debug_calloc` (function, line 139) `debug_calloc(size, count, FILENAME_ONLY, __LINE__, __FUNCTION__)

static inline void *debug_callo...`
  - `debug_free` (function, line 155) `static inline void debug_free(void *voidMemPtr, const char *file, int line,
                     ...`
  - `debug_alloc_get_size` (function, line 175) `static inline size_t debug_alloc_get_size(void *voidMemPtr)`
  - `gate` (function, line 266) `template <typename T>
T gate(T value, T min, T max)`
  - `__android_log_print` (function, line 29) `__android_log_print(ANDROID_LOG_WARN, "Native", "%s:%d:%s(): " format, \ FILENAME_ONLY, __LINE__, __func__, __VA_ARGS__);`
  - `get_id` (function, line 36) `oss << std::this_thread::get_id();`
  - `fprintf` (function, line 38) `fprintf(stderr, "Thread %s:%s:%d:%s(): " format, thread_id_str.c_str(), \ FILENAME_ONLY, __LINE__, __func__, __VA_ARGS__);`
  - `LOG` (function, line 47) `LOG(x);`
  - `LOGF` (function, line 52) `LOGF(format, __VA_ARGS__);`
  - `TIMER_END` (function, line 116) `TIMER_END(x);`
  - `free` (function, line 173) `free(sizePtr);`
  - `runtime_error` (function, line 208) `throw std::runtime_error( \ std::string(FILENAME_ONLY) + ":" + std::to_string(__LINE__) + ":" + \ std::string(__func__) + " - " + std::string(message));`
  - `snprintf` (function, line 244) `snprintf(buffer, 4, "%02x ", (unsigned char)(((x))[i]));`
  - `log_backtrace` (function, line 252) `void log_backtrace();`
  - `load_wav_data` (function, line 254) `bool load_wav_data(const char *path, float **out_float_data, size_t *out_num_samples, int32_t *out_sample_rate = nullptr);`
  - `save_wav_data` (function, line 257) `bool save_wav_data(const char *path, const float *audio_data, size_t num_samples, uint32_t sample_rate = 16000);`
  - `float_vector_stats_to_string` (function, line 260) `std::string float_vector_stats_to_string(const std::vector<float> &vector);`
  - `load_file_into_memory` (function, line 262) `std::vector<uint8_t> load_file_into_memory(const std::string &path);`
  - `save_memory_to_file` (function, line 264) `void save_memory_to_file(const std::string &path, const std::vector<uint8_t> &data);`
  - `UTILS_H` (macro, line 2) `#define UTILS_H`
  - `FILENAME_ONLY` (macro, line 22) `#define FILENAME_ONLY`
  - `LOGF` (macro, line 27) `#define LOGF(format, ...)`
  - `LOGF` (macro, line 33) `#define LOGF(format, ...)`
  - `LOG` (macro, line 43) `#define LOG(x)`
  - `LOG_IF` (macro, line 44) `#define LOG_IF(condition, x)`
  - `LOGF_IF` (macro, line 49) `#define LOGF_IF(condition, format, ...)`
  - `RETURN_ON_ERROR` (macro, line 54) `#define RETURN_ON_ERROR(error)`
  - `RETURN_ON_FALSE` (macro, line 62) `#define RETURN_ON_FALSE(expr)`
  - `RETURN_ON_NULL` (macro, line 70) `#define RETURN_ON_NULL(ptr)`
  - `RETURN_ON_NOT_EQUAL` (macro, line 78) `#define RETURN_ON_NOT_EQUAL(expr1, expr2)`
  - `RETURN_ON_FILE_DOES_NOT_EXIST` (macro, line 86) `#define RETURN_ON_FILE_DOES_NOT_EXIST(path)`
  - `ENABLE_TIMER` (macro, line 94) `#define ENABLE_TIMER`
  - `TIMER_START` (macro, line 99) `#define TIMER_START(x)`
  - `TIMER_END` (macro, line 101) `#define TIMER_END(x)`
  - `TIMER_START_IF` (macro, line 111) `#define TIMER_START_IF(condition, x)`
  - `TIMER_END_IF` (macro, line 113) `#define TIMER_END_IF(condition, x)`
  - `TIMER_START` (macro, line 119) `#define TIMER_START(x)`
  - `TIMER_END` (macro, line 120) `#define TIMER_END(x)`
  - `TIMER_START_IF` (macro, line 121) `#define TIMER_START_IF(condition, x)`
  - `TIMER_END_IF` (macro, line 122) `#define TIMER_END_IF(condition, x)`
  - `DEBUG_ALLOC_MAGIC` (macro, line 131) `#define DEBUG_ALLOC_MAGIC`
  - `DEBUG_ALLOC_ALIGNMENT` (macro, line 133) `#define DEBUG_ALLOC_ALIGNMENT`
  - `DEBUG_ALLOC_LOG_MIN_SIZE` (macro, line 135) `#define DEBUG_ALLOC_LOG_MIN_SIZE`
  - `DEBUG_CALLOC` (macro, line 137) `#define DEBUG_CALLOC(size, count)`
  - `DEBUG_FREE` (macro, line 153) `#define DEBUG_FREE(ptr)`
  - `DEBUG_CALLOC` (macro, line 194) `#define DEBUG_CALLOC(size, count)`
  - `DEBUG_FREE` (macro, line 196) `#define DEBUG_FREE(ptr)`
  - `TRACE` (macro, line 199) `#define TRACE()`
  - `THROW_WITH_LOG` (macro, line 204) `#define THROW_WITH_LOG(message)`
  - `LOG_INT` (macro, line 212) `#define LOG_INT(x)`
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
  - `LOG_STRUCT_BYTES` (macro, line 250) `#define LOG_STRUCT_BYTES(x)`
- Imported by: `core/bin-tokenizer/bin-tokenizer-test.cpp`, `core/bin-tokenizer/bin-tokenizer.cpp`, `core/gemma-embedding-model.cpp`, `core/moonshine-c-api-test.cpp`, `core/moonshine-c-api.cpp`, `core/moonshine-download-smoke.cpp`, `core/moonshine-model.cpp`, `core/moonshine-streaming-model.cpp`, `core/moonshine-tts/src/lang-specific/korean.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/moonshine-tts.cpp`, `core/moonshine-tts/src/piper-tts.cpp`, `core/moonshine-tts/src/zipvoice-tts.cpp`, `core/moonshine-utils/debug-utils-test.cpp`, `core/moonshine-utils/debug-utils.cpp`, `core/moonshine-utils/file-utils.cpp`, `core/moonshine-utils/test-utils.h`, `core/ort-utils/moonshine-ort-allocator.cpp`, `core/ort-utils/moonshine-tensor-view.cpp`, `core/ort-utils/moonshine-tensor.cpp`, `core/ort-utils/ort-utils.h`, `core/reliability/fuzz-wav-pcm.cpp`, `core/resampler-test.cpp`, `core/resampler.cpp`, `core/speaker-diarizer.cpp`, `core/spelling-model-test.cpp`, `core/spelling-model.cpp`, `core/voice-activity-detector-test.cpp`, `core/voice-activity-detector.cpp`, `core/word-alignment-test.cpp`

## core/moonshine-utils/file-utils-test.cpp
- Layer: testing
- Doc: include "file-utils.h"  include <cstdint> include <cstdio> include <cstring> include <stdexcept> include <vector>  defin
- Language: cpp
- Symbols:
  - `write_file` (function, line 14) `void write_file(const char *path, const std::vector<uint8_t> &bytes)`
  - `TEST_CASE` (function, line 24) `TEST_CASE("fread_exact")`
  - `SUBCASE` (function, line 27) `SUBCASE("reads the full requested amount")`
  - `SUBCASE` (function, line 41) `SUBCASE("reads multi-byte elements and preserves values")`
  - `SUBCASE` (function, line 58) `SUBCASE("throws when fewer elements are available than requested")`
  - `SUBCASE` (function, line 71) `SUBCASE("throws on a partial trailing element")`
  - `SUBCASE` (function, line 84) `SUBCASE("throws when reading past end of file")`
  - `SUBCASE` (function, line 99) `SUBCASE("zero count is a no-op that returns count")`
  - `SUBCASE` (function, line 108) `SUBCASE("zero size is a no-op that returns count")`
  - `REQUIRE` (function, line 16) `REQUIRE(file != nullptr);`
  - `fclose` (function, line 21) `std::fclose(file);`
  - `buffer` (function, line 33) `std::vector<uint8_t> buffer(contents.size());`
  - `fread_exact` (function, line 36) `fread_exact(buffer.data(), 1, buffer.size(), file, "byte buffer");`
  - `CHECK` (function, line 37) `CHECK(count == contents.size());`
  - `contents` (function, line 44) `std::vector<uint8_t> contents(sizeof(values));`
  - `memcpy` (function, line 45) `std::memcpy(contents.data(), values, sizeof(values));`
  - `CHECK_THROWS_AS` (function, line 66) `CHECK_THROWS_AS( fread_exact(buffer.data(), 1, buffer.size(), file, "byte buffer"), std::runtime_error);`
  - `remove` (function, line 117) `std::remove(path);`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 8) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-utils/file-utils.h`

## core/moonshine-utils/file-utils.cpp
- Layer: utility
- Doc: include "file-utils.h"  include <cstdio> include <sstream> include <stdexcept> include <string>  include "debug-utils.h"
- Language: cpp
- Symbols:
  - `fread_exact` (function, line 9) `std::size_t fread_exact(void *ptr, std::size_t size, std::size_t count,
                        s...`
  - `THROW_WITH_LOG` (function, line 26) `THROW_WITH_LOG(message.c_str());`
- Depends on: `core/moonshine-utils/debug-utils.h`, `core/moonshine-utils/file-utils.h`

## core/moonshine-utils/file-utils.h
- Layer: utility
- Doc: ifndef FILE_UTILS_H define FILE_UTILS_H  include <cstddef> include <cstdio>  Wrapper around std::fread that throws std::
- Language: h
- Symbols:
  - `fread_exact` (function, line 12) `std::size_t fread_exact(void *ptr, std::size_t size, std::size_t count, std::FILE *stream, const char *what = "file");`
  - `FILE_UTILS_H` (macro, line 2) `#define FILE_UTILS_H`
- Imported by: `core/benchmark.cpp`, `core/bin-tokenizer/bin-tokenizer.cpp`, `core/moonshine-utils/file-utils-test.cpp`, `core/moonshine-utils/file-utils.cpp`, `core/word-alignment-benchmark.cpp`

## core/moonshine-utils/string-utils-test.cpp
- Layer: testing
- Doc: include "string-utils.h"  include <cstdio>  define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN include <doctest.h>
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 7) `TEST_CASE("string-utils")`
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
  - `CHECK` (function, line 10) `CHECK(replace_all("hello world", "world", "hello") == "hello hello");`
  - `CHECK_THROWS` (function, line 47) `CHECK_THROWS(bool_from_string("invalid"));`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 4) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-utils/string-utils.h`

## core/moonshine-utils/string-utils.cpp
- Layer: utility
- Doc: include "string-utils.h"  include <algorithm> include <cstdio> include <stdexcept>  See https://stackoverflow.com/questi
- Language: cpp
- Symbols:
  - `replace_all` (function, line 9) `std::string replace_all(std::string str, const std::string &from,
                        const s...`
  - `trim` (function, line 21) `std::string trim(const std::string &str, const std::string &whitespace)`
  - `split` (function, line 30) `std::vector<std::string> split(const std::string &str,
                               const std::...`
  - `starts_with` (function, line 43) `bool starts_with(const std::string &str, const std::string &prefix)`
  - `ends_with` (function, line 48) `bool ends_with(const std::string &str, const std::string &suffix)`
  - `append_path_component` (function, line 62) `std::string append_path_component(const std::string &path,
                                  cons...`
  - `to_lowercase` (function, line 85) `std::string to_lowercase(const std::string &str)`
  - `bool_from_string` (function, line 91) `bool bool_from_string(const char *input)`
  - `bool_from_string` (function, line 98) `bool bool_from_string(const std::string &input)`
  - `float_from_string` (function, line 108) `float float_from_string(const char *input)`
  - `float_from_string` (function, line 115) `float float_from_string(const std::string &input)`
  - `int32_from_string` (function, line 126) `int32_t int32_from_string(const char *input)`
  - `int32_from_string` (function, line 133) `int32_t int32_from_string(const std::string &input)`
  - `size_t_from_string` (function, line 144) `size_t size_t_from_string(const char *input)`
  - `size_t_from_string` (function, line 151) `size_t size_t_from_string(const std::string &input)`
  - `transform` (function, line 88) `std::transform(result.begin(), result.end(), result.begin(), ::tolower);`
  - `runtime_error` (function, line 94) `throw std::runtime_error("Invalid boolean string: nullptr");`
- Depends on: `core/moonshine-utils/string-utils.h`

## core/moonshine-utils/string-utils.h
- Layer: utility
- Doc: ifndef STRING_UTILS_H define STRING_UTILS_H  include <cstdint> include <map> include <string> include <vector>
- Language: h
- Symbols:
  - `replace_all` (function, line 8) `std::string replace_all(std::string str, const std::string &from, const std::string &to);`
  - `trim` (function, line 11) `std::string trim(const std::string &str, const std::string &whitespace = " \t");`
  - `split` (function, line 13) `std::vector<std::string> split(const std::string &str, const std::string &delimiter);`
  - `starts_with` (function, line 16) `bool starts_with(const std::string &str, const std::string &prefix);`
  - `ends_with` (function, line 18) `bool ends_with(const std::string &str, const std::string &suffix);`
  - `append_path_component` (function, line 23) `std::string append_path_component(const std::string &path, const std::string &component);`
  - `to_lowercase` (function, line 26) `std::string to_lowercase(const std::string &str);`
  - `bool_from_string` (function, line 28) `bool bool_from_string(const std::string &input);`
  - `float_from_string` (function, line 31) `float float_from_string(const std::string &input);`
  - `int32_from_string` (function, line 34) `int32_t int32_from_string(const std::string &input);`
  - `size_t_from_string` (function, line 37) `size_t size_t_from_string(const std::string &input);`
  - `STRING_UTILS_H` (macro, line 2) `#define STRING_UTILS_H`
- Imported by: `core/bin-tokenizer/bin-tokenizer.cpp`, `core/gemma-embedding-model.cpp`, `core/moonshine-c-api-test.cpp`, `core/moonshine-c-api.cpp`, `core/moonshine-model.cpp`, `core/moonshine-streaming-model.cpp`, `core/moonshine-tts/src/moonshine-g2p-options.cpp`, `core/moonshine-tts/src/moonshine-tts-options.cpp`, `core/moonshine-tts/src/moonshine-tts.cpp`, `core/moonshine-utils/string-utils-test.cpp`, `core/moonshine-utils/string-utils.cpp`, `core/reliability/fuzz-string-utils.cpp`

## core/moonshine-utils/test-utils.h
- Layer: testing
- Doc: ifndef MOONSHINE_TEST_UTILS_H define MOONSHINE_TEST_UTILS_H  include <filesystem>  include "debug-utils.h"  define REQUI
- Language: h
- Symbols:
  - `FAIL` (function, line 21) `FAIL(log_message);`
  - `MOONSHINE_TEST_UTILS_H` (macro, line 2) `#define MOONSHINE_TEST_UTILS_H`
  - `REQUIRE_FILE_EXISTS` (macro, line 7) `#define REQUIRE_FILE_EXISTS(filename)`
- Depends on: `core/moonshine-utils/debug-utils.h`
