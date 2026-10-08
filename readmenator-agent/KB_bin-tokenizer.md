# Subsystem: bin-tokenizer

## core/bin-tokenizer/bin-tokenizer-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 11) `TEST_CASE("bin-tokenizer")`
  - `SUBCASE` (function, line 12) `SUBCASE("constructor-from-path")`
  - `SUBCASE` (function, line 26) `SUBCASE("constructor-from-data")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 8) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/moonshine-utils/debug-utils.h`

## core/bin-tokenizer/bin-tokenizer.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `BinTokenizer` (function, line 12) `BinTokenizer::BinTokenizer(const char *tokenizer_path,
                           const char *spa...`
  - `BinTokenizer` (function, line 50) `BinTokenizer::BinTokenizer(const uint8_t *tokenizer_data,
                           size_t token...`
  - `BinTokenizer` (function, line 106) `BinTokenizer::BinTokenizer(const char *tokenizer_path,
                           AAssetManager *...`
  - `text_to_special_token` (function, line 148) `template <typename T>
T BinTokenizer::text_to_special_token(const std::string &text)`
  - `text_to_tokens` (function, line 173) `template <typename T>
std::vector<T> BinTokenizer::text_to_tokens(const std::string &text)`
  - `tokens_to_text` (function, line 222) `template <typename T>
std::string BinTokenizer::tokens_to_text(const std::vector<T> &tokens,
    ...`
  - `bytes` (function, line 39) `std::vector<uint8_t> bytes(byte_count);`
  - `remaining_bytes` (function, line 176) `std::vector<uint8_t> remaining_bytes(replaced_spaces_text.begin(), replaced_spaces_text.end());`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/moonshine-utils/debug-utils.h`, `core/moonshine-utils/file-utils.h`, `core/moonshine-utils/string-utils.h`

## core/bin-tokenizer/bin-tokenizer.h
- Layer: utility
- Language: h
- Symbols:
  - `BinTokenizer` (struct, line 12)
  - `BIN_TOKENIZER_H` (macro, line 2) `#define BIN_TOKENIZER_H`
- Imported by: `core/bin-tokenizer/bin-tokenizer-test.cpp`, `core/bin-tokenizer/bin-tokenizer.cpp`, `core/gemma-embedding-model.cpp`, `core/gemma-embedding-model.h`, `core/moonshine-c-api.cpp`, `core/moonshine-model.cpp`, `core/moonshine-model.h`, `core/moonshine-streaming-model.cpp`, `core/moonshine-streaming-model.h`, `core/reliability/fuzz-bin-tokenizer.cpp`, `core/word-alignment.h`
