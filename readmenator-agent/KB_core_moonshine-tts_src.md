# Subsystem: core_moonshine-tts_src (page 1 of 2)
Pages: [KB_core_moonshine-tts_src.md](KB_core_moonshine-tts_src.md), [KB_core_moonshine-tts_src_p2.md](KB_core_moonshine-tts_src_p2.md)

## core/moonshine-tts/src/constants.h
- Layer: utility
- Language: h
- Symbols:
  - `MOONSHINE_TTS_CONSTANTS_H` (macro, line 2) `#define MOONSHINE_TTS_CONSTANTS_H`
- Imported by: `core/moonshine-tts/src/json-config.cpp`, `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp`

## core/moonshine-tts/src/file-information.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `FileInformation` (function, line 8) `FileInformation::FileInformation(const FileInformation& o)
    : path(o.path), owned_storage_(o.o...`
  - `load` (function, line 35) `void FileInformation::load(const uint8_t** out_memory, size_t* out_size)`
  - `free` (function, line 81) `void FileInformation::free()`
  - `set_memory` (function, line 90) `void FileInformationMap::set_memory(std::string_view key, const uint8_t* mem,
                   ...`
  - `parse_file_list` (function, line 99) `void FileInformationMap::parse_file_list(
    const std::vector<std::pair<std::string, std::strin...`
- Depends on: `core/moonshine-tts/src/file-information.h`

## core/moonshine-tts/src/file-information.h
- Doc: FileInformation: Describes a bundled asset: optional on-disk ``path`` (relative to a caller root...
- Layer: utility
- Language: h
- Symbols:
  - `FileInformation` (struct, line 18)
  - `FileInformationMap` (struct, line 51)
  - `FileInformation` (function, line 24) `FileInformation(std::filesystem::path p, const uint8_t* mem, size_t sz)
      : path(std::move(p)...`
  - `set_path` (function, line 54) `void set_path(std::string_view key, std::filesystem::path path)`
  - `erase_key` (function, line 63) `void erase_key(std::string_view key)`
  - `contains` (function, line 65) `bool contains(std::string_view key) const`
  - `load` (function, line 35) `void load(const uint8_t** out_memory, size_t* out_size);`
  - `free` (function, line 40) `void free();`
  - `parse_file_list` (function, line 71) `void parse_file_list( const std::vector<std::pair<std::string, std::string>>* key_list, const std::vector<uint8_t*>*...`
  - `MOONSHINE_TTS_FILE_INFORMATION_H` (macro, line 2) `#define MOONSHINE_TTS_FILE_INFORMATION_H`
- Imported by: `core/moonshine-tts/src/file-information.cpp`, `core/moonshine-tts/src/moonshine-asset-catalog.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-tts/src/moonshine-tts-options.h`, `core/moonshine-tts/src/ort-onnx-external-data.h`, `core/moonshine-tts/src/piper-tts.h`, `core/moonshine-tts/src/zipvoice-tts.h`, `core/moonshine-tts/tests/file-information-test.cpp`

## core/moonshine-tts/src/g2p-path.h
- Doc: resolve_path_under_root: If ``path`` is absolute, returns it unchanged.
- Layer: utility
- Language: h
- Symbols:
  - `resolve_path_under_root` (function, line 13) `inline std::filesystem::path resolve_path_under_root(
    const std::filesystem::path& root, cons...`
  - `resolve_prefer_ort_model` (function, line 30) `inline std::filesystem::path resolve_prefer_ort_model(
    const std::filesystem::path& dir, std:...`
  - `resolve_disk_model_file_path` (function, line 56) `inline void resolve_disk_model_file_path(std::filesystem::path& path)`
  - `b` (function, line 33) `const std::string b(basename);`
  - `MOONSHINE_TTS_G2P_PATH_H` (macro, line 2) `#define MOONSHINE_TTS_G2P_PATH_H`
- Imported by: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp`, `core/moonshine-tts/src/lang-specific/arabic.cpp`, `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp`, `core/moonshine-tts/src/lang-specific/chinese.cpp`, `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp`, `core/moonshine-tts/src/lang-specific/japanese.cpp`, `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp`, `core/moonshine-tts/src/moonshine-g2p-options.cpp`, `core/moonshine-tts/src/moonshine-tts.cpp`, `core/moonshine-tts/src/piper-tts.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/src/zipvoice-tts.cpp`

## core/moonshine-tts/src/g2p-word-log.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `g2p_word_path_tag` (function, line 7) `const char* g2p_word_path_tag(G2pWordPath path)`
  - `format_g2p_word_log_line` (function, line 35) `std::string format_g2p_word_log_line(const G2pWordLog& e)`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`

## core/moonshine-tts/src/g2p-word-log.h
- Doc: G2pWordPath: How a surface word was converted to IPA in ``MoonshineG2P`` / ``EnglishRuleG2p``...
- Layer: utility
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 29)
  - `G2pWordPath` (enum, line 11)
  - `G2pWordPath` (class, line 11)
  - `g2p_word_path_tag` (function, line 27) `const char* g2p_word_path_tag(G2pWordPath path);`
  - `MOONSHINE_TTS_G2P_WORD_LOG_H` (macro, line 2) `#define MOONSHINE_TTS_G2P_WORD_LOG_H`
- Imported by: `core/moonshine-tts/src/g2p-word-log.cpp`, `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp`, `core/moonshine-tts/src/lang-specific/chinese.cpp`, `core/moonshine-tts/src/lang-specific/dutch.cpp`, `core/moonshine-tts/src/lang-specific/english.cpp`, `core/moonshine-tts/src/lang-specific/french.cpp`, `core/moonshine-tts/src/lang-specific/german.cpp`, `core/moonshine-tts/src/lang-specific/hindi.cpp`, `core/moonshine-tts/src/lang-specific/italian.cpp`, `core/moonshine-tts/src/lang-specific/japanese.cpp`, `core/moonshine-tts/src/lang-specific/korean.cpp`, `core/moonshine-tts/src/lang-specific/portuguese.cpp`, `core/moonshine-tts/src/lang-specific/russian.cpp`, `core/moonshine-tts/src/lang-specific/spanish.cpp`, `core/moonshine-tts/src/lang-specific/turkish.cpp`, `core/moonshine-tts/src/lang-specific/ukrainian.cpp`, `core/moonshine-tts/src/lang-specific/vietnamese.cpp`, `core/moonshine-tts/src/moonshine-g2p.h`, `core/moonshine-tts/tools/moonshine-g2p-cli.cpp`

## core/moonshine-tts/src/ipa-postprocess.cpp
- Doc: apply_german_ipa_piper_style: U+0361 COMBINING DOUBLE INVERTED BREVE between consonants (narrow...
- Layer: utility
- Language: cpp
- Symbols:
  - `replace_utf8_all` (function, line 21) `void replace_utf8_all(std::string& s, std::string_view old_utf8,
                      std::strin...`
  - `trim_copy` (function, line 30) `std::string trim_copy(std::string t)`
  - `strip_length_markers_copy` (function, line 37) `std::string strip_length_markers_copy(std::string t)`
  - `apply_shared_g2p_to_piper_replacements` (function, line 46) `void apply_shared_g2p_to_piper_replacements(std::string& s)`
  - `apply_korean_post_normalize_ipa` (function, line 54) `void apply_korean_post_normalize_ipa(std::string& s)`
  - `apply_german_ipa_piper_style` (function, line 76) `void apply_german_ipa_piper_style(std::string& s)`
  - `apply_lang_specific_replacements` (function, line 106) `void apply_lang_specific_replacements(std::string& s,
                                      std::...`
  - `py_isspace_one_utf8_char` (function, line 151) `bool py_isspace_one_utf8_char(std::string_view ch)`
  - `unicode_category_first_char_is_p_or_s` (function, line 170) `bool unicode_category_first_char_is_p_or_s(char32_t cp)`
  - `category_is_mn_or_me` (function, line 175) `bool category_is_mn_or_me(char32_t cp)`
  - `is_ipa_like_inventory_char` (function, line 181) `bool is_ipa_like_inventory_char(char32_t cp)`
  - `utf8_singleton_codepoint` (function, line 206) `char32_t utf8_singleton_codepoint(std::string_view token)`
  - `utf8_prev_codepoint_start` (function, line 216) `size_t utf8_prev_codepoint_start(const std::string& s, size_t char_start)`
  - `rewrite_russian_combining_acute_to_primary_stress` (function, line 230) `void rewrite_russian_combining_acute_to_primary_stress(std::string& s)`
  - `apply_russian_ipa_piper_style` (function, line 276) `void apply_russian_ipa_piper_style(std::string& s)`
  - `repair_ascii_c_combining_cedilla_to_ccedilla_utf8` (function, line 368) `void repair_ascii_c_combining_cedilla_to_ccedilla_utf8(std::string& s)`
  - `normalize_russian_ipa_piper_style` (function, line 379) `std::string normalize_russian_ipa_piper_style(std::string ipa)`
  - `normalize_german_ipa_piper_style` (function, line 384) `std::string normalize_german_ipa_piper_style(std::string ipa)`
  - `is_cmn_vowel_cp` (function, line 394) `bool is_cmn_vowel_cp(char32_t cp)`
  - `is_cmn_tone_marker` (function, line 416) `bool is_cmn_tone_marker(char32_t cp)`
  - `normalize_chinese_ipa_piper_style` (function, line 421) `std::string normalize_chinese_ipa_piper_style(std::string ipa)`
  - `utf8_nfc_copy` (function, line 660) `std::string utf8_nfc_copy(std::string_view s)`
  - `normalize_g2p_ipa_for_piper` (function, line 672) `std::string normalize_g2p_ipa_for_piper(std::string_view ipa_utf8,
                              ...`
  - `coerce_unknown_ipa_chars_to_piper_inventory` (function, line 690) `std::string coerce_unknown_ipa_chars_to_piper_inventory(
    std::string_view ipa_utf8,
    const...`
  - `ipa_to_piper_ready` (function, line 762) `std::string ipa_to_piper_ready(
    std::string_view ipa_utf8, std::string_view piper_lang_key,
 ...`
  - `normalize_g2p_ipa_for_piper_engines` (function, line 774) `std::string normalize_g2p_ipa_for_piper_engines(std::string_view ipa_utf8)`
  - `ipa_string_to_phoneme_tokens` (function, line 780) `std::vector<std::string> ipa_string_to_phoneme_tokens(const std::string& s)`
  - `levenshtein_distance` (function, line 806) `int levenshtein_distance(const std::vector<std::string>& a,
                         const std::v...`
  - `pick_closest_alternative_index` (function, line 837) `int pick_closest_alternative_index(
    const std::vector<std::string>& predicted_phoneme_tokens,...`
  - `pick_closest_cmudict_ipa` (function, line 866) `std::string pick_closest_cmudict_ipa(
    const std::vector<std::string>& predicted_phoneme_token...`
  - `match_prediction_to_cmudict_ipa` (function, line 882) `std::optional<std::string> match_prediction_to_cmudict_ipa(
    const std::string& predicted, con...`
  - `kBar` (function, line 77) `static const std::string kBar("\xcd\xa1");`
  - `kTurnedACombBreve` (function, line 92) `static const std::string kTurnedACombBreve("\xc9\x90\xcc\xaf");`
  - `kAlveolarTap` (function, line 93) `static const std::string kAlveolarTap("\xc9\xbe");`
  - `kUvuR` (function, line 97) `static const std::string kUvuR("\xca\x81");`
  - `key` (function, line 141) `const std::string key(eff);`
  - `kAcute` (function, line 231) `static const std::string kAcute("\xcc\x81");`
  - `kPri` (function, line 232) `static const std::string kPri("\xcb\x88");`
  - `kSec` (function, line 233) `static const std::string kSec( "\xcb\x8c");`
  - `kZhd` (function, line 336) `static const std::string kZhd("\xca\x90");`
  - `kZhj` (function, line 337) `static const std::string kZhj("\xca\x92");`
  - `kIsp` (function, line 356) `static const std::string kIsp("\xc9\xaa ");`
  - `kPrecomposedCcedilla` (function, line 371) `static const std::string kPrecomposedCcedilla("\xc3\xa7");`
  - `kEng` (function, line 515) `static const std::string kEng("\xc5\x8b");`
  - `kStress` (function, line 602) `static const std::string kStress("\xcb\x88");`
  - `tmp` (function, line 661) `const std::string tmp(s);`
  - `prev` (function, line 816) `std::vector<int> prev(static_cast<size_t>(lb + 1));`
  - `cur` (function, line 817) `std::vector<int> cur(static_cast<size_t>(lb + 1));`
  - `0` (variable, line 5) `extern "C" { #include <utf8proc.h> } #include <algorithm> #include <cctype> #include <cstddef> #include <cstdlib>...`
- Depends on: `core/moonshine-tts/src/ipa-postprocess.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/ipa-postprocess.h
- Doc: repair_ascii_c_combining_cedilla_to_ccedilla_utf8: Replace ASCII ``c`` + U+0327 COMBINING...
- Layer: utility
- Language: h
- Symbols:
  - `repair_ascii_c_combining_cedilla_to_ccedilla_utf8` (function, line 19) `void repair_ascii_c_combining_cedilla_to_ccedilla_utf8(std::string& ipa_utf8);`
  - `levenshtein_distance` (function, line 68) `int levenshtein_distance(const std::vector<std::string>& a, const std::vector<std::string>& b);`
  - `pick_closest_alternative_index` (function, line 71) `int pick_closest_alternative_index( const std::vector<std::string>& predicted_phoneme_tokens, const...`
  - `MOONSHINE_TTS_IPA_POSTPROCESS_H` (macro, line 2) `#define MOONSHINE_TTS_IPA_POSTPROCESS_H`
- Imported by: `core/moonshine-tts/src/ipa-postprocess.cpp`, `core/moonshine-tts/src/lang-specific/german.cpp`, `core/moonshine-tts/src/lang-specific/russian.cpp`, `core/moonshine-tts/src/piper-tts.cpp`, `core/moonshine-tts/src/zipvoice-tts.cpp`, `core/moonshine-tts/tests/ipa-postprocess-test.cpp`, `core/moonshine-tts/tools/piper-ipa-normalize-cli.cpp`

## core/moonshine-tts/src/json-config.cpp
- Layer: infrastructure
- Language: cpp
- Symbols:
  - `read_json_file` (function, line 14) `nlohmann::json read_json_file(const std::filesystem::path& p)`
  - `validate_header` (function, line 24) `void validate_header(const nlohmann::json& cfg, const std::string& expect_kind,
                 ...`
  - `stoi_to_itos` (function, line 47) `std::vector<std::string> stoi_to_itos(
    const std::unordered_map<std::string, int64_t>& stoi)`
  - `load_oov_tables_from_json` (function, line 64) `OovOnnxTables load_oov_tables_from_json(const nlohmann::json& cfg,
                              ...`
  - `load_oov_tables` (function, line 88) `OovOnnxTables load_oov_tables(const std::filesystem::path& model_onnx_path)`
- Depends on: `core/moonshine-tts/src/constants.h`, `core/moonshine-tts/src/json-config.h`

## core/moonshine-tts/src/json-config.h
- Layer: infrastructure
- Language: h
- Symbols:
  - `OovOnnxTables` (struct, line 15)
  - `MOONSHINE_TTS_JSON_CONFIG_H` (macro, line 2) `#define MOONSHINE_TTS_JSON_CONFIG_H`
- Imported by: `core/moonshine-tts/src/json-config.cpp`, `core/moonshine-tts/src/lang-specific/onnx-g2p-models.h`, `core/moonshine-tts/tests/json-config-test.cpp`

## core/moonshine-tts/src/moonshine-asset-catalog.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `normalize_lang_key_cli` (function, line 16) `std::string normalize_lang_key_cli(std::string_view raw)`
  - `hyphen_to_underscore` (function, line 30) `std::string hyphen_to_underscore(std::string s)`
  - `english_g2p_keys` (function, line 39) `std::vector<std::string> english_g2p_keys()`
  - `chinese_g2p_keys` (function, line 48) `std::vector<std::string> chinese_g2p_keys()`
  - `japanese_g2p_keys` (function, line 58) `std::vector<std::string> japanese_g2p_keys()`
  - `korean_g2p_keys` (function, line 68) `std::vector<std::string> korean_g2p_keys()`
  - `arabic_g2p_keys` (function, line 74) `std::vector<std::string> arabic_g2p_keys()`
  - `french_g2p_keys` (function, line 84) `std::vector<std::string> french_g2p_keys()`
  - `lookup_g2p_dependency_keys` (function, line 223) `std::optional<std::vector<std::string>> lookup_g2p_dependency_keys(
    std::string_view raw)`
  - `moonshine_asset_catalog_populate_default_g2p_files` (function, line 240) `void moonshine_asset_catalog_populate_default_g2p_files(
    FileInformationMap& files)`
  - `moonshine_asset_catalog_g2p_dependency_keys` (function, line 249) `std::optional<std::vector<std::string>>
moonshine_asset_catalog_g2p_dependency_keys(std::string_v...`
  - `moonshine_asset_catalog_all_g2p_dependency_keys_union` (function, line 254) `std::vector<std::string>
moonshine_asset_catalog_all_g2p_dependency_keys_union()`
  - `moonshine_asset_catalog_all_registered_language_tags` (function, line 268) `std::vector<std::string>
moonshine_asset_catalog_all_registered_language_tags()`
- Depends on: `core/moonshine-tts/src/moonshine-asset-catalog.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/moonshine-asset-catalog.h
- Doc: moonshine_asset_catalog_populate_default_g2p_files: Fills ``files`` with default canonical G2P...
- Layer: utility
- Language: h
- Symbols:
  - `moonshine_asset_catalog_populate_default_g2p_files` (function, line 15) `void moonshine_asset_catalog_populate_default_g2p_files( FileInformationMap& files);`
  - `MOONSHINE_TTS_ASSET_CATALOG_H` (macro, line 2) `#define MOONSHINE_TTS_ASSET_CATALOG_H`
- Depends on: `core/moonshine-tts/src/file-information.h`
- Imported by: `core/moonshine-c-api.cpp`, `core/moonshine-tts/src/moonshine-asset-catalog.cpp`, `core/moonshine-tts/src/moonshine-g2p-options.cpp`, `core/moonshine-tts/src/moonshine-tts.cpp`

## core/moonshine-tts/src/moonshine-g2p-options.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `optional_path_from_string` (function, line 15) `std::optional<std::filesystem::path> optional_path_from_string(
    const std::string& value)`
  - `set_canonical_file` (function, line 24) `void set_canonical_file(FileInformationMap& files,
                        std::string_view canon...`
  - `set_override_file` (function, line 35) `void set_override_file(FileInformationMap& files, std::string_view map_key,
                     ...`
  - `is_known_g2p_option` (function, line 45) `bool is_known_g2p_option(std::string_view key)`
  - `prepare_g2p_file_information_path` (function, line 108) `void prepare_g2p_file_information_path(FileInformation& fi,
                                     ...`
  - `MoonshineG2POptions` (function, line 132) `MoonshineG2POptions::MoonshineG2POptions()`
  - `relative_asset_path` (function, line 136) `std::filesystem::path MoonshineG2POptions::relative_asset_path(
    std::string_view canonical_ke...`
  - `optional_override_path` (function, line 147) `std::optional<std::filesystem::path>
MoonshineG2POptions::optional_override_path(std::string_view...`
  - `asset_is_available` (function, line 159) `bool MoonshineG2POptions::asset_is_available(
    std::string_view canonical_key) const`
  - `read_binary_asset` (function, line 175) `std::vector<uint8_t> MoonshineG2POptions::read_binary_asset(
    std::string_view canonical_key) ...`
  - `read_utf8_asset` (function, line 193) `std::string MoonshineG2POptions::read_utf8_asset(
    std::string_view canonical_key) const`
  - `parse_options` (function, line 199) `void MoonshineG2POptions::parse_options(
    const std::vector<std::pair<std::string, std::string...`
  - `k` (function, line 138) `const std::string k(canonical_key);`
  - `out` (function, line 188) `std::vector<uint8_t> out(p, p + n);`
- Depends on: `core/moonshine-tts/src/g2p-path.h`, `core/moonshine-tts/src/moonshine-asset-catalog.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-utils/string-utils.h`, `core/ort-utils/ort-utils.h`

## core/moonshine-tts/src/moonshine-g2p-options.h
- Doc: MoonshineG2POptions: Options for constructing ``MoonshineG2P`` (rule-engine paths and toggles...
- Layer: utility
- Language: h
- Symbols:
  - `MoonshineG2POptions` (struct, line 134)
  - `g2p_bundle_file_key` (function, line 18) `inline std::string g2p_bundle_file_key(std::string_view bundle_dir_key,
                         ...`
  - `asset_is_available` (function, line 186) `bool asset_is_available(std::string_view canonical_key) const;`
  - `read_binary_asset` (function, line 190) `std::vector<uint8_t> read_binary_asset(std::string_view canonical_key) const;`
  - `parse_options` (function, line 198) `void parse_options( const std::vector<std::pair<std::string, std::string>>& options);`
  - `MOONSHINE_TTS_MOONSHINE_G2P_OPTIONS_H` (macro, line 2) `#define MOONSHINE_TTS_MOONSHINE_G2P_OPTIONS_H`
- Depends on: `core/moonshine-tts/src/file-information.h`
- Imported by: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp`, `core/moonshine-tts/src/lang-specific/arabic.cpp`, `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp`, `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp`, `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp`, `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp`, `core/moonshine-tts/src/lang-specific/japanese.cpp`, `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp`, `core/moonshine-tts/src/moonshine-asset-catalog.cpp`, `core/moonshine-tts/src/moonshine-g2p-options.cpp`, `core/moonshine-tts/src/moonshine-g2p.h`, `core/moonshine-tts/src/moonshine-tts-options.h`, `core/moonshine-tts/src/moonshine-tts.h`, `core/moonshine-tts/src/piper-tts.h`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.h`, `core/moonshine-tts/src/zipvoice-tts.h`, `core/moonshine-tts/tests/moonshine-g2p-options-test.cpp`

## core/moonshine-tts/src/moonshine-g2p.cpp
- Doc: normalize_spanish_dialect_cli_key: Normalize user input like ``es_ar`` / ``es-mx`` to keys...
- Layer: utility
- Language: cpp
- Symbols:
  - `trim_copy` (function, line 31) `std::string trim_copy(std::string_view s)`
  - `normalize_spanish_dialect_cli_key` (function, line 45) `std::string normalize_spanish_dialect_cli_key(std::string_view raw)`
  - `rule_backend_name` (function, line 68) `const char* rule_backend_name(RuleBasedG2pKind k)`
  - `dialect_resolves_to_spanish_rules` (function, line 108) `bool dialect_resolves_to_spanish_rules(std::string_view dialect_id,
                             ...`
  - `dialect_uses_rule_based_g2p` (function, line 122) `bool dialect_uses_rule_based_g2p(std::string_view dialect_id,
                                 co...`
  - `MoonshineG2P` (function, line 186) `MoonshineG2P::MoonshineG2P(std::string dialect_id,
                           MoonshineG2POptions...`
  - `text_to_ipa` (function, line 217) `std::string MoonshineG2P::text_to_ipa(std::string_view text,
                                    ...`
- Depends on: `core/moonshine-tts/src/lang-specific/arabic.h`, `core/moonshine-tts/src/lang-specific/chinese.h`, `core/moonshine-tts/src/lang-specific/dutch.h`, `core/moonshine-tts/src/lang-specific/english.h`, `core/moonshine-tts/src/lang-specific/french.h`, `core/moonshine-tts/src/lang-specific/german.h`, `core/moonshine-tts/src/lang-specific/hindi.h`, `core/moonshine-tts/src/lang-specific/italian.h`, `core/moonshine-tts/src/lang-specific/japanese.h`, `core/moonshine-tts/src/lang-specific/korean.h`, `core/moonshine-tts/src/lang-specific/portuguese.h`, `core/moonshine-tts/src/lang-specific/russian.h`, `core/moonshine-tts/src/lang-specific/spanish.h`, `core/moonshine-tts/src/lang-specific/turkish.h`, `core/moonshine-tts/src/lang-specific/ukrainian.h`, `core/moonshine-tts/src/lang-specific/vietnamese.h`, `core/moonshine-tts/src/moonshine-g2p.h`, `core/moonshine-tts/src/rule-based-g2p-factory.h`, `core/moonshine-tts/src/rule-based-g2p.h`, `core/moonshine-tts/src/utf8-utils.h`, `core/moonshine-utils/debug-utils.h`

## core/moonshine-tts/src/moonshine-g2p.h
- Doc: MoonshineG2P: Single entry point: *dialect_id* is a tag such as ``en_us``, ``es-AR``, ``de``...
- Layer: utility
- Language: h
- Symbols:
  - `MoonshineG2P` (class, line 34)
  - `uses_spanish_rules` (function, line 48) `bool uses_spanish_rules() const`
  - `uses_german_rules` (function, line 51) `bool uses_german_rules() const`
  - `uses_french_rules` (function, line 54) `bool uses_french_rules() const`
  - `uses_dutch_rules` (function, line 57) `bool uses_dutch_rules() const`
  - `uses_italian_rules` (function, line 60) `bool uses_italian_rules() const`
  - `uses_russian_rules` (function, line 63) `bool uses_russian_rules() const`
  - `uses_chinese_rules` (function, line 66) `bool uses_chinese_rules() const`
  - `uses_korean_rules` (function, line 69) `bool uses_korean_rules() const`
  - `uses_vietnamese_rules` (function, line 72) `bool uses_vietnamese_rules() const`
  - `uses_japanese_rules` (function, line 75) `bool uses_japanese_rules() const`
  - `uses_arabic_rules` (function, line 78) `bool uses_arabic_rules() const`
  - `uses_portuguese_rules` (function, line 81) `bool uses_portuguese_rules() const`
  - `uses_turkish_rules` (function, line 84) `bool uses_turkish_rules() const`
  - `uses_ukrainian_rules` (function, line 87) `bool uses_ukrainian_rules() const`
  - `uses_hindi_rules` (function, line 90) `bool uses_hindi_rules() const`
  - `uses_english_rules` (function, line 93) `bool uses_english_rules() const`
  - `uses_onnx` (function, line 99) `static constexpr bool uses_onnx()`
  - `dialect_id` (function, line 103) `const std::string& dialect_id() const`
  - `dialect_resolves_to_spanish_rules` (function, line 20) `bool dialect_resolves_to_spanish_rules(std::string_view dialect_id, bool spanish_narrow_obstruents = true);`
  - `MOONSHINE_TTS_G2P_H` (macro, line 2) `#define MOONSHINE_TTS_G2P_H`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-tts/src/rule-based-g2p-factory.h`
- Imported by: `core/moonshine-c-api.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/moonshine-tts.cpp`, `core/moonshine-tts/src/piper-tts.cpp`, `core/moonshine-tts/src/zipvoice-tts.cpp`, `core/moonshine-tts/tests/chinese-rule-g2p-test.cpp`, `core/moonshine-tts/tests/korean-rule-g2p-test.cpp`, `core/moonshine-tts/tests/onnx-g2p-smoke-test.cpp`, `core/moonshine-tts/tests/russian-rule-g2p-test.cpp`, `core/moonshine-tts/tests/vietnamese-rule-g2p-test.cpp`, `core/moonshine-tts/tools/moonshine-g2p-cli.cpp`

## core/moonshine-tts/src/moonshine-tts-options.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `apply_synthesis_output_effects` (function, line 13) `void apply_synthesis_output_effects(std::vector<float>& audio,
                                  ...`
  - `MoonshineTTSOptions` (function, line 39) `MoonshineTTSOptions::MoonshineTTSOptions()`
  - `apply_voice_engine_prefix` (function, line 46) `void MoonshineTTSOptions::apply_voice_engine_prefix()`
  - `tts_relative_path` (function, line 72) `std::filesystem::path MoonshineTTSOptions::tts_relative_path(
    std::string_view canonical_key)...`
  - `parse_options` (function, line 82) `void MoonshineTTSOptions::parse_options(
    const std::vector<std::pair<std::string, std::string...`
  - `k` (function, line 74) `const std::string k(canonical_key);`
  - `d` (function, line 121) `const std::filesystem::path d(t);`
- Depends on: `core/moonshine-tts/src/moonshine-tts-options.h`, `core/moonshine-utils/string-utils.h`, `core/ort-utils/ort-utils.h`

## core/moonshine-tts/src/moonshine-tts-options.h
- Doc: MoonshineTTSOptions: Shared configuration for ``MoonshineTTS`` (Kokoro and Piper file paths...
- Layer: utility
- Language: h
- Symbols:
  - `MoonshineTTSOptions` (struct, line 63)
  - `parse_options` (function, line 134) `void parse_options( const std::vector<std::pair<std::string, std::string>>& options, std::string* cli_language =...`
  - `apply_voice_engine_prefix` (function, line 142) `void apply_voice_engine_prefix();`
  - `apply_synthesis_output_effects` (function, line 149) `void apply_synthesis_output_effects(std::vector<float>& audio, bool normalize_audio, float volume);`
  - `MOONSHINE_TTS_MOONSHINE_TTS_OPTIONS_H` (macro, line 2) `#define MOONSHINE_TTS_MOONSHINE_TTS_OPTIONS_H`
- Depends on: `core/moonshine-tts/src/file-information.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`
- Imported by: `core/moonshine-tts/src/moonshine-tts-options.cpp`, `core/moonshine-tts/src/moonshine-tts.h`, `core/moonshine-tts/src/piper-tts.cpp`, `core/moonshine-tts/src/zipvoice-tts.cpp`, `core/moonshine-tts/tests/moonshine-tts-options-test.cpp`

## core/moonshine-tts/src/moonshine-tts.cpp
- Doc: SynthesisOverrides: Per-call overrides parsed from ``MoonshineTTS::synthesize`` option pairs.
- Layer: utility
- Language: cpp
- Symbols:
  - `SynthesisOverrides` (struct, line 70)
  - `LangProfile` (struct, line 158)
  - `KokoroTtsEngine` (struct, line 960)
  - `utf8_nfc` (function, line 44) `std::string utf8_nfc(std::string_view s)`
  - `replace_utf8` (function, line 56) `void replace_utf8(std::string& s, std::string_view old_s,
                  std::string_view new_s)`
  - `empty` (function, line 75) `bool empty() const`
  - `parse_synthesis_overrides_from_pairs` (function, line 81) `SynthesisOverrides parse_synthesis_overrides_from_pairs(
    const std::vector<std::pair<std::str...`
  - `py_isspace_utf8_ch` (function, line 98) `bool py_isspace_utf8_ch(std::string_view ch)`
  - `collapse_whitespace_join_single_space` (function, line 116) `std::string collapse_whitespace_join_single_space(const std::string& s)`
  - `normalize_lang_key` (function, line 144) `std::string normalize_lang_key(std::string_view raw)`
  - `lookup_lang_profile` (function, line 166) `const LangProfile* lookup_lang_profile(std::string_view key)`
  - `resolve_lang_for_tts` (function, line 202) `void resolve_lang_for_tts(const std::string& lk, const MoonshineG2POptions& opt,
                ...`
  - `kokoro_tts_lang_supported_inner` (function, line 220) `bool kokoro_tts_lang_supported_inner(std::string_view lang_cli,
                                 ...`
  - `voice_prefix_ok` (function, line 231) `bool voice_prefix_ok(char kokoro_lang, std::string_view voice)`
  - `maybe_align_en_profile_for_kokoro_voice` (function, line 252) `void maybe_align_en_profile_for_kokoro_voice(std::string_view voice,
                            ...`
  - `infer_lang_profile_from_kokoro_voice` (function, line 275) `bool infer_lang_profile_from_kokoro_voice(std::string_view voice_sv,
                            ...`
  - `resolve_lang_for_kokoro` (function, line 302) `void resolve_lang_for_kokoro(const std::string& lk,
                             const MoonshineG...`
  - `kokoro_voice_asset_exists` (function, line 316) `bool kokoro_voice_asset_exists(const std::string& voice_id,
                               const ...`
  - `select_voice_id` (function, line 358) `std::string select_voice_id(char kokoro_lang, std::string_view requested,
                       ...`
  - `apply_diphthong_map` (function, line 428) `void apply_diphthong_map(std::string& s, char kokoro_lang)`
  - `apply_chinese_kokoro_normalization` (function, line 461) `void apply_chinese_kokoro_normalization(std::string& ipa)`
  - `normalize_ipa_to_kokoro` (function, line 535) `std::string normalize_ipa_to_kokoro(
    std::string ipa, char kokoro_lang,
    const std::unorde...`
  - `chunk_phonemes` (function, line 557) `std::vector<std::string> chunk_phonemes(const std::string& ps,
                                  ...`
  - `phoneme_str_to_input_ids` (function, line 621) `std::vector<int64_t> phoneme_str_to_input_ids(
    const std::string& phonemes,
    const std::un...`
  - `read_kokorovoice_bytes` (function, line 636) `void read_kokorovoice_bytes(const uint8_t* data, size_t size,
                            std::st...`
  - `read_kokorovoice` (function, line 669) `void read_kokorovoice(const std::filesystem::path& path,
                      std::vector<float>...`
  - `kokoro_tts_lang_supported` (function, line 685) `bool kokoro_tts_lang_supported(std::string_view lang_cli,
                               const Mo...`
  - `ascii_lowercase_copy` (function, line 690) `std::string ascii_lowercase_copy(std::string_view s)`
  - `tts_map_path` (function, line 700) `std::filesystem::path tts_map_path(const FileInformationMap& m,
                                 ...`
  - `make_piper_options` (function, line 710) `PiperTTSOptions make_piper_options(std::string_view language,
                                   ...`
  - `kokoro_vocoder_dependency_keys_with_options` (function, line 760) `std::vector<std::string> kokoro_vocoder_dependency_keys_with_options(
    std::string_view langua...`
  - `piper_vocoder_dependency_keys_with_options` (function, line 866) `std::vector<std::string> piper_vocoder_dependency_keys_with_options(
    std::string_view languag...`
  - `make_zipvoice_options` (function, line 886) `ZipVoiceTTSOptions make_zipvoice_options(std::string_view language,
                             ...`
  - `zipvoice_vocoder_dependency_keys` (function, line 915) `std::vector<std::string> zipvoice_vocoder_dependency_keys()`
  - `zipvoice_asset_present` (function, line 923) `bool zipvoice_asset_present(const MoonshineTTSOptions& opt,
                            std::stri...`
  - `zipvoice_assets_available` (function, line 940) `bool zipvoice_assets_available(const MoonshineTTSOptions& opt)`
  - `detect_kokoro_style_input_name` (function, line 1000) `void detect_kokoro_style_input_name()`
  - `detect_speed_input_element_type` (function, line 1011) `void detect_speed_input_element_type()`
  - `speed` (function, line 1028) `double speed() const`
  - `set_speed` (function, line 1030) `void set_speed(double s)`
  - `normalize_audio` (function, line 1038) `bool normalize_audio() const`
  - `set_normalize_audio` (function, line 1039) `void set_normalize_audio(bool on)`
  - `output_volume` (function, line 1040) `float output_volume() const`
  - `set_output_volume` (function, line 1041) `void set_output_volume(float v)`
  - `KokoroTtsEngine` (function, line 1043) `explicit KokoroTtsEngine(std::string_view language, MoonshineTTSOptions opt)`
  - `reload_voice_tensor` (function, line 1158) `void reload_voice_tensor()`
  - `synthesize` (function, line 1199) `std::vector<float> synthesize(std::string_view text)`
  - `synthesize_from_ipa` (function, line 1210) `std::vector<float> synthesize_from_ipa(std::string_view ipa)`
  - `Impl` (function, line 1330) `explicit Impl(std::string_view language, const MoonshineTTSOptions& opt_in)`
  - `synthesize_unlocked` (function, line 1395) `std::vector<float> synthesize_unlocked(std::string_view text)`
  - `synthesize_from_phonemes_unlocked` (function, line 1412) `std::vector<float> synthesize_from_phonemes_unlocked(
      std::string_view phonemes)`
  - `synthesize` (function, line 1423) `std::vector<float> synthesize(std::string_view text)`
  - `synthesize_from_phonemes` (function, line 1428) `std::vector<float> synthesize_from_phonemes(std::string_view phonemes)`
  - `synthesize_from_phonemes_with_overrides` (function, line 1433) `std::vector<float> synthesize_from_phonemes_with_overrides(
      std::string_view phonemes, cons...`
  - `synthesize_with_overrides` (function, line 1439) `std::vector<float> synthesize_with_overrides(std::string_view text,
                             ...`
  - `run_with_overrides` (function, line 1449) `template <typename Produce>
  std::vector<float> run_with_overrides(const SynthesisOverrides& ov,...`
  - `MoonshineTTS` (function, line 1503) `MoonshineTTS::MoonshineTTS(std::string_view language,
                           const MoonshineT...`
  - `synthesize` (function, line 1512) `std::vector<float> MoonshineTTS::synthesize(std::string_view text)`
  - `synthesize` (function, line 1516) `std::vector<float> MoonshineTTS::synthesize(
    std::string_view text,
    const std::vector<std...`
  - `synthesize_from_phonemes` (function, line 1530) `std::vector<float> MoonshineTTS::synthesize_from_phonemes(
    std::string_view phonemes)`
  - `synthesize_from_phonemes` (function, line 1535) `std::vector<float> MoonshineTTS::synthesize_from_phonemes(
    std::string_view phonemes,
    con...`
  - `write_wav_mono_pcm16` (function, line 1549) `void write_wav_mono_pcm16(const std::filesystem::path& path,
                          const std:...`
  - `moonshine_catalog_tts_vocoder_only_dependency_keys` (function, line 1612) `std::vector<std::string> moonshine_catalog_tts_vocoder_only_dependency_keys(
    std::string_view...`
  - `moonshine_catalog_tts_vocoder_only_dependency_keys` (function, line 1639) `std::vector<std::string> moonshine_catalog_tts_vocoder_only_dependency_keys(
    std::string_view...`
  - `moonshine_catalog_all_tts_vocoder_dependency_keys_union` (function, line 1646) `std::vector<std::string>
moonshine_catalog_all_tts_vocoder_dependency_keys_union()`
  - `moonshine_list_tts_voices_with_availability` (function, line 1663) `std::vector<MoonshineTtsVoiceAvailability>
moonshine_list_tts_voices_with_availability(std::strin...`
  - `sort` (function, line 1718) `std::sort(
        out.begin(), out.end(),
        [](const MoonshineTtsVoiceAvailability& a,
   ...`
  - `tmp` (function, line 45) `const std::string tmp(s);`
  - `req` (function, line 384) `const std::string req(requested);`
  - `def` (function, line 397) `const std::string def(default_voice);`
  - `cand` (function, line 406) `const std::string cand(vid);`
  - `buf` (function, line 677) `std::vector<uint8_t> buf((std::istreambuf_iterator<char>(f)), std::istreambuf_iterator<char>());`
  - `k` (function, line 702) `const std::string k(canonical_key);`
  - `onnx_key` (function, line 714) `const std::string onnx_key(kTtsPiperOnnxKey);`
  - `onnx_json_key` (function, line 721) `const std::string onnx_json_key(kTtsPiperOnnxJsonKey);`
  - `pv_key` (function, line 729) `const std::string pv_key(kTtsPiperVoicesKey);`
  - `pvj_key` (function, line 737) `const std::string pvj_key(kTtsPiperVoicesJsonKey);`
  - `id` (function, line 810) `const std::string id(vid);`
  - `json_key` (function, line 869) `const std::string json_key(kTtsPiperOnnxJsonKey);`
  - `cfg_str` (function, line 1089) `const std::string cfg_str(reinterpret_cast<const char*>(cfg_buf), cfg_len);`
  - `ref_row` (function, line 1262) `std::vector<float> ref_row(voice_cols_);`
  - `pcm` (function, line 1557) `std::vector<int16_t> pcm(samples.size());`
- Depends on: `core/moonshine-tts/src/g2p-path.h`, `core/moonshine-tts/src/moonshine-asset-catalog.h`, `core/moonshine-tts/src/moonshine-g2p.h`, `core/moonshine-tts/src/moonshine-tts.h`, `core/moonshine-tts/src/ort-onnx-external-data.h`, `core/moonshine-tts/src/ort-session-options.h`, `core/moonshine-tts/src/piper-tts.h`, `core/moonshine-tts/src/utf8-utils.h`, `core/moonshine-tts/src/zipvoice-tts.h`, `core/moonshine-tts/src/zipvoice-voices.h`, `core/moonshine-utils/debug-utils.h`, `core/moonshine-utils/string-utils.h`

## core/moonshine-tts/src/moonshine-tts.h
- Doc: MoonshineTTS: Unified TTS: **Kokoro** and **Piper** ONNX backends; shared ``MoonshineG2P`` where...
- Layer: utility
- Language: h
- Symbols:
  - `Impl` (struct, line 60)
  - `MoonshineTtsVoiceAvailability` (struct, line 86)
  - `MoonshineTTS` (class, line 22)
  - `synthesize` (function, line 33) `std::vector<float> synthesize(std::string_view text);`
  - `synthesize_from_phonemes` (function, line 50) `std::vector<float> synthesize_from_phonemes(std::string_view phonemes);`
  - `write_wav_mono_pcm16` (function, line 64) `void write_wav_mono_pcm16(const std::filesystem::path& path, const std::vector<float>& samples);`
  - `MOONSHINE_TTS_MOONSHINE_TTS_H` (macro, line 2) `#define MOONSHINE_TTS_MOONSHINE_TTS_H`
- Depends on: `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-tts/src/moonshine-tts-options.h`
- Imported by: `core/moonshine-c-api.cpp`, `core/moonshine-tts/src/moonshine-tts.cpp`, `core/moonshine-tts/tests/moonshine-tts-speed-test.cpp`, `core/moonshine-tts/tools/moonshine-tts-cli.cpp`, `core/moonshine-tts/tools/piper-phoneme-infer-cli.cpp`

## core/moonshine-tts/src/ort-onnx-external-data.cpp
- Layer: data_access
- Language: cpp
- Symbols:
  - `ort_add_external_initializer_files_for_onnx_model_buffer` (function, line 10) `void ort_add_external_initializer_files_for_onnx_model_buffer(
    Ort::SessionOptions& opts, con...`
- Depends on: `core/moonshine-tts/src/ort-onnx-external-data.h`

## core/moonshine-tts/src/ort-onnx-external-data.h
- Doc: ort_add_external_initializer_files_for_onnx_model_buffer: If ``files`` contains an in-memory...
- Layer: data_access
- Language: h
- Symbols:
  - `ort_add_external_initializer_files_for_onnx_model_buffer` (function, line 18) `void ort_add_external_initializer_files_for_onnx_model_buffer( Ort::SessionOptions& opts, const FileInformationMap&...`
  - `MOONSHINE_TTS_ORT_ONNX_EXTERNAL_DATA_H` (macro, line 2) `#define MOONSHINE_TTS_ORT_ONNX_EXTERNAL_DATA_H`
- Depends on: `core/moonshine-tts/src/file-information.h`
- Imported by: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp`, `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp`, `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp`, `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp`, `core/moonshine-tts/src/moonshine-tts.cpp`, `core/moonshine-tts/src/ort-onnx-external-data.cpp`, `core/moonshine-tts/src/piper-tts.cpp`, `core/moonshine-tts/src/zipvoice-tts.cpp`


Next: [KB_core_moonshine-tts_src_p2.md](KB_core_moonshine-tts_src_p2.md)
