# Subsystem: core_moonshine-tts_src (page 2 of 2)
Previous: [KB_core_moonshine-tts_src.md](KB_core_moonshine-tts_src.md)

## core/moonshine-tts/src/ort-session-options.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `make_ort_session_options` (function, line 7) `Ort::SessionOptions make_ort_session_options(
    const std::vector<std::string>& provider_names,...`
- Depends on: `core/moonshine-tts/src/ort-session-options.h`, `core/ort-utils/ort-utils-cxx.h`

## core/moonshine-tts/src/ort-session-options.h
- Layer: utility
- Language: h
- Symbols:
  - `MOONSHINE_TTS_ORT_SESSION_OPTIONS_H` (macro, line 2) `#define MOONSHINE_TTS_ORT_SESSION_OPTIONS_H`
- Depends on: `core/ort-utils/ort-utils.h`
- Imported by: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp`, `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp`, `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp`, `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp`, `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp`, `core/moonshine-tts/src/moonshine-tts.cpp`, `core/moonshine-tts/src/ort-session-options.cpp`, `core/moonshine-tts/src/piper-tts.cpp`, `core/moonshine-tts/src/zipvoice-tts.cpp`

## core/moonshine-tts/src/piper-tts.cpp
- Doc: piper_model_json_path_for_onnx: Piper pairs ``foo.onnx`` with ``foo.onnx.json``.
- Layer: utility
- Language: cpp
- Symbols:
  - `PiperLangRow` (struct, line 67)
  - `normalize_lang_key` (function, line 35) `std::string normalize_lang_key(std::string_view raw)`
  - `py_isspace_utf8_ch` (function, line 49) `bool py_isspace_utf8_ch(std::string_view ch)`
  - `lookup_piper_lang_row` (function, line 73) `const PiperLangRow* lookup_piper_lang_row(std::string_view k)`
  - `piper_ipa_norm_lang_key` (function, line 130) `std::string piper_ipa_norm_lang_key(const std::string& lk,
                                    st...`
  - `resolve_piper_lang` (function, line 144) `void resolve_piper_lang(const std::string& lk, const MoonshineG2POptions& opt,
                  ...`
  - `pick_onnx_path` (function, line 178) `std::filesystem::path pick_onnx_path(const std::filesystem::path& voices_dir,
                   ...`
  - `piper_model_json_path_for_onnx` (function, line 233) `std::filesystem::path piper_model_json_path_for_onnx(
    const std::filesystem::path& onnx_path,...`
  - `append_phoneme_ids` (function, line 244) `void append_phoneme_ids(
    const std::unordered_map<std::string, std::vector<int64_t>>& id_map,...`
  - `ipa_utf8_to_piper_ids` (function, line 256) `std::vector<int64_t> ipa_utf8_to_piper_ids(
    const std::string& ipa_nfc,
    const std::unorde...`
  - `resample_linear` (function, line 278) `std::vector<float> resample_linear(const std::vector<float>& x, int src_sr,
                     ...`
  - `load_piper_onnx_json` (function, line 301) `void load_piper_onnx_json(
    const std::filesystem::path& json_path,
    std::unordered_map<std...`
  - `load_piper_onnx_json_bytes` (function, line 354) `void load_piper_onnx_json_bytes(
    const char* data, size_t size, std::string_view ctx,
    std...`
  - `run_ort_from_phoneme_ids` (function, line 446) `std::vector<float> run_ort_from_phoneme_ids(const std::vector<int64_t>& ids)`
  - `reload_session_from_onnx` (function, line 511) `void reload_session_from_onnx()`
  - `Impl` (function, line 566) `explicit Impl(const PiperTTSOptions& opt)
      : speed_(opt.speed),
        ort_provider_names_(...`
  - `set_speed` (function, line 613) `void set_speed(double s)`
  - `set_lang` (function, line 621) `void set_lang(const std::string& lk)`
  - `set_onnx_model` (function, line 635) `void set_onnx_model(std::string_view stem_or_base)`
  - `synthesize` (function, line 644) `std::vector<float> synthesize(std::string_view text)`
  - `synthesize_from_ipa` (function, line 649) `std::vector<float> synthesize_from_ipa(std::string_view ipa_in)`
  - `synthesize_phoneme_ids` (function, line 669) `std::vector<float> synthesize_phoneme_ids(
      const std::vector<int64_t>& phoneme_ids)`
  - `PiperTTS` (function, line 675) `PiperTTS::PiperTTS(const PiperTTSOptions& opt)
    : impl_(std::make_unique<Impl>(opt))`
  - `set_lang` (function, line 683) `void PiperTTS::set_lang(std::string_view lang_cli)`
  - `set_speed` (function, line 687) `void PiperTTS::set_speed(double speed)`
  - `speed` (function, line 689) `double PiperTTS::speed() const`
  - `set_onnx_model` (function, line 691) `void PiperTTS::set_onnx_model(std::string_view basename_or_stem)`
  - `normalize_audio` (function, line 695) `bool PiperTTS::normalize_audio() const`
  - `set_normalize_audio` (function, line 697) `void PiperTTS::set_normalize_audio(bool on)`
  - `output_volume` (function, line 699) `float PiperTTS::output_volume() const`
  - `set_output_volume` (function, line 701) `void PiperTTS::set_output_volume(float volume)`
  - `synthesize` (function, line 705) `std::vector<float> PiperTTS::synthesize(std::string_view text)`
  - `synthesize_from_ipa` (function, line 709) `std::vector<float> PiperTTS::synthesize_from_ipa(std::string_view ipa)`
  - `synthesize_phoneme_ids` (function, line 713) `std::vector<float> PiperTTS::synthesize_phoneme_ids(
    const std::vector<int64_t>& phoneme_ids)`
  - `piper_default_model_bundle_relative_paths` (function, line 796) `bool piper_default_model_bundle_relative_paths(
    std::string_view lang_cli, const MoonshineG2P...`
  - `y` (function, line 287) `std::vector<float> y(n_out);`
  - `wave` (function, line 502) `std::vector<float> wave(ptr, ptr + n_el);`
  - `k_piper_json` (function, line 512) `static const std::string k_piper_json("piper/onnx.json");`
  - `k_piper_onnx` (function, line 513) `static const std::string k_piper_onnx("piper/onnx");`
  - `p` (function, line 771) `const std::filesystem::path p(default_onnx);`
- Depends on: `core/moonshine-tts/src/g2p-path.h`, `core/moonshine-tts/src/ipa-postprocess.h`, `core/moonshine-tts/src/moonshine-g2p.h`, `core/moonshine-tts/src/moonshine-tts-options.h`, `core/moonshine-tts/src/ort-onnx-external-data.h`, `core/moonshine-tts/src/ort-session-options.h`, `core/moonshine-tts/src/piper-tts.h`, `core/moonshine-tts/src/piper-voice-catalog.h`, `core/moonshine-tts/src/utf8-utils.h`, `core/moonshine-utils/debug-utils.h`

## core/moonshine-tts/src/piper-tts.h
- Doc: PiperTTSOptions: Piper ONNX TTS + ``MoonshineG2P`` IPA (filtered to each model's...
- Layer: utility
- Language: h
- Symbols:
  - `PiperTTSOptions` (struct, line 19)
  - `Impl` (struct, line 108)
  - `PiperTTS` (class, line 65)
  - `set_lang` (function, line 74) `void set_lang(std::string_view lang_cli);`
  - `set_speed` (function, line 75) `void set_speed(double speed);`
  - `speed` (function, line 76) `double speed() const;`
  - `set_onnx_model` (function, line 78) `void set_onnx_model(std::string_view basename_or_stem);`
  - `normalize_audio` (function, line 81) `bool normalize_audio() const;`
  - `set_normalize_audio` (function, line 82) `void set_normalize_audio(bool on);`
  - `output_volume` (function, line 83) `float output_volume() const;`
  - `set_output_volume` (function, line 84) `void set_output_volume(float volume);`
  - `synthesize` (function, line 90) `std::vector<float> synthesize(std::string_view text);`
  - `synthesize_from_ipa` (function, line 96) `std::vector<float> synthesize_from_ipa(std::string_view ipa);`
  - `synthesize_phoneme_ids` (function, line 104) `std::vector<float> synthesize_phoneme_ids( const std::vector<int64_t>& phoneme_ids);`
  - `MOONSHINE_TTS_PIPER_TTS_H` (macro, line 2) `#define MOONSHINE_TTS_PIPER_TTS_H`
- Depends on: `core/moonshine-tts/src/file-information.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`
- Imported by: `core/moonshine-tts/src/moonshine-tts.cpp`, `core/moonshine-tts/src/piper-tts.cpp`, `core/moonshine-tts/tools/piper-phoneme-infer-cli.cpp`

## core/moonshine-tts/src/piper-voice-catalog.cpp
- Doc: Bundled Piper ONNX stems, kept in sync with ``moonshine-tts/data/*/piper-voices/*.onnx``.
- Layer: utility
- Language: cpp
- Depends on: `core/moonshine-tts/src/piper-voice-catalog.h`

## core/moonshine-tts/src/piper-voice-catalog.h
- Doc: piper_bundled_voice_stems_for_data_subdir: ONNX stems (no ``.onnx``) shipped under...
- Layer: utility
- Language: h
- Symbols:
  - `piper_bundled_voice_stems_for_data_subdir` (function, line 12) `const std::vector<std::string>& piper_bundled_voice_stems_for_data_subdir( const std::string& data_subdir);`
  - `MOONSHINE_TTS_PIPER_VOICE_CATALOG_H` (macro, line 2) `#define MOONSHINE_TTS_PIPER_VOICE_CATALOG_H`
- Imported by: `core/moonshine-tts/src/piper-tts.cpp`, `core/moonshine-tts/src/piper-voice-catalog.cpp`

## core/moonshine-tts/src/rule-based-g2p-factory.cpp
- Doc: g2p_onnx_bundle_includes_model_file: True when ``meta.json`` is available and the model file it...
- Layer: business_logic
- Language: cpp
- Symbols:
  - `resolve_french_dict_path` (function, line 41) `std::filesystem::path resolve_french_dict_path(const MoonshineG2POptions& opt)`
  - `resolve_french_csv_dir` (function, line 46) `std::filesystem::path resolve_french_csv_dir(const MoonshineG2POptions& opt)`
  - `normalize_spanish_dialect_cli_key` (function, line 51) `std::string normalize_spanish_dialect_cli_key(std::string_view raw)`
  - `file_looks_like_git_lfs_pointer` (function, line 74) `bool file_looks_like_git_lfs_pointer(const std::filesystem::path& p)`
  - `utf8_content_git_lfs_pointer_stub` (function, line 86) `bool utf8_content_git_lfs_pointer_stub(std::string_view content)`
  - `read_path_as_utf8` (function, line 96) `std::string read_path_as_utf8(const std::filesystem::path& p)`
  - `g2p_onnx_bundle_reachable` (function, line 129) `bool g2p_onnx_bundle_reachable(const MoonshineG2POptions& o,
                               std::...`
  - `g2p_onnx_bundle_includes_model_file` (function, line 141) `bool g2p_onnx_bundle_includes_model_file(
    const MoonshineG2POptions& o, std::string_view bund...`
  - `try_english` (function, line 174) `std::optional<RuleBasedG2pInstance> try_english(
    std::string_view trimmed, const MoonshineG2P...`
  - `try_spanish` (function, line 288) `std::optional<RuleBasedG2pInstance> try_spanish(
    std::string_view trimmed, const MoonshineG2P...`
  - `try_german` (function, line 305) `std::optional<RuleBasedG2pInstance> try_german(
    std::string_view trimmed, const MoonshineG2PO...`
  - `try_french` (function, line 335) `std::optional<RuleBasedG2pInstance> try_french(
    std::string_view trimmed, const MoonshineG2PO...`
  - `try_dutch` (function, line 385) `std::optional<RuleBasedG2pInstance> try_dutch(
    std::string_view trimmed, const MoonshineG2POp...`
  - `try_italian` (function, line 417) `std::optional<RuleBasedG2pInstance> try_italian(
    std::string_view trimmed, const MoonshineG2P...`
  - `try_russian` (function, line 449) `std::optional<RuleBasedG2pInstance> try_russian(
    std::string_view trimmed, const MoonshineG2P...`
  - `try_chinese` (function, line 480) `std::optional<RuleBasedG2pInstance> try_chinese(
    std::string_view trimmed, const MoonshineG2P...`
  - `try_korean` (function, line 521) `std::optional<RuleBasedG2pInstance> try_korean(
    std::string_view trimmed, const MoonshineG2PO...`
  - `try_vietnamese` (function, line 547) `std::optional<RuleBasedG2pInstance> try_vietnamese(
    std::string_view trimmed, const Moonshine...`
  - `try_japanese` (function, line 571) `std::optional<RuleBasedG2pInstance> try_japanese(
    std::string_view trimmed, const MoonshineG2...`
  - `try_arabic` (function, line 611) `std::optional<RuleBasedG2pInstance> try_arabic(
    std::string_view trimmed, const MoonshineG2PO...`
  - `try_turkish` (function, line 650) `std::optional<RuleBasedG2pInstance> try_turkish(
    std::string_view trimmed, const MoonshineG2P...`
  - `try_ukrainian` (function, line 665) `std::optional<RuleBasedG2pInstance> try_ukrainian(
    std::string_view trimmed, const MoonshineG...`
  - `try_hindi` (function, line 680) `std::optional<RuleBasedG2pInstance> try_hindi(
    std::string_view trimmed, const MoonshineG2POp...`
  - `try_portuguese` (function, line 707) `std::optional<RuleBasedG2pInstance> try_portuguese(
    std::string_view trimmed, const Moonshine...`
  - `create_rule_based_g2p` (function, line 786) `std::optional<RuleBasedG2pInstance> create_rule_based_g2p(
    std::string_view dialect_id, const...`
  - `pt_override_key` (function, line 716) `const std::string pt_override_key(kG2pPortugueseDictOverrideKey);`
- Depends on: `core/moonshine-tts/src/g2p-path.h`, `core/moonshine-tts/src/lang-specific/arabic.h`, `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h`, `core/moonshine-tts/src/lang-specific/chinese.h`, `core/moonshine-tts/src/lang-specific/dutch.h`, `core/moonshine-tts/src/lang-specific/english.h`, `core/moonshine-tts/src/lang-specific/french.h`, `core/moonshine-tts/src/lang-specific/german.h`, `core/moonshine-tts/src/lang-specific/hindi.h`, `core/moonshine-tts/src/lang-specific/italian.h`, `core/moonshine-tts/src/lang-specific/japanese.h`, `core/moonshine-tts/src/lang-specific/korean.h`, `core/moonshine-tts/src/lang-specific/portuguese.h`, `core/moonshine-tts/src/lang-specific/russian.h`, `core/moonshine-tts/src/lang-specific/spanish.h`, `core/moonshine-tts/src/lang-specific/turkish.h`, `core/moonshine-tts/src/lang-specific/ukrainian.h`, `core/moonshine-tts/src/lang-specific/vietnamese.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-tts/src/rule-based-g2p-factory.h`, `core/moonshine-tts/src/rule-based-g2p.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/rule-based-g2p-factory.h
- Layer: business_logic
- Language: h
- Symbols:
  - `RuleBasedG2pInstance` (struct, line 35)
  - `RuleBasedG2pKind` (enum, line 16)
  - `RuleBasedG2pKind` (class, line 16)
  - `MOONSHINE_TTS_RULE_BASED_G2P_FACTORY_H` (macro, line 2) `#define MOONSHINE_TTS_RULE_BASED_G2P_FACTORY_H`
- Depends on: `core/moonshine-tts/src/moonshine-g2p-options.h`
- Imported by: `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/moonshine-g2p.h`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`

## core/moonshine-tts/src/rule-based-g2p.h
- Doc: RuleBasedG2p: Shared interface for lexicon + rules G2P backends used by ``MoonshineG2P``.
- Layer: business_logic
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 9)
  - `RuleBasedG2p` (class, line 12)
  - `MOONSHINE_TTS_RULE_BASED_G2P_H` (macro, line 2) `#define MOONSHINE_TTS_RULE_BASED_G2P_H`
- Imported by: `core/moonshine-tts/src/lang-specific/arabic.h`, `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h`, `core/moonshine-tts/src/lang-specific/chinese.h`, `core/moonshine-tts/src/lang-specific/dutch.h`, `core/moonshine-tts/src/lang-specific/english.h`, `core/moonshine-tts/src/lang-specific/french.h`, `core/moonshine-tts/src/lang-specific/german.h`, `core/moonshine-tts/src/lang-specific/hindi.h`, `core/moonshine-tts/src/lang-specific/italian.h`, `core/moonshine-tts/src/lang-specific/japanese.h`, `core/moonshine-tts/src/lang-specific/korean.h`, `core/moonshine-tts/src/lang-specific/portuguese.h`, `core/moonshine-tts/src/lang-specific/russian.h`, `core/moonshine-tts/src/lang-specific/spanish.h`, `core/moonshine-tts/src/lang-specific/turkish.h`, `core/moonshine-tts/src/lang-specific/ukrainian.h`, `core/moonshine-tts/src/lang-specific/vietnamese.h`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`

## core/moonshine-tts/src/text-normalize.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `is_word_char_utf8` (function, line 10) `bool is_word_char_utf8(std::string_view unit)`
  - `split_text_to_words` (function, line 25) `std::vector<std::string> split_text_to_words(std::string_view text)`
  - `normalize_word_for_lookup` (function, line 48) `std::string normalize_word_for_lookup(std::string_view token)`
  - `normalize_grapheme_key` (function, line 75) `std::string normalize_grapheme_key(std::string_view word_token)`
- Depends on: `core/moonshine-tts/src/text-normalize.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/text-normalize.h
- Layer: utility
- Language: h
- Symbols:
  - `MOONSHINE_TTS_TEXT_NORMALIZE_H` (macro, line 2) `#define MOONSHINE_TTS_TEXT_NORMALIZE_H`
- Imported by: `core/moonshine-tts/src/lang-specific/cmudict-tsv.cpp`, `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp`, `core/moonshine-tts/src/lang-specific/english.cpp`, `core/moonshine-tts/src/text-normalize.cpp`, `core/moonshine-tts/tests/text-normalize-test.cpp`

## core/moonshine-tts/src/utf8-utils.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `utf8_decode_at` (function, line 7) `bool utf8_decode_at(const std::string& s, size_t i, char32_t& out_cp,
                    size_t&...`
  - `utf8_str_to_u32` (function, line 62) `std::u32string utf8_str_to_u32(const std::string& s)`
  - `utf8_append_codepoint` (function, line 75) `void utf8_append_codepoint(std::string& out, char32_t cp)`
  - `utf8_split_codepoints` (function, line 93) `std::vector<std::string> utf8_split_codepoints(const std::string& utf8)`
  - `codepoint_is_unicode_word_neighbor_for_digits` (function, line 183) `bool codepoint_is_unicode_word_neighbor_for_digits(char32_t c)`
  - `utf8_codepoint_before_index` (function, line 220) `std::optional<char32_t> utf8_codepoint_before_index(const std::string& s,
                       ...`
  - `utf8_codepoint_at_index` (function, line 237) `std::optional<char32_t> utf8_codepoint_at_index(const std::string& s,
                           ...`
  - `digit_ascii_span_expandable_python_w` (function, line 250) `bool digit_ascii_span_expandable_python_w(const std::string& text,
                              ...`
  - `normalize_rule_based_dialect_cli_key` (function, line 266) `std::string normalize_rule_based_dialect_cli_key(std::string_view raw)`
  - `dedupe_dialect_ids_preserve_first` (function, line 278) `std::vector<std::string> dedupe_dialect_ids_preserve_first(
    std::vector<std::string> ids)`
- Depends on: `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/utf8-utils.h
- Doc: erase_utf8_substr: Remove every occurrence of *sub* from *s*.
- Layer: utility
- Language: h
- Symbols:
  - `erase_utf8_substr` (function, line 27) `inline void erase_utf8_substr(std::string& s, std::string_view sub)`
  - `is_ascii_whitespace` (function, line 45) `inline bool is_ascii_whitespace(unsigned char c)`
  - `trim_ascii_ws_copy` (function, line 50) `inline std::string trim_ascii_ws_copy(std::string_view s)`
  - `utf8_append_codepoint` (function, line 14) `void utf8_append_codepoint(std::string& out, char32_t cp);`
  - `utf8_decode_at` (function, line 19) `bool utf8_decode_at(const std::string& s, size_t i, char32_t& out_cp, size_t& out_len);`
  - `codepoint_is_unicode_word_neighbor_for_digits` (function, line 72) `bool codepoint_is_unicode_word_neighbor_for_digits(char32_t cp);`
  - `utf8_codepoint_before_index` (function, line 74) `std::optional<char32_t> utf8_codepoint_before_index(const std::string& s, size_t byte_idx);`
  - `utf8_codepoint_at_index` (function, line 76) `std::optional<char32_t> utf8_codepoint_at_index(const std::string& s, size_t byte_idx);`
  - `digit_ascii_span_expandable_python_w` (function, line 81) `bool digit_ascii_span_expandable_python_w(const std::string& text, size_t start_byte, size_t end_byte);`
  - `MOONSHINE_TTS_UTF8_UTILS_H` (macro, line 2) `#define MOONSHINE_TTS_UTF8_UTILS_H`
- Imported by: `core/moonshine-tts/src/ipa-postprocess.cpp`, `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp`, `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp`, `core/moonshine-tts/src/lang-specific/arabic.cpp`, `core/moonshine-tts/src/lang-specific/chinese-numbers.cpp`, `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp`, `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp`, `core/moonshine-tts/src/lang-specific/chinese.cpp`, `core/moonshine-tts/src/lang-specific/dutch.cpp`, `core/moonshine-tts/src/lang-specific/english.cpp`, `core/moonshine-tts/src/lang-specific/french-oov.cpp`, `core/moonshine-tts/src/lang-specific/french.cpp`, `core/moonshine-tts/src/lang-specific/german.cpp`, `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp`, `core/moonshine-tts/src/lang-specific/hindi.cpp`, `core/moonshine-tts/src/lang-specific/italian.cpp`, `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp`, `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp`, `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp`, `core/moonshine-tts/src/lang-specific/japanese.cpp`, `core/moonshine-tts/src/lang-specific/korean-numbers.cpp`, `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp`, `core/moonshine-tts/src/lang-specific/korean.cpp`, `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp`, `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp`, `core/moonshine-tts/src/lang-specific/portuguese.cpp`, `core/moonshine-tts/src/lang-specific/russian-numbers.cpp`, `core/moonshine-tts/src/lang-specific/russian.cpp`, `core/moonshine-tts/src/lang-specific/spanish-numbers.cpp`, `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp`, `core/moonshine-tts/src/lang-specific/spanish.cpp`, `core/moonshine-tts/src/lang-specific/turkish.cpp`, `core/moonshine-tts/src/lang-specific/ukrainian.cpp`, `core/moonshine-tts/src/lang-specific/vietnamese.cpp`, `core/moonshine-tts/src/moonshine-asset-catalog.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/moonshine-tts.cpp`, `core/moonshine-tts/src/piper-tts.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/src/text-normalize.cpp`, `core/moonshine-tts/src/utf8-utils.cpp`, `core/moonshine-tts/src/zipvoice-tts.cpp`, `core/moonshine-tts/tests/heteronym-context-test.cpp`, `core/moonshine-tts/tests/utf8-utils-test.cpp`, `core/moonshine-tts/tools/moonshine-tts-cli.cpp`

## core/moonshine-tts/src/zipvoice-custom-ops.cpp
- Doc: Custom ONNX Runtime operators for the ZipVoice Zipformer (domain ai.zipvoice).
- Layer: utility
- Language: cpp
- Symbols:
  - `SwooshJob` (struct, line 70)
  - `SwooshKernel` (struct, line 95)
  - `GluJob` (struct, line 126)
  - `GluKernel` (struct, line 146)
  - `DwJob` (struct, line 176)
  - `DepthwiseConvKernel` (struct, line 204)
  - `BiasNormJob` (struct, line 251)
  - `BiasNormKernel` (struct, line 276)
  - `BypassJob` (struct, line 303)
  - `BypassKernel` (struct, line 322)
  - `SoftplusPoly` (function, line 52) `inline float SoftplusPoly(float z)`
  - `ComputeTile` (function, line 78) `void ComputeTile(void* user_data, size_t idx)`
  - `SwooshKernel` (function, line 96) `explicit SwooshKernel(bool is_left)
      : offset_(is_left ? kLeftOffset : kRightOffset),
      ...`
  - `Compute` (function, line 100) `void Compute(OrtKernelContext* context)`
  - `SigmoidScalar` (function, line 124) `inline float SigmoidScalar(float v)`
  - `ComputeGluRow` (function, line 132) `void ComputeGluRow(void* user_data, size_t r)`
  - `Compute` (function, line 147) `void Compute(OrtKernelContext* context)`
  - `ComputeConvRow` (function, line 184) `void ComputeConvRow(void* user_data, size_t row)`
  - `Compute` (function, line 205) `void Compute(OrtKernelContext* context)`
  - `ComputeBiasNormRow` (function, line 259) `void ComputeBiasNormRow(void* user_data, size_t r)`
  - `Compute` (function, line 277) `void Compute(OrtKernelContext* context)`
  - `ComputeBypassRow` (function, line 311) `void ComputeBypassRow(void* user_data, size_t r)`
  - `Compute` (function, line 323) `void Compute(OrtKernelContext* context)`
  - `CreateKernel` (function, line 350) `void* CreateKernel(const OrtApi& /*api*/,
                     const OrtKernelInfo* /*info*/) const`
  - `GetName` (function, line 354) `const char* GetName() const`
  - `GetInputTypeCount` (function, line 355) `size_t GetInputTypeCount() const`
  - `GetInputType` (function, line 356) `ONNXTensorElementDataType GetInputType(size_t /*index*/) const`
  - `GetOutputTypeCount` (function, line 359) `size_t GetOutputTypeCount() const`
  - `GetOutputType` (function, line 360) `ONNXTensorElementDataType GetOutputType(size_t /*index*/) const`
  - `CreateKernel` (function, line 366) `void* CreateKernel(const OrtApi& /*api*/,
                     const OrtKernelInfo* /*info*/) const`
  - `GetName` (function, line 370) `const char* GetName() const`
  - `GetInputTypeCount` (function, line 371) `size_t GetInputTypeCount() const`
  - `GetInputType` (function, line 372) `ONNXTensorElementDataType GetInputType(size_t /*index*/) const`
  - `GetOutputTypeCount` (function, line 375) `size_t GetOutputTypeCount() const`
  - `GetOutputType` (function, line 376) `ONNXTensorElementDataType GetOutputType(size_t /*index*/) const`
  - `CreateKernel` (function, line 382) `void* CreateKernel(const OrtApi& /*api*/,
                     const OrtKernelInfo* /*info*/) const`
  - `GetName` (function, line 386) `const char* GetName() const`
  - `GetInputTypeCount` (function, line 387) `size_t GetInputTypeCount() const`
  - `GetInputType` (function, line 388) `ONNXTensorElementDataType GetInputType(size_t /*index*/) const`
  - `GetOutputTypeCount` (function, line 391) `size_t GetOutputTypeCount() const`
  - `GetOutputType` (function, line 392) `ONNXTensorElementDataType GetOutputType(size_t /*index*/) const`
  - `CreateKernel` (function, line 399) `void* CreateKernel(const OrtApi& /*api*/,
                     const OrtKernelInfo* /*info*/) const`
  - `GetName` (function, line 403) `const char* GetName() const`
  - `GetInputTypeCount` (function, line 404) `size_t GetInputTypeCount() const`
  - `GetInputType` (function, line 405) `ONNXTensorElementDataType GetInputType(size_t /*index*/) const`
  - `GetOutputTypeCount` (function, line 408) `size_t GetOutputTypeCount() const`
  - `GetOutputType` (function, line 409) `ONNXTensorElementDataType GetOutputType(size_t /*index*/) const`
  - `CreateKernel` (function, line 415) `void* CreateKernel(const OrtApi& /*api*/,
                     const OrtKernelInfo* /*info*/) const`
  - `GetName` (function, line 419) `const char* GetName() const`
  - `GetInputTypeCount` (function, line 420) `size_t GetInputTypeCount() const`
  - `GetInputType` (function, line 421) `ONNXTensorElementDataType GetInputType(size_t /*index*/) const`
  - `GetOutputTypeCount` (function, line 424) `size_t GetOutputTypeCount() const`
  - `GetOutputType` (function, line 425) `ONNXTensorElementDataType GetOutputType(size_t /*index*/) const`
  - `CreateKernel` (function, line 431) `void* CreateKernel(const OrtApi& /*api*/,
                     const OrtKernelInfo* /*info*/) const`
  - `GetName` (function, line 435) `const char* GetName() const`
  - `GetInputTypeCount` (function, line 436) `size_t GetInputTypeCount() const`
  - `GetInputType` (function, line 437) `ONNXTensorElementDataType GetInputType(size_t /*index*/) const`
  - `GetOutputTypeCount` (function, line 440) `size_t GetOutputTypeCount() const`
  - `GetOutputType` (function, line 441) `ONNXTensorElementDataType GetOutputType(size_t /*index*/) const`
  - `zipvoice_domain` (function, line 457) `Ort::CustomOpDomain& zipvoice_domain()`
  - `zipvoice_register_custom_ops` (function, line 473) `void zipvoice_register_custom_ops(Ort::SessionOptions& opts)`
  - `wpacked` (function, line 230) `std::vector<float> wpacked(static_cast<size_t>(K * C));`
- Depends on: `core/moonshine-tts/src/zipvoice-custom-ops.h`

## core/moonshine-tts/src/zipvoice-custom-ops.h
- Doc: zipvoice_register_custom_ops: Registers the ``ai.zipvoice`` custom ONNX Runtime operators...
- Layer: utility
- Language: h
- Symbols:
  - `zipvoice_register_custom_ops` (function, line 15) `void zipvoice_register_custom_ops(Ort::SessionOptions& opts);`
  - `MOONSHINE_TTS_ZIPVOICE_CUSTOM_OPS_H` (macro, line 2) `#define MOONSHINE_TTS_ZIPVOICE_CUSTOM_OPS_H`
- Imported by: `core/moonshine-tts/src/zipvoice-custom-ops.cpp`, `core/moonshine-tts/src/zipvoice-tts.cpp`

## core/moonshine-tts/src/zipvoice-mel.cpp
- Doc: fft_radix2: Iterative radix-2 Cooley-Tukey FFT for power-of-two ``n`` (in-place, natural ->...
- Layer: utility
- Language: cpp
- Symbols:
  - `hz_to_bin_count` (function, line 12) `int hz_to_bin_count(int n_fft)`
  - `hz_to_mel_htk` (function, line 14) `double hz_to_mel_htk(double f)`
  - `mel_to_hz_htk` (function, line 15) `double mel_to_hz_htk(double m)`
  - `fft_radix2` (function, line 21) `void fft_radix2(std::vector<double>& re, std::vector<double>& im)`
  - `reflect_index` (function, line 64) `size_t reflect_index(long idx, long len)`
  - `VocosFbank` (function, line 81) `VocosFbank::VocosFbank()`
  - `num_frames_for` (function, line 132) `int VocosFbank::num_frames_for(size_t num_samples)`
  - `extract` (function, line 136) `std::vector<float> VocosFbank::extract(const std::vector<float>& samples,
                       ...`
  - `all_freqs` (function, line 93) `std::vector<double> all_freqs(static_cast<size_t>(n_freqs));`
  - `f_pts` (function, line 100) `std::vector<double> f_pts(static_cast<size_t>(kNMels + 2));`
  - `f_diff` (function, line 106) `std::vector<double> f_diff(static_cast<size_t>(kNMels + 1));`
  - `out` (function, line 145) `std::vector<float> out( static_cast<size_t>(frames) * static_cast<size_t>(kNMels), 0.F);`
  - `re` (function, line 151) `std::vector<double> re(static_cast<size_t>(kNFft));`
  - `im` (function, line 152) `std::vector<double> im(static_cast<size_t>(kNFft));`
  - `mag` (function, line 153) `std::vector<double> mag(static_cast<size_t>(n_freqs));`
- Depends on: `core/moonshine-tts/src/zipvoice-mel.h`

## core/moonshine-tts/src/zipvoice-mel.h
- Doc: VocosFbank: Log-mel feature frontend matching ZipVoice's ``VocosFbank``...
- Layer: utility
- Language: h
- Symbols:
  - `VocosFbank` (class, line 16)
  - `num_frames_for` (function, line 27) `static int num_frames_for(size_t num_samples);`
  - `extract` (function, line 32) `std::vector<float> extract(const std::vector<float>& samples, int* out_frames) const;`
  - `MOONSHINE_TTS_ZIPVOICE_MEL_H` (macro, line 2) `#define MOONSHINE_TTS_ZIPVOICE_MEL_H`
- Imported by: `core/moonshine-tts/src/zipvoice-mel.cpp`, `core/moonshine-tts/src/zipvoice-tts.cpp`, `core/moonshine-tts/tests/zipvoice-tts-test.cpp`

## core/moonshine-tts/src/zipvoice-tts.cpp
- Doc: resolve_zipvoice_lang: English-only for now; structured so more locales can be added.
- Layer: utility
- Language: cpp
- Symbols:
  - `Run` (struct, line 791)
  - `normalize_lang_key` (function, line 34) `std::string normalize_lang_key(std::string_view raw)`
  - `resolve_zipvoice_lang` (function, line 49) `void resolve_zipvoice_lang(const std::string& lang, std::string& g2p_dialect,
                   ...`
  - `resample_linear` (function, line 60) `std::vector<float> resample_linear(const std::vector<float>& x, int src_sr,
                     ...`
  - `trim_edge_silence` (function, line 87) `std::vector<float> trim_edge_silence(const std::vector<float>& wav,
                             ...`
  - `rms_of` (function, line 117) `float rms_of(const std::vector<float>& x)`
  - `get_time_steps` (function, line 130) `std::vector<float> get_time_steps(int num_step, float t_shift)`
  - `load_session` (function, line 218) `Ort::Session load_session(std::string_view key, bool register_custom_ops,
                       ...`
  - `load_asset_bytes` (function, line 256) `std::vector<uint8_t> load_asset_bytes(std::string_view key)`
  - `ipa_text_to_token_ids` (function, line 284) `std::vector<int64_t> ipa_text_to_token_ids(const std::string& text)`
  - `ipa_to_token_ids` (function, line 289) `std::vector<int64_t> ipa_to_token_ids(const std::string& ipa)`
  - `Impl` (function, line 306) `explicit Impl(const ZipVoiceTTSOptions& opt)`
  - `speed` (function, line 426) `double speed() const`
  - `set_speed` (function, line 427) `void set_speed(double s)`
  - `normalize_audio` (function, line 434) `bool normalize_audio() const`
  - `set_normalize_audio` (function, line 435) `void set_normalize_audio(bool on)`
  - `output_volume` (function, line 436) `float output_volume() const`
  - `set_output_volume` (function, line 437) `void set_output_volume(float v)`
  - `run_text_encoder` (function, line 441) `std::vector<float> run_text_encoder(const std::vector<int64_t>& tokens,
                         ...`
  - `sample_chunk` (function, line 489) `std::vector<float> sample_chunk(const std::vector<int64_t>& tokens,
                             ...`
  - `run_vocoder` (function, line 566) `std::vector<float> run_vocoder(const std::vector<float>& pred,
                                 i...`
  - `chunk_target_ids` (function, line 601) `std::vector<std::vector<int64_t>> chunk_target_ids(
      const std::vector<int64_t>& ids)`
  - `cross_fade_concat` (function, line 651) `static std::vector<float> cross_fade_concat(
      const std::vector<std::vector<float>>& chunks,...`
  - `synthesize` (function, line 691) `std::vector<float> synthesize(std::string_view text)`
  - `synthesize_from_ipa` (function, line 695) `std::vector<float> synthesize_from_ipa(std::string_view ipa)`
  - `synthesize_from_token_ids` (function, line 699) `std::vector<float> synthesize_from_token_ids(std::vector<int64_t> ids)`
  - `ZipVoiceTTS` (function, line 729) `ZipVoiceTTS::ZipVoiceTTS(const ZipVoiceTTSOptions& opt)
    : impl_(std::make_unique<Impl>(opt))`
  - `set_speed` (function, line 735) `void ZipVoiceTTS::set_speed(double speed)`
  - `speed` (function, line 736) `double ZipVoiceTTS::speed() const`
  - `normalize_audio` (function, line 737) `bool ZipVoiceTTS::normalize_audio() const`
  - `set_normalize_audio` (function, line 738) `void ZipVoiceTTS::set_normalize_audio(bool on)`
  - `output_volume` (function, line 741) `float ZipVoiceTTS::output_volume() const`
  - `set_output_volume` (function, line 742) `void ZipVoiceTTS::set_output_volume(float volume)`
  - `synthesize` (function, line 746) `std::vector<float> ZipVoiceTTS::synthesize(std::string_view text)`
  - `synthesize_from_ipa` (function, line 750) `std::vector<float> ZipVoiceTTS::synthesize_from_ipa(std::string_view ipa)`
  - `zipvoice_compress_long_pauses` (function, line 754) `std::vector<float> zipvoice_compress_long_pauses(const std::vector<float>& wav,
                 ...`
  - `y` (function, line 69) `std::vector<float> y(n_out);`
  - `out` (function, line 108) `std::vector<float> out(wav.begin() + static_cast<std::ptrdiff_t>(start), wav.begin() +...`
  - `ts` (function, line 131) `std::vector<float> ts(static_cast<size_t>(num_step + 1));`
  - `token` (function, line 158) `const std::string token(data + i, data + tab);`
  - `id_str` (function, line 159) `const std::string id_str(data + tab + 1, data + content_end);`
  - `k` (function, line 225) `const std::string k(key);`
  - `x` (function, line 501) `std::vector<float> x(total);`
  - `dist` (function, line 503) `std::normal_distribution<float> dist(0.F, 1.F);`
  - `speech_condition` (function, line 508) `std::vector<float> speech_condition(total, 0.F);`
  - `pred` (function, line 558) `std::vector<float> pred(static_cast<size_t>(gen_frames) * feat);`
  - `mel` (function, line 570) `std::vector<float> mel(static_cast<size_t>(gen_frames) * feat);`
  - `wav` (function, line 591) `std::vector<float> wav(n);`
  - `env` (function, line 764) `std::vector<float> env(wav.size(), 0.F);`
- Depends on: `core/moonshine-tts/src/g2p-path.h`, `core/moonshine-tts/src/ipa-postprocess.h`, `core/moonshine-tts/src/moonshine-g2p.h`, `core/moonshine-tts/src/moonshine-tts-options.h`, `core/moonshine-tts/src/ort-onnx-external-data.h`, `core/moonshine-tts/src/ort-session-options.h`, `core/moonshine-tts/src/utf8-utils.h`, `core/moonshine-tts/src/zipvoice-custom-ops.h`, `core/moonshine-tts/src/zipvoice-mel.h`, `core/moonshine-tts/src/zipvoice-tts.h`, `core/moonshine-tts/src/zipvoice-voices.h`, `core/moonshine-utils/debug-utils.h`

## core/moonshine-tts/src/zipvoice-tts.h
- Doc: ZipVoiceTTSOptions: Options for the ZipVoice zero-shot voice-cloning ONNX TTS engine.
- Layer: utility
- Language: h
- Symbols:
  - `ZipVoiceTTSOptions` (struct, line 20)
  - `Impl` (struct, line 93)
  - `ZipVoiceTTS` (class, line 65)
  - `set_speed` (function, line 76) `void set_speed(double speed);`
  - `speed` (function, line 77) `double speed() const;`
  - `normalize_audio` (function, line 78) `bool normalize_audio() const;`
  - `set_normalize_audio` (function, line 79) `void set_normalize_audio(bool on);`
  - `output_volume` (function, line 80) `float output_volume() const;`
  - `set_output_volume` (function, line 81) `void set_output_volume(float volume);`
  - `synthesize` (function, line 86) `std::vector<float> synthesize(std::string_view text);`
  - `synthesize_from_ipa` (function, line 90) `std::vector<float> synthesize_from_ipa(std::string_view ipa);`
  - `zipvoice_compress_long_pauses` (function, line 100) `std::vector<float> zipvoice_compress_long_pauses(const std::vector<float>& wav, int sample_rate, float...`
  - `MOONSHINE_TTS_ZIPVOICE_TTS_H` (macro, line 2) `#define MOONSHINE_TTS_ZIPVOICE_TTS_H`
- Depends on: `core/moonshine-tts/src/file-information.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`
- Imported by: `core/moonshine-tts/src/moonshine-tts.cpp`, `core/moonshine-tts/src/zipvoice-tts.cpp`, `core/moonshine-tts/tests/zipvoice-tts-test.cpp`

## core/moonshine-tts/src/zipvoice-voices-data.cpp
- Layer: data_access
- Language: cpp

## core/moonshine-tts/src/zipvoice-voices.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `zipvoice_find_builtin_voice` (function, line 7) `const ZipVoiceBuiltinVoice* zipvoice_find_builtin_voice(std::string_view id)`
  - `zipvoice_builtin_voice_pcm_to_float` (function, line 18) `std::vector<float> zipvoice_builtin_voice_pcm_to_float(
    const ZipVoiceBuiltinVoice& voice)`
  - `out` (function, line 20) `std::vector<float> out(voice.num_samples);`
- Depends on: `core/moonshine-tts/src/zipvoice-voices.h`

## core/moonshine-tts/src/zipvoice-voices.h
- Doc: ZipVoiceBuiltinVoice: One built-in ZipVoice reference voice to clone, sourced from the VCTK...
- Layer: utility
- Language: h
- Symbols:
  - `ZipVoiceBuiltinVoice` (struct, line 17)
  - `zipvoice_builtin_voices` (function, line 30) `const ZipVoiceBuiltinVoice* zipvoice_builtin_voices(size_t* count);`
  - `zipvoice_find_builtin_voice` (function, line 34) `const ZipVoiceBuiltinVoice* zipvoice_find_builtin_voice(std::string_view id);`
  - `zipvoice_builtin_voice_pcm_to_float` (function, line 38) `std::vector<float> zipvoice_builtin_voice_pcm_to_float( const ZipVoiceBuiltinVoice& voice);`
  - `MOONSHINE_TTS_ZIPVOICE_VOICES_H` (macro, line 2) `#define MOONSHINE_TTS_ZIPVOICE_VOICES_H`
- Imported by: `core/moonshine-tts/src/moonshine-tts.cpp`, `core/moonshine-tts/src/zipvoice-tts.cpp`, `core/moonshine-tts/src/zipvoice-voices.cpp`, `core/moonshine-tts/tests/zipvoice-tts-test.cpp`

