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
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 5)

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
  - `UTILS_H` (macro, line 2)
  - `FILENAME_ONLY` (macro, line 22)
  - `LOGF` (macro, line 27)
  - `LOGF` (macro, line 33)
  - `LOG` (macro, line 43)
  - `LOG_IF` (macro, line 44)
  - `LOGF_IF` (macro, line 49)
  - `RETURN_ON_ERROR` (macro, line 54)
  - `RETURN_ON_FALSE` (macro, line 62)
  - `RETURN_ON_NULL` (macro, line 70)
  - `RETURN_ON_NOT_EQUAL` (macro, line 78)
  - `RETURN_ON_FILE_DOES_NOT_EXIST` (macro, line 86)
  - `ENABLE_TIMER` (macro, line 94)
  - `TIMER_START` (macro, line 99)
  - `TIMER_END` (macro, line 101)
  - `TIMER_START_IF` (macro, line 111)
  - `TIMER_END_IF` (macro, line 113)
  - `TIMER_START` (macro, line 119)
  - `TIMER_END` (macro, line 120)
  - `TIMER_START_IF` (macro, line 121)
  - `TIMER_END_IF` (macro, line 122)
  - `DEBUG_ALLOC_MAGIC` (macro, line 131)
  - `DEBUG_ALLOC_ALIGNMENT` (macro, line 133)
  - `DEBUG_ALLOC_LOG_MIN_SIZE` (macro, line 135)
  - `DEBUG_CALLOC` (macro, line 137)
  - `DEBUG_FREE` (macro, line 153)
  - `DEBUG_CALLOC` (macro, line 194)
  - `DEBUG_FREE` (macro, line 196)
  - `TRACE` (macro, line 199)
  - `THROW_WITH_LOG` (macro, line 204)
  - `LOG_INT` (macro, line 212)
  - `LOG_INT64` (macro, line 214)
  - `LOG_UINT64` (macro, line 215)
  - `LOG_LONG` (macro, line 216)
  - `LOG_SIZET` (macro, line 217)
  - `LOG_PTR` (macro, line 218)
  - `LOG_VECTOR` (macro, line 219)
  - `LOG_FLOAT` (macro, line 232)
  - `LOG_STRING` (macro, line 233)
  - `LOG_BOOL` (macro, line 234)
  - `LOG_BYTES` (macro, line 235)
  - `LOG_STRUCT_BYTES` (macro, line 250)

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
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 8)

## core/moonshine-utils/file-utils.cpp
- Layer: utility
- Doc: include "file-utils.h"  include <cstdio> include <sstream> include <stdexcept> include <string>  include "debug-utils.h"
- Language: cpp
- Symbols:
  - `fread_exact` (function, line 9) `std::size_t fread_exact(void *ptr, std::size_t size, std::size_t count,
                        s...`

## core/moonshine-utils/file-utils.h
- Layer: utility
- Doc: ifndef FILE_UTILS_H define FILE_UTILS_H  include <cstddef> include <cstdio>  Wrapper around std::fread that throws std::
- Language: h
- Symbols:
  - `FILE_UTILS_H` (macro, line 2)

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
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 4)

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

## core/moonshine-utils/string-utils.h
- Layer: utility
- Doc: ifndef STRING_UTILS_H define STRING_UTILS_H  include <cstdint> include <map> include <string> include <vector>
- Language: h
- Symbols:
  - `STRING_UTILS_H` (macro, line 2)

## core/moonshine-utils/test-utils.h
- Layer: testing
- Doc: ifndef MOONSHINE_TEST_UTILS_H define MOONSHINE_TEST_UTILS_H  include <filesystem>  include "debug-utils.h"  define REQUI
- Language: h
- Symbols:
  - `MOONSHINE_TEST_UTILS_H` (macro, line 2)
  - `REQUIRE_FILE_EXISTS` (macro, line 7)
