# API (page 5 of 10)
Previous: [API_p4.md](API_p4.md)

## core/moonshine-tts/src/zipvoice-custom-ops.cpp
Depends on: `core/moonshine-tts/src/zipvoice-custom-ops.h`
- `SoftplusPoly` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:52` `inline float SoftplusPoly(float z)`
- `ComputeTile` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:78` `void ComputeTile(void* user_data, size_t idx)`
- `SwooshKernel` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:96` `explicit SwooshKernel(bool is_left)
      : offset_(is_left ? kLeftOffset : kRightOffset),
      ...`
- `Compute` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:100` `void Compute(OrtKernelContext* context)`
- `SigmoidScalar` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:124` `inline float SigmoidScalar(float v)`
- `ComputeGluRow` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:132` `void ComputeGluRow(void* user_data, size_t r)`
- `Compute` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:147` `void Compute(OrtKernelContext* context)`
- `ComputeConvRow` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:184` `void ComputeConvRow(void* user_data, size_t row)`
- `Compute` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:205` `void Compute(OrtKernelContext* context)`
- `wpacked` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:230` `std::vector<float> wpacked(static_cast<size_t>(K * C));`
- `ComputeBiasNormRow` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:259` `void ComputeBiasNormRow(void* user_data, size_t r)`
- `Compute` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:277` `void Compute(OrtKernelContext* context)`
- `ComputeBypassRow` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:311` `void ComputeBypassRow(void* user_data, size_t r)`
- `Compute` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:323` `void Compute(OrtKernelContext* context)`
- `CreateKernel` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:350` `void* CreateKernel(const OrtApi& /*api*/,
                     const OrtKernelInfo* /*info*/) const`
- `GetName` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:354` `const char* GetName() const`
- `GetInputTypeCount` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:355` `size_t GetInputTypeCount() const`
- `GetInputType` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:356` `ONNXTensorElementDataType GetInputType(size_t /*index*/) const`
- `GetOutputTypeCount` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:359` `size_t GetOutputTypeCount() const`
- `GetOutputType` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:360` `ONNXTensorElementDataType GetOutputType(size_t /*index*/) const`
- `CreateKernel` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:366` `void* CreateKernel(const OrtApi& /*api*/,
                     const OrtKernelInfo* /*info*/) const`
- `GetName` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:370` `const char* GetName() const`
- `GetInputTypeCount` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:371` `size_t GetInputTypeCount() const`
- `GetInputType` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:372` `ONNXTensorElementDataType GetInputType(size_t /*index*/) const`
- `GetOutputTypeCount` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:375` `size_t GetOutputTypeCount() const`
- `GetOutputType` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:376` `ONNXTensorElementDataType GetOutputType(size_t /*index*/) const`
- `CreateKernel` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:382` `void* CreateKernel(const OrtApi& /*api*/,
                     const OrtKernelInfo* /*info*/) const`
- `GetName` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:386` `const char* GetName() const`
- `GetInputTypeCount` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:387` `size_t GetInputTypeCount() const`
- `GetInputType` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:388` `ONNXTensorElementDataType GetInputType(size_t /*index*/) const`
- `GetOutputTypeCount` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:391` `size_t GetOutputTypeCount() const`
- `GetOutputType` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:392` `ONNXTensorElementDataType GetOutputType(size_t /*index*/) const`
- `CreateKernel` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:399` `void* CreateKernel(const OrtApi& /*api*/,
                     const OrtKernelInfo* /*info*/) const`
- `GetName` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:403` `const char* GetName() const`
- `GetInputTypeCount` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:404` `size_t GetInputTypeCount() const`
- `GetInputType` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:405` `ONNXTensorElementDataType GetInputType(size_t /*index*/) const`
- `GetOutputTypeCount` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:408` `size_t GetOutputTypeCount() const`
- `GetOutputType` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:409` `ONNXTensorElementDataType GetOutputType(size_t /*index*/) const`
- `CreateKernel` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:415` `void* CreateKernel(const OrtApi& /*api*/,
                     const OrtKernelInfo* /*info*/) const`
- `GetName` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:419` `const char* GetName() const`
- `GetInputTypeCount` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:420` `size_t GetInputTypeCount() const`
- `GetInputType` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:421` `ONNXTensorElementDataType GetInputType(size_t /*index*/) const`
- `GetOutputTypeCount` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:424` `size_t GetOutputTypeCount() const`
- `GetOutputType` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:425` `ONNXTensorElementDataType GetOutputType(size_t /*index*/) const`
- `CreateKernel` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:431` `void* CreateKernel(const OrtApi& /*api*/,
                     const OrtKernelInfo* /*info*/) const`
- `GetName` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:435` `const char* GetName() const`
- `GetInputTypeCount` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:436` `size_t GetInputTypeCount() const`
- `GetInputType` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:437` `ONNXTensorElementDataType GetInputType(size_t /*index*/) const`
- `GetOutputTypeCount` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:440` `size_t GetOutputTypeCount() const`
- `GetOutputType` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:441` `ONNXTensorElementDataType GetOutputType(size_t /*index*/) const`
- `zipvoice_domain` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:457` `Ort::CustomOpDomain& zipvoice_domain()` -- One process-lifetime domain holding all ops; safe to Add() to multiple SessionOptions.
- `zipvoice_register_custom_ops` (function) `core/moonshine-tts/src/zipvoice-custom-ops.cpp:473` `void zipvoice_register_custom_ops(Ort::SessionOptions& opts)`

## core/moonshine-tts/src/zipvoice-custom-ops.h
Imported by: `core/moonshine-tts/src/zipvoice-custom-ops.cpp`, `core/moonshine-tts/src/zipvoice-tts.cpp`
- `zipvoice_register_custom_ops` (function) `core/moonshine-tts/src/zipvoice-custom-ops.h:15` `void zipvoice_register_custom_ops(Ort::SessionOptions& opts);` -- Registers the ``ai.zipvoice`` custom ONNX Runtime operators (SwooshL / SwooshR / GluGate / DepthwiseConv1d /...

## core/moonshine-tts/src/zipvoice-mel.cpp
Depends on: `core/moonshine-tts/src/zipvoice-mel.h`
- `hz_to_bin_count` (function) `core/moonshine-tts/src/zipvoice-mel.cpp:12` `int hz_to_bin_count(int n_fft)`
- `hz_to_mel_htk` (function) `core/moonshine-tts/src/zipvoice-mel.cpp:14` `double hz_to_mel_htk(double f)`
- `mel_to_hz_htk` (function) `core/moonshine-tts/src/zipvoice-mel.cpp:15` `double mel_to_hz_htk(double m)`
- `fft_radix2` (function) `core/moonshine-tts/src/zipvoice-mel.cpp:21` `void fft_radix2(std::vector<double>& re, std::vector<double>& im)` -- Iterative radix-2 Cooley-Tukey FFT for power-of-two ``n`` (in-place, natural -> natural order).
- `reflect_index` (function) `core/moonshine-tts/src/zipvoice-mel.cpp:64` `size_t reflect_index(long idx, long len)` -- Reflect index into [0, len) the same way torch ``pad(mode="reflect")`` mirrors without repeating the edge sample.
- `VocosFbank` (function) `core/moonshine-tts/src/zipvoice-mel.cpp:81` `VocosFbank::VocosFbank()`
- `all_freqs` (function) `core/moonshine-tts/src/zipvoice-mel.cpp:93` `std::vector<double> all_freqs(static_cast<size_t>(n_freqs));`
- `f_pts` (function) `core/moonshine-tts/src/zipvoice-mel.cpp:100` `std::vector<double> f_pts(static_cast<size_t>(kNMels + 2));`
- `f_diff` (function) `core/moonshine-tts/src/zipvoice-mel.cpp:106` `std::vector<double> f_diff(static_cast<size_t>(kNMels + 1));`
- `num_frames_for` (function) `core/moonshine-tts/src/zipvoice-mel.cpp:132` `int VocosFbank::num_frames_for(size_t num_samples)`
- `extract` (function) `core/moonshine-tts/src/zipvoice-mel.cpp:136` `std::vector<float> VocosFbank::extract(const std::vector<float>& samples,
                       ...`
- `out` (function) `core/moonshine-tts/src/zipvoice-mel.cpp:145` `std::vector<float> out( static_cast<size_t>(frames) * static_cast<size_t>(kNMels), 0.F);`
- `re` (function) `core/moonshine-tts/src/zipvoice-mel.cpp:151` `std::vector<double> re(static_cast<size_t>(kNFft));`
- `im` (function) `core/moonshine-tts/src/zipvoice-mel.cpp:152` `std::vector<double> im(static_cast<size_t>(kNFft));`
- `mag` (function) `core/moonshine-tts/src/zipvoice-mel.cpp:153` `std::vector<double> mag(static_cast<size_t>(n_freqs));`

## core/moonshine-tts/src/zipvoice-mel.h
Imported by: `core/moonshine-tts/src/zipvoice-mel.cpp`, `core/moonshine-tts/src/zipvoice-tts.cpp`, `core/moonshine-tts/tests/zipvoice-tts-test.cpp`
- `num_frames_for` (function) `core/moonshine-tts/src/zipvoice-mel.h:27` `static int num_frames_for(size_t num_samples);` -- Number of STFT frames for ``num_samples`` (center padding): ``1 + num_samples / hop``.
- `extract` (function) `core/moonshine-tts/src/zipvoice-mel.h:32` `std::vector<float> extract(const std::vector<float>& samples, int* out_frames) const;` -- Returns row-major log-mel features of shape ``[frames, 100]`` (``out[t * 100 + m]``).

## core/moonshine-tts/src/zipvoice-tts.cpp
Depends on: `core/moonshine-tts/src/g2p-path.h`, `core/moonshine-tts/src/ipa-postprocess.h`, `core/moonshine-tts/src/moonshine-g2p.h`, `core/moonshine-tts/src/moonshine-tts-options.h`, `core/moonshine-tts/src/ort-onnx-external-data.h`, `core/moonshine-tts/src/ort-session-options.h`, `core/moonshine-tts/src/utf8-utils.h`, `core/moonshine-tts/src/zipvoice-custom-ops.h`, `core/moonshine-tts/src/zipvoice-mel.h`, `core/moonshine-tts/src/zipvoice-tts.h`, `core/moonshine-tts/src/zipvoice-voices.h`, `core/moonshine-utils/debug-utils.h`
- `normalize_lang_key` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:34` `std::string normalize_lang_key(std::string_view raw)`
- `resolve_zipvoice_lang` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:49` `void resolve_zipvoice_lang(const std::string& lang, std::string& g2p_dialect,
                   ...` -- English-only for now; structured so more locales can be added.
- `resample_linear` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:60` `std::vector<float> resample_linear(const std::vector<float>& x, int src_sr,
                     ...`
- `y` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:69` `std::vector<float> y(n_out);`
- `trim_edge_silence` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:87` `std::vector<float> trim_edge_silence(const std::vector<float>& wav,
                             ...` -- Approximate ``remove_silence`` edge trimming (pydub ``remove_silence_edges``): drop leading and trailing samples...
- `out` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:108` `std::vector<float> out(wav.begin() + static_cast<std::ptrdiff_t>(start), wav.begin() +...`
- `rms_of` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:117` `float rms_of(const std::vector<float>& x)`
- `get_time_steps` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:130` `std::vector<float> get_time_steps(int num_step, float t_shift)` -- ``get_time_steps``: linspace(0, 1, num_step + 1) then ``t_shift * t / (1 + (t_shift - 1) * t)``.
- `ts` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:131` `std::vector<float> ts(static_cast<size_t>(num_step + 1));`
- `token` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:158` `const std::string token(data + i, data + tab);`
- `id_str` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:159` `const std::string id_str(data + tab + 1, data + content_end);`
- `load_session` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:218` `Ort::Session load_session(std::string_view key, bool register_custom_ops,
                       ...`
- `k` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:225` `const std::string k(key);`
- `load_asset_bytes` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:256` `std::vector<uint8_t> load_asset_bytes(std::string_view key)`
- `ipa_text_to_token_ids` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:284` `std::vector<int64_t> ipa_text_to_token_ids(const std::string& text)`
- `ipa_to_token_ids` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:289` `std::vector<int64_t> ipa_to_token_ids(const std::string& ipa)`
- `Impl` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:306` `explicit Impl(const ZipVoiceTTSOptions& opt)`
- `speed` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:426` `double speed() const`
- `set_speed` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:427` `void set_speed(double s)`
- `normalize_audio` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:434` `bool normalize_audio() const`
- `set_normalize_audio` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:435` `void set_normalize_audio(bool on)`
- `output_volume` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:436` `float output_volume() const`
- `set_output_volume` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:437` `void set_output_volume(float v)`
- `run_text_encoder` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:441` `std::vector<float> run_text_encoder(const std::vector<int64_t>& tokens,
                         ...` -- Runs the text encoder for one target-token chunk and returns text_condition [frames*feat_dim] (row-major), setting...
- `sample_chunk` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:489` `std::vector<float> sample_chunk(const std::vector<int64_t>& tokens,
                             ...` -- One flow-matching Euler solve for a chunk; returns predicted features [T_gen*feat_dim] (row-major).
- `x` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:501` `std::vector<float> x(total);`
- `dist` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:503` `std::normal_distribution<float> dist(0.F, 1.F);`
- `speech_condition` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:508` `std::vector<float> speech_condition(total, 0.F);` -- speech_condition = pad(clone_features, to frames) along time.
- `pred` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:558` `std::vector<float> pred(static_cast<size_t>(gen_frames) * feat);`
- `run_vocoder` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:566` `std::vector<float> run_vocoder(const std::vector<float>& pred,
                                 i...` -- pred [T_gen*feat] row-major -> vocoder -> waveform.
- `mel` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:570` `std::vector<float> mel(static_cast<size_t>(gen_frames) * feat);` -- mel: [1, feat, T_gen], mel[0,c,t] = pred[t,c] / feat_scale.
- `wav` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:591` `std::vector<float> wav(n);`
- `chunk_target_ids` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:601` `std::vector<std::vector<int64_t>> chunk_target_ids(
      const std::vector<int64_t>& ids)` -- Split target token ids into chunks near a target size, preferring space-token boundaries.
- `cross_fade_concat` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:651` `static std::vector<float> cross_fade_concat(
      const std::vector<std::vector<float>>& chunks,...`
- `synthesize` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:691` `std::vector<float> synthesize(std::string_view text)`
- `synthesize_from_ipa` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:695` `std::vector<float> synthesize_from_ipa(std::string_view ipa)`
- `synthesize_from_token_ids` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:699` `std::vector<float> synthesize_from_token_ids(std::vector<int64_t> ids)`
- `ZipVoiceTTS` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:729` `ZipVoiceTTS::ZipVoiceTTS(const ZipVoiceTTSOptions& opt)
    : impl_(std::make_unique<Impl>(opt))`
- `set_speed` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:735` `void ZipVoiceTTS::set_speed(double speed)`
- `speed` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:736` `double ZipVoiceTTS::speed() const`
- `normalize_audio` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:737` `bool ZipVoiceTTS::normalize_audio() const`
- `set_normalize_audio` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:738` `void ZipVoiceTTS::set_normalize_audio(bool on)`
- `output_volume` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:741` `float ZipVoiceTTS::output_volume() const`
- `set_output_volume` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:742` `void ZipVoiceTTS::set_output_volume(float volume)`
- `synthesize` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:746` `std::vector<float> ZipVoiceTTS::synthesize(std::string_view text)`
- `synthesize_from_ipa` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:750` `std::vector<float> ZipVoiceTTS::synthesize_from_ipa(std::string_view ipa)`
- `zipvoice_compress_long_pauses` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:754` `std::vector<float> zipvoice_compress_long_pauses(const std::vector<float>& wav,
                 ...`
- `env` (function) `core/moonshine-tts/src/zipvoice-tts.cpp:764` `std::vector<float> env(wav.size(), 0.F);`

## core/moonshine-tts/src/zipvoice-tts.h
Depends on: `core/moonshine-tts/src/file-information.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`
Imported by: `core/moonshine-tts/src/moonshine-tts.cpp`, `core/moonshine-tts/src/zipvoice-tts.cpp`, `core/moonshine-tts/tests/zipvoice-tts-test.cpp`
- `set_speed` (function) `core/moonshine-tts/src/zipvoice-tts.h:76` `void set_speed(double speed);`
- `speed` (function) `core/moonshine-tts/src/zipvoice-tts.h:77` `double speed() const;`
- `normalize_audio` (function) `core/moonshine-tts/src/zipvoice-tts.h:78` `bool normalize_audio() const;`
- `set_normalize_audio` (function) `core/moonshine-tts/src/zipvoice-tts.h:79` `void set_normalize_audio(bool on);`
- `output_volume` (function) `core/moonshine-tts/src/zipvoice-tts.h:80` `float output_volume() const;`
- `set_output_volume` (function) `core/moonshine-tts/src/zipvoice-tts.h:81` `void set_output_volume(float volume);`
- `synthesize` (function) `core/moonshine-tts/src/zipvoice-tts.h:86` `std::vector<float> synthesize(std::string_view text);` -- Text -> IPA (MoonshineG2P) -> ZipVoice token ids -> text encoder / flow-matching decoder / vocoder -> mono float...
- `synthesize_from_ipa` (function) `core/moonshine-tts/src/zipvoice-tts.h:90` `std::vector<float> synthesize_from_ipa(std::string_view ipa);` -- Like ``synthesize`` but starts from an existing IPA phoneme string (the same format ``MoonshineG2P::text_to_ipa``...
- `zipvoice_compress_long_pauses` (function) `core/moonshine-tts/src/zipvoice-tts.h:100` `std::vector<float> zipvoice_compress_long_pauses(const std::vector<float>& wav, int sample_rate, float...` -- Post-process ZipVoice output: shorten internal pauses longer than ``max_silence_ms`` down to ``keep_silence_ms``...

## core/moonshine-tts/src/zipvoice-voices.cpp
Depends on: `core/moonshine-tts/src/zipvoice-voices.h`
- `zipvoice_find_builtin_voice` (function) `core/moonshine-tts/src/zipvoice-voices.cpp:7` `const ZipVoiceBuiltinVoice* zipvoice_find_builtin_voice(std::string_view id)`
- `zipvoice_builtin_voice_pcm_to_float` (function) `core/moonshine-tts/src/zipvoice-voices.cpp:18` `std::vector<float> zipvoice_builtin_voice_pcm_to_float(
    const ZipVoiceBuiltinVoice& voice)`
- `out` (function) `core/moonshine-tts/src/zipvoice-voices.cpp:20` `std::vector<float> out(voice.num_samples);`

## core/moonshine-tts/src/zipvoice-voices.h
Imported by: `core/moonshine-tts/src/moonshine-tts.cpp`, `core/moonshine-tts/src/zipvoice-tts.cpp`, `core/moonshine-tts/src/zipvoice-voices.cpp`, `core/moonshine-tts/tests/zipvoice-tts-test.cpp`
- `zipvoice_builtin_voices` (function) `core/moonshine-tts/src/zipvoice-voices.h:30` `const ZipVoiceBuiltinVoice* zipvoice_builtin_voices(size_t* count);` -- The compiled-in table of built-in voices.
- `zipvoice_find_builtin_voice` (function) `core/moonshine-tts/src/zipvoice-voices.h:34` `const ZipVoiceBuiltinVoice* zipvoice_find_builtin_voice(std::string_view id);` -- Looks up a built-in voice by ``id`` (without the ``zipvoice_`` prefix), or nullptr if not found.
- `zipvoice_builtin_voice_pcm_to_float` (function) `core/moonshine-tts/src/zipvoice-voices.h:38` `std::vector<float> zipvoice_builtin_voice_pcm_to_float( const ZipVoiceBuiltinVoice& voice);` -- Convenience: decode a built-in voice's PCM to normalized float samples in ``[-1, 1]``.

## core/moonshine-tts/tests/arabic-rule-g2p-test.cpp
Depends on: `core/moonshine-tts/src/lang-specific/arabic.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`
- `TEST_CASE` (function) `core/moonshine-tts/tests/arabic-rule-g2p-test.cpp:9` `TEST_CASE(
    "arabic rule g2p: first 100 wiki lines match reference IPA when assets and "
    "...`

## core/moonshine-tts/tests/chinese-rule-g2p-test.cpp
Depends on: `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h`, `core/moonshine-tts/src/lang-specific/chinese.h`, `core/moonshine-tts/src/moonshine-g2p.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`
- `make_temp_tsv` (function) `core/moonshine-tts/tests/chinese-rule-g2p-test.cpp:21` `std::filesystem::path make_temp_tsv(const char* contents)`
- `TEST_CASE` (function) `core/moonshine-tts/tests/chinese-rule-g2p-test.cpp:33` `TEST_CASE("chinese: dialect_resolves_to_chinese_rules")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/chinese-rule-g2p-test.cpp:44` `TEST_CASE(
    "chinese: lexicon lookup and Arabic numeral expansion via per-char Han "
    "IPA")`

## core/moonshine-tts/tests/dutch-rule-g2p-test.cpp
Depends on: `core/moonshine-tts/src/lang-specific/dutch.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`
- `make_temp_tsv` (function) `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp:17` `std::filesystem::path make_temp_tsv(const char* contents)`
- `TEST_CASE` (function) `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp:29` `TEST_CASE("dutch: lowercase homograph overrides capitalized")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp:38` `TEST_CASE(
    "dutch: lexicon stress not shifted by vocoder (unlike German policy)")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp:50` `TEST_CASE("dutch: rule IPA gets vocoder stress when enabled")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp:59` `TEST_CASE("dutch: normalize_ipa_stress_for_vocoder idempotent")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp:70` `TEST_CASE("dutch: dialect_resolves_to_dutch_rules")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp:79` `TEST_CASE("dutch: optional real dict fiets matches Python when data present")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp:93` `TEST_CASE(
    "dutch: wiki-text first 100 lines match reference IPA when data and golden "
    "...`

## core/moonshine-tts/tests/english-rule-g2p-test.cpp
Depends on: `core/moonshine-tts/src/lang-specific/english.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`
- `resolve_en_dict` (function) `core/moonshine-tts/tests/english-rule-g2p-test.cpp:15` `std::filesystem::path resolve_en_dict()`
- `TEST_CASE` (function) `core/moonshine-tts/tests/english-rule-g2p-test.cpp:22` `TEST_CASE("english: dialect_resolves_to_english_rules")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/english-rule-g2p-test.cpp:38` `TEST_CASE("english: tomato heteronym picks US vs British by dialect flag")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/english-rule-g2p-test.cpp:51` `TEST_CASE(
    "english: wiki-text first 100 lines match reference IPA when data and "
    "golde...`

## core/moonshine-tts/tests/french-rule-g2p-test.cpp
Depends on: `core/moonshine-tts/src/lang-specific/french.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`
- `strip_stress` (function) `core/moonshine-tts/tests/french-rule-g2p-test.cpp:16` `std::string strip_stress(std::string s)`
- `french_dict_present` (function) `core/moonshine-tts/tests/french-rule-g2p-test.cpp:36` `bool french_dict_present()`
- `TEST_CASE` (function) `core/moonshine-tts/tests/french-rule-g2p-test.cpp:43` `TEST_CASE("french: dialect_resolves_to_french_rules")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/french-rule-g2p-test.cpp:52` `TEST_CASE("french: ensure_french_nuclear_stress")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/french-rule-g2p-test.cpp:58` `TEST_CASE("french: liaison les amis" * doctest::skip(!french_dict_present()))`
- `TEST_CASE` (function) `core/moonshine-tts/tests/french-rule-g2p-test.cpp:70` `TEST_CASE("french: En 1891 cardinal expansion" *
          doctest::skip(!french_dict_present()))`
- `TEST_CASE` (function) `core/moonshine-tts/tests/french-rule-g2p-test.cpp:83` `TEST_CASE("french: punctuation keeps space before next word" *
          doctest::skip(!french_di...`
- `TEST_CASE` (function) `core/moonshine-tts/tests/french-rule-g2p-test.cpp:94` `TEST_CASE(
    "french: hyphenated OOV allez-vous matches Python (UTF-8 trim + stress)" *
    doc...`
- `TEST_CASE` (function) `core/moonshine-tts/tests/french-rule-g2p-test.cpp:105` `TEST_CASE("french: uppercase accented letters in words (Saint-Étienne)" *
          doctest::skip...`
- `TEST_CASE` (function) `core/moonshine-tts/tests/french-rule-g2p-test.cpp:115` `TEST_CASE(
    "french: wiki-text first 100 lines match reference IPA when data and "
    "golden...`

## core/moonshine-tts/tests/german-rule-g2p-test.cpp
Depends on: `core/moonshine-tts/src/lang-specific/german.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`
- `make_temp_tsv` (function) `core/moonshine-tts/tests/german-rule-g2p-test.cpp:17` `std::filesystem::path make_temp_tsv(const char* contents)`
- `TEST_CASE` (function) `core/moonshine-tts/tests/german-rule-g2p-test.cpp:29` `TEST_CASE("german: lowercase homograph overrides capitalized")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/german-rule-g2p-test.cpp:38` `TEST_CASE(
    "german: lexicon entry with syllable-initial stress gets vocoder shift")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/german-rule-g2p-test.cpp:46` `TEST_CASE(
    "german: syllable-initial stress preserved when vocoder_stress false")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/german-rule-g2p-test.cpp:56` `TEST_CASE("german: OOV rules machen")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/german-rule-g2p-test.cpp:68` `TEST_CASE("german: normalize_ipa_stress_for_vocoder idempotent")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/german-rule-g2p-test.cpp:76` `TEST_CASE("german: dialect_resolves_to_german_rules")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/german-rule-g2p-test.cpp:85` `TEST_CASE("german: text token preserves comma")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/german-rule-g2p-test.cpp:93` `TEST_CASE(
    "german: Im Jahr 1891 matches reference IPA when data and golden exist")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/german-rule-g2p-test.cpp:109` `TEST_CASE(
    "german: wiki-text first 100 lines match reference IPA when data and "
    "golden...`

## core/moonshine-tts/tests/hindi-rule-g2p-test.cpp
Depends on: `core/moonshine-tts/src/lang-specific/hindi-numbers.h`, `core/moonshine-tts/src/lang-specific/hindi.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`
- `check_wiki_parity` (function) `core/moonshine-tts/tests/hindi-rule-g2p-test.cpp:17` `void check_wiki_parity(const std::filesystem::path& wiki,
                       const std::files...`
- `TEST_CASE` (function) `core/moonshine-tts/tests/hindi-rule-g2p-test.cpp:37` `TEST_CASE("hindi: dialect_resolves_to_hindi_rules")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/hindi-rule-g2p-test.cpp:45` `TEST_CASE("hindi: कमल and मैं match reference IPA when golden exists")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/hindi-rule-g2p-test.cpp:60` `TEST_CASE("hindi: expand_cardinal_digits_to_hindi_words")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/hindi-rule-g2p-test.cpp:66` `TEST_CASE(
    "hindi: wiki-text first 100 lines match reference IPA when data and golden "
    "...`

## core/moonshine-tts/tests/italian-rule-g2p-test.cpp
Depends on: `core/moonshine-tts/src/lang-specific/italian.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`
- `make_temp_tsv` (function) `core/moonshine-tts/tests/italian-rule-g2p-test.cpp:17` `std::filesystem::path make_temp_tsv(const char* contents)`
- `TEST_CASE` (function) `core/moonshine-tts/tests/italian-rule-g2p-test.cpp:29` `TEST_CASE("italian: dialect_resolves_to_italian_rules")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/italian-rule-g2p-test.cpp:38` `TEST_CASE("italian: lowercase homograph overrides capitalized")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/italian-rule-g2p-test.cpp:47` `TEST_CASE("italian: lexicon stress not shifted by vocoder")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/italian-rule-g2p-test.cpp:56` `TEST_CASE("italian: c'è matches reference IPA when data and golden exist")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/italian-rule-g2p-test.cpp:74` `TEST_CASE(
    "italian: wiki-text first 100 lines match reference IPA when data and "
    "golde...`

## core/moonshine-tts/tests/json-config-test.cpp
Depends on: `core/moonshine-tts/src/json-config.h`
- `TEST_CASE` (function) `core/moonshine-tts/tests/json-config-test.cpp:11` `TEST_CASE("load_oov_tables from onnx-config.json")`

## core/moonshine-tts/tests/korean-rule-g2p-test.cpp
Depends on: `core/moonshine-tts/src/lang-specific/korean-numbers.h`, `core/moonshine-tts/src/lang-specific/korean.h`, `core/moonshine-tts/src/moonshine-g2p.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`
- `ko_dict_path` (function) `core/moonshine-tts/tests/korean-rule-g2p-test.cpp:19` `std::filesystem::path ko_dict_path()`
- `TEST_CASE` (function) `core/moonshine-tts/tests/korean-rule-g2p-test.cpp:25` `TEST_CASE("korean: dialect_resolves_to_korean_rules")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/korean-rule-g2p-test.cpp:34` `TEST_CASE(
    "korean: normalize strips all combining marks including tense and "
    "unreleased")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/korean-rule-g2p-test.cpp:67` `TEST_CASE("korean: int_to_sino_korean_hangul")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/korean-rule-g2p-test.cpp:79` `TEST_CASE("korean: korean_reading_fragments_from_ascii_numeral_token")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/korean-rule-g2p-test.cpp:103` `TEST_CASE("korean: G2P examples with data/ko/dict.tsv")`

## core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp
Depends on: `core/moonshine-tts/src/lang-specific/portuguese.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`
- `make_temp_tsv` (function) `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp:17` `std::filesystem::path make_temp_tsv(const char* contents)`
- `TEST_CASE` (function) `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp:29` `TEST_CASE("portuguese: dialect flags")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp:40` `TEST_CASE("portuguese: lowercase homograph overrides capitalized")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp:49` `TEST_CASE("portuguese: lexicon stress not shifted by vocoder")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp:58` `TEST_CASE("portuguese: casa matches reference IPA when data and golden exist")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp:73` `TEST_CASE(
    "portuguese: wiki-text first 100 lines pt_br match reference IPA when data "
    "...`
- `TEST_CASE` (function) `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp:99` `TEST_CASE(
    "portuguese: wiki-text first 100 lines pt_pt match reference IPA when data "
    "...`

## core/moonshine-tts/tests/rule-g2p-test-support.h
Imported by: `core/moonshine-tts/tests/arabic-rule-g2p-test.cpp`, `core/moonshine-tts/tests/chinese-rule-g2p-test.cpp`, `core/moonshine-tts/tests/chinese-tok-pos-onnx-test.cpp`, `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp`, `core/moonshine-tts/tests/english-rule-g2p-test.cpp`, `core/moonshine-tts/tests/french-rule-g2p-test.cpp`, `core/moonshine-tts/tests/german-rule-g2p-test.cpp`, `core/moonshine-tts/tests/hindi-rule-g2p-test.cpp`, `core/moonshine-tts/tests/italian-rule-g2p-test.cpp`, `core/moonshine-tts/tests/japanese-onnx-g2p-test.cpp`, `core/moonshine-tts/tests/japanese-tok-pos-onnx-test.cpp`, `core/moonshine-tts/tests/korean-rule-g2p-test.cpp`, `core/moonshine-tts/tests/korean-tok-pos-onnx-test.cpp`, `core/moonshine-tts/tests/moonshine-tts-speed-test.cpp`, `core/moonshine-tts/tests/onnx-g2p-smoke-test.cpp`, `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp`, `core/moonshine-tts/tests/russian-rule-g2p-test.cpp`, `core/moonshine-tts/tests/spanish-rule-g2p-test.cpp`, `core/moonshine-tts/tests/turkish-rule-g2p-test.cpp`, `core/moonshine-tts/tests/ukrainian-rule-g2p-test.cpp`, `core/moonshine-tts/tests/vietnamese-rule-g2p-test.cpp`
- `repo_root_from_tests_cpp` (function) `core/moonshine-tts/tests/rule-g2p-test-support.h:21` `inline std::filesystem::path repo_root_from_tests_cpp(
    const char* tests_cpp_file)` -- Directory that contains ``data/`` (lexicons, ONNX assets) and usually ``models/``.
- `tests_data_dir` (function) `core/moonshine-tts/tests/rule-g2p-test-support.h:34` `inline std::filesystem::path tests_data_dir(
    const std::filesystem::path& repo_root)` -- Pre-generated parity lines: ``<tts>/tests/data`` when built in-tree, or legacy monorepo paths.
- `split_unix_lines` (function) `core/moonshine-tts/tests/rule-g2p-test-support.h:53` `inline std::vector<std::string> split_unix_lines(std::string block)`
- `load_ref_text_trimmed` (function) `core/moonshine-tts/tests/rule-g2p-test-support.h:66` `inline std::string load_ref_text_trimmed(const std::filesystem::path& p)`
- `load_ref_lines` (function) `core/moonshine-tts/tests/rule-g2p-test-support.h:76` `inline std::vector<std::string> load_ref_lines(const std::filesystem::path& p)`
- `ref_lines_prefix` (function) `core/moonshine-tts/tests/rule-g2p-test-support.h:85` `inline std::vector<std::string> ref_lines_prefix(
    const std::filesystem::path& golden, std::s...` -- Use the first *n* lines from a golden file (generated for up to 100 wiki lines).
- `read_text_first_lines` (function) `core/moonshine-tts/tests/rule-g2p-test-support.h:96` `inline std::vector<std::string> read_text_first_lines(
    const std::filesystem::path& p, std::s...`
- `moonshine_tts_bundled_data_dir_relative` (function) `core/moonshine-tts/tests/rule-g2p-test-support.h:114` `inline std::filesystem::path moonshine_tts_bundled_data_dir_relative()` -- Path to the bundled ``moonshine-tts`` data tree, relative to the monorepo repository root.

## core/moonshine-tts/tests/russian-rule-g2p-test.cpp
Depends on: `core/moonshine-tts/src/lang-specific/russian.h`, `core/moonshine-tts/src/moonshine-g2p.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`
- `make_temp_tsv` (function) `core/moonshine-tts/tests/russian-rule-g2p-test.cpp:21` `std::filesystem::path make_temp_tsv(const char* contents)`
- `TEST_CASE` (function) `core/moonshine-tts/tests/russian-rule-g2p-test.cpp:33` `TEST_CASE("russian: dialect_resolves_to_russian_rules")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/russian-rule-g2p-test.cpp:42` `TEST_CASE("russian: lowercase homograph overrides capitalized")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/russian-rule-g2p-test.cpp:69` `TEST_CASE("russian: litva matches reference IPA when data and golden exist")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/russian-rule-g2p-test.cpp:84` `TEST_CASE(
    "russian: Cyrillic preposition plus 1891 matches reference IPA when data "
    "an...`
- `TEST_CASE` (function) `core/moonshine-tts/tests/russian-rule-g2p-test.cpp:102` `TEST_CASE(
    "russian: wiki-text first 100 lines match reference IPA when data and "
    "golde...`

## core/moonshine-tts/tests/spanish-rule-g2p-test.cpp
Depends on: `core/moonshine-tts/src/lang-specific/spanish.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`
- `check_wiki_parity` (function) `core/moonshine-tts/tests/spanish-rule-g2p-test.cpp:16` `void check_wiki_parity(const std::filesystem::path& wiki,
                       const std::files...`
- `TEST_CASE` (function) `core/moonshine-tts/tests/spanish-rule-g2p-test.cpp:35` `TEST_CASE("spanish: En 1891 matches reference IPA when golden exists")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/spanish-rule-g2p-test.cpp:47` `TEST_CASE("spanish: dialect ids include es-MX and es-ES")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/spanish-rule-g2p-test.cpp:53` `TEST_CASE(
    "spanish: wiki-text first 100 lines es_mx match reference IPA when data "
    "and...`
- `TEST_CASE` (function) `core/moonshine-tts/tests/spanish-rule-g2p-test.cpp:65` `TEST_CASE(
    "spanish: wiki-text first 100 lines es_es match reference IPA when data "
    "and...`

## core/moonshine-tts/tests/turkish-rule-g2p-test.cpp
Depends on: `core/moonshine-tts/src/lang-specific/turkish.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`
- `check_wiki_parity` (function) `core/moonshine-tts/tests/turkish-rule-g2p-test.cpp:16` `void check_wiki_parity(const std::filesystem::path& wiki,
                       const std::files...`
- `TEST_CASE` (function) `core/moonshine-tts/tests/turkish-rule-g2p-test.cpp:34` `TEST_CASE("turkish: dağ and değer match reference IPA when golden exists")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/turkish-rule-g2p-test.cpp:46` `TEST_CASE("turkish: dialect ids include tr and tr-TR")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/turkish-rule-g2p-test.cpp:52` `TEST_CASE(
    "turkish: wiki-text first 100 lines match reference IPA when data and "
    "golde...`

## core/moonshine-tts/tests/ukrainian-rule-g2p-test.cpp
Depends on: `core/moonshine-tts/src/lang-specific/ukrainian.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`
- `check_wiki_parity` (function) `core/moonshine-tts/tests/ukrainian-rule-g2p-test.cpp:16` `void check_wiki_parity(const std::filesystem::path& wiki,
                       const std::files...`
- `TEST_CASE` (function) `core/moonshine-tts/tests/ukrainian-rule-g2p-test.cpp:34` `TEST_CASE("ukrainian: m'ясо and кінь match reference IPA when golden exists")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/ukrainian-rule-g2p-test.cpp:46` `TEST_CASE("ukrainian: dialect ids include uk and uk-UA")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/ukrainian-rule-g2p-test.cpp:52` `TEST_CASE(
    "ukrainian: wiki-text first 100 lines match reference IPA when data and "
    "gol...`

## core/moonshine-tts/tests/vietnamese-rule-g2p-test.cpp
Depends on: `core/moonshine-tts/src/lang-specific/vietnamese.h`, `core/moonshine-tts/src/moonshine-g2p.h`, `core/moonshine-tts/tests/rule-g2p-test-support.h`
- `vi_dict_path` (function) `core/moonshine-tts/tests/vietnamese-rule-g2p-test.cpp:18` `std::filesystem::path vi_dict_path()`
- `TEST_CASE` (function) `core/moonshine-tts/tests/vietnamese-rule-g2p-test.cpp:24` `TEST_CASE("vietnamese: dialect_resolves_to_vietnamese_rules")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/vietnamese-rule-g2p-test.cpp:33` `TEST_CASE("vietnamese: syllable OOV parity with Python samples")`
- `TEST_CASE` (function) `core/moonshine-tts/tests/vietnamese-rule-g2p-test.cpp:42` `TEST_CASE("vietnamese: lexicon line with data/vi/dict.tsv")`

## core/moonshine-tts/tools/arabic-rule-g2p-cli.cpp
Depends on: `core/moonshine-tts/src/lang-specific/arabic.h`
- `usage` (function) `core/moonshine-tts/tools/arabic-rule-g2p-cli.cpp:12` `void usage(const char* argv0)`
- `read_all_stdin` (function) `core/moonshine-tts/tools/arabic-rule-g2p-cli.cpp:19` `std::string read_all_stdin()`
- `main` (function) `core/moonshine-tts/tools/arabic-rule-g2p-cli.cpp:27` `int main(int argc, char** argv)`

## core/moonshine-tts/tools/chinese-rule-g2p-cli.cpp
Depends on: `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h`
- `usage` (function) `core/moonshine-tts/tools/chinese-rule-g2p-cli.cpp:13` `void usage(const char* argv0)`
- `read_all_stdin` (function) `core/moonshine-tts/tools/chinese-rule-g2p-cli.cpp:20` `std::string read_all_stdin()`
- `main` (function) `core/moonshine-tts/tools/chinese-rule-g2p-cli.cpp:28` `int main(int argc, char** argv)`

## core/moonshine-tts/tools/dutch-g2p-batch-cli.cpp
Depends on: `core/moonshine-tts/src/lang-specific/dutch.h`
- `usage` (function) `core/moonshine-tts/tools/dutch-g2p-batch-cli.cpp:15` `void usage(const char* argv0)`
- `trim_sv` (function) `core/moonshine-tts/tools/dutch-g2p-batch-cli.cpp:30` `std::string trim_sv(std::string s)`
- `read_all_stdin` (function) `core/moonshine-tts/tools/dutch-g2p-batch-cli.cpp:42` `std::string read_all_stdin()`
- `main` (function) `core/moonshine-tts/tools/dutch-g2p-batch-cli.cpp:50` `int main(int argc, char** argv)`

## core/moonshine-tts/tools/dutch-rule-g2p-cli.cpp
Depends on: `core/moonshine-tts/src/lang-specific/dutch.h`
- `usage` (function) `core/moonshine-tts/tools/dutch-rule-g2p-cli.cpp:13` `void usage(const char* argv0)`
- `read_all_stdin` (function) `core/moonshine-tts/tools/dutch-rule-g2p-cli.cpp:22` `std::string read_all_stdin()`
- `main` (function) `core/moonshine-tts/tools/dutch-rule-g2p-cli.cpp:30` `int main(int argc, char** argv)`

## core/moonshine-tts/tools/french-g2p-batch-cli.cpp
Depends on: `core/moonshine-tts/src/lang-specific/french.h`
- `usage` (function) `core/moonshine-tts/tools/french-g2p-batch-cli.cpp:15` `void usage(const char* argv0)`
- `trim_sv` (function) `core/moonshine-tts/tools/french-g2p-batch-cli.cpp:31` `std::string trim_sv(std::string s)`
- `read_all_stdin` (function) `core/moonshine-tts/tools/french-g2p-batch-cli.cpp:43` `std::string read_all_stdin()`
- `main` (function) `core/moonshine-tts/tools/french-g2p-batch-cli.cpp:51` `int main(int argc, char** argv)`

## core/moonshine-tts/tools/german-rule-g2p-cli.cpp
Depends on: `core/moonshine-tts/src/lang-specific/german.h`
- `usage` (function) `core/moonshine-tts/tools/german-rule-g2p-cli.cpp:13` `void usage(const char* argv0)`
- `read_all_stdin` (function) `core/moonshine-tts/tools/german-rule-g2p-cli.cpp:21` `std::string read_all_stdin()`
- `main` (function) `core/moonshine-tts/tools/german-rule-g2p-cli.cpp:29` `int main(int argc, char** argv)`

## core/moonshine-tts/tools/hindi-rule-g2p-cli.cpp
Depends on: `core/moonshine-tts/src/lang-specific/hindi.h`
- `usage` (function) `core/moonshine-tts/tools/hindi-rule-g2p-cli.cpp:12` `void usage(const char* argv0)`
- `read_all_stdin` (function) `core/moonshine-tts/tools/hindi-rule-g2p-cli.cpp:20` `std::string read_all_stdin()`
- `main` (function) `core/moonshine-tts/tools/hindi-rule-g2p-cli.cpp:28` `int main(int argc, char** argv)`

## core/moonshine-tts/tools/italian-rule-g2p-cli.cpp
Depends on: `core/moonshine-tts/src/lang-specific/italian.h`
- `usage` (function) `core/moonshine-tts/tools/italian-rule-g2p-cli.cpp:13` `void usage(const char* argv0)`
- `read_all_stdin` (function) `core/moonshine-tts/tools/italian-rule-g2p-cli.cpp:22` `std::string read_all_stdin()`
- `main` (function) `core/moonshine-tts/tools/italian-rule-g2p-cli.cpp:30` `int main(int argc, char** argv)`

## core/moonshine-tts/tools/japanese-onnx-g2p-cli.cpp
Depends on: `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.h`
- `usage` (function) `core/moonshine-tts/tools/japanese-onnx-g2p-cli.cpp:11` `void usage(const char* argv0)`
- `read_all_stdin` (function) `core/moonshine-tts/tools/japanese-onnx-g2p-cli.cpp:16` `std::string read_all_stdin()`
- `main` (function) `core/moonshine-tts/tools/japanese-onnx-g2p-cli.cpp:24` `int main(int argc, char** argv)`

## core/moonshine-tts/tools/korean-rule-g2p-cli.cpp
Depends on: `core/moonshine-tts/src/lang-specific/korean.h`
- `usage` (function) `core/moonshine-tts/tools/korean-rule-g2p-cli.cpp:13` `void usage(const char* argv0)`
- `read_all_stdin` (function) `core/moonshine-tts/tools/korean-rule-g2p-cli.cpp:20` `std::string read_all_stdin()`
- `main` (function) `core/moonshine-tts/tools/korean-rule-g2p-cli.cpp:28` `int main(int argc, char** argv)`

## core/moonshine-tts/tools/moonshine-g2p-cli.cpp
Depends on: `core/moonshine-tts/src/g2p-word-log.h`, `core/moonshine-tts/src/lang-specific/spanish.h`, `core/moonshine-tts/src/moonshine-g2p.h`
- `usage` (function) `core/moonshine-tts/tools/moonshine-g2p-cli.cpp:24` `void usage(const char *argv0)`
- `read_all_stdin` (function) `core/moonshine-tts/tools/moonshine-g2p-cli.cpp:102` `std::string read_all_stdin()`
- `rule_based_kind_label` (function) `core/moonshine-tts/tools/moonshine-g2p-cli.cpp:108` `const char *rule_based_kind_label(RuleBasedG2pKind k)`
- `print_rule_based_dialect_catalog` (function) `core/moonshine-tts/tools/moonshine-g2p-cli.cpp:147` `void print_rule_based_dialect_catalog(std::ostream &os)`
- `main` (function) `core/moonshine-tts/tools/moonshine-g2p-cli.cpp:160` `int main(int argc, char **argv)`

## core/moonshine-tts/tools/moonshine-tts-cli.cpp
Depends on: `core/moonshine-tts/src/moonshine-tts.h`, `core/moonshine-tts/src/utf8-utils.h`
- `usage` (function) `core/moonshine-tts/tools/moonshine-tts-cli.cpp:15` `void usage(const char* argv0)`
- `infer_lang_from_text_utf8` (function) `core/moonshine-tts/tools/moonshine-tts-cli.cpp:59` `std::optional<std::string> infer_lang_from_text_utf8(const std::string& text)` -- When the user does not pass ``--lang``, infer a tag so Japanese text does not run through English G2P / ``af_heart``.
- `main` (function) `core/moonshine-tts/tools/moonshine-tts-cli.cpp:85` `int main(int argc, char** argv)`

## core/moonshine-tts/tools/piper-ipa-normalize-cli.cpp
Depends on: `core/moonshine-tts/src/ipa-postprocess.h`
- `print_usage` (function) `core/moonshine-tts/tools/piper-ipa-normalize-cli.cpp:17` `void print_usage()`
- `load_keys` (function) `core/moonshine-tts/tools/piper-ipa-normalize-cli.cpp:22` `bool load_keys(const std::string& path, std::unordered_set<std::string>& keys)`
- `main` (function) `core/moonshine-tts/tools/piper-ipa-normalize-cli.cpp:42` `int main(int argc, char** argv)`

## core/moonshine-tts/tools/piper-phoneme-infer-cli.cpp
Depends on: `core/moonshine-tts/src/moonshine-tts.h`, `core/moonshine-tts/src/piper-tts.h`
- `usage` (function) `core/moonshine-tts/tools/piper-phoneme-infer-cli.cpp:18` `void usage(const char* argv0)`
- `main` (function) `core/moonshine-tts/tools/piper-phoneme-infer-cli.cpp:34` `int main(int argc, char** argv)`

## core/moonshine-tts/tools/portuguese-rule-g2p-cli.cpp
Depends on: `core/moonshine-tts/src/lang-specific/portuguese.h`
- `usage` (function) `core/moonshine-tts/tools/portuguese-rule-g2p-cli.cpp:13` `void usage(const char* argv0)`
- `read_all_stdin` (function) `core/moonshine-tts/tools/portuguese-rule-g2p-cli.cpp:22` `std::string read_all_stdin()`
- `main` (function) `core/moonshine-tts/tools/portuguese-rule-g2p-cli.cpp:30` `int main(int argc, char** argv)`

## core/moonshine-tts/tools/vietnamese-rule-g2p-cli.cpp
Depends on: `core/moonshine-tts/src/lang-specific/vietnamese.h`
- `usage` (function) `core/moonshine-tts/tools/vietnamese-rule-g2p-cli.cpp:12` `void usage(const char* argv0)`
- `read_all_stdin` (function) `core/moonshine-tts/tools/vietnamese-rule-g2p-cli.cpp:18` `std::string read_all_stdin()`
- `main` (function) `core/moonshine-tts/tools/vietnamese-rule-g2p-cli.cpp:26` `int main(int argc, char** argv)`

## core/moonshine-utils/debug-utils.cpp
Depends on: `core/moonshine-utils/debug-utils.h`
- `log_backtrace` (function) `core/moonshine-utils/debug-utils.cpp:16` `void log_backtrace()`
- `load_wav_data` (function) `core/moonshine-utils/debug-utils.cpp:52` `bool load_wav_data(const char *path, float **out_float_data,
                   size_t *out_num_s...`
- `save_wav_data` (function) `core/moonshine-utils/debug-utils.cpp:197` `bool save_wav_data(const char *path, const float *audio_data,
                   size_t num_sampl...`
- `audio_int16` (function) `core/moonshine-utils/debug-utils.cpp:205` `std::vector<int16_t> audio_int16(num_samples);`
- `float_vector_stats_to_string` (function) `core/moonshine-utils/debug-utils.cpp:250` `std::string float_vector_stats_to_string(const std::vector<float> &vector)`
- `load_file_into_memory` (function) `core/moonshine-utils/debug-utils.cpp:269` `std::vector<uint8_t> load_file_into_memory(const std::string &path)`
- `data` (function) `core/moonshine-utils/debug-utils.cpp:277` `std::vector<uint8_t> data(size);`
- `save_memory_to_file` (function) `core/moonshine-utils/debug-utils.cpp:290` `void save_memory_to_file(const std::string &path,
                         const std::vector<uint...`


Next: [API_p6.md](API_p6.md)
