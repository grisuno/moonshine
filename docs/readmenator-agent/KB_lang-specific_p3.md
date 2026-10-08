# Subsystem: lang-specific (page 3 of 4)
Previous: [KB_lang-specific_p2.md](KB_lang-specific_p2.md)

## core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `utf8_nfc_utf8proc` (function, line 22) `std::string utf8_nfc_utf8proc(std::string_view s)`
  - `is_han_cp` (function, line 34) `bool is_han_cp(char32_t cp)`
  - `is_single_han` (function, line 40) `bool is_single_han(std::string_view s)`
  - `only_hiragana` (function, line 45) `bool only_hiragana(std::string_view s)`
  - `only_katakana` (function, line 58) `bool only_katakana(std::string_view s)`
  - `only_han` (function, line 74) `bool only_han(std::string_view s)`
  - `trailing_particles_sorted` (function, line 176) `const std::vector<std::string>& trailing_particles_sorted()`
  - `sort` (function, line 183) `std::sort(v.begin(), v.end(),
              [](const std::string& a, const std::string& b)`
  - `build_by_first` (function, line 228) `void build_by_first(
    const std::unordered_map<std::string, std::string>& lex,
    std::unorde...`
  - `sort` (function, line 246) `std::sort(vec.begin(), vec.end(),
              [](const std::string& a, const std::string& b)`
  - `default_japanese_dict_path` (function, line 255) `std::filesystem::path default_japanese_dict_path(
    const std::filesystem::path& g2p_data_root)`
  - `JapaneseOnnxG2p` (function, line 260) `JapaneseOnnxG2p::JapaneseOnnxG2p(std::filesystem::path model_dir,
                               ...`
  - `JapaneseOnnxG2p` (function, line 267) `JapaneseOnnxG2p::JapaneseOnnxG2p(std::filesystem::path model_dir,
                               ...`
  - `JapaneseOnnxG2p` (function, line 275) `JapaneseOnnxG2p::JapaneseOnnxG2p(const MoonshineG2POptions& opt,
                                ...`
  - `JapaneseOnnxG2p` (function, line 283) `JapaneseOnnxG2p::JapaneseOnnxG2p(const MoonshineG2POptions& opt,
                                ...`
  - `g2p_word` (function, line 292) `std::string JapaneseOnnxG2p::g2p_word(std::string word_utf8)`
  - `text_to_ipa` (function, line 357) `std::string JapaneseOnnxG2p::text_to_ipa(std::string text_utf8)`
  - `tmp` (function, line 23) `const std::string tmp(s);`
- Depends on: `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.h`, `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.h
- Doc: JapaneseOnnxG2p: ONNX LUW segmentation + ``data/ja/dict.tsv`` + kana IPA (mirrors...
- Layer: testing
- Language: h
- Symbols:
  - `MoonshineG2POptions` (struct, line 13)
  - `JapaneseOnnxG2p` (class, line 17)
  - `tok` (function, line 34) `const JapaneseTokPosOnnx& tok() const`
  - `MOONSHINE_TTS_JAPANESE_ONNX_G2P_H` (macro, line 2) `#define MOONSHINE_TTS_JAPANESE_ONNX_G2P_H`
- Depends on: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.h`
- Imported by: `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp`, `core/moonshine-tts/src/lang-specific/japanese.cpp`, `core/moonshine-tts/tests/japanese-onnx-g2p-test.cpp`, `core/moonshine-tts/tools/japanese-onnx-g2p-cli.cpp`

## core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp
- Doc: is_punct_char_word_group_u32: ``token_word_group_indices`` uses :func:`_is_punct_char` (Unicode...
- Layer: testing
- Language: cpp
- Symbols:
  - `BasicTokCfg` (struct, line 311)
  - `EncodedWp` (struct, line 423)
  - `Idx` (struct, line 513)
  - `open_session` (function, line 31) `std::unique_ptr<Ort::Session> open_session(
    Ort::Env& env, const std::filesystem::path& model...`
  - `open_session_memory` (function, line 48) `std::unique_ptr<Ort::Session> open_session_memory(
    Ort::Env& env, const void* data, size_t le...`
  - `slurp_utf8_file` (function, line 62) `std::string slurp_utf8_file(const std::filesystem::path& p)`
  - `bundle_load_utf8` (function, line 72) `bool bundle_load_utf8(const MoonshineG2POptions* opt,
                      std::string_view bund...`
  - `bundle_load_binary` (function, line 90) `bool bundle_load_binary(const MoonshineG2POptions* opt,
                        std::string_view ...`
  - `utf8_to_u32` (function, line 123) `std::u32string utf8_to_u32(std::string_view utf8)`
  - `u32_to_utf8` (function, line 136) `std::string u32_to_utf8(const std::u32string& s)`
  - `is_space_u32` (function, line 144) `bool is_space_u32(char32_t c)`
  - `is_control_u32` (function, line 153) `bool is_control_u32(char32_t c)`
  - `is_punctuation_u32` (function, line 162) `bool is_punctuation_u32(char32_t c)`
  - `is_punct_char_word_group_u32` (function, line 175) `bool is_punct_char_word_group_u32(char32_t c)`
  - `is_chinese_char` (function, line 180) `bool is_chinese_char(std::uint32_t cp)`
  - `u32_nfc` (function, line 189) `std::u32string u32_nfc(const std::u32string& s)`
  - `strip_mn_nfd` (function, line 201) `std::u32string strip_mn_nfd(const std::u32string& s)`
  - `to_lower_u32` (function, line 221) `std::u32string to_lower_u32(const std::u32string& s)`
  - `clean_text_u32` (function, line 230) `std::u32string clean_text_u32(const std::u32string& text)`
  - `tokenize_chinese_chars_u32` (function, line 242) `std::u32string tokenize_chinese_chars_u32(const std::u32string& text)`
  - `split_u32_whitespace` (function, line 256) `std::vector<std::u32string> split_u32_whitespace(std::u32string_view s)`
  - `run_split_on_punc_u32` (function, line 281) `std::vector<std::u32string> run_split_on_punc_u32(const std::u32string& text)`
  - `normalization_ref_u32` (function, line 317) `std::u32string normalization_ref_u32(const std::u32string& text_u32,
                            ...`
  - `basic_tokenize_u32` (function, line 326) `std::vector<std::u32string> basic_tokenize_u32(
    const std::u32string& original_text_u32, cons...`
  - `align_basic_tokens_u32` (function, line 358) `void align_basic_tokens_u32(const std::u32string& ref,
                            const std::vec...`
  - `wordpiece_tokenize_u32` (function, line 375) `std::vector<std::u32string> wordpiece_tokenize_u32(
    const std::u32string& token,
    const st...`
  - `encode_bert_wordpiece` (function, line 430) `EncodedWp encode_bert_wordpiece(
    const std::u32string& text_u32,
    const std::unordered_map...`
  - `ud_upos_set` (function, line 598) `const std::unordered_set<std::string>& ud_upos_set()`
  - `morph_label_to_upos` (function, line 606) `std::string morph_label_to_upos(std::string label)`
  - `cjk_tokpos_preferred_chunk_break_cp` (function, line 650) `bool cjk_tokpos_preferred_chunk_break_cp(char32_t c)`
  - `cjk_tokpos_chunk_exclusive_end` (function, line 684) `template <typename EncodeFn>
std::size_t cjk_tokpos_chunk_exclusive_end(const std::u32string& ful...`
  - `default_japanese_tok_pos_model_dir` (function, line 722) `std::filesystem::path default_japanese_tok_pos_model_dir(
    const std::filesystem::path& g2p_da...`
  - `JapaneseTokPosOnnx` (function, line 732) `JapaneseTokPosOnnx::JapaneseTokPosOnnx(const MoonshineG2POptions* opt,
                          ...`
  - `format_annotated_line` (function, line 793) `std::string JapaneseTokPosOnnx::format_annotated_line(
    const std::vector<std::pair<std::strin...`
  - `chars` (function, line 385) `std::vector<char32_t> chars(wt.begin(), wt.end());`
  - `buf` (function, line 645) `const std::string buf(utf8);`
  - `mask` (function, line 849) `std::vector<int64_t> mask(static_cast<size_t>(T), 1);`
  - `pooled` (function, line 883) `std::vector<double> pooled(static_cast<size_t>(num_labels), 0.0);`
- Depends on: `core/moonshine-tts/src/g2p-path.h`, `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-tts/src/ort-onnx-external-data.h`, `core/moonshine-tts/src/ort-session-options.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.h
- Doc: JapaneseTokPosOnnx: Japanese LUW surfaces + UD UPOS via ONNX...
- Layer: testing
- Language: h
- Symbols:
  - `MoonshineG2POptions` (struct, line 16)
  - `JapaneseTokPosOnnx` (class, line 23)
  - `model_dir` (function, line 42) `const std::filesystem::path& model_dir() const`
  - `format_annotated_line` (function, line 39) `static std::string format_annotated_line( const std::vector<std::pair<std::string, std::string>>& pairs);`
  - `MOONSHINE_TTS_JAPANESE_TOK_POS_ONNX_H` (macro, line 2) `#define MOONSHINE_TTS_JAPANESE_TOK_POS_ONNX_H`
- Imported by: `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.h`, `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp`, `core/moonshine-tts/tests/japanese-tok-pos-onnx-test.cpp`

## core/moonshine-tts/src/lang-specific/japanese.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `absolute_model_root` (function, line 16) `std::filesystem::path absolute_model_root(
    const std::filesystem::path& model_root)`
  - `JapaneseRuleG2p` (function, line 32) `JapaneseRuleG2p::JapaneseRuleG2p(std::filesystem::path onnx_model_dir,
                          ...`
  - `JapaneseRuleG2p` (function, line 37) `JapaneseRuleG2p::JapaneseRuleG2p(std::filesystem::path onnx_model_dir,
                          ...`
  - `JapaneseRuleG2p` (function, line 42) `JapaneseRuleG2p::JapaneseRuleG2p(const MoonshineG2POptions& opt,
                                ...`
  - `JapaneseRuleG2p` (function, line 48) `JapaneseRuleG2p::JapaneseRuleG2p(const MoonshineG2POptions& opt,
                                ...`
  - `text_to_ipa` (function, line 61) `std::string JapaneseRuleG2p::text_to_ipa(
    std::string text, std::vector<G2pWordLog>* per_word...`
  - `dialect_ids` (function, line 67) `std::vector<std::string> JapaneseRuleG2p::dialect_ids()`
  - `dialect_resolves_to_japanese_rules` (function, line 72) `bool dialect_resolves_to_japanese_rules(std::string_view dialect_id)`
  - `resolve_japanese_dict_path` (function, line 80) `std::filesystem::path resolve_japanese_dict_path(
    const std::filesystem::path& model_root)`
  - `resolve_japanese_onnx_model_dir` (function, line 86) `std::filesystem::path resolve_japanese_onnx_model_dir(
    const std::filesystem::path& model_root)`
- Depends on: `core/moonshine-tts/src/g2p-path.h`, `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.h`, `core/moonshine-tts/src/lang-specific/japanese.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/japanese.h
- Doc: JapaneseRuleG2p: Japanese G2P via ONNX LUW segmentation + ``data/ja/dict.tsv`` (mirrors...
- Layer: testing
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 14)
  - `MoonshineG2POptions` (struct, line 15)
  - `JapaneseRuleG2p` (class, line 21)
  - `dialect_id` (function, line 43) `const std::string& dialect_id() const`
  - `dialect_ids` (function, line 41) `static std::vector<std::string> dialect_ids();`
  - `dialect_resolves_to_japanese_rules` (function, line 54) `bool dialect_resolves_to_japanese_rules(std::string_view dialect_id);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_JAPANESE_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_JAPANESE_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/japanese.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`

## core/moonshine-tts/src/lang-specific/korean-numbers.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `is_ascii_digit` (function, line 21) `bool is_ascii_digit(char c)`
  - `thousands_lookahead_ok` (function, line 23) `bool thousands_lookahead_ok(std::string_view suf)`
  - `strip_thousands_commas` (function, line 39) `std::string strip_thousands_commas(std::string_view raw)`
  - `normalize_numeral_token_string` (function, line 52) `std::string normalize_numeral_token_string(std::string_view raw)`
  - `hangul_digits_only` (function, line 66) `std::string hangul_digits_only(std::string_view s)`
  - `section_under_10000` (function, line 76) `std::string section_under_10000(unsigned n)`
  - `parse_uint_strict` (function, line 124) `bool parse_uint_strict(std::string_view sv, std::uint64_t& out)`
  - `int_to_sino_korean_hangul` (function, line 147) `std::string int_to_sino_korean_hangul(std::uint64_t n)`
  - `korean_reading_fragments_from_ascii_numeral_token` (function, line 189) `std::optional<std::vector<std::string>>
korean_reading_fragments_from_ascii_numeral_token(std::st...`
  - `is_ascii_numeral_token` (function, line 287) `bool is_ascii_numeral_token(std::string_view token)`
  - `gs` (function, line 160) `std::vector<unsigned> gs(low_first.rbegin(), low_first.rend());`
- Depends on: `core/moonshine-tts/src/lang-specific/korean-numbers.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/korean-numbers.h
- Layer: testing
- Language: h
- Symbols:
  - `is_ascii_numeral_token` (function, line 22) `bool is_ascii_numeral_token(std::string_view token);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_KOREAN_NUMBERS_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_KOREAN_NUMBERS_H`
- Imported by: `core/moonshine-tts/src/lang-specific/korean-numbers.cpp`, `core/moonshine-tts/src/lang-specific/korean.cpp`, `core/moonshine-tts/tests/korean-rule-g2p-test.cpp`

## core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp
- Doc: is_punct_char_word_group_u32: ``token_word_group_indices`` uses :func:`_is_punct_char` (Unicode...
- Layer: testing
- Language: cpp
- Symbols:
  - `BasicTokCfg` (struct, line 311)
  - `EncodedWp` (struct, line 423)
  - `Idx` (struct, line 513)
  - `open_session` (function, line 31) `std::unique_ptr<Ort::Session> open_session(
    Ort::Env& env, const std::filesystem::path& model...`
  - `open_session_memory` (function, line 48) `std::unique_ptr<Ort::Session> open_session_memory(
    Ort::Env& env, const void* data, size_t le...`
  - `slurp_utf8_file` (function, line 62) `std::string slurp_utf8_file(const std::filesystem::path& p)`
  - `bundle_load_utf8` (function, line 72) `bool bundle_load_utf8(const MoonshineG2POptions* opt,
                      std::string_view bund...`
  - `bundle_load_binary` (function, line 90) `bool bundle_load_binary(const MoonshineG2POptions* opt,
                        std::string_view ...`
  - `utf8_to_u32` (function, line 123) `std::u32string utf8_to_u32(std::string_view utf8)`
  - `u32_to_utf8` (function, line 136) `std::string u32_to_utf8(const std::u32string& s)`
  - `is_space_u32` (function, line 144) `bool is_space_u32(char32_t c)`
  - `is_control_u32` (function, line 153) `bool is_control_u32(char32_t c)`
  - `is_punctuation_u32` (function, line 162) `bool is_punctuation_u32(char32_t c)`
  - `is_punct_char_word_group_u32` (function, line 175) `bool is_punct_char_word_group_u32(char32_t c)`
  - `is_chinese_char` (function, line 180) `bool is_chinese_char(std::uint32_t cp)`
  - `u32_nfc` (function, line 189) `std::u32string u32_nfc(const std::u32string& s)`
  - `strip_mn_nfd` (function, line 201) `std::u32string strip_mn_nfd(const std::u32string& s)`
  - `to_lower_u32` (function, line 221) `std::u32string to_lower_u32(const std::u32string& s)`
  - `clean_text_u32` (function, line 230) `std::u32string clean_text_u32(const std::u32string& text)`
  - `tokenize_chinese_chars_u32` (function, line 242) `std::u32string tokenize_chinese_chars_u32(const std::u32string& text)`
  - `split_u32_whitespace` (function, line 256) `std::vector<std::u32string> split_u32_whitespace(std::u32string_view s)`
  - `run_split_on_punc_u32` (function, line 281) `std::vector<std::u32string> run_split_on_punc_u32(const std::u32string& text)`
  - `normalization_ref_u32` (function, line 317) `std::u32string normalization_ref_u32(const std::u32string& text_u32,
                            ...`
  - `basic_tokenize_u32` (function, line 326) `std::vector<std::u32string> basic_tokenize_u32(
    const std::u32string& original_text_u32, cons...`
  - `align_basic_tokens_u32` (function, line 358) `void align_basic_tokens_u32(const std::u32string& ref,
                            const std::vec...`
  - `wordpiece_tokenize_u32` (function, line 375) `std::vector<std::u32string> wordpiece_tokenize_u32(
    const std::u32string& token,
    const st...`
  - `encode_bert_wordpiece` (function, line 430) `EncodedWp encode_bert_wordpiece(
    const std::u32string& text_u32,
    const std::unordered_map...`
  - `ud_upos_set` (function, line 598) `const std::unordered_set<std::string>& ud_upos_set()`
  - `morph_label_to_upos` (function, line 606) `std::string morph_label_to_upos(std::string label)`
  - `cjk_tokpos_preferred_chunk_break_cp` (function, line 650) `bool cjk_tokpos_preferred_chunk_break_cp(char32_t c)`
  - `cjk_tokpos_chunk_exclusive_end` (function, line 684) `template <typename EncodeFn>
std::size_t cjk_tokpos_chunk_exclusive_end(const std::u32string& ful...`
  - `default_korean_tok_pos_model_dir` (function, line 722) `std::filesystem::path default_korean_tok_pos_model_dir(
    const std::filesystem::path& g2p_data...`
  - `KoreanTokPosOnnx` (function, line 732) `KoreanTokPosOnnx::KoreanTokPosOnnx(const MoonshineG2POptions* opt,
                              ...`
  - `format_annotated_line` (function, line 792) `std::string KoreanTokPosOnnx::format_annotated_line(
    const std::vector<std::pair<std::string,...`
  - `chars` (function, line 385) `std::vector<char32_t> chars(wt.begin(), wt.end());`
  - `buf` (function, line 645) `const std::string buf(utf8);`
  - `mask` (function, line 848) `std::vector<int64_t> mask(static_cast<size_t>(T), 1);`
  - `pooled` (function, line 882) `std::vector<double> pooled(static_cast<size_t>(num_labels), 0.0);`
- Depends on: `core/moonshine-tts/src/g2p-path.h`, `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-tts/src/ort-onnx-external-data.h`, `core/moonshine-tts/src/ort-session-options.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.h
- Doc: KoreanTokPosOnnx: Korean whitespace-level words + UD UPOS via ONNX...
- Layer: testing
- Language: h
- Symbols:
  - `MoonshineG2POptions` (struct, line 16)
  - `KoreanTokPosOnnx` (class, line 23)
  - `model_dir` (function, line 42) `const std::filesystem::path& model_dir() const`
  - `format_annotated_line` (function, line 39) `static std::string format_annotated_line( const std::vector<std::pair<std::string, std::string>>& pairs);`
  - `MOONSHINE_TTS_KOREAN_TOK_POS_ONNX_H` (macro, line 2) `#define MOONSHINE_TTS_KOREAN_TOK_POS_ONNX_H`
- Imported by: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp`, `core/moonshine-tts/tests/korean-tok-pos-onnx-test.cpp`

## core/moonshine-tts/src/lang-specific/korean.cpp
- Doc: is_sonorant_jong: Sonorant codas: nasals (ㄴ,ㅁ,ŋ) and liquids (ㄹ and ㄹ-clusters).
- Layer: testing
- Language: cpp
- Symbols:
  - `Syllable` (struct, line 55)
  - `replace_all` (function, line 61) `void replace_all(std::string& s, const std::string& from,
                 const std::string& to)`
  - `utf8_nfc_utf8proc` (function, line 72) `std::string utf8_nfc_utf8proc(std::string_view s)`
  - `strip_mn_after_nfd` (function, line 84) `std::string strip_mn_after_nfd(const std::string& ipa)`
  - `is_sonorant_jong` (function, line 175) `bool is_sonorant_jong(int jong)`
  - `jong_triggers_tense` (function, line 183) `bool jong_triggers_tense(int jong)`
  - `tense_cho` (function, line 204) `int tense_cho(int plain_cho)`
  - `decompose_syllable_cp` (function, line 221) `std::optional<Syllable> decompose_syllable_cp(char32_t ch)`
  - `text_to_syllables` (function, line 233) `std::vector<Syllable> text_to_syllables(std::string_view text)`
  - `apply_linking` (function, line 249) `void apply_linking(std::vector<Syllable>& syls)`
  - `apply_lateralization` (function, line 277) `void apply_lateralization(std::vector<Syllable>& syls)`
  - `ipa_onset` (function, line 291) `std::string ipa_onset(int cho, bool tense, bool aspirate)`
  - `ipa_nucleus` (function, line 376) `std::string ipa_nucleus(int jung)`
  - `ipa_coda_simple` (function, line 389) `std::string ipa_coda_simple(int jong)`
  - `coda_nasal_assimilate` (function, line 425) `std::string coda_nasal_assimilate(int jong, std::optional<int> next_cho)`
  - `syllables_to_ipa` (function, line 447) `std::string syllables_to_ipa(const std::vector<Syllable>& syls,
                             std:...`
  - `sino_cardinal_speech_units` (function, line 550) `std::vector<std::string> sino_cardinal_speech_units(std::uint64_t n)`
  - `g2p_hangul_rules_only_inner` (function, line 578) `std::string g2p_hangul_rules_only_inner(std::string_view hangul,
                                ...`
  - `normalize_korean_ipa` (function, line 594) `std::string KoreanRuleG2p::normalize_korean_ipa(std::string ipa,
                                ...`
  - `extract_hangul` (function, line 723) `std::string KoreanRuleG2p::extract_hangul(std::string_view s) const`
  - `g2p_hangul_rules_only` (function, line 739) `std::string KoreanRuleG2p::g2p_hangul_rules_only(
    std::string_view hangul) const`
  - `g2p_single_fragment` (function, line 752) `std::string KoreanRuleG2p::g2p_single_fragment(std::string_view frag) const`
  - `load_korean_lexicon_stream` (function, line 775) `void load_korean_lexicon_stream(
    std::istream& in, std::unordered_map<std::string, std::strin...`
  - `KoreanRuleG2p` (function, line 804) `KoreanRuleG2p::KoreanRuleG2p(std::filesystem::path dict_tsv, Options options)
    : options_(std:...`
  - `KoreanRuleG2p` (function, line 818) `KoreanRuleG2p::KoreanRuleG2p(std::string dict_tsv_utf8, Options options)
    : options_(std::move...`
  - `text_to_ipa` (function, line 824) `std::string KoreanRuleG2p::text_to_ipa(std::string text,
                                       s...`
  - `dialect_ids` (function, line 1036) `std::vector<std::string> KoreanRuleG2p::dialect_ids()`
  - `dialect_resolves_to_korean_rules` (function, line 1041) `bool dialect_resolves_to_korean_rules(std::string_view dialect_id)`
  - `resolve_korean_dict_path` (function, line 1049) `std::filesystem::path resolve_korean_dict_path(
    const std::filesystem::path& model_root)`
  - `tmp` (function, line 73) `const std::string tmp(s);`
  - `nfd_str` (function, line 90) `const std::string nfd_str(reinterpret_cast<char*>(nfd));`
  - `num_sv` (function, line 985) `const std::string num_sv(w, 0, num_end);`
  - `0xAC00` (variable, line 20) `extern "C" { #include <utf8proc.h> } namespace moonshine_tts { namespace { constexpr char32_t kHangulBase = 0xAC00;`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/korean-numbers.h`, `core/moonshine-tts/src/lang-specific/korean.h`, `core/moonshine-tts/src/utf8-utils.h`, `core/moonshine-utils/debug-utils.h`

## core/moonshine-tts/src/lang-specific/korean.h
- Doc: KoreanRuleG2p: Lexicon + Hangul rule G2P (연음, 유음화, 비음화, ㅎ aspiration, 경음화), mirroring...
- Layer: testing
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 15)
  - `Options` (struct, line 21)
  - `KoreanRuleG2p` (class, line 19)
  - `dialect_id` (function, line 35) `const std::string& dialect_id() const`
  - `dialect_ids` (function, line 33) `static std::vector<std::string> dialect_ids();`
  - `normalize_korean_ipa` (function, line 43) `static std::string normalize_korean_ipa(std::string ipa, bool voice_lenis = true);`
  - `dialect_resolves_to_korean_rules` (function, line 60) `bool dialect_resolves_to_korean_rules(std::string_view dialect_id);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_KOREAN_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_KOREAN_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/korean.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/korean-rule-g2p-test.cpp`, `core/moonshine-tts/tools/korean-rule-g2p-cli.cpp`

## core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp
- Layer: business_logic
- Language: cpp
- Symbols:
  - `open_session` (function, line 21) `Ort::Session open_session(Ort::Env& env,
                          const std::filesystem::path& m...`
  - `open_session_memory` (function, line 38) `Ort::Session open_session_memory(Ort::Env& env, const void* data, size_t len,
                   ...`
  - `encode_chars_for_model` (function, line 46) `std::vector<int64_t> encode_chars_for_model(
    const std::string& text,
    const std::unordere...`
  - `decoder_io_padded` (function, line 58) `void decoder_io_padded(const std::vector<int64_t>& cur, int max_phoneme_len,
                    ...`
  - `argmax_vocab_row` (function, line 73) `int argmax_vocab_row(const float* logits, int64_t vocab, int time_index)`
  - `OnnxOovG2p` (function, line 90) `OnnxOovG2p::OnnxOovG2p(Ort::Env& env, const std::filesystem::path& model_onnx,
                  ...`
  - `OnnxOovG2p` (function, line 97) `OnnxOovG2p::OnnxOovG2p(Ort::Env& env, const void* model_onnx_bytes,
                       size_t...`
  - `predict_phonemes` (function, line 106) `std::vector<std::string> OnnxOovG2p::predict_phonemes(const std::string& word)`
  - `enc_ids` (function, line 115) `std::vector<int64_t> enc_ids(static_cast<size_t>(tab_.max_seq_len), tab_.pad_id);`
  - `enc_mask` (function, line 117) `std::vector<int64_t> enc_mask(static_cast<size_t>(tab_.max_seq_len), 0);`
- Depends on: `core/moonshine-tts/src/constants.h`, `core/moonshine-tts/src/lang-specific/onnx-g2p-models.h`, `core/moonshine-tts/src/ort-session-options.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/onnx-g2p-models.h
- Layer: business_logic
- Language: h
- Symbols:
  - `OnnxOovG2p` (class, line 17)
  - `MOONSHINE_TTS_ONNX_G2P_MODELS_H` (macro, line 2) `#define MOONSHINE_TTS_ONNX_G2P_MODELS_H`
- Depends on: `core/moonshine-tts/src/json-config.h`
- Imported by: `core/moonshine-tts/src/lang-specific/english.cpp`, `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp`

## core/moonshine-tts/src/lang-specific/portuguese-rules.cpp
- Layer: business_logic
- Language: cpp
- Symbols:
  - `pt_tolower` (function, line 24) `char32_t pt_tolower(char32_t c)`
  - `is_pt_key_cp` (function, line 69) `bool is_pt_key_cp(char32_t c)`
  - `normalize_lookup_key_utf8_impl` (function, line 85) `std::string normalize_lookup_key_utf8_impl(const std::string& word)`
  - `normalize_lookup_key_utf8` (function, line 106) `std::string normalize_lookup_key_utf8(const std::string& word)`
  - `utf8_to_u32_pt` (function, line 110) `std::u32string utf8_to_u32_pt(const std::string& s)`
  - `u32_to_utf8_pt` (function, line 114) `std::string u32_to_utf8_pt(const std::u32string& s)`
  - `is_allowed_pt_grapheme` (function, line 122) `bool is_allowed_pt_grapheme(char32_t c)`
  - `filter_pt_word_graphemes_utf8` (function, line 135) `std::u32string filter_pt_word_graphemes_utf8(const std::string& word)`
  - `is_vowel_pt_u32` (function, line 151) `bool is_vowel_pt_u32(char32_t ch)`
  - `strip_accent_base_pt` (function, line 159) `char32_t strip_accent_base_pt(char32_t c)`
  - `should_hiatus_pt_u32` (function, line 186) `bool should_hiatus_pt_u32(char32_t a, char32_t b)`
  - `valid_onset2_end_u32` (function, line 261) `bool valid_onset2_end_u32(char32_t a, char32_t b)`
  - `port_orthographic_syllables_u32` (function, line 297) `std::vector<std::u32string> port_orthographic_syllables_u32(
    const std::u32string& w0)`
  - `accented_syllable_u32` (function, line 352) `bool accented_syllable_u32(const std::u32string& s)`
  - `default_stressed_syllable_index_u32` (function, line 362) `size_t default_stressed_syllable_index_u32(
    const std::vector<std::u32string>& syls, const st...`
  - `strip_stress_chars` (function, line 424) `std::string strip_stress_chars(std::string s)`
  - `insert_primary_stress_before_vowel_utf8` (function, line 430) `std::string insert_primary_stress_before_vowel_utf8(std::string ipa)`
  - `roman_to_int_ascii` (function, line 453) `std::optional<int> roman_to_int_ascii(std::string_view u)`
  - `roman_numeral_token_to_ipa` (function, line 491) `std::optional<std::string> roman_numeral_token_to_ipa(
    const std::string& letters_lower, bool...`
  - `prev_global_vowel_u32` (function, line 549) `bool prev_global_vowel_u32(const std::u32string& full_word, size_t gidx)`
  - `next_global_vowel_u32` (function, line 569) `bool next_global_vowel_u32(const std::u32string& full_word, size_t gidx)`
  - `syllable_has_u32` (function, line 585) `bool syllable_has_u32(const std::u32string& s, char32_t ch)`
  - `letters_to_ipa_no_stress_u32` (function, line 589) `std::string letters_to_ipa_no_stress_u32(const std::u32string& s, bool is_pt_pt,
                ...`
  - `rules_word_to_ipa_single_u32` (function, line 964) `std::string rules_word_to_ipa_single_u32(const std::u32string& wl,
                              ...`
  - `vowel_grapheme_tail_pt` (function, line 1018) `bool vowel_grapheme_tail_pt(char32_t c)`
  - `pt_pt_apply_rules_final_s_to_esh` (function, line 1026) `std::string pt_pt_apply_rules_final_s_to_esh(std::string ipa,
                                   ...`
  - `rules_word_to_ipa_utf8` (function, line 1161) `std::string rules_word_to_ipa_utf8(const std::string& raw, bool is_pt_pt,
                       ...`
- Depends on: `core/moonshine-tts/src/lang-specific/ipa-symbols.h`, `core/moonshine-tts/src/lang-specific/portuguese-rules.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/portuguese-rules.h
- Layer: business_logic
- Language: h
- Symbols:
  - `pt_tolower` (function, line 11) `char32_t pt_tolower(char32_t c);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_PORTUGUESE_RULES_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_PORTUGUESE_RULES_H`
- Imported by: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp`, `core/moonshine-tts/src/lang-specific/portuguese.cpp`

## core/moonshine-tts/src/lang-specific/portuguese.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `utf8_lowercase_pt_surface` (function, line 39) `std::string utf8_lowercase_pt_surface(const std::string& word)`
  - `load_pt_lexicon_stream` (function, line 52) `void load_pt_lexicon_stream(std::istream& in,
                            std::unordered_map<std:...`
  - `load_pt_lexicon_file` (function, line 84) `void load_pt_lexicon_file(const std::filesystem::path& path,
                          std::unord...`
  - `is_all_ascii_digits` (function, line 97) `bool is_all_ascii_digits(std::string_view s)`
  - `teens_word_pt` (function, line 121) `std::string teens_word_pt(int n, bool is_pt_pt)`
  - `under_100_tokens_pt` (function, line 173) `void under_100_tokens_pt(int n, bool is_pt_pt, std::vector<std::string>& out)`
  - `below_1000_tokens_pt` (function, line 200) `void below_1000_tokens_pt(int n, bool is_pt_pt, std::vector<std::string>& out)`
  - `below_1_000_000_tokens_pt` (function, line 228) `void below_1_000_000_tokens_pt(int n, bool is_pt_pt,
                               std::vector<s...`
  - `expand_cardinal_digits_to_portuguese_words` (function, line 252) `std::string expand_cardinal_digits_to_portuguese_words(std::string_view s,
                      ...`
  - `expand_digit_tokens_in_text` (function, line 289) `std::string expand_digit_tokens_in_text(std::string text, bool is_pt_pt)`
  - `is_pt_word_char` (function, line 322) `bool is_pt_word_char(char32_t cp)`
  - `try_consume_pt_word` (function, line 355) `bool try_consume_pt_word(const std::string& text, size_t pos, size_t& out_end)`
  - `PortugueseRuleG2p` (function, line 411) `PortugueseRuleG2p::PortugueseRuleG2p(std::filesystem::path dict_tsv,
                            ...`
  - `PortugueseRuleG2p` (function, line 418) `PortugueseRuleG2p::PortugueseRuleG2p(std::string dict_tsv_utf8,
                                 ...`
  - `finalize_ipa` (function, line 426) `std::string PortugueseRuleG2p::finalize_ipa(std::string ipa,
                                    ...`
  - `lookup_or_rules` (function, line 445) `std::string PortugueseRuleG2p::lookup_or_rules(
    const std::string& raw_word) const`
  - `word_to_ipa` (function, line 508) `std::string PortugueseRuleG2p::word_to_ipa(const std::string& word) const`
  - `text_to_ipa_no_expand` (function, line 531) `std::string PortugueseRuleG2p::text_to_ipa_no_expand(
    const std::string& text, std::vector<G2...`
  - `text_to_ipa` (function, line 601) `std::string PortugueseRuleG2p::text_to_ipa(
    std::string text, std::vector<G2pWordLog>* per_wo...`
  - `dialect_resolves_to_portugal_rules` (function, line 609) `bool dialect_resolves_to_portugal_rules(std::string_view dialect_id)`
  - `dialect_resolves_to_brazilian_portuguese_rules` (function, line 618) `bool dialect_resolves_to_brazilian_portuguese_rules(
    std::string_view dialect_id)`
  - `dialect_ids` (function, line 628) `std::vector<std::string> PortugueseRuleG2p::dialect_ids()`
  - `resolve_portuguese_dict_path` (function, line 635) `std::filesystem::path resolve_portuguese_dict_path(
    const std::filesystem::path& model_root, ...`
  - `range_re` (function, line 290) `static const std::regex range_re(R"(\b(\d+)-(\d+)\b)", std::regex::ECMAScript);`
  - `dig_re` (function, line 292) `static const std::regex dig_re(R"(\b\d+\b)", std::regex::ECMAScript);`
  - `dig_pass` (function, line 522) `static const std::regex dig_pass(R"(^[0-9]+(?:-[0-9]+)*$)", std::regex::ECMAScript);`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/german.h`, `core/moonshine-tts/src/lang-specific/ipa-symbols.h`, `core/moonshine-tts/src/lang-specific/portuguese-rules.h`, `core/moonshine-tts/src/lang-specific/portuguese.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/portuguese.h
- Doc: PortugueseRuleG2p: Rule- and lexicon-based Portuguese G2P (Brazil / Portugal), mirroring...
- Layer: testing
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 14)
  - `Options` (struct, line 20)
  - `PortugueseRuleG2p` (class, line 18)
  - `is_portugal` (function, line 38) `bool is_portugal() const`
  - `dialect_id` (function, line 39) `const std::string& dialect_id() const`
  - `dialect_ids` (function, line 36) `static std::vector<std::string> dialect_ids();`
  - `dialect_resolves_to_portugal_rules` (function, line 61) `bool dialect_resolves_to_portugal_rules(std::string_view dialect_id);`
  - `dialect_resolves_to_brazilian_portuguese_rules` (function, line 64) `bool dialect_resolves_to_brazilian_portuguese_rules( std::string_view dialect_id);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_PORTUGUESE_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_PORTUGUESE_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/portuguese.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp`, `core/moonshine-tts/tools/portuguese-rule-g2p-cli.cpp`

## core/moonshine-tts/src/lang-specific/russian-numbers.cpp
- Doc: Russian cardinal expansion (russian_numbers.py). #include from russian.cpp (same TU).
- Layer: testing
- Language: cpp
- Symbols:
  - `ru_ascii_all_digits` (function, line 14) `bool ru_ascii_all_digits(std::string_view s)`
  - `ru_ones_digit` (function, line 99) `std::string ru_ones_digit(int n, bool feminine)`
  - `ru_append_under_100` (function, line 114) `void ru_append_under_100(int n, bool feminine, std::vector<std::string>& out)`
  - `ru_append_cardinal_1_to_999` (function, line 134) `void ru_append_cardinal_1_to_999(int n, bool feminine,
                                 std::vect...`
  - `ru_thousand_suffix` (function, line 151) `const char* ru_thousand_suffix(int q)`
  - `ru_append_below_1_000_000` (function, line 166) `void ru_append_below_1_000_000(int n, std::vector<std::string>& out)`
  - `expand_cardinal_digits_to_russian_words` (function, line 183) `std::string expand_cardinal_digits_to_russian_words(std::string_view s)`
  - `expand_russian_digit_tokens_in_text` (function, line 220) `std::string expand_russian_digit_tokens_in_text(std::string text)`
  - `range_re` (function, line 221) `static const std::regex range_re(R"(\b(\d+)-(\d+)\b)", std::regex::ECMAScript);`
  - `dig_re` (function, line 223) `static const std::regex dig_re(R"(\b\d+\b)", std::regex::ECMAScript);`
- Depends on: `core/moonshine-tts/src/utf8-utils.h`
- Imported by: `core/moonshine-tts/src/lang-specific/russian.cpp`


Next: [KB_lang-specific_p4.md](KB_lang-specific_p4.md)
