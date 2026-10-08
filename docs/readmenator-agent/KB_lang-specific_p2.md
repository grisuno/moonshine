# Subsystem: lang-specific (page 2 of 4)
Previous: [KB_lang-specific.md](KB_lang-specific.md)

## core/moonshine-tts/src/lang-specific/english.cpp
- Doc: pick_english_heteronym_ipa: CMU-style heteronyms such as ``tomato`` include both US (stressed...
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
- Doc: EnglishRuleG2p: US English lexicon + OOV ONNX + hand OOV fallback (no heteronym ONNX).
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
- Doc: is_latin1_supplement_python_word_char: Python ``re.UNICODE`` word chars in U+00AA..U+00FF...
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
- Doc: FrenchRuleG2p: Lexicon + liaison + OOV rules + cardinal digit expansion (mirrors ``french_g2p.py``).
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
- Doc: normalize_lookup_key_utf8: NFC-style key: lowercase letters + umlauts + ß only (Python...
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
- Doc: GermanRuleG2p: Rule- and lexicon-based German G2P (High German), mirroring ``german_rule_g2p.py``.
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
- Layer: testing
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
- Layer: testing
- Language: h
- Symbols:
  - `MOONSHINE_TTS_LANG_SPECIFIC_HINDI_NUMBERS_H` (macro, line 2) `#define MOONSHINE_TTS_LANG_SPECIFIC_HINDI_NUMBERS_H`
- Imported by: `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp`, `core/moonshine-tts/src/lang-specific/hindi.cpp`, `core/moonshine-tts/tests/hindi-rule-g2p-test.cpp`

## core/moonshine-tts/src/lang-specific/hindi.cpp
- Layer: testing
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
- Doc: HindiRuleG2p: Hindi Devanagari G2P: ``dict.tsv`` lookup + rule-based parsing (mirrors...
- Layer: testing
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
- Doc: italian_cg_palatal_letter: After c/g (and related digraphs): letters that palatalize, matching...
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
- Doc: ItalianRuleG2p: Rule- and lexicon-based Italian G2P, mirroring ``italian_rule_g2p.py`` /...
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


Next: [KB_lang-specific_p3.md](KB_lang-specific_p3.md)
