# Subsystem: micro_neural-tts_src

## micro/neural-tts/src/hooks.cc
- Doc: Default (no-op) progress hooks. pb_decoder.cc calls tts_checkpoint / tts_trace before every TFLM...
- Layer: utility
- Language: cc

## micro/neural-tts/src/neural_tts.cc
- Doc: Black-box neural TTS pipeline (see neural_tts.h).
- Layer: utility
- Language: cc
- Symbols:
  - `F0RunSpan` (struct, line 153)
  - `Part` (struct, line 221)
  - `Range` (struct, line 317)
  - `EmitShim` (struct, line 337)
  - `RunSeg` (struct, line 370)
  - `RenderCtx` (struct, line 1686)
  - `Kind` (enum, line 222)
  - `BitReader` (class, line 120)
  - `Bump` (class, line 234)
  - `Engine` (class, line 260)
  - `NowUs` (function, line 55) `inline uint64_t NowUs()`
  - `Exp10` (function, line 91) `inline float Exp10(float x)`
  - `BitReader` (function, line 122) `public:
  explicit BitReader(const uint8_t* p) : p_(p)`
  - `get` (function, line 123) `uint32_t get(int bits)`
  - `ReadVarU8` (function, line 140) `int ReadVarU8(const uint8_t*& p)`
  - `DecodeF0Stream` (function, line 163) `void DecodeF0Stream(const uint8_t* p, int n_frames, float* out,
                    F0RunSpan* runs)`
  - `F0FromCode` (function, line 213) `inline float F0FromCode(uint8_t q)`
  - `Bump` (function, line 236) `public:
  Bump(uint8_t* base, size_t size) : base_(base), size_(size)`
  - `Alloc` (function, line 237) `void* Alloc(size_t bytes, size_t align = 4)`
  - `AllocArray` (function, line 244) `template <typename T>
  T* AllocArray(size_t n, size_t align = 4)`
  - `Mark` (function, line 247) `size_t Mark() const`
  - `Reset` (function, line 248) `void Reset(size_t mark)`
  - `remaining` (function, line 249) `size_t remaining() const`
  - `Engine` (function, line 262) `public:
  Engine(const Pack& pk, uint8_t* arena, size_t arena_size,
         NeuralTts::Stats* st...`
  - `IsSil` (function, line 292) `bool IsSil(int pid) const`
  - `IsGap` (function, line 296) `bool IsGap(int pid) const`
  - `Canon` (function, line 299) `int Canon(int pid) const`
  - `TimedEmit` (function, line 342) `static void TimedEmit(void* user, const int16_t* samples, int n)`
  - `BlendLenUnit` (function, line 352) `static int BlendLenUnit(int rule_n, int nat_n)`
  - `PhoneId` (function, line 438) `int Engine::PhoneId(const char* token) const`
  - `BuildRunsFromPtrs` (function, line 447) `int Engine::BuildRunsFromPtrs(const char* const* tokens, int n_tokens)`
  - `BuildRuns` (function, line 492) `int Engine::BuildRuns(const std::vector<std::string>& tokens)`
  - `FindDiphoneType` (function, line 499) `int Engine::FindDiphoneType(int a, int b) const`
  - `KeyCompare` (function, line 516) `static int KeyCompare(const uint8_t* a, int la, const uint8_t* b, int lb)`
  - `FindWord` (function, line 524) `int Engine::FindWord(const uint8_t* key, int len) const`
  - `RunAfterBuild` (function, line 547) `int Engine::RunAfterBuild(NeuralTts::EmitFn emit, void* user, bool plan_only)`
  - `Run` (function, line 597) `int Engine::Run(std::vector<std::string>* tokens, NeuralTts::EmitFn emit,
                void* u...`
  - `Run` (function, line 609) `int Engine::Run(const g2p::PhoneTokenList* phones, NeuralTts::EmitFn emit,
                void* ...`
  - `ComputeProsodyBuckets` (function, line 622) `void Engine::ComputeProsodyBuckets(int n)`
  - `ProsOff` (function, line 698) `float Engine::ProsOff(const float* table, int chunk_start) const`
  - `SegOff` (function, line 703) `float Engine::SegOff(const float* table, int seg) const`
  - `MatchWords` (function, line 707) `void Engine::MatchWords(int n)`
  - `SelectDiphones` (function, line 807) `void Engine::SelectDiphones(int n)`
  - `BuildParts` (function, line 928) `void Engine::BuildParts(int n)`
  - `UnpackCodes` (function, line 1081) `void Engine::UnpackCodes(uint32_t codes_off, int n_latents, uint16_t* out)`
  - `DecodedRows` (function, line 1097) `const int16_t* Engine::DecodedRows(bool word, int idx, int frame_base,
                          ...`
  - `WarpPositions` (function, line 1129) `static void WarpPositions(int m, int n, float* pos)`
  - `WarpAnchoredPositions` (function, line 1139) `static void WarpAnchoredPositions(int m, int n, bool anchor_end,
                                ...`
  - `BuildRanges` (function, line 1167) `int Engine::BuildRanges(const Part& p, int T, Range ranges[2]) const`
  - `MaterializeF0` (function, line 1187) `void Engine::MaterializeF0()`
  - `MaterializePartTrack` (function, line 1243) `void Engine::MaterializePartTrack(int pi)`
  - `GainEqAt` (function, line 1344) `void Engine::GainEqAt(int pi)`
  - `SmoothJoinAt` (function, line 1392) `void Engine::SmoothJoinAt(int j)`
  - `FrameLnEnergy` (function, line 1423) `float Engine::FrameLnEnergy(int t) const`
  - `LoudKnotAt` (function, line 1433) `static float LoudKnotAt(const int8_t* k, float scale, float u)`
  - `PlanLoudness` (function, line 1444) `void Engine::PlanLoudness()`
  - `AdvanceJoins` (function, line 1547) `void Engine::AdvanceJoins()`
  - `EnsureFinal` (function, line 1580) `void Engine::EnsureFinal(int t)`
  - `F0Pass` (function, line 1600) `void Engine::F0Pass()`
  - `RenderGetFrame` (function, line 1695) `static void RenderGetFrame(void* user, int t, WorldFrame* frame)`
  - `SynthesizeChunk` (function, line 1720) `int Engine::SynthesizeChunk(int lo, int hi, bool first, bool last,
                            Ne...`
  - `NeuralTts` (function, line 1970) `NeuralTts::NeuralTts(const uint8_t* pack, uint8_t* arena, size_t arena_size)
    : pack_(pack), a...`
  - `SynthesizeTokens` (function, line 1975) `int NeuralTts::SynthesizeTokens(void* tokens_vec, EmitFn emit, void* user,
                      ...`
  - `Synthesize` (function, line 1984) `int NeuralTts::Synthesize(const char* text, EmitFn emit, void* user)`
  - `SynthesizeIpa` (function, line 2001) `int NeuralTts::SynthesizeIpa(const char* ipa, EmitFn emit, void* user)`
  - `EstimateSamples` (function, line 2018) `int NeuralTts::EstimateSamples(const char* text)`
  - `EstimateSamplesIpa` (function, line 2035) `int NeuralTts::EstimateSamplesIpa(const char* ipa)`
  - `exp2f` (function, line 205) `kPackF0BaseHz * exp2f(code / kPackF0StepsPerOctave);`
  - `NT_CHECKPOINT2` (macro, line 45) `#define NT_CHECKPOINT2(v)`
  - `NT_CHECKPOINT2` (macro, line 47) `#define NT_CHECKPOINT2(v)`
  - `NEURAL_TTS_MAX_CHUNK_FRAMES` (macro, line 80) `#define NEURAL_TTS_MAX_CHUNK_FRAMES`
- Depends on: `micro/g2p/include/g2p/g2p.h`, `micro/g2p/include/g2p/g2p_phones.h`, `micro/klatt-tts/include/tts/config.h`, `micro/klatt-tts/include/tts/synth_internal.h`, `micro/neural-tts/include/neural_tts/neural_tts.h`, `micro/neural-tts/include/neural_tts/pb_decoder.h`, `micro/neural-tts/include/neural_tts/worldlite_synth.h`

## micro/neural-tts/src/pb_decoder.cc
- Doc: Progress hook (defined by the app): records where the pipeline is for post-reboot hang reports...
- Layer: utility
- Language: cc
- Symbols:
  - `NowUs` (function, line 37) `uint64_t NowUs()`
  - `Exp10` (function, line 47) `inline float Exp10(float x)`
  - `BeginEvent` (function, line 57) `public:
  uint32_t BeginEvent(const char*) override`
  - `EndEvent` (function, line 62) `void EndEvent(uint32_t) override`
  - `Reset` (function, line 63) `void Reset()`
  - `PbDecoder` (function, line 73) `PbDecoder::PbDecoder(const Config& config, uint8_t* arena,
                     size_t arena_byte...`
  - `arena_used_bytes` (function, line 131) `size_t PbDecoder::arena_used_bytes() const`
  - `BeginUtterance` (function, line 135) `void PbDecoder::BeginUtterance(const PbCodedUtterance* utt)`
  - `DecodeTileAt` (function, line 144) `bool PbDecoder::DecodeTileAt(int latent_start)`
  - `GetFrame` (function, line 201) `void PbDecoder::GetFrame(int t, WorldFrame* frame)`
  - `GetFrameThunk` (function, line 235) `void PbDecoder::GetFrameThunk(void* user, int t, WorldFrame* frame)`
  - `ReadRows` (function, line 239) `void PbDecoder::ReadRows(int t0, int n, int16_t* out)`
  - `PB_CHECKPOINT` (macro, line 23) `#define PB_CHECKPOINT(v)`
  - `PB_TRACE` (macro, line 24) `#define PB_TRACE(tag, val)`
  - `PB_CHECKPOINT` (macro, line 26) `#define PB_CHECKPOINT(v)`
  - `PB_TRACE` (macro, line 29) `#define PB_TRACE(tag, val)`
- Depends on: `micro/neural-tts/include/neural_tts/pb_decoder.h`

## micro/neural-tts/src/worldlite_synth.cc
- Doc: Float32 kissfft port of WORLD Synthesis() specialized to the WORLD-lite band parameterization.
- Layer: utility
- Language: cc
- Symbols:
  - `HzToMel` (function, line 48) `float HzToMel(float hz)`
  - `InitTables` (function, line 52) `void WorldLiteSynth::InitTables()`
  - `WorldLiteSynth` (function, line 89) `WorldLiteSynth::WorldLiteSynth() : rng_state_(0x8f1bbcdcu), owns_fft_plans_(true)`
  - `WorldLiteSynth` (function, line 95) `WorldLiteSynth::WorldLiteSynth(void* plan_mem, size_t plan_mem_bytes)
    : rng_state_(0x8f1bbcdc...`
  - `FftSelfTest` (function, line 127) `float WorldLiteSynth::FftSelfTest()`
  - `Randn` (function, line 143) `float WorldLiteSynth::Randn()`
  - `ExpandFrame` (function, line 155) `void WorldLiteSynth::ExpandFrame(const WorldFrame& f, float* spec_pow,
                          ...`
  - `MinimumPhase` (function, line 171) `void WorldLiteSynth::MinimumPhase(const float* log_amp_half,
                                  ki...`
  - `RenderPulse` (function, line 200) `void WorldLiteSynth::RenderPulse(const float* spec_pow, const float* ap,
                        ...`
  - `FlushTo` (function, line 296) `void WorldLiteSynth::FlushTo(int abs_pos, float gain, EmitFn emit,
                             v...`
  - `Synthesize` (function, line 315) `void WorldLiteSynth::Synthesize(GetFrameFn get_frame, void* frame_user,
                         ...`
  - `WL_CHECKPOINT` (macro, line 23) `#define WL_CHECKPOINT(v)`
  - `WL_CHECKPOINT2` (macro, line 24) `#define WL_CHECKPOINT2(v)`
  - `WL_TRACE_RING` (macro, line 25) `#define WL_TRACE_RING(tag, val)`
  - `WL_CHECKPOINT` (macro, line 27) `#define WL_CHECKPOINT(v)`
  - `WL_CHECKPOINT2` (macro, line 30) `#define WL_CHECKPOINT2(v)`
  - `WL_TRACE_RING` (macro, line 33) `#define WL_TRACE_RING(tag, val)`
- Depends on: `micro/neural-tts/include/neural_tts/worldlite_synth.h`
