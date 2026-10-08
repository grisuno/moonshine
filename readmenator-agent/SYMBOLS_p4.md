# Symbols (page 4 of 12)
Previous: [SYMBOLS_p3.md](SYMBOLS_p3.md)

| Symbol | Kind | File:Line | Signature |
|--------|------|-----------|-----------|
| `token_has_g2p_content` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:50` | `bool token_has_g2p_content(const std::string& tok)` |
| `trim_copy_line` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:23` | `std::string trim_copy_line(std::string_view s)` |
| `try_consume_g2p_token` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:96` | `bool try_consume_g2p_token(const std::string& text, size_t pos,                            size_t...` |
| `verb_like_pos` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:78` | `const std::unordered_set<std::string>& verb_like_pos()` |
| `w` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:249` | `const std::string w(word);` |
| `word_to_ipa` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:488` | `std::string ChineseRuleG2p::word_to_ipa(std::string_view word) const` |
| `word_to_ipa_with_pos` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:492` | `std::string ChineseRuleG2p::word_to_ipa_with_pos(std::string_view word,                          ...` |
| `ChineseRuleG2p` | class | `core/moonshine-tts/src/lang-specific/chinese.h:23` | `` |
| `G2pWordLog` | struct | `core/moonshine-tts/src/lang-specific/chinese.h:14` | `` |
| `MOONSHINE_TTS_LANG_SPECIFIC_CHINESE_H` | macro | `core/moonshine-tts/src/lang-specific/chinese.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_CHINESE_H` |
| `dialect_id` | function | `core/moonshine-tts/src/lang-specific/chinese.h:30` | `const std::string& dialect_id() const` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/chinese.h:28` | `static std::vector<std::string> dialect_ids();` |
| `dialect_resolves_to_chinese_rules` | function | `core/moonshine-tts/src/lang-specific/chinese.h:57` | `bool dialect_resolves_to_chinese_rules(std::string_view dialect_id);` |
| `CmudictTsv` | function | `core/moonshine-tts/src/lang-specific/cmudict-tsv.cpp:58` | `CmudictTsv::CmudictTsv(const std::filesystem::path& path)` |
| `CmudictTsv` | function | `core/moonshine-tts/src/lang-specific/cmudict-tsv.cpp:66` | `CmudictTsv::CmudictTsv(std::string_view utf8_contents)` |
| `buf` | function | `core/moonshine-tts/src/lang-specific/cmudict-tsv.cpp:67` | `const std::string buf(utf8_contents);` |
| `k` | function | `core/moonshine-tts/src/lang-specific/cmudict-tsv.cpp:73` | `const std::string k(key.begin(), key.end());` |
| `lookup` | function | `core/moonshine-tts/src/lang-specific/cmudict-tsv.cpp:72` | `const std::vector<std::string>* CmudictTsv::lookup(std::string_view key) const` |
| `parse_cmudict_tsv_lines` | function | `core/moonshine-tts/src/lang-specific/cmudict-tsv.cpp:14` | `void parse_cmudict_tsv_lines(     std::istream& in,     std::unordered_map<std::string, std::vect...` |
| `CmudictTsv` | class | `core/moonshine-tts/src/lang-specific/cmudict-tsv.h:14` | `` |
| `MOONSHINE_TTS_CMUDICT_TSV_H` | macro | `core/moonshine-tts/src/lang-specific/cmudict-tsv.h:2` | `#define MOONSHINE_TTS_CMUDICT_TSV_H` |
| `lookup` | function | `core/moonshine-tts/src/lang-specific/cmudict-tsv.h:19` | `const std::vector<std::string>* lookup(std::string_view key) const;` |
| `DutchRuleG2p` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:1522` | `DutchRuleG2p::DutchRuleG2p(std::filesystem::path dict_tsv, Options options)     : options_(options)` |
| `DutchRuleG2p` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:1527` | `DutchRuleG2p::DutchRuleG2p(std::string dict_tsv_utf8, Options options)     : options_(options)` |
| `Slot` | struct | `core/moonshine-tts/src/lang-specific/dutch.cpp:626` | `` |
| `all_ascii_digits_string` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:544` | `bool all_ascii_digits_string(const std::string& s)` |
| `append_lexicon_folded` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:102` | `void append_lexicon_folded(std::string& out, char32_t cl)` |
| `apply_lexicon_ipa_postprocess` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:556` | `std::string apply_lexicon_ipa_postprocess(std::string ipa,                                       ...` |
| `below_100` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:237` | `std::string below_100(int n)` |
| `below_1000_spaced` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:256` | `std::string below_1000_spaced(int n)` |
| `below_1_000_000_v2` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:323` | `std::string below_1_000_000_v2(int n)` |
| `default_stress_syllable_index` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:871` | `size_t default_stress_syllable_index(const std::vector<std::u32string>& syls,                    ...` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:1471` | `std::vector<std::string> DutchRuleG2p::dialect_ids()` |
| `dialect_resolves_to_dutch_rules` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:1463` | `bool dialect_resolves_to_dutch_rules(std::string_view dialect_id)` |
| `digit_pass_through_pattern` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:520` | `bool digit_pass_through_pattern(std::string_view raw)` |
| `dutch_orthographic_syllables_u32` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:793` | `std::vector<std::u32string> dutch_orthographic_syllables_u32(     const std::u32string& word)` |
| `dutch_unicode_tolower_cp` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:31` | `char32_t dutch_unicode_tolower_cp(char32_t c)` |
| `expand_cardinal_digits_to_dutch_words` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:339` | `std::string expand_cardinal_digits_to_dutch_words(std::string_view sv)` |
| `expand_digit_tokens_in_text` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:469` | `std::string expand_digit_tokens_in_text(std::string_view text_sv)` |
| `final_devoice_obstruents` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:1045` | `std::string final_devoice_obstruents(std::string ipa)` |
| `finalize_ipa` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:1533` | `std::string DutchRuleG2p::finalize_ipa(std::string ipa,                                        bo...` |
| `fix_thousands_compound` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:310` | `std::string fix_thousands_compound(int q)` |
| `from_1000_to_9999` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:278` | `std::string from_1000_to_9999(int n)` |
| `insert_primary_stress_before_vowel_dutch` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:916` | `std::string insert_primary_stress_before_vowel_dutch(std::string s)` |
| `ipa_at_stress_mark_dutch` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:998` | `bool ipa_at_stress_mark_dutch(const std::string& ipa, size_t j)` |
| `ipa_skip_pre_nucleus_dutch` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:1007` | `size_t ipa_skip_pre_nucleus_dutch(std::string_view s, size_t j)` |
| `ipa_starts_with_nucleus_dutch` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:959` | `bool ipa_starts_with_nucleus_dutch(std::string_view rest)` |
| `is_ascii_digit` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:371` | `bool is_ascii_digit(char c)` |
| `is_dutch_word_char` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:408` | `bool is_dutch_word_char(char32_t cp)` |
| `is_grapheme_char` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:178` | `bool is_grapheme_char(char32_t cl)` |
| `is_latin1_supplement_python_word_char` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:373` | `bool is_latin1_supplement_python_word_char(char32_t cp)` |
| `is_letterlike_math_word_char` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:403` | `bool is_letterlike_math_word_char(char32_t cp)` |
| `is_vowel_letter32` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:689` | `bool is_vowel_letter32(char32_t c)` |
| `join_unit_tens` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:221` | `std::string join_unit_tens(int u, std::string_view tens_word)` |
| `kTeenWord` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:212` | `static const char* kTeenWord(int n)` |
| `letters_to_ipa_no_stress` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:1083` | `std::string letters_to_ipa_no_stress(const std::u32string& syl_in,                               ...` |
| `load_dutch_lexicon_file` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:678` | `void load_dutch_lexicon_file(     const std::filesystem::path& path,     std::unordered_map<std::...` |
| `load_dutch_lexicon_stream` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:624` | `void load_dutch_lexicon_stream(     std::istream& in, std::unordered_map<std::string, std::string...` |
| `lookup_or_rules` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:1546` | `std::string DutchRuleG2p::lookup_or_rules(const std::string& raw_word) const` |
| `normalize_grapheme_key_u32` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:190` | `std::u32string normalize_grapheme_key_u32(const std::string& word)` |
| `normalize_ipa_stress_for_vocoder` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:1475` | `std::string DutchRuleG2p::normalize_ipa_stress_for_vocoder(std::string ipa)` |
| `normalize_lexicon_key_utf8` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:160` | `std::string normalize_lexicon_key_utf8(const std::string& word)` |
| `prev_utf8_index` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:437` | `size_t prev_utf8_index(const std::string& t, size_t byte_i)` |
| `remove_if` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:851` | `std::remove_if(syllables.begin(), syllables.end(),                      [](const std::u32string& sy)` |
| `resolve_dutch_dict_path` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:1458` | `std::filesystem::path resolve_dutch_dict_path(     const std::filesystem::path& model_root)` |
| `rules_word_to_ipa_utf8` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:1426` | `std::string rules_word_to_ipa_utf8(const std::string& raw_word,                                  ...` |
| `stressed_syllable_from_acute` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:732` | `std::optional<size_t> stressed_syllable_from_acute(     const std::vector<std::u32string>& syllab...` |
| `strip_hyphens_u32` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:1416` | `std::u32string strip_hyphens_u32(const std::u32string& w)` |
| `strip_to_plain_vowel` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:699` | `char32_t strip_to_plain_vowel(char32_t c)` |
| `text_to_ipa` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:1699` | `std::string DutchRuleG2p::text_to_ipa(std::string text,                                       std...` |
| `text_to_ipa_no_expand` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:1623` | `std::string DutchRuleG2p::text_to_ipa_no_expand(     const std::string& text, std::vector<G2pWord...` |
| `unstressed_prefix_len_u32` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:857` | `size_t unstressed_prefix_len_u32(const std::u32string& wl)` |
| `word_boundary_after` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:459` | `bool word_boundary_after(const std::string& t, size_t byte_i)` |
| `word_boundary_before` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:448` | `bool word_boundary_before(const std::string& t, size_t byte_i)` |
| `word_has_written_stress_u32` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:723` | `bool word_has_written_stress_u32(const std::u32string& w)` |
| `word_to_ipa` | function | `core/moonshine-tts/src/lang-specific/dutch.cpp:1602` | `std::string DutchRuleG2p::word_to_ipa(const std::string& word) const` |
| `DutchRuleG2p` | class | `core/moonshine-tts/src/lang-specific/dutch.h:18` | `` |
| `G2pWordLog` | struct | `core/moonshine-tts/src/lang-specific/dutch.h:14` | `` |
| `MOONSHINE_TTS_LANG_SPECIFIC_DUTCH_H` | macro | `core/moonshine-tts/src/lang-specific/dutch.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_DUTCH_H` |
| `Options` | struct | `core/moonshine-tts/src/lang-specific/dutch.h:20` | `` |
| `dialect_id` | function | `core/moonshine-tts/src/lang-specific/dutch.h:38` | `const std::string& dialect_id() const` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/dutch.h:36` | `static std::vector<std::string> dialect_ids();` |
| `dialect_resolves_to_dutch_rules` | function | `core/moonshine-tts/src/lang-specific/dutch.h:62` | `bool dialect_resolves_to_dutch_rules(std::string_view dialect_id);` |
| `normalize_ipa_stress_for_vocoder` | function | `core/moonshine-tts/src/lang-specific/dutch.h:48` | `static std::string normalize_ipa_stress_for_vocoder(std::string ipa);` |
| `Literal` | struct | `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:124` | `` |
| `add_primary_stress_if_missing` | function | `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:320` | `std::string add_primary_stress_if_missing(std::string s)` |
| `english_hand_oov_rules_ipa` | function | `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:438` | `std::string english_hand_oov_rules_ipa(std::string_view word)` |
| `is_consonant` | function | `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:54` | `constexpr bool is_consonant(char c)` |
| `is_vowel` | function | `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:50` | `constexpr bool is_vowel(char c)` |
| `last_ipa_unit_is_vowel` | function | `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:38` | `bool last_ipa_unit_is_vowel(std::string_view prev)` |
| `last_utf8_char` | function | `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:23` | `std::string_view last_utf8_char(std::string_view s)` |
| `magic_e_lengthens` | function | `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:67` | `bool magic_e_lengthens(std::string_view w, int vowel_i)` |
| `next_vowel_index` | function | `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:58` | `int next_vowel_index(std::string_view w, int start)` |
| `oov_grapheme_to_ipa` | function | `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:341` | `std::string oov_grapheme_to_ipa(std::string_view word)` |
| `oov_single_consonant` | function | `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:163` | `std::string oov_single_consonant(char c, std::string_view w, int i)` |
| `p` | function | `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:329` | `const std::string_view p(pref);` |
| `th_voiced_word` | function | `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:157` | `bool th_voiced_word(std::string_view w)` |
| `utf8_starts_with` | function | `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:19` | `bool utf8_starts_with(const std::string& s, std::string_view p)` |
| `MOONSHINE_TTS_LANG_SPECIFIC_ENGLISH_HAND_OOV_H` | macro | `core/moonshine-tts/src/lang-specific/english-hand-oov.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_ENGLISH_HAND_OOV_H` |
| `Scale` | struct | `core/moonshine-tts/src/lang-specific/english-numbers.cpp:74` | `` |
| `cardinal_non_negative_ipa` | function | `core/moonshine-tts/src/lang-specific/english-numbers.cpp:64` | `std::optional<std::string> cardinal_non_negative_ipa(long long n)` |
| `digit_sequence_ipa` | function | `core/moonshine-tts/src/lang-specific/english-numbers.cpp:22` | `std::string digit_sequence_ipa(std::string_view digits)` |
| `english_number_token_ipa` | function | `core/moonshine-tts/src/lang-specific/english-numbers.cpp:200` | `std::optional<std::string> english_number_token_ipa(std::string_view token)` |
| `integer_decimal_string_ipa` | function | `core/moonshine-tts/src/lang-specific/english-numbers.cpp:107` | `std::optional<std::string> integer_decimal_string_ipa(std::string s)` |
| `under_1000_ipa` | function | `core/moonshine-tts/src/lang-specific/english-numbers.cpp:51` | `std::string under_1000_ipa(int n)` |
| `under_100_ipa` | function | `core/moonshine-tts/src/lang-specific/english-numbers.cpp:35` | `std::string under_100_ipa(int n)` |
| `MOONSHINE_TTS_LANG_SPECIFIC_ENGLISH_NUMBERS_H` | macro | `core/moonshine-tts/src/lang-specific/english-numbers.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_ENGLISH_NUMBERS_H` |
| `EnglishRuleG2p` | function | `core/moonshine-tts/src/lang-specific/english.cpp:82` | `EnglishRuleG2p::EnglishRuleG2p(     std::filesystem::path dict_tsv,     std::optional<std::filesy...` |
| `EnglishRuleG2p` | function | `core/moonshine-tts/src/lang-specific/english.cpp:110` | `EnglishRuleG2p::EnglishRuleG2p(     std::string dict_tsv_utf8, std::optional<std::filesystem::pat...` |
| `append_log` | function | `core/moonshine-tts/src/lang-specific/english.cpp:31` | `void append_log(std::vector<G2pWordLog>* out, G2pWordLog entry)` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/english.cpp:140` | `std::vector<std::string> EnglishRuleG2p::dialect_ids()` |
| `dialect_is_british_english_variant` | function | `core/moonshine-tts/src/lang-specific/english.cpp:239` | `bool dialect_is_british_english_variant(std::string_view dialect_id)` |
| `dialect_resolves_to_english_rules` | function | `core/moonshine-tts/src/lang-specific/english.cpp:244` | `bool dialect_resolves_to_english_rules(std::string_view dialect_id)` |
| `pick_english_heteronym_ipa` | function | `core/moonshine-tts/src/lang-specific/english.cpp:40` | `std::string pick_english_heteronym_ipa(std::vector<std::string> alts,                            ...` |
| `text_to_ipa` | function | `core/moonshine-tts/src/lang-specific/english.cpp:146` | `std::string EnglishRuleG2p::text_to_ipa(std::string text,                                        ...` |
| `EnglishOnnxAuxMemory` | struct | `core/moonshine-tts/src/lang-specific/english.h:20` | `` |
| `EnglishRuleG2p` | class | `core/moonshine-tts/src/lang-specific/english.h:26` | `` |
| `G2pWordLog` | struct | `core/moonshine-tts/src/lang-specific/english.h:16` | `` |
| `Impl` | struct | `core/moonshine-tts/src/lang-specific/english.h:58` | `` |
| `MOONSHINE_TTS_LANG_SPECIFIC_ENGLISH_H` | macro | `core/moonshine-tts/src/lang-specific/english.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_ENGLISH_H` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/english.h:51` | `static std::vector<std::string> dialect_ids();` |
| `dialect_is_british_english_variant` | function | `core/moonshine-tts/src/lang-specific/english.h:72` | `bool dialect_is_british_english_variant(std::string_view dialect_id);` |
| `dialect_resolves_to_english_rules` | function | `core/moonshine-tts/src/lang-specific/english.h:67` | `bool dialect_resolves_to_english_rules(std::string_view dialect_id);` |
| `MOONSHINE_TTS_LANG_SPECIFIC_FRENCH_COMPOUND_MAP_H` | macro | `core/moonshine-tts/src/lang-specific/french-compound-map.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_FRENCH_COMPOUND_MAP_H` |
| `MOONSHINE_TTS_LANG_SPECIFIC_FRENCH_INTERNAL_H` | macro | `core/moonshine-tts/src/lang-specific/french-internal.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_FRENCH_INTERNAL_H` |
| `french_tolower_cp` | function | `core/moonshine-tts/src/lang-specific/french-oov.cpp:17` | `char32_t french_tolower_cp(char32_t c)` |
| `insert_stress_final_syllable` | function | `core/moonshine-tts/src/lang-specific/french-oov.cpp:120` | `std::string insert_stress_final_syllable(std::string ipa)` |
| `is_allowed_ortho_cp` | function | `core/moonshine-tts/src/lang-specific/french-oov.cpp:64` | `bool is_allowed_ortho_cp(char32_t c)` |
| `letters_only_u32` | function | `core/moonshine-tts/src/lang-specific/french-oov.cpp:75` | `std::u32string letters_only_u32(const std::string& raw)` |
| `ms` | function | `core/moonshine-tts/src/lang-specific/french-oov.cpp:127` | `const std::string ms(m);` |
| `oov_word_to_ipa` | function | `core/moonshine-tts/src/lang-specific/french-oov.cpp:690` | `std::string oov_word_to_ipa(const std::string& word, bool with_stress)` |
| `peek_eq` | function | `core/moonshine-tts/src/lang-specific/french-oov.cpp:315` | `bool peek_eq(const std::u32string& w, size_t i, const char* ascii)` |
| `prev_is_nucleus_idx` | function | `core/moonshine-tts/src/lang-specific/french-oov.cpp:168` | `bool prev_is_nucleus_idx(const std::string& s, int idx)` |
| `scan_graphemes` | function | `core/moonshine-tts/src/lang-specific/french-oov.cpp:328` | `std::string scan_graphemes(const std::u32string& w)` |
| `trim_final_by_orthography` | function | `core/moonshine-tts/src/lang-specific/french-oov.cpp:242` | `std::string trim_final_by_orthography(std::string ipa,                                       cons...` |
| `utf8_last_cp_start` | function | `core/moonshine-tts/src/lang-specific/french-oov.cpp:214` | `size_t utf8_last_cp_start(const std::string& s)` |
| `utf8_prev_cp_start` | function | `core/moonshine-tts/src/lang-specific/french-oov.cpp:228` | `size_t utf8_prev_cp_start(const std::string& s, size_t cp_start)` |
| `v_u32` | function | `core/moonshine-tts/src/lang-specific/french-oov.cpp:90` | `bool v_u32(char32_t ch)` |
| `FrenchRuleG2p` | function | `core/moonshine-tts/src/lang-specific/french.cpp:1091` | `FrenchRuleG2p::FrenchRuleG2p(std::filesystem::path dict_tsv,                              std::fi...` |
| `FrenchRuleG2p` | function | `core/moonshine-tts/src/lang-specific/french.cpp:1098` | `FrenchRuleG2p::FrenchRuleG2p(std::string dict_tsv_utf8,                              std::filesys...` |
| `LiaisonStrength` | enum | `core/moonshine-tts/src/lang-specific/french.cpp:921` | `` |
| `LiaisonStrength` | class | `core/moonshine-tts/src/lang-specific/french.cpp:921` | `` |
| `Tok` | struct | `core/moonshine-tts/src/lang-specific/french.cpp:1188` | `` |
| `all_of` | function | `core/moonshine-tts/src/lang-specific/french.cpp:1328` | `std::all_of(t.s.begin(), t.s.end(), [](unsigned char c)` |
| `below_100` | function | `core/moonshine-tts/src/lang-specific/french.cpp:350` | `std::vector<std::string> below_100(int n)` |
| `below_1000` | function | `core/moonshine-tts/src/lang-specific/french.cpp:413` | `std::vector<std::string> below_1000(int n)` |
| `below_1_000_000` | function | `core/moonshine-tts/src/lang-specific/french.cpp:447` | `std::vector<std::string> below_1_000_000(int n)` |
| `categories_for_form` | function | `core/moonshine-tts/src/lang-specific/french.cpp:565` | `std::vector<std::string> categories_for_form(     const std::string& word,     const std::unorder...` |
| `classify_pos` | function | `core/moonshine-tts/src/lang-specific/french.cpp:583` | `std::optional<std::string> classify_pos(     const std::string& word,     const std::unordered_ma...` |
| `closed_liaison_determiners` | function | `core/moonshine-tts/src/lang-specific/french.cpp:552` | `const std::unordered_set<std::string>& closed_liaison_determiners()` |
| `count_primary_stress_marks` | function | `core/moonshine-tts/src/lang-specific/french.cpp:1039` | `size_t count_primary_stress_marks(const std::string& s)` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/french.cpp:1369` | `std::vector<std::string> FrenchRuleG2p::dialect_ids()` |
| `dialect_resolves_to_french_rules` | function | `core/moonshine-tts/src/lang-specific/french.cpp:1361` | `bool dialect_resolves_to_french_rules(std::string_view dialect_id)` |
| `ensure_french_nuclear_stress` | function | `core/moonshine-tts/src/lang-specific/french.cpp:1051` | `std::string FrenchRuleG2p::ensure_french_nuclear_stress(std::string ipa)` |
| `expand_cardinal_digits_to_french_words` | function | `core/moonshine-tts/src/lang-specific/french.cpp:494` | `std::string expand_cardinal_digits_to_french_words(std::string_view s)` |
| `expand_digit_tokens_in_text` | function | `core/moonshine-tts/src/lang-specific/french.cpp:518` | `std::string expand_digit_tokens_in_text(const std::string& text)` |
| `finalize_word_ipa` | function | `core/moonshine-tts/src/lang-specific/french.cpp:1116` | `std::string FrenchRuleG2p::finalize_word_ipa(std::string ipa,                                    ...` |
| `french_nucleus_prefixes` | function | `core/moonshine-tts/src/lang-specific/french.cpp:643` | `const std::vector<std::string>& french_nucleus_prefixes()` |
| `french_tolower_cp` | function | `core/moonshine-tts/src/lang-specific/french.cpp:30` | `char32_t french_tolower_cp(char32_t c)` |
| `h_aspire_set` | function | `core/moonshine-tts/src/lang-specific/french.cpp:541` | `const std::unordered_set<std::string>& h_aspire_set()` |
| `ipa_ends_with_audible_consonant` | function | `core/moonshine-tts/src/lang-specific/french.cpp:850` | `bool ipa_ends_with_audible_consonant(std::string_view ipa_sv)` |
| `ipa_starts_with_vowel_sound` | function | `core/moonshine-tts/src/lang-specific/french.cpp:767` | `bool ipa_starts_with_vowel_sound(std::string_view ipa_sv)` |
| `is_all_ascii_digits` | function | `core/moonshine-tts/src/lang-specific/french.cpp:482` | `bool is_all_ascii_digits(std::string_view s)` |
| `is_french_key_cp` | function | `core/moonshine-tts/src/lang-specific/french.cpp:83` | `bool is_french_key_cp(char32_t c)` |
| `is_french_word_char` | function | `core/moonshine-tts/src/lang-specific/french.cpp:149` | `bool is_french_word_char(char32_t cp)` |
| `is_latin1_supplement_python_word_char` | function | `core/moonshine-tts/src/lang-specific/french.cpp:112` | `bool is_latin1_supplement_python_word_char(char32_t cp)` |
| `is_letterlike_math_word_char` | function | `core/moonshine-tts/src/lang-specific/french.cpp:144` | `bool is_letterlike_math_word_char(char32_t cp)` |
| `join_space` | function | `core/moonshine-tts/src/lang-specific/french.cpp:471` | `std::string join_space(const std::vector<std::string>& v)` |
| `liaison_strength_fn` | function | `core/moonshine-tts/src/lang-specific/french.cpp:923` | `LiaisonStrength liaison_strength_fn(const std::optional<std::string>& pos_left,                  ...` |
| `load_french_lexicon_file` | function | `core/moonshine-tts/src/lang-specific/french.cpp:230` | `void load_french_lexicon_file(     const std::filesystem::path& path,     std::unordered_map<std:...` |
| `load_french_lexicon_stream` | function | `core/moonshine-tts/src/lang-specific/french.cpp:198` | `void load_french_lexicon_stream(     std::istream& in, std::unordered_map<std::string, std::strin...` |
| `load_french_pos_csv_stream` | function | `core/moonshine-tts/src/lang-specific/french.cpp:270` | `void load_french_pos_csv_stream(     std::istream& in, const std::string& cat_upper,     std::uno...` |
| `load_french_pos_dir` | function | `core/moonshine-tts/src/lang-specific/french.cpp:294` | `void load_french_pos_dir(     const std::filesystem::path& dir,     std::unordered_map<std::strin...` |
| `load_french_pos_from_csv_utf8_map` | function | `core/moonshine-tts/src/lang-specific/french.cpp:324` | `void load_french_pos_from_csv_utf8_map(     const std::unordered_map<std::string, std::string>& c...` |
| `lookup_lexicon` | function | `core/moonshine-tts/src/lang-specific/french.cpp:1016` | `std::optional<std::string> lookup_lexicon(     const std::unordered_map<std::string, std::string>...` |
| `nasal_liaison_transform` | function | `core/moonshine-tts/src/lang-specific/french.cpp:682` | `std::optional<std::string> nasal_liaison_transform(const std::string& word,                      ...` |
| `normalize_lookup_key_utf8` | function | `core/moonshine-tts/src/lang-specific/french.cpp:94` | `std::string normalize_lookup_key_utf8(const std::string& word)` |
| `ortho_for_liaison` | function | `core/moonshine-tts/src/lang-specific/french.cpp:703` | `std::string ortho_for_liaison(std::string_view word)` |
| `orthographic_liaison_consonant` | function | `core/moonshine-tts/src/lang-specific/french.cpp:739` | `std::optional<std::string> orthographic_liaison_consonant(     std::string_view word)` |
| `parse_first_csv_field` | function | `core/moonshine-tts/src/lang-specific/french.cpp:241` | `std::string parse_first_csv_field(std::string_view line)` |
| `pos_scan_order` | function | `core/moonshine-tts/src/lang-specific/french.cpp:559` | `const std::vector<std::string>& pos_scan_order()` |
| `re` | function | `core/moonshine-tts/src/lang-specific/french.cpp:519` | `static const std::regex re(R"(\b\d+\b)", std::regex::ECMAScript);` |
| `replace_suffix_once` | function | `core/moonshine-tts/src/lang-specific/french.cpp:672` | `std::string replace_suffix_once(std::string ipa, std::string_view old_s,                         ...` |
| `sort` | function | `core/moonshine-tts/src/lang-specific/french.cpp:333` | `std::sort(sorted.begin(), sorted.end(),             [](const auto& a, const auto& b)` |
| `strip_stress` | function | `core/moonshine-tts/src/lang-specific/french.cpp:623` | `std::string strip_stress(std::string_view ipa)` |
| `text_to_ipa` | function | `core/moonshine-tts/src/lang-specific/french.cpp:1175` | `std::string FrenchRuleG2p::text_to_ipa(std::string text,                                        s...` |
| `text_to_ipa_impl` | function | `core/moonshine-tts/src/lang-specific/french.cpp:1180` | `std::string FrenchRuleG2p::text_to_ipa_impl(     const std::string& text, bool expand_digits,    ...` |
| `to_lower_ascii` | function | `core/moonshine-tts/src/lang-specific/french.cpp:177` | `std::string to_lower_ascii(std::string_view w)` |
| `to_lower_pos_inventory_utf8` | function | `core/moonshine-tts/src/lang-specific/french.cpp:185` | `std::string to_lower_pos_inventory_utf8(const std::string& word)` |
| `utf8_last_cp` | function | `core/moonshine-tts/src/lang-specific/french.cpp:723` | `bool utf8_last_cp(const std::string& s, char32_t& out_cp)` |
| `w` | function | `core/moonshine-tts/src/lang-specific/french.cpp:705` | `const std::string w(word);` |
| `word_to_ipa` | function | `core/moonshine-tts/src/lang-specific/french.cpp:1171` | `std::string FrenchRuleG2p::word_to_ipa(const std::string& word) const` |
| `word_to_ipa_impl` | function | `core/moonshine-tts/src/lang-specific/french.cpp:1127` | `std::string FrenchRuleG2p::word_to_ipa_impl(const std::string& raw_word,                         ...` |
| `FrenchRuleG2p` | class | `core/moonshine-tts/src/lang-specific/french.h:19` | `` |
| `G2pWordLog` | struct | `core/moonshine-tts/src/lang-specific/french.h:15` | `` |
| `MOONSHINE_TTS_LANG_SPECIFIC_FRENCH_H` | macro | `core/moonshine-tts/src/lang-specific/french.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_FRENCH_H` |
| `Options` | struct | `core/moonshine-tts/src/lang-specific/french.h:21` | `` |
| `dialect_id` | function | `core/moonshine-tts/src/lang-specific/french.h:51` | `const std::string& dialect_id() const` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/french.h:49` | `static std::vector<std::string> dialect_ids();` |
| `dialect_resolves_to_french_rules` | function | `core/moonshine-tts/src/lang-specific/french.h:78` | `bool dialect_resolves_to_french_rules(std::string_view dialect_id);` |
| `ensure_french_nuclear_stress` | function | `core/moonshine-tts/src/lang-specific/french.h:60` | `static std::string ensure_french_nuclear_stress(std::string ipa);` |
| `GermanRuleG2p` | function | `core/moonshine-tts/src/lang-specific/german.cpp:1068` | `GermanRuleG2p::GermanRuleG2p(std::filesystem::path dict_tsv, Options options)     : options_(opti...` |
| `GermanRuleG2p` | function | `core/moonshine-tts/src/lang-specific/german.cpp:1073` | `GermanRuleG2p::GermanRuleG2p(std::string dict_tsv_utf8, Options options)     : options_(options)` |
| `Slot` | struct | `core/moonshine-tts/src/lang-specific/german.cpp:756` | `` |
| `append_german_below_1_000_000` | function | `core/moonshine-tts/src/lang-specific/german.cpp:908` | `void append_german_below_1_000_000(int n, std::vector<std::string>& out)` |
| `append_german_tokens_1_999` | function | `core/moonshine-tts/src/lang-specific/german.cpp:880` | `void append_german_tokens_1_999(int n, std::vector<std::string>& out)` |
| `append_german_tokens_thousands` | function | `core/moonshine-tts/src/lang-specific/german.cpp:896` | `void append_german_tokens_thousands(int q, std::vector<std::string>& out)` |
| `ch_ipa_utf8` | function | `core/moonshine-tts/src/lang-specific/german.cpp:144` | `std::string ch_ipa_utf8(const std::u32string& full_word_nh, size_t i)` |
| `char_before_for_ch` | function | `core/moonshine-tts/src/lang-specific/german.cpp:121` | `std::optional<char32_t> char_before_for_ch(const std::u32string& s, size_t i)` |
| `default_stress_syllable_index` | function | `core/moonshine-tts/src/lang-specific/german.cpp:339` | `size_t default_stress_syllable_index(const std::vector<std::u32string>& syls,                    ...` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/german.cpp:1271` | `std::vector<std::string> GermanRuleG2p::dialect_ids()` |
| `dialect_resolves_to_german_rules` | function | `core/moonshine-tts/src/lang-specific/german.cpp:1263` | `bool dialect_resolves_to_german_rules(std::string_view dialect_id)` |
| `dig_pass` | function | `core/moonshine-tts/src/lang-specific/german.cpp:1170` | `static const std::regex dig_pass(R"(^[0-9]+(?:-[0-9]+)*$)", std::regex::ECMAScript);` |
| `dig_re` | function | `core/moonshine-tts/src/lang-specific/german.cpp:965` | `static const std::regex dig_re(R"(\b\d+\b)", std::regex::ECMAScript);` |
| `expand_cardinal_digits_to_german_words` | function | `core/moonshine-tts/src/lang-specific/german.cpp:924` | `std::string expand_cardinal_digits_to_german_words(std::string_view s)` |
| `expand_german_digit_tokens_in_text` | function | `core/moonshine-tts/src/lang-specific/german.cpp:962` | `std::string expand_german_digit_tokens_in_text(std::string text)` |
| `final_devoice` | function | `core/moonshine-tts/src/lang-specific/german.cpp:162` | `std::string final_devoice(std::string ipa)` |
| `finalize_ipa` | function | `core/moonshine-tts/src/lang-specific/german.cpp:1079` | `std::string GermanRuleG2p::finalize_ipa(std::string ipa) const` |
| `g2p_all_ascii_digits` | function | `core/moonshine-tts/src/lang-specific/german.cpp:825` | `bool g2p_all_ascii_digits(std::string_view s)` |
| `german_hundred_head` | function | `core/moonshine-tts/src/lang-specific/german.cpp:868` | `std::string german_hundred_head(int h)` |
| `german_orthographic_syllables_u32` | function | `core/moonshine-tts/src/lang-specific/german.cpp:281` | `std::vector<std::u32string> german_orthographic_syllables_u32(     const std::u32string& word_lower)` |
| `german_tolower_cp` | function | `core/moonshine-tts/src/lang-specific/german.cpp:30` | `char32_t german_tolower_cp(char32_t c)` |
| `german_under_100_word` | function | `core/moonshine-tts/src/lang-specific/german.cpp:837` | `std::string german_under_100_word(int n)` |
| `insert_primary_stress_before_vowel_utf8` | function | `core/moonshine-tts/src/lang-specific/german.cpp:370` | `std::string insert_primary_stress_before_vowel_utf8(std::string s)` |
| `ipa_at_stress_mark` | function | `core/moonshine-tts/src/lang-specific/german.cpp:1012` | `bool ipa_at_stress_mark(const std::string& ipa, size_t j)` |
| `ipa_skip_pre_nucleus` | function | `core/moonshine-tts/src/lang-specific/german.cpp:404` | `size_t ipa_skip_pre_nucleus(std::string_view s, size_t j)` |
| `ipa_starts_with_nucleus` | function | `core/moonshine-tts/src/lang-specific/german.cpp:389` | `bool ipa_starts_with_nucleus(std::string_view rest)` |
| `is_german_word_char` | function | `core/moonshine-tts/src/lang-specific/german.cpp:72` | `bool is_german_word_char(char32_t cp)` |
| `is_key_char` | function | `core/moonshine-tts/src/lang-specific/german.cpp:47` | `bool is_key_char(char32_t c)` |
| `is_vowel_l` | function | `core/moonshine-tts/src/lang-specific/german.cpp:104` | `bool is_vowel_l(char32_t ch)` |
| `letters_to_ipa_no_stress` | function | `core/moonshine-tts/src/lang-specific/german.cpp:438` | `std::string letters_to_ipa_no_stress(const std::u32string& syl_lower,                            ...` |
| `load_german_lexicon_file` | function | `core/moonshine-tts/src/lang-specific/german.cpp:810` | `void load_german_lexicon_file(     const std::filesystem::path& path,     std::unordered_map<std:...` |
| `load_german_lexicon_stream` | function | `core/moonshine-tts/src/lang-specific/german.cpp:754` | `void load_german_lexicon_stream(     std::istream& in, std::unordered_map<std::string, std::strin...` |
| `lookup_or_rules` | function | `core/moonshine-tts/src/lang-specific/german.cpp:1091` | `std::string GermanRuleG2p::lookup_or_rules(const std::string& raw_word) const` |
| `normalize_ipa_stress_for_vocoder` | function | `core/moonshine-tts/src/lang-specific/german.cpp:1021` | `std::string GermanRuleG2p::normalize_ipa_stress_for_vocoder(std::string ipa)` |
| `normalize_lookup_key_utf8` | function | `core/moonshine-tts/src/lang-specific/german.cpp:56` | `std::string normalize_lookup_key_utf8(const std::string& word)` |
| `range_re` | function | `core/moonshine-tts/src/lang-specific/german.cpp:963` | `static const std::regex range_re(R"(\b(\d+)-(\d+)\b)", std::regex::ECMAScript);` |
| `rules_word_to_ipa_utf8` | function | `core/moonshine-tts/src/lang-specific/german.cpp:719` | `std::string rules_word_to_ipa_utf8(const std::string& raw_word,                                  ...` |
| `st_sp_at_morpheme_start` | function | `core/moonshine-tts/src/lang-specific/german.cpp:187` | `bool st_sp_at_morpheme_start(const std::u32string& hyphen_word,                              size...` |
| `strip_hyphens_u32` | function | `core/moonshine-tts/src/lang-specific/german.cpp:225` | `std::u32string strip_hyphens_u32(const std::u32string& w)` |
| `text_to_ipa` | function | `core/moonshine-tts/src/lang-specific/german.cpp:1255` | `std::string GermanRuleG2p::text_to_ipa(std::string text,                                        s...` |
| `text_to_ipa_no_expand` | function | `core/moonshine-tts/src/lang-specific/german.cpp:1179` | `std::string GermanRuleG2p::text_to_ipa_no_expand(     const std::string& text, std::vector<G2pWor...` |
| `unstressed_prefix_len_u32` | function | `core/moonshine-tts/src/lang-specific/german.cpp:211` | `size_t unstressed_prefix_len_u32(const std::u32string& w)` |
| `word_to_ipa` | function | `core/moonshine-tts/src/lang-specific/german.cpp:1157` | `std::string GermanRuleG2p::word_to_ipa(const std::string& word) const` |
| `G2pWordLog` | struct | `core/moonshine-tts/src/lang-specific/german.h:14` | `` |
| `GermanRuleG2p` | class | `core/moonshine-tts/src/lang-specific/german.h:18` | `` |
| `MOONSHINE_TTS_LANG_SPECIFIC_GERMAN_H` | macro | `core/moonshine-tts/src/lang-specific/german.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_GERMAN_H` |
| `Options` | struct | `core/moonshine-tts/src/lang-specific/german.h:20` | `` |
| `dialect_id` | function | `core/moonshine-tts/src/lang-specific/german.h:40` | `const std::string& dialect_id() const` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/german.h:38` | `static std::vector<std::string> dialect_ids();` |
| `dialect_resolves_to_german_rules` | function | `core/moonshine-tts/src/lang-specific/german.h:67` | `bool dialect_resolves_to_german_rules(std::string_view dialect_id);` |
| `normalize_ipa_stress_for_vocoder` | function | `core/moonshine-tts/src/lang-specific/german.h:53` | `static std::string normalize_ipa_stress_for_vocoder(std::string ipa);` |
| `join_cells` | function | `core/moonshine-tts/src/lang-specific/heteronym-context.cpp:12` | `std::string join_cells(const std::vector<std::string>& cells)` |
| `MOONSHINE_TTS_HETERONYM_CONTEXT_H` | macro | `core/moonshine-tts/src/lang-specific/heteronym-context.h:2` | `#define MOONSHINE_TTS_HETERONYM_CONTEXT_H` |
| `all_ascii_digits` | function | `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp:131` | `bool all_ascii_digits(std::string_view s)` |
| `append_join` | function | `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp:43` | `void append_join(std::vector<std::string>& out,                  const std::vector<std::string>& ...` |
| `below_1_000_000_tokens` | function | `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp:93` | `std::vector<std::string> below_1_000_000_tokens(int n)` |
| `digit_re` | function | `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp:171` | `static const std::regex digit_re(R"((\b)(\d+)(\b))");` |
| `expand_cardinal_digits_to_hindi_words` | function | `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp:145` | `std::string expand_cardinal_digits_to_hindi_words(std::string_view s)` |
| `expand_devanagari_digit_runs_in_text` | function | `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp:202` | `std::string expand_devanagari_digit_runs_in_text(std::string text)` |
| `expand_hindi_digit_tokens_in_text` | function | `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp:169` | `std::string expand_hindi_digit_tokens_in_text(std::string text)` |
| `join_space` | function | `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp:120` | `std::string join_space(const std::vector<std::string>& v)` |
| `range_re` | function | `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp:170` | `static const std::regex range_re(R"((\b)(\d+)-(\d+)(\b))");` |
| `tokens_0_999` | function | `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp:68` | `std::vector<std::string> tokens_0_999(int n)` |
| `under_100` | function | `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp:50` | `std::vector<std::string> under_100(int n)` |
| `MOONSHINE_TTS_LANG_SPECIFIC_HINDI_NUMBERS_H` | macro | `core/moonshine-tts/src/lang-specific/hindi-numbers.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_HINDI_NUMBERS_H` |
| `0x094D` | variable | `core/moonshine-tts/src/lang-specific/hindi.cpp:18` | `extern "C" { #include <utf8proc.h> } namespace moonshine_tts { namespace { constexpr char32_t kVirama = 0x094D;` |
| `HindiRuleG2p` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:507` | `HindiRuleG2p::HindiRuleG2p(std::filesystem::path dict_tsv, Options options)     : options_(options)` |
| `HindiRuleG2p` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:521` | `HindiRuleG2p::HindiRuleG2p(std::string dict_tsv_utf8, Options options)     : options_(options)` |
| `Syllable` | struct | `core/moonshine-tts/src/lang-specific/hindi.cpp:45` | `` |
| `all_ascii_digits_sv` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:458` | `bool all_ascii_digits_sv(std::string_view s)` |
| `apply_schwa_syncope` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:201` | `void apply_schwa_syncope(std::vector<Syllable>& syls)` |
| `assign_stress` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:167` | `std::string assign_stress(const std::vector<std::string>& ipa_syllables,                         ...` |
| `builtin_hindi_dict_path` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:472` | `std::filesystem::path builtin_hindi_dict_path()` |
| `cons_ipa` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:101` | `std::string cons_ipa(char32_t base, bool nukta)` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:603` | `std::vector<std::string> HindiRuleG2p::dialect_ids()` |
| `dialect_resolves_to_hindi_rules` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:607` | `bool dialect_resolves_to_hindi_rules(std::string_view dialect_id)` |
| `g2p_single_word` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:531` | `std::string HindiRuleG2p::g2p_single_word(std::string_view word) const` |
| `has_devanagari` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:448` | `bool has_devanagari(std::string_view s)` |
| `hindi_text_to_ipa` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:620` | `std::string hindi_text_to_ipa(const std::string& text, bool with_stress,                         ...` |
| `is_consonant` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:97` | `bool is_consonant(char32_t cp)` |
| `is_devanagari_digit` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:95` | `bool is_devanagari_digit(char32_t cp)` |
| `load_hindi_lexicon_stream` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:479` | `void load_hindi_lexicon_stream(     std::istream& in, std::unordered_map<std::string, std::string...` |
| `nasal_for_place` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:116` | `std::string nasal_for_place(std::string_view first_onset)` |
| `parse_devanagari_to_syllables` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:227` | `std::optional<std::vector<Syllable>> parse_devanagari_to_syllables(     const std::string& word)` |
| `render_syllables` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:358` | `std::string render_syllables(const std::vector<Syllable>& syls,                              bool...` |
| `resolve_hindi_dict_path` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:615` | `std::filesystem::path resolve_hindi_dict_path(     const std::filesystem::path& model_root)` |
| `strip_edges_punct` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:424` | `void strip_edges_punct(std::string_view w, std::string& core)` |
| `sv_starts_with` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:112` | `bool sv_starts_with(std::string_view s, std::string_view p)` |
| `syllable_weight` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:155` | `int syllable_weight(const Syllable& s)` |
| `text_to_ipa` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:594` | `std::string HindiRuleG2p::text_to_ipa(std::string text,                                       std...` |
| `text_to_ipa_no_expand` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:551` | `std::string HindiRuleG2p::text_to_ipa_no_expand(     std::string text, std::vector<G2pWordLog>* p...` |
| `tmp` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:34` | `const std::string tmp(s);` |
| `utf8_nfc_utf8proc` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:33` | `std::string utf8_nfc_utf8proc(std::string_view s)` |
| `word_to_ipa` | function | `core/moonshine-tts/src/lang-specific/hindi.cpp:527` | `std::string HindiRuleG2p::word_to_ipa(const std::string& word) const` |
| `G2pWordLog` | struct | `core/moonshine-tts/src/lang-specific/hindi.h:15` | `` |
| `HindiRuleG2p` | class | `core/moonshine-tts/src/lang-specific/hindi.h:19` | `` |
| `MOONSHINE_TTS_LANG_SPECIFIC_HINDI_H` | macro | `core/moonshine-tts/src/lang-specific/hindi.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_HINDI_H` |
| `Options` | struct | `core/moonshine-tts/src/lang-specific/hindi.h:21` | `` |
| `dialect_id` | function | `core/moonshine-tts/src/lang-specific/hindi.h:34` | `const std::string& dialect_id() const` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/hindi.h:32` | `static std::vector<std::string> dialect_ids();` |
| `dialect_resolves_to_hindi_rules` | function | `core/moonshine-tts/src/lang-specific/hindi.h:52` | `bool dialect_resolves_to_hindi_rules(std::string_view dialect_id);` |
| `MOONSHINE_TTS_IPA_SYMBOLS_H` | macro | `core/moonshine-tts/src/lang-specific/ipa-symbols.h:2` | `#define MOONSHINE_TTS_IPA_SYMBOLS_H` |
| `ItalianRuleG2p` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:1158` | `ItalianRuleG2p::ItalianRuleG2p(std::filesystem::path dict_tsv, Options options)     : options_(op...` |
| `ItalianRuleG2p` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:1163` | `ItalianRuleG2p::ItalianRuleG2p(std::string dict_tsv_utf8, Options options)     : options_(options)` |
| `accented_vowel_in_u32` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:618` | `bool accented_vowel_in_u32(char32_t c)` |
| `append_thousands_multiplier` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:296` | `void append_thousands_multiplier(int q, std::vector<std::string>& out)` |
| `append_tokens_0_999` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:247` | `void append_tokens_0_999(int n, std::vector<std::string>& out)` |
| `below_1_000_000_tokens` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:314` | `void below_1_000_000_tokens(int n, std::vector<std::string>& out)` |
| `default_stressed_syllable_index` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:624` | `size_t default_stressed_syllable_index(const std::vector<std::u32string>& syls,                  ...` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:1339` | `std::vector<std::string> ItalianRuleG2p::dialect_ids()` |
| `dialect_resolves_to_italian_rules` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:1331` | `bool dialect_resolves_to_italian_rules(std::string_view dialect_id)` |
| `dig_pass` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:1244` | `static const std::regex dig_pass(R"(^[0-9]+(?:-[0-9]+)*$)", std::regex::ECMAScript);` |
| `dig_re` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:369` | `static const std::regex dig_re(R"(\b\d+\b)", std::regex::ECMAScript);` |
| `ei_e_accent` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:705` | `bool ei_e_accent(char32_t c)` |
| `expand_cardinal_digits_to_italian_words` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:330` | `std::string expand_cardinal_digits_to_italian_words(std::string_view s)` |
| `expand_digit_tokens_in_text` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:366` | `std::string expand_digit_tokens_in_text(std::string text)` |
| `finalize_ipa` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:1169` | `std::string ItalianRuleG2p::finalize_ipa(std::string ipa,                                        ...` |
| `hundred_head` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:235` | `std::string hundred_head(int h)` |
| `insert_primary_stress_before_vowel` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:666` | `std::string insert_primary_stress_before_vowel(std::string ipa)` |
| `is_all_ascii_digits` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:162` | `bool is_all_ascii_digits(std::string_view s)` |
| `is_italian_lexicon_key_cp` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:70` | `bool is_italian_lexicon_key_cp(char32_t c)` |
| `is_italian_word_char` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:1068` | `bool is_italian_word_char(char32_t cp)` |
| `is_vowel_ch` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:422` | `bool is_vowel_ch(char32_t c)` |
| `italian_cg_palatal_letter` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:712` | `bool italian_cg_palatal_letter(char32_t c)` |
| `italian_orthographic_syllables_u32` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:544` | `std::vector<std::u32string> italian_orthographic_syllables_u32(     std::u32string w)` |
| `italian_tolower_cp` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:35` | `char32_t italian_tolower_cp(char32_t c)` |
| `letters_to_ipa_no_stress` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:718` | `std::string letters_to_ipa_no_stress(const std::u32string& su)` |
| `load_italian_lexicon_file` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:149` | `void load_italian_lexicon_file(     const std::filesystem::path& path,     std::unordered_map<std...` |
| `load_italian_lexicon_stream` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:117` | `void load_italian_lexicon_stream(     std::istream& in, std::unordered_map<std::string, std::stri...` |
| `lookup_or_rules` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:1182` | `std::string ItalianRuleG2p::lookup_or_rules(const std::string& raw_word) const` |
| `next_is_vowel_u32` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:693` | `bool next_is_vowel_u32(const std::u32string& s, size_t j)` |
| `normalize_lookup_key_utf8` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:85` | `std::string normalize_lookup_key_utf8(const std::string& word)` |
| `range_re` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:367` | `static const std::regex range_re(R"(\b(\d+)-(\d+)\b)", std::regex::ECMAScript);` |
| `resolve_italian_dict_path` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:1343` | `std::filesystem::path resolve_italian_dict_path(     const std::filesystem::path& model_root)` |
| `rules_word_to_ipa_utf8` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:980` | `std::string rules_word_to_ipa_utf8(const std::string& raw, bool with_stress)` |
| `should_hiatus_it` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:454` | `bool should_hiatus_it(char32_t a, char32_t b)` |
| `spell_1_999_fused` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:274` | `std::string spell_1_999_fused(int n)` |
| `split_intervocalic_cluster` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:523` | `void split_intervocalic_cluster(const std::string& cluster, std::string& coda,                   ...` |
| `strip_accent_letter` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:429` | `char32_t strip_accent_letter(char32_t c)` |
| `text_to_ipa` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:1323` | `std::string ItalianRuleG2p::text_to_ipa(std::string text,                                        ...` |
| `text_to_ipa_no_expand` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:1253` | `std::string ItalianRuleG2p::text_to_ipa_no_expand(     const std::string& text, std::vector<G2pWo...` |
| `try_consume_italian_word` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:1102` | `bool try_consume_italian_word(const std::string& text, size_t pos,                               ...` |
| `u32_to_utf8` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:414` | `std::string u32_to_utf8(const std::u32string& s)` |
| `under_100` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:178` | `std::string under_100(int n)` |
| `utf8_lowercase_italian` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:104` | `std::string utf8_lowercase_italian(const std::string& word)` |
| `utf8_to_u32` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:401` | `std::u32string utf8_to_u32(const std::string& s)` |
| `valid_onset2` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:509` | `bool valid_onset2(char a, char b)` |
| `vowel_nucleus_spans` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:484` | `void vowel_nucleus_spans(const std::u32string& w,                          std::vector<std::pair<...` |
| `word_to_ipa` | function | `core/moonshine-tts/src/lang-specific/italian.cpp:1231` | `std::string ItalianRuleG2p::word_to_ipa(const std::string& word) const` |
| `G2pWordLog` | struct | `core/moonshine-tts/src/lang-specific/italian.h:14` | `` |
| `ItalianRuleG2p` | class | `core/moonshine-tts/src/lang-specific/italian.h:18` | `` |
| `MOONSHINE_TTS_LANG_SPECIFIC_ITALIAN_H` | macro | `core/moonshine-tts/src/lang-specific/italian.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_ITALIAN_H` |
| `Options` | struct | `core/moonshine-tts/src/lang-specific/italian.h:20` | `` |
| `dialect_id` | function | `core/moonshine-tts/src/lang-specific/italian.h:38` | `const std::string& dialect_id() const` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/italian.h:36` | `static std::vector<std::string> dialect_ids();` |
| `dialect_resolves_to_italian_rules` | function | `core/moonshine-tts/src/lang-specific/italian.h:58` | `bool dialect_resolves_to_italian_rules(std::string_view dialect_id);` |
| `geminate_onset` | function | `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp:152` | `std::string geminate_onset(const std::string& onset,                            const std::string...` |
| `japanese_has_japanese_script` | function | `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp:255` | `bool japanese_has_japanese_script(std::string_view sv)` |
| `japanese_is_kana_only` | function | `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp:226` | `bool japanese_is_kana_only(std::string_view sv)` |
| `katakana_hiragana_to_ipa` | function | `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp:163` | `std::string katakana_hiragana_to_ipa(std::string_view sv)` |
| `katakana_to_hiragana_u32` | function | `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp:31` | `std::u32string katakana_to_hiragana_u32(const std::u32string& in)` |
| `long_mark_extend_last` | function | `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp:67` | `void long_mark_extend_last(std::vector<std::string>& parts)` |
| `tmp` | function | `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp:20` | `const std::string tmp(s);` |
| `u32_to_utf8` | function | `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp:51` | `std::string u32_to_utf8(const std::u32string& u)` |
| `utf8_nfkc_utf8proc` | function | `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp:19` | `std::string utf8_nfkc_utf8proc(std::string_view s)` |
| `utf8_starts_with_at` | function | `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp:59` | `bool utf8_starts_with_at(const std::string& s, std::size_t off,                          const st...` |
| `MOONSHINE_TTS_JAPANESE_KANA_TO_IPA_H` | macro | `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.h:2` | `#define MOONSHINE_TTS_JAPANESE_KANA_TO_IPA_H` |
| `japanese_has_japanese_script` | function | `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.h:14` | `bool japanese_has_japanese_script(std::string_view utf8);` |
| `japanese_is_kana_only` | function | `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.h:13` | `bool japanese_is_kana_only(std::string_view utf8);` |
| `JapaneseOnnxG2p` | function | `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:260` | `JapaneseOnnxG2p::JapaneseOnnxG2p(std::filesystem::path model_dir,                                ...` |
| `JapaneseOnnxG2p` | function | `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:267` | `JapaneseOnnxG2p::JapaneseOnnxG2p(std::filesystem::path model_dir,                                ...` |
| `JapaneseOnnxG2p` | function | `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:275` | `JapaneseOnnxG2p::JapaneseOnnxG2p(const MoonshineG2POptions& opt,                                 ...` |
| `JapaneseOnnxG2p` | function | `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:283` | `JapaneseOnnxG2p::JapaneseOnnxG2p(const MoonshineG2POptions& opt,                                 ...` |
| `build_by_first` | function | `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:228` | `void build_by_first(     const std::unordered_map<std::string, std::string>& lex,     std::unorde...` |
| `default_japanese_dict_path` | function | `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:255` | `std::filesystem::path default_japanese_dict_path(     const std::filesystem::path& g2p_data_root)` |
| `g2p_word` | function | `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:292` | `std::string JapaneseOnnxG2p::g2p_word(std::string word_utf8)` |
| `is_han_cp` | function | `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:34` | `bool is_han_cp(char32_t cp)` |
| `is_single_han` | function | `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:40` | `bool is_single_han(std::string_view s)` |
| `only_han` | function | `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:74` | `bool only_han(std::string_view s)` |
| `only_hiragana` | function | `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:45` | `bool only_hiragana(std::string_view s)` |
| `only_katakana` | function | `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:58` | `bool only_katakana(std::string_view s)` |
| `sort` | function | `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:183` | `std::sort(v.begin(), v.end(),               [](const std::string& a, const std::string& b)` |
| `sort` | function | `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:246` | `std::sort(vec.begin(), vec.end(),               [](const std::string& a, const std::string& b)` |
| `text_to_ipa` | function | `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:357` | `std::string JapaneseOnnxG2p::text_to_ipa(std::string text_utf8)` |
| `tmp` | function | `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:23` | `const std::string tmp(s);` |
| `trailing_particles_sorted` | function | `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:176` | `const std::vector<std::string>& trailing_particles_sorted()` |
| `utf8_nfc_utf8proc` | function | `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:22` | `std::string utf8_nfc_utf8proc(std::string_view s)` |
| `JapaneseOnnxG2p` | class | `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.h:17` | `` |
| `MOONSHINE_TTS_JAPANESE_ONNX_G2P_H` | macro | `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.h:2` | `#define MOONSHINE_TTS_JAPANESE_ONNX_G2P_H` |
| `MoonshineG2POptions` | struct | `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.h:13` | `` |
| `tok` | function | `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.h:34` | `const JapaneseTokPosOnnx& tok() const` |
| `BasicTokCfg` | struct | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:311` | `` |
| `EncodedWp` | struct | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:423` | `` |
| `Idx` | struct | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:513` | `` |
| `JapaneseTokPosOnnx` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:732` | `JapaneseTokPosOnnx::JapaneseTokPosOnnx(const MoonshineG2POptions* opt,                           ...` |
| `align_basic_tokens_u32` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:358` | `void align_basic_tokens_u32(const std::u32string& ref,                             const std::vec...` |
| `basic_tokenize_u32` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:326` | `std::vector<std::u32string> basic_tokenize_u32(     const std::u32string& original_text_u32, cons...` |
| `buf` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:645` | `const std::string buf(utf8);` |
| `bundle_load_binary` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:90` | `bool bundle_load_binary(const MoonshineG2POptions* opt,                         std::string_view ...` |
| `bundle_load_utf8` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:72` | `bool bundle_load_utf8(const MoonshineG2POptions* opt,                       std::string_view bund...` |
| `chars` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:385` | `std::vector<char32_t> chars(wt.begin(), wt.end());` |
| `cjk_tokpos_chunk_exclusive_end` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:684` | `template <typename EncodeFn> std::size_t cjk_tokpos_chunk_exclusive_end(const std::u32string& ful...` |
| `cjk_tokpos_preferred_chunk_break_cp` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:650` | `bool cjk_tokpos_preferred_chunk_break_cp(char32_t c)` |
| `clean_text_u32` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:230` | `std::u32string clean_text_u32(const std::u32string& text)` |
| `default_japanese_tok_pos_model_dir` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:722` | `std::filesystem::path default_japanese_tok_pos_model_dir(     const std::filesystem::path& g2p_da...` |
| `encode_bert_wordpiece` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:430` | `EncodedWp encode_bert_wordpiece(     const std::u32string& text_u32,     const std::unordered_map...` |
| `format_annotated_line` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:793` | `std::string JapaneseTokPosOnnx::format_annotated_line(     const std::vector<std::pair<std::strin...` |
| `is_chinese_char` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:180` | `bool is_chinese_char(std::uint32_t cp)` |
| `is_control_u32` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:153` | `bool is_control_u32(char32_t c)` |
| `is_punct_char_word_group_u32` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:175` | `bool is_punct_char_word_group_u32(char32_t c)` |
| `is_punctuation_u32` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:162` | `bool is_punctuation_u32(char32_t c)` |
| `is_space_u32` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:144` | `bool is_space_u32(char32_t c)` |
| `mask` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:849` | `std::vector<int64_t> mask(static_cast<size_t>(T), 1);` |
| `morph_label_to_upos` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:606` | `std::string morph_label_to_upos(std::string label)` |
| `normalization_ref_u32` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:317` | `std::u32string normalization_ref_u32(const std::u32string& text_u32,                             ...` |
| `open_session` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:31` | `std::unique_ptr<Ort::Session> open_session(     Ort::Env& env, const std::filesystem::path& model...` |
| `open_session_memory` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:48` | `std::unique_ptr<Ort::Session> open_session_memory(     Ort::Env& env, const void* data, size_t le...` |
| `pooled` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:883` | `std::vector<double> pooled(static_cast<size_t>(num_labels), 0.0);` |
| `run_split_on_punc_u32` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:281` | `std::vector<std::u32string> run_split_on_punc_u32(const std::u32string& text)` |
| `slurp_utf8_file` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:62` | `std::string slurp_utf8_file(const std::filesystem::path& p)` |
| `split_u32_whitespace` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:256` | `std::vector<std::u32string> split_u32_whitespace(std::u32string_view s)` |
| `strip_mn_nfd` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:201` | `std::u32string strip_mn_nfd(const std::u32string& s)` |
| `to_lower_u32` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:221` | `std::u32string to_lower_u32(const std::u32string& s)` |
| `tokenize_chinese_chars_u32` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:242` | `std::u32string tokenize_chinese_chars_u32(const std::u32string& text)` |
| `u32_nfc` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:189` | `std::u32string u32_nfc(const std::u32string& s)` |
| `u32_to_utf8` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:136` | `std::string u32_to_utf8(const std::u32string& s)` |
| `ud_upos_set` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:598` | `const std::unordered_set<std::string>& ud_upos_set()` |
| `utf8_to_u32` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:123` | `std::u32string utf8_to_u32(std::string_view utf8)` |
| `wordpiece_tokenize_u32` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:375` | `std::vector<std::u32string> wordpiece_tokenize_u32(     const std::u32string& token,     const st...` |
| `JapaneseTokPosOnnx` | class | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.h:23` | `` |
| `MOONSHINE_TTS_JAPANESE_TOK_POS_ONNX_H` | macro | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.h:2` | `#define MOONSHINE_TTS_JAPANESE_TOK_POS_ONNX_H` |
| `MoonshineG2POptions` | struct | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.h:16` | `` |
| `format_annotated_line` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.h:39` | `static std::string format_annotated_line( const std::vector<std::pair<std::string, std::string>>& pairs);` |
| `model_dir` | function | `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.h:42` | `const std::filesystem::path& model_dir() const` |
| `JapaneseRuleG2p` | function | `core/moonshine-tts/src/lang-specific/japanese.cpp:32` | `JapaneseRuleG2p::JapaneseRuleG2p(std::filesystem::path onnx_model_dir,                           ...` |
| `JapaneseRuleG2p` | function | `core/moonshine-tts/src/lang-specific/japanese.cpp:37` | `JapaneseRuleG2p::JapaneseRuleG2p(std::filesystem::path onnx_model_dir,                           ...` |
| `JapaneseRuleG2p` | function | `core/moonshine-tts/src/lang-specific/japanese.cpp:42` | `JapaneseRuleG2p::JapaneseRuleG2p(const MoonshineG2POptions& opt,                                 ...` |
| `JapaneseRuleG2p` | function | `core/moonshine-tts/src/lang-specific/japanese.cpp:48` | `JapaneseRuleG2p::JapaneseRuleG2p(const MoonshineG2POptions& opt,                                 ...` |
| `absolute_model_root` | function | `core/moonshine-tts/src/lang-specific/japanese.cpp:16` | `std::filesystem::path absolute_model_root(     const std::filesystem::path& model_root)` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/japanese.cpp:67` | `std::vector<std::string> JapaneseRuleG2p::dialect_ids()` |
| `dialect_resolves_to_japanese_rules` | function | `core/moonshine-tts/src/lang-specific/japanese.cpp:72` | `bool dialect_resolves_to_japanese_rules(std::string_view dialect_id)` |
| `resolve_japanese_dict_path` | function | `core/moonshine-tts/src/lang-specific/japanese.cpp:80` | `std::filesystem::path resolve_japanese_dict_path(     const std::filesystem::path& model_root)` |
| `resolve_japanese_onnx_model_dir` | function | `core/moonshine-tts/src/lang-specific/japanese.cpp:86` | `std::filesystem::path resolve_japanese_onnx_model_dir(     const std::filesystem::path& model_root)` |
| `text_to_ipa` | function | `core/moonshine-tts/src/lang-specific/japanese.cpp:61` | `std::string JapaneseRuleG2p::text_to_ipa(     std::string text, std::vector<G2pWordLog>* per_word...` |
| `G2pWordLog` | struct | `core/moonshine-tts/src/lang-specific/japanese.h:14` | `` |
| `JapaneseRuleG2p` | class | `core/moonshine-tts/src/lang-specific/japanese.h:21` | `` |
| `MOONSHINE_TTS_LANG_SPECIFIC_JAPANESE_H` | macro | `core/moonshine-tts/src/lang-specific/japanese.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_JAPANESE_H` |
| `MoonshineG2POptions` | struct | `core/moonshine-tts/src/lang-specific/japanese.h:15` | `` |
| `dialect_id` | function | `core/moonshine-tts/src/lang-specific/japanese.h:43` | `const std::string& dialect_id() const` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/japanese.h:41` | `static std::vector<std::string> dialect_ids();` |
| `dialect_resolves_to_japanese_rules` | function | `core/moonshine-tts/src/lang-specific/japanese.h:54` | `bool dialect_resolves_to_japanese_rules(std::string_view dialect_id);` |
| `gs` | function | `core/moonshine-tts/src/lang-specific/korean-numbers.cpp:160` | `std::vector<unsigned> gs(low_first.rbegin(), low_first.rend());` |
| `hangul_digits_only` | function | `core/moonshine-tts/src/lang-specific/korean-numbers.cpp:66` | `std::string hangul_digits_only(std::string_view s)` |
| `int_to_sino_korean_hangul` | function | `core/moonshine-tts/src/lang-specific/korean-numbers.cpp:147` | `std::string int_to_sino_korean_hangul(std::uint64_t n)` |
| `is_ascii_digit` | function | `core/moonshine-tts/src/lang-specific/korean-numbers.cpp:21` | `bool is_ascii_digit(char c)` |
| `is_ascii_numeral_token` | function | `core/moonshine-tts/src/lang-specific/korean-numbers.cpp:287` | `bool is_ascii_numeral_token(std::string_view token)` |
| `korean_reading_fragments_from_ascii_numeral_token` | function | `core/moonshine-tts/src/lang-specific/korean-numbers.cpp:189` | `std::optional<std::vector<std::string>> korean_reading_fragments_from_ascii_numeral_token(std::st...` |
| `normalize_numeral_token_string` | function | `core/moonshine-tts/src/lang-specific/korean-numbers.cpp:52` | `std::string normalize_numeral_token_string(std::string_view raw)` |
| `parse_uint_strict` | function | `core/moonshine-tts/src/lang-specific/korean-numbers.cpp:124` | `bool parse_uint_strict(std::string_view sv, std::uint64_t& out)` |
| `section_under_10000` | function | `core/moonshine-tts/src/lang-specific/korean-numbers.cpp:76` | `std::string section_under_10000(unsigned n)` |
| `strip_thousands_commas` | function | `core/moonshine-tts/src/lang-specific/korean-numbers.cpp:39` | `std::string strip_thousands_commas(std::string_view raw)` |
| `thousands_lookahead_ok` | function | `core/moonshine-tts/src/lang-specific/korean-numbers.cpp:23` | `bool thousands_lookahead_ok(std::string_view suf)` |
| `MOONSHINE_TTS_LANG_SPECIFIC_KOREAN_NUMBERS_H` | macro | `core/moonshine-tts/src/lang-specific/korean-numbers.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_KOREAN_NUMBERS_H` |
| `is_ascii_numeral_token` | function | `core/moonshine-tts/src/lang-specific/korean-numbers.h:22` | `bool is_ascii_numeral_token(std::string_view token);` |
| `BasicTokCfg` | struct | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:311` | `` |
| `EncodedWp` | struct | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:423` | `` |
| `Idx` | struct | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:513` | `` |
| `KoreanTokPosOnnx` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:732` | `KoreanTokPosOnnx::KoreanTokPosOnnx(const MoonshineG2POptions* opt,                               ...` |
| `align_basic_tokens_u32` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:358` | `void align_basic_tokens_u32(const std::u32string& ref,                             const std::vec...` |
| `basic_tokenize_u32` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:326` | `std::vector<std::u32string> basic_tokenize_u32(     const std::u32string& original_text_u32, cons...` |
| `buf` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:645` | `const std::string buf(utf8);` |
| `bundle_load_binary` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:90` | `bool bundle_load_binary(const MoonshineG2POptions* opt,                         std::string_view ...` |
| `bundle_load_utf8` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:72` | `bool bundle_load_utf8(const MoonshineG2POptions* opt,                       std::string_view bund...` |
| `chars` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:385` | `std::vector<char32_t> chars(wt.begin(), wt.end());` |
| `cjk_tokpos_chunk_exclusive_end` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:684` | `template <typename EncodeFn> std::size_t cjk_tokpos_chunk_exclusive_end(const std::u32string& ful...` |
| `cjk_tokpos_preferred_chunk_break_cp` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:650` | `bool cjk_tokpos_preferred_chunk_break_cp(char32_t c)` |
| `clean_text_u32` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:230` | `std::u32string clean_text_u32(const std::u32string& text)` |
| `default_korean_tok_pos_model_dir` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:722` | `std::filesystem::path default_korean_tok_pos_model_dir(     const std::filesystem::path& g2p_data...` |
| `encode_bert_wordpiece` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:430` | `EncodedWp encode_bert_wordpiece(     const std::u32string& text_u32,     const std::unordered_map...` |
| `format_annotated_line` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:792` | `std::string KoreanTokPosOnnx::format_annotated_line(     const std::vector<std::pair<std::string,...` |
| `is_chinese_char` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:180` | `bool is_chinese_char(std::uint32_t cp)` |
| `is_control_u32` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:153` | `bool is_control_u32(char32_t c)` |
| `is_punct_char_word_group_u32` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:175` | `bool is_punct_char_word_group_u32(char32_t c)` |
| `is_punctuation_u32` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:162` | `bool is_punctuation_u32(char32_t c)` |
| `is_space_u32` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:144` | `bool is_space_u32(char32_t c)` |
| `mask` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:848` | `std::vector<int64_t> mask(static_cast<size_t>(T), 1);` |
| `morph_label_to_upos` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:606` | `std::string morph_label_to_upos(std::string label)` |
| `normalization_ref_u32` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:317` | `std::u32string normalization_ref_u32(const std::u32string& text_u32,                             ...` |
| `open_session` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:31` | `std::unique_ptr<Ort::Session> open_session(     Ort::Env& env, const std::filesystem::path& model...` |
| `open_session_memory` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:48` | `std::unique_ptr<Ort::Session> open_session_memory(     Ort::Env& env, const void* data, size_t le...` |
| `pooled` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:882` | `std::vector<double> pooled(static_cast<size_t>(num_labels), 0.0);` |
| `run_split_on_punc_u32` | function | `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:281` | `std::vector<std::u32string> run_split_on_punc_u32(const std::u32string& text)` |

Next: [SYMBOLS_p5.md](SYMBOLS_p5.md)
