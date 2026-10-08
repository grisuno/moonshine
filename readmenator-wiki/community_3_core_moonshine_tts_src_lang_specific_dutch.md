# core/moonshine-tts/src/lang-specific: dutch

*Community 3 | 51 files | cohesion 0.69*

## Definition

This community groups 51 file(s) rooted at `core/moonshine-tts/src/lang-specific` with dominant language cpp (cohesion 0.69). Central symbols: `ArabicRuleG2p`, `ChineseOnnxG2p`, `ChineseOnnxRuleG2p`, `ChineseRuleG2p`, `CodaS`, `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`, `DutchRuleG2p`, `EnglishOnnxAuxMemory`. Core file: `core/moonshine-tts/src/lang-specific/dutch.cpp` (54 symbols). Documented purpose: Shared helpers for rule-G2P / ONNX parity tests (pre-generated reference lines under ``tests/data/``)..

## Files

### `core/moonshine-tts/src/lang-specific` (19 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `core/moonshine-tts/src/lang-specific/arabic.h` | h | testing | 7 | no |
| `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h` | h | testing | 6 | no |
| `core/moonshine-tts/src/lang-specific/chinese.h` | h | testing | 6 | no |
| `core/moonshine-tts/src/lang-specific/dutch.cpp` | cpp | testing | 54 | no |
| `core/moonshine-tts/src/lang-specific/dutch.h` | h | testing | 8 | no |

### `core/moonshine-tts/tests` (16 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `core/moonshine-tts/tests/arabic-rule-g2p-test.cpp` | cpp | business_logic | 2 | no |
| `core/moonshine-tts/tests/chinese-rule-g2p-test.cpp` | cpp | business_logic | 4 | no |
| `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp` | cpp | business_logic | 9 | no |
| `core/moonshine-tts/tests/english-rule-g2p-test.cpp` | cpp | business_logic | 5 | no |
| `core/moonshine-tts/tests/french-rule-g2p-test.cpp` | cpp | business_logic | 11 | no |

### `core/moonshine-tts/tools` (11 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `core/moonshine-tts/tools/arabic-rule-g2p-cli.cpp` | cpp | business_logic | 3 | yes |
| `core/moonshine-tts/tools/chinese-rule-g2p-cli.cpp` | cpp | business_logic | 3 | yes |
| `core/moonshine-tts/tools/dutch-g2p-batch-cli.cpp` | cpp | utility | 4 | yes |
| `core/moonshine-tts/tools/dutch-rule-g2p-cli.cpp` | cpp | business_logic | 3 | yes |
| `core/moonshine-tts/tools/french-g2p-batch-cli.cpp` | cpp | utility | 4 | yes |

### `core/moonshine-tts/src` (5 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `core/moonshine-tts/src/moonshine-g2p.cpp` | cpp | utility | 7 | no |
| `core/moonshine-tts/src/moonshine-g2p.h` | h | utility | 21 | no |
| `core/moonshine-tts/src/rule-based-g2p-factory.cpp` | cpp | business_logic | 26 | no |
| `core/moonshine-tts/src/rule-based-g2p-factory.h` | h | business_logic | 4 | no |
| `core/moonshine-tts/src/rule-based-g2p.h` | h | business_logic | 3 | no |

*... and 31 more files in this community.*


## Key Symbols

- `MOONSHINE_TTS_LANG_SPECIFIC_ARABIC_H` (macro, `core/moonshine-tts/src/lang-specific/arabic.h:2`) `#define MOONSHINE_TTS_LANG_SPECIFIC_ARABIC_H`
- `G2pWordLog` (struct, `core/moonshine-tts/src/lang-specific/arabic.h:16`)
- `MoonshineG2POptions` (struct, `core/moonshine-tts/src/lang-specific/arabic.h:17`)
- `ArabicRuleG2p` (class, `core/moonshine-tts/src/lang-specific/arabic.h:21`) - MSA Arabic G2P: ONNX partial tashkīl + lexicon + IPA rules (mirrors :mod:`arabic_rule_g2p`).
- `dialect_ids` (function, `core/moonshine-tts/src/lang-specific/arabic.h:39`) `static std::vector<std::string> dialect_ids();`
- `dialect_id` (function, `core/moonshine-tts/src/lang-specific/arabic.h:45`) `const std::string& dialect_id() const`
- `dialect_resolves_to_arabic_rules` (function, `core/moonshine-tts/src/lang-specific/arabic.h:54`) `bool dialect_resolves_to_arabic_rules(std::string_view dialect_id);`
- `MOONSHINE_TTS_CHINESE_ONNX_G2P_H` (macro, `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h:2`) `#define MOONSHINE_TTS_CHINESE_ONNX_G2P_H`
- `G2pWordLog` (struct, `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h:15`)
- `MoonshineG2POptions` (struct, `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h:16`)
- `ChineseOnnxG2p` (class, `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h:20`) - ONNX BIO segmentation + UPOS + ``data/zh_hans/dict.tsv`` (mirrors ``chinese_rule_g2p.ChineseOnnxLexi
- `tok` (function, `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h:37`) `const ChineseTokPosOnnx& tok() const`
- `ChineseOnnxRuleG2p` (class, `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h:46`) - ``MoonshineG2P`` adapter: same dialect ids as ``ChineseRuleG2p`` but requires the RoBERTa UPOS ONNX
- `MOONSHINE_TTS_LANG_SPECIFIC_CHINESE_H` (macro, `core/moonshine-tts/src/lang-specific/chinese.h:2`) `#define MOONSHINE_TTS_LANG_SPECIFIC_CHINESE_H`
- `G2pWordLog` (struct, `core/moonshine-tts/src/lang-specific/chinese.h:14`)
- `ChineseRuleG2p` (class, `core/moonshine-tts/src/lang-specific/chinese.h:23`) - Simplified Chinese lexicon G2P (``data/zh_hans/dict.tsv`` ipa-dict IPA), mirroring ``chinese_rule_g2
- `dialect_ids` (function, `core/moonshine-tts/src/lang-specific/chinese.h:28`) `static std::vector<std::string> dialect_ids();`
- `dialect_id` (function, `core/moonshine-tts/src/lang-specific/chinese.h:30`) `const std::string& dialect_id() const`
- `dialect_resolves_to_chinese_rules` (function, `core/moonshine-tts/src/lang-specific/chinese.h:57`) `bool dialect_resolves_to_chinese_rules(std::string_view dialect_id);`
- `dutch_unicode_tolower_cp` (function, `core/moonshine-tts/src/lang-specific/dutch.cpp:31`) `char32_t dutch_unicode_tolower_cp(char32_t c)`
- `append_lexicon_folded` (function, `core/moonshine-tts/src/lang-specific/dutch.cpp:102`) `void append_lexicon_folded(std::string& out, char32_t cl)` - Fold to ``a-z`` + hyphen for TSV keys (mirrors Python ``normalize_lexicon_key`` intent).
- `normalize_lexicon_key_utf8` (function, `core/moonshine-tts/src/lang-specific/dutch.cpp:160`) `std::string normalize_lexicon_key_utf8(const std::string& word)`
- `is_grapheme_char` (function, `core/moonshine-tts/src/lang-specific/dutch.cpp:178`) `bool is_grapheme_char(char32_t cl)`
- `normalize_grapheme_key_u32` (function, `core/moonshine-tts/src/lang-specific/dutch.cpp:190`) `std::u32string normalize_grapheme_key_u32(const std::string& word)`
- `kTeenWord` (function, `core/moonshine-tts/src/lang-specific/dutch.cpp:212`) `static const char* kTeenWord(int n)`
- `join_unit_tens` (function, `core/moonshine-tts/src/lang-specific/dutch.cpp:221`) `std::string join_unit_tens(int u, std::string_view tens_word)`
- `below_100` (function, `core/moonshine-tts/src/lang-specific/dutch.cpp:237`) `std::string below_100(int n)`
- `below_1000_spaced` (function, `core/moonshine-tts/src/lang-specific/dutch.cpp:256`) `std::string below_1000_spaced(int n)`
- `from_1000_to_9999` (function, `core/moonshine-tts/src/lang-specific/dutch.cpp:278`) `std::string from_1000_to_9999(int n)`
- `fix_thousands_compound` (function, `core/moonshine-tts/src/lang-specific/dutch.cpp:310`) `std::string fix_thousands_compound(int q)`

## Internal vs External Edges

- Internal resolved imports (EXTRACTED): 106
- Cross-boundary resolved imports (EXTRACTED): 47

## Connections

- [EXTRACTED] depends_on community 0 <-> 3 (strength 0.9): Extracted import edge crosses communities: core/moonshine-c-api.cpp imports core/moonshine-tts/src/moonshine-g2p.h.
- [EXTRACTED] depends_on community 2 <-> 3 (strength 0.9): Extracted import edge crosses communities: core/moonshine-tts/src/lang-specific/arabic.cpp imports core/moonshine-tts/src/lang-specific/arabic.h.
- [EXTRACTED] depends_on community 3 <-> 4 (strength 0.9): Extracted import edge crosses communities: core/moonshine-tts/src/lang-specific/arabic.h imports core/moonshine-tts/src/lang-specific/arabic-diac-onnx.h.
- [EXTRACTED] depends_on community 7 <-> 3 (strength 0.9): Extracted import edge crosses communities: core/moonshine-tts/src/lang-specific/english.cpp imports core/moonshine-tts/src/lang-specific/english.h.

## Risks

- No scoped security, taint, cycle, or layer risks.

## Open Questions

- Why do 39 file(s) lack file-level docs (e.g. `core/moonshine-tts/src/lang-specific/arabic.h`)? What purpose do they serve?
- What would break if the most connected file in core/moonshine-tts/src/lang-specific: dutch changed?
- Should core/moonshine-tts/src/lang-specific: dutch be split, given cohesion 0.69?

## Sources

- `core/moonshine-tts/src/lang-specific/arabic.h`
- `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h`
- `core/moonshine-tts/src/lang-specific/chinese.h`
- `core/moonshine-tts/src/lang-specific/dutch.cpp`
- `core/moonshine-tts/src/lang-specific/dutch.h`
- `core/moonshine-tts/src/lang-specific/english.h`
- `core/moonshine-tts/src/lang-specific/french.h`
- `core/moonshine-tts/src/lang-specific/german.h`
- `core/moonshine-tts/src/lang-specific/hindi.h`
- `core/moonshine-tts/src/lang-specific/italian.cpp`
- `core/moonshine-tts/src/lang-specific/italian.h`
- `core/moonshine-tts/src/lang-specific/japanese.h`
- `core/moonshine-tts/src/lang-specific/korean.h`
- `core/moonshine-tts/src/lang-specific/portuguese.h`
- `core/moonshine-tts/src/lang-specific/russian.h`
- `core/moonshine-tts/src/lang-specific/spanish.h`
- `core/moonshine-tts/src/lang-specific/turkish.h`
- `core/moonshine-tts/src/lang-specific/ukrainian.h`
- `core/moonshine-tts/src/lang-specific/vietnamese.h`
- `core/moonshine-tts/src/moonshine-g2p.cpp`
- *... and 31 more*
