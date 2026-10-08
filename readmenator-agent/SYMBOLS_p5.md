# Symbols (page 5 of 12)
Previous: [SYMBOLS_p4.md](SYMBOLS_p4.md)

| Symbol | Kind | File:Line | Signature |
|--------|------|-----------|-----------|
| `slurp_utf8_file` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:62` | `std::string slurp_utf8_file(const std::filesystem::path& p)` |
| `split_u32_whitespace` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:256` | `std::vector<std::u32string> split_u32_whitespace(std::u32string_view s)` |
| `strip_mn_nfd` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:201` | `std::u32string strip_mn_nfd(const std::u32string& s)` |
| `to_lower_u32` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:221` | `std::u32string to_lower_u32(const std::u32string& s)` |
| `tokenize_chinese_chars_u32` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:242` | `std::u32string tokenize_chinese_chars_u32(const std::u32string& text)` |
| `u32_nfc` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:189` | `std::u32string u32_nfc(const std::u32string& s)` |
| `u32_to_utf8` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:136` | `std::string u32_to_utf8(const std::u32string& s)` |
| `ud_upos_set` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:598` | `const std::unordered_set<std::string>& ud_upos_set()` |
| `utf8_to_u32` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:123` | `std::u32string utf8_to_u32(std::string_view utf8)` |
| `wordpiece_tokenize_u32` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:375` | `std::vector<std::u32string> wordpiece_tokenize_u32(     const std::u32string& token,     const st...` |
| `KoreanTokPosOnnx` | class | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.h:23` | `` |
| `MOONSHINE_TTS_KOREAN_TOK_POS_ONNX_H` | macro | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.h:2` | `#define MOONSHINE_TTS_KOREAN_TOK_POS_ONNX_H` |
| `MoonshineG2POptions` | struct | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.h:16` | `` |
| `format_annotated_line` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.h:39` | `static std::string format_annotated_line( const std::vector<std::pair<std::string, std::string>>& pairs);` |
| `model_dir` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.h:42` | `const std::filesystem::path& model_dir() const` |
| `0xAC00` | variable | `core/moonshine-tts/src/lang-specific/korean.cpp:20` | `extern "C" { #include <utf8proc.h> } namespace moonshine_tts { namespace { constexpr char32_t kHangulBase = 0xAC00;` |
| `KoreanRuleG2p` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:804` | `KoreanRuleG2p::KoreanRuleG2p(std::filesystem::path dict_tsv, Options options)     : options_(std:...` |
| `KoreanRuleG2p` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:818` | `KoreanRuleG2p::KoreanRuleG2p(std::string dict_tsv_utf8, Options options)     : options_(std::move...` |
| `Syllable` | struct | `core/moonshine-tts/src/lang-specific/korean.cpp:55` | `` |
| `apply_lateralization` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:277` | `void apply_lateralization(std::vector<Syllable>& syls)` |
| `apply_linking` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:249` | `void apply_linking(std::vector<Syllable>& syls)` |
| `coda_nasal_assimilate` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:425` | `std::string coda_nasal_assimilate(int jong, std::optional<int> next_cho)` |
| `decompose_syllable_cp` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:221` | `std::optional<Syllable> decompose_syllable_cp(char32_t ch)` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:1036` | `std::vector<std::string> KoreanRuleG2p::dialect_ids()` |
| `dialect_resolves_to_korean_rules` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:1041` | `bool dialect_resolves_to_korean_rules(std::string_view dialect_id)` |
| `extract_hangul` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:723` | `std::string KoreanRuleG2p::extract_hangul(std::string_view s) const` |
| `g2p_hangul_rules_only` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:739` | `std::string KoreanRuleG2p::g2p_hangul_rules_only(     std::string_view hangul) const` |
| `g2p_hangul_rules_only_inner` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:578` | `std::string g2p_hangul_rules_only_inner(std::string_view hangul,                                 ...` |
| `g2p_single_fragment` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:752` | `std::string KoreanRuleG2p::g2p_single_fragment(std::string_view frag) const` |
| `ipa_coda_simple` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:389` | `std::string ipa_coda_simple(int jong)` |
| `ipa_nucleus` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:376` | `std::string ipa_nucleus(int jung)` |
| `ipa_onset` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:291` | `std::string ipa_onset(int cho, bool tense, bool aspirate)` |
| `is_sonorant_jong` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:175` | `bool is_sonorant_jong(int jong)` |
| `jong_triggers_tense` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:183` | `bool jong_triggers_tense(int jong)` |
| `load_korean_lexicon_stream` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:775` | `void load_korean_lexicon_stream(     std::istream& in, std::unordered_map<std::string, std::strin...` |
| `nfd_str` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:90` | `const std::string nfd_str(reinterpret_cast<char*>(nfd));` |
| `normalize_korean_ipa` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:594` | `std::string KoreanRuleG2p::normalize_korean_ipa(std::string ipa,                                 ...` |
| `num_sv` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:985` | `const std::string num_sv(w, 0, num_end);` |
| `replace_all` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:61` | `void replace_all(std::string& s, const std::string& from,                  const std::string& to)` |
| `resolve_korean_dict_path` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:1049` | `std::filesystem::path resolve_korean_dict_path(     const std::filesystem::path& model_root)` |
| `sino_cardinal_speech_units` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:550` | `std::vector<std::string> sino_cardinal_speech_units(std::uint64_t n)` |
| `strip_mn_after_nfd` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:84` | `std::string strip_mn_after_nfd(const std::string& ipa)` |
| `syllables_to_ipa` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:447` | `std::string syllables_to_ipa(const std::vector<Syllable>& syls,                              std:...` |
| `tense_cho` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:204` | `int tense_cho(int plain_cho)` |
| `text_to_ipa` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:824` | `std::string KoreanRuleG2p::text_to_ipa(std::string text,                                        s...` |
| `text_to_syllables` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:233` | `std::vector<Syllable> text_to_syllables(std::string_view text)` |
| `tmp` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:73` | `const std::string tmp(s);` |
| `utf8_nfc_utf8proc` | function | `core/moonshine-tts/src/lang-specific/korean.cpp:72` | `std::string utf8_nfc_utf8proc(std::string_view s)` |
| `G2pWordLog` | struct | `core/moonshine-tts/src/lang-specific/korean.h:15` | `` |
| `KoreanRuleG2p` | class | `core/moonshine-tts/src/lang-specific/korean.h:19` | `` |
| `MOONSHINE_TTS_LANG_SPECIFIC_KOREAN_H` | macro | `core/moonshine-tts/src/lang-specific/korean.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_KOREAN_H` |
| `Options` | struct | `core/moonshine-tts/src/lang-specific/korean.h:21` | `` |
| `dialect_id` | function | `core/moonshine-tts/src/lang-specific/korean.h:35` | `const std::string& dialect_id() const` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/korean.h:33` | `static std::vector<std::string> dialect_ids();` |
| `dialect_resolves_to_korean_rules` | function | `core/moonshine-tts/src/lang-specific/korean.h:60` | `bool dialect_resolves_to_korean_rules(std::string_view dialect_id);` |
| `normalize_korean_ipa` | function | `core/moonshine-tts/src/lang-specific/korean.h:43` | `static std::string normalize_korean_ipa(std::string ipa, bool voice_lenis = true);` |
| `OnnxOovG2p` | function | `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:90` | `OnnxOovG2p::OnnxOovG2p(Ort::Env& env, const std::filesystem::path& model_onnx,                   ...` |
| `OnnxOovG2p` | function | `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:97` | `OnnxOovG2p::OnnxOovG2p(Ort::Env& env, const void* model_onnx_bytes,                        size_t...` |
| `argmax_vocab_row` | function | `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:73` | `int argmax_vocab_row(const float* logits, int64_t vocab, int time_index)` |
| `decoder_io_padded` | function | `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:58` | `void decoder_io_padded(const std::vector<int64_t>& cur, int max_phoneme_len,                     ...` |
| `enc_ids` | function | `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:115` | `std::vector<int64_t> enc_ids(static_cast<size_t>(tab_.max_seq_len), tab_.pad_id);` |
| `enc_mask` | function | `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:117` | `std::vector<int64_t> enc_mask(static_cast<size_t>(tab_.max_seq_len), 0);` |
| `encode_chars_for_model` | function | `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:46` | `std::vector<int64_t> encode_chars_for_model(     const std::string& text,     const std::unordere...` |
| `open_session` | function | `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:21` | `Ort::Session open_session(Ort::Env& env,                           const std::filesystem::path& m...` |
| `open_session_memory` | function | `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:38` | `Ort::Session open_session_memory(Ort::Env& env, const void* data, size_t len,                    ...` |
| `predict_phonemes` | function | `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:106` | `std::vector<std::string> OnnxOovG2p::predict_phonemes(const std::string& word)` |
| `MOONSHINE_TTS_ONNX_G2P_MODELS_H` | macro | `core/moonshine-tts/src/lang-specific/onnx-g2p-models.h:2` | `#define MOONSHINE_TTS_ONNX_G2P_MODELS_H` |
| `OnnxOovG2p` | class | `core/moonshine-tts/src/lang-specific/onnx-g2p-models.h:17` | `` |
| `accented_syllable_u32` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:352` | `bool accented_syllable_u32(const std::u32string& s)` |
| `default_stressed_syllable_index_u32` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:362` | `size_t default_stressed_syllable_index_u32(     const std::vector<std::u32string>& syls, const st...` |
| `filter_pt_word_graphemes_utf8` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:135` | `std::u32string filter_pt_word_graphemes_utf8(const std::string& word)` |
| `insert_primary_stress_before_vowel_utf8` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:430` | `std::string insert_primary_stress_before_vowel_utf8(std::string ipa)` |
| `is_allowed_pt_grapheme` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:122` | `bool is_allowed_pt_grapheme(char32_t c)` |
| `is_pt_key_cp` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:69` | `bool is_pt_key_cp(char32_t c)` |
| `is_vowel_pt_u32` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:151` | `bool is_vowel_pt_u32(char32_t ch)` |
| `letters_to_ipa_no_stress_u32` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:589` | `std::string letters_to_ipa_no_stress_u32(const std::u32string& s, bool is_pt_pt,                 ...` |
| `next_global_vowel_u32` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:569` | `bool next_global_vowel_u32(const std::u32string& full_word, size_t gidx)` |
| `normalize_lookup_key_utf8` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:106` | `std::string normalize_lookup_key_utf8(const std::string& word)` |
| `normalize_lookup_key_utf8_impl` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:85` | `std::string normalize_lookup_key_utf8_impl(const std::string& word)` |
| `port_orthographic_syllables_u32` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:297` | `std::vector<std::u32string> port_orthographic_syllables_u32(     const std::u32string& w0)` |
| `prev_global_vowel_u32` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:549` | `bool prev_global_vowel_u32(const std::u32string& full_word, size_t gidx)` |
| `pt_pt_apply_rules_final_s_to_esh` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:1026` | `std::string pt_pt_apply_rules_final_s_to_esh(std::string ipa,                                    ...` |
| `pt_tolower` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:24` | `char32_t pt_tolower(char32_t c)` |
| `roman_numeral_token_to_ipa` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:491` | `std::optional<std::string> roman_numeral_token_to_ipa(     const std::string& letters_lower, bool...` |
| `roman_to_int_ascii` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:453` | `std::optional<int> roman_to_int_ascii(std::string_view u)` |
| `rules_word_to_ipa_single_u32` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:964` | `std::string rules_word_to_ipa_single_u32(const std::u32string& wl,                               ...` |
| `rules_word_to_ipa_utf8` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:1161` | `std::string rules_word_to_ipa_utf8(const std::string& raw, bool is_pt_pt,                        ...` |
| `should_hiatus_pt_u32` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:186` | `bool should_hiatus_pt_u32(char32_t a, char32_t b)` |
| `strip_accent_base_pt` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:159` | `char32_t strip_accent_base_pt(char32_t c)` |
| `strip_stress_chars` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:424` | `std::string strip_stress_chars(std::string s)` |
| `syllable_has_u32` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:585` | `bool syllable_has_u32(const std::u32string& s, char32_t ch)` |
| `u32_to_utf8_pt` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:114` | `std::string u32_to_utf8_pt(const std::u32string& s)` |
| `utf8_to_u32_pt` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:110` | `std::u32string utf8_to_u32_pt(const std::string& s)` |
| `valid_onset2_end_u32` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:261` | `bool valid_onset2_end_u32(char32_t a, char32_t b)` |
| `vowel_grapheme_tail_pt` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:1018` | `bool vowel_grapheme_tail_pt(char32_t c)` |
| `MOONSHINE_TTS_LANG_SPECIFIC_PORTUGUESE_RULES_H` | macro | `core/moonshine-tts/src/lang-specific/portuguese-rules.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_PORTUGUESE_RULES_H` |
| `pt_tolower` | function | `core/moonshine-tts/src/lang-specific/portuguese-rules.h:11` | `char32_t pt_tolower(char32_t c);` |
| `PortugueseRuleG2p` | function | `core/moonshine-tts/src/lang-specific/portuguese.cpp:411` | `PortugueseRuleG2p::PortugueseRuleG2p(std::filesystem::path dict_tsv,                             ...` |
| `PortugueseRuleG2p` | function | `core/moonshine-tts/src/lang-specific/portuguese.cpp:418` | `PortugueseRuleG2p::PortugueseRuleG2p(std::string dict_tsv_utf8,                                  ...` |
| `below_1000_tokens_pt` | function | `core/moonshine-tts/src/lang-specific/portuguese.cpp:200` | `void below_1000_tokens_pt(int n, bool is_pt_pt, std::vector<std::string>& out)` |
| `below_1_000_000_tokens_pt` | function | `core/moonshine-tts/src/lang-specific/portuguese.cpp:228` | `void below_1_000_000_tokens_pt(int n, bool is_pt_pt,                                std::vector<s...` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/portuguese.cpp:628` | `std::vector<std::string> PortugueseRuleG2p::dialect_ids()` |
| `dialect_resolves_to_brazilian_portuguese_rules` | function | `core/moonshine-tts/src/lang-specific/portuguese.cpp:618` | `bool dialect_resolves_to_brazilian_portuguese_rules(     std::string_view dialect_id)` |
| `dialect_resolves_to_portugal_rules` | function | `core/moonshine-tts/src/lang-specific/portuguese.cpp:609` | `bool dialect_resolves_to_portugal_rules(std::string_view dialect_id)` |
| `dig_pass` | function | `core/moonshine-tts/src/lang-specific/portuguese.cpp:522` | `static const std::regex dig_pass(R"(^[0-9]+(?:-[0-9]+)*$)", std::regex::ECMAScript);` |
| `dig_re` | function | `core/moonshine-tts/src/lang-specific/portuguese.cpp:292` | `static const std::regex dig_re(R"(\b\d+\b)", std::regex::ECMAScript);` |
| `expand_cardinal_digits_to_portuguese_words` | function | `core/moonshine-tts/src/lang-specific/portuguese.cpp:252` | `std::string expand_cardinal_digits_to_portuguese_words(std::string_view s,                       ...` |
| `expand_digit_tokens_in_text` | function | `core/moonshine-tts/src/lang-specific/portuguese.cpp:289` | `std::string expand_digit_tokens_in_text(std::string text, bool is_pt_pt)` |
| `finalize_ipa` | function | `core/moonshine-tts/src/lang-specific/portuguese.cpp:426` | `std::string PortugueseRuleG2p::finalize_ipa(std::string ipa,                                     ...` |
| `is_all_ascii_digits` | function | `core/moonshine-tts/src/lang-specific/portuguese.cpp:97` | `bool is_all_ascii_digits(std::string_view s)` |
| `is_pt_word_char` | function | `core/moonshine-tts/src/lang-specific/portuguese.cpp:322` | `bool is_pt_word_char(char32_t cp)` |
| `load_pt_lexicon_file` | function | `core/moonshine-tts/src/lang-specific/portuguese.cpp:84` | `void load_pt_lexicon_file(const std::filesystem::path& path,                           std::unord...` |
| `load_pt_lexicon_stream` | function | `core/moonshine-tts/src/lang-specific/portuguese.cpp:52` | `void load_pt_lexicon_stream(std::istream& in,                             std::unordered_map<std:...` |
| `lookup_or_rules` | function | `core/moonshine-tts/src/lang-specific/portuguese.cpp:445` | `std::string PortugueseRuleG2p::lookup_or_rules(     const std::string& raw_word) const` |
| `range_re` | function | `core/moonshine-tts/src/lang-specific/portuguese.cpp:290` | `static const std::regex range_re(R"(\b(\d+)-(\d+)\b)", std::regex::ECMAScript);` |
| `resolve_portuguese_dict_path` | function | `core/moonshine-tts/src/lang-specific/portuguese.cpp:635` | `std::filesystem::path resolve_portuguese_dict_path(     const std::filesystem::path& model_root, ...` |
| `teens_word_pt` | function | `core/moonshine-tts/src/lang-specific/portuguese.cpp:121` | `std::string teens_word_pt(int n, bool is_pt_pt)` |
| `text_to_ipa` | function | `core/moonshine-tts/src/lang-specific/portuguese.cpp:601` | `std::string PortugueseRuleG2p::text_to_ipa(     std::string text, std::vector<G2pWordLog>* per_wo...` |
| `text_to_ipa_no_expand` | function | `core/moonshine-tts/src/lang-specific/portuguese.cpp:531` | `std::string PortugueseRuleG2p::text_to_ipa_no_expand(     const std::string& text, std::vector<G2...` |
| `try_consume_pt_word` | function | `core/moonshine-tts/src/lang-specific/portuguese.cpp:355` | `bool try_consume_pt_word(const std::string& text, size_t pos, size_t& out_end)` |
| `under_100_tokens_pt` | function | `core/moonshine-tts/src/lang-specific/portuguese.cpp:173` | `void under_100_tokens_pt(int n, bool is_pt_pt, std::vector<std::string>& out)` |
| `utf8_lowercase_pt_surface` | function | `core/moonshine-tts/src/lang-specific/portuguese.cpp:39` | `std::string utf8_lowercase_pt_surface(const std::string& word)` |
| `word_to_ipa` | function | `core/moonshine-tts/src/lang-specific/portuguese.cpp:508` | `std::string PortugueseRuleG2p::word_to_ipa(const std::string& word) const` |
| `G2pWordLog` | struct | `core/moonshine-tts/src/lang-specific/portuguese.h:14` | `` |
| `MOONSHINE_TTS_LANG_SPECIFIC_PORTUGUESE_H` | macro | `core/moonshine-tts/src/lang-specific/portuguese.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_PORTUGUESE_H` |
| `Options` | struct | `core/moonshine-tts/src/lang-specific/portuguese.h:20` | `` |
| `PortugueseRuleG2p` | class | `core/moonshine-tts/src/lang-specific/portuguese.h:18` | `` |
| `dialect_id` | function | `core/moonshine-tts/src/lang-specific/portuguese.h:39` | `const std::string& dialect_id() const` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/portuguese.h:36` | `static std::vector<std::string> dialect_ids();` |
| `dialect_resolves_to_brazilian_portuguese_rules` | function | `core/moonshine-tts/src/lang-specific/portuguese.h:64` | `bool dialect_resolves_to_brazilian_portuguese_rules( std::string_view dialect_id);` |
| `dialect_resolves_to_portugal_rules` | function | `core/moonshine-tts/src/lang-specific/portuguese.h:61` | `bool dialect_resolves_to_portugal_rules(std::string_view dialect_id);` |
| `is_portugal` | function | `core/moonshine-tts/src/lang-specific/portuguese.h:38` | `bool is_portugal() const` |
| `dig_re` | function | `core/moonshine-tts/src/lang-specific/russian-numbers.cpp:223` | `static const std::regex dig_re(R"(\b\d+\b)", std::regex::ECMAScript);` |
| `expand_cardinal_digits_to_russian_words` | function | `core/moonshine-tts/src/lang-specific/russian-numbers.cpp:183` | `std::string expand_cardinal_digits_to_russian_words(std::string_view s)` |
| `expand_russian_digit_tokens_in_text` | function | `core/moonshine-tts/src/lang-specific/russian-numbers.cpp:220` | `std::string expand_russian_digit_tokens_in_text(std::string text)` |
| `range_re` | function | `core/moonshine-tts/src/lang-specific/russian-numbers.cpp:221` | `static const std::regex range_re(R"(\b(\d+)-(\d+)\b)", std::regex::ECMAScript);` |
| `ru_append_below_1_000_000` | function | `core/moonshine-tts/src/lang-specific/russian-numbers.cpp:166` | `void ru_append_below_1_000_000(int n, std::vector<std::string>& out)` |
| `ru_append_cardinal_1_to_999` | function | `core/moonshine-tts/src/lang-specific/russian-numbers.cpp:134` | `void ru_append_cardinal_1_to_999(int n, bool feminine,                                  std::vect...` |
| `ru_append_under_100` | function | `core/moonshine-tts/src/lang-specific/russian-numbers.cpp:114` | `void ru_append_under_100(int n, bool feminine, std::vector<std::string>& out)` |
| `ru_ascii_all_digits` | function | `core/moonshine-tts/src/lang-specific/russian-numbers.cpp:14` | `bool ru_ascii_all_digits(std::string_view s)` |
| `ru_ones_digit` | function | `core/moonshine-tts/src/lang-specific/russian-numbers.cpp:99` | `std::string ru_ones_digit(int n, bool feminine)` |
| `ru_thousand_suffix` | function | `core/moonshine-tts/src/lang-specific/russian-numbers.cpp:151` | `const char* ru_thousand_suffix(int q)` |
| `RussianRuleG2p` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:993` | `RussianRuleG2p::RussianRuleG2p(std::filesystem::path dict_tsv, Options options)     : options_(op...` |
| `RussianRuleG2p` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:998` | `RussianRuleG2p::RussianRuleG2p(std::string dict_tsv_utf8, Options options)     : options_(options)` |
| `acute_stressed_vowel_ordinal` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:305` | `std::optional<int> acute_stressed_vowel_ordinal(const std::string& w_nfc)` |
| `append_nfd_expansion` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:126` | `void append_nfd_expansion(char32_t cp, std::u32string& out)` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:1173` | `std::vector<std::string> RussianRuleG2p::dialect_ids()` |
| `dialect_resolves_to_russian_rules` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:1165` | `bool dialect_resolves_to_russian_rules(std::string_view dialect_id)` |
| `dig_pass` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:1074` | `static const std::regex dig_pass(R"(^[0-9]+(?:-[0-9]+)*$)", std::regex::ECMAScript);` |
| `emit_consonant` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:473` | `std::string emit_consonant(char32_t ch, bool palatal)` |
| `filter_russian_graphemes_keep_stress` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:259` | `std::string filter_russian_graphemes_keep_stress(std::string_view raw)` |
| `finalize_ipa` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:1004` | `std::string RussianRuleG2p::finalize_ipa(std::string ipa) const` |
| `insert_primary_stress_before_vowel` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:789` | `std::string insert_primary_stress_before_vowel(std::string s)` |
| `ipa_piece_after_hard_consonant` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:547` | `bool ipa_piece_after_hard_consonant(const std::string& piece)` |
| `ipa_piece_ends_with_palatal` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:525` | `bool ipa_piece_ends_with_palatal(const std::string& piece)` |
| `ipa_piece_last_is_vowel_letter` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:534` | `bool ipa_piece_last_is_vowel_letter(const std::string& piece)` |
| `is_combining_mark` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:56` | `bool is_combining_mark(char32_t cp)` |
| `is_latin1_supplement_python_word_char` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:886` | `bool is_latin1_supplement_python_word_char(char32_t cp)` |
| `is_russian_lex_key_cp` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:76` | `bool is_russian_lex_key_cp(char32_t c)` |
| `is_russian_vowel_letter` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:68` | `bool is_russian_vowel_letter(char32_t c)` |
| `is_unicode_mn` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:37` | `bool is_unicode_mn(char32_t cp)` |
| `is_unicode_word_char_w` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:907` | `bool is_unicode_word_char_w(char32_t cp)` |
| `letters_to_ipa_rules` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:620` | `std::string letters_to_ipa_rules(const std::string& w_clean, int stress_syl)` |
| `load_russian_lexicon_file` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:248` | `void load_russian_lexicon_file(     const std::filesystem::path& path,     std::unordered_map<std...` |
| `load_russian_lexicon_stream` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:216` | `void load_russian_lexicon_stream(     std::istream& in, std::unordered_map<std::string, std::stri...` |
| `lookup_or_rules` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:1018` | `std::string RussianRuleG2p::lookup_or_rules(const std::string& raw_word) const` |
| `normalize_lookup_key_utf8` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:163` | `std::string normalize_lookup_key_utf8(const std::string& word)` |
| `normalize_russian_fleeting_palatal_markers_utf8` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:976` | `std::string normalize_russian_fleeting_palatal_markers_utf8(std::string ipa)` |
| `palatalizable_cons` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:465` | `bool palatalizable_cons(char32_t ch)` |
| `remove_if` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:423` | `std::remove_if(syllables.begin(), syllables.end(),                      [](const std::string& x)` |
| `resolve_russian_dict_path` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:1177` | `std::filesystem::path resolve_russian_dict_path(     const std::filesystem::path& model_root)` |
| `rules_word_to_ipa` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:821` | `std::string rules_word_to_ipa(const std::string& raw, bool with_stress)` |
| `rules_word_to_ipa_single` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:809` | `std::string rules_word_to_ipa_single(const std::string& w_clean,                                 ...` |
| `russian_orthographic_syllables_utf8` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:357` | `std::vector<std::string> russian_orthographic_syllables_utf8(     const std::string& word_lower)` |
| `russian_tolower_cp` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:58` | `char32_t russian_tolower_cp(char32_t c)` |
| `stress_syllable_index` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:429` | `int stress_syllable_index(const std::vector<std::string>& syls,                           const s...` |
| `strip_grapheme_diacritics_utf8` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:281` | `std::string strip_grapheme_diacritics_utf8(std::string_view sv)` |
| `surface_is_all_lowercase_russian` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:212` | `bool surface_is_all_lowercase_russian(const std::string& surf)` |
| `syllable_index_per_codepoint` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:453` | `std::vector<int> syllable_index_per_codepoint(const std::string& w)` |
| `text_to_ipa` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:1157` | `std::string RussianRuleG2p::text_to_ipa(std::string text,                                        ...` |
| `text_to_ipa_no_expand` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:1083` | `std::string RussianRuleG2p::text_to_ipa_no_expand(     const std::string& text, std::vector<G2pWo...` |
| `try_consume_unicode_word` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:946` | `bool try_consume_unicode_word(const std::string& text, size_t pos,                               ...` |
| `u32_to_utf8` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:136` | `std::string u32_to_utf8(const std::u32string& s)` |
| `unicode_tolower_like_python` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:144` | `char32_t unicode_tolower_like_python(char32_t cp)` |
| `utf8_contains_cyrillic` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:932` | `bool utf8_contains_cyrillic(const std::string& tok)` |
| `utf8_russian_lowercase` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:194` | `std::string utf8_russian_lowercase(const std::string& word)` |
| `vowel_ipa` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:560` | `std::string vowel_ipa(char32_t ch, bool stressed, bool after_palatal,                       bool ...` |
| `vowel_ordinal_to_syllable` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:336` | `int vowel_ordinal_to_syllable(const std::vector<std::string>& syls,                              ...` |
| `word_to_ipa` | function | `core/moonshine-tts/src/lang-specific/russian.cpp:1061` | `std::string RussianRuleG2p::word_to_ipa(const std::string& word) const` |
| `G2pWordLog` | struct | `core/moonshine-tts/src/lang-specific/russian.h:14` | `` |
| `MOONSHINE_TTS_LANG_SPECIFIC_RUSSIAN_H` | macro | `core/moonshine-tts/src/lang-specific/russian.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_RUSSIAN_H` |
| `Options` | struct | `core/moonshine-tts/src/lang-specific/russian.h:19` | `` |
| `RussianRuleG2p` | class | `core/moonshine-tts/src/lang-specific/russian.h:17` | `` |
| `dialect_id` | function | `core/moonshine-tts/src/lang-specific/russian.h:37` | `const std::string& dialect_id() const` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/russian.h:35` | `static std::vector<std::string> dialect_ids();` |
| `dialect_resolves_to_russian_rules` | function | `core/moonshine-tts/src/lang-specific/russian.h:57` | `bool dialect_resolves_to_russian_rules(std::string_view dialect_id);` |
| `dig_re` | function | `core/moonshine-tts/src/lang-specific/spanish-numbers.cpp:183` | `static const std::regex dig_re(R"(\b\d+\b)", std::regex::ECMAScript);` |
| `es_append_below_1000` | function | `core/moonshine-tts/src/lang-specific/spanish-numbers.cpp:98` | `void es_append_below_1000(int n, std::vector<std::string>& out)` |
| `es_append_below_1_000_000` | function | `core/moonshine-tts/src/lang-specific/spanish-numbers.cpp:123` | `void es_append_below_1_000_000(int n, std::vector<std::string>& out)` |
| `es_append_under_100` | function | `core/moonshine-tts/src/lang-specific/spanish-numbers.cpp:77` | `void es_append_under_100(int n, std::vector<std::string>& out)` |
| `es_ascii_all_digits` | function | `core/moonshine-tts/src/lang-specific/spanish-numbers.cpp:14` | `bool es_ascii_all_digits(std::string_view s)` |
| `expand_cardinal_digits_to_spanish_words` | function | `core/moonshine-tts/src/lang-specific/spanish-numbers.cpp:144` | `std::string expand_cardinal_digits_to_spanish_words(std::string_view s)` |
| `expand_spanish_digit_tokens_in_text` | function | `core/moonshine-tts/src/lang-specific/spanish-numbers.cpp:180` | `std::string expand_spanish_digit_tokens_in_text(std::string text)` |
| `range_re` | function | `core/moonshine-tts/src/lang-specific/spanish-numbers.cpp:181` | `static const std::regex range_re(R"(\b(\d+)-(\d+)\b)", std::regex::ECMAScript);` |
| `MOONSHINE_TTS_LANG_SPECIFIC_SPANISH_UNICODE_TABLES_H` | macro | `core/moonshine-tts/src/lang-specific/spanish-unicode-tables.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_SPANISH_UNICODE_TABLES_H` |
| `k_unicode_lower_table` | variable | `core/moonshine-tts/src/lang-specific/spanish-unicode-tables.h:13` | `extern const std::pair<char32_t, const char*> k_unicode_lower_table[];` |
| `k_unicode_lower_table_size` | variable | `core/moonshine-tts/src/lang-specific/spanish-unicode-tables.h:14` | `extern const std::size_t k_unicode_lower_table_size;` |
| `k_unicode_space_bitmap` | variable | `core/moonshine-tts/src/lang-specific/spanish-unicode-tables.h:17` | `extern const std::uint32_t k_unicode_space_bitmap[];` |
| `k_unicode_space_bitmap_words` | variable | `core/moonshine-tts/src/lang-specific/spanish-unicode-tables.h:18` | `extern const std::uint32_t k_unicode_space_bitmap_words;` |
| `k_unicode_strip_table` | variable | `core/moonshine-tts/src/lang-specific/spanish-unicode-tables.h:11` | `extern const std::pair<char32_t, const char*> k_unicode_strip_table[];` |
| `k_unicode_strip_table_size` | variable | `core/moonshine-tts/src/lang-specific/spanish-unicode-tables.h:12` | `extern const std::size_t k_unicode_strip_table_size;` |
| `k_unicode_word_bitmap` | variable | `core/moonshine-tts/src/lang-specific/spanish-unicode-tables.h:15` | `extern const std::uint32_t k_unicode_word_bitmap[];` |
| `k_unicode_word_bitmap_words` | variable | `core/moonshine-tts/src/lang-specific/spanish-unicode-tables.h:16` | `extern const std::uint32_t k_unicode_word_bitmap_words;` |
| `is_space_char` | function | `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp:100` | `bool is_space_char(char32_t cp)` |
| `is_word_char` | function | `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp:95` | `bool is_word_char(char32_t cp)` |
| `lookup_sorted_pair` | function | `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp:12` | `const char* lookup_sorted_pair(const std::pair<char32_t, const char*>* table,                    ...` |
| `lower_bound` | function | `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp:17` | `std::lower_bound(first, last, key,                        [](const std::pair<char32_t, const char...` |
| `strip_accents_utf8` | function | `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp:72` | `std::string strip_accents_utf8(const std::string& s)` |
| `strip_replacement_utf8` | function | `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp:105` | `const char* strip_replacement_utf8(char32_t cp)` |
| `unicode_bitmap_get` | function | `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp:26` | `bool unicode_bitmap_get(const std::uint32_t* bitmap, std::uint32_t nwords,                       ...` |
| `unicode_lower_utf8` | function | `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp:53` | `std::string unicode_lower_utf8(const std::string& s)` |
| `utf32_to_utf8` | function | `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp:40` | `std::string utf32_to_utf8(const std::u32string& u)` |
| `utf8_to_utf32` | function | `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp:49` | `std::u32string utf8_to_utf32(const std::string& s)` |
| `word_key` | function | `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp:91` | `std::string word_key(const std::string& wraw)` |
| `MOONSHINE_TTS_LANG_SPECIFIC_SPANISH_UNICODE_H` | macro | `core/moonshine-tts/src/lang-specific/spanish-unicode.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_SPANISH_UNICODE_H` |
| `is_space_char` | function | `core/moonshine-tts/src/lang-specific/spanish-unicode.h:15` | `bool is_space_char(char32_t cp);` |
| `is_word_char` | function | `core/moonshine-tts/src/lang-specific/spanish-unicode.h:14` | `bool is_word_char(char32_t cp);` |
| `strip_replacement_utf8` | function | `core/moonshine-tts/src/lang-specific/spanish-unicode.h:17` | `const char* strip_replacement_utf8(char32_t cp);` |
| `SpanishRuleG2p` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:929` | `SpanishRuleG2p::SpanishRuleG2p(SpanishDialect dialect, bool with_stress,                         ...` |
| `XExc` | struct | `core/moonshine-tts/src/lang-specific/spanish.cpp:264` | `` |
| `apply_coda_s_weakening` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:417` | `std::string apply_coda_s_weakening(std::string ipa,                                    SpanishDia...` |
| `apply_narrow_intervocalic_obstruents` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:380` | `std::string apply_narrow_intervocalic_obstruents(std::string ipa)` |
| `apply_nasal_assimilation` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:304` | `std::string apply_nasal_assimilation(std::string s,                                      const Sp...` |
| `clean_syllable_word` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:178` | `std::u32string clean_syllable_word(const std::u32string &word_lower)` |
| `count_primary_stress_utf8` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:356` | `size_t count_primary_stress_utf8(const std::string &ipa)` |
| `default_stressed_syllable_index_v2` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:226` | `size_t default_stressed_syllable_index_v2(const std::u32string &w_clean_lower)` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:823` | `std::vector<std::string> SpanishRuleG2p::dialect_ids()` |
| `dig_pass` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:957` | `static const std::regex dig_pass(R"(^[0-9]+$)", std::regex::ECMAScript);` |
| `filter_word_letters_utf32` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:773` | `std::u32string filter_word_letters_utf32(const std::string &wraw)` |
| `insert_primary_stress_before_vowel` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:333` | `std::string insert_primary_stress_before_vowel(const std::string &ipa)` |
| `ipa_stress_at_start` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:371` | `bool ipa_stress_at_start(const std::string &ipa)` |
| `is_valid_onset2` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:145` | `bool is_valid_onset2(char32_t a, char32_t b)` |
| `is_vowel_ch` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:23` | `bool is_vowel_ch(char32_t ch)` |
| `letters_to_ipa_no_stress` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:504` | `std::string letters_to_ipa_no_stress(const std::u32string &syl_lower,                            ...` |
| `lookup_x_exception` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:295` | `const char *lookup_x_exception(const std::string &wkey)` |
| `make_common` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:791` | `SpanishDialect make_common(const std::string &id, std::string ce_ci_z_ipa,                       ...` |
| `orthographic_syllables_utf8` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:189` | `std::vector<std::string> orthographic_syllables_utf8(     const std::string &word_lower_utf8)` |
| `postprocess_lexical_ipa` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:432` | `std::string postprocess_lexical_ipa(std::string ipa,                                     const Sp...` |
| `prev_phoneme_was_vowel` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:458` | `bool prev_phoneme_was_vowel(const std::vector<std::string> &out)` |
| `should_hiatus` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:43` | `bool should_hiatus(char32_t a, char32_t b)` |
| `spanish_dialect_cli_ids` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:816` | `std::vector<std::string> spanish_dialect_cli_ids()` |
| `spanish_dialect_from_cli_id` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:827` | `SpanishDialect spanish_dialect_from_cli_id(     const std::string &cli_id, bool narrow_intervocal...` |
| `spanish_text_to_ipa` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:1102` | `std::string spanish_text_to_ipa(const std::string &text,                                 const Sp...` |
| `spanish_word_to_ipa` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:1095` | `std::string spanish_word_to_ipa(const std::string &word,                                 const Sp...` |
| `text_to_ipa` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:1087` | `std::string SpanishRuleG2p::text_to_ipa(std::string text,                                        ...` |
| `text_to_ipa_no_expand` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:1003` | `std::string SpanishRuleG2p::text_to_ipa_no_expand(     const std::string &text, std::vector<G2pWo...` |
| `to_lower_cp` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:496` | `char32_t to_lower_cp(char32_t c)` |
| `word_to_ipa` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:935` | `std::string SpanishRuleG2p::word_to_ipa(const std::string &word) const` |
| `y_is_consonant` | function | `core/moonshine-tts/src/lang-specific/spanish.cpp:470` | `bool y_is_consonant(const std::u32string &letters_lower, size_t i)` |
| `CodaS` | enum | `core/moonshine-tts/src/lang-specific/spanish.h:26` | `` |
| `CodaS` | class | `core/moonshine-tts/src/lang-specific/spanish.h:26` | `` |
| `MOONSHINE_TTS_LANG_SPECIFIC_SPANISH_H` | macro | `core/moonshine-tts/src/lang-specific/spanish.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_SPANISH_H` |
| `SpanishDialect` | struct | `core/moonshine-tts/src/lang-specific/spanish.h:13` | `` |
| `SpanishRuleG2p` | class | `core/moonshine-tts/src/lang-specific/spanish.h:30` | `` |
| `dialect` | function | `core/moonshine-tts/src/lang-specific/spanish.h:37` | `const SpanishDialect& dialect() const` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/spanish.h:35` | `static std::vector<std::string> dialect_ids();` |
| `expand_cardinal_digits` | function | `core/moonshine-tts/src/lang-specific/spanish.h:39` | `bool expand_cardinal_digits() const` |
| `with_stress` | function | `core/moonshine-tts/src/lang-specific/spanish.h:38` | `bool with_stress() const` |
| `TurkishRuleG2p` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:528` | `TurkishRuleG2p::TurkishRuleG2p(Options options) : options_(options)` |
| `append_below_1_000_000` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:95` | `void append_below_1_000_000(int n, std::vector<std::string>& out)` |
| `append_tokens_0_999` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:71` | `void append_tokens_0_999(int n, std::vector<std::string>& out)` |
| `append_under_100` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:46` | `void append_under_100(int n, std::vector<std::string>& out)` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:530` | `std::vector<std::string> TurkishRuleG2p::dialect_ids()` |
| `dialect_resolves_to_turkish_rules` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:704` | `bool dialect_resolves_to_turkish_rules(std::string_view dialect_id)` |
| `dig_pass` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:549` | `static const std::regex dig_pass(R"(^[0-9]+$)", std::regex::ECMAScript);` |
| `dig_re` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:164` | `static const std::regex dig_re(R"(\b\d+\b)", std::regex::ECMAScript);` |
| `expand_cardinal_digits_to_turkish_words` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:127` | `std::string expand_cardinal_digits_to_turkish_words(std::string_view s)` |
| `expand_turkish_digit_tokens_in_text` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:161` | `std::string expand_turkish_digit_tokens_in_text(std::string text)` |
| `harmony_vowel_for_kg` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:334` | `std::optional<char32_t> harmony_vowel_for_kg(const std::u32string& w,                            ...` |
| `insert_primary_stress_final` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:448` | `std::string insert_primary_stress_final(const std::string& ipa_utf8)` |
| `is_all_ascii_digits` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:25` | `bool is_all_ascii_digits(std::string_view s)` |
| `is_front_vowel` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:291` | `bool is_front_vowel(char32_t c)` |
| `is_space_cp` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:517` | `bool is_space_cp(char32_t cp)` |
| `is_tr_g2p_letter` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:227` | `bool is_tr_g2p_letter(char32_t c)` |
| `is_turkish_word_char` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:497` | `bool is_turkish_word_char(char32_t cp)` |
| `is_vowel_ipa_char` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:430` | `bool is_vowel_ipa_char(char32_t c)` |
| `is_vowel_orth` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:285` | `bool is_vowel_orth(char32_t c)` |
| `join_space` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:116` | `std::string join_space(const std::vector<std::string>& p)` |
| `last_vowel_before` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:325` | `std::optional<char32_t> last_vowel_before(const std::u32string& w, size_t end)` |
| `letters_only_u32` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:272` | `std::u32string letters_only_u32(const std::u32string& w)` |
| `map_k_or_g` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:343` | `std::string map_k_or_g(char32_t ch, const std::u32string& w, size_t i)` |
| `map_simple_char` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:355` | `std::string map_simple_char(char32_t c)` |
| `next_letter_index` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:306` | `std::optional<size_t> next_letter_index(const std::u32string& w, size_t i)` |
| `next_vowel_from` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:316` | `std::optional<char32_t> next_vowel_from(const std::u32string& w, size_t start)` |
| `prev_letter_index` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:296` | `std::optional<size_t> prev_letter_index(const std::u32string& w, size_t i)` |
| `range_re` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:162` | `static const std::regex range_re(R"(\b(\d+)-(\d+)\b)", std::regex::ECMAScript);` |
| `text_to_ipa` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:696` | `std::string TurkishRuleG2p::text_to_ipa(std::string text,                                        ...` |
| `text_to_ipa_no_expand` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:618` | `std::string TurkishRuleG2p::text_to_ipa_no_expand(     const std::string& text, std::vector<G2pWo...` |
| `turkish_lower_u32` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:218` | `std::u32string turkish_lower_u32(const std::u32string& s)` |
| `turkish_text_to_ipa` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:723` | `std::string turkish_text_to_ipa(const std::string& text, bool with_stress,                       ...` |
| `turkish_tolower_cp` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:207` | `char32_t turkish_tolower_cp(char32_t cp)` |
| `turkish_word_to_ipa` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:715` | `std::string turkish_word_to_ipa(const std::string& word, bool with_stress,                       ...` |
| `u32_to_utf8_ipa` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:440` | `std::string u32_to_utf8_ipa(const std::u32string& s)` |
| `utf8_append_codepoint` | variable | `core/moonshine-tts/src/lang-specific/turkish.cpp:6` | `extern "C" { #include <utf8proc.h> } #include <cctype> #include <cstdlib> #include <optional> #include <regex>...` |
| `utf8_ipa_to_u32` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:435` | `std::u32string utf8_ipa_to_u32(std::string_view s)` |
| `utf8_to_u32_nfc` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:196` | `std::u32string utf8_to_u32_nfc(const std::string& s)` |
| `word_to_ipa` | function | `core/moonshine-tts/src/lang-specific/turkish.cpp:534` | `std::string TurkishRuleG2p::word_to_ipa(const std::string& word) const` |
| `G2pWordLog` | struct | `core/moonshine-tts/src/lang-specific/turkish.h:11` | `` |
| `MOONSHINE_TTS_LANG_SPECIFIC_TURKISH_H` | macro | `core/moonshine-tts/src/lang-specific/turkish.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_TURKISH_H` |
| `Options` | struct | `core/moonshine-tts/src/lang-specific/turkish.h:19` | `` |
| `TurkishRuleG2p` | class | `core/moonshine-tts/src/lang-specific/turkish.h:17` | `` |
| `dialect_id` | function | `core/moonshine-tts/src/lang-specific/turkish.h:29` | `const std::string& dialect_id() const` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/turkish.h:27` | `static std::vector<std::string> dialect_ids();` |
| `dialect_resolves_to_turkish_rules` | function | `core/moonshine-tts/src/lang-specific/turkish.h:49` | `bool dialect_resolves_to_turkish_rules(std::string_view dialect_id);` |
| `expand_cardinal_digits` | function | `core/moonshine-tts/src/lang-specific/turkish.h:31` | `bool expand_cardinal_digits() const` |
| `with_stress` | function | `core/moonshine-tts/src/lang-specific/turkish.h:30` | `bool with_stress() const` |
| `UkrainianRuleG2p` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:803` | `UkrainianRuleG2p::UkrainianRuleG2p(Options options) : options_(options)` |
| `append_below_1_000_000` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:243` | `void append_below_1_000_000(int n, std::vector<std::string>& out)` |
| `append_tokens_0_999` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:224` | `void append_tokens_0_999(int n, std::vector<std::string>& out)` |
| `append_tokens_thousands_multiplier` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:203` | `void append_tokens_thousands_multiplier(int h, std::vector<std::string>& out)` |
| `append_under_100_plain` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:183` | `void append_under_100_plain(int n, std::vector<std::string>& out)` |
| `append_under_100_thousand_mult` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:134` | `void append_under_100_thousand_mult(int n, std::vector<std::string>& out)` |
| `base_cons_ipa` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:574` | `std::string base_cons_ipa(char32_t c)` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:805` | `std::vector<std::string> UkrainianRuleG2p::dialect_ids()` |
| `dialect_resolves_to_ukrainian_rules` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:917` | `bool dialect_resolves_to_ukrainian_rules(std::string_view dialect_id)` |
| `dig_pass` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:824` | `static const std::regex dig_pass(R"(^[0-9]+$)", std::regex::ECMAScript);` |
| `dig_re` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:307` | `static const std::regex dig_re(R"(\b\d+\b)", std::regex::ECMAScript);` |
| `ends_with_palatal_suffix` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:404` | `bool ends_with_palatal_suffix(const std::string& p)` |
| `expand_cardinal_digits_to_ukrainian_words` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:270` | `std::string expand_cardinal_digits_to_ukrainian_words(std::string_view s)` |
| `expand_ukrainian_digit_tokens_in_text` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:304` | `std::string expand_ukrainian_digit_tokens_in_text(std::string text)` |
| `filter_uk_word_chars` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:727` | `std::u32string filter_uk_word_chars(const std::u32string& w)` |
| `hyphen_join_word_ipas` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:776` | `std::string hyphen_join_word_ipas(const std::string& tok, bool with_stress)` |
| `insert_primary_stress_penultimate` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:533` | `std::string insert_primary_stress_penultimate(const std::string& ipa_utf8)` |
| `ipa_vowel_char` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:520` | `bool ipa_vowel_char(char32_t c)` |
| `is_all_ascii_digits` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:27` | `bool is_all_ascii_digits(std::string_view s)` |
| `is_hard_no_pal` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:351` | `bool is_hard_no_pal(char32_t c)` |
| `is_palatalizable` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:356` | `bool is_palatalizable(char32_t c)` |
| `is_soft_vowel` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:346` | `bool is_soft_vowel(char32_t c)` |
| `is_space_cp` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:761` | `bool is_space_cp(char32_t cp)` |
| `is_ukrainian_word_char` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:744` | `bool is_ukrainian_word_char(char32_t cp)` |
| `is_vowel_ipa_piece` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:410` | `bool is_vowel_ipa_piece(const std::string& p)` |
| `is_vowel_letter` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:340` | `bool is_vowel_letter(char32_t c)` |
| `join_space` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:259` | `std::string join_space(const std::vector<std::string>& p)` |
| `next_letter_index` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:363` | `std::optional<size_t> next_letter_index(const std::u32string& w, size_t start)` |
| `palatalize_last` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:452` | `void palatalize_last(std::vector<std::string>& pieces)` |
| `piece_ends_palatalized_consonant` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:434` | `bool piece_ends_palatalized_consonant(const std::vector<std::string>& pieces)` |
| `range_re` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:305` | `static const std::regex range_re(R"(\b(\d+)-(\d+)\b)", std::regex::ECMAScript);` |
| `text_to_ipa` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:909` | `std::string UkrainianRuleG2p::text_to_ipa(     std::string text, std::vector<G2pWordLog>* per_wor...` |
| `text_to_ipa_no_expand` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:832` | `std::string UkrainianRuleG2p::text_to_ipa_no_expand(     const std::string& text, std::vector<G2p...` |
| `thousand_noun_utf8` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:120` | `std::string thousand_noun_utf8(int h)` |
| `trim_ascii_ws_copy` | variable | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:6` | `extern "C" { #include <utf8proc.h> } #include <cctype> #include <cstdlib> #include <optional> #include <regex>...` |
| `u32_to_utf8` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:525` | `std::string u32_to_utf8(const std::u32string& s)` |
| `ukrainian_lower_u32` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:90` | `std::u32string ukrainian_lower_u32(const std::u32string& s)` |
| `ukrainian_strip_stress_marks_utf8` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:53` | `std::string ukrainian_strip_stress_marks_utf8(std::string s)` |
| `ukrainian_text_to_ipa` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:936` | `std::string ukrainian_text_to_ipa(const std::string& text, bool with_stress,                     ...` |
| `ukrainian_word_to_ipa` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:928` | `std::string ukrainian_word_to_ipa(const std::string& word, bool with_stress,                     ...` |
| `utf8_nfc_utf8proc` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:42` | `std::string utf8_nfc_utf8proc(const std::string& s)` |
| `utf8_to_u32_nfc` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:79` | `std::u32string utf8_to_u32_nfc(const std::string& s)` |
| `v_allophone` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:389` | `std::string v_allophone(const std::u32string& w, size_t i)` |
| `vowel_ipa` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:471` | `std::string vowel_ipa(char32_t ch, bool force_j, bool after_vowel_letter,                       b...` |
| `word_to_ipa` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:809` | `std::string UkrainianRuleG2p::word_to_ipa(const std::string& word) const` |
| `word_to_ipa_from_utf32_word` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:768` | `std::string word_to_ipa_from_utf32_word(const std::u32string& letters,                           ...` |
| `word_to_ipa_inner` | function | `core/moonshine-tts/src/lang-specific/ukrainian.cpp:621` | `std::string word_to_ipa_inner(const std::u32string& w0, bool with_stress)` |
| `G2pWordLog` | struct | `core/moonshine-tts/src/lang-specific/ukrainian.h:11` | `` |
| `MOONSHINE_TTS_LANG_SPECIFIC_UKRAINIAN_H` | macro | `core/moonshine-tts/src/lang-specific/ukrainian.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_UKRAINIAN_H` |
| `Options` | struct | `core/moonshine-tts/src/lang-specific/ukrainian.h:18` | `` |
| `UkrainianRuleG2p` | class | `core/moonshine-tts/src/lang-specific/ukrainian.h:16` | `` |
| `dialect_id` | function | `core/moonshine-tts/src/lang-specific/ukrainian.h:28` | `const std::string& dialect_id() const` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/ukrainian.h:26` | `static std::vector<std::string> dialect_ids();` |
| `dialect_resolves_to_ukrainian_rules` | function | `core/moonshine-tts/src/lang-specific/ukrainian.h:48` | `bool dialect_resolves_to_ukrainian_rules(std::string_view dialect_id);` |
| `expand_cardinal_digits` | function | `core/moonshine-tts/src/lang-specific/ukrainian.h:30` | `bool expand_cardinal_digits() const` |
| `with_stress` | function | `core/moonshine-tts/src/lang-specific/ukrainian.h:29` | `bool with_stress() const` |
| `VietnameseRuleG2p` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:785` | `VietnameseRuleG2p::VietnameseRuleG2p(std::filesystem::path dict_tsv)` |
| `VietnameseRuleG2p` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:803` | `VietnameseRuleG2p::VietnameseRuleG2p(std::string dict_tsv_utf8)` |
| `apply_tone` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:632` | `std::string apply_tone(const std::string& base, int tone, bool has_coda,                        c...` |
| `body` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:174` | `const std::string body(body_sv);` |
| `coda_obstruent_sac` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:597` | `bool coda_obstruent_sac(const std::string& coda)` |
| `coda_simple` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:323` | `std::string coda_simple(const std::string& coda, const std::string& nuc_ipa)` |
| `combine_nucleus_coda` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:555` | `std::string combine_nucleus_coda(const std::string& nuc_orth,                                  co...` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:942` | `std::vector<std::string> VietnameseRuleG2p::dialect_ids()` |
| `dialect_resolves_to_vietnamese_rules` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:947` | `bool dialect_resolves_to_vietnamese_rules(std::string_view dialect_id)` |
| `ends_with_str` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:58` | `bool ends_with_str(const std::string& s, const std::string& suf)` |
| `front_vowel_utf8` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:131` | `bool front_vowel_utf8(std::string_view s)` |
| `g2p_single_token` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:816` | `std::string VietnameseRuleG2p::g2p_single_token(std::string_view token) const` |
| `is_unicode_edge_punct` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:646` | `bool is_unicode_edge_punct(char32_t cp, bool leading)` |
| `is_vowel_first_utf8` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:119` | `bool is_vowel_first_utf8(std::string_view s)` |
| `is_vowel_letter_char` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:101` | `bool is_vowel_letter_char(char32_t cp)` |
| `load_vietnamese_lexicon_stream` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:729` | `void load_vietnamese_lexicon_stream(     std::istream& in, std::unordered_map<std::string, std::s...` |
| `max_lex_key_words` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:715` | `int max_lex_key_words(const std::unordered_map<std::string, std::string>& lex)` |
| `nucleus_to_ipa` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:355` | `std::string nucleus_to_ipa(std::string_view nuc_sv)` |
| `resolve_vietnamese_dict_path` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:955` | `std::filesystem::path resolve_vietnamese_dict_path(     const std::filesystem::path& model_root)` |
| `rime` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:295` | `const std::string rime(rime_sv);` |
| `rime_is_only_i` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:152` | `bool rime_is_only_i(std::string_view rest)` |
| `split_tone` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:64` | `int split_tone(std::string_view in, std::string& body_nfc_out)` |
| `starts_with_sv` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:54` | `bool starts_with_sv(std::string_view s, std::string_view p)` |
| `strip_edge_punct` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:670` | `std::string strip_edge_punct(std::string_view tok)` |
| `syllable_to_ipa` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:758` | `std::string VietnameseRuleG2p::syllable_to_ipa(std::string_view syllable_utf8)` |
| `text_to_ipa` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:828` | `std::string VietnameseRuleG2p::text_to_ipa(     std::string text, std::vector<G2pWordLog>* per_wo...` |
| `tmp` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:24` | `const std::string tmp(s);` |
| `tone_suffix_ipa` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:602` | `std::string tone_suffix_ipa(int tone, const std::string& coda_orth)` |
| `utf8_lower_nfc` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:35` | `std::string utf8_lower_nfc(std::string_view s)` |
| `utf8_nfc_utf8proc` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:23` | `std::string utf8_nfc_utf8proc(std::string_view s)` |
| `wants_labial_coda` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:307` | `bool wants_labial_coda(const std::string& nuc_ipa)` |
| `word_to_ipa` | function | `core/moonshine-tts/src/lang-specific/vietnamese.cpp:812` | `std::string VietnameseRuleG2p::word_to_ipa(std::string_view word) const` |
| `G2pWordLog` | struct | `core/moonshine-tts/src/lang-specific/vietnamese.h:13` | `` |
| `MOONSHINE_TTS_LANG_SPECIFIC_VIETNAMESE_H` | macro | `core/moonshine-tts/src/lang-specific/vietnamese.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_VIETNAMESE_H` |
| `VietnameseRuleG2p` | class | `core/moonshine-tts/src/lang-specific/vietnamese.h:17` | `` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/vietnamese.h:22` | `static std::vector<std::string> dialect_ids();` |
| `dialect_resolves_to_vietnamese_rules` | function | `core/moonshine-tts/src/lang-specific/vietnamese.h:42` | `bool dialect_resolves_to_vietnamese_rules(std::string_view dialect_id);` |
| `syllable_to_ipa` | function | `core/moonshine-tts/src/lang-specific/vietnamese.h:33` | `static std::string syllable_to_ipa(std::string_view syllable_utf8);` |
| `arabic_g2p_keys` | function | `core/moonshine-tts/src/moonshine-asset-catalog.cpp:74` | `std::vector<std::string> arabic_g2p_keys()` |
| `chinese_g2p_keys` | function | `core/moonshine-tts/src/moonshine-asset-catalog.cpp:48` | `std::vector<std::string> chinese_g2p_keys()` |
| `english_g2p_keys` | function | `core/moonshine-tts/src/moonshine-asset-catalog.cpp:39` | `std::vector<std::string> english_g2p_keys()` |
| `french_g2p_keys` | function | `core/moonshine-tts/src/moonshine-asset-catalog.cpp:84` | `std::vector<std::string> french_g2p_keys()` |
| `hyphen_to_underscore` | function | `core/moonshine-tts/src/moonshine-asset-catalog.cpp:30` | `std::string hyphen_to_underscore(std::string s)` |
| `japanese_g2p_keys` | function | `core/moonshine-tts/src/moonshine-asset-catalog.cpp:58` | `std::vector<std::string> japanese_g2p_keys()` |
| `korean_g2p_keys` | function | `core/moonshine-tts/src/moonshine-asset-catalog.cpp:68` | `std::vector<std::string> korean_g2p_keys()` |
| `lookup_g2p_dependency_keys` | function | `core/moonshine-tts/src/moonshine-asset-catalog.cpp:223` | `std::optional<std::vector<std::string>> lookup_g2p_dependency_keys(     std::string_view raw)` |
| `moonshine_asset_catalog_all_g2p_dependency_keys_union` | function | `core/moonshine-tts/src/moonshine-asset-catalog.cpp:254` | `std::vector<std::string> moonshine_asset_catalog_all_g2p_dependency_keys_union()` |
| `moonshine_asset_catalog_all_registered_language_tags` | function | `core/moonshine-tts/src/moonshine-asset-catalog.cpp:268` | `std::vector<std::string> moonshine_asset_catalog_all_registered_language_tags()` |
| `moonshine_asset_catalog_g2p_dependency_keys` | function | `core/moonshine-tts/src/moonshine-asset-catalog.cpp:249` | `std::optional<std::vector<std::string>> moonshine_asset_catalog_g2p_dependency_keys(std::string_v...` |
| `moonshine_asset_catalog_populate_default_g2p_files` | function | `core/moonshine-tts/src/moonshine-asset-catalog.cpp:240` | `void moonshine_asset_catalog_populate_default_g2p_files(     FileInformationMap& files)` |
| `normalize_lang_key_cli` | function | `core/moonshine-tts/src/moonshine-asset-catalog.cpp:16` | `std::string normalize_lang_key_cli(std::string_view raw)` |
| `MOONSHINE_TTS_ASSET_CATALOG_H` | macro | `core/moonshine-tts/src/moonshine-asset-catalog.h:2` | `#define MOONSHINE_TTS_ASSET_CATALOG_H` |
| `moonshine_asset_catalog_populate_default_g2p_files` | function | `core/moonshine-tts/src/moonshine-asset-catalog.h:15` | `void moonshine_asset_catalog_populate_default_g2p_files( FileInformationMap& files);` |
| `MoonshineG2POptions` | function | `core/moonshine-tts/src/moonshine-g2p-options.cpp:132` | `MoonshineG2POptions::MoonshineG2POptions()` |
| `asset_is_available` | function | `core/moonshine-tts/src/moonshine-g2p-options.cpp:159` | `bool MoonshineG2POptions::asset_is_available(     std::string_view canonical_key) const` |
| `is_known_g2p_option` | function | `core/moonshine-tts/src/moonshine-g2p-options.cpp:45` | `bool is_known_g2p_option(std::string_view key)` |
| `k` | function | `core/moonshine-tts/src/moonshine-g2p-options.cpp:138` | `const std::string k(canonical_key);` |
| `optional_override_path` | function | `core/moonshine-tts/src/moonshine-g2p-options.cpp:147` | `std::optional<std::filesystem::path> MoonshineG2POptions::optional_override_path(std::string_view...` |
| `optional_path_from_string` | function | `core/moonshine-tts/src/moonshine-g2p-options.cpp:15` | `std::optional<std::filesystem::path> optional_path_from_string(     const std::string& value)` |
| `out` | function | `core/moonshine-tts/src/moonshine-g2p-options.cpp:188` | `std::vector<uint8_t> out(p, p + n);` |
| `parse_options` | function | `core/moonshine-tts/src/moonshine-g2p-options.cpp:199` | `void MoonshineG2POptions::parse_options(     const std::vector<std::pair<std::string, std::string...` |
| `prepare_g2p_file_information_path` | function | `core/moonshine-tts/src/moonshine-g2p-options.cpp:108` | `void prepare_g2p_file_information_path(FileInformation& fi,                                      ...` |
| `read_binary_asset` | function | `core/moonshine-tts/src/moonshine-g2p-options.cpp:175` | `std::vector<uint8_t> MoonshineG2POptions::read_binary_asset(     std::string_view canonical_key) ...` |
| `read_utf8_asset` | function | `core/moonshine-tts/src/moonshine-g2p-options.cpp:193` | `std::string MoonshineG2POptions::read_utf8_asset(     std::string_view canonical_key) const` |
| `relative_asset_path` | function | `core/moonshine-tts/src/moonshine-g2p-options.cpp:136` | `std::filesystem::path MoonshineG2POptions::relative_asset_path(     std::string_view canonical_ke...` |
| `set_canonical_file` | function | `core/moonshine-tts/src/moonshine-g2p-options.cpp:24` | `void set_canonical_file(FileInformationMap& files,                         std::string_view canon...` |
| `set_override_file` | function | `core/moonshine-tts/src/moonshine-g2p-options.cpp:35` | `void set_override_file(FileInformationMap& files, std::string_view map_key,                      ...` |
| `MOONSHINE_TTS_MOONSHINE_G2P_OPTIONS_H` | macro | `core/moonshine-tts/src/moonshine-g2p-options.h:2` | `#define MOONSHINE_TTS_MOONSHINE_G2P_OPTIONS_H` |
| `MoonshineG2POptions` | struct | `core/moonshine-tts/src/moonshine-g2p-options.h:134` | `` |
| `asset_is_available` | function | `core/moonshine-tts/src/moonshine-g2p-options.h:186` | `bool asset_is_available(std::string_view canonical_key) const;` |
| `g2p_bundle_file_key` | function | `core/moonshine-tts/src/moonshine-g2p-options.h:18` | `inline std::string g2p_bundle_file_key(std::string_view bundle_dir_key,                          ...` |
| `parse_options` | function | `core/moonshine-tts/src/moonshine-g2p-options.h:198` | `void parse_options( const std::vector<std::pair<std::string, std::string>>& options);` |
| `read_binary_asset` | function | `core/moonshine-tts/src/moonshine-g2p-options.h:190` | `std::vector<uint8_t> read_binary_asset(std::string_view canonical_key) const;` |
| `MoonshineG2P` | function | `core/moonshine-tts/src/moonshine-g2p.cpp:186` | `MoonshineG2P::MoonshineG2P(std::string dialect_id,                            MoonshineG2POptions...` |
| `dialect_resolves_to_spanish_rules` | function | `core/moonshine-tts/src/moonshine-g2p.cpp:108` | `bool dialect_resolves_to_spanish_rules(std::string_view dialect_id,                              ...` |
| `dialect_uses_rule_based_g2p` | function | `core/moonshine-tts/src/moonshine-g2p.cpp:122` | `bool dialect_uses_rule_based_g2p(std::string_view dialect_id,                                  co...` |
| `normalize_spanish_dialect_cli_key` | function | `core/moonshine-tts/src/moonshine-g2p.cpp:45` | `std::string normalize_spanish_dialect_cli_key(std::string_view raw)` |
| `rule_backend_name` | function | `core/moonshine-tts/src/moonshine-g2p.cpp:68` | `const char* rule_backend_name(RuleBasedG2pKind k)` |
| `text_to_ipa` | function | `core/moonshine-tts/src/moonshine-g2p.cpp:217` | `std::string MoonshineG2P::text_to_ipa(std::string_view text,                                     ...` |
| `trim_copy` | function | `core/moonshine-tts/src/moonshine-g2p.cpp:31` | `std::string trim_copy(std::string_view s)` |
| `MOONSHINE_TTS_G2P_H` | macro | `core/moonshine-tts/src/moonshine-g2p.h:2` | `#define MOONSHINE_TTS_G2P_H` |
| `MoonshineG2P` | class | `core/moonshine-tts/src/moonshine-g2p.h:34` | `` |
| `dialect_id` | function | `core/moonshine-tts/src/moonshine-g2p.h:103` | `const std::string& dialect_id() const` |
| `dialect_resolves_to_spanish_rules` | function | `core/moonshine-tts/src/moonshine-g2p.h:20` | `bool dialect_resolves_to_spanish_rules(std::string_view dialect_id, bool spanish_narrow_obstruents = true);` |
| `uses_arabic_rules` | function | `core/moonshine-tts/src/moonshine-g2p.h:78` | `bool uses_arabic_rules() const` |
| `uses_chinese_rules` | function | `core/moonshine-tts/src/moonshine-g2p.h:66` | `bool uses_chinese_rules() const` |
| `uses_dutch_rules` | function | `core/moonshine-tts/src/moonshine-g2p.h:57` | `bool uses_dutch_rules() const` |
| `uses_english_rules` | function | `core/moonshine-tts/src/moonshine-g2p.h:93` | `bool uses_english_rules() const` |
| `uses_french_rules` | function | `core/moonshine-tts/src/moonshine-g2p.h:54` | `bool uses_french_rules() const` |
| `uses_german_rules` | function | `core/moonshine-tts/src/moonshine-g2p.h:51` | `bool uses_german_rules() const` |
| `uses_hindi_rules` | function | `core/moonshine-tts/src/moonshine-g2p.h:90` | `bool uses_hindi_rules() const` |
| `uses_italian_rules` | function | `core/moonshine-tts/src/moonshine-g2p.h:60` | `bool uses_italian_rules() const` |
| `uses_japanese_rules` | function | `core/moonshine-tts/src/moonshine-g2p.h:75` | `bool uses_japanese_rules() const` |
| `uses_korean_rules` | function | `core/moonshine-tts/src/moonshine-g2p.h:69` | `bool uses_korean_rules() const` |
| `uses_onnx` | function | `core/moonshine-tts/src/moonshine-g2p.h:99` | `static constexpr bool uses_onnx()` |
| `uses_portuguese_rules` | function | `core/moonshine-tts/src/moonshine-g2p.h:81` | `bool uses_portuguese_rules() const` |
| `uses_russian_rules` | function | `core/moonshine-tts/src/moonshine-g2p.h:63` | `bool uses_russian_rules() const` |
| `uses_spanish_rules` | function | `core/moonshine-tts/src/moonshine-g2p.h:48` | `bool uses_spanish_rules() const` |
| `uses_turkish_rules` | function | `core/moonshine-tts/src/moonshine-g2p.h:84` | `bool uses_turkish_rules() const` |
| `uses_ukrainian_rules` | function | `core/moonshine-tts/src/moonshine-g2p.h:87` | `bool uses_ukrainian_rules() const` |
| `uses_vietnamese_rules` | function | `core/moonshine-tts/src/moonshine-g2p.h:72` | `bool uses_vietnamese_rules() const` |
| `MoonshineTTSOptions` | function | `core/moonshine-tts/src/moonshine-tts-options.cpp:39` | `MoonshineTTSOptions::MoonshineTTSOptions()` |
| `apply_synthesis_output_effects` | function | `core/moonshine-tts/src/moonshine-tts-options.cpp:13` | `void apply_synthesis_output_effects(std::vector<float>& audio,                                   ...` |
| `apply_voice_engine_prefix` | function | `core/moonshine-tts/src/moonshine-tts-options.cpp:46` | `void MoonshineTTSOptions::apply_voice_engine_prefix()` |
| `d` | function | `core/moonshine-tts/src/moonshine-tts-options.cpp:121` | `const std::filesystem::path d(t);` |
| `k` | function | `core/moonshine-tts/src/moonshine-tts-options.cpp:74` | `const std::string k(canonical_key);` |
| `parse_options` | function | `core/moonshine-tts/src/moonshine-tts-options.cpp:82` | `void MoonshineTTSOptions::parse_options(     const std::vector<std::pair<std::string, std::string...` |
| `tts_relative_path` | function | `core/moonshine-tts/src/moonshine-tts-options.cpp:72` | `std::filesystem::path MoonshineTTSOptions::tts_relative_path(     std::string_view canonical_key)...` |
| `MOONSHINE_TTS_MOONSHINE_TTS_OPTIONS_H` | macro | `core/moonshine-tts/src/moonshine-tts-options.h:2` | `#define MOONSHINE_TTS_MOONSHINE_TTS_OPTIONS_H` |
| `MoonshineTTSOptions` | struct | `core/moonshine-tts/src/moonshine-tts-options.h:63` | `` |
| `apply_synthesis_output_effects` | function | `core/moonshine-tts/src/moonshine-tts-options.h:149` | `void apply_synthesis_output_effects(std::vector<float>& audio, bool normalize_audio, float volume);` |
| `apply_voice_engine_prefix` | function | `core/moonshine-tts/src/moonshine-tts-options.h:142` | `void apply_voice_engine_prefix();` |
| `parse_options` | function | `core/moonshine-tts/src/moonshine-tts-options.h:134` | `void parse_options( const std::vector<std::pair<std::string, std::string>>& options, std::string* cli_language =...` |
| `Impl` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1330` | `explicit Impl(std::string_view language, const MoonshineTTSOptions& opt_in)` |
| `KokoroTtsEngine` | struct | `core/moonshine-tts/src/moonshine-tts.cpp:960` | `` |
| `KokoroTtsEngine` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1043` | `explicit KokoroTtsEngine(std::string_view language, MoonshineTTSOptions opt)` |
| `LangProfile` | struct | `core/moonshine-tts/src/moonshine-tts.cpp:158` | `` |
| `MoonshineTTS` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1503` | `MoonshineTTS::MoonshineTTS(std::string_view language,                            const MoonshineT...` |
| `SynthesisOverrides` | struct | `core/moonshine-tts/src/moonshine-tts.cpp:70` | `` |
| `apply_chinese_kokoro_normalization` | function | `core/moonshine-tts/src/moonshine-tts.cpp:461` | `void apply_chinese_kokoro_normalization(std::string& ipa)` |
| `apply_diphthong_map` | function | `core/moonshine-tts/src/moonshine-tts.cpp:428` | `void apply_diphthong_map(std::string& s, char kokoro_lang)` |

Next: [SYMBOLS_p6.md](SYMBOLS_p6.md)
