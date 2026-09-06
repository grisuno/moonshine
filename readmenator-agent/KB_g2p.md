# Subsystem: g2p

## micro/g2p/include/g2p/g2p.h
- Layer: utility
- Doc: English grapheme-to-phoneme front end.  Pipeline per word: runtime override -> number normalizer -> baked common-word di
- Language: h
- Symbols:
  - `G2P_G2P_H_` (macro, line 18)

## micro/g2p/include/g2p/g2p_dict.h
- Layer: infrastructure
- Doc: Baked common-word pronunciation dictionary + runtime override table.  The baked dictionary is a read-only, flash-residen
- Language: h
- Symbols:
  - `Lexicon` (class, line 30)
  - `size` (function, line 42) `size_t size() const`
  - `empty` (function, line 44) `bool empty() const`
  - `G2P_G2P_DICT_H_` (macro, line 15)

## micro/g2p/include/g2p/g2p_phones.h
- Layer: utility
- Doc: Heap-free phone-token list for on-device TTS (CYW43 leaves little malloc headroom).  PhoneTokenList stores the flat toke
- Language: h
- Symbols:
  - `PhoneTokenList` (struct, line 15)
  - `G2P_G2P_PHONES_H_` (macro, line 7)
