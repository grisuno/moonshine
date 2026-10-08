# micro/g2p/src

*Community 6 | 25 files | cohesion 0.93*

## Definition

This community groups 25 file(s) rooted at `micro/g2p/src` with dominant language cc (cohesion 0.93). Central symbols: `Add`, `AddPrimaryStressIfMissing`, `AdvanceJoins`, `Alloc`, `AllocArray`, `Antiresonator`, `AppendStop`, `ArenaBytes`. Core file: `micro/neural-tts/src/neural_tts.cc` (71 symbols). Documented purpose: English grapheme-to-phoneme front end.  Pipeline per word: runtime override -> number normalizer -> baked common-word dictionary -> rule-based letter-to-sound. .

## Files

### `micro/g2p/src` (9 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `micro/g2p/src/g2p.cc` | cc | utility | 3 | no |
| `micro/g2p/src/g2p_dict.cc` | cc | utility | 9 | no |
| `micro/g2p/src/g2p_dict_data.h` | h | data_access | 1 | yes |
| `micro/g2p/src/g2p_numbers.cc` | cc | utility | 7 | no |
| `micro/g2p/src/g2p_numbers.h` | h | utility | 2 | yes |

### `micro/klatt-tts/include/tts` (6 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `micro/klatt-tts/include/tts/config.h` | h | infrastructure | 5 | yes |
| `micro/klatt-tts/include/tts/klatt.h` | h | utility | 20 | yes |
| `micro/klatt-tts/include/tts/phonemes.h` | h | utility | 5 | yes |
| `micro/klatt-tts/include/tts/synth_internal.h` | h | utility | 9 | yes |
| `micro/klatt-tts/include/tts/synth_stream.h` | h | utility | 15 | yes |

### `micro/klatt-tts/src` (5 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `micro/klatt-tts/src/config.cc` | cc | infrastructure | 7 | no |
| `micro/klatt-tts/src/klatt.cc` | cc | utility | 11 | no |
| `micro/klatt-tts/src/phonemes.cc` | cc | utility | 2 | no |
| `micro/klatt-tts/src/synth_internal.cc` | cc | utility | 11 | no |
| `micro/klatt-tts/src/synth_stream.cc` | cc | utility | 9 | no |

### `micro/g2p/include/g2p` (3 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `micro/g2p/include/g2p/g2p.h` | h | utility | 1 | yes |
| `micro/g2p/include/g2p/g2p_dict.h` | h | utility | 9 | yes |
| `micro/g2p/include/g2p/g2p_phones.h` | h | utility | 5 | yes |

### `micro/klatt-tts/tests` (1 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `micro/klatt-tts/tests/tts_test.cc` | cc | testing | 4 | yes |

### `micro/neural-tts/src` (1 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `micro/neural-tts/src/neural_tts.cc` | cc | utility | 71 | yes |

*... and 5 more files in this community.*


## Key Symbols

- `G2P_G2P_H_` (macro, `micro/g2p/include/g2p/g2p.h:18`) `#define G2P_G2P_H_`
- `G2P_G2P_DICT_H_` (macro, `micro/g2p/include/g2p/g2p_dict.h:15`) `#define G2P_G2P_DICT_H_`
- `DictLookup` (function, `micro/g2p/include/g2p/g2p_dict.h:26`) `bool DictLookup(std::string_view word, std::string* ipa);` - Look up `word` (case-insensitive; only a-z letters are significant) in the baked flash dictionary. O
- `Lexicon` (class, `micro/g2p/include/g2p/g2p_dict.h:30`) - Runtime, user-supplied pronunciation overrides. Sorted vector + binary search; checked before the ba
- `LoadFromFile` (function, `micro/g2p/include/g2p/g2p_dict.h:35`) `bool LoadFromFile(const std::string& path);` - Parse a "word<TAB>IPA" TSV: one entry per line, '#'-comments and blank lines ignored, later duplicat
- `Add` (function, `micro/g2p/include/g2p/g2p_dict.h:38`) `void Add(std::string_view word, std::string_view ipa);` - Add/replace a single entry (word is lowercased, a-z only).
- `Lookup` (function, `micro/g2p/include/g2p/g2p_dict.h:41`) `bool Lookup(std::string_view word, std::string* ipa) const;` - On a hit, writes IPA to *ipa and returns true.
- `size` (function, `micro/g2p/include/g2p/g2p_dict.h:43`) `size_t size() const`
- `empty` (function, `micro/g2p/include/g2p/g2p_dict.h:44`) `bool empty() const`
- `EnsureSorted` (function, `micro/g2p/include/g2p/g2p_dict.h:47`) `private: void EnsureSorted() const;`
- `G2P_G2P_PHONES_H_` (macro, `micro/g2p/include/g2p/g2p_phones.h:7`) `#define G2P_G2P_PHONES_H_`
- `PhoneTokenList` (struct, `micro/g2p/include/g2p/g2p_phones.h:15`)
- `push` (function, `micro/g2p/include/g2p/g2p_phones.h:21`) `bool push(const char* tok);`
- `TextToPhoneList` (function, `micro/g2p/include/g2p/g2p_phones.h:27`) `bool TextToPhoneList(const char* text, PhoneTokenList* out, const Lexicon* overr` - Plain-text -> base-phone tokens without std::vector/std::string output. Returns false if the stream
- `TokenizeIpaToList` (function, `micro/g2p/include/g2p/g2p_phones.h:31`) `bool TokenizeIpaToList(const char* ipa, PhoneTokenList* out);` - IPA string -> base-phone tokens (heap-free output).
- `HasDigit` (function, `micro/g2p/src/g2p.cc:14`) `bool HasDigit(const std::string& s)`
- `ResolveToken` (function, `micro/g2p/src/g2p.cc:22`) `std::string ResolveToken(const std::string& tok, const Lexicon* overrides)` - Resolve a single token to an IPA string via the lookup pipeline.
- `TextToPhones` (function, `micro/g2p/src/g2p.cc:33`) `std::vector<std::string> TextToPhones(const std::string& text,`
- `DecodeIpa` (function, `micro/g2p/src/g2p_dict.cc:16`) `std::string DecodeIpa(uint32_t start, unsigned count)` - Decode `count` packed phone ids starting at body offset `start` into IPA.
- `RestartKey` (function, `micro/g2p/src/g2p_dict.cc:27`) `std::string RestartKey(int block)` - The restart (first) key of a block: its entry always has sharedPrefixLen == 0.
- `NormalizeWordKey` (function, `micro/g2p/src/g2p_dict.cc:35`) `std::string NormalizeWordKey(std::string_view word)`
- `DictLookup` (function, `micro/g2p/src/g2p_dict.cc:51`) `bool DictLookup(std::string_view word, std::string* ipa)`
- `Add` (function, `micro/g2p/src/g2p_dict.cc:106`) `void Lexicon::Add(std::string_view word, std::string_view ipa)`
- `EnsureSorted` (function, `micro/g2p/src/g2p_dict.cc:113`) `void Lexicon::EnsureSorted() const`
- `stable_sort` (function, `micro/g2p/src/g2p_dict.cc:115`) `std::stable_sort(       entries_.begin(), entries_.end(),       [](const auto& a`
- `Lookup` (function, `micro/g2p/src/g2p_dict.cc:132`) `bool Lexicon::Lookup(std::string_view word, std::string* ipa) const`
- `LoadFromFile` (function, `micro/g2p/src/g2p_dict.cc:145`) `bool Lexicon::LoadFromFile(const std::string& path)`
- `G2P_DICT_DATA_H_` (macro, `micro/g2p/src/g2p_dict_data.h:13`) `#define G2P_DICT_DATA_H_`
- `DigitSequenceIpa` (function, `micro/g2p/src/g2p_numbers.cc:40`) `std::string DigitSequenceIpa(std::string_view digits)`
- `Under100Ipa` (function, `micro/g2p/src/g2p_numbers.cc:51`) `std::string Under100Ipa(int n)`

## Internal vs External Edges

- Internal resolved imports (EXTRACTED): 39
- Cross-boundary resolved imports (EXTRACTED): 3

## Connections

- [EXTRACTED] depends_on community 6 <-> 1 (strength 0.9): Extracted import edge crosses communities: micro/neural-tts/src/neural_tts.cc imports micro/neural-tts/include/neural_tts/neural_tts.h.
- [EXTRACTED] depends_on community 6 <-> 9 (strength 0.9): Extracted import edge crosses communities: micro/neural-tts/src/neural_tts.cc imports micro/neural-tts/include/neural_tts/pb_decoder.h.
- [INFERRED] shares_context community 0 <-> 6 (strength 0.5): Inferred shared context (layer utility) with no import path between community 0 (core: moonshine-cpp) and community 6 (micro/g2p/src).

## Risks

- No scoped security, taint, cycle, or layer risks.

## Open Questions

- Why do 10 file(s) lack file-level docs (e.g. `micro/g2p/src/g2p.cc`)? What purpose do they serve?
- What would break if the most connected file in micro/g2p/src changed?
- Should micro/g2p/src be split, given cohesion 0.93?

## Sources

- `micro/g2p/include/g2p/g2p.h`
- `micro/g2p/include/g2p/g2p_dict.h`
- `micro/g2p/include/g2p/g2p_phones.h`
- `micro/g2p/src/g2p.cc`
- `micro/g2p/src/g2p_dict.cc`
- `micro/g2p/src/g2p_dict_data.h`
- `micro/g2p/src/g2p_numbers.cc`
- `micro/g2p/src/g2p_numbers.h`
- `micro/g2p/src/g2p_phones.cc`
- `micro/g2p/src/g2p_rules.cc`
- `micro/g2p/src/g2p_rules.h`
- `micro/g2p/src/ipa_tokens.cc`
- `micro/klatt-tts/include/tts/config.h`
- `micro/klatt-tts/include/tts/klatt.h`
- `micro/klatt-tts/include/tts/phonemes.h`
- `micro/klatt-tts/include/tts/synth_internal.h`
- `micro/klatt-tts/include/tts/synth_stream.h`
- `micro/klatt-tts/include/tts/tts.h`
- `micro/klatt-tts/src/config.cc`
- `micro/klatt-tts/src/klatt.cc`
- *... and 5 more*
