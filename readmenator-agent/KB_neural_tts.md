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
  - `NeuralTts` (function, line 44) `NeuralTts(const uint8_t* pack, uint8_t* arena, size_t arena_size);`
  - `void` (function, line 52) `typedef void (*EmitFn)(void* user, const int16_t* samples, int n);`
  - `Synthesize` (function, line 57) `int Synthesize(const char* text, EmitFn emit, void* user);`
  - `SynthesizeIpa` (function, line 60) `int SynthesizeIpa(const char* ipa, EmitFn emit, void* user);`
  - `EstimateSamples` (function, line 65) `int EstimateSamples(const char* text);`
  - `EstimateSamplesIpa` (function, line 66) `int EstimateSamplesIpa(const char* ipa);`
  - `SynthesizeTokens` (function, line 85) `private: int SynthesizeTokens(void* tokens_vec, EmitFn emit, void* user, bool plan_only);`
  - `NEURAL_TTS_NEURAL_TTS_H_` (macro, line 31) `#define NEURAL_TTS_NEURAL_TTS_H_`
- Depends on: `micro/neural-tts/include/neural_tts/pack_format.h`
- Imported by: `micro/examples/rp2350/src/audio_service.cc`, `micro/examples/rp2350/src/main_i2s_audio_test.cc`, `micro/examples/rp2350/src/tts_service.cc`, `micro/neural-tts/host/tts_cli.cc`, `micro/neural-tts/src/neural_tts.cc`

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
  - `NEURAL_TTS_PACK_FORMAT_H_` (macro, line 13) `#define NEURAL_TTS_PACK_FORMAT_H_`
- Imported by: `micro/neural-tts/include/neural_tts/neural_tts.h`

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
  - `PbDecoder` (function, line 53) `PbDecoder(const Config& config, uint8_t* arena, size_t arena_bytes);`
  - `arena_used_bytes` (function, line 56) `size_t arena_used_bytes() const;`
  - `BeginUtterance` (function, line 57) `void BeginUtterance(const PbCodedUtterance* utt);`
  - `GetFrameThunk` (function, line 61) `static void GetFrameThunk(void* user, int t, WorldFrame* frame);`
  - `GetFrame` (function, line 62) `void GetFrame(int t, WorldFrame* frame);`
  - `ReadRows` (function, line 72) `void ReadRows(int t0, int n, int16_t* out);`
  - `DecodeTileAt` (function, line 81) `bool DecodeTileAt(int latent_start);`
  - `NEURAL_TTS_PB_DECODER_H_` (macro, line 11) `#define NEURAL_TTS_PB_DECODER_H_`
- Depends on: `micro/neural-tts/include/neural_tts/worldlite_synth.h`
- Imported by: `micro/examples/rp2350/src/main_step6_decoder.cc`, `micro/examples/rp2350/src/main_step7_synthesize.cc`, `micro/examples/rp2350/src/main_step7b_framesweep.cc`, `micro/examples/rp2350/src/main_tts_ladder_test.cc`, `micro/neural-tts/src/neural_tts.cc`, `micro/neural-tts/src/pb_decoder.cc`

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
  - `kiss_fftr_alloc` (function, line 41) `kiss_fftr_alloc(nfft, inverse_fft, nullptr, &n);`
  - `WorldLiteSynth` (function, line 60) `WorldLiteSynth();`
  - `void` (function, line 71) `typedef void (*GetFrameFn)(void* user, int t, WorldFrame* frame);`
  - `Synthesize` (function, line 77) `void Synthesize(GetFrameFn get_frame, void* frame_user, int num_frames, float gain, EmitFn emit, void* emit_user);`
  - `FftSelfTest` (function, line 89) `float FftSelfTest();`
  - `InitTables` (function, line 96) `void InitTables();`
  - `ExpandFrame` (function, line 98) `void ExpandFrame(const WorldFrame& f, float* spec_pow, float* ap) const;`
  - `MinimumPhase` (function, line 99) `void MinimumPhase(const float* log_amp_half, kiss_fft_cpx* min_phase);`
  - `RenderPulse` (function, line 100) `void RenderPulse(const float* spec_pow, const float* ap, bool voiced, int noise_size, float frac_shift_s, float* response);`
  - `FlushTo` (function, line 102) `void FlushTo(int abs_pos, float gain, EmitFn emit, void* emit_user);`
  - `Randn` (function, line 103) `float Randn();`
  - `NEURAL_TTS_WORLDLITE_SYNTH_H_` (macro, line 23) `#define NEURAL_TTS_WORLDLITE_SYNTH_H_`
- Imported by: `micro/examples/rp2350/src/main_step5_synth.cc`, `micro/examples/rp2350/src/main_step6_decoder.cc`, `micro/examples/rp2350/src/main_step7_synthesize.cc`, `micro/examples/rp2350/src/main_step7c_synthonly.cc`, `micro/examples/rp2350/src/main_tts_ladder_test.cc`, `micro/neural-tts/host/worldlite_synth_cli.cc`, `micro/neural-tts/include/neural_tts/pb_decoder.h`, `micro/neural-tts/src/neural_tts.cc`, `micro/neural-tts/src/worldlite_synth.cc`
