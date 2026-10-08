# core/moonshine-tts/src/lang-specific: french

*Community 2 | 51 files | cohesion 0.60*

## Definition

This community groups 51 file(s) rooted at `core/moonshine-tts/src/lang-specific` with dominant language cpp (cohesion 0.60). Central symbols: `0`, `0x094D`, `0xAC00`, `ArabicRuleG2p`, `ChineseOnnxG2p`, `ChineseOnnxRuleG2p`, `ChineseRuleG2p`, `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`. Core file: `core/moonshine-tts/src/lang-specific/french.cpp` (55 symbols). Documented purpose: Russian cardinal expansion (russian_numbers.py). #include from russian.cpp (same TU)..

## Files

### `core/moonshine-tts/src/lang-specific` (39 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp` | cpp | testing | 15 | no |
| `core/moonshine-tts/src/lang-specific/arabic-ipa.h` | h | testing | 1 | no |
| `core/moonshine-tts/src/lang-specific/arabic.cpp` | cpp | testing | 13 | no |
| `core/moonshine-tts/src/lang-specific/chinese-numbers.cpp` | cpp | testing | 9 | no |
| `core/moonshine-tts/src/lang-specific/chinese-numbers.h` | h | testing | 1 | no |
| `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp` | cpp | testing | 12 | no |
| `core/moonshine-tts/src/lang-specific/chinese.cpp` | cpp | testing | 28 | no |
| `core/moonshine-tts/src/lang-specific/french-compound-map.cpp` | cpp | testing | 0 | no |

### `core/moonshine-tts/src` (6 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `core/moonshine-tts/src/g2p-word-log.cpp` | cpp | utility | 2 | no |
| `core/moonshine-tts/src/g2p-word-log.h` | h | utility | 5 | no |
| `core/moonshine-tts/src/ipa-postprocess.cpp` | cpp | utility | 49 | no |
| `core/moonshine-tts/src/ipa-postprocess.h` | h | utility | 4 | no |
| `core/moonshine-tts/src/utf8-utils.cpp` | cpp | utility | 10 | no |
| `core/moonshine-tts/src/utf8-utils.h` | h | utility | 10 | no |

### `core/moonshine-tts/tests` (4 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `core/moonshine-tts/tests/heteronym-context-test.cpp` | cpp | testing | 3 | no |
| `core/moonshine-tts/tests/hindi-rule-g2p-test.cpp` | cpp | business_logic | 6 | no |
| `core/moonshine-tts/tests/ipa-postprocess-test.cpp` | cpp | testing | 27 | no |
| `core/moonshine-tts/tests/utf8-utils-test.cpp` | cpp | testing | 5 | no |

### `core/moonshine-tts/tools` (2 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `core/moonshine-tts/tools/moonshine-g2p-cli.cpp` | cpp | utility | 5 | yes |
| `core/moonshine-tts/tools/piper-ipa-normalize-cli.cpp` | cpp | utility | 3 | yes |

*... and 31 more files in this community.*


## Key Symbols

- `g2p_word_path_tag` (function, `core/moonshine-tts/src/g2p-word-log.cpp:7`) `const char* g2p_word_path_tag(G2pWordPath path)`
- `format_g2p_word_log_line` (function, `core/moonshine-tts/src/g2p-word-log.cpp:35`) `std::string format_g2p_word_log_line(const G2pWordLog& e)`
- `MOONSHINE_TTS_G2P_WORD_LOG_H` (macro, `core/moonshine-tts/src/g2p-word-log.h:2`) `#define MOONSHINE_TTS_G2P_WORD_LOG_H`
- `G2pWordPath` (enum, `core/moonshine-tts/src/g2p-word-log.h:11`) - How a surface word was converted to IPA in ``MoonshineG2P`` / ``EnglishRuleG2p`` pipelines.
- `G2pWordPath` (class, `core/moonshine-tts/src/g2p-word-log.h:11`) - How a surface word was converted to IPA in ``MoonshineG2P`` / ``EnglishRuleG2p`` pipelines.
- `g2p_word_path_tag` (function, `core/moonshine-tts/src/g2p-word-log.h:27`) `const char* g2p_word_path_tag(G2pWordPath path);`
- `G2pWordLog` (struct, `core/moonshine-tts/src/g2p-word-log.h:29`)
- `0` (variable, `core/moonshine-tts/src/ipa-postprocess.cpp:5`) `extern "C" { #include <utf8proc.h> } #include <algorithm> #include <cctype> #inc`
- `replace_utf8_all` (function, `core/moonshine-tts/src/ipa-postprocess.cpp:21`) `void replace_utf8_all(std::string& s, std::string_view old_utf8,`
- `trim_copy` (function, `core/moonshine-tts/src/ipa-postprocess.cpp:30`) `std::string trim_copy(std::string t)`
- `strip_length_markers_copy` (function, `core/moonshine-tts/src/ipa-postprocess.cpp:37`) `std::string strip_length_markers_copy(std::string t)`
- `apply_shared_g2p_to_piper_replacements` (function, `core/moonshine-tts/src/ipa-postprocess.cpp:46`) `void apply_shared_g2p_to_piper_replacements(std::string& s)`
- `apply_korean_post_normalize_ipa` (function, `core/moonshine-tts/src/ipa-postprocess.cpp:54`) `void apply_korean_post_normalize_ipa(std::string& s)`
- `apply_german_ipa_piper_style` (function, `core/moonshine-tts/src/ipa-postprocess.cpp:76`) `void apply_german_ipa_piper_style(std::string& s)` - U+0361 COMBINING DOUBLE INVERTED BREVE between consonants (narrow IPA tie bar) → espeak digraph.
- `kBar` (function, `core/moonshine-tts/src/ipa-postprocess.cpp:77`) `static const std::string kBar("\xcd\xa1");`
- `kTurnedACombBreve` (function, `core/moonshine-tts/src/ipa-postprocess.cpp:92`) `static const std::string kTurnedACombBreve("\xc9\x90\xcc\xaf");` - Non-syllabic turned-a (common for post-vocalic /ɐ/ in German narrow IPA) → alveolar tap like Piper.
- `kAlveolarTap` (function, `core/moonshine-tts/src/ipa-postprocess.cpp:93`) `static const std::string kAlveolarTap("\xc9\xbe");`
- `kUvuR` (function, `core/moonshine-tts/src/ipa-postprocess.cpp:97`) `static const std::string kUvuR("\xca\x81");` - Uvular fricative/approximant ʁ (U+0281) → ɾ for Piper/de voice inventory overlap.
- `apply_lang_specific_replacements` (function, `core/moonshine-tts/src/ipa-postprocess.cpp:106`) `void apply_lang_specific_replacements(std::string& s,`
- `key` (function, `core/moonshine-tts/src/ipa-postprocess.cpp:141`) `const std::string key(eff);`
- `py_isspace_one_utf8_char` (function, `core/moonshine-tts/src/ipa-postprocess.cpp:151`) `bool py_isspace_one_utf8_char(std::string_view ch)`
- `unicode_category_first_char_is_p_or_s` (function, `core/moonshine-tts/src/ipa-postprocess.cpp:170`) `bool unicode_category_first_char_is_p_or_s(char32_t cp)`
- `category_is_mn_or_me` (function, `core/moonshine-tts/src/ipa-postprocess.cpp:175`) `bool category_is_mn_or_me(char32_t cp)`
- `is_ipa_like_inventory_char` (function, `core/moonshine-tts/src/ipa-postprocess.cpp:181`) `bool is_ipa_like_inventory_char(char32_t cp)`
- `utf8_singleton_codepoint` (function, `core/moonshine-tts/src/ipa-postprocess.cpp:206`) `char32_t utf8_singleton_codepoint(std::string_view token)`
- `utf8_prev_codepoint_start` (function, `core/moonshine-tts/src/ipa-postprocess.cpp:216`) `size_t utf8_prev_codepoint_start(const std::string& s, size_t char_start)`
- `rewrite_russian_combining_acute_to_primary_stress` (function, `core/moonshine-tts/src/ipa-postprocess.cpp:230`) `void rewrite_russian_combining_acute_to_primary_stress(std::string& s)` - Map combining acute (U+0301) after a nucleus onto U+02C8 ˈ (Piper-style modifier stress). If the nuc
- `kAcute` (function, `core/moonshine-tts/src/ipa-postprocess.cpp:231`) `static const std::string kAcute("\xcc\x81");`
- `kPri` (function, `core/moonshine-tts/src/ipa-postprocess.cpp:232`) `static const std::string kPri("\xcb\x88");`
- `kSec` (function, `core/moonshine-tts/src/ipa-postprocess.cpp:233`) `static const std::string kSec( "\xcb\x8c");`

## Internal vs External Edges

- Internal resolved imports (EXTRACTED): 78
- Cross-boundary resolved imports (EXTRACTED): 53

## Connections

- [EXTRACTED] depends_on community 4 <-> 2 (strength 0.9): Extracted import edge crosses communities: core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp imports core/moonshine-tts/src/utf8-utils.h.
- [EXTRACTED] depends_on community 2 <-> 3 (strength 0.9): Extracted import edge crosses communities: core/moonshine-tts/src/lang-specific/arabic.cpp imports core/moonshine-tts/src/lang-specific/arabic.h.
- [EXTRACTED] depends_on community 7 <-> 2 (strength 0.9): Extracted import edge crosses communities: core/moonshine-tts/src/lang-specific/english.cpp imports core/moonshine-tts/src/g2p-word-log.h.
- [EXTRACTED] depends_on community 2 <-> 0 (strength 0.9): Extracted import edge crosses communities: core/moonshine-tts/src/lang-specific/korean.cpp imports core/moonshine-utils/debug-utils.h.

## Risks

- No scoped security, taint, cycle, or layer risks.

## Open Questions

- Why do 47 file(s) lack file-level docs (e.g. `core/moonshine-tts/src/g2p-word-log.cpp`)? What purpose do they serve?
- What would break if the most connected file in core/moonshine-tts/src/lang-specific: french changed?
- Should core/moonshine-tts/src/lang-specific: french be split, given cohesion 0.60?

## Sources

- `core/moonshine-tts/src/g2p-word-log.cpp`
- `core/moonshine-tts/src/g2p-word-log.h`
- `core/moonshine-tts/src/ipa-postprocess.cpp`
- `core/moonshine-tts/src/ipa-postprocess.h`
- `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp`
- `core/moonshine-tts/src/lang-specific/arabic-ipa.h`
- `core/moonshine-tts/src/lang-specific/arabic.cpp`
- `core/moonshine-tts/src/lang-specific/chinese-numbers.cpp`
- `core/moonshine-tts/src/lang-specific/chinese-numbers.h`
- `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp`
- `core/moonshine-tts/src/lang-specific/chinese.cpp`
- `core/moonshine-tts/src/lang-specific/french-compound-map.cpp`
- `core/moonshine-tts/src/lang-specific/french-compound-map.h`
- `core/moonshine-tts/src/lang-specific/french-internal.h`
- `core/moonshine-tts/src/lang-specific/french-oov.cpp`
- `core/moonshine-tts/src/lang-specific/french.cpp`
- `core/moonshine-tts/src/lang-specific/german.cpp`
- `core/moonshine-tts/src/lang-specific/heteronym-context.cpp`
- `core/moonshine-tts/src/lang-specific/heteronym-context.h`
- `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp`
- *... and 31 more*
