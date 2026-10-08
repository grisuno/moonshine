# Subsystem: lang-specific (page 1 of 4)
Pages: [KB_lang-specific.md](KB_lang-specific.md), [KB_lang-specific_p2.md](KB_lang-specific_p2.md), [KB_lang-specific_p3.md](KB_lang-specific_p3.md), [KB_lang-specific_p4.md](KB_lang-specific_p4.md)

## core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp
- Doc: is_punct_char_word_group_u32: ``token_word_group_indices`` uses :func:`_is_punct_char` (Unicode...
- Layer: testing
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
- Doc: ArabicDiacOnnx: BERT token-classification tashkīl (Arabert-style), mirroring...
- Layer: testing
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
- Doc: ArabicRuleG2p: MSA Arabic G2P: ONNX partial tashkīl + lexicon + IPA rules (mirrors...
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
- Doc: ChineseOnnxG2p: ONNX BIO segmentation + UPOS + ``data/zh_hans/dict.tsv`` (mirrors...
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
- Doc: is_punct_char_word_group_u32: ``token_word_group_indices`` uses :func:`_is_punct_char` (Unicode...
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
- Doc: ChineseTokPosOnnx: Simplified-Chinese surfaces + UD UPOS via ONNX...
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
- Doc: ChineseRuleG2p: Simplified Chinese lexicon G2P (``data/zh_hans/dict.tsv`` ipa-dict IPA)...
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
- Layer: testing
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
- Doc: CmudictTsv: word key (normalized grapheme) -> sorted unique IPA strings (TSV: word<TAB>ipa).
- Layer: testing
- Language: h
- Symbols:
  - `CmudictTsv` (class, line 14)
  - `lookup` (function, line 19) `const std::vector<std::string>* lookup(std::string_view key) const;`
  - `MOONSHINE_TTS_CMUDICT_TSV_H` (macro, line 2) `#define MOONSHINE_TTS_CMUDICT_TSV_H`
- Imported by: `core/moonshine-tts/src/lang-specific/cmudict-tsv.cpp`, `core/moonshine-tts/src/lang-specific/english.cpp`, `core/moonshine-tts/tests/cmudict-tsv-test.cpp`

## core/moonshine-tts/src/lang-specific/dutch.cpp
- Doc: append_lexicon_folded: Fold to ``a-z`` + hyphen for TSV keys (mirrors Python...
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
- Doc: DutchRuleG2p: Rule- and lexicon-based Dutch G2P, mirroring ``dutch_rule_g2p.py`` /...
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


Next: [KB_lang-specific_p2.md](KB_lang-specific_p2.md)
