# Subsystem: lang-specific (page 4 of 4)
Previous: [KB_lang-specific_p3.md](KB_lang-specific_p3.md)

## core/moonshine-tts/src/lang-specific/russian.cpp
- Doc: normalize_lookup_key_utf8: Mirrors Python ``normalize_lookup_key`` (lower + NFD + Mn strip +...
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
- Doc: RussianRuleG2p: Rule- and lexicon-based Russian G2P, mirroring ``russian_rule_g2p.py``.
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
- Doc: Spanish cardinal expansion (spanish_numbers.py). #include from spanish.cpp (same TU).
- Layer: testing
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
- Doc: k_unicode_strip_table: Definitions in spanish_unicode_tables.cpp (generated Unicode data).
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
- Doc: strip_replacement_utf8: UTF-8 replacement from the strip table, or nullptr when absent.
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
- Doc: SpanishRuleG2p: Rule-based Spanish G2P (mirrors ``spanish_rule_g2p.py``).
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
  - `utf8_append_codepoint` (variable, line 6) `extern "C" { #include <utf8proc.h> } #include <cctype> #include <cstdlib> #include <optional> #include <regex>...`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/turkish.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/turkish.h
- Doc: TurkishRuleG2p: Rule-based Turkish G2P (mirrors ``turkish_rule_g2p.py``): nearly phonemic...
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
  - `trim_ascii_ws_copy` (variable, line 6) `extern "C" { #include <utf8proc.h> } #include <cctype> #include <cstdlib> #include <optional> #include <regex>...`
- Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/ukrainian.h`, `core/moonshine-tts/src/utf8-utils.h`

## core/moonshine-tts/src/lang-specific/ukrainian.h
- Doc: UkrainianRuleG2p: Rule-based Ukrainian G2P (mirrors ``ukrainian_rule_g2p.py``): Cyrillic +...
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
- Doc: split_tone: Tone combining marks (NFD) -> id 2..6; default 1 (ngang).
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
- Doc: VietnameseRuleG2p: Vietnamese lexicon + greedy longest-match + OOV syllable rules (Northern IPA...
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

