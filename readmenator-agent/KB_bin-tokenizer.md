# Subsystem: bin-tokenizer

## core/bin-tokenizer/bin-tokenizer-test.cpp
- Layer: testing
- Doc: include "bin-tokenizer.h"  include <cstdio> include <filesystem>  include "debug-utils.h"  define DOCTEST_CONFIG_IMPLEME
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 10) `TEST_CASE("bin-tokenizer")`
  - `SUBCASE` (function, line 12) `SUBCASE("constructor-from-path")`
  - `SUBCASE` (function, line 26) `SUBCASE("constructor-from-data")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 7)

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

## core/bin-tokenizer/bin-tokenizer.h
- Layer: utility
- Doc: ifndef BIN_TOKENIZER_H define BIN_TOKENIZER_H  include <cstdint> include <string> include <vector>  if defined(ANDROID) 
- Language: h
- Symbols:
  - `BinTokenizer` (struct, line 12)
  - `BIN_TOKENIZER_H` (macro, line 2)
