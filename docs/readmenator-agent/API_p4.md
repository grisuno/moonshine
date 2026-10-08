# API (page 4 of 10)
Previous: [API_p3.md](API_p3.md)

## core/moonshine-tts/src/lang-specific/portuguese-rules.cpp
Depends on: `core/moonshine-tts/src/lang-specific/ipa-symbols.h`, `core/moonshine-tts/src/lang-specific/portuguese-rules.h`, `core/moonshine-tts/src/utf8-utils.h`
- `pt_tolower` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:24` `char32_t pt_tolower(char32_t c)`
- `is_pt_key_cp` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:69` `bool is_pt_key_cp(char32_t c)`
- `normalize_lookup_key_utf8_impl` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:85` `std::string normalize_lookup_key_utf8_impl(const std::string& word)`
- `normalize_lookup_key_utf8` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:106` `std::string normalize_lookup_key_utf8(const std::string& word)`
- `utf8_to_u32_pt` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:110` `std::u32string utf8_to_u32_pt(const std::string& s)`
- `u32_to_utf8_pt` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:114` `std::string u32_to_utf8_pt(const std::u32string& s)`
- `is_allowed_pt_grapheme` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:122` `bool is_allowed_pt_grapheme(char32_t c)`
- `filter_pt_word_graphemes_utf8` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:135` `std::u32string filter_pt_word_graphemes_utf8(const std::string& word)`
- `is_vowel_pt_u32` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:151` `bool is_vowel_pt_u32(char32_t ch)`
- `strip_accent_base_pt` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:159` `char32_t strip_accent_base_pt(char32_t c)`
- `should_hiatus_pt_u32` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:186` `bool should_hiatus_pt_u32(char32_t a, char32_t b)`
- `valid_onset2_end_u32` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:261` `bool valid_onset2_end_u32(char32_t a, char32_t b)`
- `port_orthographic_syllables_u32` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:297` `std::vector<std::u32string> port_orthographic_syllables_u32(
    const std::u32string& w0)`
- `accented_syllable_u32` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:352` `bool accented_syllable_u32(const std::u32string& s)`
- `default_stressed_syllable_index_u32` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:362` `size_t default_stressed_syllable_index_u32(
    const std::vector<std::u32string>& syls, const st...`
- `strip_stress_chars` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:424` `std::string strip_stress_chars(std::string s)`
- `insert_primary_stress_before_vowel_utf8` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:430` `std::string insert_primary_stress_before_vowel_utf8(std::string ipa)`
- `roman_to_int_ascii` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:453` `std::optional<int> roman_to_int_ascii(std::string_view u)`
- `roman_numeral_token_to_ipa` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:491` `std::optional<std::string> roman_numeral_token_to_ipa(
    const std::string& letters_lower, bool...`
- `prev_global_vowel_u32` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:549` `bool prev_global_vowel_u32(const std::u32string& full_word, size_t gidx)`
- `next_global_vowel_u32` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:569` `bool next_global_vowel_u32(const std::u32string& full_word, size_t gidx)`
- `syllable_has_u32` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:585` `bool syllable_has_u32(const std::u32string& s, char32_t ch)`
- `letters_to_ipa_no_stress_u32` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:589` `std::string letters_to_ipa_no_stress_u32(const std::u32string& s, bool is_pt_pt,
                ...`
- `rules_word_to_ipa_single_u32` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:964` `std::string rules_word_to_ipa_single_u32(const std::u32string& wl,
                              ...`
- `vowel_grapheme_tail_pt` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:1018` `bool vowel_grapheme_tail_pt(char32_t c)`
- `pt_pt_apply_rules_final_s_to_esh` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:1026` `std::string pt_pt_apply_rules_final_s_to_esh(std::string ipa,
                                   ...`
- `rules_word_to_ipa_utf8` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:1161` `std::string rules_word_to_ipa_utf8(const std::string& raw, bool is_pt_pt,
                       ...`

## core/moonshine-tts/src/lang-specific/portuguese-rules.h
Imported by: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp`, `core/moonshine-tts/src/lang-specific/portuguese.cpp`
- `pt_tolower` (function) `core/moonshine-tts/src/lang-specific/portuguese-rules.h:11` `char32_t pt_tolower(char32_t c);`

## core/moonshine-tts/src/moonshine-asset-catalog.cpp
Depends on: `core/moonshine-tts/src/moonshine-asset-catalog.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-tts/src/utf8-utils.h`
- `normalize_lang_key_cli` (function) `core/moonshine-tts/src/moonshine-asset-catalog.cpp:16` `std::string normalize_lang_key_cli(std::string_view raw)`
- `hyphen_to_underscore` (function) `core/moonshine-tts/src/moonshine-asset-catalog.cpp:30` `std::string hyphen_to_underscore(std::string s)`
- `english_g2p_keys` (function) `core/moonshine-tts/src/moonshine-asset-catalog.cpp:39` `std::vector<std::string> english_g2p_keys()`
- `chinese_g2p_keys` (function) `core/moonshine-tts/src/moonshine-asset-catalog.cpp:48` `std::vector<std::string> chinese_g2p_keys()`
- `japanese_g2p_keys` (function) `core/moonshine-tts/src/moonshine-asset-catalog.cpp:58` `std::vector<std::string> japanese_g2p_keys()`
- `korean_g2p_keys` (function) `core/moonshine-tts/src/moonshine-asset-catalog.cpp:68` `std::vector<std::string> korean_g2p_keys()`
- `arabic_g2p_keys` (function) `core/moonshine-tts/src/moonshine-asset-catalog.cpp:74` `std::vector<std::string> arabic_g2p_keys()`
- `french_g2p_keys` (function) `core/moonshine-tts/src/moonshine-asset-catalog.cpp:84` `std::vector<std::string> french_g2p_keys()`
- `lookup_g2p_dependency_keys` (function) `core/moonshine-tts/src/moonshine-asset-catalog.cpp:223` `std::optional<std::vector<std::string>> lookup_g2p_dependency_keys(
    std::string_view raw)`
- `moonshine_asset_catalog_populate_default_g2p_files` (function) `core/moonshine-tts/src/moonshine-asset-catalog.cpp:240` `void moonshine_asset_catalog_populate_default_g2p_files(
    FileInformationMap& files)`
- `moonshine_asset_catalog_g2p_dependency_keys` (function) `core/moonshine-tts/src/moonshine-asset-catalog.cpp:249` `std::optional<std::vector<std::string>>
moonshine_asset_catalog_g2p_dependency_keys(std::string_v...`
- `moonshine_asset_catalog_all_g2p_dependency_keys_union` (function) `core/moonshine-tts/src/moonshine-asset-catalog.cpp:254` `std::vector<std::string>
moonshine_asset_catalog_all_g2p_dependency_keys_union()`
- `moonshine_asset_catalog_all_registered_language_tags` (function) `core/moonshine-tts/src/moonshine-asset-catalog.cpp:268` `std::vector<std::string>
moonshine_asset_catalog_all_registered_language_tags()`

## core/moonshine-tts/src/moonshine-asset-catalog.h
Depends on: `core/moonshine-tts/src/file-information.h`
Imported by: `core/moonshine-c-api.cpp`, `core/moonshine-tts/src/moonshine-asset-catalog.cpp`, `core/moonshine-tts/src/moonshine-g2p-options.cpp`, `core/moonshine-tts/src/moonshine-tts.cpp`
- `moonshine_asset_catalog_populate_default_g2p_files` (function) `core/moonshine-tts/src/moonshine-asset-catalog.h:15` `void moonshine_asset_catalog_populate_default_g2p_files( FileInformationMap& files);` -- Fills ``files`` with default canonical G2P paths (union of all per-language G2P dependencies).

## core/moonshine-tts/src/moonshine-g2p-options.cpp
Depends on: `core/moonshine-tts/src/g2p-path.h`, `core/moonshine-tts/src/moonshine-asset-catalog.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-utils/string-utils.h`, `core/ort-utils/ort-utils.h`
- `optional_path_from_string` (function) `core/moonshine-tts/src/moonshine-g2p-options.cpp:15` `std::optional<std::filesystem::path> optional_path_from_string(
    const std::string& value)`
- `set_canonical_file` (function) `core/moonshine-tts/src/moonshine-g2p-options.cpp:24` `void set_canonical_file(FileInformationMap& files,
                        std::string_view canon...`
- `set_override_file` (function) `core/moonshine-tts/src/moonshine-g2p-options.cpp:35` `void set_override_file(FileInformationMap& files, std::string_view map_key,
                     ...`
- `is_known_g2p_option` (function) `core/moonshine-tts/src/moonshine-g2p-options.cpp:45` `bool is_known_g2p_option(std::string_view key)`
- `prepare_g2p_file_information_path` (function) `core/moonshine-tts/src/moonshine-g2p-options.cpp:108` `void prepare_g2p_file_information_path(FileInformation& fi,
                                     ...`
- `MoonshineG2POptions` (function) `core/moonshine-tts/src/moonshine-g2p-options.cpp:132` `MoonshineG2POptions::MoonshineG2POptions()`
- `relative_asset_path` (function) `core/moonshine-tts/src/moonshine-g2p-options.cpp:136` `std::filesystem::path MoonshineG2POptions::relative_asset_path(
    std::string_view canonical_ke...`
- `k` (function) `core/moonshine-tts/src/moonshine-g2p-options.cpp:138` `const std::string k(canonical_key);`
- `optional_override_path` (function) `core/moonshine-tts/src/moonshine-g2p-options.cpp:147` `std::optional<std::filesystem::path>
MoonshineG2POptions::optional_override_path(std::string_view...`
- `asset_is_available` (function) `core/moonshine-tts/src/moonshine-g2p-options.cpp:159` `bool MoonshineG2POptions::asset_is_available(
    std::string_view canonical_key) const`
- `read_binary_asset` (function) `core/moonshine-tts/src/moonshine-g2p-options.cpp:175` `std::vector<uint8_t> MoonshineG2POptions::read_binary_asset(
    std::string_view canonical_key) ...`
- `out` (function) `core/moonshine-tts/src/moonshine-g2p-options.cpp:188` `std::vector<uint8_t> out(p, p + n);`
- `read_utf8_asset` (function) `core/moonshine-tts/src/moonshine-g2p-options.cpp:193` `std::string MoonshineG2POptions::read_utf8_asset(
    std::string_view canonical_key) const`
- `parse_options` (function) `core/moonshine-tts/src/moonshine-g2p-options.cpp:199` `void MoonshineG2POptions::parse_options(
    const std::vector<std::pair<std::string, std::string...`

## core/moonshine-tts/src/moonshine-g2p-options.h
Depends on: `core/moonshine-tts/src/file-information.h`
Imported by: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp`, `core/moonshine-tts/src/lang-specific/arabic.cpp`, `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp`, `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp`, `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp`, `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp`, `core/moonshine-tts/src/lang-specific/japanese.cpp`, `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp`, `core/moonshine-tts/src/moonshine-asset-catalog.cpp`, `core/moonshine-tts/src/moonshine-g2p-options.cpp`, `core/moonshine-tts/src/moonshine-g2p.h`, `core/moonshine-tts/src/moonshine-tts-options.h`, `core/moonshine-tts/src/moonshine-tts.h`, `core/moonshine-tts/src/piper-tts.h`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.h`, `core/moonshine-tts/src/zipvoice-tts.h`, `core/moonshine-tts/tests/moonshine-g2p-options-test.cpp`
- `g2p_bundle_file_key` (function) `core/moonshine-tts/src/moonshine-g2p-options.h:18` `inline std::string g2p_bundle_file_key(std::string_view bundle_dir_key,
                         ...` -- ``<bundle_dir_key>/<filename>`` for ``FileInformationMap`` / ``read_*_asset``.
- `asset_is_available` (function) `core/moonshine-tts/src/moonshine-g2p-options.h:186` `bool asset_is_available(std::string_view canonical_key) const;` -- True if the asset has a client buffer or exists on disk under ``g2p_root`` (canonical key or map key).
- `read_binary_asset` (function) `core/moonshine-tts/src/moonshine-g2p-options.h:190` `std::vector<uint8_t> read_binary_asset(std::string_view canonical_key) const;` -- Full file contents via ``FileInformation::load`` (memory buffer or disk).
- `parse_options` (function) `core/moonshine-tts/src/moonshine-g2p-options.h:198` `void parse_options( const std::vector<std::pair<std::string, std::string>>& options);`

## core/moonshine-tts/src/moonshine-g2p.cpp
Depends on: `core/moonshine-tts/src/lang-specific/arabic.h`, `core/moonshine-tts/src/lang-specific/chinese.h`, `core/moonshine-tts/src/lang-specific/dutch.h`, `core/moonshine-tts/src/lang-specific/english.h`, `core/moonshine-tts/src/lang-specific/french.h`, `core/moonshine-tts/src/lang-specific/german.h`, `core/moonshine-tts/src/lang-specific/hindi.h`, `core/moonshine-tts/src/lang-specific/italian.h`, `core/moonshine-tts/src/lang-specific/japanese.h`, `core/moonshine-tts/src/lang-specific/korean.h`, `core/moonshine-tts/src/lang-specific/portuguese.h`, `core/moonshine-tts/src/lang-specific/russian.h`, `core/moonshine-tts/src/lang-specific/spanish.h`, `core/moonshine-tts/src/lang-specific/turkish.h`, `core/moonshine-tts/src/lang-specific/ukrainian.h`, `core/moonshine-tts/src/lang-specific/vietnamese.h`, `core/moonshine-tts/src/moonshine-g2p.h`, `core/moonshine-tts/src/rule-based-g2p-factory.h`, `core/moonshine-tts/src/rule-based-g2p.h`, `core/moonshine-tts/src/utf8-utils.h`, `core/moonshine-utils/debug-utils.h`
- `trim_copy` (function) `core/moonshine-tts/src/moonshine-g2p.cpp:31` `std::string trim_copy(std::string_view s)`
- `normalize_spanish_dialect_cli_key` (function) `core/moonshine-tts/src/moonshine-g2p.cpp:45` `std::string normalize_spanish_dialect_cli_key(std::string_view raw)` -- Normalize user input like ``es_ar`` / ``es-mx`` to keys accepted by ``spanish_dialect_from_cli_id`` (e.g.
- `rule_backend_name` (function) `core/moonshine-tts/src/moonshine-g2p.cpp:68` `const char* rule_backend_name(RuleBasedG2pKind k)`
- `dialect_resolves_to_spanish_rules` (function) `core/moonshine-tts/src/moonshine-g2p.cpp:108` `bool dialect_resolves_to_spanish_rules(std::string_view dialect_id,
                             ...`
- `dialect_uses_rule_based_g2p` (function) `core/moonshine-tts/src/moonshine-g2p.cpp:122` `bool dialect_uses_rule_based_g2p(std::string_view dialect_id,
                                 co...`
- `MoonshineG2P` (function) `core/moonshine-tts/src/moonshine-g2p.cpp:186` `MoonshineG2P::MoonshineG2P(std::string dialect_id,
                           MoonshineG2POptions...`
- `text_to_ipa` (function) `core/moonshine-tts/src/moonshine-g2p.cpp:217` `std::string MoonshineG2P::text_to_ipa(std::string_view text,
                                    ...`

## core/moonshine-tts/src/moonshine-g2p.h
Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-tts/src/rule-based-g2p-factory.h`
Imported by: `core/moonshine-c-api.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/moonshine-tts.cpp`, `core/moonshine-tts/src/piper-tts.cpp`, `core/moonshine-tts/src/zipvoice-tts.cpp`, `core/moonshine-tts/tests/chinese-rule-g2p-test.cpp`, `core/moonshine-tts/tests/korean-rule-g2p-test.cpp`, `core/moonshine-tts/tests/onnx-g2p-smoke-test.cpp`, `core/moonshine-tts/tests/russian-rule-g2p-test.cpp`, `core/moonshine-tts/tests/vietnamese-rule-g2p-test.cpp`, `core/moonshine-tts/tools/moonshine-g2p-cli.cpp`
- `dialect_resolves_to_spanish_rules` (function) `core/moonshine-tts/src/moonshine-g2p.h:20` `bool dialect_resolves_to_spanish_rules(std::string_view dialect_id, bool spanish_narrow_obstruents = true);` -- True if *dialect_id* maps to the built-in Spanish rule engine (e.g.
- `uses_spanish_rules` (function) `core/moonshine-tts/src/moonshine-g2p.h:48` `bool uses_spanish_rules() const`
- `uses_german_rules` (function) `core/moonshine-tts/src/moonshine-g2p.h:51` `bool uses_german_rules() const`
- `uses_french_rules` (function) `core/moonshine-tts/src/moonshine-g2p.h:54` `bool uses_french_rules() const`
- `uses_dutch_rules` (function) `core/moonshine-tts/src/moonshine-g2p.h:57` `bool uses_dutch_rules() const`
- `uses_italian_rules` (function) `core/moonshine-tts/src/moonshine-g2p.h:60` `bool uses_italian_rules() const`
- `uses_russian_rules` (function) `core/moonshine-tts/src/moonshine-g2p.h:63` `bool uses_russian_rules() const`
- `uses_chinese_rules` (function) `core/moonshine-tts/src/moonshine-g2p.h:66` `bool uses_chinese_rules() const`
- `uses_korean_rules` (function) `core/moonshine-tts/src/moonshine-g2p.h:69` `bool uses_korean_rules() const`
- `uses_vietnamese_rules` (function) `core/moonshine-tts/src/moonshine-g2p.h:72` `bool uses_vietnamese_rules() const`
- `uses_japanese_rules` (function) `core/moonshine-tts/src/moonshine-g2p.h:75` `bool uses_japanese_rules() const`
- `uses_arabic_rules` (function) `core/moonshine-tts/src/moonshine-g2p.h:78` `bool uses_arabic_rules() const`
- `uses_portuguese_rules` (function) `core/moonshine-tts/src/moonshine-g2p.h:81` `bool uses_portuguese_rules() const`
- `uses_turkish_rules` (function) `core/moonshine-tts/src/moonshine-g2p.h:84` `bool uses_turkish_rules() const`
- `uses_ukrainian_rules` (function) `core/moonshine-tts/src/moonshine-g2p.h:87` `bool uses_ukrainian_rules() const`
- `uses_hindi_rules` (function) `core/moonshine-tts/src/moonshine-g2p.h:90` `bool uses_hindi_rules() const`
- `uses_english_rules` (function) `core/moonshine-tts/src/moonshine-g2p.h:93` `bool uses_english_rules() const`
- `uses_onnx` (function) `core/moonshine-tts/src/moonshine-g2p.h:99` `static constexpr bool uses_onnx()` -- Always false: full-bundle ONNX G2P was removed; English may still load OOV ONNX inside ``EnglishRuleG2p``.
- `dialect_id` (function) `core/moonshine-tts/src/moonshine-g2p.h:103` `const std::string& dialect_id() const` -- Canonical dialect id (e.g.

## core/moonshine-tts/src/moonshine-tts-options.cpp
Depends on: `core/moonshine-tts/src/moonshine-tts-options.h`, `core/moonshine-utils/string-utils.h`, `core/ort-utils/ort-utils.h`
- `apply_synthesis_output_effects` (function) `core/moonshine-tts/src/moonshine-tts-options.cpp:13` `void apply_synthesis_output_effects(std::vector<float>& audio,
                                  ...`
- `MoonshineTTSOptions` (function) `core/moonshine-tts/src/moonshine-tts-options.cpp:39` `MoonshineTTSOptions::MoonshineTTSOptions()`
- `apply_voice_engine_prefix` (function) `core/moonshine-tts/src/moonshine-tts-options.cpp:46` `void MoonshineTTSOptions::apply_voice_engine_prefix()`
- `tts_relative_path` (function) `core/moonshine-tts/src/moonshine-tts-options.cpp:72` `std::filesystem::path MoonshineTTSOptions::tts_relative_path(
    std::string_view canonical_key)...`
- `k` (function) `core/moonshine-tts/src/moonshine-tts-options.cpp:74` `const std::string k(canonical_key);`
- `parse_options` (function) `core/moonshine-tts/src/moonshine-tts-options.cpp:82` `void MoonshineTTSOptions::parse_options(
    const std::vector<std::pair<std::string, std::string...`
- `d` (function) `core/moonshine-tts/src/moonshine-tts-options.cpp:121` `const std::filesystem::path d(t);`

## core/moonshine-tts/src/moonshine-tts-options.h
Depends on: `core/moonshine-tts/src/file-information.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`
Imported by: `core/moonshine-tts/src/moonshine-tts-options.cpp`, `core/moonshine-tts/src/moonshine-tts.h`, `core/moonshine-tts/src/piper-tts.cpp`, `core/moonshine-tts/src/zipvoice-tts.cpp`, `core/moonshine-tts/tests/moonshine-tts-options-test.cpp`
- `parse_options` (function) `core/moonshine-tts/src/moonshine-tts-options.h:134` `void parse_options( const std::vector<std::pair<std::string, std::string>>& options, std::string* cli_language =...` -- throws.
- `apply_voice_engine_prefix` (function) `core/moonshine-tts/src/moonshine-tts-options.h:142` `void apply_voice_engine_prefix();` -- If ``voice`` starts with ``kokoro_`` or ``piper_`` (ASCII case-insensitive), sets ``vocoder_engine`` accordingly and...
- `apply_synthesis_output_effects` (function) `core/moonshine-tts/src/moonshine-tts-options.h:149` `void apply_synthesis_output_effects(std::vector<float>& audio, bool normalize_audio, float volume);` -- Shared post-synthesis effects step for Kokoro and Piper output.

## core/moonshine-tts/src/moonshine-tts.cpp
Depends on: `core/moonshine-tts/src/g2p-path.h`, `core/moonshine-tts/src/moonshine-asset-catalog.h`, `core/moonshine-tts/src/moonshine-g2p.h`, `core/moonshine-tts/src/moonshine-tts.h`, `core/moonshine-tts/src/ort-onnx-external-data.h`, `core/moonshine-tts/src/ort-session-options.h`, `core/moonshine-tts/src/piper-tts.h`, `core/moonshine-tts/src/utf8-utils.h`, `core/moonshine-tts/src/zipvoice-tts.h`, `core/moonshine-tts/src/zipvoice-voices.h`, `core/moonshine-utils/debug-utils.h`, `core/moonshine-utils/string-utils.h`
- `utf8_nfc` (function) `core/moonshine-tts/src/moonshine-tts.cpp:44` `std::string utf8_nfc(std::string_view s)`
- `tmp` (function) `core/moonshine-tts/src/moonshine-tts.cpp:45` `const std::string tmp(s);`
- `replace_utf8` (function) `core/moonshine-tts/src/moonshine-tts.cpp:56` `void replace_utf8(std::string& s, std::string_view old_s,
                  std::string_view new_s)`
- `empty` (function) `core/moonshine-tts/src/moonshine-tts.cpp:75` `bool empty() const`
- `parse_synthesis_overrides_from_pairs` (function) `core/moonshine-tts/src/moonshine-tts.cpp:81` `SynthesisOverrides parse_synthesis_overrides_from_pairs(
    const std::vector<std::pair<std::str...`
- `py_isspace_utf8_ch` (function) `core/moonshine-tts/src/moonshine-tts.cpp:98` `bool py_isspace_utf8_ch(std::string_view ch)`
- `collapse_whitespace_join_single_space` (function) `core/moonshine-tts/src/moonshine-tts.cpp:116` `std::string collapse_whitespace_join_single_space(const std::string& s)`
- `normalize_lang_key` (function) `core/moonshine-tts/src/moonshine-tts.cpp:144` `std::string normalize_lang_key(std::string_view raw)`
- `lookup_lang_profile` (function) `core/moonshine-tts/src/moonshine-tts.cpp:166` `const LangProfile* lookup_lang_profile(std::string_view key)`
- `resolve_lang_for_tts` (function) `core/moonshine-tts/src/moonshine-tts.cpp:202` `void resolve_lang_for_tts(const std::string& lk, const MoonshineG2POptions& opt,
                ...` -- Fills *profile* and *g2p_dialect* for ``MoonshineG2P`` (Kokoro locale + rule-based tag).
- `kokoro_tts_lang_supported_inner` (function) `core/moonshine-tts/src/moonshine-tts.cpp:220` `bool kokoro_tts_lang_supported_inner(std::string_view lang_cli,
                                 ...`
- `voice_prefix_ok` (function) `core/moonshine-tts/src/moonshine-tts.cpp:231` `bool voice_prefix_ok(char kokoro_lang, std::string_view voice)`
- `maybe_align_en_profile_for_kokoro_voice` (function) `core/moonshine-tts/src/moonshine-tts.cpp:252` `void maybe_align_en_profile_for_kokoro_voice(std::string_view voice,
                            ...` -- If ``--lang`` is US English but the user asked for a British Kokoro voice id (``bf_*`` / ``bm_*``), or the reverse...
- `infer_lang_profile_from_kokoro_voice` (function) `core/moonshine-tts/src/moonshine-tts.cpp:275` `bool infer_lang_profile_from_kokoro_voice(std::string_view voice_sv,
                            ...` -- When the CLI language is not a Kokoro-backed locale (e.g.
- `resolve_lang_for_kokoro` (function) `core/moonshine-tts/src/moonshine-tts.cpp:302` `void resolve_lang_for_kokoro(const std::string& lk,
                             const MoonshineG...` -- Like ``resolve_lang_for_tts`` for Kokoro paths, but if *lk* is not Kokoro-capable (Piper-only language), fall back...
- `kokoro_voice_asset_exists` (function) `core/moonshine-tts/src/moonshine-tts.cpp:316` `bool kokoro_voice_asset_exists(const std::string& voice_id,
                               const ...`
- `select_voice_id` (function) `core/moonshine-tts/src/moonshine-tts.cpp:358` `std::string select_voice_id(char kokoro_lang, std::string_view requested,
                       ...`
- `req` (function) `core/moonshine-tts/src/moonshine-tts.cpp:384` `const std::string req(requested);`
- `def` (function) `core/moonshine-tts/src/moonshine-tts.cpp:397` `const std::string def(default_voice);`
- `cand` (function) `core/moonshine-tts/src/moonshine-tts.cpp:406` `const std::string cand(vid);`
- `apply_diphthong_map` (function) `core/moonshine-tts/src/moonshine-tts.cpp:428` `void apply_diphthong_map(std::string& s, char kokoro_lang)`
- `apply_chinese_kokoro_normalization` (function) `core/moonshine-tts/src/moonshine-tts.cpp:461` `void apply_chinese_kokoro_normalization(std::string& ipa)` -- Mandarin Chinese IPA normalization for Kokoro: Chao tone letters → arrow contour symbols, consonant mappings to...
- `normalize_ipa_to_kokoro` (function) `core/moonshine-tts/src/moonshine-tts.cpp:535` `std::string normalize_ipa_to_kokoro(
    std::string ipa, char kokoro_lang,
    const std::unorde...`
- `chunk_phonemes` (function) `core/moonshine-tts/src/moonshine-tts.cpp:557` `std::vector<std::string> chunk_phonemes(const std::string& ps,
                                  ...`
- `phoneme_str_to_input_ids` (function) `core/moonshine-tts/src/moonshine-tts.cpp:621` `std::vector<int64_t> phoneme_str_to_input_ids(
    const std::string& phonemes,
    const std::un...`
- `read_kokorovoice_bytes` (function) `core/moonshine-tts/src/moonshine-tts.cpp:636` `void read_kokorovoice_bytes(const uint8_t* data, size_t size,
                            std::st...`
- `read_kokorovoice` (function) `core/moonshine-tts/src/moonshine-tts.cpp:669` `void read_kokorovoice(const std::filesystem::path& path,
                      std::vector<float>...`
- `buf` (function) `core/moonshine-tts/src/moonshine-tts.cpp:677` `std::vector<uint8_t> buf((std::istreambuf_iterator<char>(f)), std::istreambuf_iterator<char>());`
- `kokoro_tts_lang_supported` (function) `core/moonshine-tts/src/moonshine-tts.cpp:685` `bool kokoro_tts_lang_supported(std::string_view lang_cli,
                               const Mo...`
- `ascii_lowercase_copy` (function) `core/moonshine-tts/src/moonshine-tts.cpp:690` `std::string ascii_lowercase_copy(std::string_view s)`
- `tts_map_path` (function) `core/moonshine-tts/src/moonshine-tts.cpp:700` `std::filesystem::path tts_map_path(const FileInformationMap& m,
                                 ...`
- `k` (function) `core/moonshine-tts/src/moonshine-tts.cpp:702` `const std::string k(canonical_key);`
- `make_piper_options` (function) `core/moonshine-tts/src/moonshine-tts.cpp:710` `PiperTTSOptions make_piper_options(std::string_view language,
                                   ...`
- `onnx_key` (function) `core/moonshine-tts/src/moonshine-tts.cpp:714` `const std::string onnx_key(kTtsPiperOnnxKey);`
- `onnx_json_key` (function) `core/moonshine-tts/src/moonshine-tts.cpp:721` `const std::string onnx_json_key(kTtsPiperOnnxJsonKey);`
- `pv_key` (function) `core/moonshine-tts/src/moonshine-tts.cpp:729` `const std::string pv_key(kTtsPiperVoicesKey);`
- `pvj_key` (function) `core/moonshine-tts/src/moonshine-tts.cpp:737` `const std::string pvj_key(kTtsPiperVoicesJsonKey);`
- `kokoro_vocoder_dependency_keys_with_options` (function) `core/moonshine-tts/src/moonshine-tts.cpp:760` `std::vector<std::string> kokoro_vocoder_dependency_keys_with_options(
    std::string_view langua...`
- `id` (function) `core/moonshine-tts/src/moonshine-tts.cpp:810` `const std::string id(vid);`
- `piper_vocoder_dependency_keys_with_options` (function) `core/moonshine-tts/src/moonshine-tts.cpp:866` `std::vector<std::string> piper_vocoder_dependency_keys_with_options(
    std::string_view languag...`
- `json_key` (function) `core/moonshine-tts/src/moonshine-tts.cpp:869` `const std::string json_key(kTtsPiperOnnxJsonKey);`
- `make_zipvoice_options` (function) `core/moonshine-tts/src/moonshine-tts.cpp:886` `ZipVoiceTTSOptions make_zipvoice_options(std::string_view language,
                             ...`
- `zipvoice_vocoder_dependency_keys` (function) `core/moonshine-tts/src/moonshine-tts.cpp:915` `std::vector<std::string> zipvoice_vocoder_dependency_keys()`
- `zipvoice_asset_present` (function) `core/moonshine-tts/src/moonshine-tts.cpp:923` `bool zipvoice_asset_present(const MoonshineTTSOptions& opt,
                            std::stri...`
- `zipvoice_assets_available` (function) `core/moonshine-tts/src/moonshine-tts.cpp:940` `bool zipvoice_assets_available(const MoonshineTTSOptions& opt)`
- `detect_kokoro_style_input_name` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1000` `void detect_kokoro_style_input_name()`
- `detect_speed_input_element_type` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1011` `void detect_speed_input_element_type()`
- `speed` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1028` `double speed() const`
- `set_speed` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1030` `void set_speed(double s)`
- `normalize_audio` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1038` `bool normalize_audio() const`
- `set_normalize_audio` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1039` `void set_normalize_audio(bool on)`
- `output_volume` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1040` `float output_volume() const`
- `set_output_volume` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1041` `void set_output_volume(float v)`
- `KokoroTtsEngine` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1043` `explicit KokoroTtsEngine(std::string_view language, MoonshineTTSOptions opt)`
- `cfg_str` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1089` `const std::string cfg_str(reinterpret_cast<const char*>(cfg_buf), cfg_len);`
- `reload_voice_tensor` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1158` `void reload_voice_tensor()`
- `synthesize` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1199` `std::vector<float> synthesize(std::string_view text)`
- `synthesize_from_ipa` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1210` `std::vector<float> synthesize_from_ipa(std::string_view ipa)` -- Synthesize from an existing IPA phoneme string (skips G2P).
- `ref_row` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1262` `std::vector<float> ref_row(voice_cols_);`
- `Impl` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1330` `explicit Impl(std::string_view language, const MoonshineTTSOptions& opt_in)`
- `synthesize_unlocked` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1395` `std::vector<float> synthesize_unlocked(std::string_view text)`
- `synthesize_from_phonemes_unlocked` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1412` `std::vector<float> synthesize_from_phonemes_unlocked(
      std::string_view phonemes)`
- `synthesize` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1423` `std::vector<float> synthesize(std::string_view text)`
- `synthesize_from_phonemes` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1428` `std::vector<float> synthesize_from_phonemes(std::string_view phonemes)`
- `synthesize_from_phonemes_with_overrides` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1433` `std::vector<float> synthesize_from_phonemes_with_overrides(
      std::string_view phonemes, cons...`
- `synthesize_with_overrides` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1439` `std::vector<float> synthesize_with_overrides(std::string_view text,
                             ...`
- `run_with_overrides` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1449` `template <typename Produce>
  std::vector<float> run_with_overrides(const SynthesisOverrides& ov,...`
- `MoonshineTTS` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1503` `MoonshineTTS::MoonshineTTS(std::string_view language,
                           const MoonshineT...`
- `synthesize` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1512` `std::vector<float> MoonshineTTS::synthesize(std::string_view text)`
- `synthesize` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1516` `std::vector<float> MoonshineTTS::synthesize(
    std::string_view text,
    const std::vector<std...`
- `synthesize_from_phonemes` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1530` `std::vector<float> MoonshineTTS::synthesize_from_phonemes(
    std::string_view phonemes)`
- `synthesize_from_phonemes` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1535` `std::vector<float> MoonshineTTS::synthesize_from_phonemes(
    std::string_view phonemes,
    con...`
- `write_wav_mono_pcm16` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1549` `void write_wav_mono_pcm16(const std::filesystem::path& path,
                          const std:...`
- `pcm` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1557` `std::vector<int16_t> pcm(samples.size());`
- `moonshine_catalog_tts_vocoder_only_dependency_keys` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1612` `std::vector<std::string> moonshine_catalog_tts_vocoder_only_dependency_keys(
    std::string_view...`
- `moonshine_catalog_tts_vocoder_only_dependency_keys` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1639` `std::vector<std::string> moonshine_catalog_tts_vocoder_only_dependency_keys(
    std::string_view...`
- `moonshine_catalog_all_tts_vocoder_dependency_keys_union` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1646` `std::vector<std::string>
moonshine_catalog_all_tts_vocoder_dependency_keys_union()`
- `moonshine_list_tts_voices_with_availability` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1663` `std::vector<MoonshineTtsVoiceAvailability>
moonshine_list_tts_voices_with_availability(std::strin...`
- `sort` (function) `core/moonshine-tts/src/moonshine-tts.cpp:1718` `std::sort(
        out.begin(), out.end(),
        [](const MoonshineTtsVoiceAvailability& a,
   ...`

## core/moonshine-tts/src/moonshine-tts.h
Depends on: `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-tts/src/moonshine-tts-options.h`
Imported by: `core/moonshine-c-api.cpp`, `core/moonshine-tts/src/moonshine-tts.cpp`, `core/moonshine-tts/tests/moonshine-tts-speed-test.cpp`, `core/moonshine-tts/tools/moonshine-tts-cli.cpp`, `core/moonshine-tts/tools/piper-phoneme-infer-cli.cpp`
- `synthesize` (function) `core/moonshine-tts/src/moonshine-tts.h:33` `std::vector<float> synthesize(std::string_view text);`
- `synthesize_from_phonemes` (function) `core/moonshine-tts/src/moonshine-tts.h:50` `std::vector<float> synthesize_from_phonemes(std::string_view phonemes);` -- Synthesize from an existing IPA phoneme string, skipping grapheme-to- phoneme conversion.
- `write_wav_mono_pcm16` (function) `core/moonshine-tts/src/moonshine-tts.h:64` `void write_wav_mono_pcm16(const std::filesystem::path& path, const std::vector<float>& samples);`

## core/moonshine-tts/src/ort-onnx-external-data.cpp
Depends on: `core/moonshine-tts/src/ort-onnx-external-data.h`
- `ort_add_external_initializer_files_for_onnx_model_buffer` (function) `core/moonshine-tts/src/ort-onnx-external-data.cpp:10` `void ort_add_external_initializer_files_for_onnx_model_buffer(
    Ort::SessionOptions& opts, con...`

## core/moonshine-tts/src/ort-onnx-external-data.h
Depends on: `core/moonshine-tts/src/file-information.h`
Imported by: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp`, `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp`, `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp`, `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp`, `core/moonshine-tts/src/moonshine-tts.cpp`, `core/moonshine-tts/src/ort-onnx-external-data.cpp`, `core/moonshine-tts/src/piper-tts.cpp`, `core/moonshine-tts/src/zipvoice-tts.cpp`
- `ort_add_external_initializer_files_for_onnx_model_buffer` (function) `core/moonshine-tts/src/ort-onnx-external-data.h:18` `void ort_add_external_initializer_files_for_onnx_model_buffer( Ort::SessionOptions& opts, const FileInformationMap&...` -- If ``files`` contains an in-memory ``<stem>.onnx.data`` companion for ``model_map_key`` (either ``…/model.onnx`` or...

## core/moonshine-tts/src/ort-session-options.cpp
Depends on: `core/moonshine-tts/src/ort-session-options.h`, `core/ort-utils/ort-utils-cxx.h`
- `make_ort_session_options` (function) `core/moonshine-tts/src/ort-session-options.cpp:7` `Ort::SessionOptions make_ort_session_options(
    const std::vector<std::string>& provider_names,...`

## core/moonshine-tts/src/piper-tts.cpp
Depends on: `core/moonshine-tts/src/g2p-path.h`, `core/moonshine-tts/src/ipa-postprocess.h`, `core/moonshine-tts/src/moonshine-g2p.h`, `core/moonshine-tts/src/moonshine-tts-options.h`, `core/moonshine-tts/src/ort-onnx-external-data.h`, `core/moonshine-tts/src/ort-session-options.h`, `core/moonshine-tts/src/piper-tts.h`, `core/moonshine-tts/src/piper-voice-catalog.h`, `core/moonshine-tts/src/utf8-utils.h`, `core/moonshine-utils/debug-utils.h`
- `normalize_lang_key` (function) `core/moonshine-tts/src/piper-tts.cpp:35` `std::string normalize_lang_key(std::string_view raw)`
- `py_isspace_utf8_ch` (function) `core/moonshine-tts/src/piper-tts.cpp:49` `bool py_isspace_utf8_ch(std::string_view ch)`
- `lookup_piper_lang_row` (function) `core/moonshine-tts/src/piper-tts.cpp:73` `const PiperLangRow* lookup_piper_lang_row(std::string_view k)`
- `piper_ipa_norm_lang_key` (function) `core/moonshine-tts/src/piper-tts.cpp:130` `std::string piper_ipa_norm_lang_key(const std::string& lk,
                                    st...`
- `resolve_piper_lang` (function) `core/moonshine-tts/src/piper-tts.cpp:144` `void resolve_piper_lang(const std::string& lk, const MoonshineG2POptions& opt,
                  ...`
- `pick_onnx_path` (function) `core/moonshine-tts/src/piper-tts.cpp:178` `std::filesystem::path pick_onnx_path(const std::filesystem::path& voices_dir,
                   ...`
- `piper_model_json_path_for_onnx` (function) `core/moonshine-tts/src/piper-tts.cpp:233` `std::filesystem::path piper_model_json_path_for_onnx(
    const std::filesystem::path& onnx_path,...` -- Piper pairs ``foo.onnx`` with ``foo.onnx.json``.
- `append_phoneme_ids` (function) `core/moonshine-tts/src/piper-tts.cpp:244` `void append_phoneme_ids(
    const std::unordered_map<std::string, std::vector<int64_t>>& id_map,...`
- `ipa_utf8_to_piper_ids` (function) `core/moonshine-tts/src/piper-tts.cpp:256` `std::vector<int64_t> ipa_utf8_to_piper_ids(
    const std::string& ipa_nfc,
    const std::unorde...`
- `resample_linear` (function) `core/moonshine-tts/src/piper-tts.cpp:278` `std::vector<float> resample_linear(const std::vector<float>& x, int src_sr,
                     ...`
- `y` (function) `core/moonshine-tts/src/piper-tts.cpp:287` `std::vector<float> y(n_out);`
- `load_piper_onnx_json` (function) `core/moonshine-tts/src/piper-tts.cpp:301` `void load_piper_onnx_json(
    const std::filesystem::path& json_path,
    std::unordered_map<std...`
- `load_piper_onnx_json_bytes` (function) `core/moonshine-tts/src/piper-tts.cpp:354` `void load_piper_onnx_json_bytes(
    const char* data, size_t size, std::string_view ctx,
    std...`
- `run_ort_from_phoneme_ids` (function) `core/moonshine-tts/src/piper-tts.cpp:446` `std::vector<float> run_ort_from_phoneme_ids(const std::vector<int64_t>& ids)`
- `wave` (function) `core/moonshine-tts/src/piper-tts.cpp:502` `std::vector<float> wave(ptr, ptr + n_el);`
- `reload_session_from_onnx` (function) `core/moonshine-tts/src/piper-tts.cpp:511` `void reload_session_from_onnx()`
- `k_piper_json` (function) `core/moonshine-tts/src/piper-tts.cpp:512` `static const std::string k_piper_json("piper/onnx.json");`
- `k_piper_onnx` (function) `core/moonshine-tts/src/piper-tts.cpp:513` `static const std::string k_piper_onnx("piper/onnx");`
- `Impl` (function) `core/moonshine-tts/src/piper-tts.cpp:566` `explicit Impl(const PiperTTSOptions& opt)
      : speed_(opt.speed),
        ort_provider_names_(...`
- `set_speed` (function) `core/moonshine-tts/src/piper-tts.cpp:613` `void set_speed(double s)`
- `set_lang` (function) `core/moonshine-tts/src/piper-tts.cpp:621` `void set_lang(const std::string& lk)`
- `set_onnx_model` (function) `core/moonshine-tts/src/piper-tts.cpp:635` `void set_onnx_model(std::string_view stem_or_base)`
- `synthesize` (function) `core/moonshine-tts/src/piper-tts.cpp:644` `std::vector<float> synthesize(std::string_view text)`
- `synthesize_from_ipa` (function) `core/moonshine-tts/src/piper-tts.cpp:649` `std::vector<float> synthesize_from_ipa(std::string_view ipa_in)`
- `synthesize_phoneme_ids` (function) `core/moonshine-tts/src/piper-tts.cpp:669` `std::vector<float> synthesize_phoneme_ids(
      const std::vector<int64_t>& phoneme_ids)`
- `PiperTTS` (function) `core/moonshine-tts/src/piper-tts.cpp:675` `PiperTTS::PiperTTS(const PiperTTSOptions& opt)
    : impl_(std::make_unique<Impl>(opt))`
- `set_lang` (function) `core/moonshine-tts/src/piper-tts.cpp:683` `void PiperTTS::set_lang(std::string_view lang_cli)`
- `set_speed` (function) `core/moonshine-tts/src/piper-tts.cpp:687` `void PiperTTS::set_speed(double speed)`
- `speed` (function) `core/moonshine-tts/src/piper-tts.cpp:689` `double PiperTTS::speed() const`
- `set_onnx_model` (function) `core/moonshine-tts/src/piper-tts.cpp:691` `void PiperTTS::set_onnx_model(std::string_view basename_or_stem)`
- `normalize_audio` (function) `core/moonshine-tts/src/piper-tts.cpp:695` `bool PiperTTS::normalize_audio() const`
- `set_normalize_audio` (function) `core/moonshine-tts/src/piper-tts.cpp:697` `void PiperTTS::set_normalize_audio(bool on)`
- `output_volume` (function) `core/moonshine-tts/src/piper-tts.cpp:699` `float PiperTTS::output_volume() const`
- `set_output_volume` (function) `core/moonshine-tts/src/piper-tts.cpp:701` `void PiperTTS::set_output_volume(float volume)`
- `synthesize` (function) `core/moonshine-tts/src/piper-tts.cpp:705` `std::vector<float> PiperTTS::synthesize(std::string_view text)`
- `synthesize_from_ipa` (function) `core/moonshine-tts/src/piper-tts.cpp:709` `std::vector<float> PiperTTS::synthesize_from_ipa(std::string_view ipa)`
- `synthesize_phoneme_ids` (function) `core/moonshine-tts/src/piper-tts.cpp:713` `std::vector<float> PiperTTS::synthesize_phoneme_ids(
    const std::vector<int64_t>& phoneme_ids)`
- `p` (function) `core/moonshine-tts/src/piper-tts.cpp:771` `const std::filesystem::path p(default_onnx);`
- `piper_default_model_bundle_relative_paths` (function) `core/moonshine-tts/src/piper-tts.cpp:796` `bool piper_default_model_bundle_relative_paths(
    std::string_view lang_cli, const MoonshineG2P...`

## core/moonshine-tts/src/piper-tts.h
Depends on: `core/moonshine-tts/src/file-information.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`
Imported by: `core/moonshine-tts/src/moonshine-tts.cpp`, `core/moonshine-tts/src/piper-tts.cpp`, `core/moonshine-tts/tools/piper-phoneme-infer-cli.cpp`
- `set_lang` (function) `core/moonshine-tts/src/piper-tts.h:74` `void set_lang(std::string_view lang_cli);`
- `set_speed` (function) `core/moonshine-tts/src/piper-tts.h:75` `void set_speed(double speed);`
- `speed` (function) `core/moonshine-tts/src/piper-tts.h:76` `double speed() const;`
- `set_onnx_model` (function) `core/moonshine-tts/src/piper-tts.h:78` `void set_onnx_model(std::string_view basename_or_stem);` -- Basename or stem of an ``.onnx`` under ``voices_dir``.
- `normalize_audio` (function) `core/moonshine-tts/src/piper-tts.h:81` `bool normalize_audio() const;` -- Post-synthesis effects (``apply_synthesis_output_effects``).
- `set_normalize_audio` (function) `core/moonshine-tts/src/piper-tts.h:82` `void set_normalize_audio(bool on);`
- `output_volume` (function) `core/moonshine-tts/src/piper-tts.h:83` `float output_volume() const;`
- `set_output_volume` (function) `core/moonshine-tts/src/piper-tts.h:84` `void set_output_volume(float volume);`
- `synthesize` (function) `core/moonshine-tts/src/piper-tts.h:90` `std::vector<float> synthesize(std::string_view text);` -- Text → IPA (MoonshineG2P) → Piper phoneme ids → ONNX → mono float waveform at ``kSampleRateHz``.
- `synthesize_from_ipa` (function) `core/moonshine-tts/src/piper-tts.h:96` `std::vector<float> synthesize_from_ipa(std::string_view ipa);` -- Like ``synthesize`` but starts from an existing IPA phoneme string (the same format ``MoonshineG2P::text_to_ipa``...
- `synthesize_phoneme_ids` (function) `core/moonshine-tts/src/piper-tts.h:104` `std::vector<float> synthesize_phoneme_ids( const std::vector<int64_t>& phoneme_ids);` -- Run ONNX on an existing Piper phoneme-id sequence (same layout as ``piper.phoneme_ids.phonemes_to_ids``), then apply...

## core/moonshine-tts/src/piper-voice-catalog.h
Imported by: `core/moonshine-tts/src/piper-tts.cpp`, `core/moonshine-tts/src/piper-voice-catalog.cpp`
- `piper_bundled_voice_stems_for_data_subdir` (function) `core/moonshine-tts/src/piper-voice-catalog.h:12` `const std::vector<std::string>& piper_bundled_voice_stems_for_data_subdir( const std::string& data_subdir);` -- ONNX stems (no ``.onnx``) shipped under ``moonshine-tts/data/<data_subdir>/piper-voices/``.

## core/moonshine-tts/src/rule-based-g2p-factory.cpp
Depends on: `core/moonshine-tts/src/g2p-path.h`, `core/moonshine-tts/src/lang-specific/arabic.h`, `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h`, `core/moonshine-tts/src/lang-specific/chinese.h`, `core/moonshine-tts/src/lang-specific/dutch.h`, `core/moonshine-tts/src/lang-specific/english.h`, `core/moonshine-tts/src/lang-specific/french.h`, `core/moonshine-tts/src/lang-specific/german.h`, `core/moonshine-tts/src/lang-specific/hindi.h`, `core/moonshine-tts/src/lang-specific/italian.h`, `core/moonshine-tts/src/lang-specific/japanese.h`, `core/moonshine-tts/src/lang-specific/korean.h`, `core/moonshine-tts/src/lang-specific/portuguese.h`, `core/moonshine-tts/src/lang-specific/russian.h`, `core/moonshine-tts/src/lang-specific/spanish.h`, `core/moonshine-tts/src/lang-specific/turkish.h`, `core/moonshine-tts/src/lang-specific/ukrainian.h`, `core/moonshine-tts/src/lang-specific/vietnamese.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-tts/src/rule-based-g2p-factory.h`, `core/moonshine-tts/src/rule-based-g2p.h`, `core/moonshine-tts/src/utf8-utils.h`
- `resolve_french_dict_path` (function) `core/moonshine-tts/src/rule-based-g2p-factory.cpp:41` `std::filesystem::path resolve_french_dict_path(const MoonshineG2POptions& opt)`
- `resolve_french_csv_dir` (function) `core/moonshine-tts/src/rule-based-g2p-factory.cpp:46` `std::filesystem::path resolve_french_csv_dir(const MoonshineG2POptions& opt)`
- `normalize_spanish_dialect_cli_key` (function) `core/moonshine-tts/src/rule-based-g2p-factory.cpp:51` `std::string normalize_spanish_dialect_cli_key(std::string_view raw)`
- `file_looks_like_git_lfs_pointer` (function) `core/moonshine-tts/src/rule-based-g2p-factory.cpp:74` `bool file_looks_like_git_lfs_pointer(const std::filesystem::path& p)`
- `utf8_content_git_lfs_pointer_stub` (function) `core/moonshine-tts/src/rule-based-g2p-factory.cpp:86` `bool utf8_content_git_lfs_pointer_stub(std::string_view content)`
- `read_path_as_utf8` (function) `core/moonshine-tts/src/rule-based-g2p-factory.cpp:96` `std::string read_path_as_utf8(const std::filesystem::path& p)`
- `g2p_onnx_bundle_reachable` (function) `core/moonshine-tts/src/rule-based-g2p-factory.cpp:129` `bool g2p_onnx_bundle_reachable(const MoonshineG2POptions& o,
                               std::...`
- `g2p_onnx_bundle_includes_model_file` (function) `core/moonshine-tts/src/rule-based-g2p-factory.cpp:141` `bool g2p_onnx_bundle_includes_model_file(
    const MoonshineG2POptions& o, std::string_view bund...` -- True when ``meta.json`` is available and the model file it names exists on disk or in memory.
- `try_english` (function) `core/moonshine-tts/src/rule-based-g2p-factory.cpp:174` `std::optional<RuleBasedG2pInstance> try_english(
    std::string_view trimmed, const MoonshineG2P...`
- `try_spanish` (function) `core/moonshine-tts/src/rule-based-g2p-factory.cpp:288` `std::optional<RuleBasedG2pInstance> try_spanish(
    std::string_view trimmed, const MoonshineG2P...`
- `try_german` (function) `core/moonshine-tts/src/rule-based-g2p-factory.cpp:305` `std::optional<RuleBasedG2pInstance> try_german(
    std::string_view trimmed, const MoonshineG2PO...`
- `try_french` (function) `core/moonshine-tts/src/rule-based-g2p-factory.cpp:335` `std::optional<RuleBasedG2pInstance> try_french(
    std::string_view trimmed, const MoonshineG2PO...`
- `try_dutch` (function) `core/moonshine-tts/src/rule-based-g2p-factory.cpp:385` `std::optional<RuleBasedG2pInstance> try_dutch(
    std::string_view trimmed, const MoonshineG2POp...`
- `try_italian` (function) `core/moonshine-tts/src/rule-based-g2p-factory.cpp:417` `std::optional<RuleBasedG2pInstance> try_italian(
    std::string_view trimmed, const MoonshineG2P...`
- `try_russian` (function) `core/moonshine-tts/src/rule-based-g2p-factory.cpp:449` `std::optional<RuleBasedG2pInstance> try_russian(
    std::string_view trimmed, const MoonshineG2P...`
- `try_chinese` (function) `core/moonshine-tts/src/rule-based-g2p-factory.cpp:480` `std::optional<RuleBasedG2pInstance> try_chinese(
    std::string_view trimmed, const MoonshineG2P...`
- `try_korean` (function) `core/moonshine-tts/src/rule-based-g2p-factory.cpp:521` `std::optional<RuleBasedG2pInstance> try_korean(
    std::string_view trimmed, const MoonshineG2PO...`
- `try_vietnamese` (function) `core/moonshine-tts/src/rule-based-g2p-factory.cpp:547` `std::optional<RuleBasedG2pInstance> try_vietnamese(
    std::string_view trimmed, const Moonshine...`
- `try_japanese` (function) `core/moonshine-tts/src/rule-based-g2p-factory.cpp:571` `std::optional<RuleBasedG2pInstance> try_japanese(
    std::string_view trimmed, const MoonshineG2...`
- `try_arabic` (function) `core/moonshine-tts/src/rule-based-g2p-factory.cpp:611` `std::optional<RuleBasedG2pInstance> try_arabic(
    std::string_view trimmed, const MoonshineG2PO...`
- `try_turkish` (function) `core/moonshine-tts/src/rule-based-g2p-factory.cpp:650` `std::optional<RuleBasedG2pInstance> try_turkish(
    std::string_view trimmed, const MoonshineG2P...`
- `try_ukrainian` (function) `core/moonshine-tts/src/rule-based-g2p-factory.cpp:665` `std::optional<RuleBasedG2pInstance> try_ukrainian(
    std::string_view trimmed, const MoonshineG...`
- `try_hindi` (function) `core/moonshine-tts/src/rule-based-g2p-factory.cpp:680` `std::optional<RuleBasedG2pInstance> try_hindi(
    std::string_view trimmed, const MoonshineG2POp...`
- `try_portuguese` (function) `core/moonshine-tts/src/rule-based-g2p-factory.cpp:707` `std::optional<RuleBasedG2pInstance> try_portuguese(
    std::string_view trimmed, const Moonshine...`
- `pt_override_key` (function) `core/moonshine-tts/src/rule-based-g2p-factory.cpp:716` `const std::string pt_override_key(kG2pPortugueseDictOverrideKey);`
- `create_rule_based_g2p` (function) `core/moonshine-tts/src/rule-based-g2p-factory.cpp:786` `std::optional<RuleBasedG2pInstance> create_rule_based_g2p(
    std::string_view dialect_id, const...`

## core/moonshine-tts/src/text-normalize.cpp
Depends on: `core/moonshine-tts/src/text-normalize.h`, `core/moonshine-tts/src/utf8-utils.h`
- `is_word_char_utf8` (function) `core/moonshine-tts/src/text-normalize.cpp:10` `bool is_word_char_utf8(std::string_view unit)`
- `split_text_to_words` (function) `core/moonshine-tts/src/text-normalize.cpp:25` `std::vector<std::string> split_text_to_words(std::string_view text)`
- `normalize_word_for_lookup` (function) `core/moonshine-tts/src/text-normalize.cpp:48` `std::string normalize_word_for_lookup(std::string_view token)`
- `normalize_grapheme_key` (function) `core/moonshine-tts/src/text-normalize.cpp:75` `std::string normalize_grapheme_key(std::string_view word_token)`

## core/moonshine-tts/src/utf8-utils.cpp
Depends on: `core/moonshine-tts/src/utf8-utils.h`
- `utf8_decode_at` (function) `core/moonshine-tts/src/utf8-utils.cpp:7` `bool utf8_decode_at(const std::string& s, size_t i, char32_t& out_cp,
                    size_t&...`
- `utf8_str_to_u32` (function) `core/moonshine-tts/src/utf8-utils.cpp:62` `std::u32string utf8_str_to_u32(const std::string& s)`
- `utf8_append_codepoint` (function) `core/moonshine-tts/src/utf8-utils.cpp:75` `void utf8_append_codepoint(std::string& out, char32_t cp)`
- `utf8_split_codepoints` (function) `core/moonshine-tts/src/utf8-utils.cpp:93` `std::vector<std::string> utf8_split_codepoints(const std::string& utf8)`
- `codepoint_is_unicode_word_neighbor_for_digits` (function) `core/moonshine-tts/src/utf8-utils.cpp:183` `bool codepoint_is_unicode_word_neighbor_for_digits(char32_t c)`
- `utf8_codepoint_before_index` (function) `core/moonshine-tts/src/utf8-utils.cpp:220` `std::optional<char32_t> utf8_codepoint_before_index(const std::string& s,
                       ...`
- `utf8_codepoint_at_index` (function) `core/moonshine-tts/src/utf8-utils.cpp:237` `std::optional<char32_t> utf8_codepoint_at_index(const std::string& s,
                           ...`
- `digit_ascii_span_expandable_python_w` (function) `core/moonshine-tts/src/utf8-utils.cpp:250` `bool digit_ascii_span_expandable_python_w(const std::string& text,
                              ...`
- `normalize_rule_based_dialect_cli_key` (function) `core/moonshine-tts/src/utf8-utils.cpp:266` `std::string normalize_rule_based_dialect_cli_key(std::string_view raw)`
- `dedupe_dialect_ids_preserve_first` (function) `core/moonshine-tts/src/utf8-utils.cpp:278` `std::vector<std::string> dedupe_dialect_ids_preserve_first(
    std::vector<std::string> ids)`

## core/moonshine-tts/src/utf8-utils.h
Imported by: `core/moonshine-tts/src/ipa-postprocess.cpp`, `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp`, `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp`, `core/moonshine-tts/src/lang-specific/arabic.cpp`, `core/moonshine-tts/src/lang-specific/chinese-numbers.cpp`, `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp`, `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp`, `core/moonshine-tts/src/lang-specific/chinese.cpp`, `core/moonshine-tts/src/lang-specific/dutch.cpp`, `core/moonshine-tts/src/lang-specific/english.cpp`, `core/moonshine-tts/src/lang-specific/french-oov.cpp`, `core/moonshine-tts/src/lang-specific/french.cpp`, `core/moonshine-tts/src/lang-specific/german.cpp`, `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp`, `core/moonshine-tts/src/lang-specific/hindi.cpp`, `core/moonshine-tts/src/lang-specific/italian.cpp`, `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp`, `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp`, `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp`, `core/moonshine-tts/src/lang-specific/japanese.cpp`, `core/moonshine-tts/src/lang-specific/korean-numbers.cpp`, `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp`, `core/moonshine-tts/src/lang-specific/korean.cpp`, `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp`, `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp`, `core/moonshine-tts/src/lang-specific/portuguese.cpp`, `core/moonshine-tts/src/lang-specific/russian-numbers.cpp`, `core/moonshine-tts/src/lang-specific/russian.cpp`, `core/moonshine-tts/src/lang-specific/spanish-numbers.cpp`, `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp`, `core/moonshine-tts/src/lang-specific/spanish.cpp`, `core/moonshine-tts/src/lang-specific/turkish.cpp`, `core/moonshine-tts/src/lang-specific/ukrainian.cpp`, `core/moonshine-tts/src/lang-specific/vietnamese.cpp`, `core/moonshine-tts/src/moonshine-asset-catalog.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/moonshine-tts.cpp`, `core/moonshine-tts/src/piper-tts.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/src/text-normalize.cpp`, `core/moonshine-tts/src/utf8-utils.cpp`, `core/moonshine-tts/src/zipvoice-tts.cpp`, `core/moonshine-tts/tests/heteronym-context-test.cpp`, `core/moonshine-tts/tests/utf8-utils-test.cpp`, `core/moonshine-tts/tools/moonshine-tts-cli.cpp`
- `utf8_append_codepoint` (function) `core/moonshine-tts/src/utf8-utils.h:14` `void utf8_append_codepoint(std::string& out, char32_t cp);`
- `utf8_decode_at` (function) `core/moonshine-tts/src/utf8-utils.h:19` `bool utf8_decode_at(const std::string& s, size_t i, char32_t& out_cp, size_t& out_len);` -- Decode one UTF-8 code point starting at byte index *i* in *s*.
- `erase_utf8_substr` (function) `core/moonshine-tts/src/utf8-utils.h:27` `inline void erase_utf8_substr(std::string& s, std::string_view sub)` -- Remove every occurrence of *sub* from *s*.
- `is_ascii_whitespace` (function) `core/moonshine-tts/src/utf8-utils.h:45` `inline bool is_ascii_whitespace(unsigned char c)` -- Trim ASCII whitespace only (same policy as legacy ``trim_copy_sv`` helpers in language files).
- `trim_ascii_ws_copy` (function) `core/moonshine-tts/src/utf8-utils.h:50` `inline std::string trim_ascii_ws_copy(std::string_view s)`
- `codepoint_is_unicode_word_neighbor_for_digits` (function) `core/moonshine-tts/src/utf8-utils.h:72` `bool codepoint_is_unicode_word_neighbor_for_digits(char32_t cp);` -- Rough Python ``\\w`` neighbor for ``re`` digit spans: ASCII alnum + underscore + major script blocks.
- `utf8_codepoint_before_index` (function) `core/moonshine-tts/src/utf8-utils.h:74` `std::optional<char32_t> utf8_codepoint_before_index(const std::string& s, size_t byte_idx);`
- `utf8_codepoint_at_index` (function) `core/moonshine-tts/src/utf8-utils.h:76` `std::optional<char32_t> utf8_codepoint_at_index(const std::string& s, size_t byte_idx);`
- `digit_ascii_span_expandable_python_w` (function) `core/moonshine-tts/src/utf8-utils.h:81` `bool digit_ascii_span_expandable_python_w(const std::string& text, size_t start_byte, size_t end_byte);` -- True if the ASCII digit substring ``text[start_byte:end_byte]`` should expand like Python ``\\b\\d+\\b``.


Next: [API_p5.md](API_p5.md)
