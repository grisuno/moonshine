# Subsystem: lang-specific

## core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp
- Layer: infrastructure
- Doc: include "arabic-diac-onnx.h"  include <nlohmann/json.h> include <onnxruntime_cxx_api.h>  include <array> include <cctype
- Language: cpp
- Symbols:
  - `BasicTokCfg` (struct, line 315)
  - `EncodedWp` (struct, line 427)
  - `Idx` (struct, line 517)
  - `open_ar_session` (function, line 33) `std::unique_ptr<Ort::Session> open_ar_session(
    Ort::Env& env, const std::filesystem::path& mo...`
  - `open_ar_session_memory` (function, line 50) `std::unique_ptr<Ort::Session> open_ar_session_memory(
    Ort::Env& env, const void* data, size_t...`
  - `slurp_utf8_file_ar` (function, line 64) `std::string slurp_utf8_file_ar(const std::filesystem::path& p)`
  - `bundle_load_utf8_ar` (function, line 74) `bool bundle_load_utf8_ar(const MoonshineG2POptions* opt,
                         std::string_vie...`
  - `bundle_load_binary_ar` (function, line 93) `bool bundle_load_binary_ar(const MoonshineG2POptions* opt,
                           std::string...`
  - `utf8_to_u32` (function, line 126) `std::u32string utf8_to_u32(std::string_view utf8)`
  - `u32_to_utf8` (function, line 139) `std::string u32_to_utf8(const std::u32string& s)`
  - `is_space_u32` (function, line 147) `bool is_space_u32(char32_t c)`
  - `is_control_u32` (function, line 156) `bool is_control_u32(char32_t c)`
  - `is_punctuation_u32` (function, line 165) `bool is_punctuation_u32(char32_t c)`
  - `is_punct_char_word_group_u32` (function, line 179) `bool is_punct_char_word_group_u32(char32_t c)`
  - `is_chinese_char` (function, line 183) `bool is_chinese_char(std::uint32_t cp)`
  - `u32_nfc` (function, line 192) `std::u32string u32_nfc(const std::u32string& s)`
  - `strip_mn_nfd` (function, line 204) `std::u32string strip_mn_nfd(const std::u32string& s)`
  - `to_lower_u32` (function, line 224) `std::u32string to_lower_u32(const std::u32string& s)`
  - `clean_text_u32` (function, line 233) `std::u32string clean_text_u32(const std::u32string& text)`
  - `tokenize_chinese_chars_u32` (function, line 245) `std::u32string tokenize_chinese_chars_u32(const std::u32string& text)`
  - `split_u32_whitespace` (function, line 259) `std::vector<std::u32string> split_u32_whitespace(std::u32string_view s)`
  - `run_split_on_punc_u32` (function, line 284) `std::vector<std::u32string> run_split_on_punc_u32(const std::u32string& text)`
  - `normalization_ref_u32` (function, line 320) `std::u32string normalization_ref_u32(const std::u32string& text_u32,
                            ...`
  - `basic_tokenize_u32` (function, line 329) `std::vector<std::u32string> basic_tokenize_u32(
    const std::u32string& original_text_u32, cons...`
  - `align_basic_tokens_u32` (function, line 361) `void align_basic_tokens_u32(const std::u32string& ref,
                            const std::vec...`
  - `wordpiece_tokenize_u32` (function, line 378) `std::vector<std::u32string> wordpiece_tokenize_u32(
    const std::u32string& token,
    const st...`
  - `encode_bert_wordpiece` (function, line 433) `EncodedWp encode_bert_wordpiece(
    const std::u32string& text_u32,
    const std::unordered_map...`
  - `is_arabic_anchor_char` (function, line 671) `bool is_arabic_anchor_char(char32_t c)`
  - `anchor_index_for_span` (function, line 685) `std::optional<int> anchor_index_for_span(const std::u32string& ref, int s,
                      ...`
  - `strip_arabic_diacritics_u32` (function, line 699) `std::u32string strip_arabic_diacritics_u32(const std::u32string& s)`
  - `ArabicDiacOnnx` (function, line 725) `ArabicDiacOnnx::ArabicDiacOnnx(const MoonshineG2POptions* opt,
                               std...`
  - `diacritize` (function, line 786) `std::string ArabicDiacOnnx::diacritize(std::string_view text_utf8) const`
  - `make_g2p_ort_session_options` (function, line 42) `make_g2p_ort_session_options(ort_providers, coreml_cache_dir));`
  - `ort_add_external_initializer_files_for_onnx_model_buffer` (function, line 59) `ort_add_external_initializer_files_for_onnx_model_buffer(so, opt->files, model_map_key);`
  - `in` (function, line 66) `std::ifstream in(p, std::ios::binary);`
  - `utf8_decode_at` (function, line 133) `utf8_decode_at(std::string(utf8), i, cp, adv);`
  - `utf8_append_codepoint` (function, line 143) `utf8_append_codepoint(out, cp);`
  - `utf8proc_NFC` (function, line 196) `utf8proc_NFC(reinterpret_cast<const utf8proc_uint8_t*>(utf8.c_str()));`
  - `composed` (function, line 200) `std::string composed(reinterpret_cast<char*>(nfc));`
  - `free` (function, line 201) `std::free(nfc);`
  - `utf8proc_NFD` (function, line 208) `utf8proc_NFD(reinterpret_cast<const utf8proc_uint8_t*>(utf8.c_str()));`
  - `nfd_str` (function, line 212) `std::string nfd_str(reinterpret_cast<char*>(nfd));`
  - `utf8proc_tolower` (function, line 229) `utf8proc_tolower(static_cast<utf8proc_int32_t>(cp))));`
  - `runtime_error` (function, line 371) `throw std::runtime_error( "Arabic WordPiece: basic token alignment failed at offset " + std::to_string(cursor));`
  - `chars` (function, line 389) `std::vector<char32_t> chars(wt.begin(), wt.end());`
  - `piece_u32` (function, line 397) `std::u32string piece_u32( chars.begin() + static_cast<std::ptrdiff_t>(start), chars.begin() + static_cast<std::ptrdiff_t>(end));`
  - `load_vocab_txt_stream` (function, line 623) `return load_vocab_txt_stream(in);`
  - `buf` (function, line 628) `const std::string buf(utf8);`
  - `string` (function, line 637) `std::string("\xd9\x80", 2);`
  - `g2p_bundle_file_key` (function, line 766) `g2p_bundle_file_key(onnx_bundle_key, onnx_name);`
  - `load_vocab_txt_string` (function, line 803) `ar_wp::load_vocab_txt_string(cached_vocab_txt_);`
  - `inner` (function, line 821) `std::vector<int64_t> inner(enc.input_ids.begin() + 1, enc.input_ids.end() - 1);`
  - `mask` (function, line 844) `std::vector<int64_t> mask(static_cast<size_t>(T), 1);`
- Depends on: `core/moonshine-tts/src/g2p-path.h`, `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-tts/src/ort-onnx-external-data.h`, `core/moonshine-tts/src/ort-session-options.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/arabic-diac-onnx.h
- Layer: infrastructure
- Doc: ifndef MOONSHINE_TTS_ARABIC_DIAC_ONNX_H define MOONSHINE_TTS_ARABIC_DIAC_ONNX_H  include <onnxruntime_cxx_api.h>  includ
- Language: h
- Symbols:
  - `MoonshineG2POptions` (struct, line 16)
  - `ArabicDiacOnnx` (class, line 20)
  - `model_dir` (function, line 38) `const std::filesystem::path& model_dir() const`
  - `ArabicDiacOnnx` (function, line 21) `public: explicit ArabicDiacOnnx(std::filesystem::path model_dir, bool use_cuda = false);`
  - `diacritize` (function, line 37) `std::string diacritize(std::string_view text_utf8) const;`
  - `MOONSHINE_TTS_ARABIC_DIAC_ONNX_H` (macro, line 2) `#define MOONSHINE_TTS_ARABIC_DIAC_ONNX_H`
- Imported by: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp`, `core/moonshine-tts/src/lang-specific/arabic.h`

## core/moonshine-tts/src/lang-specific/arabic-ipa.cpp
- Layer: testing
- Doc: include "arabic-ipa.h"  include "utf8-utils.h"
- Language: cpp
- Symbols:
  - `is_ar_combining` (function, line 22) `bool is_ar_combining(char32_t ch)`
  - `is_ar_base_letter` (function, line 35) `bool is_ar_base_letter(char32_t ch)`
  - `u32_nfc_u32` (function, line 52) `std::u32string u32_nfc_u32(const std::u32string& s)`
  - `strip_ar_diac_u32` (function, line 67) `std::u32string strip_ar_diac_u32(const std::u32string& s)`
  - `u32_to_utf8_str` (function, line 78) `std::string u32_to_utf8_str(const std::u32string& s)`
  - `has_vowel_mark_u32` (function, line 86) `bool has_vowel_mark_u32(const std::u32string& marks)`
  - `strip_spurious_tatweil_u32` (function, line 135) `std::u32string strip_spurious_tatweil_u32(const std::u32string& w)`
  - `apply_default_fatha_u32` (function, line 159) `std::u32string apply_default_fatha_u32(const std::u32string& w)`
  - `onset_ipa` (function, line 202) `std::string onset_ipa(char32_t base)`
  - `vowel_from_marks` (function, line 272) `std::string vowel_from_marks(const std::u32string& marks)`
  - `gem_ipa` (function, line 308) `std::string gem_ipa(const std::string& onset)`
  - `diac_word_to_ipa_u32` (function, line 319) `std::string diac_word_to_ipa_u32(const std::u32string& word)`
  - `arabic_msa_strip_diacritics_utf8` (function, line 401) `std::string arabic_msa_strip_diacritics_utf8(std::string_view utf8)`
  - `arabic_msa_apply_onnx_partial_postprocess_utf8` (function, line 406) `std::string arabic_msa_apply_onnx_partial_postprocess_utf8(
    std::string_view utf8)`
  - `arabic_msa_word_to_ipa_with_assimilation_utf8` (function, line 414) `std::string arabic_msa_word_to_ipa_with_assimilation_utf8(
    std::string_view filled_diac_utf8,...`
  - `utf8_append_codepoint` (function, line 56) `utf8_append_codepoint(u8, c);`
  - `utf8proc_NFC` (function, line 59) `utf8proc_NFC(reinterpret_cast<const utf8proc_uint8_t*>(u8.c_str()));`
  - `composed` (function, line 63) `std::string composed(reinterpret_cast<char*>(nfc));`
  - `free` (function, line 64) `std::free(nfc);`
  - `utf8_str_to_u32` (function, line 65) `return utf8_str_to_u32(composed);`
  - `string` (function, line 426) `: std::string(assimilation_prefix_source_utf8);`
- Depends on: `core/moonshine-tts/src/lang-specific/arabic-ipa.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/arabic-ipa.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_ARABIC_IPA_H define MOONSHINE_TTS_LANG_SPECIFIC_ARABIC_IPA_H  include <string> includ
- Language: h
- Symbols:
  - `arabic_msa_strip_diacritics_utf8` (function, line 8) `std::string arabic_msa_strip_diacritics_utf8(std::string_view utf8);`
  - `arabic_msa_apply_onnx_partial_postprocess_utf8` (function, line 10) `std::string arabic_msa_apply_onnx_partial_postprocess_utf8( std::string_view utf8);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_ARABIC_IPA_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_ARABIC_IPA_H`
- Imported by: `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp`, `core/moonshine-tts/src/lang-specific/arabic.cpp`

## core/moonshine-tts/src/lang-specific/arabic.cpp
- Layer: testing
- Doc: include "arabic.h"  include <algorithm> include <cctype> include <fstream> include <istream> include <sstream> include <
- Language: cpp
- Symbols:
  - `absolute_model_root_ar` (function, line 18) `std::filesystem::path absolute_model_root_ar(
    const std::filesystem::path& model_root)`
  - `has_arabic_script` (function, line 32) `bool has_arabic_script(std::string_view s)`
  - `strip_lex_ipa_segment_dots` (function, line 92) `std::string strip_lex_ipa_segment_dots(std::string ipa)`
  - `ArabicRuleG2p` (function, line 99) `ArabicRuleG2p::ArabicRuleG2p(std::filesystem::path onnx_model_dir,
                             s...`
  - `ArabicRuleG2p` (function, line 105) `ArabicRuleG2p::ArabicRuleG2p(std::filesystem::path onnx_model_dir,
                             s...`
  - `ArabicRuleG2p` (function, line 114) `ArabicRuleG2p::ArabicRuleG2p(const MoonshineG2POptions& opt,
                             std::fi...`
  - `ArabicRuleG2p` (function, line 121) `ArabicRuleG2p::ArabicRuleG2p(const MoonshineG2POptions& opt,
                             std::fi...`
  - `dialect_ids` (function, line 131) `std::vector<std::string> ArabicRuleG2p::dialect_ids()`
  - `dialect_resolves_to_arabic_rules` (function, line 136) `bool dialect_resolves_to_arabic_rules(std::string_view dialect_id)`
  - `resolve_arabic_dict_path` (function, line 145) `std::filesystem::path resolve_arabic_dict_path(
    const std::filesystem::path& model_root)`
  - `resolve_arabic_onnx_model_dir` (function, line 151) `std::filesystem::path resolve_arabic_onnx_model_dir(
    const std::filesystem::path& model_root)`
  - `g2p_word` (function, line 157) `std::string ArabicRuleG2p::g2p_word(std::string_view word_utf8)`
  - `text_to_ipa` (function, line 173) `std::string ArabicRuleG2p::text_to_ipa(std::string text,
                                       s...`
  - `absolute` (function, line 24) `std::filesystem::absolute(model_root), ec);`
  - `tmp` (function, line 34) `std::string tmp(s);`
  - `iss` (function, line 72) `std::istringstream iss(ipa_col);`
  - `in` (function, line 86) `std::ifstream in(p);`
  - `load_lex_first_tsv_stream` (function, line 90) `return load_lex_first_tsv_stream(in);`
  - `arabic_msa_apply_onnx_partial_postprocess_utf8` (function, line 170) `arabic_msa_apply_onnx_partial_postprocess_utf8(diac);`
  - `arabic_msa_word_to_ipa_with_assimilation_utf8` (function, line 171) `return arabic_msa_word_to_ipa_with_assimilation_utf8(filled, w);`
- Depends on: `core/moonshine-tts/src/g2p-path.h`, `core/moonshine-tts/src/lang-specific/arabic-ipa.h`, `core/moonshine-tts/src/lang-specific/arabic.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/arabic.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_ARABIC_H define MOONSHINE_TTS_LANG_SPECIFIC_ARABIC_H  include <filesystem> include <m
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 16)
  - `MoonshineG2POptions` (struct, line 17)
  - `ArabicRuleG2p` (class, line 21)
  - `dialect_id` (function, line 44) `const std::string& dialect_id() const`
  - `ArabicRuleG2p` (function, line 22) `public: ArabicRuleG2p(std::filesystem::path onnx_model_dir, std::filesystem::path dict_tsv, bool use_cuda = false);`
  - `dialect_ids` (function, line 38) `static std::vector<std::string> dialect_ids();`
  - `g2p_word` (function, line 51) `std::string g2p_word(std::string_view word_utf8);`
  - `dialect_resolves_to_arabic_rules` (function, line 53) `bool dialect_resolves_to_arabic_rules(std::string_view dialect_id);`
  - `resolve_arabic_dict_path` (function, line 55) `std::filesystem::path resolve_arabic_dict_path( const std::filesystem::path& model_root);`
  - `resolve_arabic_onnx_model_dir` (function, line 58) `std::filesystem::path resolve_arabic_onnx_model_dir( const std::filesystem::path& model_root);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_ARABIC_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_ARABIC_H`
- Depends on: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.h`, `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/arabic.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/arabic-rule-g2p-test.cpp`, `core/moonshine-tts/tools/arabic-rule-g2p-cli.cpp`

## core/moonshine-tts/src/lang-specific/chinese-numbers.cpp
- Layer: testing
- Doc: include "chinese-numbers.h"  include <cstdint> include <limits> include <stdexcept> include <string> include <string_vie
- Language: cpp
- Symbols:
  - `digit_cp` (function, line 16) `char32_t digit_cp(unsigned d)`
  - `cn_digit` (function, line 26) `std::string cn_digit(unsigned d)`
  - `ends_with_ling_utf8` (function, line 32) `bool ends_with_ling_utf8(const std::string& s)`
  - `section_under_10000` (function, line 40) `std::string section_under_10000(unsigned n)`
  - `int_to_han_u64` (function, line 95) `std::string int_to_han_u64(std::uint64_t n)`
  - `ascii_digit_string` (function, line 145) `bool ascii_digit_string(std::string_view t, std::uint64_t& out_val)`
  - `int_to_mandarin_cardinal_han` (function, line 165) `std::string int_to_mandarin_cardinal_han(std::uint64_t n)`
  - `arabic_numeral_token_to_han` (function, line 169) `std::optional<std::string> arabic_numeral_token_to_han(
    std::string_view token_sv)`
  - `utf8_append_codepoint` (function, line 29) `utf8_append_codepoint(o, digit_cp(d));`
  - `logic_error` (function, line 43) `throw std::logic_error("section_under_10000");`
  - `gs` (function, line 116) `std::vector<unsigned> gs(low_first.rbegin(), low_first.rend());`
  - `token` (function, line 172) `std::string token(trim_ascii_ws_copy(token_sv));`
- Depends on: `core/moonshine-tts/src/lang-specific/chinese-numbers.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/chinese-numbers.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_CHINESE_NUMBERS_H define MOONSHINE_TTS_LANG_SPECIFIC_CHINESE_NUMBERS_H  include <cstd
- Language: h
- Symbols:
  - `int_to_mandarin_cardinal_han` (function, line 12) `std::string int_to_mandarin_cardinal_han(std::uint64_t n);`
  - `arabic_numeral_token_to_han` (function, line 16) `std::optional<std::string> arabic_numeral_token_to_han(std::string_view token);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_CHINESE_NUMBERS_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_CHINESE_NUMBERS_H`
- Imported by: `core/moonshine-tts/src/lang-specific/chinese-numbers.cpp`, `core/moonshine-tts/src/lang-specific/chinese.cpp`

## core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp
- Layer: testing
- Doc: include "chinese-onnx-g2p.h"  include <utility>  include "g2p-word-log.h" include "moonshine-g2p-options.h" include "utf
- Language: cpp
- Symbols:
  - `utf8_nfc_utf8proc` (function, line 15) `std::string utf8_nfc_utf8proc(std::string_view s)`
  - `ChineseOnnxG2p` (function, line 29) `ChineseOnnxG2p::ChineseOnnxG2p(std::filesystem::path model_dir,
                               st...`
  - `ChineseOnnxG2p` (function, line 33) `ChineseOnnxG2p::ChineseOnnxG2p(std::filesystem::path model_dir,
                               st...`
  - `ChineseOnnxG2p` (function, line 37) `ChineseOnnxG2p::ChineseOnnxG2p(const MoonshineG2POptions& opt,
                               std...`
  - `ChineseOnnxG2p` (function, line 43) `ChineseOnnxG2p::ChineseOnnxG2p(const MoonshineG2POptions& opt,
                               std...`
  - `text_to_ipa` (function, line 49) `std::string ChineseOnnxG2p::text_to_ipa(std::string text_utf8,
                                  ...`
  - `ChineseOnnxRuleG2p` (function, line 75) `ChineseOnnxRuleG2p::ChineseOnnxRuleG2p(std::filesystem::path onnx_model_dir,
                    ...`
  - `ChineseOnnxRuleG2p` (function, line 81) `ChineseOnnxRuleG2p::ChineseOnnxRuleG2p(std::filesystem::path onnx_model_dir,
                    ...`
  - `ChineseOnnxRuleG2p` (function, line 86) `ChineseOnnxRuleG2p::ChineseOnnxRuleG2p(const MoonshineG2POptions& opt,
                          ...`
  - `ChineseOnnxRuleG2p` (function, line 93) `ChineseOnnxRuleG2p::ChineseOnnxRuleG2p(const MoonshineG2POptions& opt,
                          ...`
  - `text_to_ipa` (function, line 100) `std::string ChineseOnnxRuleG2p::text_to_ipa(
    std::string text, std::vector<G2pWordLog>* per_w...`
  - `tmp` (function, line 17) `const std::string tmp(s);`
  - `utf8proc_NFC` (function, line 19) `utf8proc_NFC(reinterpret_cast<const utf8proc_uint8_t*>(tmp.c_str()));`
  - `string` (function, line 21) `return std::string(s);`
  - `out` (function, line 23) `std::string out(reinterpret_cast<char*>(p));`
  - `free` (function, line 24) `std::free(p);`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_CHINESE_ONNX_G2P_H define MOONSHINE_TTS_CHINESE_ONNX_G2P_H  include <filesystem> include <memory> i
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 15)
  - `MoonshineG2POptions` (struct, line 16)
  - `ChineseOnnxG2p` (class, line 20)
  - `ChineseOnnxRuleG2p` (class, line 46)
  - `tok` (function, line 36) `const ChineseTokPosOnnx& tok() const`
  - `ChineseOnnxG2p` (function, line 21) `public: explicit ChineseOnnxG2p(std::filesystem::path model_dir, std::filesystem::path dict_tsv, bool use_cuda = false);`
  - `text_to_ipa` (function, line 33) `std::string text_to_ipa(std::string text_utf8, std::vector<G2pWordLog>* per_word_log = nullptr);`
  - `ChineseOnnxRuleG2p` (function, line 47) `public: explicit ChineseOnnxRuleG2p(std::filesystem::path onnx_model_dir, std::filesystem::path dict_tsv, bool use_cuda = false);`
  - `MOONSHINE_TTS_CHINESE_ONNX_G2P_H` (macro, line 2) `#define MOONSHINE_TTS_CHINESE_ONNX_G2P_H`
- Depends on: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.h`, `core/moonshine-tts/src/lang-specific/chinese.h`, `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/chinese-rule-g2p-test.cpp`, `core/moonshine-tts/tools/chinese-rule-g2p-cli.cpp`

## core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp
- Layer: testing
- Doc: include "chinese-tok-pos-onnx.h"  include <nlohmann/json.h>  include <algorithm> include <array> include <cctype> includ
- Language: cpp
- Symbols:
  - `BasicTokCfg` (struct, line 311)
  - `EncodedWp` (struct, line 435)
  - `Idx` (struct, line 525)
  - `open_session` (function, line 30) `std::unique_ptr<Ort::Session> open_session(
    Ort::Env& env, const std::filesystem::path& model...`
  - `open_session_memory` (function, line 47) `std::unique_ptr<Ort::Session> open_session_memory(
    Ort::Env& env, const void* data, size_t le...`
  - `slurp_utf8_file` (function, line 61) `std::string slurp_utf8_file(const std::filesystem::path& p)`
  - `bundle_load_utf8` (function, line 71) `bool bundle_load_utf8(const MoonshineG2POptions* opt,
                      std::string_view bund...`
  - `bundle_load_binary` (function, line 89) `bool bundle_load_binary(const MoonshineG2POptions* opt,
                        std::string_view ...`
  - `utf8_to_u32` (function, line 122) `std::u32string utf8_to_u32(std::string_view utf8)`
  - `u32_to_utf8` (function, line 135) `std::string u32_to_utf8(const std::u32string& s)`
  - `is_space_u32` (function, line 143) `bool is_space_u32(char32_t c)`
  - `is_control_u32` (function, line 152) `bool is_control_u32(char32_t c)`
  - `is_punctuation_u32` (function, line 161) `bool is_punctuation_u32(char32_t c)`
  - `is_punct_char_word_group_u32` (function, line 175) `bool is_punct_char_word_group_u32(char32_t c)`
  - `is_chinese_char` (function, line 179) `bool is_chinese_char(std::uint32_t cp)`
  - `u32_nfc` (function, line 188) `std::u32string u32_nfc(const std::u32string& s)`
  - `strip_mn_nfd` (function, line 200) `std::u32string strip_mn_nfd(const std::u32string& s)`
  - `to_lower_u32` (function, line 220) `std::u32string to_lower_u32(const std::u32string& s)`
  - `clean_text_u32` (function, line 229) `std::u32string clean_text_u32(const std::u32string& text)`
  - `tokenize_chinese_chars_u32` (function, line 241) `std::u32string tokenize_chinese_chars_u32(const std::u32string& text)`
  - `split_u32_whitespace` (function, line 255) `std::vector<std::u32string> split_u32_whitespace(std::u32string_view s)`
  - `run_split_on_punc_u32` (function, line 280) `std::vector<std::u32string> run_split_on_punc_u32(const std::u32string& text)`
  - `normalization_ref_u32` (function, line 316) `std::u32string normalization_ref_u32(const std::u32string& text_u32,
                            ...`
  - `basic_tokenize_u32` (function, line 337) `std::vector<std::u32string> basic_tokenize_u32(
    const std::u32string& original_text_u32, cons...`
  - `align_basic_tokens_u32` (function, line 369) `void align_basic_tokens_u32(const std::u32string& ref,
                            const std::vec...`
  - `wordpiece_tokenize_u32` (function, line 386) `std::vector<std::u32string> wordpiece_tokenize_u32(
    const std::u32string& token,
    const st...`
  - `encode_bert_wordpiece` (function, line 441) `EncodedWp encode_bert_wordpiece(
    const std::u32string& text_u32,
    const std::unordered_map...`
  - `cjk_tokpos_preferred_chunk_break_cp` (function, line 631) `bool cjk_tokpos_preferred_chunk_break_cp(char32_t c)`
  - `cjk_tokpos_chunk_exclusive_end` (function, line 664) `template <typename EncodeFn>
std::size_t cjk_tokpos_chunk_exclusive_end(const std::u32string& ful...`
  - `default_chinese_tok_pos_model_dir` (function, line 703) `std::filesystem::path default_chinese_tok_pos_model_dir(
    const std::filesystem::path& g2p_dat...`
  - `ChineseTokPosOnnx` (function, line 713) `ChineseTokPosOnnx::ChineseTokPosOnnx(const MoonshineG2POptions* opt,
                            ...`
  - `format_annotated_line` (function, line 774) `std::string ChineseTokPosOnnx::format_annotated_line(
    const std::vector<std::pair<std::string...`
  - `make_g2p_ort_session_options` (function, line 39) `make_g2p_ort_session_options(ort_providers, coreml_cache_dir));`
  - `ort_add_external_initializer_files_for_onnx_model_buffer` (function, line 56) `ort_add_external_initializer_files_for_onnx_model_buffer(so, opt->files, model_map_key);`
  - `in` (function, line 63) `std::ifstream in(p, std::ios::binary);`
  - `utf8_decode_at` (function, line 129) `utf8_decode_at(std::string(utf8), i, cp, adv);`
  - `utf8_append_codepoint` (function, line 139) `utf8_append_codepoint(out, cp);`
  - `utf8proc_NFC` (function, line 192) `utf8proc_NFC(reinterpret_cast<const utf8proc_uint8_t*>(utf8.c_str()));`
  - `composed` (function, line 196) `std::string composed(reinterpret_cast<char*>(nfc));`
  - `free` (function, line 197) `std::free(nfc);`
  - `utf8proc_NFD` (function, line 204) `utf8proc_NFD(reinterpret_cast<const utf8proc_uint8_t*>(utf8.c_str()));`
  - `nfd_str` (function, line 208) `std::string nfd_str(reinterpret_cast<char*>(nfd));`
  - `utf8proc_tolower` (function, line 225) `utf8proc_tolower(static_cast<utf8proc_int32_t>(cp))));`
  - `runtime_error` (function, line 379) `throw std::runtime_error( "Chinese WordPiece: basic token alignment failed at offset " + std::to_string(cursor));`
  - `chars` (function, line 397) `std::vector<char32_t> chars(wt.begin(), wt.end());`
  - `piece_u32` (function, line 405) `std::u32string piece_u32( chars.begin() + static_cast<std::ptrdiff_t>(start), chars.begin() + static_cast<std::ptrdiff_t>(end));`
  - `buf` (function, line 627) `const std::string buf(utf8);`
  - `load_vocab_txt_stream` (function, line 629) `return load_vocab_txt_stream(in);`
  - `g2p_bundle_file_key` (function, line 756) `g2p_bundle_file_key(onnx_bundle_key, onnx_name);`
  - `load_vocab_txt_string` (function, line 798) `load_vocab_txt_string(cached_vocab_txt_);`
  - `mask` (function, line 831) `std::vector<int64_t> mask(static_cast<size_t>(T), 1);`
  - `flush` (function, line 885) `flush();`
- Depends on: `core/moonshine-tts/src/g2p-path.h`, `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-tts/src/ort-onnx-external-data.h`, `core/moonshine-tts/src/ort-session-options.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_CHINESE_TOK_POS_ONNX_H define MOONSHINE_TTS_CHINESE_TOK_POS_ONNX_H  include <onnxruntime_cxx_api.h>
- Language: h
- Symbols:
  - `MoonshineG2POptions` (struct, line 16)
  - `ChineseTokPosOnnx` (class, line 22)
  - `model_dir` (function, line 41) `const std::filesystem::path& model_dir() const`
  - `ChineseTokPosOnnx` (function, line 23) `public: explicit ChineseTokPosOnnx(std::filesystem::path model_dir, bool use_cuda = false);`
  - `format_annotated_line` (function, line 39) `static std::string format_annotated_line( const std::vector<std::pair<std::string, std::string>>& pairs);`
  - `default_chinese_tok_pos_model_dir` (function, line 60) `std::filesystem::path default_chinese_tok_pos_model_dir( const std::filesystem::path& g2p_data_root);`
  - `MOONSHINE_TTS_CHINESE_TOK_POS_ONNX_H` (macro, line 2) `#define MOONSHINE_TTS_CHINESE_TOK_POS_ONNX_H`
- Imported by: `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h`, `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp`, `core/moonshine-tts/tests/chinese-tok-pos-onnx-test.cpp`

## core/moonshine-tts/src/lang-specific/chinese.cpp
- Layer: testing
- Doc: include "chinese.h"  include <cctype> include <cstdint> include <fstream> include <istream> include <sstream> include <s
- Language: cpp
- Symbols:
  - `trim_copy_line` (function, line 22) `std::string trim_copy_line(std::string_view s)`
  - `is_cjk_cp` (function, line 36) `bool is_cjk_cp(char32_t cp)`
  - `is_ascii_digit_cp` (function, line 43) `bool is_ascii_digit_cp(char32_t cp)`
  - `is_fullwidth_digit_cp` (function, line 45) `bool is_fullwidth_digit_cp(char32_t cp)`
  - `token_has_g2p_content` (function, line 49) `bool token_has_g2p_content(const std::string& tok)`
  - `pos_in_set` (function, line 67) `bool pos_in_set(std::string_view p, const std::unordered_set<std::string>& s)`
  - `skip_phonetic_pos` (function, line 71) `const std::unordered_set<std::string>& skip_phonetic_pos()`
  - `verb_like_pos` (function, line 77) `const std::unordered_set<std::string>& verb_like_pos()`
  - `noun_like_pos` (function, line 84) `const std::unordered_set<std::string>& noun_like_pos()`
  - `ipa_contains` (function, line 91) `bool ipa_contains(const std::string& ipa, std::string_view sub)`
  - `try_consume_g2p_token` (function, line 95) `bool try_consume_g2p_token(const std::string& text, size_t pos,
                           size_t...`
  - `load_chinese_lexicon_stream` (function, line 190) `void load_chinese_lexicon_stream(
    std::istream& in,
    std::unordered_map<std::string, std::...`
  - `ChineseRuleG2p` (function, line 214) `ChineseRuleG2p::ChineseRuleG2p(std::filesystem::path dict_tsv)`
  - `ChineseRuleG2p` (function, line 231) `ChineseRuleG2p::ChineseRuleG2p(std::string dict_tsv_utf8)`
  - `disambiguate_heteronym` (function, line 239) `std::string ChineseRuleG2p::disambiguate_heteronym(
    std::string_view word, std::string_view p...`
  - `han_reading_to_ipa` (function, line 400) `std::string ChineseRuleG2p::han_reading_to_ipa(std::string_view han) const`
  - `char_fallback_ipa` (function, line 425) `std::string ChineseRuleG2p::char_fallback_ipa(std::string_view word) const`
  - `g2p_word_impl` (function, line 440) `std::string ChineseRuleG2p::g2p_word_impl(std::string_view word,
                                ...`
  - `word_to_ipa` (function, line 487) `std::string ChineseRuleG2p::word_to_ipa(std::string_view word) const`
  - `word_to_ipa_with_pos` (function, line 491) `std::string ChineseRuleG2p::word_to_ipa_with_pos(std::string_view word,
                         ...`
  - `text_to_ipa` (function, line 496) `std::string ChineseRuleG2p::text_to_ipa(std::string text,
                                       ...`
  - `dialect_resolves_to_chinese_rules` (function, line 546) `bool dialect_resolves_to_chinese_rules(std::string_view dialect_id)`
  - `dialect_ids` (function, line 555) `std::vector<std::string> ChineseRuleG2p::dialect_ids()`
  - `resolve_chinese_dict_path` (function, line 560) `std::filesystem::path resolve_chinese_dict_path(
    const std::filesystem::path& model_root)`
  - `resolve_chinese_onnx_model_dir` (function, line 565) `std::filesystem::path resolve_chinese_onnx_model_dir(
    const std::filesystem::path& model_root)`
  - `string` (function, line 34) `return std::string(s.substr(a, b - a));`
  - `utf8_decode_at` (function, line 119) `utf8_decode_at(text, p, cp, adv);`
  - `runtime_error` (function, line 217) `throw std::runtime_error("Chinese G2P: lexicon not found: " + dict_tsv.generic_string());`
  - `in` (function, line 220) `std::ifstream in(dict_tsv);`
  - `w` (function, line 249) `const std::string w(word);`
  - `p` (function, line 250) `const std::string p(pos);`
  - `h` (function, line 402) `const std::string h(han);`
  - `utf8_append_codepoint` (function, line 411) `utf8_append_codepoint(ch, cp);`
- Depends on: `core/moonshine-tts/src/g2p-path.h`, `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/chinese-numbers.h`, `core/moonshine-tts/src/lang-specific/chinese.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/chinese.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_CHINESE_H define MOONSHINE_TTS_LANG_SPECIFIC_CHINESE_H  include <filesystem> include 
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 14)
  - `ChineseRuleG2p` (class, line 23)
  - `dialect_id` (function, line 29) `const std::string& dialect_id() const`
  - `ChineseRuleG2p` (function, line 24) `public: explicit ChineseRuleG2p(std::filesystem::path dict_tsv);`
  - `dialect_ids` (function, line 27) `static std::vector<std::string> dialect_ids();`
  - `word_to_ipa` (function, line 34) `std::string word_to_ipa(std::string_view word) const;`
  - `word_to_ipa_with_pos` (function, line 38) `std::string word_to_ipa_with_pos(std::string_view word, std::string_view pos) const;`
  - `han_reading_to_ipa` (function, line 48) `std::string han_reading_to_ipa(std::string_view han) const;`
  - `char_fallback_ipa` (function, line 50) `std::string char_fallback_ipa(std::string_view word) const;`
  - `disambiguate_heteronym` (function, line 51) `std::string disambiguate_heteronym( std::string_view word, std::string_view pos, const std::vector<std::string>& readings) const;`
  - `g2p_word_impl` (function, line 54) `std::string g2p_word_impl(std::string_view word, std::string_view pos) const;`
  - `dialect_resolves_to_chinese_rules` (function, line 56) `bool dialect_resolves_to_chinese_rules(std::string_view dialect_id);`
  - `resolve_chinese_dict_path` (function, line 60) `std::filesystem::path resolve_chinese_dict_path( const std::filesystem::path& model_root);`
  - `resolve_chinese_onnx_model_dir` (function, line 65) `std::filesystem::path resolve_chinese_onnx_model_dir( const std::filesystem::path& model_root);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_CHINESE_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_CHINESE_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h`, `core/moonshine-tts/src/lang-specific/chinese.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/chinese-rule-g2p-test.cpp`

## core/moonshine-tts/src/lang-specific/cmudict-tsv.cpp
- Layer: infrastructure
- Doc: include "cmudict-tsv.h"  include <fstream> include <istream> include <set> include <sstream>  include "text-normalize.h"
- Language: cpp
- Symbols:
  - `parse_cmudict_tsv_lines` (function, line 13) `void parse_cmudict_tsv_lines(
    std::istream& in,
    std::unordered_map<std::string, std::vect...`
  - `CmudictTsv` (function, line 57) `CmudictTsv::CmudictTsv(const std::filesystem::path& path)`
  - `CmudictTsv` (function, line 65) `CmudictTsv::CmudictTsv(std::string_view utf8_contents)`
  - `lookup` (function, line 71) `const std::vector<std::string>* CmudictTsv::lookup(std::string_view key) const`
  - `in` (function, line 59) `std::ifstream in(path);`
  - `runtime_error` (function, line 61) `throw std::runtime_error("failed to open dictionary: " + path.string());`
  - `buf` (function, line 67) `const std::string buf(utf8_contents);`
  - `k` (function, line 73) `const std::string k(key.begin(), key.end());`
- Depends on: `core/moonshine-tts/src/lang-specific/cmudict-tsv.h`, `core/moonshine-tts/src/text-normalize.h`

## core/moonshine-tts/src/lang-specific/cmudict-tsv.h
- Layer: infrastructure
- Doc: ifndef MOONSHINE_TTS_CMUDICT_TSV_H define MOONSHINE_TTS_CMUDICT_TSV_H  include <filesystem> include <string> include <st
- Language: h
- Symbols:
  - `CmudictTsv` (class, line 14)
  - `CmudictTsv` (function, line 15) `public: explicit CmudictTsv(const std::filesystem::path& path);`
  - `lookup` (function, line 18) `const std::vector<std::string>* lookup(std::string_view key) const;`
  - `MOONSHINE_TTS_CMUDICT_TSV_H` (macro, line 2) `#define MOONSHINE_TTS_CMUDICT_TSV_H`
- Imported by: `core/moonshine-tts/src/lang-specific/cmudict-tsv.cpp`, `core/moonshine-tts/src/lang-specific/english.cpp`, `core/moonshine-tts/tests/cmudict-tsv-test.cpp`

## core/moonshine-tts/src/lang-specific/dutch.cpp
- Layer: testing
- Doc: include "dutch.h"  include <algorithm> include <array> include <cctype> include <cstdint> include <cstring> include <fst
- Language: cpp
- Symbols:
  - `Slot` (struct, line 626)
  - `dutch_unicode_tolower_cp` (function, line 30) `char32_t dutch_unicode_tolower_cp(char32_t c)`
  - `append_lexicon_folded` (function, line 102) `void append_lexicon_folded(std::string& out, char32_t cl)`
  - `normalize_lexicon_key_utf8` (function, line 159) `std::string normalize_lexicon_key_utf8(const std::string& word)`
  - `is_grapheme_char` (function, line 177) `bool is_grapheme_char(char32_t cl)`
  - `normalize_grapheme_key_u32` (function, line 189) `std::u32string normalize_grapheme_key_u32(const std::string& word)`
  - `kTeenWord` (function, line 211) `static const char* kTeenWord(int n)`
  - `join_unit_tens` (function, line 220) `std::string join_unit_tens(int u, std::string_view tens_word)`
  - `below_100` (function, line 236) `std::string below_100(int n)`
  - `below_1000_spaced` (function, line 255) `std::string below_1000_spaced(int n)`
  - `from_1000_to_9999` (function, line 277) `std::string from_1000_to_9999(int n)`
  - `fix_thousands_compound` (function, line 309) `std::string fix_thousands_compound(int q)`
  - `below_1_000_000_v2` (function, line 322) `std::string below_1_000_000_v2(int n)`
  - `expand_cardinal_digits_to_dutch_words` (function, line 338) `std::string expand_cardinal_digits_to_dutch_words(std::string_view sv)`
  - `is_ascii_digit` (function, line 370) `bool is_ascii_digit(char c)`
  - `is_latin1_supplement_python_word_char` (function, line 372) `bool is_latin1_supplement_python_word_char(char32_t cp)`
  - `is_letterlike_math_word_char` (function, line 402) `bool is_letterlike_math_word_char(char32_t cp)`
  - `is_dutch_word_char` (function, line 407) `bool is_dutch_word_char(char32_t cp)`
  - `prev_utf8_index` (function, line 436) `size_t prev_utf8_index(const std::string& t, size_t byte_i)`
  - `word_boundary_before` (function, line 447) `bool word_boundary_before(const std::string& t, size_t byte_i)`
  - `word_boundary_after` (function, line 458) `bool word_boundary_after(const std::string& t, size_t byte_i)`
  - `expand_digit_tokens_in_text` (function, line 468) `std::string expand_digit_tokens_in_text(std::string_view text_sv)`
  - `digit_pass_through_pattern` (function, line 519) `bool digit_pass_through_pattern(std::string_view raw)`
  - `all_ascii_digits_string` (function, line 543) `bool all_ascii_digits_string(const std::string& s)`
  - `apply_lexicon_ipa_postprocess` (function, line 555) `std::string apply_lexicon_ipa_postprocess(std::string ipa,
                                      ...`
  - `load_dutch_lexicon_stream` (function, line 623) `void load_dutch_lexicon_stream(
    std::istream& in, std::unordered_map<std::string, std::string...`
  - `load_dutch_lexicon_file` (function, line 677) `void load_dutch_lexicon_file(
    const std::filesystem::path& path,
    std::unordered_map<std::...`
  - `is_vowel_letter32` (function, line 688) `bool is_vowel_letter32(char32_t c)`
  - `strip_to_plain_vowel` (function, line 698) `char32_t strip_to_plain_vowel(char32_t c)`
  - `word_has_written_stress_u32` (function, line 722) `bool word_has_written_stress_u32(const std::u32string& w)`
  - `stressed_syllable_from_acute` (function, line 731) `std::optional<size_t> stressed_syllable_from_acute(
    const std::vector<std::u32string>& syllab...`
  - `dutch_orthographic_syllables_u32` (function, line 792) `std::vector<std::u32string> dutch_orthographic_syllables_u32(
    const std::u32string& word)`
  - `remove_if` (function, line 851) `std::remove_if(syllables.begin(), syllables.end(),
                     [](const std::u32string& sy)`
  - `unstressed_prefix_len_u32` (function, line 856) `size_t unstressed_prefix_len_u32(const std::u32string& wl)`
  - `default_stress_syllable_index` (function, line 870) `size_t default_stress_syllable_index(const std::vector<std::u32string>& syls,
                   ...`
  - `insert_primary_stress_before_vowel_dutch` (function, line 915) `std::string insert_primary_stress_before_vowel_dutch(std::string s)`
  - `ipa_starts_with_nucleus_dutch` (function, line 958) `bool ipa_starts_with_nucleus_dutch(std::string_view rest)`
  - `ipa_at_stress_mark_dutch` (function, line 997) `bool ipa_at_stress_mark_dutch(const std::string& ipa, size_t j)`
  - `ipa_skip_pre_nucleus_dutch` (function, line 1006) `size_t ipa_skip_pre_nucleus_dutch(std::string_view s, size_t j)`
  - `final_devoice_obstruents` (function, line 1044) `std::string final_devoice_obstruents(std::string ipa)`
  - `letters_to_ipa_no_stress` (function, line 1082) `std::string letters_to_ipa_no_stress(const std::u32string& syl_in,
                              ...`
  - `strip_hyphens_u32` (function, line 1415) `std::u32string strip_hyphens_u32(const std::u32string& w)`
  - `rules_word_to_ipa_utf8` (function, line 1425) `std::string rules_word_to_ipa_utf8(const std::string& raw_word,
                                 ...`
  - `resolve_dutch_dict_path` (function, line 1457) `std::filesystem::path resolve_dutch_dict_path(
    const std::filesystem::path& model_root)`
  - `dialect_resolves_to_dutch_rules` (function, line 1462) `bool dialect_resolves_to_dutch_rules(std::string_view dialect_id)`
  - `dialect_ids` (function, line 1470) `std::vector<std::string> DutchRuleG2p::dialect_ids()`
  - `normalize_ipa_stress_for_vocoder` (function, line 1474) `std::string DutchRuleG2p::normalize_ipa_stress_for_vocoder(std::string ipa)`
  - `DutchRuleG2p` (function, line 1521) `DutchRuleG2p::DutchRuleG2p(std::filesystem::path dict_tsv, Options options)
    : options_(options)`
  - `DutchRuleG2p` (function, line 1526) `DutchRuleG2p::DutchRuleG2p(std::string dict_tsv_utf8, Options options)
    : options_(options)`
  - `finalize_ipa` (function, line 1532) `std::string DutchRuleG2p::finalize_ipa(std::string ipa,
                                       bo...`
  - `lookup_or_rules` (function, line 1545) `std::string DutchRuleG2p::lookup_or_rules(const std::string& raw_word) const`
  - `word_to_ipa` (function, line 1601) `std::string DutchRuleG2p::word_to_ipa(const std::string& word) const`
  - `text_to_ipa_no_expand` (function, line 1622) `std::string DutchRuleG2p::text_to_ipa_no_expand(
    const std::string& text, std::vector<G2pWord...`
  - `text_to_ipa` (function, line 1698) `std::string DutchRuleG2p::text_to_ipa(std::string text,
                                      std...`
  - `utf8_append_codepoint` (function, line 108) `utf8_append_codepoint(out, cl);`
  - `utf8_decode_at` (function, line 166) `utf8_decode_at(word, i, cp, adv);`
  - `string` (function, line 223) `return std::string(tens_word);`
  - `out_of_range` (function, line 239) `throw std::out_of_range("below_100");`
  - `s` (function, line 340) `std::string s(sv);`
  - `binary_search` (function, line 404) `return std::binary_search(kLetterlikeWordChars.begin(), kLetterlikeWordChars.end(), cp);`
  - `text` (function, line 470) `std::string text(text_sv);`
  - `trim_ascii_ws_copy` (function, line 641) `trim_ascii_ws_copy(std::string_view(line).substr(0, tab));`
  - `in` (function, line 681) `std::ifstream in(path);`
  - `runtime_error` (function, line 683) `throw std::runtime_error("Dutch lexicon: cannot open " + path.generic_string());`
  - `min` (function, line 909) `return std::min(idx + 1, n - 1);`
  - `erase_utf8_substr` (function, line 917) `erase_utf8_substr(s, kPrimaryStressUtf8);`
  - `append` (function, line 1104) `append("sx");`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/dutch.h`, `core/moonshine-tts/src/lang-specific/ipa-symbols.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/dutch.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_DUTCH_H define MOONSHINE_TTS_LANG_SPECIFIC_DUTCH_H  include <filesystem> include <str
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 14)
  - `Options` (struct, line 20)
  - `DutchRuleG2p` (class, line 18)
  - `dialect_id` (function, line 37) `const std::string& dialect_id() const`
  - `DutchRuleG2p` (function, line 29) `explicit DutchRuleG2p(std::filesystem::path dict_tsv);`
  - `dialect_ids` (function, line 35) `static std::vector<std::string> dialect_ids();`
  - `word_to_ipa` (function, line 39) `std::string word_to_ipa(const std::string& word) const;`
  - `normalize_ipa_stress_for_vocoder` (function, line 48) `static std::string normalize_ipa_stress_for_vocoder(std::string ipa);`
  - `lookup_or_rules` (function, line 54) `std::string lookup_or_rules(const std::string& raw_word) const;`
  - `finalize_ipa` (function, line 56) `std::string finalize_ipa(std::string ipa, bool from_lexicon) const;`
  - `text_to_ipa_no_expand` (function, line 57) `std::string text_to_ipa_no_expand( const std::string& text, std::vector<G2pWordLog>* per_word_log) const;`
  - `dialect_resolves_to_dutch_rules` (function, line 62) `bool dialect_resolves_to_dutch_rules(std::string_view dialect_id);`
  - `resolve_dutch_dict_path` (function, line 66) `std::filesystem::path resolve_dutch_dict_path( const std::filesystem::path& model_root);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_DUTCH_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_DUTCH_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/dutch.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp`, `core/moonshine-tts/tools/dutch-g2p-batch-cli.cpp`, `core/moonshine-tts/tools/dutch-rule-g2p-cli.cpp`

## core/moonshine-tts/src/lang-specific/english-hand-oov.cpp
- Layer: testing
- Doc: include "english-hand-oov.h"  include <cctype> include <cstring> include <string> include <string_view> include <unorder
- Language: cpp
- Symbols:
  - `Literal` (struct, line 124)
  - `utf8_starts_with` (function, line 18) `bool utf8_starts_with(const std::string& s, std::string_view p)`
  - `last_utf8_char` (function, line 22) `std::string_view last_utf8_char(std::string_view s)`
  - `last_ipa_unit_is_vowel` (function, line 37) `bool last_ipa_unit_is_vowel(std::string_view prev)`
  - `is_vowel` (function, line 49) `constexpr bool is_vowel(char c)`
  - `is_consonant` (function, line 53) `constexpr bool is_consonant(char c)`
  - `next_vowel_index` (function, line 57) `int next_vowel_index(std::string_view w, int start)`
  - `magic_e_lengthens` (function, line 66) `bool magic_e_lengthens(std::string_view w, int vowel_i)`
  - `th_voiced_word` (function, line 156) `bool th_voiced_word(std::string_view w)`
  - `oov_single_consonant` (function, line 162) `std::string oov_single_consonant(char c, std::string_view w, int i)`
  - `add_primary_stress_if_missing` (function, line 319) `std::string add_primary_stress_if_missing(std::string s)`
  - `oov_grapheme_to_ipa` (function, line 340) `std::string oov_grapheme_to_ipa(std::string_view word)`
  - `english_hand_oov_rules_ipa` (function, line 437) `std::string english_hand_oov_rules_ipa(std::string_view word)`
  - `string` (function, line 230) `default: return std::string(1, c);`
  - `p` (function, line 329) `const std::string_view p(pref);`
- Depends on: `core/moonshine-tts/src/lang-specific/english-hand-oov.h`, `core/moonshine-tts/src/text-normalize.h`

## core/moonshine-tts/src/lang-specific/english-hand-oov.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_ENGLISH_HAND_OOV_H define MOONSHINE_TTS_LANG_SPECIFIC_ENGLISH_HAND_OOV_H  include <st
- Language: h
- Symbols:
  - `english_hand_oov_rules_ipa` (function, line 11) `std::string english_hand_oov_rules_ipa(std::string_view word);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_ENGLISH_HAND_OOV_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_ENGLISH_HAND_OOV_H`
- Imported by: `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp`, `core/moonshine-tts/src/lang-specific/english.cpp`, `core/moonshine-tts/tests/english-hand-oov-test.cpp`

## core/moonshine-tts/src/lang-specific/english-numbers.cpp
- Layer: testing
- Doc: include "english-numbers.h"  include <algorithm> include <cctype> include <string> include <vector>
- Language: cpp
- Symbols:
  - `Scale` (struct, line 74)
  - `digit_sequence_ipa` (function, line 21) `std::string digit_sequence_ipa(std::string_view digits)`
  - `under_100_ipa` (function, line 34) `std::string under_100_ipa(int n)`
  - `under_1000_ipa` (function, line 50) `std::string under_1000_ipa(int n)`
  - `cardinal_non_negative_ipa` (function, line 63) `std::optional<std::string> cardinal_non_negative_ipa(long long n)`
  - `integer_decimal_string_ipa` (function, line 106) `std::optional<std::string> integer_decimal_string_ipa(std::string s)`
  - `english_number_token_ipa` (function, line 199) `std::optional<std::string> english_number_token_ipa(std::string_view token)`
  - `string` (function, line 69) `return std::string("ˈzɪroʊ");`
  - `strip_sep` (function, line 119) `strip_sep(s);`
  - `prefix_neg` (function, line 178) `return prefix_neg(std::move(left));`
  - `isdigit` (function, line 183) `return std::isdigit(static_cast<unsigned char>(c));`
  - `t` (function, line 201) `std::string t(token.begin(), token.end());`
- Depends on: `core/moonshine-tts/src/lang-specific/english-numbers.h`

## core/moonshine-tts/src/lang-specific/english-numbers.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_ENGLISH_NUMBERS_H define MOONSHINE_TTS_LANG_SPECIFIC_ENGLISH_NUMBERS_H  include <opti
- Language: h
- Symbols:
  - `english_number_token_ipa` (function, line 12) `std::optional<std::string> english_number_token_ipa(std::string_view token);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_ENGLISH_NUMBERS_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_ENGLISH_NUMBERS_H`
- Imported by: `core/moonshine-tts/src/lang-specific/english-numbers.cpp`, `core/moonshine-tts/src/lang-specific/english.cpp`, `core/moonshine-tts/tests/english-hand-oov-test.cpp`

## core/moonshine-tts/src/lang-specific/english.cpp
- Layer: testing
- Doc: include "english.h"  include <nlohmann/json.h>  include <algorithm> include <cctype> include <filesystem> include <optio
- Language: cpp
- Symbols:
  - `append_log` (function, line 30) `void append_log(std::vector<G2pWordLog>* out, G2pWordLog entry)`
  - `pick_english_heteronym_ipa` (function, line 40) `std::string pick_english_heteronym_ipa(std::vector<std::string> alts,
                           ...`
  - `EnglishRuleG2p` (function, line 81) `EnglishRuleG2p::EnglishRuleG2p(
    std::filesystem::path dict_tsv,
    std::optional<std::filesy...`
  - `EnglishRuleG2p` (function, line 109) `EnglishRuleG2p::EnglishRuleG2p(
    std::string dict_tsv_utf8, std::optional<std::filesystem::pat...`
  - `dialect_ids` (function, line 139) `std::vector<std::string> EnglishRuleG2p::dialect_ids()`
  - `text_to_ipa` (function, line 145) `std::string EnglishRuleG2p::text_to_ipa(std::string text,
                                       ...`
  - `dialect_is_british_english_variant` (function, line 238) `bool dialect_is_british_english_variant(std::string_view dialect_id)`
  - `dialect_resolves_to_english_rules` (function, line 243) `bool dialect_resolves_to_english_rules(std::string_view dialect_id)`
  - `sort` (function, line 48) `std::sort(alts.begin(), alts.end());`
  - `runtime_error` (function, line 93) `throw std::runtime_error("English G2P: dictionary not found at " + dict_tsv.generic_string());`
  - `parse` (function, line 102) `nlohmann::json::parse(oov_from_memory->onnx_config_json_utf8), ort_providers, coreml_cache_dir);`
  - `utf8_find_token_codepoints` (function, line 152) `utf8_find_token_codepoints(text, token, pos);`
  - `move` (function, line 220) `std::move(alts), prefer_british_heteronyms_);`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/cmudict-tsv.h`, `core/moonshine-tts/src/lang-specific/english-hand-oov.h`, `core/moonshine-tts/src/lang-specific/english-numbers.h`, `core/moonshine-tts/src/lang-specific/english.h`, `core/moonshine-tts/src/lang-specific/onnx-g2p-models.h`, `core/moonshine-tts/src/text-normalize.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/english.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_ENGLISH_H define MOONSHINE_TTS_LANG_SPECIFIC_ENGLISH_H  include <cstdint> include <fi
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 16)
  - `EnglishOnnxAuxMemory` (struct, line 20)
  - `Impl` (struct, line 58)
  - `EnglishRuleG2p` (class, line 26)
  - `EnglishRuleG2p` (function, line 44) `EnglishRuleG2p(EnglishRuleG2p&&) noexcept;`
  - `dialect_ids` (function, line 50) `static std::vector<std::string> dialect_ids();`
  - `dialect_resolves_to_english_rules` (function, line 67) `bool dialect_resolves_to_english_rules(std::string_view dialect_id);`
  - `dialect_is_british_english_variant` (function, line 72) `bool dialect_is_british_english_variant(std::string_view dialect_id);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_ENGLISH_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_ENGLISH_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/english.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/english-rule-g2p-test.cpp`

## core/moonshine-tts/src/lang-specific/french-compound-map.cpp
- Layer: testing
- Doc: include "french-compound-map.h"
- Language: cpp
- Depends on: `core/moonshine-tts/src/lang-specific/french-compound-map.h`

## core/moonshine-tts/src/lang-specific/french-compound-map.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_FRENCH_COMPOUND_MAP_H define MOONSHINE_TTS_LANG_SPECIFIC_FRENCH_COMPOUND_MAP_H  inclu
- Language: h
- Symbols:
  - `MOONSHINE_TTS_LANG_SPECIFIC_FRENCH_COMPOUND_MAP_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_FRENCH_COMPOUND_MAP_H`
- Imported by: `core/moonshine-tts/src/lang-specific/french-compound-map.cpp`, `core/moonshine-tts/src/lang-specific/french.cpp`

## core/moonshine-tts/src/lang-specific/french-internal.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_FRENCH_INTERNAL_H define MOONSHINE_TTS_LANG_SPECIFIC_FRENCH_INTERNAL_H  include <stri
- Language: h
- Symbols:
  - `oov_word_to_ipa` (function, line 9) `std::string oov_word_to_ipa(const std::string& word, bool with_stress);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_FRENCH_INTERNAL_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_FRENCH_INTERNAL_H`
- Imported by: `core/moonshine-tts/src/lang-specific/french-oov.cpp`, `core/moonshine-tts/src/lang-specific/french.cpp`

## core/moonshine-tts/src/lang-specific/french-oov.cpp
- Layer: testing
- Doc: include <cctype> include <string> include <unordered_map> include <vector>  include "french-internal.h" include "ipa-sym
- Language: cpp
- Symbols:
  - `french_tolower_cp` (function, line 16) `char32_t french_tolower_cp(char32_t c)`
  - `is_allowed_ortho_cp` (function, line 63) `bool is_allowed_ortho_cp(char32_t c)`
  - `letters_only_u32` (function, line 74) `std::u32string letters_only_u32(const std::string& raw)`
  - `v_u32` (function, line 89) `bool v_u32(char32_t ch)`
  - `insert_stress_final_syllable` (function, line 119) `std::string insert_stress_final_syllable(std::string ipa)`
  - `prev_is_nucleus_idx` (function, line 167) `bool prev_is_nucleus_idx(const std::string& s, int idx)`
  - `utf8_last_cp_start` (function, line 213) `size_t utf8_last_cp_start(const std::string& s)`
  - `utf8_prev_cp_start` (function, line 227) `size_t utf8_prev_cp_start(const std::string& s, size_t cp_start)`
  - `trim_final_by_orthography` (function, line 241) `std::string trim_final_by_orthography(std::string ipa,
                                      cons...`
  - `peek_eq` (function, line 314) `bool peek_eq(const std::u32string& w, size_t i, const char* ascii)`
  - `scan_graphemes` (function, line 327) `std::string scan_graphemes(const std::u32string& w)`
  - `oov_word_to_ipa` (function, line 689) `std::string oov_word_to_ipa(const std::string& word, bool with_stress)`
  - `utf8_decode_at` (function, line 81) `utf8_decode_at(raw, i, cp, adv);`
  - `ms` (function, line 127) `const std::string ms(m);`
  - `append_utf8` (function, line 355) `append_utf8(out, "ɛ");`
- Depends on: `core/moonshine-tts/src/lang-specific/french-internal.h`, `core/moonshine-tts/src/lang-specific/ipa-symbols.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/french.cpp
- Layer: testing
- Doc: include "french.h"  include <algorithm> include <array> include <cctype> include <fstream> include <istream> include <re
- Language: cpp
- Symbols:
  - `Tok` (struct, line 1188)
  - `LiaisonStrength` (enum, line 921)
  - `LiaisonStrength` (class, line 921)
  - `french_tolower_cp` (function, line 29) `char32_t french_tolower_cp(char32_t c)`
  - `is_french_key_cp` (function, line 82) `bool is_french_key_cp(char32_t c)`
  - `normalize_lookup_key_utf8` (function, line 93) `std::string normalize_lookup_key_utf8(const std::string& word)`
  - `is_latin1_supplement_python_word_char` (function, line 112) `bool is_latin1_supplement_python_word_char(char32_t cp)`
  - `is_letterlike_math_word_char` (function, line 143) `bool is_letterlike_math_word_char(char32_t cp)`
  - `is_french_word_char` (function, line 148) `bool is_french_word_char(char32_t cp)`
  - `to_lower_ascii` (function, line 176) `std::string to_lower_ascii(std::string_view w)`
  - `to_lower_pos_inventory_utf8` (function, line 184) `std::string to_lower_pos_inventory_utf8(const std::string& word)`
  - `load_french_lexicon_stream` (function, line 197) `void load_french_lexicon_stream(
    std::istream& in, std::unordered_map<std::string, std::strin...`
  - `load_french_lexicon_file` (function, line 229) `void load_french_lexicon_file(
    const std::filesystem::path& path,
    std::unordered_map<std:...`
  - `parse_first_csv_field` (function, line 240) `std::string parse_first_csv_field(std::string_view line)`
  - `load_french_pos_csv_stream` (function, line 269) `void load_french_pos_csv_stream(
    std::istream& in, const std::string& cat_upper,
    std::uno...`
  - `load_french_pos_dir` (function, line 293) `void load_french_pos_dir(
    const std::filesystem::path& dir,
    std::unordered_map<std::strin...`
  - `load_french_pos_from_csv_utf8_map` (function, line 323) `void load_french_pos_from_csv_utf8_map(
    const std::unordered_map<std::string, std::string>& c...`
  - `sort` (function, line 333) `std::sort(sorted.begin(), sorted.end(),
            [](const auto& a, const auto& b)`
  - `below_100` (function, line 349) `std::vector<std::string> below_100(int n)`
  - `below_1000` (function, line 412) `std::vector<std::string> below_1000(int n)`
  - `below_1_000_000` (function, line 446) `std::vector<std::string> below_1_000_000(int n)`
  - `join_space` (function, line 470) `std::string join_space(const std::vector<std::string>& v)`
  - `is_all_ascii_digits` (function, line 481) `bool is_all_ascii_digits(std::string_view s)`
  - `expand_cardinal_digits_to_french_words` (function, line 493) `std::string expand_cardinal_digits_to_french_words(std::string_view s)`
  - `expand_digit_tokens_in_text` (function, line 517) `std::string expand_digit_tokens_in_text(const std::string& text)`
  - `h_aspire_set` (function, line 540) `const std::unordered_set<std::string>& h_aspire_set()`
  - `closed_liaison_determiners` (function, line 551) `const std::unordered_set<std::string>& closed_liaison_determiners()`
  - `pos_scan_order` (function, line 558) `const std::vector<std::string>& pos_scan_order()`
  - `categories_for_form` (function, line 564) `std::vector<std::string> categories_for_form(
    const std::string& word,
    const std::unorder...`
  - `classify_pos` (function, line 582) `std::optional<std::string> classify_pos(
    const std::string& word,
    const std::unordered_ma...`
  - `strip_stress` (function, line 622) `std::string strip_stress(std::string_view ipa)`
  - `french_nucleus_prefixes` (function, line 643) `const std::vector<std::string>& french_nucleus_prefixes()`
  - `replace_suffix_once` (function, line 671) `std::string replace_suffix_once(std::string ipa, std::string_view old_s,
                        ...`
  - `nasal_liaison_transform` (function, line 681) `std::optional<std::string> nasal_liaison_transform(const std::string& word,
                     ...`
  - `ortho_for_liaison` (function, line 702) `std::string ortho_for_liaison(std::string_view word)`
  - `utf8_last_cp` (function, line 722) `bool utf8_last_cp(const std::string& s, char32_t& out_cp)`
  - `orthographic_liaison_consonant` (function, line 738) `std::optional<std::string> orthographic_liaison_consonant(
    std::string_view word)`
  - `ipa_starts_with_vowel_sound` (function, line 766) `bool ipa_starts_with_vowel_sound(std::string_view ipa_sv)`
  - `ipa_ends_with_audible_consonant` (function, line 849) `bool ipa_ends_with_audible_consonant(std::string_view ipa_sv)`
  - `liaison_strength_fn` (function, line 922) `LiaisonStrength liaison_strength_fn(const std::optional<std::string>& pos_left,
                 ...`
  - `lookup_lexicon` (function, line 1015) `std::optional<std::string> lookup_lexicon(
    const std::unordered_map<std::string, std::string>...`
  - `count_primary_stress_marks` (function, line 1038) `size_t count_primary_stress_marks(const std::string& s)`
  - `ensure_french_nuclear_stress` (function, line 1050) `std::string FrenchRuleG2p::ensure_french_nuclear_stress(std::string ipa)`
  - `FrenchRuleG2p` (function, line 1090) `FrenchRuleG2p::FrenchRuleG2p(std::filesystem::path dict_tsv,
                             std::fi...`
  - `FrenchRuleG2p` (function, line 1097) `FrenchRuleG2p::FrenchRuleG2p(std::string dict_tsv_utf8,
                             std::filesys...`
  - `finalize_word_ipa` (function, line 1115) `std::string FrenchRuleG2p::finalize_word_ipa(std::string ipa,
                                   ...`
  - `word_to_ipa_impl` (function, line 1126) `std::string FrenchRuleG2p::word_to_ipa_impl(const std::string& raw_word,
                        ...`
  - `word_to_ipa` (function, line 1170) `std::string FrenchRuleG2p::word_to_ipa(const std::string& word) const`
  - `text_to_ipa` (function, line 1174) `std::string FrenchRuleG2p::text_to_ipa(std::string text,
                                       s...`
  - `text_to_ipa_impl` (function, line 1179) `std::string FrenchRuleG2p::text_to_ipa_impl(
    const std::string& text, bool expand_digits,
   ...`
  - `all_of` (function, line 1328) `std::all_of(t.s.begin(), t.s.end(), [](unsigned char c)`
  - `dialect_resolves_to_french_rules` (function, line 1360) `bool dialect_resolves_to_french_rules(std::string_view dialect_id)`
  - `dialect_ids` (function, line 1368) `std::vector<std::string> FrenchRuleG2p::dialect_ids()`
  - `utf8_decode_at` (function, line 100) `utf8_decode_at(word, i, cp, adv);`
  - `utf8_append_codepoint` (function, line 103) `utf8_append_codepoint(out, cl);`
  - `binary_search` (function, line 145) `return std::binary_search(kLetterlikeWordChars.begin(), kLetterlikeWordChars.end(), cp);`
  - `s` (function, line 178) `std::string s(w);`
  - `in` (function, line 233) `std::ifstream in(path);`
  - `runtime_error` (function, line 235) `throw std::runtime_error("French G2P: cannot read lexicon " + path.generic_string());`
  - `trim_ascii_ws_copy` (function, line 263) `return trim_ascii_ws_copy(out);`
  - `out_of_range` (function, line 352) `throw std::out_of_range("below_100");`
  - `string` (function, line 496) `return std::string(s);`
  - `re` (function, line 519) `static const std::regex re(R"(\b\d+\b)", std::regex::ECMAScript);`
  - `it` (function, line 521) `std::sregex_iterator it(text.begin(), text.end(), re);`
  - `cardinal_compound_ipa_entries` (function, line 538) `return french_compound_map::cardinal_compound_ipa_entries();`
  - `w` (function, line 705) `const std::string w(word);`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/french-compound-map.h`, `core/moonshine-tts/src/lang-specific/french-internal.h`, `core/moonshine-tts/src/lang-specific/french.h`, `core/moonshine-tts/src/lang-specific/ipa-symbols.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/french.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_FRENCH_H define MOONSHINE_TTS_LANG_SPECIFIC_FRENCH_H  include <filesystem> include <s
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 15)
  - `Options` (struct, line 21)
  - `FrenchRuleG2p` (class, line 19)
  - `dialect_id` (function, line 50) `const std::string& dialect_id() const`
  - `FrenchRuleG2p` (function, line 31) `explicit FrenchRuleG2p(std::filesystem::path dict_tsv, std::filesystem::path csv_dir);`
  - `dialect_ids` (function, line 48) `static std::vector<std::string> dialect_ids();`
  - `word_to_ipa` (function, line 52) `std::string word_to_ipa(const std::string& word) const;`
  - `ensure_french_nuclear_stress` (function, line 60) `static std::string ensure_french_nuclear_stress(std::string ipa);`
  - `text_to_ipa_impl` (function, line 68) `std::string text_to_ipa_impl(const std::string& text, bool expand_digits, std::vector<G2pWordLog>* per_word_log) const;`
  - `word_to_ipa_impl` (function, line 71) `std::string word_to_ipa_impl(const std::string& raw_word, bool expand_digits) const;`
  - `finalize_word_ipa` (function, line 74) `std::string finalize_word_ipa(std::string ipa, bool from_compound) const;`
  - `dialect_resolves_to_french_rules` (function, line 78) `bool dialect_resolves_to_french_rules(std::string_view dialect_id);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_FRENCH_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_FRENCH_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/french.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/french-rule-g2p-test.cpp`, `core/moonshine-tts/tools/french-g2p-batch-cli.cpp`

## core/moonshine-tts/src/lang-specific/german.cpp
- Layer: testing
- Doc: include "german.h"  include <algorithm> include <cctype> include <fstream> include <istream> include <regex> include <ss
- Language: cpp
- Symbols:
  - `Slot` (struct, line 756)
  - `german_tolower_cp` (function, line 29) `char32_t german_tolower_cp(char32_t c)`
  - `is_key_char` (function, line 46) `bool is_key_char(char32_t c)`
  - `normalize_lookup_key_utf8` (function, line 56) `std::string normalize_lookup_key_utf8(const std::string& word)`
  - `is_german_word_char` (function, line 71) `bool is_german_word_char(char32_t cp)`
  - `is_vowel_l` (function, line 103) `bool is_vowel_l(char32_t ch)`
  - `char_before_for_ch` (function, line 120) `std::optional<char32_t> char_before_for_ch(const std::u32string& s, size_t i)`
  - `ch_ipa_utf8` (function, line 143) `std::string ch_ipa_utf8(const std::u32string& full_word_nh, size_t i)`
  - `final_devoice` (function, line 161) `std::string final_devoice(std::string ipa)`
  - `st_sp_at_morpheme_start` (function, line 186) `bool st_sp_at_morpheme_start(const std::u32string& hyphen_word,
                             size...`
  - `unstressed_prefix_len_u32` (function, line 210) `size_t unstressed_prefix_len_u32(const std::u32string& w)`
  - `strip_hyphens_u32` (function, line 224) `std::u32string strip_hyphens_u32(const std::u32string& w)`
  - `german_orthographic_syllables_u32` (function, line 280) `std::vector<std::u32string> german_orthographic_syllables_u32(
    const std::u32string& word_lower)`
  - `default_stress_syllable_index` (function, line 338) `size_t default_stress_syllable_index(const std::vector<std::u32string>& syls,
                   ...`
  - `insert_primary_stress_before_vowel_utf8` (function, line 369) `std::string insert_primary_stress_before_vowel_utf8(std::string s)`
  - `ipa_starts_with_nucleus` (function, line 388) `bool ipa_starts_with_nucleus(std::string_view rest)`
  - `ipa_skip_pre_nucleus` (function, line 403) `size_t ipa_skip_pre_nucleus(std::string_view s, size_t j)`
  - `letters_to_ipa_no_stress` (function, line 437) `std::string letters_to_ipa_no_stress(const std::u32string& syl_lower,
                           ...`
  - `rules_word_to_ipa_utf8` (function, line 718) `std::string rules_word_to_ipa_utf8(const std::string& raw_word,
                                 ...`
  - `load_german_lexicon_stream` (function, line 753) `void load_german_lexicon_stream(
    std::istream& in, std::unordered_map<std::string, std::strin...`
  - `load_german_lexicon_file` (function, line 809) `void load_german_lexicon_file(
    const std::filesystem::path& path,
    std::unordered_map<std:...`
  - `g2p_all_ascii_digits` (function, line 824) `bool g2p_all_ascii_digits(std::string_view s)`
  - `german_under_100_word` (function, line 836) `std::string german_under_100_word(int n)`
  - `german_hundred_head` (function, line 867) `std::string german_hundred_head(int h)`
  - `append_german_tokens_1_999` (function, line 879) `void append_german_tokens_1_999(int n, std::vector<std::string>& out)`
  - `append_german_tokens_thousands` (function, line 895) `void append_german_tokens_thousands(int q, std::vector<std::string>& out)`
  - `append_german_below_1_000_000` (function, line 907) `void append_german_below_1_000_000(int n, std::vector<std::string>& out)`
  - `expand_cardinal_digits_to_german_words` (function, line 923) `std::string expand_cardinal_digits_to_german_words(std::string_view s)`
  - `expand_german_digit_tokens_in_text` (function, line 961) `std::string expand_german_digit_tokens_in_text(std::string text)`
  - `ipa_at_stress_mark` (function, line 1011) `bool ipa_at_stress_mark(const std::string& ipa, size_t j)`
  - `normalize_ipa_stress_for_vocoder` (function, line 1020) `std::string GermanRuleG2p::normalize_ipa_stress_for_vocoder(std::string ipa)`
  - `GermanRuleG2p` (function, line 1067) `GermanRuleG2p::GermanRuleG2p(std::filesystem::path dict_tsv, Options options)
    : options_(opti...`
  - `GermanRuleG2p` (function, line 1072) `GermanRuleG2p::GermanRuleG2p(std::string dict_tsv_utf8, Options options)
    : options_(options)`
  - `finalize_ipa` (function, line 1078) `std::string GermanRuleG2p::finalize_ipa(std::string ipa) const`
  - `lookup_or_rules` (function, line 1090) `std::string GermanRuleG2p::lookup_or_rules(const std::string& raw_word) const`
  - `word_to_ipa` (function, line 1156) `std::string GermanRuleG2p::word_to_ipa(const std::string& word) const`
  - `text_to_ipa_no_expand` (function, line 1178) `std::string GermanRuleG2p::text_to_ipa_no_expand(
    const std::string& text, std::vector<G2pWor...`
  - `text_to_ipa` (function, line 1254) `std::string GermanRuleG2p::text_to_ipa(std::string text,
                                       s...`
  - `dialect_resolves_to_german_rules` (function, line 1262) `bool dialect_resolves_to_german_rules(std::string_view dialect_id)`
  - `dialect_ids` (function, line 1270) `std::vector<std::string> GermanRuleG2p::dialect_ids()`
  - `utf8_decode_at` (function, line 62) `utf8_decode_at(word, i, cp, adv);`
  - `utf8_append_codepoint` (function, line 65) `utf8_append_codepoint(out, cl);`
  - `min` (function, line 363) `return std::min(idx + 1, n - 1);`
  - `erase_utf8_substr` (function, line 371) `erase_utf8_substr(s, kPrimaryStressUtf8);`
  - `append` (function, line 458) `append("tʃ");`
  - `trim_ascii_ws_copy` (function, line 771) `trim_ascii_ws_copy(std::string_view(line).substr(0, tab));`
  - `in` (function, line 813) `std::ifstream in(path);`
  - `runtime_error` (function, line 815) `throw std::runtime_error("German lexicon: cannot open " + path.generic_string());`
  - `out_of_range` (function, line 848) `throw std::out_of_range("german_under_100_word");`
  - `string` (function, line 926) `return std::string(s);`
  - `range_re` (function, line 963) `static const std::regex range_re(R"(\b(\d+)-(\d+)\b)", std::regex::ECMAScript);`
  - `dig_re` (function, line 965) `static const std::regex dig_re(R"(\b\d+\b)", std::regex::ECMAScript);`
  - `it` (function, line 967) `std::sregex_iterator it(text.begin(), text.end(), range_re);`
  - `it2` (function, line 992) `std::sregex_iterator it2(text.begin(), text.end(), dig_re);`
  - `normalize_german_ipa_piper_style` (function, line 1083) `return normalize_german_ipa_piper_style(std::move(ipa));`
  - `dig_pass` (function, line 1170) `static const std::regex dig_pass(R"(^[0-9]+(?:-[0-9]+)*$)", std::regex::ECMAScript);`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/ipa-postprocess.h`, `core/moonshine-tts/src/lang-specific/german.h`, `core/moonshine-tts/src/lang-specific/ipa-symbols.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/german.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_GERMAN_H define MOONSHINE_TTS_LANG_SPECIFIC_GERMAN_H  include <filesystem> include <s
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 14)
  - `Options` (struct, line 20)
  - `GermanRuleG2p` (class, line 18)
  - `dialect_id` (function, line 39) `const std::string& dialect_id() const`
  - `GermanRuleG2p` (function, line 32) `explicit GermanRuleG2p(std::filesystem::path dict_tsv);`
  - `dialect_ids` (function, line 37) `static std::vector<std::string> dialect_ids();`
  - `word_to_ipa` (function, line 44) `std::string word_to_ipa(const std::string& word) const;`
  - `normalize_ipa_stress_for_vocoder` (function, line 53) `static std::string normalize_ipa_stress_for_vocoder(std::string ipa);`
  - `lookup_or_rules` (function, line 59) `std::string lookup_or_rules(const std::string& raw_word) const;`
  - `finalize_ipa` (function, line 61) `std::string finalize_ipa(std::string ipa) const;`
  - `text_to_ipa_no_expand` (function, line 62) `std::string text_to_ipa_no_expand( const std::string& text, std::vector<G2pWordLog>* per_word_log) const;`
  - `dialect_resolves_to_german_rules` (function, line 67) `bool dialect_resolves_to_german_rules(std::string_view dialect_id);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_GERMAN_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_GERMAN_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/german.cpp`, `core/moonshine-tts/src/lang-specific/italian.cpp`, `core/moonshine-tts/src/lang-specific/portuguese.cpp`, `core/moonshine-tts/src/lang-specific/russian.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/german-rule-g2p-test.cpp`, `core/moonshine-tts/tools/german-rule-g2p-cli.cpp`

## core/moonshine-tts/src/lang-specific/heteronym-context.cpp
- Layer: testing
- Doc: include "heteronym-context.h"  include <algorithm> include <cmath> include <string> include <vector>
- Language: cpp
- Symbols:
  - `join_cells` (function, line 11) `std::string join_cells(const std::vector<std::string>& cells)`
  - `cells` (function, line 36) `std::vector<std::string> cells(full_cells.begin(), full_cells.end());`
  - `llround` (function, line 59) `std::llround(static_cast<double>(max_chars) / 2.0 - center));`
  - `make_tuple` (function, line 75) `return std::make_tuple(join_cells(cells), s, e);`
- Depends on: `core/moonshine-tts/src/lang-specific/heteronym-context.h`

## core/moonshine-tts/src/lang-specific/heteronym-context.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_HETERONYM_CONTEXT_H define MOONSHINE_TTS_HETERONYM_CONTEXT_H  include <optional> include <string> i
- Language: h
- Symbols:
  - `MOONSHINE_TTS_HETERONYM_CONTEXT_H` (macro, line 2) `#define MOONSHINE_TTS_HETERONYM_CONTEXT_H`
- Imported by: `core/moonshine-tts/src/lang-specific/heteronym-context.cpp`, `core/moonshine-tts/tests/heteronym-context-test.cpp`

## core/moonshine-tts/src/lang-specific/hindi-numbers.cpp
- Layer: infrastructure
- Doc: include "hindi-numbers.h"  include <cctype> include <cstdlib> include <regex> include <string> include <vector>  include
- Language: cpp
- Symbols:
  - `append_join` (function, line 42) `void append_join(std::vector<std::string>& out,
                 const std::vector<std::string>& ...`
  - `under_100` (function, line 49) `std::vector<std::string> under_100(int n)`
  - `tokens_0_999` (function, line 67) `std::vector<std::string> tokens_0_999(int n)`
  - `below_1_000_000_tokens` (function, line 92) `std::vector<std::string> below_1_000_000_tokens(int n)`
  - `join_space` (function, line 119) `std::string join_space(const std::vector<std::string>& v)`
  - `all_ascii_digits` (function, line 130) `bool all_ascii_digits(std::string_view s)`
  - `expand_cardinal_digits_to_hindi_words` (function, line 144) `std::string expand_cardinal_digits_to_hindi_words(std::string_view s)`
  - `expand_hindi_digit_tokens_in_text` (function, line 168) `std::string expand_hindi_digit_tokens_in_text(std::string text)`
  - `expand_devanagari_digit_runs_in_text` (function, line 201) `std::string expand_devanagari_digit_runs_in_text(std::string text)`
  - `string` (function, line 147) `return std::string(s);`
  - `range_re` (function, line 170) `static const std::regex range_re(R"((\b)(\d+)-(\d+)(\b))");`
  - `digit_re` (function, line 171) `static const std::regex digit_re(R"((\b)(\d+)(\b))");`
  - `it` (function, line 174) `std::sregex_iterator it(text.begin(), text.end(), range_re);`
  - `it2` (function, line 191) `std::sregex_iterator it2(text.begin(), text.end(), digit_re);`
  - `utf8_append_codepoint` (function, line 222) `utf8_append_codepoint(result, cp);`
- Depends on: `core/moonshine-tts/src/lang-specific/hindi-numbers.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/hindi-numbers.h
- Layer: infrastructure
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_HINDI_NUMBERS_H define MOONSHINE_TTS_LANG_SPECIFIC_HINDI_NUMBERS_H  include <string> 
- Language: h
- Symbols:
  - `expand_cardinal_digits_to_hindi_words` (function, line 11) `std::string expand_cardinal_digits_to_hindi_words(std::string_view s);`
  - `expand_hindi_digit_tokens_in_text` (function, line 15) `std::string expand_hindi_digit_tokens_in_text(std::string text);`
  - `expand_devanagari_digit_runs_in_text` (function, line 18) `std::string expand_devanagari_digit_runs_in_text(std::string text);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_HINDI_NUMBERS_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_HINDI_NUMBERS_H`
- Imported by: `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp`, `core/moonshine-tts/src/lang-specific/hindi.cpp`, `core/moonshine-tts/tests/hindi-rule-g2p-test.cpp`

## core/moonshine-tts/src/lang-specific/hindi.cpp
- Layer: infrastructure
- Doc: include "hindi.h"  include <cctype> include <filesystem> include <fstream> include <istream> include <optional> include 
- Language: cpp
- Symbols:
  - `Syllable` (struct, line 45)
  - `utf8_nfc_utf8proc` (function, line 32) `std::string utf8_nfc_utf8proc(std::string_view s)`
  - `is_devanagari_digit` (function, line 94) `bool is_devanagari_digit(char32_t cp)`
  - `is_consonant` (function, line 96) `bool is_consonant(char32_t cp)`
  - `cons_ipa` (function, line 100) `std::string cons_ipa(char32_t base, bool nukta)`
  - `sv_starts_with` (function, line 111) `bool sv_starts_with(std::string_view s, std::string_view p)`
  - `nasal_for_place` (function, line 115) `std::string nasal_for_place(std::string_view first_onset)`
  - `syllable_weight` (function, line 154) `int syllable_weight(const Syllable& s)`
  - `assign_stress` (function, line 166) `std::string assign_stress(const std::vector<std::string>& ipa_syllables,
                        ...`
  - `apply_schwa_syncope` (function, line 200) `void apply_schwa_syncope(std::vector<Syllable>& syls)`
  - `parse_devanagari_to_syllables` (function, line 226) `std::optional<std::vector<Syllable>> parse_devanagari_to_syllables(
    const std::string& word)`
  - `render_syllables` (function, line 357) `std::string render_syllables(const std::vector<Syllable>& syls,
                             bool...`
  - `strip_edges_punct` (function, line 423) `void strip_edges_punct(std::string_view w, std::string& core)`
  - `has_devanagari` (function, line 447) `bool has_devanagari(std::string_view s)`
  - `all_ascii_digits_sv` (function, line 457) `bool all_ascii_digits_sv(std::string_view s)`
  - `builtin_hindi_dict_path` (function, line 471) `std::filesystem::path builtin_hindi_dict_path()`
  - `load_hindi_lexicon_stream` (function, line 478) `void load_hindi_lexicon_stream(
    std::istream& in, std::unordered_map<std::string, std::string...`
  - `HindiRuleG2p` (function, line 506) `HindiRuleG2p::HindiRuleG2p(std::filesystem::path dict_tsv, Options options)
    : options_(options)`
  - `HindiRuleG2p` (function, line 520) `HindiRuleG2p::HindiRuleG2p(std::string dict_tsv_utf8, Options options)
    : options_(options)`
  - `word_to_ipa` (function, line 526) `std::string HindiRuleG2p::word_to_ipa(const std::string& word) const`
  - `g2p_single_word` (function, line 530) `std::string HindiRuleG2p::g2p_single_word(std::string_view word) const`
  - `text_to_ipa_no_expand` (function, line 550) `std::string HindiRuleG2p::text_to_ipa_no_expand(
    std::string text, std::vector<G2pWordLog>* p...`
  - `text_to_ipa` (function, line 593) `std::string HindiRuleG2p::text_to_ipa(std::string text,
                                      std...`
  - `dialect_ids` (function, line 602) `std::vector<std::string> HindiRuleG2p::dialect_ids()`
  - `dialect_resolves_to_hindi_rules` (function, line 606) `bool dialect_resolves_to_hindi_rules(std::string_view dialect_id)`
  - `resolve_hindi_dict_path` (function, line 614) `std::filesystem::path resolve_hindi_dict_path(
    const std::filesystem::path& model_root)`
  - `hindi_text_to_ipa` (function, line 619) `std::string hindi_text_to_ipa(const std::string& text, bool with_stress,
                        ...`
  - `tmp` (function, line 34) `const std::string tmp(s);`
  - `utf8proc_NFC` (function, line 36) `utf8proc_NFC(reinterpret_cast<const utf8proc_uint8_t*>(tmp.c_str()));`
  - `string` (function, line 38) `return std::string(s);`
  - `out` (function, line 40) `std::string out(reinterpret_cast<char*>(p));`
  - `free` (function, line 41) `std::free(p);`
  - `base_cons_map` (function, line 98) `return base_cons_map().find(cp) != base_cons_map().end();`
  - `skip_joiners` (function, line 246) `skip_joiners();`
  - `utf8proc_category` (function, line 428) `utf8proc_category(static_cast<utf8proc_int32_t>(cp)));`
  - `utf8_append_codepoint` (function, line 444) `utf8_append_codepoint(core, u[i]);`
  - `trim_ascii_ws_copy` (function, line 494) `trim_ascii_ws_copy(std::string_view(line).substr(0, tab));`
  - `runtime_error` (function, line 510) `throw std::runtime_error("Hindi G2P: lexicon not found at " + dict_tsv.generic_string());`
  - `in` (function, line 513) `std::ifstream in(dict_tsv);`
  - `iss` (function, line 559) `std::istringstream iss(raw);`
  - `expand_cardinal_digits_to_hindi_words` (function, line 572) `expand_cardinal_digits_to_hindi_words(core);`
  - `iss2` (function, line 573) `std::istringstream iss2(expanded);`
  - `g` (function, line 629) `HindiRuleG2p g(path, o);`
  - `0x094D` (variable, line 17) `extern "C" { #include <utf8proc.h> } namespace moonshine_tts { namespace { constexpr char32_t kVirama = 0x094D;`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/hindi-numbers.h`, `core/moonshine-tts/src/lang-specific/hindi.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/hindi.h
- Layer: infrastructure
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_HINDI_H define MOONSHINE_TTS_LANG_SPECIFIC_HINDI_H  include <filesystem> include <str
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 15)
  - `Options` (struct, line 21)
  - `HindiRuleG2p` (class, line 19)
  - `dialect_id` (function, line 33) `const std::string& dialect_id() const`
  - `HindiRuleG2p` (function, line 25) `explicit HindiRuleG2p(std::filesystem::path dict_tsv);`
  - `dialect_ids` (function, line 31) `static std::vector<std::string> dialect_ids();`
  - `word_to_ipa` (function, line 35) `std::string word_to_ipa(const std::string& word) const;`
  - `g2p_single_word` (function, line 46) `std::string g2p_single_word(std::string_view word) const;`
  - `text_to_ipa_no_expand` (function, line 48) `std::string text_to_ipa_no_expand( std::string text, std::vector<G2pWordLog>* per_word_log) const;`
  - `dialect_resolves_to_hindi_rules` (function, line 51) `bool dialect_resolves_to_hindi_rules(std::string_view dialect_id);`
  - `resolve_hindi_dict_path` (function, line 55) `std::filesystem::path resolve_hindi_dict_path( const std::filesystem::path& model_root);`
  - `builtin_hindi_dict_path` (function, line 60) `std::filesystem::path builtin_hindi_dict_path();`
  - `MOONSHINE_TTS_LANG_SPECIFIC_HINDI_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_HINDI_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/hindi.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/hindi-rule-g2p-test.cpp`, `core/moonshine-tts/tools/hindi-rule-g2p-cli.cpp`

## core/moonshine-tts/src/lang-specific/ipa-symbols.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_IPA_SYMBOLS_H define MOONSHINE_TTS_IPA_SYMBOLS_H  include <string>
- Language: h
- Symbols:
  - `MOONSHINE_TTS_IPA_SYMBOLS_H` (macro, line 2) `#define MOONSHINE_TTS_IPA_SYMBOLS_H`
- Imported by: `core/moonshine-tts/src/lang-specific/dutch.cpp`, `core/moonshine-tts/src/lang-specific/french-oov.cpp`, `core/moonshine-tts/src/lang-specific/french.cpp`, `core/moonshine-tts/src/lang-specific/german.cpp`, `core/moonshine-tts/src/lang-specific/italian.cpp`, `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp`, `core/moonshine-tts/src/lang-specific/portuguese.cpp`, `core/moonshine-tts/src/lang-specific/russian.cpp`

## core/moonshine-tts/src/lang-specific/italian.cpp
- Layer: testing
- Doc: include "italian.h"  include <algorithm> include <cctype> include <clocale> include <cstdint> include <cwctype> include 
- Language: cpp
- Symbols:
  - `italian_tolower_cp` (function, line 34) `char32_t italian_tolower_cp(char32_t c)`
  - `is_italian_lexicon_key_cp` (function, line 69) `bool is_italian_lexicon_key_cp(char32_t c)`
  - `normalize_lookup_key_utf8` (function, line 84) `std::string normalize_lookup_key_utf8(const std::string& word)`
  - `utf8_lowercase_italian` (function, line 103) `std::string utf8_lowercase_italian(const std::string& word)`
  - `load_italian_lexicon_stream` (function, line 116) `void load_italian_lexicon_stream(
    std::istream& in, std::unordered_map<std::string, std::stri...`
  - `load_italian_lexicon_file` (function, line 148) `void load_italian_lexicon_file(
    const std::filesystem::path& path,
    std::unordered_map<std...`
  - `is_all_ascii_digits` (function, line 161) `bool is_all_ascii_digits(std::string_view s)`
  - `under_100` (function, line 177) `std::string under_100(int n)`
  - `hundred_head` (function, line 234) `std::string hundred_head(int h)`
  - `append_tokens_0_999` (function, line 246) `void append_tokens_0_999(int n, std::vector<std::string>& out)`
  - `spell_1_999_fused` (function, line 273) `std::string spell_1_999_fused(int n)`
  - `append_thousands_multiplier` (function, line 295) `void append_thousands_multiplier(int q, std::vector<std::string>& out)`
  - `below_1_000_000_tokens` (function, line 313) `void below_1_000_000_tokens(int n, std::vector<std::string>& out)`
  - `expand_cardinal_digits_to_italian_words` (function, line 329) `std::string expand_cardinal_digits_to_italian_words(std::string_view s)`
  - `expand_digit_tokens_in_text` (function, line 365) `std::string expand_digit_tokens_in_text(std::string text)`
  - `utf8_to_u32` (function, line 400) `std::u32string utf8_to_u32(const std::string& s)`
  - `u32_to_utf8` (function, line 413) `std::string u32_to_utf8(const std::u32string& s)`
  - `is_vowel_ch` (function, line 421) `bool is_vowel_ch(char32_t c)`
  - `strip_accent_letter` (function, line 428) `char32_t strip_accent_letter(char32_t c)`
  - `should_hiatus_it` (function, line 453) `bool should_hiatus_it(char32_t a, char32_t b)`
  - `vowel_nucleus_spans` (function, line 483) `void vowel_nucleus_spans(const std::u32string& w,
                         std::vector<std::pair<...`
  - `valid_onset2` (function, line 508) `bool valid_onset2(char a, char b)`
  - `split_intervocalic_cluster` (function, line 522) `void split_intervocalic_cluster(const std::string& cluster, std::string& coda,
                  ...`
  - `italian_orthographic_syllables_u32` (function, line 543) `std::vector<std::u32string> italian_orthographic_syllables_u32(
    std::u32string w)`
  - `accented_vowel_in_u32` (function, line 617) `bool accented_vowel_in_u32(char32_t c)`
  - `default_stressed_syllable_index` (function, line 623) `size_t default_stressed_syllable_index(const std::vector<std::u32string>& syls,
                 ...`
  - `insert_primary_stress_before_vowel` (function, line 665) `std::string insert_primary_stress_before_vowel(std::string ipa)`
  - `next_is_vowel_u32` (function, line 692) `bool next_is_vowel_u32(const std::u32string& s, size_t j)`
  - `ei_e_accent` (function, line 704) `bool ei_e_accent(char32_t c)`
  - `italian_cg_palatal_letter` (function, line 712) `bool italian_cg_palatal_letter(char32_t c)`
  - `letters_to_ipa_no_stress` (function, line 717) `std::string letters_to_ipa_no_stress(const std::u32string& su)`
  - `rules_word_to_ipa_utf8` (function, line 979) `std::string rules_word_to_ipa_utf8(const std::string& raw, bool with_stress)`
  - `is_italian_word_char` (function, line 1067) `bool is_italian_word_char(char32_t cp)`
  - `try_consume_italian_word` (function, line 1101) `bool try_consume_italian_word(const std::string& text, size_t pos,
                              ...`
  - `ItalianRuleG2p` (function, line 1157) `ItalianRuleG2p::ItalianRuleG2p(std::filesystem::path dict_tsv, Options options)
    : options_(op...`
  - `ItalianRuleG2p` (function, line 1162) `ItalianRuleG2p::ItalianRuleG2p(std::string dict_tsv_utf8, Options options)
    : options_(options)`
  - `finalize_ipa` (function, line 1168) `std::string ItalianRuleG2p::finalize_ipa(std::string ipa,
                                       ...`
  - `lookup_or_rules` (function, line 1181) `std::string ItalianRuleG2p::lookup_or_rules(const std::string& raw_word) const`
  - `word_to_ipa` (function, line 1230) `std::string ItalianRuleG2p::word_to_ipa(const std::string& word) const`
  - `text_to_ipa_no_expand` (function, line 1252) `std::string ItalianRuleG2p::text_to_ipa_no_expand(
    const std::string& text, std::vector<G2pWo...`
  - `text_to_ipa` (function, line 1322) `std::string ItalianRuleG2p::text_to_ipa(std::string text,
                                       ...`
  - `dialect_resolves_to_italian_rules` (function, line 1330) `bool dialect_resolves_to_italian_rules(std::string_view dialect_id)`
  - `dialect_ids` (function, line 1338) `std::vector<std::string> ItalianRuleG2p::dialect_ids()`
  - `resolve_italian_dict_path` (function, line 1342) `std::filesystem::path resolve_italian_dict_path(
    const std::filesystem::path& model_root)`
  - `utf8_decode_at` (function, line 91) `utf8_decode_at(word, i, cp, adv);`
  - `utf8_append_codepoint` (function, line 97) `utf8_append_codepoint(out, cl);`
  - `in` (function, line 152) `std::ifstream in(path);`
  - `runtime_error` (function, line 154) `throw std::runtime_error("Italian G2P: cannot read lexicon " + path.generic_string());`
  - `out_of_range` (function, line 186) `throw std::out_of_range("under_100");`
  - `stem` (function, line 203) `std::string stem(tn);`
  - `string` (function, line 332) `return std::string(s);`
  - `range_re` (function, line 367) `static const std::regex range_re(R"(\b(\d+)-(\d+)\b)", std::regex::ECMAScript);`
  - `dig_re` (function, line 369) `static const std::regex dig_re(R"(\b\d+\b)", std::regex::ECMAScript);`
  - `it` (function, line 371) `std::sregex_iterator it(text.begin(), text.end(), range_re);`
  - `it2` (function, line 387) `std::sregex_iterator it2(text.begin(), text.end(), dig_re);`
  - `erase_utf8_substr` (function, line 1172) `erase_utf8_substr(ipa, kPri);`
  - `normalize_ipa_stress_for_vocoder` (function, line 1177) `return GermanRuleG2p::normalize_ipa_stress_for_vocoder(std::move(ipa));`
  - `dig_pass` (function, line 1244) `static const std::regex dig_pass(R"(^[0-9]+(?:-[0-9]+)*$)", std::regex::ECMAScript);`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/german.h`, `core/moonshine-tts/src/lang-specific/ipa-symbols.h`, `core/moonshine-tts/src/lang-specific/italian.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/italian.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_ITALIAN_H define MOONSHINE_TTS_LANG_SPECIFIC_ITALIAN_H  include <filesystem> include 
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 14)
  - `Options` (struct, line 20)
  - `ItalianRuleG2p` (class, line 18)
  - `dialect_id` (function, line 37) `const std::string& dialect_id() const`
  - `ItalianRuleG2p` (function, line 29) `explicit ItalianRuleG2p(std::filesystem::path dict_tsv);`
  - `dialect_ids` (function, line 35) `static std::vector<std::string> dialect_ids();`
  - `word_to_ipa` (function, line 39) `std::string word_to_ipa(const std::string& word) const;`
  - `lookup_or_rules` (function, line 50) `std::string lookup_or_rules(const std::string& raw_word) const;`
  - `finalize_ipa` (function, line 52) `std::string finalize_ipa(std::string ipa, bool from_lexicon) const;`
  - `text_to_ipa_no_expand` (function, line 53) `std::string text_to_ipa_no_expand( const std::string& text, std::vector<G2pWordLog>* per_word_log) const;`
  - `dialect_resolves_to_italian_rules` (function, line 58) `bool dialect_resolves_to_italian_rules(std::string_view dialect_id);`
  - `resolve_italian_dict_path` (function, line 62) `std::filesystem::path resolve_italian_dict_path( const std::filesystem::path& model_root);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_ITALIAN_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_ITALIAN_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/italian.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/italian-rule-g2p-test.cpp`, `core/moonshine-tts/tools/italian-rule-g2p-cli.cpp`

## core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp
- Layer: testing
- Doc: include "japanese-kana-to-ipa.h"  include <cctype> include <optional> include <string> include <tuple> include <utility>
- Language: cpp
- Symbols:
  - `utf8_nfkc_utf8proc` (function, line 18) `std::string utf8_nfkc_utf8proc(std::string_view s)`
  - `katakana_to_hiragana_u32` (function, line 30) `std::u32string katakana_to_hiragana_u32(const std::u32string& in)`
  - `u32_to_utf8` (function, line 50) `std::string u32_to_utf8(const std::u32string& u)`
  - `utf8_starts_with_at` (function, line 58) `bool utf8_starts_with_at(const std::string& s, std::size_t off,
                         const st...`
  - `long_mark_extend_last` (function, line 66) `void long_mark_extend_last(std::vector<std::string>& parts)`
  - `geminate_onset` (function, line 151) `std::string geminate_onset(const std::string& onset,
                           const std::string...`
  - `katakana_hiragana_to_ipa` (function, line 162) `std::string katakana_hiragana_to_ipa(std::string_view sv)`
  - `japanese_is_kana_only` (function, line 225) `bool japanese_is_kana_only(std::string_view sv)`
  - `japanese_has_japanese_script` (function, line 254) `bool japanese_has_japanese_script(std::string_view sv)`
  - `tmp` (function, line 20) `const std::string tmp(s);`
  - `utf8proc_NFKC` (function, line 22) `utf8proc_NFKC(reinterpret_cast<const utf8proc_uint8_t*>(tmp.c_str()));`
  - `string` (function, line 24) `return std::string(s);`
  - `out` (function, line 26) `std::string out(reinterpret_cast<char*>(p));`
  - `free` (function, line 27) `std::free(p);`
  - `utf8_append_codepoint` (function, line 54) `utf8_append_codepoint(s, c);`
  - `utf8_decode_at` (function, line 208) `utf8_decode_at(s, i, cp, adv);`
- Depends on: `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_JAPANESE_KANA_TO_IPA_H define MOONSHINE_TTS_JAPANESE_KANA_TO_IPA_H  include <string> include <strin
- Language: h
- Symbols:
  - `katakana_hiragana_to_ipa` (function, line 11) `std::string katakana_hiragana_to_ipa(std::string_view utf8);`
  - `japanese_is_kana_only` (function, line 12) `bool japanese_is_kana_only(std::string_view utf8);`
  - `japanese_has_japanese_script` (function, line 14) `bool japanese_has_japanese_script(std::string_view utf8);`
  - `MOONSHINE_TTS_JAPANESE_KANA_TO_IPA_H` (macro, line 2) `#define MOONSHINE_TTS_JAPANESE_KANA_TO_IPA_H`
- Imported by: `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp`, `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp`

## core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp
- Layer: testing
- Doc: include "japanese-onnx-g2p.h"  include <algorithm> include <fstream> include <istream> include <sstream> include <stdexc
- Language: cpp
- Symbols:
  - `utf8_nfc_utf8proc` (function, line 21) `std::string utf8_nfc_utf8proc(std::string_view s)`
  - `is_han_cp` (function, line 33) `bool is_han_cp(char32_t cp)`
  - `is_single_han` (function, line 39) `bool is_single_han(std::string_view s)`
  - `only_hiragana` (function, line 44) `bool only_hiragana(std::string_view s)`
  - `only_katakana` (function, line 57) `bool only_katakana(std::string_view s)`
  - `only_han` (function, line 73) `bool only_han(std::string_view s)`
  - `trailing_particles_sorted` (function, line 175) `const std::vector<std::string>& trailing_particles_sorted()`
  - `sort` (function, line 183) `std::sort(v.begin(), v.end(),
              [](const std::string& a, const std::string& b)`
  - `build_by_first` (function, line 227) `void build_by_first(
    const std::unordered_map<std::string, std::string>& lex,
    std::unorde...`
  - `sort` (function, line 246) `std::sort(vec.begin(), vec.end(),
              [](const std::string& a, const std::string& b)`
  - `default_japanese_dict_path` (function, line 254) `std::filesystem::path default_japanese_dict_path(
    const std::filesystem::path& g2p_data_root)`
  - `JapaneseOnnxG2p` (function, line 259) `JapaneseOnnxG2p::JapaneseOnnxG2p(std::filesystem::path model_dir,
                               ...`
  - `JapaneseOnnxG2p` (function, line 266) `JapaneseOnnxG2p::JapaneseOnnxG2p(std::filesystem::path model_dir,
                               ...`
  - `JapaneseOnnxG2p` (function, line 274) `JapaneseOnnxG2p::JapaneseOnnxG2p(const MoonshineG2POptions& opt,
                                ...`
  - `JapaneseOnnxG2p` (function, line 282) `JapaneseOnnxG2p::JapaneseOnnxG2p(const MoonshineG2POptions& opt,
                                ...`
  - `g2p_word` (function, line 291) `std::string JapaneseOnnxG2p::g2p_word(std::string word_utf8)`
  - `text_to_ipa` (function, line 356) `std::string JapaneseOnnxG2p::text_to_ipa(std::string text_utf8)`
  - `tmp` (function, line 23) `const std::string tmp(s);`
  - `utf8proc_NFC` (function, line 25) `utf8proc_NFC(reinterpret_cast<const utf8proc_uint8_t*>(tmp.c_str()));`
  - `string` (function, line 27) `return std::string(s);`
  - `out` (function, line 29) `std::string out(reinterpret_cast<char*>(p));`
  - `free` (function, line 30) `std::free(p);`
  - `merge_verb_adj_okurigana` (function, line 173) `return merge_verb_adj_okurigana(std::move(b));`
  - `iss` (function, line 209) `std::istringstream iss(ipa_col);`
  - `in` (function, line 221) `std::ifstream in(p);`
  - `runtime_error` (function, line 223) `throw std::runtime_error("JapaneseOnnxG2p: cannot open dict " + p.string());`
  - `load_ja_lexicon_first_ipa_stream` (function, line 225) `return load_ja_lexicon_first_ipa_stream(in);`
  - `katakana_hiragana_to_ipa` (function, line 318) `return katakana_hiragana_to_ipa(w);`
  - `utf8_decode_at` (function, line 325) `utf8_decode_at(w, i, cp0, adv0);`
- Depends on: `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.h`, `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_JAPANESE_ONNX_G2P_H define MOONSHINE_TTS_JAPANESE_ONNX_G2P_H  include <filesystem> include <string>
- Language: h
- Symbols:
  - `MoonshineG2POptions` (struct, line 13)
  - `JapaneseOnnxG2p` (class, line 17)
  - `tok` (function, line 33) `const JapaneseTokPosOnnx& tok() const`
  - `JapaneseOnnxG2p` (function, line 18) `public: explicit JapaneseOnnxG2p(std::filesystem::path model_dir, std::filesystem::path dict_tsv, bool use_cuda = false);`
  - `g2p_word` (function, line 30) `std::string g2p_word(std::string word_utf8);`
  - `text_to_ipa` (function, line 32) `std::string text_to_ipa(std::string text_utf8);`
  - `default_japanese_dict_path` (function, line 41) `std::filesystem::path default_japanese_dict_path( const std::filesystem::path& g2p_data_root);`
  - `MOONSHINE_TTS_JAPANESE_ONNX_G2P_H` (macro, line 2) `#define MOONSHINE_TTS_JAPANESE_ONNX_G2P_H`
- Depends on: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.h`
- Imported by: `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp`, `core/moonshine-tts/src/lang-specific/japanese.cpp`, `core/moonshine-tts/tests/japanese-onnx-g2p-test.cpp`, `core/moonshine-tts/tools/japanese-onnx-g2p-cli.cpp`

## core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp
- Layer: testing
- Doc: include "japanese-tok-pos-onnx.h"  include <nlohmann/json.h>  include <algorithm> include <array> include <cctype> inclu
- Language: cpp
- Symbols:
  - `BasicTokCfg` (struct, line 311)
  - `EncodedWp` (struct, line 423)
  - `Idx` (struct, line 513)
  - `open_session` (function, line 30) `std::unique_ptr<Ort::Session> open_session(
    Ort::Env& env, const std::filesystem::path& model...`
  - `open_session_memory` (function, line 47) `std::unique_ptr<Ort::Session> open_session_memory(
    Ort::Env& env, const void* data, size_t le...`
  - `slurp_utf8_file` (function, line 61) `std::string slurp_utf8_file(const std::filesystem::path& p)`
  - `bundle_load_utf8` (function, line 71) `bool bundle_load_utf8(const MoonshineG2POptions* opt,
                      std::string_view bund...`
  - `bundle_load_binary` (function, line 89) `bool bundle_load_binary(const MoonshineG2POptions* opt,
                        std::string_view ...`
  - `utf8_to_u32` (function, line 122) `std::u32string utf8_to_u32(std::string_view utf8)`
  - `u32_to_utf8` (function, line 135) `std::string u32_to_utf8(const std::u32string& s)`
  - `is_space_u32` (function, line 143) `bool is_space_u32(char32_t c)`
  - `is_control_u32` (function, line 152) `bool is_control_u32(char32_t c)`
  - `is_punctuation_u32` (function, line 161) `bool is_punctuation_u32(char32_t c)`
  - `is_punct_char_word_group_u32` (function, line 175) `bool is_punct_char_word_group_u32(char32_t c)`
  - `is_chinese_char` (function, line 179) `bool is_chinese_char(std::uint32_t cp)`
  - `u32_nfc` (function, line 188) `std::u32string u32_nfc(const std::u32string& s)`
  - `strip_mn_nfd` (function, line 200) `std::u32string strip_mn_nfd(const std::u32string& s)`
  - `to_lower_u32` (function, line 220) `std::u32string to_lower_u32(const std::u32string& s)`
  - `clean_text_u32` (function, line 229) `std::u32string clean_text_u32(const std::u32string& text)`
  - `tokenize_chinese_chars_u32` (function, line 241) `std::u32string tokenize_chinese_chars_u32(const std::u32string& text)`
  - `split_u32_whitespace` (function, line 255) `std::vector<std::u32string> split_u32_whitespace(std::u32string_view s)`
  - `run_split_on_punc_u32` (function, line 280) `std::vector<std::u32string> run_split_on_punc_u32(const std::u32string& text)`
  - `normalization_ref_u32` (function, line 316) `std::u32string normalization_ref_u32(const std::u32string& text_u32,
                            ...`
  - `basic_tokenize_u32` (function, line 325) `std::vector<std::u32string> basic_tokenize_u32(
    const std::u32string& original_text_u32, cons...`
  - `align_basic_tokens_u32` (function, line 357) `void align_basic_tokens_u32(const std::u32string& ref,
                            const std::vec...`
  - `wordpiece_tokenize_u32` (function, line 374) `std::vector<std::u32string> wordpiece_tokenize_u32(
    const std::u32string& token,
    const st...`
  - `encode_bert_wordpiece` (function, line 429) `EncodedWp encode_bert_wordpiece(
    const std::u32string& text_u32,
    const std::unordered_map...`
  - `ud_upos_set` (function, line 597) `const std::unordered_set<std::string>& ud_upos_set()`
  - `morph_label_to_upos` (function, line 605) `std::string morph_label_to_upos(std::string label)`
  - `cjk_tokpos_preferred_chunk_break_cp` (function, line 649) `bool cjk_tokpos_preferred_chunk_break_cp(char32_t c)`
  - `cjk_tokpos_chunk_exclusive_end` (function, line 682) `template <typename EncodeFn>
std::size_t cjk_tokpos_chunk_exclusive_end(const std::u32string& ful...`
  - `default_japanese_tok_pos_model_dir` (function, line 721) `std::filesystem::path default_japanese_tok_pos_model_dir(
    const std::filesystem::path& g2p_da...`
  - `JapaneseTokPosOnnx` (function, line 731) `JapaneseTokPosOnnx::JapaneseTokPosOnnx(const MoonshineG2POptions* opt,
                          ...`
  - `format_annotated_line` (function, line 792) `std::string JapaneseTokPosOnnx::format_annotated_line(
    const std::vector<std::pair<std::strin...`
  - `make_g2p_ort_session_options` (function, line 39) `make_g2p_ort_session_options(ort_providers, coreml_cache_dir));`
  - `ort_add_external_initializer_files_for_onnx_model_buffer` (function, line 56) `ort_add_external_initializer_files_for_onnx_model_buffer(so, opt->files, model_map_key);`
  - `in` (function, line 63) `std::ifstream in(p, std::ios::binary);`
  - `utf8_decode_at` (function, line 129) `utf8_decode_at(std::string(utf8), i, cp, adv);`
  - `utf8_append_codepoint` (function, line 139) `utf8_append_codepoint(out, cp);`
  - `utf8proc_NFC` (function, line 192) `utf8proc_NFC(reinterpret_cast<const utf8proc_uint8_t*>(utf8.c_str()));`
  - `composed` (function, line 196) `std::string composed(reinterpret_cast<char*>(nfc));`
  - `free` (function, line 197) `std::free(nfc);`
  - `utf8proc_NFD` (function, line 204) `utf8proc_NFD(reinterpret_cast<const utf8proc_uint8_t*>(utf8.c_str()));`
  - `nfd_str` (function, line 208) `std::string nfd_str(reinterpret_cast<char*>(nfd));`
  - `utf8proc_tolower` (function, line 225) `utf8proc_tolower(static_cast<utf8proc_int32_t>(cp))));`
  - `runtime_error` (function, line 367) `throw std::runtime_error( "Japanese WordPiece: basic token alignment failed at offset " + std::to_string(cursor));`
  - `chars` (function, line 385) `std::vector<char32_t> chars(wt.begin(), wt.end());`
  - `piece_u32` (function, line 393) `std::u32string piece_u32( chars.begin() + static_cast<std::ptrdiff_t>(start), chars.begin() + static_cast<std::ptrdiff_t>(end));`
  - `buf` (function, line 645) `const std::string buf(utf8);`
  - `load_vocab_txt_stream` (function, line 647) `return load_vocab_txt_stream(in);`
  - `g2p_bundle_file_key` (function, line 774) `g2p_bundle_file_key(onnx_bundle_key, onnx_name);`
  - `load_vocab_txt_string` (function, line 816) `load_vocab_txt_string(cached_vocab_txt_);`
  - `mask` (function, line 849) `std::vector<int64_t> mask(static_cast<size_t>(T), 1);`
  - `pooled` (function, line 883) `std::vector<double> pooled(static_cast<size_t>(num_labels), 0.0);`
- Depends on: `core/moonshine-tts/src/g2p-path.h`, `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-tts/src/ort-onnx-external-data.h`, `core/moonshine-tts/src/ort-session-options.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_JAPANESE_TOK_POS_ONNX_H define MOONSHINE_TTS_JAPANESE_TOK_POS_ONNX_H  include <onnxruntime_cxx_api.
- Language: h
- Symbols:
  - `MoonshineG2POptions` (struct, line 16)
  - `JapaneseTokPosOnnx` (class, line 23)
  - `model_dir` (function, line 41) `const std::filesystem::path& model_dir() const`
  - `JapaneseTokPosOnnx` (function, line 24) `public: explicit JapaneseTokPosOnnx(std::filesystem::path model_dir, bool use_cuda = false);`
  - `format_annotated_line` (function, line 39) `static std::string format_annotated_line( const std::vector<std::pair<std::string, std::string>>& pairs);`
  - `default_japanese_tok_pos_model_dir` (function, line 60) `std::filesystem::path default_japanese_tok_pos_model_dir( const std::filesystem::path& g2p_data_root);`
  - `MOONSHINE_TTS_JAPANESE_TOK_POS_ONNX_H` (macro, line 2) `#define MOONSHINE_TTS_JAPANESE_TOK_POS_ONNX_H`
- Imported by: `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.h`, `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp`, `core/moonshine-tts/tests/japanese-tok-pos-onnx-test.cpp`

## core/moonshine-tts/src/lang-specific/japanese.cpp
- Layer: testing
- Doc: include "japanese.h"  include <cctype> include <utility>  include "g2p-path.h" include "g2p-word-log.h" include "japanes
- Language: cpp
- Symbols:
  - `absolute_model_root` (function, line 15) `std::filesystem::path absolute_model_root(
    const std::filesystem::path& model_root)`
  - `JapaneseRuleG2p` (function, line 31) `JapaneseRuleG2p::JapaneseRuleG2p(std::filesystem::path onnx_model_dir,
                          ...`
  - `JapaneseRuleG2p` (function, line 36) `JapaneseRuleG2p::JapaneseRuleG2p(std::filesystem::path onnx_model_dir,
                          ...`
  - `JapaneseRuleG2p` (function, line 41) `JapaneseRuleG2p::JapaneseRuleG2p(const MoonshineG2POptions& opt,
                                ...`
  - `JapaneseRuleG2p` (function, line 47) `JapaneseRuleG2p::JapaneseRuleG2p(const MoonshineG2POptions& opt,
                                ...`
  - `text_to_ipa` (function, line 60) `std::string JapaneseRuleG2p::text_to_ipa(
    std::string text, std::vector<G2pWordLog>* per_word...`
  - `dialect_ids` (function, line 66) `std::vector<std::string> JapaneseRuleG2p::dialect_ids()`
  - `dialect_resolves_to_japanese_rules` (function, line 71) `bool dialect_resolves_to_japanese_rules(std::string_view dialect_id)`
  - `resolve_japanese_dict_path` (function, line 79) `std::filesystem::path resolve_japanese_dict_path(
    const std::filesystem::path& model_root)`
  - `resolve_japanese_onnx_model_dir` (function, line 85) `std::filesystem::path resolve_japanese_onnx_model_dir(
    const std::filesystem::path& model_root)`
  - `absolute` (function, line 21) `std::filesystem::absolute(model_root), ec);`
- Depends on: `core/moonshine-tts/src/g2p-path.h`, `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.h`, `core/moonshine-tts/src/lang-specific/japanese.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/japanese.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_JAPANESE_H define MOONSHINE_TTS_LANG_SPECIFIC_JAPANESE_H  include <filesystem> includ
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 14)
  - `MoonshineG2POptions` (struct, line 15)
  - `JapaneseRuleG2p` (class, line 21)
  - `dialect_id` (function, line 42) `const std::string& dialect_id() const`
  - `JapaneseRuleG2p` (function, line 22) `public: explicit JapaneseRuleG2p(std::filesystem::path onnx_model_dir, std::filesystem::path dict_tsv, bool use_cuda = false);`
  - `dialect_ids` (function, line 40) `static std::vector<std::string> dialect_ids();`
  - `dialect_resolves_to_japanese_rules` (function, line 53) `bool dialect_resolves_to_japanese_rules(std::string_view dialect_id);`
  - `resolve_japanese_dict_path` (function, line 57) `std::filesystem::path resolve_japanese_dict_path( const std::filesystem::path& model_root);`
  - `resolve_japanese_onnx_model_dir` (function, line 62) `std::filesystem::path resolve_japanese_onnx_model_dir( const std::filesystem::path& model_root);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_JAPANESE_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_JAPANESE_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/japanese.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`

## core/moonshine-tts/src/lang-specific/korean-numbers.cpp
- Layer: testing
- Doc: include "korean-numbers.h"  include <cctype> include <cstring> include <limits> include <optional> include <string> incl
- Language: cpp
- Symbols:
  - `is_ascii_digit` (function, line 20) `bool is_ascii_digit(char c)`
  - `thousands_lookahead_ok` (function, line 22) `bool thousands_lookahead_ok(std::string_view suf)`
  - `strip_thousands_commas` (function, line 38) `std::string strip_thousands_commas(std::string_view raw)`
  - `normalize_numeral_token_string` (function, line 51) `std::string normalize_numeral_token_string(std::string_view raw)`
  - `hangul_digits_only` (function, line 65) `std::string hangul_digits_only(std::string_view s)`
  - `section_under_10000` (function, line 75) `std::string section_under_10000(unsigned n)`
  - `parse_uint_strict` (function, line 123) `bool parse_uint_strict(std::string_view sv, std::uint64_t& out)`
  - `int_to_sino_korean_hangul` (function, line 146) `std::string int_to_sino_korean_hangul(std::uint64_t n)`
  - `korean_reading_fragments_from_ascii_numeral_token` (function, line 187) `std::optional<std::vector<std::string>>
korean_reading_fragments_from_ascii_numeral_token(std::st...`
  - `is_ascii_numeral_token` (function, line 286) `bool is_ascii_numeral_token(std::string_view token)`
  - `gs` (function, line 160) `std::vector<unsigned> gs(low_first.rbegin(), low_first.rend());`
  - `string_view` (function, line 221) `std::string_view(raw).substr(i, dot_or_comma - i);`
- Depends on: `core/moonshine-tts/src/lang-specific/korean-numbers.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/korean-numbers.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_KOREAN_NUMBERS_H define MOONSHINE_TTS_LANG_SPECIFIC_KOREAN_NUMBERS_H  include <cstdin
- Language: h
- Symbols:
  - `int_to_sino_korean_hangul` (function, line 14) `std::string int_to_sino_korean_hangul(std::uint64_t n);`
  - `korean_reading_fragments_from_ascii_numeral_token` (function, line 19) `std::optional<std::vector<std::string>> korean_reading_fragments_from_ascii_numeral_token(std::string_view token);`
  - `is_ascii_numeral_token` (function, line 21) `bool is_ascii_numeral_token(std::string_view token);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_KOREAN_NUMBERS_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_KOREAN_NUMBERS_H`
- Imported by: `core/moonshine-tts/src/lang-specific/korean-numbers.cpp`, `core/moonshine-tts/src/lang-specific/korean.cpp`, `core/moonshine-tts/tests/korean-rule-g2p-test.cpp`

## core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp
- Layer: testing
- Doc: include "korean-tok-pos-onnx.h"  include <nlohmann/json.h>  include <algorithm> include <array> include <cctype> include
- Language: cpp
- Symbols:
  - `BasicTokCfg` (struct, line 311)
  - `EncodedWp` (struct, line 423)
  - `Idx` (struct, line 513)
  - `open_session` (function, line 30) `std::unique_ptr<Ort::Session> open_session(
    Ort::Env& env, const std::filesystem::path& model...`
  - `open_session_memory` (function, line 47) `std::unique_ptr<Ort::Session> open_session_memory(
    Ort::Env& env, const void* data, size_t le...`
  - `slurp_utf8_file` (function, line 61) `std::string slurp_utf8_file(const std::filesystem::path& p)`
  - `bundle_load_utf8` (function, line 71) `bool bundle_load_utf8(const MoonshineG2POptions* opt,
                      std::string_view bund...`
  - `bundle_load_binary` (function, line 89) `bool bundle_load_binary(const MoonshineG2POptions* opt,
                        std::string_view ...`
  - `utf8_to_u32` (function, line 122) `std::u32string utf8_to_u32(std::string_view utf8)`
  - `u32_to_utf8` (function, line 135) `std::string u32_to_utf8(const std::u32string& s)`
  - `is_space_u32` (function, line 143) `bool is_space_u32(char32_t c)`
  - `is_control_u32` (function, line 152) `bool is_control_u32(char32_t c)`
  - `is_punctuation_u32` (function, line 161) `bool is_punctuation_u32(char32_t c)`
  - `is_punct_char_word_group_u32` (function, line 175) `bool is_punct_char_word_group_u32(char32_t c)`
  - `is_chinese_char` (function, line 179) `bool is_chinese_char(std::uint32_t cp)`
  - `u32_nfc` (function, line 188) `std::u32string u32_nfc(const std::u32string& s)`
  - `strip_mn_nfd` (function, line 200) `std::u32string strip_mn_nfd(const std::u32string& s)`
  - `to_lower_u32` (function, line 220) `std::u32string to_lower_u32(const std::u32string& s)`
  - `clean_text_u32` (function, line 229) `std::u32string clean_text_u32(const std::u32string& text)`
  - `tokenize_chinese_chars_u32` (function, line 241) `std::u32string tokenize_chinese_chars_u32(const std::u32string& text)`
  - `split_u32_whitespace` (function, line 255) `std::vector<std::u32string> split_u32_whitespace(std::u32string_view s)`
  - `run_split_on_punc_u32` (function, line 280) `std::vector<std::u32string> run_split_on_punc_u32(const std::u32string& text)`
  - `normalization_ref_u32` (function, line 316) `std::u32string normalization_ref_u32(const std::u32string& text_u32,
                            ...`
  - `basic_tokenize_u32` (function, line 325) `std::vector<std::u32string> basic_tokenize_u32(
    const std::u32string& original_text_u32, cons...`
  - `align_basic_tokens_u32` (function, line 357) `void align_basic_tokens_u32(const std::u32string& ref,
                            const std::vec...`
  - `wordpiece_tokenize_u32` (function, line 374) `std::vector<std::u32string> wordpiece_tokenize_u32(
    const std::u32string& token,
    const st...`
  - `encode_bert_wordpiece` (function, line 429) `EncodedWp encode_bert_wordpiece(
    const std::u32string& text_u32,
    const std::unordered_map...`
  - `ud_upos_set` (function, line 597) `const std::unordered_set<std::string>& ud_upos_set()`
  - `morph_label_to_upos` (function, line 605) `std::string morph_label_to_upos(std::string label)`
  - `cjk_tokpos_preferred_chunk_break_cp` (function, line 649) `bool cjk_tokpos_preferred_chunk_break_cp(char32_t c)`
  - `cjk_tokpos_chunk_exclusive_end` (function, line 682) `template <typename EncodeFn>
std::size_t cjk_tokpos_chunk_exclusive_end(const std::u32string& ful...`
  - `default_korean_tok_pos_model_dir` (function, line 721) `std::filesystem::path default_korean_tok_pos_model_dir(
    const std::filesystem::path& g2p_data...`
  - `KoreanTokPosOnnx` (function, line 731) `KoreanTokPosOnnx::KoreanTokPosOnnx(const MoonshineG2POptions* opt,
                              ...`
  - `format_annotated_line` (function, line 791) `std::string KoreanTokPosOnnx::format_annotated_line(
    const std::vector<std::pair<std::string,...`
  - `make_g2p_ort_session_options` (function, line 39) `make_g2p_ort_session_options(ort_providers, coreml_cache_dir));`
  - `ort_add_external_initializer_files_for_onnx_model_buffer` (function, line 56) `ort_add_external_initializer_files_for_onnx_model_buffer(so, opt->files, model_map_key);`
  - `in` (function, line 63) `std::ifstream in(p, std::ios::binary);`
  - `utf8_decode_at` (function, line 129) `utf8_decode_at(std::string(utf8), i, cp, adv);`
  - `utf8_append_codepoint` (function, line 139) `utf8_append_codepoint(out, cp);`
  - `utf8proc_NFC` (function, line 192) `utf8proc_NFC(reinterpret_cast<const utf8proc_uint8_t*>(utf8.c_str()));`
  - `composed` (function, line 196) `std::string composed(reinterpret_cast<char*>(nfc));`
  - `free` (function, line 197) `std::free(nfc);`
  - `utf8proc_NFD` (function, line 204) `utf8proc_NFD(reinterpret_cast<const utf8proc_uint8_t*>(utf8.c_str()));`
  - `nfd_str` (function, line 208) `std::string nfd_str(reinterpret_cast<char*>(nfd));`
  - `utf8proc_tolower` (function, line 225) `utf8proc_tolower(static_cast<utf8proc_int32_t>(cp))));`
  - `runtime_error` (function, line 367) `throw std::runtime_error( "Korean WordPiece: basic token alignment failed at offset " + std::to_string(cursor));`
  - `chars` (function, line 385) `std::vector<char32_t> chars(wt.begin(), wt.end());`
  - `piece_u32` (function, line 393) `std::u32string piece_u32( chars.begin() + static_cast<std::ptrdiff_t>(start), chars.begin() + static_cast<std::ptrdiff_t>(end));`
  - `buf` (function, line 645) `const std::string buf(utf8);`
  - `load_vocab_txt_stream` (function, line 647) `return load_vocab_txt_stream(in);`
  - `g2p_bundle_file_key` (function, line 773) `g2p_bundle_file_key(onnx_bundle_key, onnx_name);`
  - `load_vocab_txt_string` (function, line 815) `load_vocab_txt_string(cached_vocab_txt_);`
  - `mask` (function, line 848) `std::vector<int64_t> mask(static_cast<size_t>(T), 1);`
  - `pooled` (function, line 882) `std::vector<double> pooled(static_cast<size_t>(num_labels), 0.0);`
- Depends on: `core/moonshine-tts/src/g2p-path.h`, `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-tts/src/ort-onnx-external-data.h`, `core/moonshine-tts/src/ort-session-options.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_KOREAN_TOK_POS_ONNX_H define MOONSHINE_TTS_KOREAN_TOK_POS_ONNX_H  include <onnxruntime_cxx_api.h>  
- Language: h
- Symbols:
  - `MoonshineG2POptions` (struct, line 16)
  - `KoreanTokPosOnnx` (class, line 23)
  - `model_dir` (function, line 41) `const std::filesystem::path& model_dir() const`
  - `KoreanTokPosOnnx` (function, line 24) `public: explicit KoreanTokPosOnnx(std::filesystem::path model_dir, bool use_cuda = false);`
  - `format_annotated_line` (function, line 39) `static std::string format_annotated_line( const std::vector<std::pair<std::string, std::string>>& pairs);`
  - `default_korean_tok_pos_model_dir` (function, line 60) `std::filesystem::path default_korean_tok_pos_model_dir( const std::filesystem::path& g2p_data_root);`
  - `MOONSHINE_TTS_KOREAN_TOK_POS_ONNX_H` (macro, line 2) `#define MOONSHINE_TTS_KOREAN_TOK_POS_ONNX_H`
- Imported by: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp`, `core/moonshine-tts/tests/korean-tok-pos-onnx-test.cpp`

## core/moonshine-tts/src/lang-specific/korean.cpp
- Layer: testing
- Doc: include "korean.h"  include <cctype> include <cstdlib> include <fstream> include <istream> include <limits> include <opt
- Language: cpp
- Symbols:
  - `Syllable` (struct, line 55)
  - `replace_all` (function, line 60) `void replace_all(std::string& s, const std::string& from,
                 const std::string& to)`
  - `utf8_nfc_utf8proc` (function, line 71) `std::string utf8_nfc_utf8proc(std::string_view s)`
  - `strip_mn_after_nfd` (function, line 83) `std::string strip_mn_after_nfd(const std::string& ipa)`
  - `is_sonorant_jong` (function, line 175) `bool is_sonorant_jong(int jong)`
  - `jong_triggers_tense` (function, line 182) `bool jong_triggers_tense(int jong)`
  - `tense_cho` (function, line 203) `int tense_cho(int plain_cho)`
  - `decompose_syllable_cp` (function, line 220) `std::optional<Syllable> decompose_syllable_cp(char32_t ch)`
  - `text_to_syllables` (function, line 232) `std::vector<Syllable> text_to_syllables(std::string_view text)`
  - `apply_linking` (function, line 248) `void apply_linking(std::vector<Syllable>& syls)`
  - `apply_lateralization` (function, line 276) `void apply_lateralization(std::vector<Syllable>& syls)`
  - `ipa_onset` (function, line 290) `std::string ipa_onset(int cho, bool tense, bool aspirate)`
  - `ipa_nucleus` (function, line 375) `std::string ipa_nucleus(int jung)`
  - `ipa_coda_simple` (function, line 388) `std::string ipa_coda_simple(int jong)`
  - `coda_nasal_assimilate` (function, line 424) `std::string coda_nasal_assimilate(int jong, std::optional<int> next_cho)`
  - `syllables_to_ipa` (function, line 446) `std::string syllables_to_ipa(const std::vector<Syllable>& syls,
                             std:...`
  - `sino_cardinal_speech_units` (function, line 550) `std::vector<std::string> sino_cardinal_speech_units(std::uint64_t n)`
  - `g2p_hangul_rules_only_inner` (function, line 577) `std::string g2p_hangul_rules_only_inner(std::string_view hangul,
                                ...`
  - `normalize_korean_ipa` (function, line 593) `std::string KoreanRuleG2p::normalize_korean_ipa(std::string ipa,
                                ...`
  - `extract_hangul` (function, line 722) `std::string KoreanRuleG2p::extract_hangul(std::string_view s) const`
  - `g2p_hangul_rules_only` (function, line 738) `std::string KoreanRuleG2p::g2p_hangul_rules_only(
    std::string_view hangul) const`
  - `g2p_single_fragment` (function, line 751) `std::string KoreanRuleG2p::g2p_single_fragment(std::string_view frag) const`
  - `load_korean_lexicon_stream` (function, line 774) `void load_korean_lexicon_stream(
    std::istream& in, std::unordered_map<std::string, std::strin...`
  - `KoreanRuleG2p` (function, line 803) `KoreanRuleG2p::KoreanRuleG2p(std::filesystem::path dict_tsv, Options options)
    : options_(std:...`
  - `KoreanRuleG2p` (function, line 817) `KoreanRuleG2p::KoreanRuleG2p(std::string dict_tsv_utf8, Options options)
    : options_(std::move...`
  - `text_to_ipa` (function, line 823) `std::string KoreanRuleG2p::text_to_ipa(std::string text,
                                       s...`
  - `dialect_ids` (function, line 1035) `std::vector<std::string> KoreanRuleG2p::dialect_ids()`
  - `dialect_resolves_to_korean_rules` (function, line 1040) `bool dialect_resolves_to_korean_rules(std::string_view dialect_id)`
  - `resolve_korean_dict_path` (function, line 1048) `std::filesystem::path resolve_korean_dict_path(
    const std::filesystem::path& model_root)`
  - `tmp` (function, line 73) `const std::string tmp(s);`
  - `utf8proc_NFC` (function, line 75) `utf8proc_NFC(reinterpret_cast<const utf8proc_uint8_t*>(tmp.c_str()));`
  - `string` (function, line 77) `return std::string(s);`
  - `out` (function, line 79) `std::string out(reinterpret_cast<char*>(p));`
  - `free` (function, line 80) `std::free(p);`
  - `utf8proc_NFD` (function, line 86) `utf8proc_NFD(reinterpret_cast<const utf8proc_uint8_t*>(ipa.c_str()));`
  - `nfd_str` (function, line 90) `const std::string nfd_str(reinterpret_cast<char*>(nfd));`
  - `utf8_append_codepoint` (function, line 102) `utf8_append_codepoint(filtered, cp);`
  - `composed` (function, line 109) `std::string composed(reinterpret_cast<char*>(nfc));`
  - `utf8_decode_at` (function, line 240) `utf8_decode_at(nfc, i, cp, adv);`
  - `trim_ascii_ws_copy` (function, line 790) `trim_ascii_ws_copy(std::string_view(line).substr(0, tab));`
  - `runtime_error` (function, line 807) `throw std::runtime_error("Korean G2P: lexicon not found at " + dict_tsv.generic_string());`
  - `in` (function, line 810) `std::ifstream in(dict_tsv);`
  - `LOGF` (function, line 904) `LOGF("ko g2p [%s] %s -> %s", path, grapheme.c_str(), ipa.c_str());`
  - `iss` (function, line 909) `std::istringstream iss(tokenizable);`
  - `log_mapping` (function, line 919) `log_mapping(w + " -> " + frag, stressed, "numeral");`
  - `num_sv` (function, line 985) `const std::string num_sv(w, 0, num_end);`
  - `0xAC00` (variable, line 19) `extern "C" { #include <utf8proc.h> } namespace moonshine_tts { namespace { constexpr char32_t kHangulBase = 0xAC00;`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/korean-numbers.h`, `core/moonshine-tts/src/lang-specific/korean.h`, `core/moonshine-tts/src/utf8-utils.h`, `core/moonshine-utils/debug-utils.h`

## core/moonshine-tts/src/lang-specific/korean.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_KOREAN_H define MOONSHINE_TTS_LANG_SPECIFIC_KOREAN_H  include <filesystem> include <s
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 15)
  - `Options` (struct, line 21)
  - `KoreanRuleG2p` (class, line 19)
  - `dialect_id` (function, line 34) `const std::string& dialect_id() const`
  - `KoreanRuleG2p` (function, line 26) `explicit KoreanRuleG2p(std::filesystem::path dict_tsv);`
  - `dialect_ids` (function, line 32) `static std::vector<std::string> dialect_ids();`
  - `normalize_korean_ipa` (function, line 43) `static std::string normalize_korean_ipa(std::string ipa, bool voice_lenis = true);`
  - `g2p_single_fragment` (function, line 54) `std::string g2p_single_fragment(std::string_view frag) const;`
  - `g2p_hangul_rules_only` (function, line 56) `std::string g2p_hangul_rules_only(std::string_view hangul) const;`
  - `extract_hangul` (function, line 57) `std::string extract_hangul(std::string_view s) const;`
  - `dialect_resolves_to_korean_rules` (function, line 59) `bool dialect_resolves_to_korean_rules(std::string_view dialect_id);`
  - `resolve_korean_dict_path` (function, line 63) `std::filesystem::path resolve_korean_dict_path( const std::filesystem::path& model_root);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_KOREAN_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_KOREAN_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/korean.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/korean-rule-g2p-test.cpp`, `core/moonshine-tts/tools/korean-rule-g2p-cli.cpp`

## core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp
- Layer: business_logic
- Doc: include "onnx-g2p-models.h"  include <nlohmann/json.h>  include <array> include <cstddef> include <filesystem> include <
- Language: cpp
- Symbols:
  - `open_session` (function, line 20) `Ort::Session open_session(Ort::Env& env,
                          const std::filesystem::path& m...`
  - `open_session_memory` (function, line 37) `Ort::Session open_session_memory(Ort::Env& env, const void* data, size_t len,
                   ...`
  - `encode_chars_for_model` (function, line 45) `std::vector<int64_t> encode_chars_for_model(
    const std::string& text,
    const std::unordere...`
  - `decoder_io_padded` (function, line 57) `void decoder_io_padded(const std::vector<int64_t>& cur, int max_phoneme_len,
                    ...`
  - `argmax_vocab_row` (function, line 72) `int argmax_vocab_row(const float* logits, int64_t vocab, int time_index)`
  - `OnnxOovG2p` (function, line 89) `OnnxOovG2p::OnnxOovG2p(Ort::Env& env, const std::filesystem::path& model_onnx,
                  ...`
  - `OnnxOovG2p` (function, line 96) `OnnxOovG2p::OnnxOovG2p(Ort::Env& env, const void* model_onnx_bytes,
                       size_t...`
  - `predict_phonemes` (function, line 105) `std::vector<std::string> OnnxOovG2p::predict_phonemes(const std::string& word)`
  - `Session` (function, line 27) `return Ort::Session( env, w.c_str(), make_g2p_ort_session_options(ort_providers, coreml_cache_dir));`
  - `runtime_error` (function, line 63) `throw std::runtime_error("decoder length > max_phoneme_len");`
  - `enc_ids` (function, line 115) `std::vector<int64_t> enc_ids(static_cast<size_t>(tab_.max_seq_len), tab_.pad_id);`
  - `enc_mask` (function, line 117) `std::vector<int64_t> enc_mask(static_cast<size_t>(tab_.max_seq_len), 0);`
- Depends on: `core/moonshine-tts/src/constants.h`, `core/moonshine-tts/src/lang-specific/onnx-g2p-models.h`, `core/moonshine-tts/src/ort-session-options.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/onnx-g2p-models.h
- Layer: business_logic
- Doc: ifndef MOONSHINE_TTS_ONNX_G2P_MODELS_H define MOONSHINE_TTS_ONNX_G2P_MODELS_H  include <nlohmann/json.h> include <onnxru
- Language: h
- Symbols:
  - `OnnxOovG2p` (class, line 17)
  - `predict_phonemes` (function, line 26) `std::vector<std::string> predict_phonemes(const std::string& word);`
  - `MOONSHINE_TTS_ONNX_G2P_MODELS_H` (macro, line 2) `#define MOONSHINE_TTS_ONNX_G2P_MODELS_H`
- Depends on: `core/moonshine-tts/src/json-config.h`
- Imported by: `core/moonshine-tts/src/lang-specific/english.cpp`, `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp`

## core/moonshine-tts/src/lang-specific/portuguese-rules.cpp
- Layer: business_logic
- Doc: include "portuguese-rules.h"  include <algorithm> include <cctype> include <cstdint> include <optional> include <string>
- Language: cpp
- Symbols:
  - `pt_tolower` (function, line 23) `char32_t pt_tolower(char32_t c)`
  - `is_pt_key_cp` (function, line 68) `bool is_pt_key_cp(char32_t c)`
  - `normalize_lookup_key_utf8_impl` (function, line 84) `std::string normalize_lookup_key_utf8_impl(const std::string& word)`
  - `normalize_lookup_key_utf8` (function, line 105) `std::string normalize_lookup_key_utf8(const std::string& word)`
  - `utf8_to_u32_pt` (function, line 109) `std::u32string utf8_to_u32_pt(const std::string& s)`
  - `u32_to_utf8_pt` (function, line 113) `std::string u32_to_utf8_pt(const std::u32string& s)`
  - `is_allowed_pt_grapheme` (function, line 121) `bool is_allowed_pt_grapheme(char32_t c)`
  - `filter_pt_word_graphemes_utf8` (function, line 134) `std::u32string filter_pt_word_graphemes_utf8(const std::string& word)`
  - `is_vowel_pt_u32` (function, line 150) `bool is_vowel_pt_u32(char32_t ch)`
  - `strip_accent_base_pt` (function, line 158) `char32_t strip_accent_base_pt(char32_t c)`
  - `should_hiatus_pt_u32` (function, line 185) `bool should_hiatus_pt_u32(char32_t a, char32_t b)`
  - `valid_onset2_end_u32` (function, line 260) `bool valid_onset2_end_u32(char32_t a, char32_t b)`
  - `port_orthographic_syllables_u32` (function, line 296) `std::vector<std::u32string> port_orthographic_syllables_u32(
    const std::u32string& w0)`
  - `accented_syllable_u32` (function, line 351) `bool accented_syllable_u32(const std::u32string& s)`
  - `default_stressed_syllable_index_u32` (function, line 361) `size_t default_stressed_syllable_index_u32(
    const std::vector<std::u32string>& syls, const st...`
  - `strip_stress_chars` (function, line 423) `std::string strip_stress_chars(std::string s)`
  - `insert_primary_stress_before_vowel_utf8` (function, line 429) `std::string insert_primary_stress_before_vowel_utf8(std::string ipa)`
  - `roman_to_int_ascii` (function, line 452) `std::optional<int> roman_to_int_ascii(std::string_view u)`
  - `roman_numeral_token_to_ipa` (function, line 490) `std::optional<std::string> roman_numeral_token_to_ipa(
    const std::string& letters_lower, bool...`
  - `prev_global_vowel_u32` (function, line 548) `bool prev_global_vowel_u32(const std::u32string& full_word, size_t gidx)`
  - `next_global_vowel_u32` (function, line 568) `bool next_global_vowel_u32(const std::u32string& full_word, size_t gidx)`
  - `syllable_has_u32` (function, line 584) `bool syllable_has_u32(const std::u32string& s, char32_t ch)`
  - `letters_to_ipa_no_stress_u32` (function, line 588) `std::string letters_to_ipa_no_stress_u32(const std::u32string& s, bool is_pt_pt,
                ...`
  - `rules_word_to_ipa_single_u32` (function, line 963) `std::string rules_word_to_ipa_single_u32(const std::u32string& wl,
                              ...`
  - `vowel_grapheme_tail_pt` (function, line 1017) `bool vowel_grapheme_tail_pt(char32_t c)`
  - `pt_pt_apply_rules_final_s_to_esh` (function, line 1025) `std::string pt_pt_apply_rules_final_s_to_esh(std::string ipa,
                                   ...`
  - `rules_word_to_ipa_utf8` (function, line 1160) `std::string rules_word_to_ipa_utf8(const std::string& raw, bool is_pt_pt,
                       ...`
  - `utf8_decode_at` (function, line 91) `moonshine_tts::utf8_decode_at(word, i, cp, adv);`
  - `utf8_append_codepoint` (function, line 97) `moonshine_tts::utf8_append_codepoint(out, cl);`
  - `utf8_str_to_u32` (function, line 111) `return moonshine_tts::utf8_str_to_u32(s);`
  - `erase_utf8_substr` (function, line 425) `moonshine_tts::erase_utf8_substr(s, kPri);`
  - `s` (function, line 454) `std::string s(u);`
  - `unstressed_vowel` (function, line 672) `return unstressed_vowel(U'i');`
  - `fw_pt_map_impl` (function, line 1212) `return fw_pt_map_impl();`
  - `fw_br_map_impl` (function, line 1216) `return fw_br_map_impl();`
  - `sc_straddle_map_impl` (function, line 1220) `return sc_straddle_map_impl();`
- Depends on: `core/moonshine-tts/src/lang-specific/ipa-symbols.h`, `core/moonshine-tts/src/lang-specific/portuguese-rules.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/portuguese-rules.h
- Layer: business_logic
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_PORTUGUESE_RULES_H define MOONSHINE_TTS_LANG_SPECIFIC_PORTUGUESE_RULES_H  include <cs
- Language: h
- Symbols:
  - `pt_tolower` (function, line 10) `char32_t pt_tolower(char32_t c);`
  - `normalize_lookup_key_utf8` (function, line 12) `std::string normalize_lookup_key_utf8(const std::string& word);`
  - `roman_numeral_token_to_ipa` (function, line 13) `std::optional<std::string> roman_numeral_token_to_ipa( const std::string& letters_lower, bool is_pt_pt);`
  - `rules_word_to_ipa_utf8` (function, line 16) `std::string rules_word_to_ipa_utf8(const std::string& raw, bool is_pt_pt, bool with_stress);`
  - `pt_pt_apply_rules_final_s_to_esh` (function, line 18) `std::string pt_pt_apply_rules_final_s_to_esh(std::string ipa, const std::string& letters_key);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_PORTUGUESE_RULES_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_PORTUGUESE_RULES_H`
- Imported by: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp`, `core/moonshine-tts/src/lang-specific/portuguese.cpp`

## core/moonshine-tts/src/lang-specific/portuguese.cpp
- Layer: testing
- Doc: include "portuguese.h"  include <algorithm> include <cctype> include <clocale> include <cstdint> include <cwctype> inclu
- Language: cpp
- Symbols:
  - `utf8_lowercase_pt_surface` (function, line 38) `std::string utf8_lowercase_pt_surface(const std::string& word)`
  - `load_pt_lexicon_stream` (function, line 51) `void load_pt_lexicon_stream(std::istream& in,
                            std::unordered_map<std:...`
  - `load_pt_lexicon_file` (function, line 83) `void load_pt_lexicon_file(const std::filesystem::path& path,
                          std::unord...`
  - `is_all_ascii_digits` (function, line 96) `bool is_all_ascii_digits(std::string_view s)`
  - `teens_word_pt` (function, line 120) `std::string teens_word_pt(int n, bool is_pt_pt)`
  - `under_100_tokens_pt` (function, line 172) `void under_100_tokens_pt(int n, bool is_pt_pt, std::vector<std::string>& out)`
  - `below_1000_tokens_pt` (function, line 199) `void below_1000_tokens_pt(int n, bool is_pt_pt, std::vector<std::string>& out)`
  - `below_1_000_000_tokens_pt` (function, line 227) `void below_1_000_000_tokens_pt(int n, bool is_pt_pt,
                               std::vector<s...`
  - `expand_cardinal_digits_to_portuguese_words` (function, line 251) `std::string expand_cardinal_digits_to_portuguese_words(std::string_view s,
                      ...`
  - `expand_digit_tokens_in_text` (function, line 288) `std::string expand_digit_tokens_in_text(std::string text, bool is_pt_pt)`
  - `is_pt_word_char` (function, line 321) `bool is_pt_word_char(char32_t cp)`
  - `try_consume_pt_word` (function, line 354) `bool try_consume_pt_word(const std::string& text, size_t pos, size_t& out_end)`
  - `PortugueseRuleG2p` (function, line 410) `PortugueseRuleG2p::PortugueseRuleG2p(std::filesystem::path dict_tsv,
                            ...`
  - `PortugueseRuleG2p` (function, line 417) `PortugueseRuleG2p::PortugueseRuleG2p(std::string dict_tsv_utf8,
                                 ...`
  - `finalize_ipa` (function, line 425) `std::string PortugueseRuleG2p::finalize_ipa(std::string ipa,
                                    ...`
  - `lookup_or_rules` (function, line 444) `std::string PortugueseRuleG2p::lookup_or_rules(
    const std::string& raw_word) const`
  - `word_to_ipa` (function, line 507) `std::string PortugueseRuleG2p::word_to_ipa(const std::string& word) const`
  - `text_to_ipa_no_expand` (function, line 530) `std::string PortugueseRuleG2p::text_to_ipa_no_expand(
    const std::string& text, std::vector<G2...`
  - `text_to_ipa` (function, line 600) `std::string PortugueseRuleG2p::text_to_ipa(
    std::string text, std::vector<G2pWordLog>* per_wo...`
  - `dialect_resolves_to_portugal_rules` (function, line 608) `bool dialect_resolves_to_portugal_rules(std::string_view dialect_id)`
  - `dialect_resolves_to_brazilian_portuguese_rules` (function, line 617) `bool dialect_resolves_to_brazilian_portuguese_rules(
    std::string_view dialect_id)`
  - `dialect_ids` (function, line 627) `std::vector<std::string> PortugueseRuleG2p::dialect_ids()`
  - `resolve_portuguese_dict_path` (function, line 634) `std::filesystem::path resolve_portuguese_dict_path(
    const std::filesystem::path& model_root, ...`
  - `utf8_decode_at` (function, line 45) `utf8_decode_at(word, i, cp, adv);`
  - `utf8_append_codepoint` (function, line 46) `utf8_append_codepoint(out, portuguese_rules::pt_tolower(cp));`
  - `in` (function, line 86) `std::ifstream in(path);`
  - `runtime_error` (function, line 88) `throw std::runtime_error("Portuguese G2P: cannot read lexicon " + path.generic_string());`
  - `out_of_range` (function, line 123) `throw std::out_of_range("teens");`
  - `string` (function, line 255) `return std::string(s);`
  - `range_re` (function, line 290) `static const std::regex range_re(R"(\b(\d+)-(\d+)\b)", std::regex::ECMAScript);`
  - `dig_re` (function, line 292) `static const std::regex dig_re(R"(\b\d+\b)", std::regex::ECMAScript);`
  - `it` (function, line 294) `std::sregex_iterator it(text.begin(), text.end(), range_re);`
  - `it2` (function, line 310) `std::sregex_iterator it2(text.begin(), text.end(), dig_re);`
  - `erase_utf8_substr` (function, line 429) `erase_utf8_substr(ipa, kPri);`
  - `normalize_lookup_key_utf8` (function, line 448) `portuguese_rules::normalize_lookup_key_utf8(raw_word);`
  - `roman_numeral_token_to_ipa` (function, line 453) `portuguese_rules::roman_numeral_token_to_ipa(letters_only, is_portugal_);`
  - `trim_ascii_ws_copy` (function, line 499) `trim_ascii_ws_copy(raw_word), is_portugal_, options_.with_stress);`
  - `move` (function, line 503) `std::move(ipa_rules), letters_only);`
  - `dig_pass` (function, line 522) `static const std::regex dig_pass(R"(^[0-9]+(?:-[0-9]+)*$)", std::regex::ECMAScript);`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/german.h`, `core/moonshine-tts/src/lang-specific/ipa-symbols.h`, `core/moonshine-tts/src/lang-specific/portuguese-rules.h`, `core/moonshine-tts/src/lang-specific/portuguese.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/portuguese.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_PORTUGUESE_H define MOONSHINE_TTS_LANG_SPECIFIC_PORTUGUESE_H  include <filesystem> in
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 14)
  - `Options` (struct, line 20)
  - `PortugueseRuleG2p` (class, line 18)
  - `is_portugal` (function, line 37) `bool is_portugal() const`
  - `dialect_id` (function, line 39) `const std::string& dialect_id() const`
  - `PortugueseRuleG2p` (function, line 27) `explicit PortugueseRuleG2p(std::filesystem::path dict_tsv, bool is_portugal);`
  - `dialect_ids` (function, line 35) `static std::vector<std::string> dialect_ids();`
  - `word_to_ipa` (function, line 40) `std::string word_to_ipa(const std::string& word) const;`
  - `lookup_or_rules` (function, line 52) `std::string lookup_or_rules(const std::string& raw_word) const;`
  - `finalize_ipa` (function, line 54) `std::string finalize_ipa(std::string ipa, bool from_lexicon) const;`
  - `text_to_ipa_no_expand` (function, line 55) `std::string text_to_ipa_no_expand( const std::string& text, std::vector<G2pWordLog>* per_word_log) const;`
  - `dialect_resolves_to_portugal_rules` (function, line 61) `bool dialect_resolves_to_portugal_rules(std::string_view dialect_id);`
  - `dialect_resolves_to_brazilian_portuguese_rules` (function, line 64) `bool dialect_resolves_to_brazilian_portuguese_rules( std::string_view dialect_id);`
  - `resolve_portuguese_dict_path` (function, line 69) `std::filesystem::path resolve_portuguese_dict_path( const std::filesystem::path& model_root, bool is_portugal);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_PORTUGUESE_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_PORTUGUESE_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/portuguese.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp`, `core/moonshine-tts/tools/portuguese-rule-g2p-cli.cpp`

## core/moonshine-tts/src/lang-specific/russian-numbers.cpp
- Layer: testing
- Doc: Russian cardinal expansion (russian_numbers.py). #include from russian.cpp (same TU).  include <regex> include <stdexcep
- Language: cpp
- Symbols:
  - `ru_ascii_all_digits` (function, line 13) `bool ru_ascii_all_digits(std::string_view s)`
  - `ru_ones_digit` (function, line 98) `std::string ru_ones_digit(int n, bool feminine)`
  - `ru_append_under_100` (function, line 113) `void ru_append_under_100(int n, bool feminine, std::vector<std::string>& out)`
  - `ru_append_cardinal_1_to_999` (function, line 133) `void ru_append_cardinal_1_to_999(int n, bool feminine,
                                 std::vect...`
  - `ru_thousand_suffix` (function, line 150) `const char* ru_thousand_suffix(int q)`
  - `ru_append_below_1_000_000` (function, line 165) `void ru_append_below_1_000_000(int n, std::vector<std::string>& out)`
  - `expand_cardinal_digits_to_russian_words` (function, line 182) `std::string expand_cardinal_digits_to_russian_words(std::string_view s)`
  - `expand_russian_digit_tokens_in_text` (function, line 219) `std::string expand_russian_digit_tokens_in_text(std::string text)`
  - `out_of_range` (function, line 101) `throw std::out_of_range("ru_ones_digit");`
  - `string` (function, line 185) `return std::string(s);`
  - `range_re` (function, line 221) `static const std::regex range_re(R"(\b(\d+)-(\d+)\b)", std::regex::ECMAScript);`
  - `dig_re` (function, line 223) `static const std::regex dig_re(R"(\b\d+\b)", std::regex::ECMAScript);`
  - `it` (function, line 225) `std::sregex_iterator it(text.begin(), text.end(), range_re);`
  - `it2` (function, line 250) `std::sregex_iterator it2(text.begin(), text.end(), dig_re);`
- Depends on: `core/moonshine-tts/src/utf8-utils.h`
- Imported by: `core/moonshine-tts/src/lang-specific/russian.cpp`

## core/moonshine-tts/src/lang-specific/russian.cpp
- Layer: testing
- Doc: include "russian.h"  include <algorithm> include <cctype> include <cstdint> include <cwctype> include <fstream> include 
- Language: cpp
- Symbols:
  - `is_unicode_mn` (function, line 36) `bool is_unicode_mn(char32_t cp)`
  - `is_combining_mark` (function, line 55) `bool is_combining_mark(char32_t cp)`
  - `russian_tolower_cp` (function, line 57) `char32_t russian_tolower_cp(char32_t c)`
  - `is_russian_vowel_letter` (function, line 67) `bool is_russian_vowel_letter(char32_t c)`
  - `is_russian_lex_key_cp` (function, line 75) `bool is_russian_lex_key_cp(char32_t c)`
  - `append_nfd_expansion` (function, line 125) `void append_nfd_expansion(char32_t cp, std::u32string& out)`
  - `u32_to_utf8` (function, line 135) `std::string u32_to_utf8(const std::u32string& s)`
  - `unicode_tolower_like_python` (function, line 143) `char32_t unicode_tolower_like_python(char32_t cp)`
  - `normalize_lookup_key_utf8` (function, line 163) `std::string normalize_lookup_key_utf8(const std::string& word)`
  - `utf8_russian_lowercase` (function, line 193) `std::string utf8_russian_lowercase(const std::string& word)`
  - `surface_is_all_lowercase_russian` (function, line 211) `bool surface_is_all_lowercase_russian(const std::string& surf)`
  - `load_russian_lexicon_stream` (function, line 215) `void load_russian_lexicon_stream(
    std::istream& in, std::unordered_map<std::string, std::stri...`
  - `load_russian_lexicon_file` (function, line 247) `void load_russian_lexicon_file(
    const std::filesystem::path& path,
    std::unordered_map<std...`
  - `filter_russian_graphemes_keep_stress` (function, line 258) `std::string filter_russian_graphemes_keep_stress(std::string_view raw)`
  - `strip_grapheme_diacritics_utf8` (function, line 280) `std::string strip_grapheme_diacritics_utf8(std::string_view sv)`
  - `acute_stressed_vowel_ordinal` (function, line 304) `std::optional<int> acute_stressed_vowel_ordinal(const std::string& w_nfc)`
  - `vowel_ordinal_to_syllable` (function, line 335) `int vowel_ordinal_to_syllable(const std::vector<std::string>& syls,
                             ...`
  - `russian_orthographic_syllables_utf8` (function, line 356) `std::vector<std::string> russian_orthographic_syllables_utf8(
    const std::string& word_lower)`
  - `remove_if` (function, line 423) `std::remove_if(syllables.begin(), syllables.end(),
                     [](const std::string& x)`
  - `stress_syllable_index` (function, line 428) `int stress_syllable_index(const std::vector<std::string>& syls,
                          const s...`
  - `syllable_index_per_codepoint` (function, line 452) `std::vector<int> syllable_index_per_codepoint(const std::string& w)`
  - `palatalizable_cons` (function, line 464) `bool palatalizable_cons(char32_t ch)`
  - `emit_consonant` (function, line 472) `std::string emit_consonant(char32_t ch, bool palatal)`
  - `ipa_piece_ends_with_palatal` (function, line 524) `bool ipa_piece_ends_with_palatal(const std::string& piece)`
  - `ipa_piece_last_is_vowel_letter` (function, line 533) `bool ipa_piece_last_is_vowel_letter(const std::string& piece)`
  - `ipa_piece_after_hard_consonant` (function, line 546) `bool ipa_piece_after_hard_consonant(const std::string& piece)`
  - `vowel_ipa` (function, line 559) `std::string vowel_ipa(char32_t ch, bool stressed, bool after_palatal,
                      bool ...`
  - `letters_to_ipa_rules` (function, line 619) `std::string letters_to_ipa_rules(const std::string& w_clean, int stress_syl)`
  - `insert_primary_stress_before_vowel` (function, line 788) `std::string insert_primary_stress_before_vowel(std::string s)`
  - `rules_word_to_ipa_single` (function, line 808) `std::string rules_word_to_ipa_single(const std::string& w_clean,
                                ...`
  - `rules_word_to_ipa` (function, line 820) `std::string rules_word_to_ipa(const std::string& raw, bool with_stress)`
  - `is_latin1_supplement_python_word_char` (function, line 885) `bool is_latin1_supplement_python_word_char(char32_t cp)`
  - `is_unicode_word_char_w` (function, line 906) `bool is_unicode_word_char_w(char32_t cp)`
  - `utf8_contains_cyrillic` (function, line 931) `bool utf8_contains_cyrillic(const std::string& tok)`
  - `try_consume_unicode_word` (function, line 945) `bool try_consume_unicode_word(const std::string& text, size_t pos,
                              ...`
  - `normalize_russian_fleeting_palatal_markers_utf8` (function, line 976) `std::string normalize_russian_fleeting_palatal_markers_utf8(std::string ipa)`
  - `RussianRuleG2p` (function, line 992) `RussianRuleG2p::RussianRuleG2p(std::filesystem::path dict_tsv, Options options)
    : options_(op...`
  - `RussianRuleG2p` (function, line 997) `RussianRuleG2p::RussianRuleG2p(std::string dict_tsv_utf8, Options options)
    : options_(options)`
  - `finalize_ipa` (function, line 1003) `std::string RussianRuleG2p::finalize_ipa(std::string ipa) const`
  - `lookup_or_rules` (function, line 1017) `std::string RussianRuleG2p::lookup_or_rules(const std::string& raw_word) const`
  - `word_to_ipa` (function, line 1060) `std::string RussianRuleG2p::word_to_ipa(const std::string& word) const`
  - `text_to_ipa_no_expand` (function, line 1082) `std::string RussianRuleG2p::text_to_ipa_no_expand(
    const std::string& text, std::vector<G2pWo...`
  - `text_to_ipa` (function, line 1156) `std::string RussianRuleG2p::text_to_ipa(std::string text,
                                       ...`
  - `dialect_resolves_to_russian_rules` (function, line 1164) `bool dialect_resolves_to_russian_rules(std::string_view dialect_id)`
  - `dialect_ids` (function, line 1172) `std::vector<std::string> RussianRuleG2p::dialect_ids()`
  - `resolve_russian_dict_path` (function, line 1176) `std::filesystem::path resolve_russian_dict_path(
    const std::filesystem::path& model_root)`
  - `utf8_append_codepoint` (function, line 139) `utf8_append_codepoint(out, cp);`
  - `utf8_decode_at` (function, line 170) `utf8_decode_at(trimmed, i, cp, adv);`
  - `in` (function, line 251) `std::ifstream in(path);`
  - `runtime_error` (function, line 253) `throw std::runtime_error("Russian G2P: cannot read lexicon " + path.generic_string());`
  - `erase_utf8_substr` (function, line 790) `erase_utf8_substr(s, kPri);`
  - `normalize_russian_ipa_piper_style` (function, line 1009) `return normalize_russian_ipa_piper_style(std::move(ipa));`
  - `dig_pass` (function, line 1074) `static const std::regex dig_pass(R"(^[0-9]+(?:-[0-9]+)*$)", std::regex::ECMAScript);`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/ipa-postprocess.h`, `core/moonshine-tts/src/lang-specific/german.h`, `core/moonshine-tts/src/lang-specific/ipa-symbols.h`, `core/moonshine-tts/src/lang-specific/russian-numbers.cpp`, `core/moonshine-tts/src/lang-specific/russian.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/russian.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_RUSSIAN_H define MOONSHINE_TTS_LANG_SPECIFIC_RUSSIAN_H  include <filesystem> include 
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 14)
  - `Options` (struct, line 19)
  - `RussianRuleG2p` (class, line 17)
  - `dialect_id` (function, line 36) `const std::string& dialect_id() const`
  - `RussianRuleG2p` (function, line 28) `explicit RussianRuleG2p(std::filesystem::path dict_tsv);`
  - `dialect_ids` (function, line 34) `static std::vector<std::string> dialect_ids();`
  - `word_to_ipa` (function, line 38) `std::string word_to_ipa(const std::string& word) const;`
  - `lookup_or_rules` (function, line 49) `std::string lookup_or_rules(const std::string& raw_word) const;`
  - `finalize_ipa` (function, line 51) `std::string finalize_ipa(std::string ipa) const;`
  - `text_to_ipa_no_expand` (function, line 52) `std::string text_to_ipa_no_expand( const std::string& text, std::vector<G2pWordLog>* per_word_log) const;`
  - `dialect_resolves_to_russian_rules` (function, line 57) `bool dialect_resolves_to_russian_rules(std::string_view dialect_id);`
  - `resolve_russian_dict_path` (function, line 61) `std::filesystem::path resolve_russian_dict_path( const std::filesystem::path& model_root);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_RUSSIAN_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_RUSSIAN_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/russian.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/russian-rule-g2p-test.cpp`

## core/moonshine-tts/src/lang-specific/spanish-numbers.cpp
- Layer: testing
- Doc: Spanish cardinal expansion (spanish_numbers.py). #include from spanish.cpp (same TU).  include <regex> include <stdexcep
- Language: cpp
- Symbols:
  - `es_ascii_all_digits` (function, line 13) `bool es_ascii_all_digits(std::string_view s)`
  - `es_append_under_100` (function, line 76) `void es_append_under_100(int n, std::vector<std::string>& out)`
  - `es_append_below_1000` (function, line 97) `void es_append_below_1000(int n, std::vector<std::string>& out)`
  - `es_append_below_1_000_000` (function, line 122) `void es_append_below_1_000_000(int n, std::vector<std::string>& out)`
  - `expand_cardinal_digits_to_spanish_words` (function, line 143) `std::string expand_cardinal_digits_to_spanish_words(std::string_view s)`
  - `expand_spanish_digit_tokens_in_text` (function, line 179) `std::string expand_spanish_digit_tokens_in_text(std::string text)`
  - `out_of_range` (function, line 79) `throw std::out_of_range("es_append_under_100");`
  - `string` (function, line 146) `return std::string(s);`
  - `range_re` (function, line 181) `static const std::regex range_re(R"(\b(\d+)-(\d+)\b)", std::regex::ECMAScript);`
  - `dig_re` (function, line 183) `static const std::regex dig_re(R"(\b\d+\b)", std::regex::ECMAScript);`
  - `it` (function, line 185) `std::sregex_iterator it(text.begin(), text.end(), range_re);`
  - `it2` (function, line 210) `std::sregex_iterator it2(text.begin(), text.end(), dig_re);`
- Depends on: `core/moonshine-tts/src/utf8-utils.h`
- Imported by: `core/moonshine-tts/src/lang-specific/spanish.cpp`

## core/moonshine-tts/src/lang-specific/spanish-unicode-tables.cpp
- Layer: testing
- Doc: include "spanish-unicode-tables.h"
- Language: cpp
- Depends on: `core/moonshine-tts/src/lang-specific/spanish-unicode-tables.h`

## core/moonshine-tts/src/lang-specific/spanish-unicode-tables.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_SPANISH_UNICODE_TABLES_H define MOONSHINE_TTS_LANG_SPECIFIC_SPANISH_UNICODE_TABLES_H 
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
- Doc: include "spanish-unicode.h"  include <algorithm> include <string>  include "spanish-unicode-tables.h" include "utf8-util
- Language: cpp
- Symbols:
  - `lookup_sorted_pair` (function, line 11) `const char* lookup_sorted_pair(const std::pair<char32_t, const char*>* table,
                   ...`
  - `lower_bound` (function, line 17) `std::lower_bound(first, last, key,
                       [](const std::pair<char32_t, const char...`
  - `unicode_bitmap_get` (function, line 25) `bool unicode_bitmap_get(const std::uint32_t* bitmap, std::uint32_t nwords,
                      ...`
  - `utf32_to_utf8` (function, line 39) `std::string utf32_to_utf8(const std::u32string& u)`
  - `utf8_to_utf32` (function, line 48) `std::u32string utf8_to_utf32(const std::string& s)`
  - `unicode_lower_utf8` (function, line 52) `std::string unicode_lower_utf8(const std::string& s)`
  - `strip_accents_utf8` (function, line 71) `std::string strip_accents_utf8(const std::string& s)`
  - `word_key` (function, line 90) `std::string word_key(const std::string& wraw)`
  - `is_word_char` (function, line 94) `bool is_word_char(char32_t cp)`
  - `is_space_char` (function, line 99) `bool is_space_char(char32_t cp)`
  - `strip_replacement_utf8` (function, line 104) `const char* strip_replacement_utf8(char32_t cp)`
  - `utf8_append_codepoint` (function, line 44) `utf8_append_codepoint(out, cp);`
  - `utf8_str_to_u32` (function, line 50) `return utf8_str_to_u32(s);`
  - `utf8_decode_at` (function, line 59) `utf8_decode_at(s, i, cp, adv);`
- Depends on: `core/moonshine-tts/src/lang-specific/spanish-unicode-tables.h`, `core/moonshine-tts/src/lang-specific/spanish-unicode.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/spanish-unicode.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_SPANISH_UNICODE_H define MOONSHINE_TTS_LANG_SPECIFIC_SPANISH_UNICODE_H  include <cstd
- Language: h
- Symbols:
  - `utf32_to_utf8` (function, line 8) `std::string utf32_to_utf8(const std::u32string& u);`
  - `utf8_to_utf32` (function, line 10) `std::u32string utf8_to_utf32(const std::string& s);`
  - `unicode_lower_utf8` (function, line 11) `std::string unicode_lower_utf8(const std::string& s);`
  - `strip_accents_utf8` (function, line 12) `std::string strip_accents_utf8(const std::string& s);`
  - `word_key` (function, line 13) `std::string word_key(const std::string& wraw);`
  - `is_word_char` (function, line 14) `bool is_word_char(char32_t cp);`
  - `is_space_char` (function, line 15) `bool is_space_char(char32_t cp);`
  - `strip_replacement_utf8` (function, line 17) `const char* strip_replacement_utf8(char32_t cp);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_SPANISH_UNICODE_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_SPANISH_UNICODE_H`
- Imported by: `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp`, `core/moonshine-tts/src/lang-specific/spanish.cpp`

## core/moonshine-tts/src/lang-specific/spanish.cpp
- Layer: testing
- Doc: include "spanish.h"  include <algorithm> include <cctype> include <cstdint> include <regex> include <stdexcept> include 
- Language: cpp
- Symbols:
  - `XExc` (struct, line 264)
  - `is_vowel_ch` (function, line 22) `bool is_vowel_ch(char32_t ch)`
  - `should_hiatus` (function, line 42) `bool should_hiatus(char32_t a, char32_t b)`
  - `is_valid_onset2` (function, line 144) `bool is_valid_onset2(char32_t a, char32_t b)`
  - `clean_syllable_word` (function, line 177) `std::u32string clean_syllable_word(const std::u32string &word_lower)`
  - `orthographic_syllables_utf8` (function, line 188) `std::vector<std::string> orthographic_syllables_utf8(
    const std::string &word_lower_utf8)`
  - `default_stressed_syllable_index_v2` (function, line 225) `size_t default_stressed_syllable_index_v2(const std::u32string &w_clean_lower)`
  - `lookup_x_exception` (function, line 294) `const char *lookup_x_exception(const std::string &wkey)`
  - `apply_nasal_assimilation` (function, line 303) `std::string apply_nasal_assimilation(std::string s,
                                     const Sp...`
  - `insert_primary_stress_before_vowel` (function, line 332) `std::string insert_primary_stress_before_vowel(const std::string &ipa)`
  - `count_primary_stress_utf8` (function, line 355) `size_t count_primary_stress_utf8(const std::string &ipa)`
  - `ipa_stress_at_start` (function, line 370) `bool ipa_stress_at_start(const std::string &ipa)`
  - `apply_narrow_intervocalic_obstruents` (function, line 379) `std::string apply_narrow_intervocalic_obstruents(std::string ipa)`
  - `apply_coda_s_weakening` (function, line 416) `std::string apply_coda_s_weakening(std::string ipa,
                                   SpanishDia...`
  - `postprocess_lexical_ipa` (function, line 431) `std::string postprocess_lexical_ipa(std::string ipa,
                                    const Sp...`
  - `prev_phoneme_was_vowel` (function, line 457) `bool prev_phoneme_was_vowel(const std::vector<std::string> &out)`
  - `y_is_consonant` (function, line 469) `bool y_is_consonant(const std::u32string &letters_lower, size_t i)`
  - `to_lower_cp` (function, line 495) `char32_t to_lower_cp(char32_t c)`
  - `letters_to_ipa_no_stress` (function, line 503) `std::string letters_to_ipa_no_stress(const std::u32string &syl_lower,
                           ...`
  - `filter_word_letters_utf32` (function, line 772) `std::u32string filter_word_letters_utf32(const std::string &wraw)`
  - `make_common` (function, line 790) `SpanishDialect make_common(const std::string &id, std::string ce_ci_z_ipa,
                      ...`
  - `spanish_dialect_cli_ids` (function, line 815) `std::vector<std::string> spanish_dialect_cli_ids()`
  - `dialect_ids` (function, line 822) `std::vector<std::string> SpanishRuleG2p::dialect_ids()`
  - `spanish_dialect_from_cli_id` (function, line 826) `SpanishDialect spanish_dialect_from_cli_id(
    const std::string &cli_id, bool narrow_intervocal...`
  - `SpanishRuleG2p` (function, line 928) `SpanishRuleG2p::SpanishRuleG2p(SpanishDialect dialect, bool with_stress,
                        ...`
  - `word_to_ipa` (function, line 934) `std::string SpanishRuleG2p::word_to_ipa(const std::string &word) const`
  - `text_to_ipa_no_expand` (function, line 1002) `std::string SpanishRuleG2p::text_to_ipa_no_expand(
    const std::string &text, std::vector<G2pWo...`
  - `text_to_ipa` (function, line 1086) `std::string SpanishRuleG2p::text_to_ipa(std::string text,
                                       ...`
  - `spanish_word_to_ipa` (function, line 1094) `std::string spanish_word_to_ipa(const std::string &word,
                                const Sp...`
  - `spanish_text_to_ipa` (function, line 1101) `std::string spanish_text_to_ipa(const std::string &text,
                                const Sp...`
  - `tmp` (function, line 62) `std::string tmp(r);`
  - `utf32_to_utf8` (function, line 250) `spanish_unicode::utf32_to_utf8(std::u32string(1, w_clean_lower.back())));`
  - `string` (function, line 353) `return std::string("\xcb\x88") + spanish_unicode::utf32_to_utf8(no);`
  - `utf8_decode_at` (function, line 362) `utf8_decode_at(ipa, i, cp, adv);`
  - `utf8_append_codepoint` (function, line 498) `utf8_append_codepoint(tmp, c);`
  - `dedupe_dialect_ids_preserve_first` (function, line 824) `return dedupe_dialect_ids_preserve_first(spanish_dialect_cli_ids());`
  - `invalid_argument` (function, line 839) `throw std::invalid_argument("empty dialect id");`
  - `dig_pass` (function, line 957) `static const std::regex dig_pass(R"(^[0-9]+$)", std::regex::ECMAScript);`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/spanish-numbers.cpp`, `core/moonshine-tts/src/lang-specific/spanish-unicode.h`, `core/moonshine-tts/src/lang-specific/spanish.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/spanish.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_SPANISH_H define MOONSHINE_TTS_LANG_SPECIFIC_SPANISH_H  include <string> include <vec
- Language: h
- Symbols:
  - `SpanishDialect` (struct, line 13)
  - `CodaS` (enum, line 26)
  - `CodaS` (class, line 26)
  - `SpanishRuleG2p` (class, line 30)
  - `dialect` (function, line 36) `const SpanishDialect& dialect() const`
  - `with_stress` (function, line 38) `bool with_stress() const`
  - `expand_cardinal_digits` (function, line 39) `bool expand_cardinal_digits() const`
  - `SpanishRuleG2p` (function, line 31) `public: SpanishRuleG2p(SpanishDialect dialect, bool with_stress, bool expand_cardinal_digits = true);`
  - `dialect_ids` (function, line 34) `static std::vector<std::string> dialect_ids();`
  - `word_to_ipa` (function, line 43) `std::string word_to_ipa(const std::string& word) const;`
  - `text_to_ipa_no_expand` (function, line 53) `std::string text_to_ipa_no_expand( const std::string& text, std::vector<G2pWordLog>* per_word_log) const;`
  - `spanish_dialect_cli_ids` (function, line 59) `std::vector<std::string> spanish_dialect_cli_ids();`
  - `spanish_dialect_from_cli_id` (function, line 62) `SpanishDialect spanish_dialect_from_cli_id( const std::string& cli_id, bool narrow_intervocalic_obstruents = true);`
  - `spanish_word_to_ipa` (function, line 67) `std::string spanish_word_to_ipa(const std::string& word, const SpanishDialect& dialect, bool with_stress = true, bool expand_cardinal_digits = true);`
  - `spanish_text_to_ipa` (function, line 75) `std::string spanish_text_to_ipa(const std::string& text, const SpanishDialect& dialect, bool with_stress = true, std::vector<G2pWordLog>* per_word_log = nullptr, bool expand_cardinal_digits = true);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_SPANISH_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_SPANISH_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/spanish.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/spanish-rule-g2p-test.cpp`, `core/moonshine-tts/tools/moonshine-g2p-cli.cpp`

## core/moonshine-tts/src/lang-specific/turkish.cpp
- Layer: testing
- Doc: include "turkish.h"  include "g2p-word-log.h" include "utf8-utils.h"
- Language: cpp
- Symbols:
  - `is_all_ascii_digits` (function, line 24) `bool is_all_ascii_digits(std::string_view s)`
  - `append_under_100` (function, line 45) `void append_under_100(int n, std::vector<std::string>& out)`
  - `append_tokens_0_999` (function, line 70) `void append_tokens_0_999(int n, std::vector<std::string>& out)`
  - `append_below_1_000_000` (function, line 94) `void append_below_1_000_000(int n, std::vector<std::string>& out)`
  - `join_space` (function, line 115) `std::string join_space(const std::vector<std::string>& p)`
  - `expand_cardinal_digits_to_turkish_words` (function, line 126) `std::string expand_cardinal_digits_to_turkish_words(std::string_view s)`
  - `expand_turkish_digit_tokens_in_text` (function, line 160) `std::string expand_turkish_digit_tokens_in_text(std::string text)`
  - `utf8_to_u32_nfc` (function, line 195) `std::u32string utf8_to_u32_nfc(const std::string& s)`
  - `turkish_tolower_cp` (function, line 206) `char32_t turkish_tolower_cp(char32_t cp)`
  - `turkish_lower_u32` (function, line 217) `std::u32string turkish_lower_u32(const std::u32string& s)`
  - `is_tr_g2p_letter` (function, line 226) `bool is_tr_g2p_letter(char32_t c)`
  - `letters_only_u32` (function, line 271) `std::u32string letters_only_u32(const std::u32string& w)`
  - `is_vowel_orth` (function, line 284) `bool is_vowel_orth(char32_t c)`
  - `is_front_vowel` (function, line 290) `bool is_front_vowel(char32_t c)`
  - `prev_letter_index` (function, line 295) `std::optional<size_t> prev_letter_index(const std::u32string& w, size_t i)`
  - `next_letter_index` (function, line 305) `std::optional<size_t> next_letter_index(const std::u32string& w, size_t i)`
  - `next_vowel_from` (function, line 315) `std::optional<char32_t> next_vowel_from(const std::u32string& w, size_t start)`
  - `last_vowel_before` (function, line 324) `std::optional<char32_t> last_vowel_before(const std::u32string& w, size_t end)`
  - `harmony_vowel_for_kg` (function, line 333) `std::optional<char32_t> harmony_vowel_for_kg(const std::u32string& w,
                           ...`
  - `map_k_or_g` (function, line 342) `std::string map_k_or_g(char32_t ch, const std::u32string& w, size_t i)`
  - `map_simple_char` (function, line 354) `std::string map_simple_char(char32_t c)`
  - `is_vowel_ipa_char` (function, line 429) `bool is_vowel_ipa_char(char32_t c)`
  - `utf8_ipa_to_u32` (function, line 434) `std::u32string utf8_ipa_to_u32(std::string_view s)`
  - `u32_to_utf8_ipa` (function, line 439) `std::string u32_to_utf8_ipa(const std::u32string& s)`
  - `insert_primary_stress_final` (function, line 447) `std::string insert_primary_stress_final(const std::string& ipa_utf8)`
  - `is_turkish_word_char` (function, line 496) `bool is_turkish_word_char(char32_t cp)`
  - `is_space_cp` (function, line 516) `bool is_space_cp(char32_t cp)`
  - `TurkishRuleG2p` (function, line 527) `TurkishRuleG2p::TurkishRuleG2p(Options options) : options_(options)`
  - `dialect_ids` (function, line 529) `std::vector<std::string> TurkishRuleG2p::dialect_ids()`
  - `word_to_ipa` (function, line 533) `std::string TurkishRuleG2p::word_to_ipa(const std::string& word) const`
  - `text_to_ipa_no_expand` (function, line 617) `std::string TurkishRuleG2p::text_to_ipa_no_expand(
    const std::string& text, std::vector<G2pWo...`
  - `text_to_ipa` (function, line 695) `std::string TurkishRuleG2p::text_to_ipa(std::string text,
                                       ...`
  - `dialect_resolves_to_turkish_rules` (function, line 703) `bool dialect_resolves_to_turkish_rules(std::string_view dialect_id)`
  - `turkish_word_to_ipa` (function, line 714) `std::string turkish_word_to_ipa(const std::string& word, bool with_stress,
                      ...`
  - `turkish_text_to_ipa` (function, line 722) `std::string turkish_text_to_ipa(const std::string& text, bool with_stress,
                      ...`
  - `string` (function, line 129) `return std::string(s);`
  - `range_re` (function, line 162) `static const std::regex range_re(R"(\b(\d+)-(\d+)\b)", std::regex::ECMAScript);`
  - `dig_re` (function, line 164) `static const std::regex dig_re(R"(\b\d+\b)", std::regex::ECMAScript);`
  - `it` (function, line 166) `std::sregex_iterator it(text.begin(), text.end(), range_re);`
  - `it2` (function, line 182) `std::sregex_iterator it2(text.begin(), text.end(), dig_re);`
  - `utf8proc_NFC` (function, line 198) `utf8proc_NFC(reinterpret_cast<const utf8proc_uint8_t*>(s.c_str()));`
  - `utf8_str_to_u32` (function, line 200) `return utf8_str_to_u32(s);`
  - `composed` (function, line 202) `std::string composed(reinterpret_cast<char*>(nfc));`
  - `free` (function, line 203) `std::free(nfc);`
  - `utf8proc_tolower` (function, line 215) `utf8proc_tolower(static_cast<utf8proc_int32_t>(cp)));`
  - `tmp` (function, line 436) `std::string tmp(s);`
  - `utf8_append_codepoint` (function, line 443) `utf8_append_codepoint(o, c);`
  - `utf8proc_category` (function, line 508) `utf8proc_category(static_cast<utf8proc_int32_t>(cp)));`
  - `dig_pass` (function, line 549) `static const std::regex dig_pass(R"(^[0-9]+$)", std::regex::ECMAScript);`
  - `utf8_decode_at` (function, line 626) `utf8_decode_at(text, pos, cp, adv);`
  - `utf8_append_codepoint` (variable, line 5) `extern "C" { #include <utf8proc.h> } #include <cctype> #include <cstdlib> #include <optional> #include <regex> #include <string> #include <string_view> #include <vector> namespace moonshine_tts { name`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/turkish.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/turkish.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_TURKISH_H define MOONSHINE_TTS_LANG_SPECIFIC_TURKISH_H  include <string> include <vec
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 11)
  - `Options` (struct, line 19)
  - `TurkishRuleG2p` (class, line 17)
  - `dialect_id` (function, line 28) `const std::string& dialect_id() const`
  - `with_stress` (function, line 30) `bool with_stress() const`
  - `expand_cardinal_digits` (function, line 31) `bool expand_cardinal_digits() const`
  - `TurkishRuleG2p` (function, line 23) `TurkishRuleG2p();`
  - `dialect_ids` (function, line 26) `static std::vector<std::string> dialect_ids();`
  - `word_to_ipa` (function, line 34) `std::string word_to_ipa(const std::string& word) const;`
  - `text_to_ipa_no_expand` (function, line 44) `std::string text_to_ipa_no_expand( const std::string& text, std::vector<G2pWordLog>* per_word_log) const;`
  - `dialect_resolves_to_turkish_rules` (function, line 48) `bool dialect_resolves_to_turkish_rules(std::string_view dialect_id);`
  - `turkish_word_to_ipa` (function, line 52) `std::string turkish_word_to_ipa(const std::string& word, bool with_stress = true, bool expand_cardinal_digits = true);`
  - `turkish_text_to_ipa` (function, line 57) `std::string turkish_text_to_ipa(const std::string& text, bool with_stress = true, std::vector<G2pWordLog>* per_word_log = nullptr, bool expand_cardinal_digits = true);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_TURKISH_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_TURKISH_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/turkish.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/turkish-rule-g2p-test.cpp`

## core/moonshine-tts/src/lang-specific/ukrainian.cpp
- Layer: testing
- Doc: include "ukrainian.h"  include "g2p-word-log.h" include "utf8-utils.h"
- Language: cpp
- Symbols:
  - `is_all_ascii_digits` (function, line 26) `bool is_all_ascii_digits(std::string_view s)`
  - `utf8_nfc_utf8proc` (function, line 41) `std::string utf8_nfc_utf8proc(const std::string& s)`
  - `ukrainian_strip_stress_marks_utf8` (function, line 52) `std::string ukrainian_strip_stress_marks_utf8(std::string s)`
  - `utf8_to_u32_nfc` (function, line 78) `std::u32string utf8_to_u32_nfc(const std::string& s)`
  - `ukrainian_lower_u32` (function, line 89) `std::u32string ukrainian_lower_u32(const std::u32string& s)`
  - `thousand_noun_utf8` (function, line 119) `std::string thousand_noun_utf8(int h)`
  - `append_under_100_thousand_mult` (function, line 133) `void append_under_100_thousand_mult(int n, std::vector<std::string>& out)`
  - `append_under_100_plain` (function, line 182) `void append_under_100_plain(int n, std::vector<std::string>& out)`
  - `append_tokens_thousands_multiplier` (function, line 202) `void append_tokens_thousands_multiplier(int h, std::vector<std::string>& out)`
  - `append_tokens_0_999` (function, line 223) `void append_tokens_0_999(int n, std::vector<std::string>& out)`
  - `append_below_1_000_000` (function, line 242) `void append_below_1_000_000(int n, std::vector<std::string>& out)`
  - `join_space` (function, line 258) `std::string join_space(const std::vector<std::string>& p)`
  - `expand_cardinal_digits_to_ukrainian_words` (function, line 269) `std::string expand_cardinal_digits_to_ukrainian_words(std::string_view s)`
  - `expand_ukrainian_digit_tokens_in_text` (function, line 303) `std::string expand_ukrainian_digit_tokens_in_text(std::string text)`
  - `is_vowel_letter` (function, line 339) `bool is_vowel_letter(char32_t c)`
  - `is_soft_vowel` (function, line 345) `bool is_soft_vowel(char32_t c)`
  - `is_hard_no_pal` (function, line 350) `bool is_hard_no_pal(char32_t c)`
  - `is_palatalizable` (function, line 355) `bool is_palatalizable(char32_t c)`
  - `next_letter_index` (function, line 362) `std::optional<size_t> next_letter_index(const std::u32string& w, size_t start)`
  - `v_allophone` (function, line 388) `std::string v_allophone(const std::u32string& w, size_t i)`
  - `ends_with_palatal_suffix` (function, line 403) `bool ends_with_palatal_suffix(const std::string& p)`
  - `is_vowel_ipa_piece` (function, line 409) `bool is_vowel_ipa_piece(const std::string& p)`
  - `piece_ends_palatalized_consonant` (function, line 433) `bool piece_ends_palatalized_consonant(const std::vector<std::string>& pieces)`
  - `palatalize_last` (function, line 451) `void palatalize_last(std::vector<std::string>& pieces)`
  - `vowel_ipa` (function, line 470) `std::string vowel_ipa(char32_t ch, bool force_j, bool after_vowel_letter,
                      b...`
  - `ipa_vowel_char` (function, line 519) `bool ipa_vowel_char(char32_t c)`
  - `u32_to_utf8` (function, line 524) `std::string u32_to_utf8(const std::u32string& s)`
  - `insert_primary_stress_penultimate` (function, line 532) `std::string insert_primary_stress_penultimate(const std::string& ipa_utf8)`
  - `base_cons_ipa` (function, line 573) `std::string base_cons_ipa(char32_t c)`
  - `word_to_ipa_inner` (function, line 620) `std::string word_to_ipa_inner(const std::u32string& w0, bool with_stress)`
  - `filter_uk_word_chars` (function, line 726) `std::u32string filter_uk_word_chars(const std::u32string& w)`
  - `is_ukrainian_word_char` (function, line 743) `bool is_ukrainian_word_char(char32_t cp)`
  - `is_space_cp` (function, line 760) `bool is_space_cp(char32_t cp)`
  - `word_to_ipa_from_utf32_word` (function, line 767) `std::string word_to_ipa_from_utf32_word(const std::u32string& letters,
                          ...`
  - `hyphen_join_word_ipas` (function, line 775) `std::string hyphen_join_word_ipas(const std::string& tok, bool with_stress)`
  - `UkrainianRuleG2p` (function, line 802) `UkrainianRuleG2p::UkrainianRuleG2p(Options options) : options_(options)`
  - `dialect_ids` (function, line 804) `std::vector<std::string> UkrainianRuleG2p::dialect_ids()`
  - `word_to_ipa` (function, line 808) `std::string UkrainianRuleG2p::word_to_ipa(const std::string& word) const`
  - `text_to_ipa_no_expand` (function, line 831) `std::string UkrainianRuleG2p::text_to_ipa_no_expand(
    const std::string& text, std::vector<G2p...`
  - `text_to_ipa` (function, line 908) `std::string UkrainianRuleG2p::text_to_ipa(
    std::string text, std::vector<G2pWordLog>* per_wor...`
  - `dialect_resolves_to_ukrainian_rules` (function, line 916) `bool dialect_resolves_to_ukrainian_rules(std::string_view dialect_id)`
  - `ukrainian_word_to_ipa` (function, line 927) `std::string ukrainian_word_to_ipa(const std::string& word, bool with_stress,
                    ...`
  - `ukrainian_text_to_ipa` (function, line 935) `std::string ukrainian_text_to_ipa(const std::string& text, bool with_stress,
                    ...`
  - `utf8proc_NFC` (function, line 44) `utf8proc_NFC(reinterpret_cast<const utf8proc_uint8_t*>(s.c_str()));`
  - `out` (function, line 48) `std::string out(reinterpret_cast<char*>(p));`
  - `free` (function, line 49) `std::free(p);`
  - `utf8proc_NFD` (function, line 55) `utf8proc_NFD(reinterpret_cast<const utf8proc_uint8_t*>(s.c_str()));`
  - `utf8_append_codepoint` (function, line 72) `utf8_append_codepoint(stripped, static_cast<char32_t>(cp));`
  - `utf8_str_to_u32` (function, line 83) `return utf8_str_to_u32(s);`
  - `composed` (function, line 85) `std::string composed(reinterpret_cast<char*>(nfc));`
  - `utf8proc_tolower` (function, line 95) `utf8proc_tolower(static_cast<utf8proc_int32_t>(c));`
  - `string` (function, line 272) `return std::string(s);`
  - `range_re` (function, line 305) `static const std::regex range_re(R"(\b(\d+)-(\d+)\b)", std::regex::ECMAScript);`
  - `dig_re` (function, line 307) `static const std::regex dig_re(R"(\b\d+\b)", std::regex::ECMAScript);`
  - `it` (function, line 309) `std::sregex_iterator it(text.begin(), text.end(), range_re);`
  - `it2` (function, line 325) `std::sregex_iterator it2(text.begin(), text.end(), dig_re);`
  - `utf8proc_category` (function, line 735) `utf8proc_category(static_cast<utf8proc_int32_t>(c)));`
  - `dig_pass` (function, line 824) `static const std::regex dig_pass(R"(^[0-9]+$)", std::regex::ECMAScript);`
  - `utf8_decode_at` (function, line 840) `utf8_decode_at(text, pos, cp, adv);`
  - `trim_ascii_ws_copy` (variable, line 5) `extern "C" { #include <utf8proc.h> } #include <cctype> #include <cstdlib> #include <optional> #include <regex> #include <string> #include <string_view> #include <unordered_set> #include <vector> names`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/ukrainian.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/ukrainian.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_UKRAINIAN_H define MOONSHINE_TTS_LANG_SPECIFIC_UKRAINIAN_H  include <string> include 
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 11)
  - `Options` (struct, line 18)
  - `UkrainianRuleG2p` (class, line 16)
  - `dialect_id` (function, line 27) `const std::string& dialect_id() const`
  - `with_stress` (function, line 29) `bool with_stress() const`
  - `expand_cardinal_digits` (function, line 30) `bool expand_cardinal_digits() const`
  - `UkrainianRuleG2p` (function, line 22) `UkrainianRuleG2p();`
  - `dialect_ids` (function, line 25) `static std::vector<std::string> dialect_ids();`
  - `word_to_ipa` (function, line 33) `std::string word_to_ipa(const std::string& word) const;`
  - `text_to_ipa_no_expand` (function, line 43) `std::string text_to_ipa_no_expand( const std::string& text, std::vector<G2pWordLog>* per_word_log) const;`
  - `dialect_resolves_to_ukrainian_rules` (function, line 47) `bool dialect_resolves_to_ukrainian_rules(std::string_view dialect_id);`
  - `ukrainian_word_to_ipa` (function, line 49) `std::string ukrainian_word_to_ipa(const std::string& word, bool with_stress = true, bool expand_cardinal_digits = true);`
  - `ukrainian_text_to_ipa` (function, line 53) `std::string ukrainian_text_to_ipa( const std::string& text, bool with_stress = true, std::vector<G2pWordLog>* per_word_log = nullptr, bool expand_cardinal_digits = true);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_UKRAINIAN_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_UKRAINIAN_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/ukrainian.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/ukrainian-rule-g2p-test.cpp`

## core/moonshine-tts/src/lang-specific/vietnamese.cpp
- Layer: testing
- Doc: include "vietnamese.h"  include <cctype> include <cstring> include <fstream> include <istream> include <sstream> include
- Language: cpp
- Symbols:
  - `utf8_nfc_utf8proc` (function, line 22) `std::string utf8_nfc_utf8proc(std::string_view s)`
  - `utf8_lower_nfc` (function, line 34) `std::string utf8_lower_nfc(std::string_view s)`
  - `starts_with_sv` (function, line 53) `bool starts_with_sv(std::string_view s, std::string_view p)`
  - `ends_with_str` (function, line 57) `bool ends_with_str(const std::string& s, const std::string& suf)`
  - `split_tone` (function, line 64) `int split_tone(std::string_view in, std::string& body_nfc_out)`
  - `is_vowel_letter_char` (function, line 100) `bool is_vowel_letter_char(char32_t cp)`
  - `is_vowel_first_utf8` (function, line 118) `bool is_vowel_first_utf8(std::string_view s)`
  - `front_vowel_utf8` (function, line 130) `bool front_vowel_utf8(std::string_view s)`
  - `rime_is_only_i` (function, line 151) `bool rime_is_only_i(std::string_view rest)`
  - `wants_labial_coda` (function, line 306) `bool wants_labial_coda(const std::string& nuc_ipa)`
  - `coda_simple` (function, line 322) `std::string coda_simple(const std::string& coda, const std::string& nuc_ipa)`
  - `nucleus_to_ipa` (function, line 355) `std::string nucleus_to_ipa(std::string_view nuc_sv)`
  - `combine_nucleus_coda` (function, line 554) `std::string combine_nucleus_coda(const std::string& nuc_orth,
                                 co...`
  - `coda_obstruent_sac` (function, line 596) `bool coda_obstruent_sac(const std::string& coda)`
  - `tone_suffix_ipa` (function, line 601) `std::string tone_suffix_ipa(int tone, const std::string& coda_orth)`
  - `apply_tone` (function, line 631) `std::string apply_tone(const std::string& base, int tone, bool has_coda,
                       c...`
  - `is_unicode_edge_punct` (function, line 645) `bool is_unicode_edge_punct(char32_t cp, bool leading)`
  - `strip_edge_punct` (function, line 670) `std::string strip_edge_punct(std::string_view tok)`
  - `max_lex_key_words` (function, line 714) `int max_lex_key_words(const std::unordered_map<std::string, std::string>& lex)`
  - `load_vietnamese_lexicon_stream` (function, line 728) `void load_vietnamese_lexicon_stream(
    std::istream& in, std::unordered_map<std::string, std::s...`
  - `syllable_to_ipa` (function, line 757) `std::string VietnameseRuleG2p::syllable_to_ipa(std::string_view syllable_utf8)`
  - `VietnameseRuleG2p` (function, line 784) `VietnameseRuleG2p::VietnameseRuleG2p(std::filesystem::path dict_tsv)`
  - `VietnameseRuleG2p` (function, line 802) `VietnameseRuleG2p::VietnameseRuleG2p(std::string dict_tsv_utf8)`
  - `word_to_ipa` (function, line 811) `std::string VietnameseRuleG2p::word_to_ipa(std::string_view word) const`
  - `g2p_single_token` (function, line 815) `std::string VietnameseRuleG2p::g2p_single_token(std::string_view token) const`
  - `text_to_ipa` (function, line 827) `std::string VietnameseRuleG2p::text_to_ipa(
    std::string text, std::vector<G2pWordLog>* per_wo...`
  - `dialect_ids` (function, line 941) `std::vector<std::string> VietnameseRuleG2p::dialect_ids()`
  - `dialect_resolves_to_vietnamese_rules` (function, line 946) `bool dialect_resolves_to_vietnamese_rules(std::string_view dialect_id)`
  - `resolve_vietnamese_dict_path` (function, line 954) `std::filesystem::path resolve_vietnamese_dict_path(
    const std::filesystem::path& model_root)`
  - `tmp` (function, line 24) `const std::string tmp(s);`
  - `utf8proc_NFC` (function, line 26) `utf8proc_NFC(reinterpret_cast<const utf8proc_uint8_t*>(tmp.c_str()));`
  - `string` (function, line 28) `return std::string(s);`
  - `out` (function, line 30) `std::string out(reinterpret_cast<char*>(p));`
  - `free` (function, line 31) `std::free(p);`
  - `utf8proc_tolower` (function, line 47) `utf8proc_tolower(static_cast<utf8proc_int32_t>(cp));`
  - `utf8_append_codepoint` (function, line 48) `utf8_append_codepoint(out, static_cast<char32_t>(lo));`
  - `utf8proc_NFD` (function, line 67) `utf8proc_NFD(reinterpret_cast<const utf8proc_uint8_t*>(nfc.c_str()));`
  - `body` (function, line 174) `const std::string body(body_sv);`
  - `utf8_decode_at` (function, line 232) `utf8_decode_at(body, 0, cp0, a0);`
  - `rime` (function, line 295) `const std::string rime(rime_sv);`
  - `n` (function, line 356) `std::string n(nuc_sv);`
  - `take` (function, line 368) `take(4, "i\xC9\x99w");`
  - `trim_ascii_ws_copy` (function, line 744) `trim_ascii_ws_copy(std::string_view(line).substr(0, tab)));`
  - `runtime_error` (function, line 787) `throw std::runtime_error("Vietnamese G2P: lexicon not found at " + dict_tsv.generic_string());`
  - `in` (function, line 790) `std::ifstream in(dict_tsv);`
  - `iss` (function, line 836) `std::istringstream iss(raw);`
  - `min` (function, line 846) `std::min(max_key_words_, static_cast<int>(tokens.size() - pos));`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/vietnamese.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/vietnamese.h
- Layer: testing
- Doc: ifndef MOONSHINE_TTS_LANG_SPECIFIC_VIETNAMESE_H define MOONSHINE_TTS_LANG_SPECIFIC_VIETNAMESE_H  include <filesystem> in
- Language: h
- Symbols:
  - `G2pWordLog` (struct, line 13)
  - `VietnameseRuleG2p` (class, line 17)
  - `VietnameseRuleG2p` (function, line 18) `public: explicit VietnameseRuleG2p(std::filesystem::path dict_tsv);`
  - `dialect_ids` (function, line 21) `static std::vector<std::string> dialect_ids();`
  - `word_to_ipa` (function, line 26) `std::string word_to_ipa(std::string_view word) const;`
  - `syllable_to_ipa` (function, line 33) `static std::string syllable_to_ipa(std::string_view syllable_utf8);`
  - `g2p_single_token` (function, line 38) `std::string g2p_single_token(std::string_view token) const;`
  - `dialect_resolves_to_vietnamese_rules` (function, line 41) `bool dialect_resolves_to_vietnamese_rules(std::string_view dialect_id);`
  - `resolve_vietnamese_dict_path` (function, line 43) `std::filesystem::path resolve_vietnamese_dict_path( const std::filesystem::path& model_root);`
  - `MOONSHINE_TTS_LANG_SPECIFIC_VIETNAMESE_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_VIETNAMESE_H`
- Depends on: `core/moonshine-tts/src/rule-based-g2p.h`
- Imported by: `core/moonshine-tts/src/lang-specific/vietnamese.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/tests/vietnamese-rule-g2p-test.cpp`, `core/moonshine-tts/tools/vietnamese-rule-g2p-cli.cpp`
