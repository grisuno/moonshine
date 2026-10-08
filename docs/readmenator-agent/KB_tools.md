# Subsystem: tools

## core/moonshine-tts/tools/arabic-rule-g2p-cli.cpp
- Doc: MSA Arabic ONNX + rule G2P (mirrors ``arabic_rule_g2p.py`` CLI subset).
- Layer: business_logic
- Language: cpp
- Symbols:
  - `usage` (function, line 12) `void usage(const char* argv0)`
  - `read_all_stdin` (function, line 19) `std::string read_all_stdin()`
  - `main` (function, line 27) `int main(int argc, char** argv)`
- Depends on: `core/moonshine-tts/src/lang-specific/arabic.h`

## core/moonshine-tts/tools/chinese-rule-g2p-cli.cpp
- Doc: Simplified Chinese ONNX segmentation + UPOS + lexicon G2P (mirrors ``chinese_rule_g2p.py`` CLI).
- Layer: business_logic
- Language: cpp
- Symbols:
  - `usage` (function, line 13) `void usage(const char* argv0)`
  - `read_all_stdin` (function, line 20) `std::string read_all_stdin()`
  - `main` (function, line 28) `int main(int argc, char** argv)`
- Depends on: `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h`

## core/moonshine-tts/tools/dutch-g2p-batch-cli.cpp
- Doc: Dutch rule + lexicon G2P (no ONNX).
- Layer: utility
- Language: cpp
- Symbols:
  - `usage` (function, line 15) `void usage(const char* argv0)`
  - `trim_sv` (function, line 30) `std::string trim_sv(std::string s)`
  - `read_all_stdin` (function, line 42) `std::string read_all_stdin()`
  - `main` (function, line 50) `int main(int argc, char** argv)`
- Depends on: `core/moonshine-tts/src/lang-specific/dutch.h`

## core/moonshine-tts/tools/dutch-rule-g2p-cli.cpp
- Doc: Stand-alone Dutch rule + lexicon G2P (no ONNX).
- Layer: business_logic
- Language: cpp
- Symbols:
  - `usage` (function, line 13) `void usage(const char* argv0)`
  - `read_all_stdin` (function, line 22) `std::string read_all_stdin()`
  - `main` (function, line 30) `int main(int argc, char** argv)`
- Depends on: `core/moonshine-tts/src/lang-specific/dutch.h`

## core/moonshine-tts/tools/french-g2p-batch-cli.cpp
- Doc: French rule + lexicon G2P (no ONNX).
- Layer: utility
- Language: cpp
- Symbols:
  - `usage` (function, line 15) `void usage(const char* argv0)`
  - `trim_sv` (function, line 31) `std::string trim_sv(std::string s)`
  - `read_all_stdin` (function, line 43) `std::string read_all_stdin()`
  - `main` (function, line 51) `int main(int argc, char** argv)`
- Depends on: `core/moonshine-tts/src/lang-specific/french.h`

## core/moonshine-tts/tools/german-rule-g2p-cli.cpp
- Doc: Stand-alone German rule + lexicon G2P (no ONNX).
- Layer: business_logic
- Language: cpp
- Symbols:
  - `usage` (function, line 13) `void usage(const char* argv0)`
  - `read_all_stdin` (function, line 21) `std::string read_all_stdin()`
  - `main` (function, line 29) `int main(int argc, char** argv)`
- Depends on: `core/moonshine-tts/src/lang-specific/german.h`

## core/moonshine-tts/tools/hindi-rule-g2p-cli.cpp
- Doc: Hindi rule + lexicon G2P (no ONNX).
- Layer: business_logic
- Language: cpp
- Symbols:
  - `usage` (function, line 12) `void usage(const char* argv0)`
  - `read_all_stdin` (function, line 20) `std::string read_all_stdin()`
  - `main` (function, line 28) `int main(int argc, char** argv)`
- Depends on: `core/moonshine-tts/src/lang-specific/hindi.h`

## core/moonshine-tts/tools/italian-rule-g2p-cli.cpp
- Doc: Stand-alone Italian rule + lexicon G2P (no ONNX).
- Layer: business_logic
- Language: cpp
- Symbols:
  - `usage` (function, line 13) `void usage(const char* argv0)`
  - `read_all_stdin` (function, line 22) `std::string read_all_stdin()`
  - `main` (function, line 30) `int main(int argc, char** argv)`
- Depends on: `core/moonshine-tts/src/lang-specific/italian.h`

## core/moonshine-tts/tools/japanese-onnx-g2p-cli.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `usage` (function, line 11) `void usage(const char* argv0)`
  - `read_all_stdin` (function, line 16) `std::string read_all_stdin()`
  - `main` (function, line 24) `int main(int argc, char** argv)`
- Depends on: `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.h`

## core/moonshine-tts/tools/korean-rule-g2p-cli.cpp
- Doc: Korean rule + lexicon G2P (no ONNX).
- Layer: business_logic
- Language: cpp
- Symbols:
  - `usage` (function, line 13) `void usage(const char* argv0)`
  - `read_all_stdin` (function, line 20) `std::string read_all_stdin()`
  - `main` (function, line 28) `int main(int argc, char** argv)`
- Depends on: `core/moonshine-tts/src/lang-specific/korean.h`

## core/moonshine-tts/tools/moonshine-g2p-cli.cpp
- Doc: Unified G2P CLI: rule-based dialects (English, Spanish, German, …).
- Layer: utility
- Language: cpp
- Symbols:
  - `usage` (function, line 24) `void usage(const char *argv0)`
  - `read_all_stdin` (function, line 102) `std::string read_all_stdin()`
  - `rule_based_kind_label` (function, line 108) `const char *rule_based_kind_label(RuleBasedG2pKind k)`
  - `print_rule_based_dialect_catalog` (function, line 147) `void print_rule_based_dialect_catalog(std::ostream &os)`
  - `main` (function, line 160) `int main(int argc, char **argv)`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/spanish.h`, `core/moonshine-tts/src/moonshine-g2p.h`

## core/moonshine-tts/tools/moonshine-tts-cli.cpp
- Doc: CLI: Moonshine G2P + Kokoro or Piper ONNX → WAV (via MoonshineTTS).
- Layer: utility
- Language: cpp
- Symbols:
  - `usage` (function, line 15) `void usage(const char* argv0)`
  - `infer_lang_from_text_utf8` (function, line 59) `std::optional<std::string> infer_lang_from_text_utf8(const std::string& text)`
  - `main` (function, line 85) `int main(int argc, char** argv)`
- Depends on: `core/moonshine-tts/src/moonshine-tts.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/tools/piper-ipa-normalize-cli.cpp
- Doc: Prints Piper-ready IPA (NFC + replacements + optional inventory coercion) for parity tests.
- Layer: utility
- Language: cpp
- Symbols:
  - `print_usage` (function, line 17) `void print_usage()`
  - `load_keys` (function, line 22) `bool load_keys(const std::string& path, std::unordered_set<std::string>& keys)`
  - `main` (function, line 42) `int main(int argc, char** argv)`
- Depends on: `core/moonshine-tts/src/ipa-postprocess.h`

## core/moonshine-tts/tools/piper-phoneme-infer-cli.cpp
- Doc: Dev / CI: Piper ONNX from a JSON list of int64 phoneme ids (parity with ``speak.py`` ORT path).
- Layer: utility
- Language: cpp
- Symbols:
  - `usage` (function, line 18) `void usage(const char* argv0)`
  - `main` (function, line 34) `int main(int argc, char** argv)`
- Depends on: `core/moonshine-tts/src/moonshine-tts.h`, `core/moonshine-tts/src/piper-tts.h`

## core/moonshine-tts/tools/portuguese-rule-g2p-cli.cpp
- Doc: Stand-alone Portuguese rule + lexicon G2P (no ONNX).
- Layer: business_logic
- Language: cpp
- Symbols:
  - `usage` (function, line 13) `void usage(const char* argv0)`
  - `read_all_stdin` (function, line 22) `std::string read_all_stdin()`
  - `main` (function, line 30) `int main(int argc, char** argv)`
- Depends on: `core/moonshine-tts/src/lang-specific/portuguese.h`

## core/moonshine-tts/tools/vietnamese-rule-g2p-cli.cpp
- Doc: Vietnamese rule + lexicon G2P.
- Layer: business_logic
- Language: cpp
- Symbols:
  - `usage` (function, line 12) `void usage(const char* argv0)`
  - `read_all_stdin` (function, line 18) `std::string read_all_stdin()`
  - `main` (function, line 26) `int main(int argc, char** argv)`
- Depends on: `core/moonshine-tts/src/lang-specific/vietnamese.h`
