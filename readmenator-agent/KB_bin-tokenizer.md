# Subsystem: bin-tokenizer

## core/bin-tokenizer/bin-tokenizer-test.cpp
- Layer: testing
- Doc: include "bin-tokenizer.h"  include <cstdio> include <filesystem>  include "debug-utils.h"  define DOCTEST_CONFIG_IMPLEME
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 10) `TEST_CASE("bin-tokenizer")`
  - `SUBCASE` (function, line 12) `SUBCASE("constructor-from-path")`
  - `SUBCASE` (function, line 26) `SUBCASE("constructor-from-data")`
  - `save_memory_to_file` (function, line 14) `save_memory_to_file("tokenizer.bin", data);`
  - `REQUIRE` (function, line 15) `REQUIRE(std::filesystem::exists("tokenizer.bin"));`
  - `tokenizer` (function, line 16) `BinTokenizer tokenizer("tokenizer.bin");`
  - `CHECK` (function, line 18) `CHECK(tokenizer.tokens_to_bytes.size() == 3);`
  - `remove` (function, line 24) `std::remove("tokenizer.bin");`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 7) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/moonshine-utils/debug-utils.h`

## core/bin-tokenizer/bin-tokenizer.cpp
- Layer: utility
- Doc: include "bin-tokenizer.h"  include <cstdint> include <cstdlib> include <cstring> include <stdexcept>  include "debug-uti
- Language: cpp
- Symbols:
  - `BinTokenizer` (function, line 11) `BinTokenizer::BinTokenizer(const char *tokenizer_path,
                           const char *spa...`
  - `BinTokenizer` (function, line 49) `BinTokenizer::BinTokenizer(const uint8_t *tokenizer_data,
                           size_t token...`
  - `BinTokenizer` (function, line 106) `BinTokenizer::BinTokenizer(const char *tokenizer_path,
                           AAssetManager *...`
  - `text_to_special_token` (function, line 146) `template <typename T>
T BinTokenizer::text_to_special_token(const std::string &text)`
  - `text_to_tokens` (function, line 172) `template <typename T>
std::vector<T> BinTokenizer::text_to_tokens(const std::string &text)`
  - `tokens_to_text` (function, line 220) `template <typename T>
std::string BinTokenizer::tokens_to_text(const std::vector<T> &tokens,
    ...`
  - `perror` (function, line 19) `std::perror(message.c_str());`
  - `runtime_error` (function, line 20) `throw std::runtime_error(message);`
  - `fread_exact` (function, line 36) `fread_exact(&second_byte, 1, 1, file, "tokenizer length byte");`
  - `bytes` (function, line 39) `std::vector<uint8_t> bytes(byte_count);`
  - `fclose` (function, line 43) `std::fclose(file);`
  - `memcpy` (function, line 93) `std::memcpy(bytes.data(), tokenizer_data + offset, byte_count);`
  - `AAssetManager_open` (function, line 111) `AAssetManager_open(assetManager, tokenizer_path, AASSET_MODE_STREAMING);`
  - `fprintf` (function, line 113) `fprintf(stderr, "Failed to open asset %s at %s:%d\n", tokenizer_path, __FILE__, __LINE__);`
  - `AAsset_read` (function, line 132) `AAsset_read(asset, &second_byte, 1);`
  - `AAsset_close` (function, line 139) `AAsset_close(asset);`
  - `remaining_bytes` (function, line 176) `std::vector<uint8_t> remaining_bytes(replaced_spaces_text.begin(), replaced_spaces_text.end());`
  - `snprintf` (function, line 201) `snprintf(hex_byte, sizeof(hex_byte), "0x%02X", byte);`
  - `result` (function, line 237) `std::string result(result_bytes.begin(), result_bytes.end());`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/moonshine-utils/debug-utils.h`, `core/moonshine-utils/file-utils.h`, `core/moonshine-utils/string-utils.h`

## core/bin-tokenizer/bin-tokenizer.h
- Layer: utility
- Doc: ifndef BIN_TOKENIZER_H define BIN_TOKENIZER_H  include <cstdint> include <string> include <vector>  if defined(ANDROID) 
- Language: h
- Symbols:
  - `BinTokenizer` (struct, line 12)
  - `BinTokenizer` (function, line 15) `BinTokenizer(const char *tokenizer_path, const char *space_string = "▁");`
  - `text_to_tokens` (function, line 23) `template <typename T> std::vector<T> text_to_tokens(const std::string &text);`
  - `tokens_to_text` (function, line 25) `template <typename T> std::string tokens_to_text(const std::vector<T> &tokens, bool skipSpecials = true);`
  - `text_to_special_token` (function, line 28) `template <typename T> T text_to_special_token(const std::string &text);`
  - `BIN_TOKENIZER_H` (macro, line 2) `#define BIN_TOKENIZER_H`
- Imported by: `core/bin-tokenizer/bin-tokenizer-test.cpp`, `core/bin-tokenizer/bin-tokenizer.cpp`, `core/gemma-embedding-model.cpp`, `core/gemma-embedding-model.h`, `core/moonshine-c-api.cpp`, `core/moonshine-model.cpp`, `core/moonshine-model.h`, `core/moonshine-streaming-model.cpp`, `core/moonshine-streaming-model.h`, `core/reliability/fuzz-bin-tokenizer.cpp`, `core/word-alignment.h`
