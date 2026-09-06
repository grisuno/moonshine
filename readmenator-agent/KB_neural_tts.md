# Subsystem: neural_tts

## micro/neural-tts/include/neural_tts/neural_tts.h
- Layer: utility
- Doc: neural_tts -- black-box text-to-speech for the RP2350.  Text in, 16 kHz mono int16 PCM chunks out. Everything else -- G2
- Language: h
- Symbols:
  - `Stats` (struct, line 70)
  - `NeuralTts` (class, line 40)
  - `ok` (function, line 48) `bool ok() const`
  - `stats` (function, line 84) `const Stats& stats() const`
  - `NEURAL_TTS_NEURAL_TTS_H_` (macro, line 31)

## micro/neural-tts/include/neural_tts/pack_format.h
- Layer: data_access
- Doc: Binary layout of the neural-TTS flash pack, mirroring scripts/export_neural_tts_pack.py (the writer is the source of tru
- Language: h
- Symbols:
  - `PackHeader` (struct, line 46)
  - `DiphoneTypeRec` (struct, line 96)
  - `DiphoneUnitRec` (struct, line 105)
  - `WordUnitRec` (struct, line 120)
  - `Pack` (class, line 141)
  - `Pack` (function, line 142) `public:
  explicit Pack(const uint8_t* base)
      : base_(base),
        h_(reinterpret_cast<con...`
  - `ok` (function, line 146) `bool ok() const`
  - `h` (function, line 151) `const PackHeader& h() const`
  - `raw` (function, line 152) `const uint8_t* raw(uint32_t off) const`
  - `model` (function, line 153) `const unsigned char* model() const`
  - `codebook` (function, line 155) `const int8_t* codebook(int s) const`
  - `codebook_scale` (function, line 158) `const float* codebook_scale(int s) const`
  - `dtypes` (function, line 161) `const DiphoneTypeRec* dtypes() const`
  - `dunits` (function, line 164) `const DiphoneUnitRec* dunits() const`
  - `wunits` (function, line 167) `const WordUnitRec* wunits() const`
  - `wkeys` (function, line 170) `const uint8_t* wkeys() const`
  - `centroid` (function, line 171) `const int8_t* centroid(int type_idx) const`
  - `codes` (function, line 175) `const uint8_t* codes(uint32_t off) const`
  - `f0_stream` (function, line 178) `const uint8_t* f0_stream(uint32_t off) const`
  - `phone_token` (function, line 181) `const char* phone_token(int id) const`
  - `dur_ratio` (function, line 184) `const float* dur_ratio() const`
  - `phone_class` (function, line 187) `const uint8_t* phone_class() const`
  - `func_idx` (function, line 188) `const uint16_t* func_idx() const`
  - `func_blob` (function, line 191) `const uint8_t* func_blob() const`
  - `NEURAL_TTS_PACK_FORMAT_H_` (macro, line 13)

## micro/neural-tts/include/neural_tts/pb_decoder.h
- Layer: utility
- Doc: TFLM wrapper for the Phase B RVQ decoder (s16x8: int16 activations, int8 weights). Streams WORLD-lite control frames out
- Language: h
- Symbols:
  - `Model` (struct, line 20)
  - `PbCodedUtterance` (struct, line 31)
  - `Config` (struct, line 40)
  - `PbDecoder` (class, line 38)
  - `ok` (function, line 54) `bool ok() const`
  - `decode_us` (function, line 75) `uint64_t decode_us() const`
  - `tiles_decoded` (function, line 76) `int tiles_decoded() const`
  - `NEURAL_TTS_PB_DECODER_H_` (macro, line 11)

## micro/neural-tts/include/neural_tts/worldlite_synth.h
- Layer: utility
- Doc: WORLD-lite vocoder synthesis (float32, kissfft) for the RP2350.  Renders 61-control WORLD-lite frames -- f0 (Hz, 0 = unv
- Language: h
- Symbols:
  - `WorldFrame` (struct, line 51)
  - `BinMap` (struct, line 92)
  - `WorldLiteSynth` (class, line 57)
  - `KissFftrPlanBytes` (function, line 39) `inline size_t KissFftrPlanBytes(int nfft, int inverse_fft)`
  - `KissFftrPairBytes` (function, line 46) `inline size_t KissFftrPairBytes(int nfft)`
  - `ok` (function, line 82) `bool ok() const`
  - `fwd_plan` (function, line 87) `const void* fwd_plan() const`
  - `inv_plan` (function, line 88) `const void* inv_plan() const`
  - `NEURAL_TTS_WORLDLITE_SYNTH_H_` (macro, line 23)
