# core/moonshine-tts/src/lang-specific: english-hand-oov

*Community 7 | 18 files | cohesion 0.78*

## Definition

This community groups 18 file(s) rooted at `core/moonshine-tts/src/lang-specific` with dominant language cpp (cohesion 0.78). Central symbols: `CmudictTsv`, `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`, `EnglishRuleG2p`, `Literal`, `MOONSHINE_TTS_CMUDICT_TSV_H`, `MOONSHINE_TTS_CONSTANTS_H`, `MOONSHINE_TTS_JSON_CONFIG_H`, `MOONSHINE_TTS_LANG_SPECIFIC_ENGLISH_HAND_OOV_H`. Core file: `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp` (14 symbols).

## Files

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `core/moonshine-tts/src/constants.h` | h | utility | 1 | no |
| `core/moonshine-tts/src/json-config.cpp` | cpp | infrastructure | 5 | no |
| `core/moonshine-tts/src/json-config.h` | h | infrastructure | 2 | no |
| `core/moonshine-tts/src/lang-specific/cmudict-tsv.cpp` | cpp | testing | 6 | no |
| `core/moonshine-tts/src/lang-specific/cmudict-tsv.h` | h | testing | 3 | no |
| `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp` | cpp | testing | 14 | no |
| `core/moonshine-tts/src/lang-specific/english-hand-oov.h` | h | testing | 1 | no |
| `core/moonshine-tts/src/lang-specific/english-numbers.cpp` | cpp | testing | 7 | no |
| `core/moonshine-tts/src/lang-specific/english-numbers.h` | h | testing | 1 | no |
| `core/moonshine-tts/src/lang-specific/english.cpp` | cpp | testing | 8 | no |
| `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp` | cpp | business_logic | 10 | no |
| `core/moonshine-tts/src/lang-specific/onnx-g2p-models.h` | h | business_logic | 2 | no |
| `core/moonshine-tts/src/text-normalize.cpp` | cpp | utility | 4 | no |
| `core/moonshine-tts/src/text-normalize.h` | h | utility | 1 | no |
| `core/moonshine-tts/tests/cmudict-tsv-test.cpp` | cpp | testing | 2 | no |
| `core/moonshine-tts/tests/english-hand-oov-test.cpp` | cpp | testing | 3 | no |
| `core/moonshine-tts/tests/json-config-test.cpp` | cpp | infrastructure | 2 | no |
| `core/moonshine-tts/tests/text-normalize-test.cpp` | cpp | testing | 4 | no |

## Key Symbols

- `MOONSHINE_TTS_CONSTANTS_H` (macro, `core/moonshine-tts/src/constants.h:2`) `#define MOONSHINE_TTS_CONSTANTS_H`
- `read_json_file` (function, `core/moonshine-tts/src/json-config.cpp:14`) `nlohmann::json read_json_file(const std::filesystem::path& p)`
- `validate_header` (function, `core/moonshine-tts/src/json-config.cpp:24`) `void validate_header(const nlohmann::json& cfg, const std::string& expect_kind,`
- `stoi_to_itos` (function, `core/moonshine-tts/src/json-config.cpp:47`) `std::vector<std::string> stoi_to_itos(     const std::unordered_map<std::string,`
- `load_oov_tables_from_json` (function, `core/moonshine-tts/src/json-config.cpp:64`) `OovOnnxTables load_oov_tables_from_json(const nlohmann::json& cfg,`
- `load_oov_tables` (function, `core/moonshine-tts/src/json-config.cpp:88`) `OovOnnxTables load_oov_tables(const std::filesystem::path& model_onnx_path)`
- `MOONSHINE_TTS_JSON_CONFIG_H` (macro, `core/moonshine-tts/src/json-config.h:2`) `#define MOONSHINE_TTS_JSON_CONFIG_H`
- `OovOnnxTables` (struct, `core/moonshine-tts/src/json-config.h:15`)
- `parse_cmudict_tsv_lines` (function, `core/moonshine-tts/src/lang-specific/cmudict-tsv.cpp:14`) `void parse_cmudict_tsv_lines(     std::istream& in,     std::unordered_map<std::`
- `CmudictTsv` (function, `core/moonshine-tts/src/lang-specific/cmudict-tsv.cpp:58`) `CmudictTsv::CmudictTsv(const std::filesystem::path& path)`
- `CmudictTsv` (function, `core/moonshine-tts/src/lang-specific/cmudict-tsv.cpp:66`) `CmudictTsv::CmudictTsv(std::string_view utf8_contents)`
- `buf` (function, `core/moonshine-tts/src/lang-specific/cmudict-tsv.cpp:67`) `const std::string buf(utf8_contents);`
- `lookup` (function, `core/moonshine-tts/src/lang-specific/cmudict-tsv.cpp:72`) `const std::vector<std::string>* CmudictTsv::lookup(std::string_view key) const`
- `k` (function, `core/moonshine-tts/src/lang-specific/cmudict-tsv.cpp:73`) `const std::string k(key.begin(), key.end());`
- `MOONSHINE_TTS_CMUDICT_TSV_H` (macro, `core/moonshine-tts/src/lang-specific/cmudict-tsv.h:2`) `#define MOONSHINE_TTS_CMUDICT_TSV_H`
- `CmudictTsv` (class, `core/moonshine-tts/src/lang-specific/cmudict-tsv.h:14`) - word key (normalized grapheme) -> sorted unique IPA strings (TSV: word<TAB>ipa).
- `lookup` (function, `core/moonshine-tts/src/lang-specific/cmudict-tsv.h:19`) `const std::vector<std::string>* lookup(std::string_view key) const;`
- `utf8_starts_with` (function, `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:19`) `bool utf8_starts_with(const std::string& s, std::string_view p)`
- `last_utf8_char` (function, `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:23`) `std::string_view last_utf8_char(std::string_view s)`
- `last_ipa_unit_is_vowel` (function, `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:38`) `bool last_ipa_unit_is_vowel(std::string_view prev)`
- `is_vowel` (function, `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:50`) `constexpr bool is_vowel(char c)`
- `is_consonant` (function, `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:54`) `constexpr bool is_consonant(char c)`
- `next_vowel_index` (function, `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:58`) `int next_vowel_index(std::string_view w, int start)`
- `magic_e_lengthens` (function, `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:67`) `bool magic_e_lengthens(std::string_view w, int vowel_i)`
- `Literal` (struct, `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:124`)
- `th_voiced_word` (function, `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:157`) `bool th_voiced_word(std::string_view w)`
- `oov_single_consonant` (function, `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:163`) `std::string oov_single_consonant(char c, std::string_view w, int i)`
- `add_primary_stress_if_missing` (function, `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:320`) `std::string add_primary_stress_if_missing(std::string s)`
- `p` (function, `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:329`) `const std::string_view p(pref);`
- `oov_grapheme_to_ipa` (function, `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:341`) `std::string oov_grapheme_to_ipa(std::string_view word)`

## Internal vs External Edges

- Internal resolved imports (EXTRACTED): 21
- Cross-boundary resolved imports (EXTRACTED): 6

## Connections

- [EXTRACTED] depends_on community 7 <-> 3 (strength 0.9): Extracted import edge crosses communities: core/moonshine-tts/src/lang-specific/english.cpp imports core/moonshine-tts/src/lang-specific/english.h.
- [EXTRACTED] depends_on community 7 <-> 2 (strength 0.9): Extracted import edge crosses communities: core/moonshine-tts/src/lang-specific/english.cpp imports core/moonshine-tts/src/g2p-word-log.h.
- [EXTRACTED] depends_on community 7 <-> 4 (strength 0.9): Extracted import edge crosses communities: core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp imports core/moonshine-tts/src/ort-session-options.h.
- [INFERRED] shares_context community 0 <-> 7 (strength 0.5): Inferred shared context (language cpp) with no import path between community 0 (core: moonshine-cpp) and community 7 (core/moonshine-tts/src/lang-specific: english-hand-oov).

## Risks

- No scoped security, taint, cycle, or layer risks.

## Open Questions

- Why do 18 file(s) lack file-level docs (e.g. `core/moonshine-tts/src/constants.h`)? What purpose do they serve?
- What would break if the most connected file in core/moonshine-tts/src/lang-specific: english-hand-oov changed?
- Should core/moonshine-tts/src/lang-specific: english-hand-oov be split, given cohesion 0.78?

## Sources

- `core/moonshine-tts/src/constants.h`
- `core/moonshine-tts/src/json-config.cpp`
- `core/moonshine-tts/src/json-config.h`
- `core/moonshine-tts/src/lang-specific/cmudict-tsv.cpp`
- `core/moonshine-tts/src/lang-specific/cmudict-tsv.h`
- `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp`
- `core/moonshine-tts/src/lang-specific/english-hand-oov.h`
- `core/moonshine-tts/src/lang-specific/english-numbers.cpp`
- `core/moonshine-tts/src/lang-specific/english-numbers.h`
- `core/moonshine-tts/src/lang-specific/english.cpp`
- `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp`
- `core/moonshine-tts/src/lang-specific/onnx-g2p-models.h`
- `core/moonshine-tts/src/text-normalize.cpp`
- `core/moonshine-tts/src/text-normalize.h`
- `core/moonshine-tts/tests/cmudict-tsv-test.cpp`
- `core/moonshine-tts/tests/english-hand-oov-test.cpp`
- `core/moonshine-tts/tests/json-config-test.cpp`
- `core/moonshine-tts/tests/text-normalize-test.cpp`
