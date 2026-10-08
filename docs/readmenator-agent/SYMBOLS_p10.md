# Symbols (page 10 of 12)
Previous: [SYMBOLS_p9.md](SYMBOLS_p9.md)

| Symbol | Kind | File:Line | Signature |
|--------|------|-----------|-----------|
| `ComputeProsodyBuckets` | function | `micro/neural-tts/src/neural_tts.cc:622` | `void Engine::ComputeProsodyBuckets(int n)` |
| `DecodeF0Stream` | function | `micro/neural-tts/src/neural_tts.cc:163` | `void DecodeF0Stream(const uint8_t* p, int n_frames, float* out,                     F0RunSpan* runs)` |
| `DecodedRows` | function | `micro/neural-tts/src/neural_tts.cc:1097` | `const int16_t* Engine::DecodedRows(bool word, int idx, int frame_base,                           ...` |
| `EmitShim` | struct | `micro/neural-tts/src/neural_tts.cc:337` | `` |
| `Engine` | class | `micro/neural-tts/src/neural_tts.cc:260` | `` |
| `Engine` | function | `micro/neural-tts/src/neural_tts.cc:262` | `public:   Engine(const Pack& pk, uint8_t* arena, size_t arena_size,          NeuralTts::Stats* st...` |
| `EnsureFinal` | function | `micro/neural-tts/src/neural_tts.cc:1580` | `void Engine::EnsureFinal(int t)` |
| `EstimateSamples` | function | `micro/neural-tts/src/neural_tts.cc:2018` | `int NeuralTts::EstimateSamples(const char* text)` |
| `EstimateSamplesIpa` | function | `micro/neural-tts/src/neural_tts.cc:2035` | `int NeuralTts::EstimateSamplesIpa(const char* ipa)` |
| `Exp10` | function | `micro/neural-tts/src/neural_tts.cc:91` | `inline float Exp10(float x)` |
| `F0FromCode` | function | `micro/neural-tts/src/neural_tts.cc:213` | `inline float F0FromCode(uint8_t q)` |
| `F0Pass` | function | `micro/neural-tts/src/neural_tts.cc:1600` | `void Engine::F0Pass()` |
| `F0RunSpan` | struct | `micro/neural-tts/src/neural_tts.cc:153` | `` |
| `FindDiphoneType` | function | `micro/neural-tts/src/neural_tts.cc:499` | `int Engine::FindDiphoneType(int a, int b) const` |
| `FindWord` | function | `micro/neural-tts/src/neural_tts.cc:524` | `int Engine::FindWord(const uint8_t* key, int len) const` |
| `FrameLnEnergy` | function | `micro/neural-tts/src/neural_tts.cc:1423` | `float Engine::FrameLnEnergy(int t) const` |
| `GainEqAt` | function | `micro/neural-tts/src/neural_tts.cc:1344` | `void Engine::GainEqAt(int pi)` |
| `IsGap` | function | `micro/neural-tts/src/neural_tts.cc:296` | `bool IsGap(int pid) const` |
| `IsSil` | function | `micro/neural-tts/src/neural_tts.cc:292` | `bool IsSil(int pid) const` |
| `KeyCompare` | function | `micro/neural-tts/src/neural_tts.cc:516` | `static int KeyCompare(const uint8_t* a, int la, const uint8_t* b, int lb)` |
| `Kind` | enum | `micro/neural-tts/src/neural_tts.cc:222` | `` |
| `LoudKnotAt` | function | `micro/neural-tts/src/neural_tts.cc:1433` | `static float LoudKnotAt(const int8_t* k, float scale, float u)` |
| `Mark` | function | `micro/neural-tts/src/neural_tts.cc:247` | `size_t Mark() const` |
| `MatchWords` | function | `micro/neural-tts/src/neural_tts.cc:707` | `void Engine::MatchWords(int n)` |
| `MaterializeF0` | function | `micro/neural-tts/src/neural_tts.cc:1187` | `void Engine::MaterializeF0()` |
| `MaterializePartTrack` | function | `micro/neural-tts/src/neural_tts.cc:1243` | `void Engine::MaterializePartTrack(int pi)` |
| `NEURAL_TTS_MAX_CHUNK_FRAMES` | macro | `micro/neural-tts/src/neural_tts.cc:80` | `#define NEURAL_TTS_MAX_CHUNK_FRAMES` |
| `NT_CHECKPOINT2` | macro | `micro/neural-tts/src/neural_tts.cc:45` | `#define NT_CHECKPOINT2(v)` |
| `NT_CHECKPOINT2` | macro | `micro/neural-tts/src/neural_tts.cc:47` | `#define NT_CHECKPOINT2(v)` |
| `NeuralTts` | function | `micro/neural-tts/src/neural_tts.cc:1970` | `NeuralTts::NeuralTts(const uint8_t* pack, uint8_t* arena, size_t arena_size)     : pack_(pack), a...` |
| `NowUs` | function | `micro/neural-tts/src/neural_tts.cc:55` | `inline uint64_t NowUs()` |
| `Part` | struct | `micro/neural-tts/src/neural_tts.cc:221` | `` |
| `PhoneId` | function | `micro/neural-tts/src/neural_tts.cc:438` | `int Engine::PhoneId(const char* token) const` |
| `PlanLoudness` | function | `micro/neural-tts/src/neural_tts.cc:1444` | `void Engine::PlanLoudness()` |
| `ProsOff` | function | `micro/neural-tts/src/neural_tts.cc:698` | `float Engine::ProsOff(const float* table, int chunk_start) const` |
| `Range` | struct | `micro/neural-tts/src/neural_tts.cc:317` | `` |
| `ReadVarU8` | function | `micro/neural-tts/src/neural_tts.cc:140` | `int ReadVarU8(const uint8_t*& p)` |
| `RenderCtx` | struct | `micro/neural-tts/src/neural_tts.cc:1686` | `` |
| `RenderGetFrame` | function | `micro/neural-tts/src/neural_tts.cc:1695` | `static void RenderGetFrame(void* user, int t, WorldFrame* frame)` |
| `Reset` | function | `micro/neural-tts/src/neural_tts.cc:248` | `void Reset(size_t mark)` |
| `Run` | function | `micro/neural-tts/src/neural_tts.cc:597` | `int Engine::Run(std::vector<std::string>* tokens, NeuralTts::EmitFn emit,                 void* u...` |
| `Run` | function | `micro/neural-tts/src/neural_tts.cc:609` | `int Engine::Run(const g2p::PhoneTokenList* phones, NeuralTts::EmitFn emit,                 void* ...` |
| `RunAfterBuild` | function | `micro/neural-tts/src/neural_tts.cc:547` | `int Engine::RunAfterBuild(NeuralTts::EmitFn emit, void* user, bool plan_only)` |
| `RunSeg` | struct | `micro/neural-tts/src/neural_tts.cc:370` | `` |
| `SegOff` | function | `micro/neural-tts/src/neural_tts.cc:703` | `float Engine::SegOff(const float* table, int seg) const` |
| `SelectDiphones` | function | `micro/neural-tts/src/neural_tts.cc:807` | `void Engine::SelectDiphones(int n)` |
| `SmoothJoinAt` | function | `micro/neural-tts/src/neural_tts.cc:1392` | `void Engine::SmoothJoinAt(int j)` |
| `Synthesize` | function | `micro/neural-tts/src/neural_tts.cc:1984` | `int NeuralTts::Synthesize(const char* text, EmitFn emit, void* user)` |
| `SynthesizeChunk` | function | `micro/neural-tts/src/neural_tts.cc:1720` | `int Engine::SynthesizeChunk(int lo, int hi, bool first, bool last,                             Ne...` |
| `SynthesizeIpa` | function | `micro/neural-tts/src/neural_tts.cc:2001` | `int NeuralTts::SynthesizeIpa(const char* ipa, EmitFn emit, void* user)` |
| `SynthesizeTokens` | function | `micro/neural-tts/src/neural_tts.cc:1975` | `int NeuralTts::SynthesizeTokens(void* tokens_vec, EmitFn emit, void* user,                       ...` |
| `TimedEmit` | function | `micro/neural-tts/src/neural_tts.cc:342` | `static void TimedEmit(void* user, const int16_t* samples, int n)` |
| `UnpackCodes` | function | `micro/neural-tts/src/neural_tts.cc:1081` | `void Engine::UnpackCodes(uint32_t codes_off, int n_latents, uint16_t* out)` |
| `WarpAnchoredPositions` | function | `micro/neural-tts/src/neural_tts.cc:1139` | `static void WarpAnchoredPositions(int m, int n, bool anchor_end,                                 ...` |
| `WarpPositions` | function | `micro/neural-tts/src/neural_tts.cc:1129` | `static void WarpPositions(int m, int n, float* pos)` |
| `exp2f` | function | `micro/neural-tts/src/neural_tts.cc:205` | `kPackF0BaseHz * exp2f(code / kPackF0StepsPerOctave);` |
| `get` | function | `micro/neural-tts/src/neural_tts.cc:123` | `uint32_t get(int bits)` |
| `remaining` | function | `micro/neural-tts/src/neural_tts.cc:249` | `size_t remaining() const` |
| `BeginEvent` | function | `micro/neural-tts/src/pb_decoder.cc:57` | `public:   uint32_t BeginEvent(const char*) override` |
| `BeginUtterance` | function | `micro/neural-tts/src/pb_decoder.cc:135` | `void PbDecoder::BeginUtterance(const PbCodedUtterance* utt)` |
| `DecodeTileAt` | function | `micro/neural-tts/src/pb_decoder.cc:144` | `bool PbDecoder::DecodeTileAt(int latent_start)` |
| `EndEvent` | function | `micro/neural-tts/src/pb_decoder.cc:62` | `void EndEvent(uint32_t) override` |
| `Exp10` | function | `micro/neural-tts/src/pb_decoder.cc:47` | `inline float Exp10(float x)` |
| `GetFrame` | function | `micro/neural-tts/src/pb_decoder.cc:201` | `void PbDecoder::GetFrame(int t, WorldFrame* frame)` |
| `GetFrameThunk` | function | `micro/neural-tts/src/pb_decoder.cc:235` | `void PbDecoder::GetFrameThunk(void* user, int t, WorldFrame* frame)` |
| `NowUs` | function | `micro/neural-tts/src/pb_decoder.cc:37` | `uint64_t NowUs()` |
| `PB_CHECKPOINT` | macro | `micro/neural-tts/src/pb_decoder.cc:23` | `#define PB_CHECKPOINT(v)` |
| `PB_CHECKPOINT` | macro | `micro/neural-tts/src/pb_decoder.cc:26` | `#define PB_CHECKPOINT(v)` |
| `PB_TRACE` | macro | `micro/neural-tts/src/pb_decoder.cc:24` | `#define PB_TRACE(tag, val)` |
| `PB_TRACE` | macro | `micro/neural-tts/src/pb_decoder.cc:29` | `#define PB_TRACE(tag, val)` |
| `PbDecoder` | function | `micro/neural-tts/src/pb_decoder.cc:73` | `PbDecoder::PbDecoder(const Config& config, uint8_t* arena,                      size_t arena_byte...` |
| `ReadRows` | function | `micro/neural-tts/src/pb_decoder.cc:239` | `void PbDecoder::ReadRows(int t0, int n, int16_t* out)` |
| `Reset` | function | `micro/neural-tts/src/pb_decoder.cc:63` | `void Reset()` |
| `arena_used_bytes` | function | `micro/neural-tts/src/pb_decoder.cc:131` | `size_t PbDecoder::arena_used_bytes() const` |
| `ExpandFrame` | function | `micro/neural-tts/src/worldlite_synth.cc:155` | `void WorldLiteSynth::ExpandFrame(const WorldFrame& f, float* spec_pow,                           ...` |
| `FftSelfTest` | function | `micro/neural-tts/src/worldlite_synth.cc:127` | `float WorldLiteSynth::FftSelfTest()` |
| `FlushTo` | function | `micro/neural-tts/src/worldlite_synth.cc:296` | `void WorldLiteSynth::FlushTo(int abs_pos, float gain, EmitFn emit,                              v...` |
| `HzToMel` | function | `micro/neural-tts/src/worldlite_synth.cc:48` | `float HzToMel(float hz)` |
| `InitTables` | function | `micro/neural-tts/src/worldlite_synth.cc:52` | `void WorldLiteSynth::InitTables()` |
| `MinimumPhase` | function | `micro/neural-tts/src/worldlite_synth.cc:171` | `void WorldLiteSynth::MinimumPhase(const float* log_amp_half,                                   ki...` |
| `Randn` | function | `micro/neural-tts/src/worldlite_synth.cc:143` | `float WorldLiteSynth::Randn()` |
| `RenderPulse` | function | `micro/neural-tts/src/worldlite_synth.cc:200` | `void WorldLiteSynth::RenderPulse(const float* spec_pow, const float* ap,                         ...` |
| `Synthesize` | function | `micro/neural-tts/src/worldlite_synth.cc:315` | `void WorldLiteSynth::Synthesize(GetFrameFn get_frame, void* frame_user,                          ...` |
| `WL_CHECKPOINT` | macro | `micro/neural-tts/src/worldlite_synth.cc:23` | `#define WL_CHECKPOINT(v)` |
| `WL_CHECKPOINT` | macro | `micro/neural-tts/src/worldlite_synth.cc:27` | `#define WL_CHECKPOINT(v)` |
| `WL_CHECKPOINT2` | macro | `micro/neural-tts/src/worldlite_synth.cc:24` | `#define WL_CHECKPOINT2(v)` |
| `WL_CHECKPOINT2` | macro | `micro/neural-tts/src/worldlite_synth.cc:30` | `#define WL_CHECKPOINT2(v)` |
| `WL_TRACE_RING` | macro | `micro/neural-tts/src/worldlite_synth.cc:25` | `#define WL_TRACE_RING(tag, val)` |
| `WL_TRACE_RING` | macro | `micro/neural-tts/src/worldlite_synth.cc:33` | `#define WL_TRACE_RING(tag, val)` |
| `WorldLiteSynth` | function | `micro/neural-tts/src/worldlite_synth.cc:89` | `WorldLiteSynth::WorldLiteSynth() : rng_state_(0x8f1bbcdcu), owns_fft_plans_(true)` |
| `WorldLiteSynth` | function | `micro/neural-tts/src/worldlite_synth.cc:95` | `WorldLiteSynth::WorldLiteSynth(void* plan_mem, size_t plan_mem_bytes)     : rng_state_(0x8f1bbcdc...` |
| `WaveformAugment` | class | `micro/stt-training/stt_training/augment.py:25` | `class WaveformAugment(Module)` |
| `__init__` | method | `micro/stt-training/stt_training/augment.py:36` | `def __init__(self, sample_rate, musan_noise_dir, rir_dir, gain_db, noise_snr_min, noise_snr_max, bandpass_p...` |
| `_bandpass` | method | `micro/stt-training/stt_training/augment.py:194` | `def _bandpass(self, x, b, t, dev)` |
| `_bg_noise` | method | `micro/stt-training/stt_training/augment.py:210` | `def _bg_noise(self, x, b, t, dev)` |
| `_colored_noise` | method | `micro/stt-training/stt_training/augment.py:181` | `def _colored_noise(self, x, b, t, dev)` |
| `_gain` | method | `micro/stt-training/stt_training/augment.py:155` | `def _gain(self, x, b, dev)` |
| `_load_concat_noise` | method | `micro/stt-training/stt_training/augment.py:82` | `def _load_concat_noise(self, noise_dir, max_seconds)` |
| `_load_rirs` | method | `micro/stt-training/stt_training/augment.py:106` | `def _load_rirs(self, rir_dir, max_rirs)` |
| `_mask` | method | `micro/stt-training/stt_training/augment.py:148` | `def _mask(p, b, dev)` |
| `_polarity` | method | `micro/stt-training/stt_training/augment.py:161` | `def _polarity(self, x, b, dev)` |
| `_rir` | method | `micro/stt-training/stt_training/augment.py:219` | `def _rir(self, x, b, t, dev)` |
| `_rms` | method | `micro/stt-training/stt_training/augment.py:152` | `def _rms(x)` |
| `_shift` | method | `micro/stt-training/stt_training/augment.py:165` | `def _shift(self, x, b, t, dev)` |
| `_snr_scale` | method | `micro/stt-training/stt_training/augment.py:174` | `def _snr_scale(self, sig, noise, b, dev)` |
| `forward` | method | `micro/stt-training/stt_training/augment.py:238` | `def forward(self, waveform)` |
| `has_external_data` | method | `micro/stt-training/stt_training/augment.py:143` | `def has_external_data(self)` |
| `n_transforms` | method | `micro/stt-training/stt_training/augment.py:139` | `def n_transforms(self)` |
| `load_model` | function | `micro/stt-training/stt_training/checkpoint.py:35` | `def load_model(path, device)` |
| `load_representative_waveforms` | function | `micro/stt-training/stt_training/checkpoint.py:61` | `def load_representative_waveforms(data_roots, n, target_samples, sample_rate, seed)` |
| `resolve_checkpoint` | function | `micro/stt-training/stt_training/checkpoint.py:17` | `def resolve_checkpoint(path)` |
| `SpeechCommandsDataset` | class | `micro/stt-training/stt_training/dataset.py:51` | `class SpeechCommandsDataset(Dataset)` |
| `__getitem__` | method | `micro/stt-training/stt_training/dataset.py:109` | `def __getitem__(self, idx)` |
| `__init__` | method | `micro/stt-training/stt_training/dataset.py:54` | `def __init__(self, roots, classes, sample_rate, clip_seconds)` |
| `__len__` | method | `micro/stt-training/stt_training/dataset.py:89` | `def __len__(self)` |
| `_load_wav` | method | `micro/stt-training/stt_training/dataset.py:92` | `def _load_wav(self, path)` |
| `_warn_decode_failure` | function | `micro/stt-training/stt_training/dataset.py:27` | `def _warn_decode_failure(src, exc)` |
| `build_class_balanced_sampler` | method | `micro/stt-training/stt_training/dataset.py:142` | `def build_class_balanced_sampler(labels, power)` |
| `load_waveform` | method | `micro/stt-training/stt_training/dataset.py:116` | `def load_waveform(self, idx)` |
| `mixup` | method | `micro/stt-training/stt_training/dataset.py:190` | `def mixup(x, y, num_classes, alpha)` |
| `report_class_coverage` | method | `micro/stt-training/stt_training/dataset.py:163` | `def report_class_coverage(dataset, classes)` |
| `soft_cross_entropy` | method | `micro/stt-training/stt_training/dataset.py:205` | `def soft_cross_entropy(logits, soft_targets, smoothing)` |
| `speaker_independent_split` | method | `micro/stt-training/stt_training/dataset.py:120` | `def speaker_independent_split(dataset, val_fraction, seed)` |
| `voice_id_from_path` | function | `micro/stt-training/stt_training/dataset.py:39` | `def voice_id_from_path(path)` |
| `voice_ids` | method | `micro/stt-training/stt_training/dataset.py:113` | `def voice_ids(self)` |
| `_confusions` | function | `micro/stt-training/stt_training/evaluate.py:30` | `def _confusions(y_true, y_pred, classes, top)` |
| `_report` | function | `micro/stt-training/stt_training/evaluate.py:102` | `def _report(name, y_true, y_pred, classes)` |
| `main` | function | `micro/stt-training/stt_training/evaluate.py:38` | `def main()` |
| `_default_calibration_roots` | function | `micro/stt-training/stt_training/export.py:197` | `def _default_calibration_roots(args)` |
| `_inline_buffers` | function | `micro/stt-training/stt_training/export.py:37` | `def _inline_buffers(buf)` |
| `_interpreter` | function | `micro/stt-training/stt_training/export.py:62` | `def _interpreter(path)` |
| `_run_tflite` | function | `micro/stt-training/stt_training/export.py:70` | `def _run_tflite(interp, feats)` |
| `build_argparser` | function | `micro/stt-training/stt_training/export.py:207` | `def build_argparser()` |
| `export` | function | `micro/stt-training/stt_training/export.py:86` | `def export(args)` |
| `main` | function | `micro/stt-training/stt_training/export.py:220` | `def main()` |
| `LogMelSpectrogram` | class | `micro/stt-training/stt_training/features.py:16` | `class LogMelSpectrogram(Module)` |
| `SpecAugment` | class | `micro/stt-training/stt_training/features.py:70` | `class SpecAugment(Module)` |
| `__init__` | method | `micro/stt-training/stt_training/features.py:23` | `def __init__(self, sample_rate, n_fft, hop_length, n_mels, f_min, f_max, target_frames, eps)` |
| `__init__` | method | `micro/stt-training/stt_training/features.py:73` | `def __init__(self, freq_mask_param, time_mask_param, n_freq_masks, n_time_masks)` |
| `_fix_length` | method | `micro/stt-training/stt_training/features.py:50` | `def _fix_length(self, x)` |
| `forward` | method | `micro/stt-training/stt_training/features.py:58` | `def forward(self, waveform)` |
| `forward` | method | `micro/stt-training/stt_training/features.py:86` | `def forward(self, x)` |
| `ConvBNAct` | class | `micro/stt-training/stt_training/model.py:46` | `class ConvBNAct(Sequential)` |
| `InvertedResidual` | class | `micro/stt-training/stt_training/model.py:58` | `class InvertedResidual(Module)` |
| `WordCNN` | class | `micro/stt-training/stt_training/model.py:82` | `class WordCNN(Module)` |
| `__init__` | method | `micro/stt-training/stt_training/model.py:47` | `def __init__(self, in_c, out_c, kernel, stride, groups, act)` |
| `__init__` | method | `micro/stt-training/stt_training/model.py:61` | `def __init__(self, in_c, out_c, stride, expand_ratio)` |
| `__init__` | method | `micro/stt-training/stt_training/model.py:100` | `def __init__(self, num_classes, width_mult, dropout, stem_stride, pad_to_odd)` |
| `_init_weights` | method | `micro/stt-training/stt_training/model.py:146` | `def _init_weights(self)` |
| `_make_divisible` | function | `micro/stt-training/stt_training/model.py:19` | `def _make_divisible(v, divisor)` |
| `build_model` | method | `micro/stt-training/stt_training/model.py:167` | `def build_model(num_classes)` |
| `forward` | method | `micro/stt-training/stt_training/model.py:77` | `def forward(self, x)` |
| `forward` | method | `micro/stt-training/stt_training/model.py:157` | `def forward(self, x)` |
| `normalize_stride` | function | `micro/stt-training/stt_training/model.py:27` | `def normalize_stride(v)` |
| `build_argparser` | function | `micro/stt-training/stt_training/train.py:275` | `def build_argparser()` |
| `default_data_roots` | function | `micro/stt-training/stt_training/train.py:49` | `def default_data_roots(tts_dir, ps_dir)` |
| `evaluate` | function | `micro/stt-training/stt_training/train.py:60` | `def evaluate(model, feature_fn, loader, device)` |
| `lr_at` | function | `micro/stt-training/stt_training/train.py:193` | `def lr_at(step)` |
| `main` | function | `micro/stt-training/stt_training/train.py:317` | `def main()` |
| `train` | function | `micro/stt-training/stt_training/train.py:88` | `def train(args)` |
| `folder_for_word` | function | `micro/stt-training/stt_training/words.py:18` | `def folder_for_word(word)` |
| `load_words` | function | `micro/stt-training/stt_training/words.py:31` | `def load_words(path)` |
| `resolve_classes` | function | `micro/stt-training/stt_training/words.py:53` | `def resolve_classes(path, include_unknown)` |
| `download_musan_noise` | function | `micro/stt-training/tools/download_musan_rirs.py:37` | `def download_musan_noise(out_dir, small, seed)` |
| `download_rirs` | function | `micro/stt-training/tools/download_musan_rirs.py:67` | `def download_rirs(out_dir, max_files, seed)` |
| `main` | function | `micro/stt-training/tools/download_musan_rirs.py:94` | `def main()` |
| `AlignedWord` | class | `micro/stt-training/tools/extract_clips.py:46` | `class AlignedWord` |
| `MMSAligner` | class | `micro/stt-training/tools/extract_clips.py:53` | `class MMSAligner` |
| `__init__` | method | `micro/stt-training/tools/extract_clips.py:56` | `def __init__(self, device, with_star)` |
| `_cut_natural_clip` | method | `micro/stt-training/tools/extract_clips.py:116` | `def _cut_natural_clip(audio, start_s, end_s)` |
| `_ids` | method | `micro/stt-training/tools/extract_clips.py:71` | `def _ids(self, word)` |
| `_load_rows` | method | `micro/stt-training/tools/extract_clips.py:156` | `def _load_rows(path)` |
| `_resolve_device` | method | `micro/stt-training/tools/extract_clips.py:144` | `def _resolve_device(choice)` |
| `_safe` | method | `micro/stt-training/tools/extract_clips.py:167` | `def _safe(s)` |
| `align` | method | `micro/stt-training/tools/extract_clips.py:74` | `def align(self, audio_1d, words)` |
| `emit` | method | `micro/stt-training/tools/extract_clips.py:212` | `def emit(label, clip_id, char_start, speaker, clip, sample_rate)` |
| `main` | method | `micro/stt-training/tools/extract_clips.py:171` | `def main()` |
| `_ShardReader` | class | `micro/stt-training/tools/mine_peoples_speech.py:80` | `class _ShardReader` |
| `__init__` | method | `micro/stt-training/tools/mine_peoples_speech.py:90` | `def __init__(self, shard, max_attempts)` |
| `_fetch` | method | `micro/stt-training/tools/mine_peoples_speech.py:157` | `def _fetch(_rg, _i)` |
| `_load_seen_keys` | method | `micro/stt-training/tools/mine_peoples_speech.py:231` | `def _load_seen_keys(path)` |
| `_new_fs` | function | `micro/stt-training/tools/mine_peoples_speech.py:69` | `def _new_fs()` |
| `_open` | method | `micro/stt-training/tools/mine_peoples_speech.py:98` | `def _open(self)` |
| `_safe_name` | method | `micro/stt-training/tools/mine_peoples_speech.py:207` | `def _safe_name(clip_id)` |
| `_shard_paths` | function | `micro/stt-training/tools/mine_peoples_speech.py:75` | `def _shard_paths(config, split)` |
| `_tokens_with_pos` | method | `micro/stt-training/tools/mine_peoples_speech.py:187` | `def _tokens_with_pos(text)` |
| `find_matches` | method | `micro/stt-training/tools/mine_peoples_speech.py:191` | `def find_matches(text, targets)` |
| `iter_peoples_speech` | method | `micro/stt-training/tools/mine_peoples_speech.py:131` | `def iter_peoples_speech(config, split, offset, limit)` |
| `main` | method | `micro/stt-training/tools/mine_peoples_speech.py:247` | `def main()` |
| `num_row_groups` | method | `micro/stt-training/tools/mine_peoples_speech.py:103` | `def num_row_groups(self)` |
| `read_columns` | method | `micro/stt-training/tools/mine_peoples_speech.py:109` | `def read_columns(self, rg, columns)` |
| `row_group_num_rows` | method | `micro/stt-training/tools/mine_peoples_speech.py:106` | `def row_group_num_rows(self, rg)` |
| `save_audio_16k` | method | `micro/stt-training/tools/mine_peoples_speech.py:211` | `def save_audio_16k(fetch, out_path)` |
| `_resample_to_16k` | function | `micro/stt-training/tools/synthesize.py:76` | `def _resample_to_16k(samples, sr)` |
| `discover_voices` | function | `micro/stt-training/tools/synthesize.py:58` | `def discover_voices(language)` |
| `main` | function | `micro/stt-training/tools/synthesize.py:85` | `def main()` |
| `Argmax` | function | `micro/stt/include/stt/stt.h:90` | `int Argmax(const float* logits, int n_logits);` |
| `Classifier` | class | `micro/stt/include/stt/stt.h:40` | `` |
| `Impl` | struct | `micro/stt/include/stt/stt.h:74` | `` |
| `Run` | function | `micro/stt/include/stt/stt.h:60` | `void Run(const float* features, float* logits_out) const;` |
| `STT_STT_H_` | macro | `micro/stt/include/stt/stt.h:19` | `#define STT_STT_H_` |
| `SoftmaxProb` | function | `micro/stt/include/stt/stt.h:93` | `float SoftmaxProb(const float* logits, int n_logits, int index);` |
| `TensorQuant` | struct | `micro/stt/include/stt/stt.h:35` | `` |
| `arena_used_bytes` | function | `micro/stt/include/stt/stt.h:71` | `std::size_t arena_used_bytes() const` |
| `feature_scratch` | function | `micro/stt/include/stt/stt.h:65` | `float* feature_scratch() const` |
| `input_count` | function | `micro/stt/include/stt/stt.h:70` | `std::size_t input_count() const` |
| `input_quant` | function | `micro/stt/include/stt/stt.h:67` | `TensorQuant input_quant() const` |
| `n_classes` | function | `micro/stt/include/stt/stt.h:69` | `int n_classes() const` |
| `output_quant` | function | `micro/stt/include/stt/stt.h:68` | `TensorQuant output_quant() const` |
| `_int16_roundtrip` | function | `micro/stt/scripts/desktop_parity.py:76` | `def _int16_roundtrip(samples)` |
| `_parse_device_log` | function | `micro/stt/scripts/desktop_parity.py:98` | `def _parse_device_log(path)` |
| `_resolve_meta` | function | `micro/stt/scripts/desktop_parity.py:60` | `def _resolve_meta(tflite)` |
| `_softmax_prob` | function | `micro/stt/scripts/desktop_parity.py:92` | `def _softmax_prob(logits, idx)` |
| `main` | function | `micro/stt/scripts/desktop_parity.py:111` | `def main(argv)` |
| `_f32` | function | `micro/stt/scripts/generate_embedded_data.py:160` | `def _f32(x)` |
| `_format_byte_array` | function | `micro/stt/scripts/generate_embedded_data.py:142` | `def _format_byte_array(data, width)` |
| `_format_float32_array` | function | `micro/stt/scripts/generate_embedded_data.py:171` | `def _format_float32_array(vals, width)` |
| `_format_int16_array` | function | `micro/stt/scripts/generate_embedded_data.py:151` | `def _format_int16_array(samples, width)` |
| `_format_plain_int_array` | function | `micro/stt/scripts/generate_embedded_data.py:180` | `def _format_plain_int_array(vals, width)` |
| `_fp32_to_int16_pcm` | function | `micro/stt/scripts/generate_embedded_data.py:189` | `def _fp32_to_int16_pcm(samples)` |
| `_include_guard` | function | `micro/stt/scripts/generate_embedded_data.py:63` | `def _include_guard(stem)` |
| `_is_riff_wav` | function | `micro/stt/scripts/generate_embedded_data.py:207` | `def _is_riff_wav(path)` |
| `_load_clip` | function | `micro/stt/scripts/generate_embedded_data.py:216` | `def _load_clip(path, sample_rate, n_samples)` |
| `_load_meta` | function | `micro/stt/scripts/generate_embedded_data.py:103` | `def _load_meta(tflite)` |
| `_meta_sidecar` | function | `micro/stt/scripts/generate_embedded_data.py:90` | `def _meta_sidecar(tflite)` |
| `_pick_clips` | function | `micro/stt/scripts/generate_embedded_data.py:586` | `def _pick_clips(wavs_roots, classes, clips_per_class, max_classes)` |
| `_pick_clips_hub` | function | `micro/stt/scripts/generate_embedded_data.py:617` | `def _pick_clips_hub(repo_id, configs, classes, clips_per_class, max_classes, sample_rate, n_samples, cache_dir)` |
| `_resolve_int8_mel_tflite` | function | `micro/stt/scripts/generate_embedded_data.py:68` | `def _resolve_int8_mel_tflite(explicit)` |
| `_write_audio_config_file` | function | `micro/stt/scripts/generate_embedded_data.py:268` | `def _write_audio_config_file(out_dir)` |
| `_write_classes_files` | function | `micro/stt/scripts/generate_embedded_data.py:465` | `def _write_classes_files(out_dir, classes)` |
| `_write_clips_files` | function | `micro/stt/scripts/generate_embedded_data.py:501` | `def _write_clips_files(out_dir, decoded, sample_rate, n_samples)` |
| `_write_mel_tables_file` | function | `micro/stt/scripts/generate_embedded_data.py:327` | `def _write_mel_tables_file(out_dir)` |
| `_write_model_files` | function | `micro/stt/scripts/generate_embedded_data.py:228` | `def _write_model_files(out_dir, tflite)` |
| `main` | function | `micro/stt/scripts/generate_embedded_data.py:680` | `def main(argv)` |
| `Classifier` | function | `micro/stt/src/classifier.cc:53` | `Classifier::Classifier(const unsigned char* model_data,                        unsigned int /*mod...` |
| `Run` | function | `micro/stt/src/classifier.cc:226` | `void Classifier::Run(const float* features, float* logits_out) const` |
| `Saturate8` | function | `micro/stt/src/classifier.cc:26` | `inline int8_t Saturate8(float v)` |
| `Argmax` | function | `micro/stt/src/predictor.cc:7` | `int Argmax(const float* logits, int n_logits)` |
| `SoftmaxProb` | function | `micro/stt/src/predictor.cc:20` | `float SoftmaxProb(const float* logits, int n_logits, int index)` |
| `TF_LITE_MICRO_TEST` | function | `micro/stt/tests/predictor_test.cc:14` | `TF_LITE_MICRO_TESTS_BEGIN  TF_LITE_MICRO_TEST(ArgmaxPicksLargest)` |
| `TF_LITE_MICRO_TEST` | function | `micro/stt/tests/predictor_test.cc:19` | `TF_LITE_MICRO_TEST(ArgmaxTiesGoToLowestIndex)` |
| `TF_LITE_MICRO_TEST` | function | `micro/stt/tests/predictor_test.cc:24` | `TF_LITE_MICRO_TEST(SoftmaxProbsSumToOne)` |
| `TF_LITE_MICRO_TEST` | function | `micro/stt/tests/predictor_test.cc:31` | `TF_LITE_MICRO_TEST(SoftmaxProbMatchesHandComputed)` |
| `TF_LITE_MICRO_TEST` | function | `micro/stt/tests/predictor_test.cc:37` | `TF_LITE_MICRO_TEST(SoftmaxStableOnLargeLogits)` |
| `InitializeTarget` | function | `micro/test-support/host/tflm_host_stub.cc:46` | `void InitializeTarget()` |
| `MicroPrintf` | function | `micro/test-support/host/tflm_host_stub.cc:19` | `void MicroPrintf(const char* format, ...)` |
| `MicroSnprintf` | function | `micro/test-support/host/tflm_host_stub.cc:32` | `int MicroSnprintf(char* buffer, size_t buf_size, const char* format, ...)` |
| `MicroVsnprintf` | function | `micro/test-support/host/tflm_host_stub.cc:40` | `int MicroVsnprintf(char* buffer, size_t buf_size, const char* format,                    va_list ...` |
| `VMicroPrintf` | function | `micro/test-support/host/tflm_host_stub.cc:27` | `void VMicroPrintf(const char* format, va_list args)` |
| `EnergyCentroidIndex` | function | `micro/vad/include/vad/vad.h:145` | `std::size_t EnergyCentroidIndex(const int16_t* buf, std::size_t start, std::size_t end);` |
| `ExtractClipFrontAligned` | function | `micro/vad/include/vad/vad.h:135` | `void ExtractClipFrontAligned(const float* src, std::size_t src_len, std::size_t start, std::size_t end, float* out...` |
| `Impl` | struct | `micro/vad/include/vad/vad.h:72` | `` |
| `Predict` | function | `micro/vad/include/vad/vad.h:60` | `float Predict(const float* features) const;` |
| `Start` | function | `micro/vad/include/vad/vad.h:103` | `void Start();` |
| `VAD_VAD_H_` | macro | `micro/vad/include/vad/vad.h:23` | `#define VAD_VAD_H_` |
| `Vad` | class | `micro/vad/include/vad/vad.h:43` | `` |
| `VadEvent` | enum | `micro/vad/include/vad/vad.h:85` | `` |
| `VadEvent` | class | `micro/vad/include/vad/vad.h:85` | `` |
| `VadSegmenter` | class | `micro/vad/include/vad/vad.h:96` | `` |
| `VadTensorQuant` | struct | `micro/vad/include/vad/vad.h:38` | `` |
| `arena_used_bytes` | function | `micro/vad/include/vad/vad.h:69` | `std::size_t arena_used_bytes() const` |
| `feature_scratch` | function | `micro/vad/include/vad/vad.h:64` | `float* feature_scratch() const` |
| `input_count` | function | `micro/vad/include/vad/vad.h:68` | `std::size_t input_count() const` |
| `input_quant` | function | `micro/vad/include/vad/vad.h:66` | `VadTensorQuant input_quant() const` |
| `output_quant` | function | `micro/vad/include/vad/vad.h:67` | `VadTensorQuant output_quant() const` |
| `samples_processed` | function | `micro/vad/include/vad/vad.h:115` | `std::size_t samples_processed() const` |
| `segment_end_sample` | function | `micro/vad/include/vad/vad.h:114` | `std::size_t segment_end_sample() const` |
| `segment_start_sample` | function | `micro/vad/include/vad/vad.h:113` | `std::size_t segment_start_sample() const` |
| `_auto_tflite` | function | `micro/vad/scripts/generate_vad_embedded_data.py:224` | `def _auto_tflite()` |
| `_smooth_window_frames` | function | `micro/vad/scripts/generate_vad_embedded_data.py:66` | `def _smooth_window_frames()` |
| `_write_vad_config` | function | `micro/vad/scripts/generate_vad_embedded_data.py:72` | `def _write_vad_config(out_dir)` |
| `_write_vad_mel_tables` | function | `micro/vad/scripts/generate_vad_embedded_data.py:117` | `def _write_vad_mel_tables(out_dir)` |
| `_write_vad_model` | function | `micro/vad/scripts/generate_vad_embedded_data.py:190` | `def _write_vad_model(out_dir, tflite)` |
| `main` | function | `micro/vad/scripts/generate_vad_embedded_data.py:229` | `def main(argv)` |
| `Predict` | function | `micro/vad/src/vad.cc:171` | `float Vad::Predict(const float* features) const` |
| `Saturate8` | function | `micro/vad/src/vad.cc:22` | `inline int8_t Saturate8(float v)` |
| `Vad` | function | `micro/vad/src/vad.cc:38` | `Vad::Vad(const unsigned char* model_data, unsigned int /*model_size*/,          uint8_t* tensor_a...` |
| `EnergyCentroidIndex` | function | `micro/vad/src/vad_segmenter.cc:106` | `std::size_t EnergyCentroidIndex(const int16_t* buf, std::size_t start,                           ...` |
| `ExtractClipFrontAligned` | function | `micro/vad/src/vad_segmenter.cc:93` | `void ExtractClipFrontAligned(const float* src, std::size_t src_len,                              ...` |
| `Finish` | function | `micro/vad/src/vad_segmenter.cc:84` | `VadEvent VadSegmenter::Finish()` |
| `ProcessFrame` | function | `micro/vad/src/vad_segmenter.cc:32` | `VadEvent VadSegmenter::ProcessFrame(float raw_probability)` |
| `Start` | function | `micro/vad/src/vad_segmenter.cc:22` | `void VadSegmenter::Start()` |
| `VadSegmenter` | function | `micro/vad/src/vad_segmenter.cc:6` | `VadSegmenter::VadSegmenter(float threshold, int window_frames, int hop,                          ...` |
| `Concat` | function | `micro/vad/tests/vad_segmenter_test.cc:22` | `std::vector<float> Concat(std::initializer_list<std::vector<float>> parts)` |
| `Repeat` | function | `micro/vad/tests/vad_segmenter_test.cc:20` | `std::vector<float> Repeat(float v, int n)` |
| `TF_LITE_MICRO_TEST` | function | `micro/vad/tests/vad_segmenter_test.cc:50` | `TF_LITE_MICRO_TESTS_BEGIN  TF_LITE_MICRO_TEST(SingleSegmentDetected)` |
| `TF_LITE_MICRO_TEST` | function | `micro/vad/tests/vad_segmenter_test.cc:60` | `TF_LITE_MICRO_TEST(TwoSegmentsDetected)` |
| `TF_LITE_MICRO_TEST` | function | `micro/vad/tests/vad_segmenter_test.cc:68` | `TF_LITE_MICRO_TEST(TrailingSegmentFlushed)` |
| `TF_LITE_MICRO_TEST` | function | `micro/vad/tests/vad_segmenter_test.cc:75` | `TF_LITE_MICRO_TEST(NoLookBehindStartsLater)` |
| `TF_LITE_MICRO_TEST` | function | `micro/vad/tests/vad_segmenter_test.cc:86` | `TF_LITE_MICRO_TEST(ExtractClipFrontAlignedZeroPads)` |
| `TF_LITE_MICRO_TEST` | function | `micro/vad/tests/vad_segmenter_test.cc:96` | `TF_LITE_MICRO_TEST(EnergyCentroidIndexWeightsByPower)` |
| `BinaryDistribution` | class | `python/setup.py:9` | `class BinaryDistribution(Distribution)` |
| `PlatformWheel` | class | `python/setup.py:14` | `class PlatformWheel(bdist_wheel)` |
| `finalize_options` | method | `python/setup.py:15` | `def finalize_options(self)` |
| `get_tag` | method | `python/setup.py:20` | `def get_tag(self)` |
| `has_ext_modules` | method | `python/setup.py:10` | `def has_ext_modules(self)` |
| `read_license` | method | `python/setup.py:32` | `def read_license()` |
| `read_readme` | method | `python/setup.py:26` | `def read_readme()` |
| `read_requirements` | method | `python/setup.py:39` | `def read_requirements()` |
| `__getattr__` | function | `python/src/moonshine_voice/__init__.py:81` | `def __getattr__(name)` |
| `AlphanumericEvent` | class | `python/src/moonshine_voice/alphanumeric_listener.py:49` | `class AlphanumericEvent` |
| `AlphanumericEventType` | class | `python/src/moonshine_voice/alphanumeric_listener.py:40` | `class AlphanumericEventType(Enum)` |
| `AlphanumericListener` | class | `python/src/moonshine_voice/alphanumeric_listener.py:738` | `class AlphanumericListener` |
| `AlphanumericMatch` | class | `python/src/moonshine_voice/alphanumeric_listener.py:69` | `class AlphanumericMatch` |
| `AlphanumericMatcher` | class | `python/src/moonshine_voice/alphanumeric_listener.py:512` | `class AlphanumericMatcher` |
| `__call__` | method | `python/src/moonshine_voice/alphanumeric_listener.py:829` | `def __call__(self, event)` |
| `__init__` | method | `python/src/moonshine_voice/alphanumeric_listener.py:542` | `def __init__(self)` |
| `__init__` | method | `python/src/moonshine_voice/alphanumeric_listener.py:808` | `def __init__(self, callback)` |
| `_build_lookup` | method | `python/src/moonshine_voice/alphanumeric_listener.py:370` | `def _build_lookup()` |
| `_char_accepted` | method | `python/src/moonshine_voice/alphanumeric_listener.py:705` | `def _char_accepted(self, char)` |
| `_normalize` | method | `python/src/moonshine_voice/alphanumeric_listener.py:355` | `def _normalize(text)` |
| `_parse_number_words` | method | `python/src/moonshine_voice/alphanumeric_listener.py:424` | `def _parse_number_words(text)` |
| `_play_error_feedback` | method | `python/src/moonshine_voice/alphanumeric_listener.py:957` | `def _play_error_feedback(self)` |
| `_process_utterance` | method | `python/src/moonshine_voice/alphanumeric_listener.py:879` | `def _process_utterance(self, line)` |
| `_resolve` | method | `python/src/moonshine_voice/alphanumeric_listener.py:637` | `def _resolve(self, text)` |
| `_resolve_spelled_letter` | method | `python/src/moonshine_voice/alphanumeric_listener.py:652` | `def _resolve_spelled_letter(self, text)` |
| `_speak_character` | method | `python/src/moonshine_voice/alphanumeric_listener.py:941` | `def _speak_character(self, char)` |
| `classify` | method | `python/src/moonshine_voice/alphanumeric_listener.py:570` | `def classify(self, raw_text)` |
| `classify_sequence` | method | `python/src/moonshine_voice/alphanumeric_listener.py:606` | `def classify_sequence(self, raw_text)` |
| `clear` | method | `python/src/moonshine_voice/alphanumeric_listener.py:854` | `def clear(self)` |
| `digits_only_matcher` | method | `python/src/moonshine_voice/alphanumeric_listener.py:720` | `def digits_only_matcher()` |
| `is_character` | method | `python/src/moonshine_voice/alphanumeric_listener.py:80` | `def is_character(self)` |
| `is_recognized` | method | `python/src/moonshine_voice/alphanumeric_listener.py:88` | `def is_recognized(self)` |
| `is_terminator` | method | `python/src/moonshine_voice/alphanumeric_listener.py:84` | `def is_terminator(self)` |
| `letters_only_matcher` | method | `python/src/moonshine_voice/alphanumeric_listener.py:716` | `def letters_only_matcher()` |
| `matcher` | method | `python/src/moonshine_voice/alphanumeric_listener.py:850` | `def matcher(self)` |
| `on_event` | method | `python/src/moonshine_voice/alphanumeric_listener.py:1063` | `def on_event(event)` |
| `spoken_form` | method | `python/src/moonshine_voice/alphanumeric_listener.py:306` | `def spoken_form(char)` |
| `stopped` | method | `python/src/moonshine_voice/alphanumeric_listener.py:845` | `def stopped(self)` |
| `text` | method | `python/src/moonshine_voice/alphanumeric_listener.py:840` | `def text(self)` |
| `undo` | method | `python/src/moonshine_voice/alphanumeric_listener.py:865` | `def undo(self)` |
| `CachedEmbeddings` | class | `python/src/moonshine_voice/cached_embeddings.py:68` | `class CachedEmbeddings` |
| `_EmbeddingBackend` | class | `python/src/moonshine_voice/cached_embeddings.py:45` | `class _EmbeddingBackend(Protocol)` |
| `__contains__` | method | `python/src/moonshine_voice/cached_embeddings.py:170` | `def __contains__(self, sentence)` |
| `__init__` | method | `python/src/moonshine_voice/cached_embeddings.py:95` | `def __init__(self)` |
| `__len__` | method | `python/src/moonshine_voice/cached_embeddings.py:167` | `def __len__(self)` |
| `_load` | method | `python/src/moonshine_voice/cached_embeddings.py:218` | `def _load(self, path)` |
| `_normalize` | method | `python/src/moonshine_voice/cached_embeddings.py:245` | `def _normalize(s)` |
| `_parse_meta` | method | `python/src/moonshine_voice/cached_embeddings.py:238` | `def _parse_meta(self, s)` |
| `active` | method | `python/src/moonshine_voice/cached_embeddings.py:150` | `def active(self)` |
| `calculate_embedding` | method | `python/src/moonshine_voice/cached_embeddings.py:52` | `def calculate_embedding(self, sentence)` |
| `calculate_embedding` | method | `python/src/moonshine_voice/cached_embeddings.py:179` | `def calculate_embedding(self, sentence)` |
| `default_cached_embeddings_path` | method | `python/src/moonshine_voice/cached_embeddings.py:62` | `def default_cached_embeddings_path()` |
| `distance` | method | `python/src/moonshine_voice/cached_embeddings.py:54` | `def distance(self, embedding_a, embedding_b)` |
| `distance` | method | `python/src/moonshine_voice/cached_embeddings.py:195` | `def distance(self, embedding_a, embedding_b)` |
| `get` | method | `python/src/moonshine_voice/cached_embeddings.py:175` | `def get(self, sentence)` |
| `metadata` | method | `python/src/moonshine_voice/cached_embeddings.py:159` | `def metadata(self)` |
| `path` | method | `python/src/moonshine_voice/cached_embeddings.py:155` | `def path(self)` |
| `phrases` | method | `python/src/moonshine_voice/cached_embeddings.py:163` | `def phrases(self)` |
| `write_cached_embeddings_tsv` | method | `python/src/moonshine_voice/cached_embeddings.py:260` | `def write_cached_embeddings_tsv(path, entries)` |
| `_package_version` | function | `python/src/moonshine_voice/cli.py:50` | `def _package_version()` |
| `_usage` | function | `python/src/moonshine_voice/cli.py:68` | `def _usage()` |
| `main` | function | `python/src/moonshine_voice/cli.py:91` | `def main(argv)` |
| `Ask` | class | `python/src/moonshine_voice/dialog_flow.py:110` | `class Ask(Prompt)` |
| `Choose` | class | `python/src/moonshine_voice/dialog_flow.py:166` | `class Choose(Prompt)` |
| `Confirm` | class | `python/src/moonshine_voice/dialog_flow.py:147` | `class Confirm(Prompt)` |
| `Dialog` | class | `python/src/moonshine_voice/dialog_flow.py:335` | `class Dialog` |
| `DialogCancelled` | class | `python/src/moonshine_voice/dialog_flow.py:191` | `class DialogCancelled(DialogError)` |
| `DialogError` | class | `python/src/moonshine_voice/dialog_flow.py:187` | `class DialogError(Exception)` |
| `DialogFlow` | class | `python/src/moonshine_voice/dialog_flow.py:453` | `class DialogFlow(TranscriptEventListener)` |
| `DialogRestart` | class | `python/src/moonshine_voice/dialog_flow.py:195` | `class DialogRestart(DialogError)` |
| `EmbeddingBackend` | class | `python/src/moonshine_voice/dialog_flow.py:212` | `class EmbeddingBackend(Protocol)` |
| `NoInputError` | class | `python/src/moonshine_voice/dialog_flow.py:199` | `class NoInputError(DialogError)` |
| `NoMatchError` | class | `python/src/moonshine_voice/dialog_flow.py:203` | `class NoMatchError(DialogError)` |
| `PhraseMatcher` | class | `python/src/moonshine_voice/dialog_flow.py:229` | `class PhraseMatcher` |
| `Prompt` | class | `python/src/moonshine_voice/dialog_flow.py:97` | `class Prompt` |
| `Say` | class | `python/src/moonshine_voice/dialog_flow.py:102` | `class Say(Prompt)` |
| `_AbandonPrompt` | class | `python/src/moonshine_voice/dialog_flow.py:1624` | `class _AbandonPrompt(Exception)` |
| `_ActiveFlow` | class | `python/src/moonshine_voice/dialog_flow.py:440` | `class _ActiveFlow` |
| `_AlphaSession` | class | `python/src/moonshine_voice/dialog_flow.py:432` | `class _AlphaSession` |
| `_CompletedLinePrinter` | class | `python/src/moonshine_voice/dialog_flow.py:2097` | `class _CompletedLinePrinter(TranscriptEventListener)` |
| `_PartialInput` | class | `python/src/moonshine_voice/dialog_flow.py:1629` | `class _PartialInput(Exception)` |
| `_Reprompt` | class | `python/src/moonshine_voice/dialog_flow.py:1619` | `class _Reprompt(Exception)` |
| `_SpelledPhrase` | class | `python/src/moonshine_voice/dialog_flow.py:1635` | `class _SpelledPhrase(str)` |
| `__init__` | method | `python/src/moonshine_voice/dialog_flow.py:255` | `def __init__(self, backend, phrases_by_key)` |
| `__init__` | method | `python/src/moonshine_voice/dialog_flow.py:345` | `def __init__(self, trigger_phrase)` |
| `__init__` | method | `python/src/moonshine_voice/dialog_flow.py:435` | `def __init__(self, matcher)` |
| `__init__` | method | `python/src/moonshine_voice/dialog_flow.py:443` | `def __init__(self, flow_fn, trigger_phrase)` |
| `__init__` | method | `python/src/moonshine_voice/dialog_flow.py:558` | `def __init__(self)` |
| `__init__` | method | `python/src/moonshine_voice/dialog_flow.py:1620` | `def __init__(self, text)` |
| `__init__` | method | `python/src/moonshine_voice/dialog_flow.py:1625` | `def __init__(self, exc)` |
| `__iter__` | method | `python/src/moonshine_voice/dialog_flow.py:1650` | `def __iter__(self)` |
| `_advance` | method | `python/src/moonshine_voice/dialog_flow.py:991` | `def _advance(self, active, value)` |
| `_alpha_session_for` | method | `python/src/moonshine_voice/dialog_flow.py:1118` | `def _alpha_session_for(self, prompt)` |
| `_build_matcher` | method | `python/src/moonshine_voice/dialog_flow.py:1407` | `def _build_matcher(self, phrases_by_key, threshold)` |
| `_default_factory` | method | `python/src/moonshine_voice/dialog_flow.py:633` | `def _default_factory(phrases_by_key, threshold)` |
| `_deliver_to_active` | method | `python/src/moonshine_voice/dialog_flow.py:944` | `def _deliver_to_active(self, active, utterance)` |
| `_finish_flow` | method | `python/src/moonshine_voice/dialog_flow.py:1146` | `def _finish_flow(self, active)` |
| `_get_choose_matcher` | method | `python/src/moonshine_voice/dialog_flow.py:1388` | `def _get_choose_matcher(self, prompt)` |
| `_get_confirm_matcher` | method | `python/src/moonshine_voice/dialog_flow.py:1372` | `def _get_confirm_matcher(self, prompt)` |
| `_get_digits_matcher` | method | `python/src/moonshine_voice/dialog_flow.py:1132` | `def _get_digits_matcher(self)` |
| `_get_spelled_matcher` | method | `python/src/moonshine_voice/dialog_flow.py:1127` | `def _get_spelled_matcher(self)` |
| `_get_trigger_matcher` | method | `python/src/moonshine_voice/dialog_flow.py:910` | `def _get_trigger_matcher(self)` |
| `_interpret_alphanumeric` | method | `python/src/moonshine_voice/dialog_flow.py:1259` | `def _interpret_alphanumeric(self, prompt, utterance, active)` |
| `_interpret_answer` | method | `python/src/moonshine_voice/dialog_flow.py:1236` | `def _interpret_answer(self, prompt, utterance, active)` |
| `_interpret_ask` | method | `python/src/moonshine_voice/dialog_flow.py:1247` | `def _interpret_ask(self, prompt, utterance, active)` |
| `_interpret_choose` | method | `python/src/moonshine_voice/dialog_flow.py:1355` | `def _interpret_choose(self, prompt, utterance, active)` |
| `_interpret_confirm` | method | `python/src/moonshine_voice/dialog_flow.py:1338` | `def _interpret_confirm(self, prompt, utterance, active)` |
| `_invalidate_trigger_matcher` | method | `python/src/moonshine_voice/dialog_flow.py:691` | `def _invalidate_trigger_matcher(self)` |
| `_invoke_global` | method | `python/src/moonshine_voice/dialog_flow.py:1199` | `def _invoke_global(self, trigger_phrase)` |
| `_log` | method | `python/src/moonshine_voice/dialog_flow.py:1589` | `def _log(self, msg)` |
| `_match_trigger` | method | `python/src/moonshine_voice/dialog_flow.py:888` | `def _match_trigger(self, utterance)` |
| `_play_beep` | method | `python/src/moonshine_voice/dialog_flow.py:1504` | `def _play_beep(self, kind)` |
| `_play_error_beep` | method | `python/src/moonshine_voice/dialog_flow.py:1560` | `def _play_error_beep(self)` |
| `_play_success_beep` | method | `python/src/moonshine_voice/dialog_flow.py:1551` | `def _play_success_beep(self)` |
| `_reprompt_or_abandon` | method | `python/src/moonshine_voice/dialog_flow.py:1424` | `def _reprompt_or_abandon(self, prompt, active, exc)` |
| `_restart_flow` | method | `python/src/moonshine_voice/dialog_flow.py:1137` | `def _restart_flow(self, active)` |
| `_run_beep_diagnostic` | method | `python/src/moonshine_voice/dialog_flow.py:1704` | `def _run_beep_diagnostic()` |
| `_set_spelling_mode` | method | `python/src/moonshine_voice/dialog_flow.py:1091` | `def _set_spelling_mode(self, active)` |
| `_should_short_circuit_to_alpha` | method | `python/src/moonshine_voice/dialog_flow.py:870` | `def _should_short_circuit_to_alpha(self, active, utterance)` |
| `_speak` | method | `python/src/moonshine_voice/dialog_flow.py:1440` | `def _speak(self, text)` |
| `_speak_character_feedback` | method | `python/src/moonshine_voice/dialog_flow.py:1485` | `def _speak_character_feedback(self, character)` |
| `_speak_undo_feedback` | method | `python/src/moonshine_voice/dialog_flow.py:1569` | `def _speak_undo_feedback(self, character)` |
| `_spelling_mode_for_prompt` | method | `python/src/moonshine_voice/dialog_flow.py:1114` | `def _spelling_mode_for_prompt(self, prompt)` |
| `_start_flow` | method | `python/src/moonshine_voice/dialog_flow.py:934` | `def _start_flow(self, trigger_phrase)` |
| `_summarise` | method | `python/src/moonshine_voice/dialog_flow.py:1684` | `def _summarise(text, max_len)` |
| `_throw` | method | `python/src/moonshine_voice/dialog_flow.py:1055` | `def _throw(self, active, exc)` |
| `active_trigger` | method | `python/src/moonshine_voice/dialog_flow.py:702` | `def active_trigger(self)` |
| `ask` | method | `python/src/moonshine_voice/dialog_flow.py:354` | `def ask(self, prompt)` |
| `calculate_embedding` | method | `python/src/moonshine_voice/dialog_flow.py:222` | `def calculate_embedding(self, sentence)` |
| `cancel` | method | `python/src/moonshine_voice/dialog_flow.py:402` | `def cancel(self)` |
| `cancel_active` | method | `python/src/moonshine_voice/dialog_flow.py:1156` | `def cancel_active(self)` |
| `choose` | method | `python/src/moonshine_voice/dialog_flow.py:384` | `def choose(self, prompt, options)` |
| `confirm` | method | `python/src/moonshine_voice/dialog_flow.py:374` | `def confirm(self, prompt)` |
| `distance` | method | `python/src/moonshine_voice/dialog_flow.py:224` | `def distance(self, embedding_a, embedding_b)` |
| `is_active` | method | `python/src/moonshine_voice/dialog_flow.py:697` | `def is_active(self)` |
| `match` | method | `python/src/moonshine_voice/dialog_flow.py:285` | `def match(self, utterance)` |
| `match_with_score` | method | `python/src/moonshine_voice/dialog_flow.py:290` | `def match_with_score(self, utterance)` |
| `mute` | method | `python/src/moonshine_voice/dialog_flow.py:2069` | `def mute(should_mute)` |
| `on_error` | method | `python/src/moonshine_voice/dialog_flow.py:772` | `def on_error(self, event)` |
| `on_line_completed` | method | `python/src/moonshine_voice/dialog_flow.py:746` | `def on_line_completed(self, event)` |
| `on_line_completed` | method | `python/src/moonshine_voice/dialog_flow.py:2105` | `def on_line_completed(self, event)` |
| `on_line_started` | method | `python/src/moonshine_voice/dialog_flow.py:712` | `def on_line_started(self, event)` |
| `process_utterance` | method | `python/src/moonshine_voice/dialog_flow.py:777` | `def process_utterance(self, utterance)` |
| `register_flow` | method | `python/src/moonshine_voice/dialog_flow.py:662` | `def register_flow(self, trigger_phrase, flow)` |
| `register_global` | method | `python/src/moonshine_voice/dialog_flow.py:680` | `def register_global(self, trigger_phrase, handler)` |
| `registered_flows` | method | `python/src/moonshine_voice/dialog_flow.py:707` | `def registered_flows(self)` |
| `replay_last_prompt` | method | `python/src/moonshine_voice/dialog_flow.py:408` | `def replay_last_prompt(self)` |
| `restart` | method | `python/src/moonshine_voice/dialog_flow.py:405` | `def restart(self)` |
| `say` | method | `python/src/moonshine_voice/dialog_flow.py:350` | `def say(self, text)` |
| `say` | method | `python/src/moonshine_voice/dialog_flow.py:1169` | `def say(self, text)` |
| `set_spelling_mode` | method | `python/src/moonshine_voice/dialog_flow.py:2073` | `def set_spelling_mode(active)` |
| `speak` | method | `python/src/moonshine_voice/dialog_flow.py:2081` | `def speak(text)` |
| `spell_out` | method | `python/src/moonshine_voice/dialog_flow.py:1656` | `def spell_out(s)` |
| `threshold` | method | `python/src/moonshine_voice/dialog_flow.py:282` | `def threshold(self)` |
| `unregister_flow` | method | `python/src/moonshine_voice/dialog_flow.py:674` | `def unregister_flow(self, trigger_phrase)` |
| `wifi_setup` | method | `python/src/moonshine_voice/dialog_flow.py:1980` | `def wifi_setup(d)` |
| `EmbeddingModelArch` | class | `python/src/moonshine_voice/download.py:29` | `class EmbeddingModelArch(IntEnum)` |
| `TtsVoiceEntry` | class | `python/src/moonshine_voice/download.py:549` | `class TtsVoiceEntry` |
| `TtsVoicesByAvailability` | class | `python/src/moonshine_voice/download.py:556` | `class TtsVoicesByAvailability(TypedDict)` |
| `_entries_to_present_and_downloadable` | method | `python/src/moonshine_voice/download.py:563` | `def _entries_to_present_and_downloadable(entries)` |
| `_merge_tts_query_options` | method | `python/src/moonshine_voice/download.py:496` | `def _merge_tts_query_options(options)` |
| `_normalize_tts_language_tag_display` | method | `python/src/moonshine_voice/download.py:467` | `def _normalize_tts_language_tag_display(tag)` |
| `_normalize_tts_voice_stem` | method | `python/src/moonshine_voice/download.py:701` | `def _normalize_tts_voice_stem(stem)` |
| `_options_specify_asset_root` | method | `python/src/moonshine_voice/download.py:511` | `def _options_specify_asset_root(opts)` |
| `_spelling_language_key` | method | `python/src/moonshine_voice/download.py:339` | `def _spelling_language_key(language)` |
| `_spelling_model_root_path` | method | `python/src/moonshine_voice/download.py:358` | `def _spelling_model_root_path(language_key, cache_root)` |
| `_tts_asset_cache_root` | method | `python/src/moonshine_voice/download.py:485` | `def _tts_asset_cache_root(override)` |
| `_tts_voice_want_aliases` | method | `python/src/moonshine_voice/download.py:711` | `def _tts_voice_want_aliases(voice)` |
| `_tts_voices_json_to_catalog` | method | `python/src/moonshine_voice/download.py:569` | `def _tts_voices_json_to_catalog(raw)` |
| `_voice_query_options` | method | `python/src/moonshine_voice/download.py:522` | `def _voice_query_options(options)` |
| `cdn_url_for_tts_asset_key` | method | `python/src/moonshine_voice/download.py:850` | `def cdn_url_for_tts_asset_key(key)` |
| `dedupe_tts_language_tags_for_display` | method | `python/src/moonshine_voice/download.py:474` | `def dedupe_tts_language_tags_for_display(tags)` |
| `download_g2p_assets` | method | `python/src/moonshine_voice/download.py:953` | `def download_g2p_assets(language)` |
| `download_model_from_info` | method | `python/src/moonshine_voice/download.py:234` | `def download_model_from_info(model_info)` |
| `download_spelling_model_for_language` | method | `python/src/moonshine_voice/download.py:365` | `def download_spelling_model_for_language(language)` |
| `download_tts_assets` | method | `python/src/moonshine_voice/download.py:897` | `def download_tts_assets(language)` |
| `ensure_tts_voice_downloaded` | method | `python/src/moonshine_voice/download.py:799` | `def ensure_tts_voice_downloaded(language, voice, asset_root)` |
| `find_model_info` | method | `python/src/moonshine_voice/download.py:168` | `def find_model_info(language, model_arch)` |
| `get_components_for_model_info` | method | `python/src/moonshine_voice/download.py:207` | `def get_components_for_model_info(model_info)` |
| `get_embedding_model` | method | `python/src/moonshine_voice/download.py:276` | `def get_embedding_model(model_name, variant)` |
| `get_embedding_model_variants` | method | `python/src/moonshine_voice/download.py:266` | `def get_embedding_model_variants(model_name)` |
| `get_model_for_language` | method | `python/src/moonshine_voice/download.py:410` | `def get_model_for_language(wanted_language, wanted_model_arch)` |
| `get_spelling_model_path` | method | `python/src/moonshine_voice/download.py:395` | `def get_spelling_model_path(language)` |
| `get_tts_voice_catalog` | method | `python/src/moonshine_voice/download.py:611` | `def get_tts_voice_catalog()` |
| `is_downloadable_tts_asset_key` | method | `python/src/moonshine_voice/download.py:842` | `def is_downloadable_tts_asset_key(key)` |
| `list_g2p_dependency_keys` | method | `python/src/moonshine_voice/download.py:882` | `def list_g2p_dependency_keys(languages, options)` |
| `list_tts_dependency_keys` | method | `python/src/moonshine_voice/download.py:857` | `def list_tts_dependency_keys(languages)` |
| `list_tts_languages` | method | `python/src/moonshine_voice/download.py:588` | `def list_tts_languages()` |
| `list_tts_voices` | method | `python/src/moonshine_voice/download.py:634` | `def list_tts_voices(language)` |
| `log_model_info` | method | `python/src/moonshine_voice/download.py:438` | `def log_model_info(wanted_language, wanted_model_arch)` |
| `normalize_moonshine_language_tag` | method | `python/src/moonshine_voice/download.py:461` | `def normalize_moonshine_language_tag(language)` |
| `supported_embedding_models` | method | `python/src/moonshine_voice/download.py:254` | `def supported_embedding_models()` |
| `supported_embedding_models_friendly` | method | `python/src/moonshine_voice/download.py:259` | `def supported_embedding_models_friendly()` |
| `supported_languages` | method | `python/src/moonshine_voice/download.py:203` | `def supported_languages()` |
| `supported_languages_friendly` | method | `python/src/moonshine_voice/download.py:197` | `def supported_languages_friendly()` |
| `tts_asset_cache_path` | method | `python/src/moonshine_voice/download.py:491` | `def tts_asset_cache_path(cache_root)` |
| `validate_tts_language` | method | `python/src/moonshine_voice/download.py:673` | `def validate_tts_language(language)` |
| `validate_tts_voice_downloaded` | method | `python/src/moonshine_voice/download.py:728` | `def validate_tts_voice_downloaded(language, voice, asset_root)` |
| `validate_tts_voice_known` | method | `python/src/moonshine_voice/download.py:760` | `def validate_tts_voice_known(language, voice)` |
| `download_file` | function | `python/src/moonshine_voice/download_file.py:28` | `def download_file(url, dest, expected_sha256, resume, show_progress, timeout)` |
| `download_model` | function | `python/src/moonshine_voice/download_file.py:149` | `def download_model(url, filename, expected_sha256, app_name)` |
| `get_cache_dir` | function | `python/src/moonshine_voice/download_file.py:13` | `def get_cache_dir(app_name)` |

Next: [SYMBOLS_p11.md](SYMBOLS_p11.md)
