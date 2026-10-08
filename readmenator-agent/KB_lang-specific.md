# Subsystem: lang-specific

## core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp
- Layer: infrastructure
- Language: cpp
- Symbols:
  - `BasicTokCfg` (struct, line 315)
  - `EncodedWp` (struct, line 427)
  - `Idx` (struct, line 517)
  - `open_ar_session` (function, line 34) `std::unique_ptr<Ort::Session> open_ar_session(
    Ort::Env& env, const std::filesystem::path& mo...`
  - `open_ar_session_memory` (function, line 51) `std::unique_ptr<Ort::Session> open_ar_session_memory(
    Ort::Env& env, const void* data, size_t...`
  - `slurp_utf8_file_ar` (function, line 65) `std::string slurp_utf8_file_ar(const std::filesystem::path& p)`
  - `bundle_load_utf8_ar` (function, line 75) `bool bundle_load_utf8_ar(const MoonshineG2POptions* opt,
                         std::string_vie...`
  - `bundle_load_binary_ar` (function, line 94) `bool bundle_load_binary_ar(const MoonshineG2POptions* opt,
                           std::string...`
  - `utf8_to_u32` (function, line 127) `std::u32string utf8_to_u32(std::string_view utf8)`
  - `u32_to_utf8` (function, line 140) `std::string u32_to_utf8(const std::u32string& s)`
  - `is_space_u32` (function, line 148) `bool is_space_u32(char32_t c)`
  - `is_control_u32` (function, line 157) `bool is_control_u32(char32_t c)`
  - `is_punctuation_u32` (function, line 166) `bool is_punctuation_u32(char32_t c)`
  - `is_punct_char_word_group_u32` (function, line 179) `bool is_punct_char_word_group_u32(char32_t c)`
  - `is_chinese_char` (function, line 184) `bool is_chinese_char(std::uint32_t cp)`
  - `u32_nfc` (function, line 193) `std::u32string u32_nfc(const std::u32string& s)`
  - `strip_mn_nfd` (function, line 205) `std::u32string strip_mn_nfd(const std::u32string& s)`
  - `to_lower_u32` (function, line 225) `std::u32string to_lower_u32(const std::u32string& s)`
  - `clean_text_u32` (function, line 234) `std::u32string clean_text_u32(const std::u32string& text)`
  - `tokenize_chinese_chars_u32` (function, line 246) `std::u32string tokenize_chinese_chars_u32(const std::u32string& text)`
  - `split_u32_whitespace` (function, line 260) `std::vector<std::u32string> split_u32_whitespace(std::u32string_view s)`
  - `run_split_on_punc_u32` (function, line 285) `std::vector<std::u32string> run_split_on_punc_u32(const std::u32string& text)`
  - `normalization_ref_u32` (function, line 321) `std::u32string normalization_ref_u32(const std::u32string& text_u32,
                            ...`
  - `basic_tokenize_u32` (function, line 330) `std::vector<std::u32string> basic_tokenize_u32(
    const std::u32string& original_text_u32, cons...`
  - `align_basic_tokens_u32` (function, line 362) `void align_basic_tokens_u32(const std::u32string& ref,
                            const std::vec...`
  - `wordpiece_tokenize_u32` (function, line 379) `std::vector<std::u32string> wordpiece_tokenize_u32(
    const std::u32string& token,
    const st...`
  - `encode_bert_wordpiece` (function, line 434) `EncodedWp encode_bert_wordpiece(
    const std::u32string& text_u32,
    const std::unordered_map...`
  - `is_arabic_anchor_char` (function, line 672) `bool is_arabic_anchor_char(char32_t c)`
  - `anchor_index_for_span` (function, line 686) `std::optional<int> anchor_index_for_span(const std::u32string& ref, int s,
                      ...`
  - `strip_arabic_diacritics_u32` (function, line 700) `std::u32string strip_arabic_diacritics_u32(const std::u32string& s)`
  - `ArabicDiacOnnx` (function, line 726) `ArabicDiacOnnx::ArabicDiacOnnx(const MoonshineG2POptions* opt,
                               std...`
  - `diacritize` (function, line 787) `std::string ArabicDiacOnnx::diacritize(std::string_view text_utf8) const`
  - `chars` (function, line 389) `std::vector<char32_t> chars(wt.begin(), wt.end());`
  - `buf` (function, line 628) `const std::string buf(utf8);`
  - `inner` (function, line 821) `std::vector<int64_t> inner(enc.input_ids.begin() + 1, enc.input_ids.end() - 1);`
  - `mask` (function, line 844) `std::vector<int64_t> mask(static_cast<size_t>(T), 1);`
- Depends on: `core/moonshine-tts/src/g2p-path.h`, `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-tts/src/ort-onnx-external-data.h`, `core/moonshine-tts/src/ort-session-options.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/arabic-diac-onnx.h
- Layer: infrastructure
- Language: h
- Symbols:
  - `MoonshineG2POptions` (struct, line 16)
  - `ArabicDiacOnnx` (class, line 20)
  - `model_dir` (function, line 39) `const std::filesystem::path& model_dir() const`
  - `MOONSHINE_TTS_ARABIC_DIAC_ONNX_H` (macro, line 2) `#define MOONSHINE_TTS_ARABIC_DIAC_ONNX_H`
- Imported by: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp`, `core/moonshine-tts/src/lang-specific/arabic.h`

## core/moonshine-tts/src/lang-specific/arabic-ipa.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `is_ar_combining` (function, line 23) `bool is_ar_combining(char32_t ch)`
  - `is_ar_base_letter` (function, line 36) `bool is_ar_base_letter(char32_t ch)`
  - `u32_nfc_u32` (function, line 53) `std::u32string u32_nfc_u32(const std::u32string& s)`
  - `strip_ar_diac_u32` (function, line 68) `std::u32string strip_ar_diac_u32(const std::u32string& s)`
  - `u32_to_utf8_str` (function, line 79) `std::string u32_to_utf8_str(const std::u32string& s)`
  - `has_vowel_mark_u32` (function, line 87) `bool has_vowel_mark_u32(const std::u32string& marks)`
  - `strip_spurious_tatweil_u32` (function, line 136) `std::u32string strip_spurious_tatweil_u32(const std::u32string& w)`
  - `apply_default_fatha_u32` (function, line 160) `std::u32string apply_default_fatha_u32(const std::u32string& w)`
  - `onset_ipa` (function, line 203) `std::string onset_ipa(char32_t base)`
  - `vowel_from_marks` (function, line 273) `std::string vowel_from_marks(const std::u32string& marks)`
  - `gem_ipa` (function, line 309) `std::string gem_ipa(const std::string& onset)`
  - `diac_word_to_ipa_u32` (function, line 320) `std::string diac_word_to_ipa_u32(const std::u32string& word)`
  - `arabic_msa_strip_diacritics_utf8` (function, line 402) `std::string arabic_msa_strip_diacritics_utf8(std::string_view utf8)`
  - `arabic_msa_apply_onnx_partial_postprocess_utf8` (function, line 407) `std::string arabic_msa_apply_onnx_partial_postprocess_utf8(
    std::string_view utf8)`
  - `arabic_msa_word_to_ipa_with_assimilation_utf8` (function, line 415) `std::string arabic_msa_word_to_ipa_with_assimilation_utf8(
    std::string_view filled_diac_utf8,...`
- Depends on: `core/moonshine-tts/src/lang-specific/arabic-ipa.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/arabic-ipa.h
- Layer: testing
- Language: h
- Symbols:
  - `MOONSHINE_TTS_LANG_SPECIFIC_ARABIC_IPA_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_ARABIC_IPA_H`
- Imported by: `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp`, `core/moonshine-tts/src/lang-specific/arabic.cpp`

## core/moonshine-tts/src/lang-specific/arabic.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `absolute_model_root_ar` (function, line 19) `std::filesystem::path absolute_model_root_ar(
    const std::filesystem::path& model_root)`
  - `has_arabic_script` (function, line 33) `bool has_arabic_script(std::string_view s)`
  - `strip_lex_ipa_segment_dots` (function, line 93) `std::string strip_lex_ipa_segment_dots(std::string ipa)`
  - `ArabicRuleG2p` (function, line 100) `ArabicRuleG2p::ArabicRuleG2p(std::filesystem::path onnx_model_dir,
                             s...`
  - `ArabicRuleG2p` (function, line 106) `ArabicRuleG2p::ArabicRuleG2p(std::filesystem::path onnx_model_dir,
                             s...`
  - `ArabicRuleG2p` (function, line 115) `ArabicRuleG2p::ArabicRuleG2p(const MoonshineG2POptions& opt,
                             std::fi...`
  - `ArabicRuleG2p` (function, line 122) `ArabicRuleG2p::ArabicRuleG2p(const MoonshineG2POptions& opt,
                             std::fi...`
  - `dialect_ids` (function, line 132) `std::vector<std::string> ArabicRuleG2p::dialect_ids()`
  - `dialect_resolves_to_arabic_rules` (function, line 137) `bool dialect_resolves_to_arabic_rules(std::string_view dialect_id)`
  - `resolve_arabic_dict_path` (function, line 146) `std::filesystem::path resolve_arabic_dict_path(
    const std::filesystem::path& model_root)`
  - `resolve_arabic_onnx_model_dir` (function, line 152) `std::filesystem::path resolve_arabic_onnx_model_dir(
    const std::filesystem::path& model_root)`
  - `g2p_word` (function, line 158) `std::string ArabicRuleG2p::g2p_word(std::string_view word_utf8)`
  - `text_to_ipa` (function, line 174) `std::string ArabicRuleG2p::text_to_ipa(std::string text,
                                       s...`
- Depends on: `core/moonshine-tts/src/g2p-path.h`, `core/moonshine-tts/src/lang-specific/arabic-ipa.h`, `core/moonshine-tts/src/lang-specific/arabic.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/arabic.h
- Layer: testing
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 16)
  - `MoonshineG2POptions` (struct, line 17)
  - `ArabicRuleG2p` (class, line 21)
  - `dialect_id` (function, line 45) `const std::string& dialect_id() const`
  - `dialect_ids` (function, line 39) `static std::vector<std::string> dialect_ids();`
  - `dialect_resolves_to_arabic_rules` (function, line 54) `bool dialect_resolves_to_arabic_rules(std::string_view dialect_id);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_ARABIC_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_ARABIC_H`
- Depends on: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.h`, `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/arabic.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/arabic-rule-g2p-test.cpp`, `core/moonshine-tts/tools/arabic-rule-g2p-cli.cpp`

## core/moonshine-tts/src/lang-specific/chinese-numbers.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `digit_cp` (function, line 17) `char32_t digit_cp(unsigned d)`
  - `cn_digit` (function, line 27) `std::string cn_digit(unsigned d)`
  - `ends_with_ling_utf8` (function, line 33) `bool ends_with_ling_utf8(const std::string& s)`
  - `section_under_10000` (function, line 41) `std::string section_under_10000(unsigned n)`
  - `int_to_han_u64` (function, line 96) `std::string int_to_han_u64(std::uint64_t n)`
  - `ascii_digit_string` (function, line 146) `bool ascii_digit_string(std::string_view t, std::uint64_t& out_val)`
  - `int_to_mandarin_cardinal_han` (function, line 166) `std::string int_to_mandarin_cardinal_han(std::uint64_t n)`
  - `arabic_numeral_token_to_han` (function, line 170) `std::optional<std::string> arabic_numeral_token_to_han(
    std::string_view token_sv)`
  - `gs` (function, line 116) `std::vector<unsigned> gs(low_first.rbegin(), low_first.rend());`
- Depends on: `core/moonshine-tts/src/lang-specific/chinese-numbers.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/chinese-numbers.h
- Layer: testing
- Language: h
- Symbols:
  - `MOONSHINE_TTS_LANG_SPECIFIC_CHINESE_NUMBERS_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_CHINESE_NUMBERS_H`
- Imported by: `core/moonshine-tts/src/lang-specific/chinese-numbers.cpp`, `core/moonshine-tts/src/lang-specific/chinese.cpp`

## core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `utf8_nfc_utf8proc` (function, line 16) `std::string utf8_nfc_utf8proc(std::string_view s)`
  - `ChineseOnnxG2p` (function, line 30) `ChineseOnnxG2p::ChineseOnnxG2p(std::filesystem::path model_dir,
                               st...`
  - `ChineseOnnxG2p` (function, line 34) `ChineseOnnxG2p::ChineseOnnxG2p(std::filesystem::path model_dir,
                               st...`
  - `ChineseOnnxG2p` (function, line 38) `ChineseOnnxG2p::ChineseOnnxG2p(const MoonshineG2POptions& opt,
                               std...`
  - `ChineseOnnxG2p` (function, line 44) `ChineseOnnxG2p::ChineseOnnxG2p(const MoonshineG2POptions& opt,
                               std...`
  - `text_to_ipa` (function, line 50) `std::string ChineseOnnxG2p::text_to_ipa(std::string text_utf8,
                                  ...`
  - `ChineseOnnxRuleG2p` (function, line 76) `ChineseOnnxRuleG2p::ChineseOnnxRuleG2p(std::filesystem::path onnx_model_dir,
                    ...`
  - `ChineseOnnxRuleG2p` (function, line 82) `ChineseOnnxRuleG2p::ChineseOnnxRuleG2p(std::filesystem::path onnx_model_dir,
                    ...`
  - `ChineseOnnxRuleG2p` (function, line 87) `ChineseOnnxRuleG2p::ChineseOnnxRuleG2p(const MoonshineG2POptions& opt,
                          ...`
  - `ChineseOnnxRuleG2p` (function, line 94) `ChineseOnnxRuleG2p::ChineseOnnxRuleG2p(const MoonshineG2POptions& opt,
                          ...`
  - `text_to_ipa` (function, line 101) `std::string ChineseOnnxRuleG2p::text_to_ipa(
    std::string text, std::vector<G2pWordLog>* per_w...`
  - `tmp` (function, line 17) `const std::string tmp(s);`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h
- Layer: testing
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 15)
  - `MoonshineG2POptions` (struct, line 16)
  - `ChineseOnnxG2p` (class, line 20)
  - `ChineseOnnxRuleG2p` (class, line 46)
  - `tok` (function, line 37) `const ChineseTokPosOnnx& tok() const`
  - `MOONSHINE_TTS_CHINESE_ONNX_G2P_H` (macro, line 2) `#define MOONSHINE_TTS_CHINESE_ONNX_G2P_H`
- Depends on: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.h`, `core/moonshine-tts/src/lang-specific/chinese.h`, `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/chinese-rule-g2p-test.cpp`, `core/moonshine-tts/tools/chinese-rule-g2p-cli.cpp`

## core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `BasicTokCfg` (struct, line 311)
  - `EncodedWp` (struct, line 435)
  - `Idx` (struct, line 525)
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
  - `basic_tokenize_u32` (function, line 338) `std::vector<std::u32string> basic_tokenize_u32(
    const std::u32string& original_text_u32, cons...`
  - `align_basic_tokens_u32` (function, line 370) `void align_basic_tokens_u32(const std::u32string& ref,
                            const std::vec...`
  - `wordpiece_tokenize_u32` (function, line 387) `std::vector<std::u32string> wordpiece_tokenize_u32(
    const std::u32string& token,
    const st...`
  - `encode_bert_wordpiece` (function, line 442) `EncodedWp encode_bert_wordpiece(
    const std::u32string& text_u32,
    const std::unordered_map...`
  - `cjk_tokpos_preferred_chunk_break_cp` (function, line 632) `bool cjk_tokpos_preferred_chunk_break_cp(char32_t c)`
  - `cjk_tokpos_chunk_exclusive_end` (function, line 666) `template <typename EncodeFn>
std::size_t cjk_tokpos_chunk_exclusive_end(const std::u32string& ful...`
  - `default_chinese_tok_pos_model_dir` (function, line 704) `std::filesystem::path default_chinese_tok_pos_model_dir(
    const std::filesystem::path& g2p_dat...`
  - `ChineseTokPosOnnx` (function, line 714) `ChineseTokPosOnnx::ChineseTokPosOnnx(const MoonshineG2POptions* opt,
                            ...`
  - `format_annotated_line` (function, line 775) `std::string ChineseTokPosOnnx::format_annotated_line(
    const std::vector<std::pair<std::string...`
  - `chars` (function, line 397) `std::vector<char32_t> chars(wt.begin(), wt.end());`
  - `buf` (function, line 627) `const std::string buf(utf8);`
  - `mask` (function, line 831) `std::vector<int64_t> mask(static_cast<size_t>(T), 1);`
- Depends on: `core/moonshine-tts/src/g2p-path.h`, `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-tts/src/ort-onnx-external-data.h`, `core/moonshine-tts/src/ort-session-options.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.h
- Layer: testing
- Language: h
- Symbols:
  - `MoonshineG2POptions` (struct, line 16)
  - `ChineseTokPosOnnx` (class, line 22)
  - `model_dir` (function, line 42) `const std::filesystem::path& model_dir() const`
  - `format_annotated_line` (function, line 39) `static std::string format_annotated_line( const std::vector<std::pair<std::string, std::string>>& pairs);`
  - `MOONSHINE_TTS_CHINESE_TOK_POS_ONNX_H` (macro, line 2) `#define MOONSHINE_TTS_CHINESE_TOK_POS_ONNX_H`
- Imported by: `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h`, `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp`, `core/moonshine-tts/tests/chinese-tok-pos-onnx-test.cpp`

## core/moonshine-tts/src/lang-specific/chinese.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `trim_copy_line` (function, line 23) `std::string trim_copy_line(std::string_view s)`
  - `is_cjk_cp` (function, line 37) `bool is_cjk_cp(char32_t cp)`
  - `is_ascii_digit_cp` (function, line 44) `bool is_ascii_digit_cp(char32_t cp)`
  - `is_fullwidth_digit_cp` (function, line 46) `bool is_fullwidth_digit_cp(char32_t cp)`
  - `token_has_g2p_content` (function, line 50) `bool token_has_g2p_content(const std::string& tok)`
  - `pos_in_set` (function, line 68) `bool pos_in_set(std::string_view p, const std::unordered_set<std::string>& s)`
  - `skip_phonetic_pos` (function, line 72) `const std::unordered_set<std::string>& skip_phonetic_pos()`
  - `verb_like_pos` (function, line 78) `const std::unordered_set<std::string>& verb_like_pos()`
  - `noun_like_pos` (function, line 85) `const std::unordered_set<std::string>& noun_like_pos()`
  - `ipa_contains` (function, line 92) `bool ipa_contains(const std::string& ipa, std::string_view sub)`
  - `try_consume_g2p_token` (function, line 96) `bool try_consume_g2p_token(const std::string& text, size_t pos,
                           size_t...`
  - `load_chinese_lexicon_stream` (function, line 191) `void load_chinese_lexicon_stream(
    std::istream& in,
    std::unordered_map<std::string, std::...`
  - `ChineseRuleG2p` (function, line 215) `ChineseRuleG2p::ChineseRuleG2p(std::filesystem::path dict_tsv)`
  - `ChineseRuleG2p` (function, line 232) `ChineseRuleG2p::ChineseRuleG2p(std::string dict_tsv_utf8)`
  - `disambiguate_heteronym` (function, line 240) `std::string ChineseRuleG2p::disambiguate_heteronym(
    std::string_view word, std::string_view p...`
  - `han_reading_to_ipa` (function, line 401) `std::string ChineseRuleG2p::han_reading_to_ipa(std::string_view han) const`
  - `char_fallback_ipa` (function, line 426) `std::string ChineseRuleG2p::char_fallback_ipa(std::string_view word) const`
  - `g2p_word_impl` (function, line 441) `std::string ChineseRuleG2p::g2p_word_impl(std::string_view word,
                                ...`
  - `word_to_ipa` (function, line 488) `std::string ChineseRuleG2p::word_to_ipa(std::string_view word) const`
  - `word_to_ipa_with_pos` (function, line 492) `std::string ChineseRuleG2p::word_to_ipa_with_pos(std::string_view word,
                         ...`
  - `text_to_ipa` (function, line 497) `std::string ChineseRuleG2p::text_to_ipa(std::string text,
                                       ...`
  - `dialect_resolves_to_chinese_rules` (function, line 547) `bool dialect_resolves_to_chinese_rules(std::string_view dialect_id)`
  - `dialect_ids` (function, line 556) `std::vector<std::string> ChineseRuleG2p::dialect_ids()`
  - `resolve_chinese_dict_path` (function, line 561) `std::filesystem::path resolve_chinese_dict_path(
    const std::filesystem::path& model_root)`
  - `resolve_chinese_onnx_model_dir` (function, line 566) `std::filesystem::path resolve_chinese_onnx_model_dir(
    const std::filesystem::path& model_root)`
  - `w` (function, line 249) `const std::string w(word);`
  - `p` (function, line 250) `const std::string p(pos);`
  - `h` (function, line 402) `const std::string h(han);`
- Depends on: `core/moonshine-tts/src/g2p-path.h`, `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/chinese-numbers.h`, `core/moonshine-tts/src/lang-specific/chinese.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/chinese.h
- Layer: testing
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 14)
  - `ChineseRuleG2p` (class, line 23)
  - `dialect_id` (function, line 30) `const std::string& dialect_id() const`
  - `dialect_ids` (function, line 28) `static std::vector<std::string> dialect_ids();`
  - `dialect_resolves_to_chinese_rules` (function, line 57) `bool dialect_resolves_to_chinese_rules(std::string_view dialect_id);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_CHINESE_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_CHINESE_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h`, `core/moonshine-tts/src/lang-specific/chinese.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/chinese-rule-g2p-test.cpp`

## core/moonshine-tts/src/lang-specific/cmudict-tsv.cpp
- Layer: infrastructure
- Language: cpp
- Symbols:
  - `parse_cmudict_tsv_lines` (function, line 14) `void parse_cmudict_tsv_lines(
    std::istream& in,
    std::unordered_map<std::string, std::vect...`
  - `CmudictTsv` (function, line 58) `CmudictTsv::CmudictTsv(const std::filesystem::path& path)`
  - `CmudictTsv` (function, line 66) `CmudictTsv::CmudictTsv(std::string_view utf8_contents)`
  - `lookup` (function, line 72) `const std::vector<std::string>* CmudictTsv::lookup(std::string_view key) const`
  - `buf` (function, line 67) `const std::string buf(utf8_contents);`
  - `k` (function, line 73) `const std::string k(key.begin(), key.end());`
- Depends on: `core/moonshine-tts/src/lang-specific/cmudict-tsv.h`, `core/moonshine-tts/src/text-normalize.h`

## core/moonshine-tts/src/lang-specific/cmudict-tsv.h
- Layer: infrastructure
- Language: h
- Symbols:
  - `CmudictTsv` (class, line 14)
  - `lookup` (function, line 19) `const std::vector<std::string>* lookup(std::string_view key) const;`
  - `MOONSHINE_TTS_CMUDICT_TSV_H` (macro, line 2) `#define MOONSHINE_TTS_CMUDICT_TSV_H`
- Imported by: `core/moonshine-tts/src/lang-specific/cmudict-tsv.cpp`, `core/moonshine-tts/src/lang-specific/english.cpp`, `core/moonshine-tts/tests/cmudict-tsv-test.cpp`

## core/moonshine-tts/src/lang-specific/dutch.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `Slot` (struct, line 626)
  - `dutch_unicode_tolower_cp` (function, line 31) `char32_t dutch_unicode_tolower_cp(char32_t c)`
  - `append_lexicon_folded` (function, line 102) `void append_lexicon_folded(std::string& out, char32_t cl)`
  - `normalize_lexicon_key_utf8` (function, line 160) `std::string normalize_lexicon_key_utf8(const std::string& word)`
  - `is_grapheme_char` (function, line 178) `bool is_grapheme_char(char32_t cl)`
  - `normalize_grapheme_key_u32` (function, line 190) `std::u32string normalize_grapheme_key_u32(const std::string& word)`
  - `kTeenWord` (function, line 212) `static const char* kTeenWord(int n)`
  - `join_unit_tens` (function, line 221) `std::string join_unit_tens(int u, std::string_view tens_word)`
  - `below_100` (function, line 237) `std::string below_100(int n)`
  - `below_1000_spaced` (function, line 256) `std::string below_1000_spaced(int n)`
  - `from_1000_to_9999` (function, line 278) `std::string from_1000_to_9999(int n)`
  - `fix_thousands_compound` (function, line 310) `std::string fix_thousands_compound(int q)`
  - `below_1_000_000_v2` (function, line 323) `std::string below_1_000_000_v2(int n)`
  - `expand_cardinal_digits_to_dutch_words` (function, line 339) `std::string expand_cardinal_digits_to_dutch_words(std::string_view sv)`
  - `is_ascii_digit` (function, line 371) `bool is_ascii_digit(char c)`
  - `is_latin1_supplement_python_word_char` (function, line 373) `bool is_latin1_supplement_python_word_char(char32_t cp)`
  - `is_letterlike_math_word_char` (function, line 403) `bool is_letterlike_math_word_char(char32_t cp)`
  - `is_dutch_word_char` (function, line 408) `bool is_dutch_word_char(char32_t cp)`
  - `prev_utf8_index` (function, line 437) `size_t prev_utf8_index(const std::string& t, size_t byte_i)`
  - `word_boundary_before` (function, line 448) `bool word_boundary_before(const std::string& t, size_t byte_i)`
  - `word_boundary_after` (function, line 459) `bool word_boundary_after(const std::string& t, size_t byte_i)`
  - `expand_digit_tokens_in_text` (function, line 469) `std::string expand_digit_tokens_in_text(std::string_view text_sv)`
  - `digit_pass_through_pattern` (function, line 520) `bool digit_pass_through_pattern(std::string_view raw)`
  - `all_ascii_digits_string` (function, line 544) `bool all_ascii_digits_string(const std::string& s)`
  - `apply_lexicon_ipa_postprocess` (function, line 556) `std::string apply_lexicon_ipa_postprocess(std::string ipa,
                                      ...`
  - `load_dutch_lexicon_stream` (function, line 624) `void load_dutch_lexicon_stream(
    std::istream& in, std::unordered_map<std::string, std::string...`
  - `load_dutch_lexicon_file` (function, line 678) `void load_dutch_lexicon_file(
    const std::filesystem::path& path,
    std::unordered_map<std::...`
  - `is_vowel_letter32` (function, line 689) `bool is_vowel_letter32(char32_t c)`
  - `strip_to_plain_vowel` (function, line 699) `char32_t strip_to_plain_vowel(char32_t c)`
  - `word_has_written_stress_u32` (function, line 723) `bool word_has_written_stress_u32(const std::u32string& w)`
  - `stressed_syllable_from_acute` (function, line 732) `std::optional<size_t> stressed_syllable_from_acute(
    const std::vector<std::u32string>& syllab...`
  - `dutch_orthographic_syllables_u32` (function, line 793) `std::vector<std::u32string> dutch_orthographic_syllables_u32(
    const std::u32string& word)`
  - `remove_if` (function, line 851) `std::remove_if(syllables.begin(), syllables.end(),
                     [](const std::u32string& sy)`
  - `unstressed_prefix_len_u32` (function, line 857) `size_t unstressed_prefix_len_u32(const std::u32string& wl)`
  - `default_stress_syllable_index` (function, line 871) `size_t default_stress_syllable_index(const std::vector<std::u32string>& syls,
                   ...`
  - `insert_primary_stress_before_vowel_dutch` (function, line 916) `std::string insert_primary_stress_before_vowel_dutch(std::string s)`
  - `ipa_starts_with_nucleus_dutch` (function, line 959) `bool ipa_starts_with_nucleus_dutch(std::string_view rest)`
  - `ipa_at_stress_mark_dutch` (function, line 998) `bool ipa_at_stress_mark_dutch(const std::string& ipa, size_t j)`
  - `ipa_skip_pre_nucleus_dutch` (function, line 1007) `size_t ipa_skip_pre_nucleus_dutch(std::string_view s, size_t j)`
  - `final_devoice_obstruents` (function, line 1045) `std::string final_devoice_obstruents(std::string ipa)`
  - `letters_to_ipa_no_stress` (function, line 1083) `std::string letters_to_ipa_no_stress(const std::u32string& syl_in,
                              ...`
  - `strip_hyphens_u32` (function, line 1416) `std::u32string strip_hyphens_u32(const std::u32string& w)`
  - `rules_word_to_ipa_utf8` (function, line 1426) `std::string rules_word_to_ipa_utf8(const std::string& raw_word,
                                 ...`
  - `resolve_dutch_dict_path` (function, line 1458) `std::filesystem::path resolve_dutch_dict_path(
    const std::filesystem::path& model_root)`
  - `dialect_resolves_to_dutch_rules` (function, line 1463) `bool dialect_resolves_to_dutch_rules(std::string_view dialect_id)`
  - `dialect_ids` (function, line 1471) `std::vector<std::string> DutchRuleG2p::dialect_ids()`
  - `normalize_ipa_stress_for_vocoder` (function, line 1475) `std::string DutchRuleG2p::normalize_ipa_stress_for_vocoder(std::string ipa)`
  - `DutchRuleG2p` (function, line 1522) `DutchRuleG2p::DutchRuleG2p(std::filesystem::path dict_tsv, Options options)
    : options_(options)`
  - `DutchRuleG2p` (function, line 1527) `DutchRuleG2p::DutchRuleG2p(std::string dict_tsv_utf8, Options options)
    : options_(options)`
  - `finalize_ipa` (function, line 1533) `std::string DutchRuleG2p::finalize_ipa(std::string ipa,
                                       bo...`
  - `lookup_or_rules` (function, line 1546) `std::string DutchRuleG2p::lookup_or_rules(const std::string& raw_word) const`
  - `word_to_ipa` (function, line 1602) `std::string DutchRuleG2p::word_to_ipa(const std::string& word) const`
  - `text_to_ipa_no_expand` (function, line 1623) `std::string DutchRuleG2p::text_to_ipa_no_expand(
    const std::string& text, std::vector<G2pWord...`
  - `text_to_ipa` (function, line 1699) `std::string DutchRuleG2p::text_to_ipa(std::string text,
                                      std...`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/dutch.h`, `core/moonshine-tts/src/lang-specific/ipa-symbols.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/dutch.h
- Layer: testing
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 14)
  - `Options` (struct, line 20)
  - `DutchRuleG2p` (class, line 18)
  - `dialect_id` (function, line 38) `const std::string& dialect_id() const`
  - `dialect_ids` (function, line 36) `static std::vector<std::string> dialect_ids();`
  - `normalize_ipa_stress_for_vocoder` (function, line 48) `static std::string normalize_ipa_stress_for_vocoder(std::string ipa);`
  - `dialect_resolves_to_dutch_rules` (function, line 62) `bool dialect_resolves_to_dutch_rules(std::string_view dialect_id);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_DUTCH_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_DUTCH_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/dutch.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp`, `core/moonshine-tts/tools/dutch-g2p-batch-cli.cpp`, `core/moonshine-tts/tools/dutch-rule-g2p-cli.cpp`

## core/moonshine-tts/src/lang-specific/english-hand-oov.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `Literal` (struct, line 124)
  - `utf8_starts_with` (function, line 19) `bool utf8_starts_with(const std::string& s, std::string_view p)`
  - `last_utf8_char` (function, line 23) `std::string_view last_utf8_char(std::string_view s)`
  - `last_ipa_unit_is_vowel` (function, line 38) `bool last_ipa_unit_is_vowel(std::string_view prev)`
  - `is_vowel` (function, line 50) `constexpr bool is_vowel(char c)`
  - `is_consonant` (function, line 54) `constexpr bool is_consonant(char c)`
  - `next_vowel_index` (function, line 58) `int next_vowel_index(std::string_view w, int start)`
  - `magic_e_lengthens` (function, line 67) `bool magic_e_lengthens(std::string_view w, int vowel_i)`
  - `th_voiced_word` (function, line 157) `bool th_voiced_word(std::string_view w)`
  - `oov_single_consonant` (function, line 163) `std::string oov_single_consonant(char c, std::string_view w, int i)`
  - `add_primary_stress_if_missing` (function, line 320) `std::string add_primary_stress_if_missing(std::string s)`
  - `oov_grapheme_to_ipa` (function, line 341) `std::string oov_grapheme_to_ipa(std::string_view word)`
  - `english_hand_oov_rules_ipa` (function, line 438) `std::string english_hand_oov_rules_ipa(std::string_view word)`
  - `p` (function, line 329) `const std::string_view p(pref);`
- Depends on: `core/moonshine-tts/src/lang-specific/english-hand-oov.h`, `core/moonshine-tts/src/text-normalize.h`

## core/moonshine-tts/src/lang-specific/english-hand-oov.h
- Layer: testing
- Language: h
- Symbols:
  - `MOONSHINE_TTS_LANG_SPECIFIC_ENGLISH_HAND_OOV_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_ENGLISH_HAND_OOV_H`
- Imported by: `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp`, `core/moonshine-tts/src/lang-specific/english.cpp`, `core/moonshine-tts/tests/english-hand-oov-test.cpp`

## core/moonshine-tts/src/lang-specific/english-numbers.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `Scale` (struct, line 74)
  - `digit_sequence_ipa` (function, line 22) `std::string digit_sequence_ipa(std::string_view digits)`
  - `under_100_ipa` (function, line 35) `std::string under_100_ipa(int n)`
  - `under_1000_ipa` (function, line 51) `std::string under_1000_ipa(int n)`
  - `cardinal_non_negative_ipa` (function, line 64) `std::optional<std::string> cardinal_non_negative_ipa(long long n)`
  - `integer_decimal_string_ipa` (function, line 107) `std::optional<std::string> integer_decimal_string_ipa(std::string s)`
  - `english_number_token_ipa` (function, line 200) `std::optional<std::string> english_number_token_ipa(std::string_view token)`
- Depends on: `core/moonshine-tts/src/lang-specific/english-numbers.h`

## core/moonshine-tts/src/lang-specific/english-numbers.h
- Layer: testing
- Language: h
- Symbols:
  - `MOONSHINE_TTS_LANG_SPECIFIC_ENGLISH_NUMBERS_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_ENGLISH_NUMBERS_H`
- Imported by: `core/moonshine-tts/src/lang-specific/english-numbers.cpp`, `core/moonshine-tts/src/lang-specific/english.cpp`, `core/moonshine-tts/tests/english-hand-oov-test.cpp`

## core/moonshine-tts/src/lang-specific/english.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `append_log` (function, line 31) `void append_log(std::vector<G2pWordLog>* out, G2pWordLog entry)`
  - `pick_english_heteronym_ipa` (function, line 40) `std::string pick_english_heteronym_ipa(std::vector<std::string> alts,
                           ...`
  - `EnglishRuleG2p` (function, line 82) `EnglishRuleG2p::EnglishRuleG2p(
    std::filesystem::path dict_tsv,
    std::optional<std::filesy...`
  - `EnglishRuleG2p` (function, line 110) `EnglishRuleG2p::EnglishRuleG2p(
    std::string dict_tsv_utf8, std::optional<std::filesystem::pat...`
  - `dialect_ids` (function, line 140) `std::vector<std::string> EnglishRuleG2p::dialect_ids()`
  - `text_to_ipa` (function, line 146) `std::string EnglishRuleG2p::text_to_ipa(std::string text,
                                       ...`
  - `dialect_is_british_english_variant` (function, line 239) `bool dialect_is_british_english_variant(std::string_view dialect_id)`
  - `dialect_resolves_to_english_rules` (function, line 244) `bool dialect_resolves_to_english_rules(std::string_view dialect_id)`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/cmudict-tsv.h`, `core/moonshine-tts/src/lang-specific/english-hand-oov.h`, `core/moonshine-tts/src/lang-specific/english-numbers.h`, `core/moonshine-tts/src/lang-specific/english.h`, `core/moonshine-tts/src/lang-specific/onnx-g2p-models.h`, `core/moonshine-tts/src/text-normalize.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/english.h
- Layer: testing
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 16)
  - `EnglishOnnxAuxMemory` (struct, line 20)
  - `Impl` (struct, line 58)
  - `EnglishRuleG2p` (class, line 26)
  - `dialect_ids` (function, line 51) `static std::vector<std::string> dialect_ids();`
  - `dialect_resolves_to_english_rules` (function, line 67) `bool dialect_resolves_to_english_rules(std::string_view dialect_id);`
  - `dialect_is_british_english_variant` (function, line 72) `bool dialect_is_british_english_variant(std::string_view dialect_id);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_ENGLISH_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_ENGLISH_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/english.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/english-rule-g2p-test.cpp`

## core/moonshine-tts/src/lang-specific/french-compound-map.cpp
- Layer: testing
- Language: cpp
- Depends on: `core/moonshine-tts/src/lang-specific/french-compound-map.h`

## core/moonshine-tts/src/lang-specific/french-compound-map.h
- Layer: testing
- Language: h
- Symbols:
  - `MOONSHINE_TTS_LANG_SPECIFIC_FRENCH_COMPOUND_MAP_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_FRENCH_COMPOUND_MAP_H`
- Imported by: `core/moonshine-tts/src/lang-specific/french-compound-map.cpp`, `core/moonshine-tts/src/lang-specific/french.cpp`

## core/moonshine-tts/src/lang-specific/french-internal.h
- Layer: testing
- Language: h
- Symbols:
  - `MOONSHINE_TTS_LANG_SPECIFIC_FRENCH_INTERNAL_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_FRENCH_INTERNAL_H`
- Imported by: `core/moonshine-tts/src/lang-specific/french-oov.cpp`, `core/moonshine-tts/src/lang-specific/french.cpp`

## core/moonshine-tts/src/lang-specific/french-oov.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `french_tolower_cp` (function, line 17) `char32_t french_tolower_cp(char32_t c)`
  - `is_allowed_ortho_cp` (function, line 64) `bool is_allowed_ortho_cp(char32_t c)`
  - `letters_only_u32` (function, line 75) `std::u32string letters_only_u32(const std::string& raw)`
  - `v_u32` (function, line 90) `bool v_u32(char32_t ch)`
  - `insert_stress_final_syllable` (function, line 120) `std::string insert_stress_final_syllable(std::string ipa)`
  - `prev_is_nucleus_idx` (function, line 168) `bool prev_is_nucleus_idx(const std::string& s, int idx)`
  - `utf8_last_cp_start` (function, line 214) `size_t utf8_last_cp_start(const std::string& s)`
  - `utf8_prev_cp_start` (function, line 228) `size_t utf8_prev_cp_start(const std::string& s, size_t cp_start)`
  - `trim_final_by_orthography` (function, line 242) `std::string trim_final_by_orthography(std::string ipa,
                                      cons...`
  - `peek_eq` (function, line 315) `bool peek_eq(const std::u32string& w, size_t i, const char* ascii)`
  - `scan_graphemes` (function, line 328) `std::string scan_graphemes(const std::u32string& w)`
  - `oov_word_to_ipa` (function, line 690) `std::string oov_word_to_ipa(const std::string& word, bool with_stress)`
  - `ms` (function, line 127) `const std::string ms(m);`
- Depends on: `core/moonshine-tts/src/lang-specific/french-internal.h`, `core/moonshine-tts/src/lang-specific/ipa-symbols.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/french.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `Tok` (struct, line 1188)
  - `LiaisonStrength` (enum, line 921)
  - `LiaisonStrength` (class, line 921)
  - `french_tolower_cp` (function, line 30) `char32_t french_tolower_cp(char32_t c)`
  - `is_french_key_cp` (function, line 83) `bool is_french_key_cp(char32_t c)`
  - `normalize_lookup_key_utf8` (function, line 94) `std::string normalize_lookup_key_utf8(const std::string& word)`
  - `is_latin1_supplement_python_word_char` (function, line 112) `bool is_latin1_supplement_python_word_char(char32_t cp)`
  - `is_letterlike_math_word_char` (function, line 144) `bool is_letterlike_math_word_char(char32_t cp)`
  - `is_french_word_char` (function, line 149) `bool is_french_word_char(char32_t cp)`
  - `to_lower_ascii` (function, line 177) `std::string to_lower_ascii(std::string_view w)`
  - `to_lower_pos_inventory_utf8` (function, line 185) `std::string to_lower_pos_inventory_utf8(const std::string& word)`
  - `load_french_lexicon_stream` (function, line 198) `void load_french_lexicon_stream(
    std::istream& in, std::unordered_map<std::string, std::strin...`
  - `load_french_lexicon_file` (function, line 230) `void load_french_lexicon_file(
    const std::filesystem::path& path,
    std::unordered_map<std:...`
  - `parse_first_csv_field` (function, line 241) `std::string parse_first_csv_field(std::string_view line)`
  - `load_french_pos_csv_stream` (function, line 270) `void load_french_pos_csv_stream(
    std::istream& in, const std::string& cat_upper,
    std::uno...`
  - `load_french_pos_dir` (function, line 294) `void load_french_pos_dir(
    const std::filesystem::path& dir,
    std::unordered_map<std::strin...`
  - `load_french_pos_from_csv_utf8_map` (function, line 324) `void load_french_pos_from_csv_utf8_map(
    const std::unordered_map<std::string, std::string>& c...`
  - `sort` (function, line 333) `std::sort(sorted.begin(), sorted.end(),
            [](const auto& a, const auto& b)`
  - `below_100` (function, line 350) `std::vector<std::string> below_100(int n)`
  - `below_1000` (function, line 413) `std::vector<std::string> below_1000(int n)`
  - `below_1_000_000` (function, line 447) `std::vector<std::string> below_1_000_000(int n)`
  - `join_space` (function, line 471) `std::string join_space(const std::vector<std::string>& v)`
  - `is_all_ascii_digits` (function, line 482) `bool is_all_ascii_digits(std::string_view s)`
  - `expand_cardinal_digits_to_french_words` (function, line 494) `std::string expand_cardinal_digits_to_french_words(std::string_view s)`
  - `expand_digit_tokens_in_text` (function, line 518) `std::string expand_digit_tokens_in_text(const std::string& text)`
  - `h_aspire_set` (function, line 541) `const std::unordered_set<std::string>& h_aspire_set()`
  - `closed_liaison_determiners` (function, line 552) `const std::unordered_set<std::string>& closed_liaison_determiners()`
  - `pos_scan_order` (function, line 559) `const std::vector<std::string>& pos_scan_order()`
  - `categories_for_form` (function, line 565) `std::vector<std::string> categories_for_form(
    const std::string& word,
    const std::unorder...`
  - `classify_pos` (function, line 583) `std::optional<std::string> classify_pos(
    const std::string& word,
    const std::unordered_ma...`
  - `strip_stress` (function, line 623) `std::string strip_stress(std::string_view ipa)`
  - `french_nucleus_prefixes` (function, line 643) `const std::vector<std::string>& french_nucleus_prefixes()`
  - `replace_suffix_once` (function, line 672) `std::string replace_suffix_once(std::string ipa, std::string_view old_s,
                        ...`
  - `nasal_liaison_transform` (function, line 682) `std::optional<std::string> nasal_liaison_transform(const std::string& word,
                     ...`
  - `ortho_for_liaison` (function, line 703) `std::string ortho_for_liaison(std::string_view word)`
  - `utf8_last_cp` (function, line 723) `bool utf8_last_cp(const std::string& s, char32_t& out_cp)`
  - `orthographic_liaison_consonant` (function, line 739) `std::optional<std::string> orthographic_liaison_consonant(
    std::string_view word)`
  - `ipa_starts_with_vowel_sound` (function, line 767) `bool ipa_starts_with_vowel_sound(std::string_view ipa_sv)`
  - `ipa_ends_with_audible_consonant` (function, line 850) `bool ipa_ends_with_audible_consonant(std::string_view ipa_sv)`
  - `liaison_strength_fn` (function, line 923) `LiaisonStrength liaison_strength_fn(const std::optional<std::string>& pos_left,
                 ...`
  - `lookup_lexicon` (function, line 1016) `std::optional<std::string> lookup_lexicon(
    const std::unordered_map<std::string, std::string>...`
  - `count_primary_stress_marks` (function, line 1039) `size_t count_primary_stress_marks(const std::string& s)`
  - `ensure_french_nuclear_stress` (function, line 1051) `std::string FrenchRuleG2p::ensure_french_nuclear_stress(std::string ipa)`
  - `FrenchRuleG2p` (function, line 1091) `FrenchRuleG2p::FrenchRuleG2p(std::filesystem::path dict_tsv,
                             std::fi...`
  - `FrenchRuleG2p` (function, line 1098) `FrenchRuleG2p::FrenchRuleG2p(std::string dict_tsv_utf8,
                             std::filesys...`
  - `finalize_word_ipa` (function, line 1116) `std::string FrenchRuleG2p::finalize_word_ipa(std::string ipa,
                                   ...`
  - `word_to_ipa_impl` (function, line 1127) `std::string FrenchRuleG2p::word_to_ipa_impl(const std::string& raw_word,
                        ...`
  - `word_to_ipa` (function, line 1171) `std::string FrenchRuleG2p::word_to_ipa(const std::string& word) const`
  - `text_to_ipa` (function, line 1175) `std::string FrenchRuleG2p::text_to_ipa(std::string text,
                                       s...`
  - `text_to_ipa_impl` (function, line 1180) `std::string FrenchRuleG2p::text_to_ipa_impl(
    const std::string& text, bool expand_digits,
   ...`
  - `all_of` (function, line 1328) `std::all_of(t.s.begin(), t.s.end(), [](unsigned char c)`
  - `dialect_resolves_to_french_rules` (function, line 1361) `bool dialect_resolves_to_french_rules(std::string_view dialect_id)`
  - `dialect_ids` (function, line 1369) `std::vector<std::string> FrenchRuleG2p::dialect_ids()`
  - `re` (function, line 519) `static const std::regex re(R"(\b\d+\b)", std::regex::ECMAScript);`
  - `w` (function, line 705) `const std::string w(word);`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/french-compound-map.h`, `core/moonshine-tts/src/lang-specific/french-internal.h`, `core/moonshine-tts/src/lang-specific/french.h`, `core/moonshine-tts/src/lang-specific/ipa-symbols.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/french.h
- Layer: testing
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 15)
  - `Options` (struct, line 21)
  - `FrenchRuleG2p` (class, line 19)
  - `dialect_id` (function, line 51) `const std::string& dialect_id() const`
  - `dialect_ids` (function, line 49) `static std::vector<std::string> dialect_ids();`
  - `ensure_french_nuclear_stress` (function, line 60) `static std::string ensure_french_nuclear_stress(std::string ipa);`
  - `dialect_resolves_to_french_rules` (function, line 78) `bool dialect_resolves_to_french_rules(std::string_view dialect_id);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_FRENCH_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_FRENCH_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/french.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/french-rule-g2p-test.cpp`, `core/moonshine-tts/tools/french-g2p-batch-cli.cpp`

## core/moonshine-tts/src/lang-specific/german.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `Slot` (struct, line 756)
  - `german_tolower_cp` (function, line 30) `char32_t german_tolower_cp(char32_t c)`
  - `is_key_char` (function, line 47) `bool is_key_char(char32_t c)`
  - `normalize_lookup_key_utf8` (function, line 56) `std::string normalize_lookup_key_utf8(const std::string& word)`
  - `is_german_word_char` (function, line 72) `bool is_german_word_char(char32_t cp)`
  - `is_vowel_l` (function, line 104) `bool is_vowel_l(char32_t ch)`
  - `char_before_for_ch` (function, line 121) `std::optional<char32_t> char_before_for_ch(const std::u32string& s, size_t i)`
  - `ch_ipa_utf8` (function, line 144) `std::string ch_ipa_utf8(const std::u32string& full_word_nh, size_t i)`
  - `final_devoice` (function, line 162) `std::string final_devoice(std::string ipa)`
  - `st_sp_at_morpheme_start` (function, line 187) `bool st_sp_at_morpheme_start(const std::u32string& hyphen_word,
                             size...`
  - `unstressed_prefix_len_u32` (function, line 211) `size_t unstressed_prefix_len_u32(const std::u32string& w)`
  - `strip_hyphens_u32` (function, line 225) `std::u32string strip_hyphens_u32(const std::u32string& w)`
  - `german_orthographic_syllables_u32` (function, line 281) `std::vector<std::u32string> german_orthographic_syllables_u32(
    const std::u32string& word_lower)`
  - `default_stress_syllable_index` (function, line 339) `size_t default_stress_syllable_index(const std::vector<std::u32string>& syls,
                   ...`
  - `insert_primary_stress_before_vowel_utf8` (function, line 370) `std::string insert_primary_stress_before_vowel_utf8(std::string s)`
  - `ipa_starts_with_nucleus` (function, line 389) `bool ipa_starts_with_nucleus(std::string_view rest)`
  - `ipa_skip_pre_nucleus` (function, line 404) `size_t ipa_skip_pre_nucleus(std::string_view s, size_t j)`
  - `letters_to_ipa_no_stress` (function, line 438) `std::string letters_to_ipa_no_stress(const std::u32string& syl_lower,
                           ...`
  - `rules_word_to_ipa_utf8` (function, line 719) `std::string rules_word_to_ipa_utf8(const std::string& raw_word,
                                 ...`
  - `load_german_lexicon_stream` (function, line 754) `void load_german_lexicon_stream(
    std::istream& in, std::unordered_map<std::string, std::strin...`
  - `load_german_lexicon_file` (function, line 810) `void load_german_lexicon_file(
    const std::filesystem::path& path,
    std::unordered_map<std:...`
  - `g2p_all_ascii_digits` (function, line 825) `bool g2p_all_ascii_digits(std::string_view s)`
  - `german_under_100_word` (function, line 837) `std::string german_under_100_word(int n)`
  - `german_hundred_head` (function, line 868) `std::string german_hundred_head(int h)`
  - `append_german_tokens_1_999` (function, line 880) `void append_german_tokens_1_999(int n, std::vector<std::string>& out)`
  - `append_german_tokens_thousands` (function, line 896) `void append_german_tokens_thousands(int q, std::vector<std::string>& out)`
  - `append_german_below_1_000_000` (function, line 908) `void append_german_below_1_000_000(int n, std::vector<std::string>& out)`
  - `expand_cardinal_digits_to_german_words` (function, line 924) `std::string expand_cardinal_digits_to_german_words(std::string_view s)`
  - `expand_german_digit_tokens_in_text` (function, line 962) `std::string expand_german_digit_tokens_in_text(std::string text)`
  - `ipa_at_stress_mark` (function, line 1012) `bool ipa_at_stress_mark(const std::string& ipa, size_t j)`
  - `normalize_ipa_stress_for_vocoder` (function, line 1021) `std::string GermanRuleG2p::normalize_ipa_stress_for_vocoder(std::string ipa)`
  - `GermanRuleG2p` (function, line 1068) `GermanRuleG2p::GermanRuleG2p(std::filesystem::path dict_tsv, Options options)
    : options_(opti...`
  - `GermanRuleG2p` (function, line 1073) `GermanRuleG2p::GermanRuleG2p(std::string dict_tsv_utf8, Options options)
    : options_(options)`
  - `finalize_ipa` (function, line 1079) `std::string GermanRuleG2p::finalize_ipa(std::string ipa) const`
  - `lookup_or_rules` (function, line 1091) `std::string GermanRuleG2p::lookup_or_rules(const std::string& raw_word) const`
  - `word_to_ipa` (function, line 1157) `std::string GermanRuleG2p::word_to_ipa(const std::string& word) const`
  - `text_to_ipa_no_expand` (function, line 1179) `std::string GermanRuleG2p::text_to_ipa_no_expand(
    const std::string& text, std::vector<G2pWor...`
  - `text_to_ipa` (function, line 1255) `std::string GermanRuleG2p::text_to_ipa(std::string text,
                                       s...`
  - `dialect_resolves_to_german_rules` (function, line 1263) `bool dialect_resolves_to_german_rules(std::string_view dialect_id)`
  - `dialect_ids` (function, line 1271) `std::vector<std::string> GermanRuleG2p::dialect_ids()`
  - `range_re` (function, line 963) `static const std::regex range_re(R"(\b(\d+)-(\d+)\b)", std::regex::ECMAScript);`
  - `dig_re` (function, line 965) `static const std::regex dig_re(R"(\b\d+\b)", std::regex::ECMAScript);`
  - `dig_pass` (function, line 1170) `static const std::regex dig_pass(R"(^[0-9]+(?:-[0-9]+)*$)", std::regex::ECMAScript);`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/ipa-postprocess.h`, `core/moonshine-tts/src/lang-specific/german.h`, `core/moonshine-tts/src/lang-specific/ipa-symbols.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/german.h
- Layer: testing
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 14)
  - `Options` (struct, line 20)
  - `GermanRuleG2p` (class, line 18)
  - `dialect_id` (function, line 40) `const std::string& dialect_id() const`
  - `dialect_ids` (function, line 38) `static std::vector<std::string> dialect_ids();`
  - `normalize_ipa_stress_for_vocoder` (function, line 53) `static std::string normalize_ipa_stress_for_vocoder(std::string ipa);`
  - `dialect_resolves_to_german_rules` (function, line 67) `bool dialect_resolves_to_german_rules(std::string_view dialect_id);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_GERMAN_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_GERMAN_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/german.cpp`, `core/moonshine-tts/src/lang-specific/italian.cpp`, `core/moonshine-tts/src/lang-specific/portuguese.cpp`, `core/moonshine-tts/src/lang-specific/russian.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/german-rule-g2p-test.cpp`, `core/moonshine-tts/tools/german-rule-g2p-cli.cpp`

## core/moonshine-tts/src/lang-specific/heteronym-context.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `join_cells` (function, line 12) `std::string join_cells(const std::vector<std::string>& cells)`
- Depends on: `core/moonshine-tts/src/lang-specific/heteronym-context.h`

## core/moonshine-tts/src/lang-specific/heteronym-context.h
- Layer: testing
- Language: h
- Symbols:
  - `MOONSHINE_TTS_HETERONYM_CONTEXT_H` (macro, line 2) `#define MOONSHINE_TTS_HETERONYM_CONTEXT_H`
- Imported by: `core/moonshine-tts/src/lang-specific/heteronym-context.cpp`, `core/moonshine-tts/tests/heteronym-context-test.cpp`

## core/moonshine-tts/src/lang-specific/hindi-numbers.cpp
- Layer: infrastructure
- Language: cpp
- Symbols:
  - `append_join` (function, line 43) `void append_join(std::vector<std::string>& out,
                 const std::vector<std::string>& ...`
  - `under_100` (function, line 50) `std::vector<std::string> under_100(int n)`
  - `tokens_0_999` (function, line 68) `std::vector<std::string> tokens_0_999(int n)`
  - `below_1_000_000_tokens` (function, line 93) `std::vector<std::string> below_1_000_000_tokens(int n)`
  - `join_space` (function, line 120) `std::string join_space(const std::vector<std::string>& v)`
  - `all_ascii_digits` (function, line 131) `bool all_ascii_digits(std::string_view s)`
  - `expand_cardinal_digits_to_hindi_words` (function, line 145) `std::string expand_cardinal_digits_to_hindi_words(std::string_view s)`
  - `expand_hindi_digit_tokens_in_text` (function, line 169) `std::string expand_hindi_digit_tokens_in_text(std::string text)`
  - `expand_devanagari_digit_runs_in_text` (function, line 202) `std::string expand_devanagari_digit_runs_in_text(std::string text)`
  - `range_re` (function, line 170) `static const std::regex range_re(R"((\b)(\d+)-(\d+)(\b))");`
  - `digit_re` (function, line 171) `static const std::regex digit_re(R"((\b)(\d+)(\b))");`
- Depends on: `core/moonshine-tts/src/lang-specific/hindi-numbers.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/hindi-numbers.h
- Layer: infrastructure
- Language: h
- Symbols:
  - `MOONSHINE_TTS_LANG_SPECIFIC_HINDI_NUMBERS_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_HINDI_NUMBERS_H`
- Imported by: `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp`, `core/moonshine-tts/src/lang-specific/hindi.cpp`, `core/moonshine-tts/tests/hindi-rule-g2p-test.cpp`

## core/moonshine-tts/src/lang-specific/hindi.cpp
- Layer: infrastructure
- Language: cpp
- Symbols:
  - `Syllable` (struct, line 45)
  - `utf8_nfc_utf8proc` (function, line 33) `std::string utf8_nfc_utf8proc(std::string_view s)`
  - `is_devanagari_digit` (function, line 95) `bool is_devanagari_digit(char32_t cp)`
  - `is_consonant` (function, line 97) `bool is_consonant(char32_t cp)`
  - `cons_ipa` (function, line 101) `std::string cons_ipa(char32_t base, bool nukta)`
  - `sv_starts_with` (function, line 112) `bool sv_starts_with(std::string_view s, std::string_view p)`
  - `nasal_for_place` (function, line 116) `std::string nasal_for_place(std::string_view first_onset)`
  - `syllable_weight` (function, line 155) `int syllable_weight(const Syllable& s)`
  - `assign_stress` (function, line 167) `std::string assign_stress(const std::vector<std::string>& ipa_syllables,
                        ...`
  - `apply_schwa_syncope` (function, line 201) `void apply_schwa_syncope(std::vector<Syllable>& syls)`
  - `parse_devanagari_to_syllables` (function, line 227) `std::optional<std::vector<Syllable>> parse_devanagari_to_syllables(
    const std::string& word)`
  - `render_syllables` (function, line 358) `std::string render_syllables(const std::vector<Syllable>& syls,
                             bool...`
  - `strip_edges_punct` (function, line 424) `void strip_edges_punct(std::string_view w, std::string& core)`
  - `has_devanagari` (function, line 448) `bool has_devanagari(std::string_view s)`
  - `all_ascii_digits_sv` (function, line 458) `bool all_ascii_digits_sv(std::string_view s)`
  - `builtin_hindi_dict_path` (function, line 472) `std::filesystem::path builtin_hindi_dict_path()`
  - `load_hindi_lexicon_stream` (function, line 479) `void load_hindi_lexicon_stream(
    std::istream& in, std::unordered_map<std::string, std::string...`
  - `HindiRuleG2p` (function, line 507) `HindiRuleG2p::HindiRuleG2p(std::filesystem::path dict_tsv, Options options)
    : options_(options)`
  - `HindiRuleG2p` (function, line 521) `HindiRuleG2p::HindiRuleG2p(std::string dict_tsv_utf8, Options options)
    : options_(options)`
  - `word_to_ipa` (function, line 527) `std::string HindiRuleG2p::word_to_ipa(const std::string& word) const`
  - `g2p_single_word` (function, line 531) `std::string HindiRuleG2p::g2p_single_word(std::string_view word) const`
  - `text_to_ipa_no_expand` (function, line 551) `std::string HindiRuleG2p::text_to_ipa_no_expand(
    std::string text, std::vector<G2pWordLog>* p...`
  - `text_to_ipa` (function, line 594) `std::string HindiRuleG2p::text_to_ipa(std::string text,
                                      std...`
  - `dialect_ids` (function, line 603) `std::vector<std::string> HindiRuleG2p::dialect_ids()`
  - `dialect_resolves_to_hindi_rules` (function, line 607) `bool dialect_resolves_to_hindi_rules(std::string_view dialect_id)`
  - `resolve_hindi_dict_path` (function, line 615) `std::filesystem::path resolve_hindi_dict_path(
    const std::filesystem::path& model_root)`
  - `hindi_text_to_ipa` (function, line 620) `std::string hindi_text_to_ipa(const std::string& text, bool with_stress,
                        ...`
  - `tmp` (function, line 34) `const std::string tmp(s);`
  - `0x094D` (variable, line 18) `extern "C" { #include <utf8proc.h> } namespace moonshine_tts { namespace { constexpr char32_t kVirama = 0x094D;`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/hindi-numbers.h`, `core/moonshine-tts/src/lang-specific/hindi.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/hindi.h
- Layer: infrastructure
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 15)
  - `Options` (struct, line 21)
  - `HindiRuleG2p` (class, line 19)
  - `dialect_id` (function, line 34) `const std::string& dialect_id() const`
  - `dialect_ids` (function, line 32) `static std::vector<std::string> dialect_ids();`
  - `dialect_resolves_to_hindi_rules` (function, line 52) `bool dialect_resolves_to_hindi_rules(std::string_view dialect_id);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_HINDI_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_HINDI_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/hindi.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/hindi-rule-g2p-test.cpp`, `core/moonshine-tts/tools/hindi-rule-g2p-cli.cpp`

## core/moonshine-tts/src/lang-specific/ipa-symbols.h
- Layer: testing
- Language: h
- Symbols:
  - `MOONSHINE_TTS_IPA_SYMBOLS_H` (macro, line 2) `#define MOONSHINE_TTS_IPA_SYMBOLS_H`
- Imported by: `core/moonshine-tts/src/lang-specific/dutch.cpp`, `core/moonshine-tts/src/lang-specific/french-oov.cpp`, `core/moonshine-tts/src/lang-specific/french.cpp`, `core/moonshine-tts/src/lang-specific/german.cpp`, `core/moonshine-tts/src/lang-specific/italian.cpp`, `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp`, `core/moonshine-tts/src/lang-specific/portuguese.cpp`, `core/moonshine-tts/src/lang-specific/russian.cpp`

## core/moonshine-tts/src/lang-specific/italian.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `italian_tolower_cp` (function, line 35) `char32_t italian_tolower_cp(char32_t c)`
  - `is_italian_lexicon_key_cp` (function, line 70) `bool is_italian_lexicon_key_cp(char32_t c)`
  - `normalize_lookup_key_utf8` (function, line 85) `std::string normalize_lookup_key_utf8(const std::string& word)`
  - `utf8_lowercase_italian` (function, line 104) `std::string utf8_lowercase_italian(const std::string& word)`
  - `load_italian_lexicon_stream` (function, line 117) `void load_italian_lexicon_stream(
    std::istream& in, std::unordered_map<std::string, std::stri...`
  - `load_italian_lexicon_file` (function, line 149) `void load_italian_lexicon_file(
    const std::filesystem::path& path,
    std::unordered_map<std...`
  - `is_all_ascii_digits` (function, line 162) `bool is_all_ascii_digits(std::string_view s)`
  - `under_100` (function, line 178) `std::string under_100(int n)`
  - `hundred_head` (function, line 235) `std::string hundred_head(int h)`
  - `append_tokens_0_999` (function, line 247) `void append_tokens_0_999(int n, std::vector<std::string>& out)`
  - `spell_1_999_fused` (function, line 274) `std::string spell_1_999_fused(int n)`
  - `append_thousands_multiplier` (function, line 296) `void append_thousands_multiplier(int q, std::vector<std::string>& out)`
  - `below_1_000_000_tokens` (function, line 314) `void below_1_000_000_tokens(int n, std::vector<std::string>& out)`
  - `expand_cardinal_digits_to_italian_words` (function, line 330) `std::string expand_cardinal_digits_to_italian_words(std::string_view s)`
  - `expand_digit_tokens_in_text` (function, line 366) `std::string expand_digit_tokens_in_text(std::string text)`
  - `utf8_to_u32` (function, line 401) `std::u32string utf8_to_u32(const std::string& s)`
  - `u32_to_utf8` (function, line 414) `std::string u32_to_utf8(const std::u32string& s)`
  - `is_vowel_ch` (function, line 422) `bool is_vowel_ch(char32_t c)`
  - `strip_accent_letter` (function, line 429) `char32_t strip_accent_letter(char32_t c)`
  - `should_hiatus_it` (function, line 454) `bool should_hiatus_it(char32_t a, char32_t b)`
  - `vowel_nucleus_spans` (function, line 484) `void vowel_nucleus_spans(const std::u32string& w,
                         std::vector<std::pair<...`
  - `valid_onset2` (function, line 509) `bool valid_onset2(char a, char b)`
  - `split_intervocalic_cluster` (function, line 523) `void split_intervocalic_cluster(const std::string& cluster, std::string& coda,
                  ...`
  - `italian_orthographic_syllables_u32` (function, line 544) `std::vector<std::u32string> italian_orthographic_syllables_u32(
    std::u32string w)`
  - `accented_vowel_in_u32` (function, line 618) `bool accented_vowel_in_u32(char32_t c)`
  - `default_stressed_syllable_index` (function, line 624) `size_t default_stressed_syllable_index(const std::vector<std::u32string>& syls,
                 ...`
  - `insert_primary_stress_before_vowel` (function, line 666) `std::string insert_primary_stress_before_vowel(std::string ipa)`
  - `next_is_vowel_u32` (function, line 693) `bool next_is_vowel_u32(const std::u32string& s, size_t j)`
  - `ei_e_accent` (function, line 705) `bool ei_e_accent(char32_t c)`
  - `italian_cg_palatal_letter` (function, line 712) `bool italian_cg_palatal_letter(char32_t c)`
  - `letters_to_ipa_no_stress` (function, line 718) `std::string letters_to_ipa_no_stress(const std::u32string& su)`
  - `rules_word_to_ipa_utf8` (function, line 980) `std::string rules_word_to_ipa_utf8(const std::string& raw, bool with_stress)`
  - `is_italian_word_char` (function, line 1068) `bool is_italian_word_char(char32_t cp)`
  - `try_consume_italian_word` (function, line 1102) `bool try_consume_italian_word(const std::string& text, size_t pos,
                              ...`
  - `ItalianRuleG2p` (function, line 1158) `ItalianRuleG2p::ItalianRuleG2p(std::filesystem::path dict_tsv, Options options)
    : options_(op...`
  - `ItalianRuleG2p` (function, line 1163) `ItalianRuleG2p::ItalianRuleG2p(std::string dict_tsv_utf8, Options options)
    : options_(options)`
  - `finalize_ipa` (function, line 1169) `std::string ItalianRuleG2p::finalize_ipa(std::string ipa,
                                       ...`
  - `lookup_or_rules` (function, line 1182) `std::string ItalianRuleG2p::lookup_or_rules(const std::string& raw_word) const`
  - `word_to_ipa` (function, line 1231) `std::string ItalianRuleG2p::word_to_ipa(const std::string& word) const`
  - `text_to_ipa_no_expand` (function, line 1253) `std::string ItalianRuleG2p::text_to_ipa_no_expand(
    const std::string& text, std::vector<G2pWo...`
  - `text_to_ipa` (function, line 1323) `std::string ItalianRuleG2p::text_to_ipa(std::string text,
                                       ...`
  - `dialect_resolves_to_italian_rules` (function, line 1331) `bool dialect_resolves_to_italian_rules(std::string_view dialect_id)`
  - `dialect_ids` (function, line 1339) `std::vector<std::string> ItalianRuleG2p::dialect_ids()`
  - `resolve_italian_dict_path` (function, line 1343) `std::filesystem::path resolve_italian_dict_path(
    const std::filesystem::path& model_root)`
  - `range_re` (function, line 367) `static const std::regex range_re(R"(\b(\d+)-(\d+)\b)", std::regex::ECMAScript);`
  - `dig_re` (function, line 369) `static const std::regex dig_re(R"(\b\d+\b)", std::regex::ECMAScript);`
  - `dig_pass` (function, line 1244) `static const std::regex dig_pass(R"(^[0-9]+(?:-[0-9]+)*$)", std::regex::ECMAScript);`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/german.h`, `core/moonshine-tts/src/lang-specific/ipa-symbols.h`, `core/moonshine-tts/src/lang-specific/italian.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/italian.h
- Layer: testing
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 14)
  - `Options` (struct, line 20)
  - `ItalianRuleG2p` (class, line 18)
  - `dialect_id` (function, line 38) `const std::string& dialect_id() const`
  - `dialect_ids` (function, line 36) `static std::vector<std::string> dialect_ids();`
  - `dialect_resolves_to_italian_rules` (function, line 58) `bool dialect_resolves_to_italian_rules(std::string_view dialect_id);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_ITALIAN_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_ITALIAN_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/italian.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/italian-rule-g2p-test.cpp`, `core/moonshine-tts/tools/italian-rule-g2p-cli.cpp`

## core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `utf8_nfkc_utf8proc` (function, line 19) `std::string utf8_nfkc_utf8proc(std::string_view s)`
  - `katakana_to_hiragana_u32` (function, line 31) `std::u32string katakana_to_hiragana_u32(const std::u32string& in)`
  - `u32_to_utf8` (function, line 51) `std::string u32_to_utf8(const std::u32string& u)`
  - `utf8_starts_with_at` (function, line 59) `bool utf8_starts_with_at(const std::string& s, std::size_t off,
                         const st...`
  - `long_mark_extend_last` (function, line 67) `void long_mark_extend_last(std::vector<std::string>& parts)`
  - `geminate_onset` (function, line 152) `std::string geminate_onset(const std::string& onset,
                           const std::string...`
  - `katakana_hiragana_to_ipa` (function, line 163) `std::string katakana_hiragana_to_ipa(std::string_view sv)`
  - `japanese_is_kana_only` (function, line 226) `bool japanese_is_kana_only(std::string_view sv)`
  - `japanese_has_japanese_script` (function, line 255) `bool japanese_has_japanese_script(std::string_view sv)`
  - `tmp` (function, line 20) `const std::string tmp(s);`
- Depends on: `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.h
- Layer: testing
- Language: h
- Symbols:
  - `japanese_is_kana_only` (function, line 13) `bool japanese_is_kana_only(std::string_view utf8);`
  - `japanese_has_japanese_script` (function, line 14) `bool japanese_has_japanese_script(std::string_view utf8);`
  - `MOONSHINE_TTS_JAPANESE_KANA_TO_IPA_H` (macro, line 2) `#define MOONSHINE_TTS_JAPANESE_KANA_TO_IPA_H`
- Imported by: `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp`, `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp`

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
- Layer: testing
- Doc: Russian cardinal expansion (russian_numbers.py). #include from russian.cpp (same TU).
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

## core/moonshine-tts/src/lang-specific/russian.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `is_unicode_mn` (function, line 37) `bool is_unicode_mn(char32_t cp)`
  - `is_combining_mark` (function, line 56) `bool is_combining_mark(char32_t cp)`
  - `russian_tolower_cp` (function, line 58) `char32_t russian_tolower_cp(char32_t c)`
  - `is_russian_vowel_letter` (function, line 68) `bool is_russian_vowel_letter(char32_t c)`
  - `is_russian_lex_key_cp` (function, line 76) `bool is_russian_lex_key_cp(char32_t c)`
  - `append_nfd_expansion` (function, line 126) `void append_nfd_expansion(char32_t cp, std::u32string& out)`
  - `u32_to_utf8` (function, line 136) `std::string u32_to_utf8(const std::u32string& s)`
  - `unicode_tolower_like_python` (function, line 144) `char32_t unicode_tolower_like_python(char32_t cp)`
  - `normalize_lookup_key_utf8` (function, line 163) `std::string normalize_lookup_key_utf8(const std::string& word)`
  - `utf8_russian_lowercase` (function, line 194) `std::string utf8_russian_lowercase(const std::string& word)`
  - `surface_is_all_lowercase_russian` (function, line 212) `bool surface_is_all_lowercase_russian(const std::string& surf)`
  - `load_russian_lexicon_stream` (function, line 216) `void load_russian_lexicon_stream(
    std::istream& in, std::unordered_map<std::string, std::stri...`
  - `load_russian_lexicon_file` (function, line 248) `void load_russian_lexicon_file(
    const std::filesystem::path& path,
    std::unordered_map<std...`
  - `filter_russian_graphemes_keep_stress` (function, line 259) `std::string filter_russian_graphemes_keep_stress(std::string_view raw)`
  - `strip_grapheme_diacritics_utf8` (function, line 281) `std::string strip_grapheme_diacritics_utf8(std::string_view sv)`
  - `acute_stressed_vowel_ordinal` (function, line 305) `std::optional<int> acute_stressed_vowel_ordinal(const std::string& w_nfc)`
  - `vowel_ordinal_to_syllable` (function, line 336) `int vowel_ordinal_to_syllable(const std::vector<std::string>& syls,
                             ...`
  - `russian_orthographic_syllables_utf8` (function, line 357) `std::vector<std::string> russian_orthographic_syllables_utf8(
    const std::string& word_lower)`
  - `remove_if` (function, line 423) `std::remove_if(syllables.begin(), syllables.end(),
                     [](const std::string& x)`
  - `stress_syllable_index` (function, line 429) `int stress_syllable_index(const std::vector<std::string>& syls,
                          const s...`
  - `syllable_index_per_codepoint` (function, line 453) `std::vector<int> syllable_index_per_codepoint(const std::string& w)`
  - `palatalizable_cons` (function, line 465) `bool palatalizable_cons(char32_t ch)`
  - `emit_consonant` (function, line 473) `std::string emit_consonant(char32_t ch, bool palatal)`
  - `ipa_piece_ends_with_palatal` (function, line 525) `bool ipa_piece_ends_with_palatal(const std::string& piece)`
  - `ipa_piece_last_is_vowel_letter` (function, line 534) `bool ipa_piece_last_is_vowel_letter(const std::string& piece)`
  - `ipa_piece_after_hard_consonant` (function, line 547) `bool ipa_piece_after_hard_consonant(const std::string& piece)`
  - `vowel_ipa` (function, line 560) `std::string vowel_ipa(char32_t ch, bool stressed, bool after_palatal,
                      bool ...`
  - `letters_to_ipa_rules` (function, line 620) `std::string letters_to_ipa_rules(const std::string& w_clean, int stress_syl)`
  - `insert_primary_stress_before_vowel` (function, line 789) `std::string insert_primary_stress_before_vowel(std::string s)`
  - `rules_word_to_ipa_single` (function, line 809) `std::string rules_word_to_ipa_single(const std::string& w_clean,
                                ...`
  - `rules_word_to_ipa` (function, line 821) `std::string rules_word_to_ipa(const std::string& raw, bool with_stress)`
  - `is_latin1_supplement_python_word_char` (function, line 886) `bool is_latin1_supplement_python_word_char(char32_t cp)`
  - `is_unicode_word_char_w` (function, line 907) `bool is_unicode_word_char_w(char32_t cp)`
  - `utf8_contains_cyrillic` (function, line 932) `bool utf8_contains_cyrillic(const std::string& tok)`
  - `try_consume_unicode_word` (function, line 946) `bool try_consume_unicode_word(const std::string& text, size_t pos,
                              ...`
  - `normalize_russian_fleeting_palatal_markers_utf8` (function, line 976) `std::string normalize_russian_fleeting_palatal_markers_utf8(std::string ipa)`
  - `RussianRuleG2p` (function, line 993) `RussianRuleG2p::RussianRuleG2p(std::filesystem::path dict_tsv, Options options)
    : options_(op...`
  - `RussianRuleG2p` (function, line 998) `RussianRuleG2p::RussianRuleG2p(std::string dict_tsv_utf8, Options options)
    : options_(options)`
  - `finalize_ipa` (function, line 1004) `std::string RussianRuleG2p::finalize_ipa(std::string ipa) const`
  - `lookup_or_rules` (function, line 1018) `std::string RussianRuleG2p::lookup_or_rules(const std::string& raw_word) const`
  - `word_to_ipa` (function, line 1061) `std::string RussianRuleG2p::word_to_ipa(const std::string& word) const`
  - `text_to_ipa_no_expand` (function, line 1083) `std::string RussianRuleG2p::text_to_ipa_no_expand(
    const std::string& text, std::vector<G2pWo...`
  - `text_to_ipa` (function, line 1157) `std::string RussianRuleG2p::text_to_ipa(std::string text,
                                       ...`
  - `dialect_resolves_to_russian_rules` (function, line 1165) `bool dialect_resolves_to_russian_rules(std::string_view dialect_id)`
  - `dialect_ids` (function, line 1173) `std::vector<std::string> RussianRuleG2p::dialect_ids()`
  - `resolve_russian_dict_path` (function, line 1177) `std::filesystem::path resolve_russian_dict_path(
    const std::filesystem::path& model_root)`
  - `dig_pass` (function, line 1074) `static const std::regex dig_pass(R"(^[0-9]+(?:-[0-9]+)*$)", std::regex::ECMAScript);`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/ipa-postprocess.h`, `core/moonshine-tts/src/lang-specific/german.h`, `core/moonshine-tts/src/lang-specific/ipa-symbols.h`, `core/moonshine-tts/src/lang-specific/russian-numbers.cpp`, `core/moonshine-tts/src/lang-specific/russian.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/russian.h
- Layer: testing
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 14)
  - `Options` (struct, line 19)
  - `RussianRuleG2p` (class, line 17)
  - `dialect_id` (function, line 37) `const std::string& dialect_id() const`
  - `dialect_ids` (function, line 35) `static std::vector<std::string> dialect_ids();`
  - `dialect_resolves_to_russian_rules` (function, line 57) `bool dialect_resolves_to_russian_rules(std::string_view dialect_id);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_RUSSIAN_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_RUSSIAN_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/russian.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/russian-rule-g2p-test.cpp`

## core/moonshine-tts/src/lang-specific/spanish-numbers.cpp
- Layer: testing
- Doc: Spanish cardinal expansion (spanish_numbers.py). #include from spanish.cpp (same TU).
- Language: cpp
- Symbols:
  - `es_ascii_all_digits` (function, line 14) `bool es_ascii_all_digits(std::string_view s)`
  - `es_append_under_100` (function, line 77) `void es_append_under_100(int n, std::vector<std::string>& out)`
  - `es_append_below_1000` (function, line 98) `void es_append_below_1000(int n, std::vector<std::string>& out)`
  - `es_append_below_1_000_000` (function, line 123) `void es_append_below_1_000_000(int n, std::vector<std::string>& out)`
  - `expand_cardinal_digits_to_spanish_words` (function, line 144) `std::string expand_cardinal_digits_to_spanish_words(std::string_view s)`
  - `expand_spanish_digit_tokens_in_text` (function, line 180) `std::string expand_spanish_digit_tokens_in_text(std::string text)`
  - `range_re` (function, line 181) `static const std::regex range_re(R"(\b(\d+)-(\d+)\b)", std::regex::ECMAScript);`
  - `dig_re` (function, line 183) `static const std::regex dig_re(R"(\b\d+\b)", std::regex::ECMAScript);`
- Depends on: `core/moonshine-tts/src/utf8-utils.h`
- Imported by: `core/moonshine-tts/src/lang-specific/spanish.cpp`

## core/moonshine-tts/src/lang-specific/spanish-unicode-tables.cpp
- Layer: testing
- Language: cpp
- Depends on: `core/moonshine-tts/src/lang-specific/spanish-unicode-tables.h`

## core/moonshine-tts/src/lang-specific/spanish-unicode-tables.h
- Layer: testing
- Language: h
- Symbols:
  - `k_unicode_strip_table` (variable, line 11) `extern const std::pair<char32_t, const char*> k_unicode_strip_table[];`
  - `k_unicode_strip_table_size` (variable, line 12) `extern const std::size_t k_unicode_strip_table_size;`
  - `k_unicode_lower_table` (variable, line 13) `extern const std::pair<char32_t, const char*> k_unicode_lower_table[];`
  - `k_unicode_lower_table_size` (variable, line 14) `extern const std::size_t k_unicode_lower_table_size;`
  - `k_unicode_word_bitmap` (variable, line 15) `extern const std::uint32_t k_unicode_word_bitmap[];`
  - `k_unicode_word_bitmap_words` (variable, line 16) `extern const std::uint32_t k_unicode_word_bitmap_words;`
  - `k_unicode_space_bitmap` (variable, line 17) `extern const std::uint32_t k_unicode_space_bitmap[];`
  - `k_unicode_space_bitmap_words` (variable, line 18) `extern const std::uint32_t k_unicode_space_bitmap_words;`
  - `MOONSHINE_TTS_LANG_SPECIFIC_SPANISH_UNICODE_TABLES_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_SPANISH_UNICODE_TABLES_H`
- Imported by: `core/moonshine-tts/src/lang-specific/spanish-unicode-tables.cpp`, `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp`

## core/moonshine-tts/src/lang-specific/spanish-unicode.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `lookup_sorted_pair` (function, line 12) `const char* lookup_sorted_pair(const std::pair<char32_t, const char*>* table,
                   ...`
  - `lower_bound` (function, line 17) `std::lower_bound(first, last, key,
                       [](const std::pair<char32_t, const char...`
  - `unicode_bitmap_get` (function, line 26) `bool unicode_bitmap_get(const std::uint32_t* bitmap, std::uint32_t nwords,
                      ...`
  - `utf32_to_utf8` (function, line 40) `std::string utf32_to_utf8(const std::u32string& u)`
  - `utf8_to_utf32` (function, line 49) `std::u32string utf8_to_utf32(const std::string& s)`
  - `unicode_lower_utf8` (function, line 53) `std::string unicode_lower_utf8(const std::string& s)`
  - `strip_accents_utf8` (function, line 72) `std::string strip_accents_utf8(const std::string& s)`
  - `word_key` (function, line 91) `std::string word_key(const std::string& wraw)`
  - `is_word_char` (function, line 95) `bool is_word_char(char32_t cp)`
  - `is_space_char` (function, line 100) `bool is_space_char(char32_t cp)`
  - `strip_replacement_utf8` (function, line 105) `const char* strip_replacement_utf8(char32_t cp)`
- Depends on: `core/moonshine-tts/src/lang-specific/spanish-unicode-tables.h`, `core/moonshine-tts/src/lang-specific/spanish-unicode.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/spanish-unicode.h
- Layer: testing
- Language: h
- Symbols:
  - `is_word_char` (function, line 14) `bool is_word_char(char32_t cp);`
  - `is_space_char` (function, line 15) `bool is_space_char(char32_t cp);`
  - `strip_replacement_utf8` (function, line 17) `const char* strip_replacement_utf8(char32_t cp);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_SPANISH_UNICODE_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_SPANISH_UNICODE_H`
- Imported by: `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp`, `core/moonshine-tts/src/lang-specific/spanish.cpp`

## core/moonshine-tts/src/lang-specific/spanish.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `XExc` (struct, line 264)
  - `is_vowel_ch` (function, line 23) `bool is_vowel_ch(char32_t ch)`
  - `should_hiatus` (function, line 43) `bool should_hiatus(char32_t a, char32_t b)`
  - `is_valid_onset2` (function, line 145) `bool is_valid_onset2(char32_t a, char32_t b)`
  - `clean_syllable_word` (function, line 178) `std::u32string clean_syllable_word(const std::u32string &word_lower)`
  - `orthographic_syllables_utf8` (function, line 189) `std::vector<std::string> orthographic_syllables_utf8(
    const std::string &word_lower_utf8)`
  - `default_stressed_syllable_index_v2` (function, line 226) `size_t default_stressed_syllable_index_v2(const std::u32string &w_clean_lower)`
  - `lookup_x_exception` (function, line 295) `const char *lookup_x_exception(const std::string &wkey)`
  - `apply_nasal_assimilation` (function, line 304) `std::string apply_nasal_assimilation(std::string s,
                                     const Sp...`
  - `insert_primary_stress_before_vowel` (function, line 333) `std::string insert_primary_stress_before_vowel(const std::string &ipa)`
  - `count_primary_stress_utf8` (function, line 356) `size_t count_primary_stress_utf8(const std::string &ipa)`
  - `ipa_stress_at_start` (function, line 371) `bool ipa_stress_at_start(const std::string &ipa)`
  - `apply_narrow_intervocalic_obstruents` (function, line 380) `std::string apply_narrow_intervocalic_obstruents(std::string ipa)`
  - `apply_coda_s_weakening` (function, line 417) `std::string apply_coda_s_weakening(std::string ipa,
                                   SpanishDia...`
  - `postprocess_lexical_ipa` (function, line 432) `std::string postprocess_lexical_ipa(std::string ipa,
                                    const Sp...`
  - `prev_phoneme_was_vowel` (function, line 458) `bool prev_phoneme_was_vowel(const std::vector<std::string> &out)`
  - `y_is_consonant` (function, line 470) `bool y_is_consonant(const std::u32string &letters_lower, size_t i)`
  - `to_lower_cp` (function, line 496) `char32_t to_lower_cp(char32_t c)`
  - `letters_to_ipa_no_stress` (function, line 504) `std::string letters_to_ipa_no_stress(const std::u32string &syl_lower,
                           ...`
  - `filter_word_letters_utf32` (function, line 773) `std::u32string filter_word_letters_utf32(const std::string &wraw)`
  - `make_common` (function, line 791) `SpanishDialect make_common(const std::string &id, std::string ce_ci_z_ipa,
                      ...`
  - `spanish_dialect_cli_ids` (function, line 816) `std::vector<std::string> spanish_dialect_cli_ids()`
  - `dialect_ids` (function, line 823) `std::vector<std::string> SpanishRuleG2p::dialect_ids()`
  - `spanish_dialect_from_cli_id` (function, line 827) `SpanishDialect spanish_dialect_from_cli_id(
    const std::string &cli_id, bool narrow_intervocal...`
  - `SpanishRuleG2p` (function, line 929) `SpanishRuleG2p::SpanishRuleG2p(SpanishDialect dialect, bool with_stress,
                        ...`
  - `word_to_ipa` (function, line 935) `std::string SpanishRuleG2p::word_to_ipa(const std::string &word) const`
  - `text_to_ipa_no_expand` (function, line 1003) `std::string SpanishRuleG2p::text_to_ipa_no_expand(
    const std::string &text, std::vector<G2pWo...`
  - `text_to_ipa` (function, line 1087) `std::string SpanishRuleG2p::text_to_ipa(std::string text,
                                       ...`
  - `spanish_word_to_ipa` (function, line 1095) `std::string spanish_word_to_ipa(const std::string &word,
                                const Sp...`
  - `spanish_text_to_ipa` (function, line 1102) `std::string spanish_text_to_ipa(const std::string &text,
                                const Sp...`
  - `dig_pass` (function, line 957) `static const std::regex dig_pass(R"(^[0-9]+$)", std::regex::ECMAScript);`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/spanish-numbers.cpp`, `core/moonshine-tts/src/lang-specific/spanish-unicode.h`, `core/moonshine-tts/src/lang-specific/spanish.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/spanish.h
- Layer: testing
- Language: h
- Symbols:
  - `SpanishDialect` (struct, line 13)
  - `CodaS` (enum, line 26)
  - `CodaS` (class, line 26)
  - `SpanishRuleG2p` (class, line 30)
  - `dialect` (function, line 37) `const SpanishDialect& dialect() const`
  - `with_stress` (function, line 38) `bool with_stress() const`
  - `expand_cardinal_digits` (function, line 39) `bool expand_cardinal_digits() const`
  - `dialect_ids` (function, line 35) `static std::vector<std::string> dialect_ids();`
  - `MOONSHINE_TTS_LANG_SPECIFIC_SPANISH_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_SPANISH_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/spanish.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/spanish-rule-g2p-test.cpp`, `core/moonshine-tts/tools/moonshine-g2p-cli.cpp`

## core/moonshine-tts/src/lang-specific/turkish.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `is_all_ascii_digits` (function, line 25) `bool is_all_ascii_digits(std::string_view s)`
  - `append_under_100` (function, line 46) `void append_under_100(int n, std::vector<std::string>& out)`
  - `append_tokens_0_999` (function, line 71) `void append_tokens_0_999(int n, std::vector<std::string>& out)`
  - `append_below_1_000_000` (function, line 95) `void append_below_1_000_000(int n, std::vector<std::string>& out)`
  - `join_space` (function, line 116) `std::string join_space(const std::vector<std::string>& p)`
  - `expand_cardinal_digits_to_turkish_words` (function, line 127) `std::string expand_cardinal_digits_to_turkish_words(std::string_view s)`
  - `expand_turkish_digit_tokens_in_text` (function, line 161) `std::string expand_turkish_digit_tokens_in_text(std::string text)`
  - `utf8_to_u32_nfc` (function, line 196) `std::u32string utf8_to_u32_nfc(const std::string& s)`
  - `turkish_tolower_cp` (function, line 207) `char32_t turkish_tolower_cp(char32_t cp)`
  - `turkish_lower_u32` (function, line 218) `std::u32string turkish_lower_u32(const std::u32string& s)`
  - `is_tr_g2p_letter` (function, line 227) `bool is_tr_g2p_letter(char32_t c)`
  - `letters_only_u32` (function, line 272) `std::u32string letters_only_u32(const std::u32string& w)`
  - `is_vowel_orth` (function, line 285) `bool is_vowel_orth(char32_t c)`
  - `is_front_vowel` (function, line 291) `bool is_front_vowel(char32_t c)`
  - `prev_letter_index` (function, line 296) `std::optional<size_t> prev_letter_index(const std::u32string& w, size_t i)`
  - `next_letter_index` (function, line 306) `std::optional<size_t> next_letter_index(const std::u32string& w, size_t i)`
  - `next_vowel_from` (function, line 316) `std::optional<char32_t> next_vowel_from(const std::u32string& w, size_t start)`
  - `last_vowel_before` (function, line 325) `std::optional<char32_t> last_vowel_before(const std::u32string& w, size_t end)`
  - `harmony_vowel_for_kg` (function, line 334) `std::optional<char32_t> harmony_vowel_for_kg(const std::u32string& w,
                           ...`
  - `map_k_or_g` (function, line 343) `std::string map_k_or_g(char32_t ch, const std::u32string& w, size_t i)`
  - `map_simple_char` (function, line 355) `std::string map_simple_char(char32_t c)`
  - `is_vowel_ipa_char` (function, line 430) `bool is_vowel_ipa_char(char32_t c)`
  - `utf8_ipa_to_u32` (function, line 435) `std::u32string utf8_ipa_to_u32(std::string_view s)`
  - `u32_to_utf8_ipa` (function, line 440) `std::string u32_to_utf8_ipa(const std::u32string& s)`
  - `insert_primary_stress_final` (function, line 448) `std::string insert_primary_stress_final(const std::string& ipa_utf8)`
  - `is_turkish_word_char` (function, line 497) `bool is_turkish_word_char(char32_t cp)`
  - `is_space_cp` (function, line 517) `bool is_space_cp(char32_t cp)`
  - `TurkishRuleG2p` (function, line 528) `TurkishRuleG2p::TurkishRuleG2p(Options options) : options_(options)`
  - `dialect_ids` (function, line 530) `std::vector<std::string> TurkishRuleG2p::dialect_ids()`
  - `word_to_ipa` (function, line 534) `std::string TurkishRuleG2p::word_to_ipa(const std::string& word) const`
  - `text_to_ipa_no_expand` (function, line 618) `std::string TurkishRuleG2p::text_to_ipa_no_expand(
    const std::string& text, std::vector<G2pWo...`
  - `text_to_ipa` (function, line 696) `std::string TurkishRuleG2p::text_to_ipa(std::string text,
                                       ...`
  - `dialect_resolves_to_turkish_rules` (function, line 704) `bool dialect_resolves_to_turkish_rules(std::string_view dialect_id)`
  - `turkish_word_to_ipa` (function, line 715) `std::string turkish_word_to_ipa(const std::string& word, bool with_stress,
                      ...`
  - `turkish_text_to_ipa` (function, line 723) `std::string turkish_text_to_ipa(const std::string& text, bool with_stress,
                      ...`
  - `range_re` (function, line 162) `static const std::regex range_re(R"(\b(\d+)-(\d+)\b)", std::regex::ECMAScript);`
  - `dig_re` (function, line 164) `static const std::regex dig_re(R"(\b\d+\b)", std::regex::ECMAScript);`
  - `dig_pass` (function, line 549) `static const std::regex dig_pass(R"(^[0-9]+$)", std::regex::ECMAScript);`
  - `utf8_append_codepoint` (variable, line 6) `extern "C" { #include <utf8proc.h> } #include <cctype> #include <cstdlib> #include <optional> #include <regex> #include <string> #include <string_view> #include <vector> namespace moonshine_tts { name`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/turkish.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/turkish.h
- Layer: testing
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 11)
  - `Options` (struct, line 19)
  - `TurkishRuleG2p` (class, line 17)
  - `dialect_id` (function, line 29) `const std::string& dialect_id() const`
  - `with_stress` (function, line 30) `bool with_stress() const`
  - `expand_cardinal_digits` (function, line 31) `bool expand_cardinal_digits() const`
  - `dialect_ids` (function, line 27) `static std::vector<std::string> dialect_ids();`
  - `dialect_resolves_to_turkish_rules` (function, line 49) `bool dialect_resolves_to_turkish_rules(std::string_view dialect_id);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_TURKISH_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_TURKISH_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/turkish.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/turkish-rule-g2p-test.cpp`

## core/moonshine-tts/src/lang-specific/ukrainian.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `is_all_ascii_digits` (function, line 27) `bool is_all_ascii_digits(std::string_view s)`
  - `utf8_nfc_utf8proc` (function, line 42) `std::string utf8_nfc_utf8proc(const std::string& s)`
  - `ukrainian_strip_stress_marks_utf8` (function, line 53) `std::string ukrainian_strip_stress_marks_utf8(std::string s)`
  - `utf8_to_u32_nfc` (function, line 79) `std::u32string utf8_to_u32_nfc(const std::string& s)`
  - `ukrainian_lower_u32` (function, line 90) `std::u32string ukrainian_lower_u32(const std::u32string& s)`
  - `thousand_noun_utf8` (function, line 120) `std::string thousand_noun_utf8(int h)`
  - `append_under_100_thousand_mult` (function, line 134) `void append_under_100_thousand_mult(int n, std::vector<std::string>& out)`
  - `append_under_100_plain` (function, line 183) `void append_under_100_plain(int n, std::vector<std::string>& out)`
  - `append_tokens_thousands_multiplier` (function, line 203) `void append_tokens_thousands_multiplier(int h, std::vector<std::string>& out)`
  - `append_tokens_0_999` (function, line 224) `void append_tokens_0_999(int n, std::vector<std::string>& out)`
  - `append_below_1_000_000` (function, line 243) `void append_below_1_000_000(int n, std::vector<std::string>& out)`
  - `join_space` (function, line 259) `std::string join_space(const std::vector<std::string>& p)`
  - `expand_cardinal_digits_to_ukrainian_words` (function, line 270) `std::string expand_cardinal_digits_to_ukrainian_words(std::string_view s)`
  - `expand_ukrainian_digit_tokens_in_text` (function, line 304) `std::string expand_ukrainian_digit_tokens_in_text(std::string text)`
  - `is_vowel_letter` (function, line 340) `bool is_vowel_letter(char32_t c)`
  - `is_soft_vowel` (function, line 346) `bool is_soft_vowel(char32_t c)`
  - `is_hard_no_pal` (function, line 351) `bool is_hard_no_pal(char32_t c)`
  - `is_palatalizable` (function, line 356) `bool is_palatalizable(char32_t c)`
  - `next_letter_index` (function, line 363) `std::optional<size_t> next_letter_index(const std::u32string& w, size_t start)`
  - `v_allophone` (function, line 389) `std::string v_allophone(const std::u32string& w, size_t i)`
  - `ends_with_palatal_suffix` (function, line 404) `bool ends_with_palatal_suffix(const std::string& p)`
  - `is_vowel_ipa_piece` (function, line 410) `bool is_vowel_ipa_piece(const std::string& p)`
  - `piece_ends_palatalized_consonant` (function, line 434) `bool piece_ends_palatalized_consonant(const std::vector<std::string>& pieces)`
  - `palatalize_last` (function, line 452) `void palatalize_last(std::vector<std::string>& pieces)`
  - `vowel_ipa` (function, line 471) `std::string vowel_ipa(char32_t ch, bool force_j, bool after_vowel_letter,
                      b...`
  - `ipa_vowel_char` (function, line 520) `bool ipa_vowel_char(char32_t c)`
  - `u32_to_utf8` (function, line 525) `std::string u32_to_utf8(const std::u32string& s)`
  - `insert_primary_stress_penultimate` (function, line 533) `std::string insert_primary_stress_penultimate(const std::string& ipa_utf8)`
  - `base_cons_ipa` (function, line 574) `std::string base_cons_ipa(char32_t c)`
  - `word_to_ipa_inner` (function, line 621) `std::string word_to_ipa_inner(const std::u32string& w0, bool with_stress)`
  - `filter_uk_word_chars` (function, line 727) `std::u32string filter_uk_word_chars(const std::u32string& w)`
  - `is_ukrainian_word_char` (function, line 744) `bool is_ukrainian_word_char(char32_t cp)`
  - `is_space_cp` (function, line 761) `bool is_space_cp(char32_t cp)`
  - `word_to_ipa_from_utf32_word` (function, line 768) `std::string word_to_ipa_from_utf32_word(const std::u32string& letters,
                          ...`
  - `hyphen_join_word_ipas` (function, line 776) `std::string hyphen_join_word_ipas(const std::string& tok, bool with_stress)`
  - `UkrainianRuleG2p` (function, line 803) `UkrainianRuleG2p::UkrainianRuleG2p(Options options) : options_(options)`
  - `dialect_ids` (function, line 805) `std::vector<std::string> UkrainianRuleG2p::dialect_ids()`
  - `word_to_ipa` (function, line 809) `std::string UkrainianRuleG2p::word_to_ipa(const std::string& word) const`
  - `text_to_ipa_no_expand` (function, line 832) `std::string UkrainianRuleG2p::text_to_ipa_no_expand(
    const std::string& text, std::vector<G2p...`
  - `text_to_ipa` (function, line 909) `std::string UkrainianRuleG2p::text_to_ipa(
    std::string text, std::vector<G2pWordLog>* per_wor...`
  - `dialect_resolves_to_ukrainian_rules` (function, line 917) `bool dialect_resolves_to_ukrainian_rules(std::string_view dialect_id)`
  - `ukrainian_word_to_ipa` (function, line 928) `std::string ukrainian_word_to_ipa(const std::string& word, bool with_stress,
                    ...`
  - `ukrainian_text_to_ipa` (function, line 936) `std::string ukrainian_text_to_ipa(const std::string& text, bool with_stress,
                    ...`
  - `range_re` (function, line 305) `static const std::regex range_re(R"(\b(\d+)-(\d+)\b)", std::regex::ECMAScript);`
  - `dig_re` (function, line 307) `static const std::regex dig_re(R"(\b\d+\b)", std::regex::ECMAScript);`
  - `dig_pass` (function, line 824) `static const std::regex dig_pass(R"(^[0-9]+$)", std::regex::ECMAScript);`
  - `trim_ascii_ws_copy` (variable, line 6) `extern "C" { #include <utf8proc.h> } #include <cctype> #include <cstdlib> #include <optional> #include <regex> #include <string> #include <string_view> #include <unordered_set> #include <vector> names`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/ukrainian.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/ukrainian.h
- Layer: testing
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 11)
  - `Options` (struct, line 18)
  - `UkrainianRuleG2p` (class, line 16)
  - `dialect_id` (function, line 28) `const std::string& dialect_id() const`
  - `with_stress` (function, line 29) `bool with_stress() const`
  - `expand_cardinal_digits` (function, line 30) `bool expand_cardinal_digits() const`
  - `dialect_ids` (function, line 26) `static std::vector<std::string> dialect_ids();`
  - `dialect_resolves_to_ukrainian_rules` (function, line 48) `bool dialect_resolves_to_ukrainian_rules(std::string_view dialect_id);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_UKRAINIAN_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_UKRAINIAN_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/ukrainian.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/ukrainian-rule-g2p-test.cpp`

## core/moonshine-tts/src/lang-specific/vietnamese.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `utf8_nfc_utf8proc` (function, line 23) `std::string utf8_nfc_utf8proc(std::string_view s)`
  - `utf8_lower_nfc` (function, line 35) `std::string utf8_lower_nfc(std::string_view s)`
  - `starts_with_sv` (function, line 54) `bool starts_with_sv(std::string_view s, std::string_view p)`
  - `ends_with_str` (function, line 58) `bool ends_with_str(const std::string& s, const std::string& suf)`
  - `split_tone` (function, line 64) `int split_tone(std::string_view in, std::string& body_nfc_out)`
  - `is_vowel_letter_char` (function, line 101) `bool is_vowel_letter_char(char32_t cp)`
  - `is_vowel_first_utf8` (function, line 119) `bool is_vowel_first_utf8(std::string_view s)`
  - `front_vowel_utf8` (function, line 131) `bool front_vowel_utf8(std::string_view s)`
  - `rime_is_only_i` (function, line 152) `bool rime_is_only_i(std::string_view rest)`
  - `wants_labial_coda` (function, line 307) `bool wants_labial_coda(const std::string& nuc_ipa)`
  - `coda_simple` (function, line 323) `std::string coda_simple(const std::string& coda, const std::string& nuc_ipa)`
  - `nucleus_to_ipa` (function, line 355) `std::string nucleus_to_ipa(std::string_view nuc_sv)`
  - `combine_nucleus_coda` (function, line 555) `std::string combine_nucleus_coda(const std::string& nuc_orth,
                                 co...`
  - `coda_obstruent_sac` (function, line 597) `bool coda_obstruent_sac(const std::string& coda)`
  - `tone_suffix_ipa` (function, line 602) `std::string tone_suffix_ipa(int tone, const std::string& coda_orth)`
  - `apply_tone` (function, line 632) `std::string apply_tone(const std::string& base, int tone, bool has_coda,
                       c...`
  - `is_unicode_edge_punct` (function, line 646) `bool is_unicode_edge_punct(char32_t cp, bool leading)`
  - `strip_edge_punct` (function, line 670) `std::string strip_edge_punct(std::string_view tok)`
  - `max_lex_key_words` (function, line 715) `int max_lex_key_words(const std::unordered_map<std::string, std::string>& lex)`
  - `load_vietnamese_lexicon_stream` (function, line 729) `void load_vietnamese_lexicon_stream(
    std::istream& in, std::unordered_map<std::string, std::s...`
  - `syllable_to_ipa` (function, line 758) `std::string VietnameseRuleG2p::syllable_to_ipa(std::string_view syllable_utf8)`
  - `VietnameseRuleG2p` (function, line 785) `VietnameseRuleG2p::VietnameseRuleG2p(std::filesystem::path dict_tsv)`
  - `VietnameseRuleG2p` (function, line 803) `VietnameseRuleG2p::VietnameseRuleG2p(std::string dict_tsv_utf8)`
  - `word_to_ipa` (function, line 812) `std::string VietnameseRuleG2p::word_to_ipa(std::string_view word) const`
  - `g2p_single_token` (function, line 816) `std::string VietnameseRuleG2p::g2p_single_token(std::string_view token) const`
  - `text_to_ipa` (function, line 828) `std::string VietnameseRuleG2p::text_to_ipa(
    std::string text, std::vector<G2pWordLog>* per_wo...`
  - `dialect_ids` (function, line 942) `std::vector<std::string> VietnameseRuleG2p::dialect_ids()`
  - `dialect_resolves_to_vietnamese_rules` (function, line 947) `bool dialect_resolves_to_vietnamese_rules(std::string_view dialect_id)`
  - `resolve_vietnamese_dict_path` (function, line 955) `std::filesystem::path resolve_vietnamese_dict_path(
    const std::filesystem::path& model_root)`
  - `tmp` (function, line 24) `const std::string tmp(s);`
  - `body` (function, line 174) `const std::string body(body_sv);`
  - `rime` (function, line 295) `const std::string rime(rime_sv);`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/vietnamese.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/vietnamese.h
- Layer: testing
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 13)
  - `VietnameseRuleG2p` (class, line 17)
  - `dialect_ids` (function, line 22) `static std::vector<std::string> dialect_ids();`
  - `syllable_to_ipa` (function, line 33) `static std::string syllable_to_ipa(std::string_view syllable_utf8);`
  - `dialect_resolves_to_vietnamese_rules` (function, line 42) `bool dialect_resolves_to_vietnamese_rules(std::string_view dialect_id);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_VIETNAMESE_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_VIETNAMESE_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/vietnamese.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/vietnamese-rule-g2p-test.cpp`, `core/moonshine-tts/tools/vietnamese-rule-g2p-cli.cpp`
