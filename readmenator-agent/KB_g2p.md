# Subsystem: g2p

## micro/g2p/include/g2p/g2p.h
- Layer: utility
- Doc: English grapheme-to-phoneme front end.  Pipeline per word: runtime override -> number normalizer -> baked common-word di
- Language: h
- Symbols:
  - `G2P_G2P_H_` (macro, line 18) `#define G2P_G2P_H_`
- Depends on: `micro/g2p/include/g2p/g2p_dict.h`
- Imported by: `micro/g2p/src/g2p.cc`, `micro/g2p/src/g2p_phones.cc`, `micro/g2p/src/ipa_tokens.cc`, `micro/klatt-tts/src/synth_stream.cc`, `micro/klatt-tts/tests/tts_test.cc`, `micro/neural-tts/src/neural_tts.cc`

## micro/g2p/include/g2p/g2p_dict.h
- Layer: infrastructure
- Doc: Baked common-word pronunciation dictionary + runtime override table.  The baked dictionary is a read-only, flash-residen
- Language: h
- Symbols:
  - `Lexicon` (class, line 30)
  - `size` (function, line 43) `size_t size() const`
  - `empty` (function, line 44) `bool empty() const`
  - `DictLookup` (function, line 26) `bool DictLookup(std::string_view word, std::string* ipa);`
  - `LoadFromFile` (function, line 35) `bool LoadFromFile(const std::string& path);`
  - `Add` (function, line 38) `void Add(std::string_view word, std::string_view ipa);`
  - `Lookup` (function, line 41) `bool Lookup(std::string_view word, std::string* ipa) const;`
  - `EnsureSorted` (function, line 47) `private: void EnsureSorted() const;`
  - `G2P_G2P_DICT_H_` (macro, line 15) `#define G2P_G2P_DICT_H_`
- Imported by: `micro/g2p/include/g2p/g2p.h`, `micro/g2p/include/g2p/g2p_phones.h`, `micro/g2p/src/g2p.cc`, `micro/g2p/src/g2p_dict.cc`, `micro/g2p/src/g2p_phones.cc`, `micro/klatt-tts/include/tts/synth_stream.h`

## micro/g2p/include/g2p/g2p_phones.h
- Layer: utility
- Doc: Heap-free phone-token list for on-device TTS (CYW43 leaves little malloc headroom).  PhoneTokenList stores the flat toke
- Language: h
- Symbols:
  - `PhoneTokenList` (struct, line 15)
  - `push` (function, line 21) `bool push(const char* tok);`
  - `TextToPhoneList` (function, line 27) `bool TextToPhoneList(const char* text, PhoneTokenList* out, const Lexicon* overrides = nullptr);`
  - `TokenizeIpaToList` (function, line 31) `bool TokenizeIpaToList(const char* ipa, PhoneTokenList* out);`
  - `G2P_G2P_PHONES_H_` (macro, line 7) `#define G2P_G2P_PHONES_H_`
- Depends on: `micro/g2p/include/g2p/g2p_dict.h`
- Imported by: `micro/g2p/src/g2p_phones.cc`, `micro/neural-tts/src/neural_tts.cc`
