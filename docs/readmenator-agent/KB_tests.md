# Subsystem: tests

## core/moonshine-tts/tests/arabic-rule-g2p-test.cpp
- Layer: business_logic
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 9) `TEST_CASE(
    "arabic rule g2p: first 100 wiki lines match reference IPA when assets and "
    "...`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/lang-specific/arabic.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`

## core/moonshine-tts/tests/chinese-rule-g2p-test.cpp
- Layer: business_logic
- Language: cpp
- Symbols:
  - `make_temp_tsv` (function, line 21) `std::filesystem::path make_temp_tsv(const char* contents)`
  - `TEST_CASE` (function, line 33) `TEST_CASE("chinese: dialect_resolves_to_chinese_rules")`
  - `TEST_CASE` (function, line 44) `TEST_CASE(
    "chinese: lexicon lookup and Arabic numeral expansion via per-char Han "
    "IPA")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h`, `core/moonshine-tts/src/lang-specific/chinese.h`, `core/moonshine-tts/src/moonshine-g2p.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`

## core/moonshine-tts/tests/chinese-tok-pos-onnx-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 10) `TEST_CASE("chinese tok pos: single sentence matches reference file")`
  - `TEST_CASE` (function, line 27) `TEST_CASE(
    "chinese tok pos: first 100 wiki lines match reference when assets and "
    "gold...`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`

## core/moonshine-tts/tests/cmudict-tsv-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 11) `TEST_CASE("cmudict-tsv load and lookup")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/lang-specific/cmudict-tsv.h`

## core/moonshine-tts/tests/dutch-rule-g2p-test.cpp
- Layer: business_logic
- Language: cpp
- Symbols:
  - `make_temp_tsv` (function, line 17) `std::filesystem::path make_temp_tsv(const char* contents)`
  - `TEST_CASE` (function, line 29) `TEST_CASE("dutch: lowercase homograph overrides capitalized")`
  - `TEST_CASE` (function, line 38) `TEST_CASE(
    "dutch: lexicon stress not shifted by vocoder (unlike German policy)")`
  - `TEST_CASE` (function, line 50) `TEST_CASE("dutch: rule IPA gets vocoder stress when enabled")`
  - `TEST_CASE` (function, line 59) `TEST_CASE("dutch: normalize_ipa_stress_for_vocoder idempotent")`
  - `TEST_CASE` (function, line 70) `TEST_CASE("dutch: dialect_resolves_to_dutch_rules")`
  - `TEST_CASE` (function, line 79) `TEST_CASE("dutch: optional real dict fiets matches Python when data present")`
  - `TEST_CASE` (function, line 93) `TEST_CASE(
    "dutch: wiki-text first 100 lines match reference IPA when data and golden "
    "...`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/lang-specific/dutch.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`

## core/moonshine-tts/tests/english-hand-oov-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 13) `TEST_CASE("english_number_token_ipa")`
  - `TEST_CASE` (function, line 20) `TEST_CASE("english_hand_oov_rules_ipa nonempty")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/lang-specific/english-hand-oov.h`, `core/moonshine-tts/src/lang-specific/english-numbers.h`

## core/moonshine-tts/tests/english-rule-g2p-test.cpp
- Layer: business_logic
- Language: cpp
- Symbols:
  - `resolve_en_dict` (function, line 15) `std::filesystem::path resolve_en_dict()`
  - `TEST_CASE` (function, line 22) `TEST_CASE("english: dialect_resolves_to_english_rules")`
  - `TEST_CASE` (function, line 38) `TEST_CASE("english: tomato heteronym picks US vs British by dialect flag")`
  - `TEST_CASE` (function, line 51) `TEST_CASE(
    "english: wiki-text first 100 lines match reference IPA when data and "
    "golde...`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/lang-specific/english.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`

## core/moonshine-tts/tests/file-information-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 11) `TEST_CASE("FileInformation default memory fields")`
  - `TEST_CASE` (function, line 18) `TEST_CASE("FileInformationMap set_path and contains")`
  - `TEST_CASE` (function, line 28) `TEST_CASE("FileInformationMap erase_key")`
  - `TEST_CASE` (function, line 35) `TEST_CASE("FileInformationMap::parse_file_list")`
  - `TEST_CASE` (function, line 60) `TEST_CASE("FileInformationMap::parse_file_list null key_list throws")`
  - `TEST_CASE` (function, line 66) `TEST_CASE("FileInformationMap::parse_file_list memory size mismatch throws")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/file-information.h`

## core/moonshine-tts/tests/french-rule-g2p-test.cpp
- Layer: business_logic
- Language: cpp
- Symbols:
  - `strip_stress` (function, line 16) `std::string strip_stress(std::string s)`
  - `french_dict_present` (function, line 36) `bool french_dict_present()`
  - `TEST_CASE` (function, line 43) `TEST_CASE("french: dialect_resolves_to_french_rules")`
  - `TEST_CASE` (function, line 52) `TEST_CASE("french: ensure_french_nuclear_stress")`
  - `TEST_CASE` (function, line 58) `TEST_CASE("french: liaison les amis" * doctest::skip(!french_dict_present()))`
  - `TEST_CASE` (function, line 70) `TEST_CASE("french: En 1891 cardinal expansion" *
          doctest::skip(!french_dict_present()))`
  - `TEST_CASE` (function, line 83) `TEST_CASE("french: punctuation keeps space before next word" *
          doctest::skip(!french_di...`
  - `TEST_CASE` (function, line 94) `TEST_CASE(
    "french: hyphenated OOV allez-vous matches Python (UTF-8 trim + stress)" *
    doc...`
  - `TEST_CASE` (function, line 105) `TEST_CASE("french: uppercase accented letters in words (Saint-Étienne)" *
          doctest::skip...`
  - `TEST_CASE` (function, line 115) `TEST_CASE(
    "french: wiki-text first 100 lines match reference IPA when data and "
    "golden...`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/lang-specific/french.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`

## core/moonshine-tts/tests/german-rule-g2p-test.cpp
- Layer: business_logic
- Language: cpp
- Symbols:
  - `make_temp_tsv` (function, line 17) `std::filesystem::path make_temp_tsv(const char* contents)`
  - `TEST_CASE` (function, line 29) `TEST_CASE("german: lowercase homograph overrides capitalized")`
  - `TEST_CASE` (function, line 38) `TEST_CASE(
    "german: lexicon entry with syllable-initial stress gets vocoder shift")`
  - `TEST_CASE` (function, line 46) `TEST_CASE(
    "german: syllable-initial stress preserved when vocoder_stress false")`
  - `TEST_CASE` (function, line 56) `TEST_CASE("german: OOV rules machen")`
  - `TEST_CASE` (function, line 68) `TEST_CASE("german: normalize_ipa_stress_for_vocoder idempotent")`
  - `TEST_CASE` (function, line 76) `TEST_CASE("german: dialect_resolves_to_german_rules")`
  - `TEST_CASE` (function, line 85) `TEST_CASE("german: text token preserves comma")`
  - `TEST_CASE` (function, line 93) `TEST_CASE(
    "german: Im Jahr 1891 matches reference IPA when data and golden exist")`
  - `TEST_CASE` (function, line 109) `TEST_CASE(
    "german: wiki-text first 100 lines match reference IPA when data and "
    "golden...`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/lang-specific/german.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`

## core/moonshine-tts/tests/heteronym-context-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 10) `TEST_CASE("heteronym_centered_context_window_cells short pad")`
  - `TEST_CASE` (function, line 20) `TEST_CASE("heteronym_centered_context_window_cells crop")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/lang-specific/heteronym-context.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/tests/hindi-rule-g2p-test.cpp
- Layer: business_logic
- Language: cpp
- Symbols:
  - `check_wiki_parity` (function, line 17) `void check_wiki_parity(const std::filesystem::path& wiki,
                       const std::files...`
  - `TEST_CASE` (function, line 37) `TEST_CASE("hindi: dialect_resolves_to_hindi_rules")`
  - `TEST_CASE` (function, line 45) `TEST_CASE("hindi: कमल and मैं match reference IPA when golden exists")`
  - `TEST_CASE` (function, line 60) `TEST_CASE("hindi: expand_cardinal_digits_to_hindi_words")`
  - `TEST_CASE` (function, line 66) `TEST_CASE(
    "hindi: wiki-text first 100 lines match reference IPA when data and golden "
    "...`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/lang-specific/hindi-numbers.h`, `core/moonshine-tts/src/lang-specific/hindi.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`

## core/moonshine-tts/tests/ipa-postprocess-test.cpp
- Doc: ma_in: 妈 ma˥˥ → mˈa5 via the zh path
- Layer: testing
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 10) `TEST_CASE("levenshtein_distance")`
  - `TEST_CASE` (function, line 17) `TEST_CASE("pick_closest_cmudict_ipa single")`
  - `TEST_CASE` (function, line 22) `TEST_CASE("match_prediction_to_cmudict_ipa")`
  - `TEST_CASE` (function, line 29) `TEST_CASE("normalize_g2p_ipa_for_piper_engines")`
  - `TEST_CASE` (function, line 45) `TEST_CASE("repair_ascii_c_combining_cedilla_to_ccedilla_utf8")`
  - `TEST_CASE` (function, line 57) `TEST_CASE("normalize_g2p_ipa_for_piper NFC plus shared rules")`
  - `TEST_CASE` (function, line 66) `TEST_CASE("coerce_unknown_ipa_chars_to_piper_inventory toy map")`
  - `TEST_CASE` (function, line 78) `TEST_CASE("ipa_to_piper_ready without coercion")`
  - `TEST_CASE` (function, line 89) `TEST_CASE("normalize_g2p_ipa_for_piper Korean rule IPA toward eSpeak-ng")`
  - `TEST_CASE` (function, line 111) `TEST_CASE("normalize_russian_ipa_piper_style")`
  - `TEST_CASE` (function, line 167) `TEST_CASE("normalize_german_ipa_piper_style")`
  - `TEST_CASE` (function, line 190) `TEST_CASE("normalize_g2p_ipa_for_piper German applies piper-style pass")`
  - `TEST_CASE` (function, line 198) `TEST_CASE("normalize_chinese_ipa_piper_style full pipeline single syllables")`
  - `TEST_CASE` (function, line 223) `TEST_CASE("normalize_chinese_ipa_piper_style retroflexes")`
  - `TEST_CASE` (function, line 240) `TEST_CASE("normalize_chinese_ipa_piper_style dental sibilants")`
  - `TEST_CASE` (function, line 247) `TEST_CASE("normalize_chinese_ipa_piper_style velar fricative")`
  - `TEST_CASE` (function, line 254) `TEST_CASE("normalize_chinese_ipa_piper_style er/erhua")`
  - `TEST_CASE` (function, line 261) `TEST_CASE("normalize_chinese_ipa_piper_style mid vowel")`
  - `TEST_CASE` (function, line 274) `TEST_CASE("normalize_chinese_ipa_piper_style -ong and -uo finals")`
  - `TEST_CASE` (function, line 287) `TEST_CASE("normalize_chinese_ipa_piper_style ü-finals")`
  - `TEST_CASE` (function, line 301) `TEST_CASE(
    "normalize_chinese_ipa_piper_style tone repositioning before nasals")`
  - `TEST_CASE` (function, line 321) `TEST_CASE("normalize_chinese_ipa_piper_style aspiration")`
  - `TEST_CASE` (function, line 334) `TEST_CASE("normalize_g2p_ipa_for_piper Chinese wired up for zh keys")`
  - `kBar` (function, line 168) `static const std::string kBar("\xcd\xa1");`
  - `ma_in` (function, line 336) `const std::string ma_in("ma\xcb\xa5\xcb\xa5");`
  - `expected` (function, line 337) `const std::string expected( "m\xcb\x88" "a5");`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/ipa-postprocess.h`

## core/moonshine-tts/tests/italian-rule-g2p-test.cpp
- Layer: business_logic
- Language: cpp
- Symbols:
  - `make_temp_tsv` (function, line 17) `std::filesystem::path make_temp_tsv(const char* contents)`
  - `TEST_CASE` (function, line 29) `TEST_CASE("italian: dialect_resolves_to_italian_rules")`
  - `TEST_CASE` (function, line 38) `TEST_CASE("italian: lowercase homograph overrides capitalized")`
  - `TEST_CASE` (function, line 47) `TEST_CASE("italian: lexicon stress not shifted by vocoder")`
  - `TEST_CASE` (function, line 56) `TEST_CASE("italian: c'è matches reference IPA when data and golden exist")`
  - `TEST_CASE` (function, line 74) `TEST_CASE(
    "italian: wiki-text first 100 lines match reference IPA when data and "
    "golde...`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/lang-specific/italian.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`

## core/moonshine-tts/tests/japanese-onnx-g2p-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 10) `TEST_CASE(
    "japanese onnx g2p: first 100 wiki IPA lines match reference when assets "
    "an...`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`

## core/moonshine-tts/tests/japanese-tok-pos-onnx-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 10) `TEST_CASE("japanese tok pos: single sentence matches reference file")`
  - `TEST_CASE` (function, line 28) `TEST_CASE(
    "japanese tok pos: long input is split and does not exceed model length")`
  - `TEST_CASE` (function, line 48) `TEST_CASE(
    "japanese tok pos: first 100 wiki lines match reference when assets and "
    "gol...`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`

## core/moonshine-tts/tests/json-config-test.cpp
- Layer: infrastructure
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 11) `TEST_CASE("load_oov_tables from onnx-config.json")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/json-config.h`

## core/moonshine-tts/tests/korean-rule-g2p-test.cpp
- Layer: business_logic
- Language: cpp
- Symbols:
  - `ko_dict_path` (function, line 19) `std::filesystem::path ko_dict_path()`
  - `TEST_CASE` (function, line 25) `TEST_CASE("korean: dialect_resolves_to_korean_rules")`
  - `TEST_CASE` (function, line 34) `TEST_CASE(
    "korean: normalize strips all combining marks including tense and "
    "unreleased")`
  - `TEST_CASE` (function, line 67) `TEST_CASE("korean: int_to_sino_korean_hangul")`
  - `TEST_CASE` (function, line 79) `TEST_CASE("korean: korean_reading_fragments_from_ascii_numeral_token")`
  - `TEST_CASE` (function, line 103) `TEST_CASE("korean: G2P examples with data/ko/dict.tsv")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/lang-specific/korean-numbers.h`, `core/moonshine-tts/src/lang-specific/korean.h`, `core/moonshine-tts/src/moonshine-g2p.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`

## core/moonshine-tts/tests/korean-tok-pos-onnx-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 10) `TEST_CASE("korean tok pos: single sentence matches reference file")`
  - `TEST_CASE` (function, line 27) `TEST_CASE(
    "korean tok pos: first 100 wiki lines match reference when assets and "
    "golde...`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`

## core/moonshine-tts/tests/moonshine-g2p-options-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 19) `TEST_CASE("MoonshineG2POptions default constructor seeds canonical file keys")`
  - `TEST_CASE` (function, line 35) `TEST_CASE(
    "MoonshineG2POptions relative_asset_path falls back when key absent")`
  - `TEST_CASE` (function, line 43) `TEST_CASE("MoonshineG2POptions parse_options rejects unknown keys")`
  - `TEST_CASE` (function, line 49) `TEST_CASE("MoonshineG2POptions parse_options accepts every known option")`
  - `TEST_CASE` (function, line 125) `TEST_CASE(
    "MoonshineG2POptions parse_options empty path clears canonical entry")`
  - `TEST_CASE` (function, line 134) `TEST_CASE("MoonshineG2POptions option names are case-insensitive")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/moonshine-g2p-options.h`

## core/moonshine-tts/tests/moonshine-tts-options-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 12) `TEST_CASE("MoonshineTTSOptions parse_options ort_providers")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/moonshine-tts-options.h`

## core/moonshine-tts/tests/moonshine-tts-speed-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `bundled_tts_data_present` (function, line 14) `bool bundled_tts_data_present(const std::filesystem::path& root)`
  - `TEST_CASE` (function, line 24) `TEST_CASE(
    "MoonshineTTS Kokoro: per-call speed changes duration and restores "
    "default")`
  - `TEST_CASE` (function, line 47) `TEST_CASE("MoonshineTTS Piper: per-call speed reduces duration vs baseline")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/moonshine-tts.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`

## core/moonshine-tts/tests/onnx-g2p-smoke-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 13) `TEST_CASE(
    "MoonshineG2P en_us rule-based when MOONSHINE_TTS_MODELS_ROOT is set")`
  - `TEST_CASE` (function, line 33) `TEST_CASE("MoonshineG2P ja-JP when data/ja assets exist under repo")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/moonshine-g2p.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`

## core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp
- Layer: business_logic
- Language: cpp
- Symbols:
  - `make_temp_tsv` (function, line 17) `std::filesystem::path make_temp_tsv(const char* contents)`
  - `TEST_CASE` (function, line 29) `TEST_CASE("portuguese: dialect flags")`
  - `TEST_CASE` (function, line 40) `TEST_CASE("portuguese: lowercase homograph overrides capitalized")`
  - `TEST_CASE` (function, line 49) `TEST_CASE("portuguese: lexicon stress not shifted by vocoder")`
  - `TEST_CASE` (function, line 58) `TEST_CASE("portuguese: casa matches reference IPA when data and golden exist")`
  - `TEST_CASE` (function, line 73) `TEST_CASE(
    "portuguese: wiki-text first 100 lines pt_br match reference IPA when data "
    "...`
  - `TEST_CASE` (function, line 99) `TEST_CASE(
    "portuguese: wiki-text first 100 lines pt_pt match reference IPA when data "
    "...`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/lang-specific/portuguese.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`

## core/moonshine-tts/tests/rule-g2p-test-support.h
- Doc: Shared helpers for rule-G2P / ONNX parity tests (pre-generated reference lines under...
- Layer: business_logic
- Language: h
- Symbols:
  - `repo_root_from_tests_cpp` (function, line 21) `inline std::filesystem::path repo_root_from_tests_cpp(
    const char* tests_cpp_file)`
  - `tests_data_dir` (function, line 34) `inline std::filesystem::path tests_data_dir(
    const std::filesystem::path& repo_root)`
  - `split_unix_lines` (function, line 53) `inline std::vector<std::string> split_unix_lines(std::string block)`
  - `load_ref_text_trimmed` (function, line 66) `inline std::string load_ref_text_trimmed(const std::filesystem::path& p)`
  - `load_ref_lines` (function, line 76) `inline std::vector<std::string> load_ref_lines(const std::filesystem::path& p)`
  - `ref_lines_prefix` (function, line 85) `inline std::vector<std::string> ref_lines_prefix(
    const std::filesystem::path& golden, std::s...`
  - `read_text_first_lines` (function, line 96) `inline std::vector<std::string> read_text_first_lines(
    const std::filesystem::path& p, std::s...`
  - `moonshine_tts_bundled_data_dir_relative` (function, line 114) `inline std::filesystem::path moonshine_tts_bundled_data_dir_relative()`
  - `MOONSHINE_TTS_TESTS_RULE_G2P_TEST_SUPPORT_H` (macro, line 2) `#define MOONSHINE_TTS_TESTS_RULE_G2P_TEST_SUPPORT_H`
- Imported by: `core/moonshine-tts/tests/arabic-rule-g2p-test.cpp`, `core/moonshine-tts/tests/chinese-rule-g2p-test.cpp`, `core/moonshine-tts/tests/chinese-tok-pos-onnx-test.cpp`, `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp`, `core/moonshine-tts/tests/english-rule-g2p-test.cpp`, `core/moonshine-tts/tests/french-rule-g2p-test.cpp`, `core/moonshine-tts/tests/german-rule-g2p-test.cpp`, `core/moonshine-tts/tests/hindi-rule-g2p-test.cpp`, `core/moonshine-tts/tests/italian-rule-g2p-test.cpp`, `core/moonshine-tts/tests/japanese-onnx-g2p-test.cpp`, `core/moonshine-tts/tests/japanese-tok-pos-onnx-test.cpp`, `core/moonshine-tts/tests/korean-rule-g2p-test.cpp`, `core/moonshine-tts/tests/korean-tok-pos-onnx-test.cpp`, `core/moonshine-tts/tests/moonshine-tts-speed-test.cpp`, `core/moonshine-tts/tests/onnx-g2p-smoke-test.cpp`, `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp`, `core/moonshine-tts/tests/russian-rule-g2p-test.cpp`, `core/moonshine-tts/tests/spanish-rule-g2p-test.cpp`, `core/moonshine-tts/tests/turkish-rule-g2p-test.cpp`, `core/moonshine-tts/tests/ukrainian-rule-g2p-test.cpp`, `core/moonshine-tts/tests/vietnamese-rule-g2p-test.cpp`

## core/moonshine-tts/tests/russian-rule-g2p-test.cpp
- Layer: business_logic
- Language: cpp
- Symbols:
  - `make_temp_tsv` (function, line 21) `std::filesystem::path make_temp_tsv(const char* contents)`
  - `TEST_CASE` (function, line 33) `TEST_CASE("russian: dialect_resolves_to_russian_rules")`
  - `TEST_CASE` (function, line 42) `TEST_CASE("russian: lowercase homograph overrides capitalized")`
  - `TEST_CASE` (function, line 69) `TEST_CASE("russian: litva matches reference IPA when data and golden exist")`
  - `TEST_CASE` (function, line 84) `TEST_CASE(
    "russian: Cyrillic preposition plus 1891 matches reference IPA when data "
    "an...`
  - `TEST_CASE` (function, line 102) `TEST_CASE(
    "russian: wiki-text first 100 lines match reference IPA when data and "
    "golde...`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/lang-specific/russian.h`, `core/moonshine-tts/src/moonshine-g2p.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`

## core/moonshine-tts/tests/spanish-rule-g2p-test.cpp
- Layer: business_logic
- Language: cpp
- Symbols:
  - `check_wiki_parity` (function, line 16) `void check_wiki_parity(const std::filesystem::path& wiki,
                       const std::files...`
  - `TEST_CASE` (function, line 35) `TEST_CASE("spanish: En 1891 matches reference IPA when golden exists")`
  - `TEST_CASE` (function, line 47) `TEST_CASE("spanish: dialect ids include es-MX and es-ES")`
  - `TEST_CASE` (function, line 53) `TEST_CASE(
    "spanish: wiki-text first 100 lines es_mx match reference IPA when data "
    "and...`
  - `TEST_CASE` (function, line 65) `TEST_CASE(
    "spanish: wiki-text first 100 lines es_es match reference IPA when data "
    "and...`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/lang-specific/spanish.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`

## core/moonshine-tts/tests/text-normalize-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 8) `TEST_CASE("split_text_to_words")`
  - `TEST_CASE` (function, line 16) `TEST_CASE("normalize_word_for_lookup")`
  - `TEST_CASE` (function, line 21) `TEST_CASE("normalize_grapheme_key strips alternate suffix")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/text-normalize.h`

## core/moonshine-tts/tests/turkish-rule-g2p-test.cpp
- Layer: business_logic
- Language: cpp
- Symbols:
  - `check_wiki_parity` (function, line 16) `void check_wiki_parity(const std::filesystem::path& wiki,
                       const std::files...`
  - `TEST_CASE` (function, line 34) `TEST_CASE("turkish: dağ and değer match reference IPA when golden exists")`
  - `TEST_CASE` (function, line 46) `TEST_CASE("turkish: dialect ids include tr and tr-TR")`
  - `TEST_CASE` (function, line 52) `TEST_CASE(
    "turkish: wiki-text first 100 lines match reference IPA when data and "
    "golde...`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/lang-specific/turkish.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`

## core/moonshine-tts/tests/ukrainian-rule-g2p-test.cpp
- Layer: business_logic
- Language: cpp
- Symbols:
  - `check_wiki_parity` (function, line 16) `void check_wiki_parity(const std::filesystem::path& wiki,
                       const std::files...`
  - `TEST_CASE` (function, line 34) `TEST_CASE("ukrainian: m'ясо and кінь match reference IPA when golden exists")`
  - `TEST_CASE` (function, line 46) `TEST_CASE("ukrainian: dialect ids include uk and uk-UA")`
  - `TEST_CASE` (function, line 52) `TEST_CASE(
    "ukrainian: wiki-text first 100 lines match reference IPA when data and "
    "gol...`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/lang-specific/ukrainian.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`

## core/moonshine-tts/tests/utf8-utils-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 8) `TEST_CASE("utf8_split_codepoints ascii")`
  - `TEST_CASE` (function, line 16) `TEST_CASE("utf8_split_codepoints two-byte")`
  - `TEST_CASE` (function, line 23) `TEST_CASE("utf8_find_token_codepoints")`
  - `TEST_CASE` (function, line 31) `TEST_CASE("digit_ascii_span_expandable_python_w")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/tests/vietnamese-rule-g2p-test.cpp
- Layer: business_logic
- Language: cpp
- Symbols:
  - `vi_dict_path` (function, line 18) `std::filesystem::path vi_dict_path()`
  - `TEST_CASE` (function, line 24) `TEST_CASE("vietnamese: dialect_resolves_to_vietnamese_rules")`
  - `TEST_CASE` (function, line 33) `TEST_CASE("vietnamese: syllable OOV parity with Python samples")`
  - `TEST_CASE` (function, line 42) `TEST_CASE("vietnamese: lexicon line with data/vi/dict.tsv")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/lang-specific/vietnamese.h`, `core/moonshine-tts/src/moonshine-g2p.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`

## core/moonshine-tts/tests/zipvoice-tts-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 14) `TEST_CASE("zipvoice-builtin-voices")`
  - `TEST_CASE` (function, line 46) `TEST_CASE("zipvoice-vocos-fbank")`
  - `TEST_CASE` (function, line 67) `TEST_CASE("zipvoice-compress-long-pauses")`
  - `tone` (function, line 50) `std::vector<float> tone(static_cast<size_t>(sr));`
  - `x` (function, line 70) `std::vector<float> x(n);`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 1) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-tts/src/zipvoice-mel.h`, `core/moonshine-tts/src/zipvoice-tts.h`, `core/moonshine-tts/src/zipvoice-voices.h`
