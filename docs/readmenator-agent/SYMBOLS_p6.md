# Symbols (page 6 of 12)
Previous: [SYMBOLS_p5.md](SYMBOLS_p5.md)

| Symbol | Kind | File:Line | Signature |
|--------|------|-----------|-----------|
| `ascii_lowercase_copy` | function | `core/moonshine-tts/src/moonshine-tts.cpp:690` | `std::string ascii_lowercase_copy(std::string_view s)` |
| `buf` | function | `core/moonshine-tts/src/moonshine-tts.cpp:677` | `std::vector<uint8_t> buf((std::istreambuf_iterator<char>(f)), std::istreambuf_iterator<char>());` |
| `cand` | function | `core/moonshine-tts/src/moonshine-tts.cpp:406` | `const std::string cand(vid);` |
| `cfg_str` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1089` | `const std::string cfg_str(reinterpret_cast<const char*>(cfg_buf), cfg_len);` |
| `chunk_phonemes` | function | `core/moonshine-tts/src/moonshine-tts.cpp:557` | `std::vector<std::string> chunk_phonemes(const std::string& ps,                                   ...` |
| `collapse_whitespace_join_single_space` | function | `core/moonshine-tts/src/moonshine-tts.cpp:116` | `std::string collapse_whitespace_join_single_space(const std::string& s)` |
| `def` | function | `core/moonshine-tts/src/moonshine-tts.cpp:397` | `const std::string def(default_voice);` |
| `detect_kokoro_style_input_name` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1000` | `void detect_kokoro_style_input_name()` |
| `detect_speed_input_element_type` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1011` | `void detect_speed_input_element_type()` |
| `empty` | function | `core/moonshine-tts/src/moonshine-tts.cpp:75` | `bool empty() const` |
| `id` | function | `core/moonshine-tts/src/moonshine-tts.cpp:810` | `const std::string id(vid);` |
| `infer_lang_profile_from_kokoro_voice` | function | `core/moonshine-tts/src/moonshine-tts.cpp:275` | `bool infer_lang_profile_from_kokoro_voice(std::string_view voice_sv,                             ...` |
| `json_key` | function | `core/moonshine-tts/src/moonshine-tts.cpp:869` | `const std::string json_key(kTtsPiperOnnxJsonKey);` |
| `k` | function | `core/moonshine-tts/src/moonshine-tts.cpp:702` | `const std::string k(canonical_key);` |
| `kokoro_tts_lang_supported` | function | `core/moonshine-tts/src/moonshine-tts.cpp:685` | `bool kokoro_tts_lang_supported(std::string_view lang_cli,                                const Mo...` |
| `kokoro_tts_lang_supported_inner` | function | `core/moonshine-tts/src/moonshine-tts.cpp:220` | `bool kokoro_tts_lang_supported_inner(std::string_view lang_cli,                                  ...` |
| `kokoro_vocoder_dependency_keys_with_options` | function | `core/moonshine-tts/src/moonshine-tts.cpp:760` | `std::vector<std::string> kokoro_vocoder_dependency_keys_with_options(     std::string_view langua...` |
| `kokoro_voice_asset_exists` | function | `core/moonshine-tts/src/moonshine-tts.cpp:316` | `bool kokoro_voice_asset_exists(const std::string& voice_id,                                const ...` |
| `lookup_lang_profile` | function | `core/moonshine-tts/src/moonshine-tts.cpp:166` | `const LangProfile* lookup_lang_profile(std::string_view key)` |
| `make_piper_options` | function | `core/moonshine-tts/src/moonshine-tts.cpp:710` | `PiperTTSOptions make_piper_options(std::string_view language,                                    ...` |
| `make_zipvoice_options` | function | `core/moonshine-tts/src/moonshine-tts.cpp:886` | `ZipVoiceTTSOptions make_zipvoice_options(std::string_view language,                              ...` |
| `maybe_align_en_profile_for_kokoro_voice` | function | `core/moonshine-tts/src/moonshine-tts.cpp:252` | `void maybe_align_en_profile_for_kokoro_voice(std::string_view voice,                             ...` |
| `moonshine_catalog_all_tts_vocoder_dependency_keys_union` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1646` | `std::vector<std::string> moonshine_catalog_all_tts_vocoder_dependency_keys_union()` |
| `moonshine_catalog_tts_vocoder_only_dependency_keys` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1612` | `std::vector<std::string> moonshine_catalog_tts_vocoder_only_dependency_keys(     std::string_view...` |
| `moonshine_catalog_tts_vocoder_only_dependency_keys` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1639` | `std::vector<std::string> moonshine_catalog_tts_vocoder_only_dependency_keys(     std::string_view...` |
| `moonshine_list_tts_voices_with_availability` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1663` | `std::vector<MoonshineTtsVoiceAvailability> moonshine_list_tts_voices_with_availability(std::strin...` |
| `normalize_audio` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1038` | `bool normalize_audio() const` |
| `normalize_ipa_to_kokoro` | function | `core/moonshine-tts/src/moonshine-tts.cpp:535` | `std::string normalize_ipa_to_kokoro(     std::string ipa, char kokoro_lang,     const std::unorde...` |
| `normalize_lang_key` | function | `core/moonshine-tts/src/moonshine-tts.cpp:144` | `std::string normalize_lang_key(std::string_view raw)` |
| `onnx_json_key` | function | `core/moonshine-tts/src/moonshine-tts.cpp:721` | `const std::string onnx_json_key(kTtsPiperOnnxJsonKey);` |
| `onnx_key` | function | `core/moonshine-tts/src/moonshine-tts.cpp:714` | `const std::string onnx_key(kTtsPiperOnnxKey);` |
| `output_volume` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1040` | `float output_volume() const` |
| `parse_synthesis_overrides_from_pairs` | function | `core/moonshine-tts/src/moonshine-tts.cpp:81` | `SynthesisOverrides parse_synthesis_overrides_from_pairs(     const std::vector<std::pair<std::str...` |
| `pcm` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1557` | `std::vector<int16_t> pcm(samples.size());` |
| `phoneme_str_to_input_ids` | function | `core/moonshine-tts/src/moonshine-tts.cpp:621` | `std::vector<int64_t> phoneme_str_to_input_ids(     const std::string& phonemes,     const std::un...` |
| `piper_vocoder_dependency_keys_with_options` | function | `core/moonshine-tts/src/moonshine-tts.cpp:866` | `std::vector<std::string> piper_vocoder_dependency_keys_with_options(     std::string_view languag...` |
| `pv_key` | function | `core/moonshine-tts/src/moonshine-tts.cpp:729` | `const std::string pv_key(kTtsPiperVoicesKey);` |
| `pvj_key` | function | `core/moonshine-tts/src/moonshine-tts.cpp:737` | `const std::string pvj_key(kTtsPiperVoicesJsonKey);` |
| `py_isspace_utf8_ch` | function | `core/moonshine-tts/src/moonshine-tts.cpp:98` | `bool py_isspace_utf8_ch(std::string_view ch)` |
| `read_kokorovoice` | function | `core/moonshine-tts/src/moonshine-tts.cpp:669` | `void read_kokorovoice(const std::filesystem::path& path,                       std::vector<float>...` |
| `read_kokorovoice_bytes` | function | `core/moonshine-tts/src/moonshine-tts.cpp:636` | `void read_kokorovoice_bytes(const uint8_t* data, size_t size,                             std::st...` |
| `ref_row` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1262` | `std::vector<float> ref_row(voice_cols_);` |
| `reload_voice_tensor` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1158` | `void reload_voice_tensor()` |
| `replace_utf8` | function | `core/moonshine-tts/src/moonshine-tts.cpp:56` | `void replace_utf8(std::string& s, std::string_view old_s,                   std::string_view new_s)` |
| `req` | function | `core/moonshine-tts/src/moonshine-tts.cpp:384` | `const std::string req(requested);` |
| `resolve_lang_for_kokoro` | function | `core/moonshine-tts/src/moonshine-tts.cpp:302` | `void resolve_lang_for_kokoro(const std::string& lk,                              const MoonshineG...` |
| `resolve_lang_for_tts` | function | `core/moonshine-tts/src/moonshine-tts.cpp:202` | `void resolve_lang_for_tts(const std::string& lk, const MoonshineG2POptions& opt,                 ...` |
| `run_with_overrides` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1449` | `template <typename Produce>   std::vector<float> run_with_overrides(const SynthesisOverrides& ov,...` |
| `select_voice_id` | function | `core/moonshine-tts/src/moonshine-tts.cpp:358` | `std::string select_voice_id(char kokoro_lang, std::string_view requested,                        ...` |
| `set_normalize_audio` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1039` | `void set_normalize_audio(bool on)` |
| `set_output_volume` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1041` | `void set_output_volume(float v)` |
| `set_speed` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1030` | `void set_speed(double s)` |
| `sort` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1718` | `std::sort(         out.begin(), out.end(),         [](const MoonshineTtsVoiceAvailability& a,    ...` |
| `speed` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1028` | `double speed() const` |
| `synthesize` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1199` | `std::vector<float> synthesize(std::string_view text)` |
| `synthesize` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1423` | `std::vector<float> synthesize(std::string_view text)` |
| `synthesize` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1512` | `std::vector<float> MoonshineTTS::synthesize(std::string_view text)` |
| `synthesize` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1516` | `std::vector<float> MoonshineTTS::synthesize(     std::string_view text,     const std::vector<std...` |
| `synthesize_from_ipa` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1210` | `std::vector<float> synthesize_from_ipa(std::string_view ipa)` |
| `synthesize_from_phonemes` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1428` | `std::vector<float> synthesize_from_phonemes(std::string_view phonemes)` |
| `synthesize_from_phonemes` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1530` | `std::vector<float> MoonshineTTS::synthesize_from_phonemes(     std::string_view phonemes)` |
| `synthesize_from_phonemes` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1535` | `std::vector<float> MoonshineTTS::synthesize_from_phonemes(     std::string_view phonemes,     con...` |
| `synthesize_from_phonemes_unlocked` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1412` | `std::vector<float> synthesize_from_phonemes_unlocked(       std::string_view phonemes)` |
| `synthesize_from_phonemes_with_overrides` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1433` | `std::vector<float> synthesize_from_phonemes_with_overrides(       std::string_view phonemes, cons...` |
| `synthesize_unlocked` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1395` | `std::vector<float> synthesize_unlocked(std::string_view text)` |
| `synthesize_with_overrides` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1439` | `std::vector<float> synthesize_with_overrides(std::string_view text,                              ...` |
| `tmp` | function | `core/moonshine-tts/src/moonshine-tts.cpp:45` | `const std::string tmp(s);` |
| `tts_map_path` | function | `core/moonshine-tts/src/moonshine-tts.cpp:700` | `std::filesystem::path tts_map_path(const FileInformationMap& m,                                  ...` |
| `utf8_nfc` | function | `core/moonshine-tts/src/moonshine-tts.cpp:44` | `std::string utf8_nfc(std::string_view s)` |
| `voice_prefix_ok` | function | `core/moonshine-tts/src/moonshine-tts.cpp:231` | `bool voice_prefix_ok(char kokoro_lang, std::string_view voice)` |
| `write_wav_mono_pcm16` | function | `core/moonshine-tts/src/moonshine-tts.cpp:1549` | `void write_wav_mono_pcm16(const std::filesystem::path& path,                           const std:...` |
| `zipvoice_asset_present` | function | `core/moonshine-tts/src/moonshine-tts.cpp:923` | `bool zipvoice_asset_present(const MoonshineTTSOptions& opt,                             std::stri...` |
| `zipvoice_assets_available` | function | `core/moonshine-tts/src/moonshine-tts.cpp:940` | `bool zipvoice_assets_available(const MoonshineTTSOptions& opt)` |
| `zipvoice_vocoder_dependency_keys` | function | `core/moonshine-tts/src/moonshine-tts.cpp:915` | `std::vector<std::string> zipvoice_vocoder_dependency_keys()` |
| `Impl` | struct | `core/moonshine-tts/src/moonshine-tts.h:60` | `` |
| `MOONSHINE_TTS_MOONSHINE_TTS_H` | macro | `core/moonshine-tts/src/moonshine-tts.h:2` | `#define MOONSHINE_TTS_MOONSHINE_TTS_H` |
| `MoonshineTTS` | class | `core/moonshine-tts/src/moonshine-tts.h:22` | `` |
| `MoonshineTtsVoiceAvailability` | struct | `core/moonshine-tts/src/moonshine-tts.h:86` | `` |
| `synthesize` | function | `core/moonshine-tts/src/moonshine-tts.h:33` | `std::vector<float> synthesize(std::string_view text);` |
| `synthesize_from_phonemes` | function | `core/moonshine-tts/src/moonshine-tts.h:50` | `std::vector<float> synthesize_from_phonemes(std::string_view phonemes);` |
| `write_wav_mono_pcm16` | function | `core/moonshine-tts/src/moonshine-tts.h:64` | `void write_wav_mono_pcm16(const std::filesystem::path& path, const std::vector<float>& samples);` |
| `ort_add_external_initializer_files_for_onnx_model_buffer` | function | `core/moonshine-tts/src/ort-onnx-external-data.cpp:10` | `void ort_add_external_initializer_files_for_onnx_model_buffer(     Ort::SessionOptions& opts, con...` |
| `MOONSHINE_TTS_ORT_ONNX_EXTERNAL_DATA_H` | macro | `core/moonshine-tts/src/ort-onnx-external-data.h:2` | `#define MOONSHINE_TTS_ORT_ONNX_EXTERNAL_DATA_H` |
| `ort_add_external_initializer_files_for_onnx_model_buffer` | function | `core/moonshine-tts/src/ort-onnx-external-data.h:18` | `void ort_add_external_initializer_files_for_onnx_model_buffer( Ort::SessionOptions& opts, const FileInformationMap&...` |
| `make_ort_session_options` | function | `core/moonshine-tts/src/ort-session-options.cpp:7` | `Ort::SessionOptions make_ort_session_options(     const std::vector<std::string>& provider_names,...` |
| `MOONSHINE_TTS_ORT_SESSION_OPTIONS_H` | macro | `core/moonshine-tts/src/ort-session-options.h:2` | `#define MOONSHINE_TTS_ORT_SESSION_OPTIONS_H` |
| `Impl` | function | `core/moonshine-tts/src/piper-tts.cpp:566` | `explicit Impl(const PiperTTSOptions& opt)       : speed_(opt.speed),         ort_provider_names_(...` |
| `PiperLangRow` | struct | `core/moonshine-tts/src/piper-tts.cpp:67` | `` |
| `PiperTTS` | function | `core/moonshine-tts/src/piper-tts.cpp:675` | `PiperTTS::PiperTTS(const PiperTTSOptions& opt)     : impl_(std::make_unique<Impl>(opt))` |
| `append_phoneme_ids` | function | `core/moonshine-tts/src/piper-tts.cpp:244` | `void append_phoneme_ids(     const std::unordered_map<std::string, std::vector<int64_t>>& id_map,...` |
| `ipa_utf8_to_piper_ids` | function | `core/moonshine-tts/src/piper-tts.cpp:256` | `std::vector<int64_t> ipa_utf8_to_piper_ids(     const std::string& ipa_nfc,     const std::unorde...` |
| `k_piper_json` | function | `core/moonshine-tts/src/piper-tts.cpp:512` | `static const std::string k_piper_json("piper/onnx.json");` |
| `k_piper_onnx` | function | `core/moonshine-tts/src/piper-tts.cpp:513` | `static const std::string k_piper_onnx("piper/onnx");` |
| `load_piper_onnx_json` | function | `core/moonshine-tts/src/piper-tts.cpp:301` | `void load_piper_onnx_json(     const std::filesystem::path& json_path,     std::unordered_map<std...` |
| `load_piper_onnx_json_bytes` | function | `core/moonshine-tts/src/piper-tts.cpp:354` | `void load_piper_onnx_json_bytes(     const char* data, size_t size, std::string_view ctx,     std...` |
| `lookup_piper_lang_row` | function | `core/moonshine-tts/src/piper-tts.cpp:73` | `const PiperLangRow* lookup_piper_lang_row(std::string_view k)` |
| `normalize_audio` | function | `core/moonshine-tts/src/piper-tts.cpp:695` | `bool PiperTTS::normalize_audio() const` |
| `normalize_lang_key` | function | `core/moonshine-tts/src/piper-tts.cpp:35` | `std::string normalize_lang_key(std::string_view raw)` |
| `output_volume` | function | `core/moonshine-tts/src/piper-tts.cpp:699` | `float PiperTTS::output_volume() const` |
| `p` | function | `core/moonshine-tts/src/piper-tts.cpp:771` | `const std::filesystem::path p(default_onnx);` |
| `pick_onnx_path` | function | `core/moonshine-tts/src/piper-tts.cpp:178` | `std::filesystem::path pick_onnx_path(const std::filesystem::path& voices_dir,                    ...` |
| `piper_default_model_bundle_relative_paths` | function | `core/moonshine-tts/src/piper-tts.cpp:796` | `bool piper_default_model_bundle_relative_paths(     std::string_view lang_cli, const MoonshineG2P...` |
| `piper_ipa_norm_lang_key` | function | `core/moonshine-tts/src/piper-tts.cpp:130` | `std::string piper_ipa_norm_lang_key(const std::string& lk,                                     st...` |
| `piper_model_json_path_for_onnx` | function | `core/moonshine-tts/src/piper-tts.cpp:233` | `std::filesystem::path piper_model_json_path_for_onnx(     const std::filesystem::path& onnx_path,...` |
| `py_isspace_utf8_ch` | function | `core/moonshine-tts/src/piper-tts.cpp:49` | `bool py_isspace_utf8_ch(std::string_view ch)` |
| `reload_session_from_onnx` | function | `core/moonshine-tts/src/piper-tts.cpp:511` | `void reload_session_from_onnx()` |
| `resample_linear` | function | `core/moonshine-tts/src/piper-tts.cpp:278` | `std::vector<float> resample_linear(const std::vector<float>& x, int src_sr,                      ...` |
| `resolve_piper_lang` | function | `core/moonshine-tts/src/piper-tts.cpp:144` | `void resolve_piper_lang(const std::string& lk, const MoonshineG2POptions& opt,                   ...` |
| `run_ort_from_phoneme_ids` | function | `core/moonshine-tts/src/piper-tts.cpp:446` | `std::vector<float> run_ort_from_phoneme_ids(const std::vector<int64_t>& ids)` |
| `set_lang` | function | `core/moonshine-tts/src/piper-tts.cpp:621` | `void set_lang(const std::string& lk)` |
| `set_lang` | function | `core/moonshine-tts/src/piper-tts.cpp:683` | `void PiperTTS::set_lang(std::string_view lang_cli)` |
| `set_normalize_audio` | function | `core/moonshine-tts/src/piper-tts.cpp:697` | `void PiperTTS::set_normalize_audio(bool on)` |
| `set_onnx_model` | function | `core/moonshine-tts/src/piper-tts.cpp:635` | `void set_onnx_model(std::string_view stem_or_base)` |
| `set_onnx_model` | function | `core/moonshine-tts/src/piper-tts.cpp:691` | `void PiperTTS::set_onnx_model(std::string_view basename_or_stem)` |
| `set_output_volume` | function | `core/moonshine-tts/src/piper-tts.cpp:701` | `void PiperTTS::set_output_volume(float volume)` |
| `set_speed` | function | `core/moonshine-tts/src/piper-tts.cpp:613` | `void set_speed(double s)` |
| `set_speed` | function | `core/moonshine-tts/src/piper-tts.cpp:687` | `void PiperTTS::set_speed(double speed)` |
| `speed` | function | `core/moonshine-tts/src/piper-tts.cpp:689` | `double PiperTTS::speed() const` |
| `synthesize` | function | `core/moonshine-tts/src/piper-tts.cpp:644` | `std::vector<float> synthesize(std::string_view text)` |
| `synthesize` | function | `core/moonshine-tts/src/piper-tts.cpp:705` | `std::vector<float> PiperTTS::synthesize(std::string_view text)` |
| `synthesize_from_ipa` | function | `core/moonshine-tts/src/piper-tts.cpp:649` | `std::vector<float> synthesize_from_ipa(std::string_view ipa_in)` |
| `synthesize_from_ipa` | function | `core/moonshine-tts/src/piper-tts.cpp:709` | `std::vector<float> PiperTTS::synthesize_from_ipa(std::string_view ipa)` |
| `synthesize_phoneme_ids` | function | `core/moonshine-tts/src/piper-tts.cpp:669` | `std::vector<float> synthesize_phoneme_ids(       const std::vector<int64_t>& phoneme_ids)` |
| `synthesize_phoneme_ids` | function | `core/moonshine-tts/src/piper-tts.cpp:713` | `std::vector<float> PiperTTS::synthesize_phoneme_ids(     const std::vector<int64_t>& phoneme_ids)` |
| `wave` | function | `core/moonshine-tts/src/piper-tts.cpp:502` | `std::vector<float> wave(ptr, ptr + n_el);` |
| `y` | function | `core/moonshine-tts/src/piper-tts.cpp:287` | `std::vector<float> y(n_out);` |
| `Impl` | struct | `core/moonshine-tts/src/piper-tts.h:108` | `` |
| `MOONSHINE_TTS_PIPER_TTS_H` | macro | `core/moonshine-tts/src/piper-tts.h:2` | `#define MOONSHINE_TTS_PIPER_TTS_H` |
| `PiperTTS` | class | `core/moonshine-tts/src/piper-tts.h:65` | `` |
| `PiperTTSOptions` | struct | `core/moonshine-tts/src/piper-tts.h:19` | `` |
| `normalize_audio` | function | `core/moonshine-tts/src/piper-tts.h:81` | `bool normalize_audio() const;` |
| `output_volume` | function | `core/moonshine-tts/src/piper-tts.h:83` | `float output_volume() const;` |
| `set_lang` | function | `core/moonshine-tts/src/piper-tts.h:74` | `void set_lang(std::string_view lang_cli);` |
| `set_normalize_audio` | function | `core/moonshine-tts/src/piper-tts.h:82` | `void set_normalize_audio(bool on);` |
| `set_onnx_model` | function | `core/moonshine-tts/src/piper-tts.h:78` | `void set_onnx_model(std::string_view basename_or_stem);` |
| `set_output_volume` | function | `core/moonshine-tts/src/piper-tts.h:84` | `void set_output_volume(float volume);` |
| `set_speed` | function | `core/moonshine-tts/src/piper-tts.h:75` | `void set_speed(double speed);` |
| `speed` | function | `core/moonshine-tts/src/piper-tts.h:76` | `double speed() const;` |
| `synthesize` | function | `core/moonshine-tts/src/piper-tts.h:90` | `std::vector<float> synthesize(std::string_view text);` |
| `synthesize_from_ipa` | function | `core/moonshine-tts/src/piper-tts.h:96` | `std::vector<float> synthesize_from_ipa(std::string_view ipa);` |
| `synthesize_phoneme_ids` | function | `core/moonshine-tts/src/piper-tts.h:104` | `std::vector<float> synthesize_phoneme_ids( const std::vector<int64_t>& phoneme_ids);` |
| `MOONSHINE_TTS_PIPER_VOICE_CATALOG_H` | macro | `core/moonshine-tts/src/piper-voice-catalog.h:2` | `#define MOONSHINE_TTS_PIPER_VOICE_CATALOG_H` |
| `piper_bundled_voice_stems_for_data_subdir` | function | `core/moonshine-tts/src/piper-voice-catalog.h:12` | `const std::vector<std::string>& piper_bundled_voice_stems_for_data_subdir( const std::string& data_subdir);` |
| `create_rule_based_g2p` | function | `core/moonshine-tts/src/rule-based-g2p-factory.cpp:786` | `std::optional<RuleBasedG2pInstance> create_rule_based_g2p(     std::string_view dialect_id, const...` |
| `file_looks_like_git_lfs_pointer` | function | `core/moonshine-tts/src/rule-based-g2p-factory.cpp:74` | `bool file_looks_like_git_lfs_pointer(const std::filesystem::path& p)` |
| `g2p_onnx_bundle_includes_model_file` | function | `core/moonshine-tts/src/rule-based-g2p-factory.cpp:141` | `bool g2p_onnx_bundle_includes_model_file(     const MoonshineG2POptions& o, std::string_view bund...` |
| `g2p_onnx_bundle_reachable` | function | `core/moonshine-tts/src/rule-based-g2p-factory.cpp:129` | `bool g2p_onnx_bundle_reachable(const MoonshineG2POptions& o,                                std::...` |
| `normalize_spanish_dialect_cli_key` | function | `core/moonshine-tts/src/rule-based-g2p-factory.cpp:51` | `std::string normalize_spanish_dialect_cli_key(std::string_view raw)` |
| `pt_override_key` | function | `core/moonshine-tts/src/rule-based-g2p-factory.cpp:716` | `const std::string pt_override_key(kG2pPortugueseDictOverrideKey);` |
| `read_path_as_utf8` | function | `core/moonshine-tts/src/rule-based-g2p-factory.cpp:96` | `std::string read_path_as_utf8(const std::filesystem::path& p)` |
| `resolve_french_csv_dir` | function | `core/moonshine-tts/src/rule-based-g2p-factory.cpp:46` | `std::filesystem::path resolve_french_csv_dir(const MoonshineG2POptions& opt)` |
| `resolve_french_dict_path` | function | `core/moonshine-tts/src/rule-based-g2p-factory.cpp:41` | `std::filesystem::path resolve_french_dict_path(const MoonshineG2POptions& opt)` |
| `try_arabic` | function | `core/moonshine-tts/src/rule-based-g2p-factory.cpp:611` | `std::optional<RuleBasedG2pInstance> try_arabic(     std::string_view trimmed, const MoonshineG2PO...` |
| `try_chinese` | function | `core/moonshine-tts/src/rule-based-g2p-factory.cpp:480` | `std::optional<RuleBasedG2pInstance> try_chinese(     std::string_view trimmed, const MoonshineG2P...` |
| `try_dutch` | function | `core/moonshine-tts/src/rule-based-g2p-factory.cpp:385` | `std::optional<RuleBasedG2pInstance> try_dutch(     std::string_view trimmed, const MoonshineG2POp...` |
| `try_english` | function | `core/moonshine-tts/src/rule-based-g2p-factory.cpp:174` | `std::optional<RuleBasedG2pInstance> try_english(     std::string_view trimmed, const MoonshineG2P...` |
| `try_french` | function | `core/moonshine-tts/src/rule-based-g2p-factory.cpp:335` | `std::optional<RuleBasedG2pInstance> try_french(     std::string_view trimmed, const MoonshineG2PO...` |
| `try_german` | function | `core/moonshine-tts/src/rule-based-g2p-factory.cpp:305` | `std::optional<RuleBasedG2pInstance> try_german(     std::string_view trimmed, const MoonshineG2PO...` |
| `try_hindi` | function | `core/moonshine-tts/src/rule-based-g2p-factory.cpp:680` | `std::optional<RuleBasedG2pInstance> try_hindi(     std::string_view trimmed, const MoonshineG2POp...` |
| `try_italian` | function | `core/moonshine-tts/src/rule-based-g2p-factory.cpp:417` | `std::optional<RuleBasedG2pInstance> try_italian(     std::string_view trimmed, const MoonshineG2P...` |
| `try_japanese` | function | `core/moonshine-tts/src/rule-based-g2p-factory.cpp:571` | `std::optional<RuleBasedG2pInstance> try_japanese(     std::string_view trimmed, const MoonshineG2...` |
| `try_korean` | function | `core/moonshine-tts/src/rule-based-g2p-factory.cpp:521` | `std::optional<RuleBasedG2pInstance> try_korean(     std::string_view trimmed, const MoonshineG2PO...` |
| `try_portuguese` | function | `core/moonshine-tts/src/rule-based-g2p-factory.cpp:707` | `std::optional<RuleBasedG2pInstance> try_portuguese(     std::string_view trimmed, const Moonshine...` |
| `try_russian` | function | `core/moonshine-tts/src/rule-based-g2p-factory.cpp:449` | `std::optional<RuleBasedG2pInstance> try_russian(     std::string_view trimmed, const MoonshineG2P...` |
| `try_spanish` | function | `core/moonshine-tts/src/rule-based-g2p-factory.cpp:288` | `std::optional<RuleBasedG2pInstance> try_spanish(     std::string_view trimmed, const MoonshineG2P...` |
| `try_turkish` | function | `core/moonshine-tts/src/rule-based-g2p-factory.cpp:650` | `std::optional<RuleBasedG2pInstance> try_turkish(     std::string_view trimmed, const MoonshineG2P...` |
| `try_ukrainian` | function | `core/moonshine-tts/src/rule-based-g2p-factory.cpp:665` | `std::optional<RuleBasedG2pInstance> try_ukrainian(     std::string_view trimmed, const MoonshineG...` |
| `try_vietnamese` | function | `core/moonshine-tts/src/rule-based-g2p-factory.cpp:547` | `std::optional<RuleBasedG2pInstance> try_vietnamese(     std::string_view trimmed, const Moonshine...` |
| `utf8_content_git_lfs_pointer_stub` | function | `core/moonshine-tts/src/rule-based-g2p-factory.cpp:86` | `bool utf8_content_git_lfs_pointer_stub(std::string_view content)` |
| `MOONSHINE_TTS_RULE_BASED_G2P_FACTORY_H` | macro | `core/moonshine-tts/src/rule-based-g2p-factory.h:2` | `#define MOONSHINE_TTS_RULE_BASED_G2P_FACTORY_H` |
| `RuleBasedG2pInstance` | struct | `core/moonshine-tts/src/rule-based-g2p-factory.h:35` | `` |
| `RuleBasedG2pKind` | enum | `core/moonshine-tts/src/rule-based-g2p-factory.h:16` | `` |
| `RuleBasedG2pKind` | class | `core/moonshine-tts/src/rule-based-g2p-factory.h:16` | `` |
| `G2pWordLog` | struct | `core/moonshine-tts/src/rule-based-g2p.h:9` | `` |
| `MOONSHINE_TTS_RULE_BASED_G2P_H` | macro | `core/moonshine-tts/src/rule-based-g2p.h:2` | `#define MOONSHINE_TTS_RULE_BASED_G2P_H` |
| `RuleBasedG2p` | class | `core/moonshine-tts/src/rule-based-g2p.h:12` | `` |
| `is_word_char_utf8` | function | `core/moonshine-tts/src/text-normalize.cpp:10` | `bool is_word_char_utf8(std::string_view unit)` |
| `normalize_grapheme_key` | function | `core/moonshine-tts/src/text-normalize.cpp:75` | `std::string normalize_grapheme_key(std::string_view word_token)` |
| `normalize_word_for_lookup` | function | `core/moonshine-tts/src/text-normalize.cpp:48` | `std::string normalize_word_for_lookup(std::string_view token)` |
| `split_text_to_words` | function | `core/moonshine-tts/src/text-normalize.cpp:25` | `std::vector<std::string> split_text_to_words(std::string_view text)` |
| `MOONSHINE_TTS_TEXT_NORMALIZE_H` | macro | `core/moonshine-tts/src/text-normalize.h:2` | `#define MOONSHINE_TTS_TEXT_NORMALIZE_H` |
| `codepoint_is_unicode_word_neighbor_for_digits` | function | `core/moonshine-tts/src/utf8-utils.cpp:183` | `bool codepoint_is_unicode_word_neighbor_for_digits(char32_t c)` |
| `dedupe_dialect_ids_preserve_first` | function | `core/moonshine-tts/src/utf8-utils.cpp:278` | `std::vector<std::string> dedupe_dialect_ids_preserve_first(     std::vector<std::string> ids)` |
| `digit_ascii_span_expandable_python_w` | function | `core/moonshine-tts/src/utf8-utils.cpp:250` | `bool digit_ascii_span_expandable_python_w(const std::string& text,                               ...` |
| `normalize_rule_based_dialect_cli_key` | function | `core/moonshine-tts/src/utf8-utils.cpp:266` | `std::string normalize_rule_based_dialect_cli_key(std::string_view raw)` |
| `utf8_append_codepoint` | function | `core/moonshine-tts/src/utf8-utils.cpp:75` | `void utf8_append_codepoint(std::string& out, char32_t cp)` |
| `utf8_codepoint_at_index` | function | `core/moonshine-tts/src/utf8-utils.cpp:237` | `std::optional<char32_t> utf8_codepoint_at_index(const std::string& s,                            ...` |
| `utf8_codepoint_before_index` | function | `core/moonshine-tts/src/utf8-utils.cpp:220` | `std::optional<char32_t> utf8_codepoint_before_index(const std::string& s,                        ...` |
| `utf8_decode_at` | function | `core/moonshine-tts/src/utf8-utils.cpp:7` | `bool utf8_decode_at(const std::string& s, size_t i, char32_t& out_cp,                     size_t&...` |
| `utf8_split_codepoints` | function | `core/moonshine-tts/src/utf8-utils.cpp:93` | `std::vector<std::string> utf8_split_codepoints(const std::string& utf8)` |
| `utf8_str_to_u32` | function | `core/moonshine-tts/src/utf8-utils.cpp:62` | `std::u32string utf8_str_to_u32(const std::string& s)` |
| `MOONSHINE_TTS_UTF8_UTILS_H` | macro | `core/moonshine-tts/src/utf8-utils.h:2` | `#define MOONSHINE_TTS_UTF8_UTILS_H` |
| `codepoint_is_unicode_word_neighbor_for_digits` | function | `core/moonshine-tts/src/utf8-utils.h:72` | `bool codepoint_is_unicode_word_neighbor_for_digits(char32_t cp);` |
| `digit_ascii_span_expandable_python_w` | function | `core/moonshine-tts/src/utf8-utils.h:81` | `bool digit_ascii_span_expandable_python_w(const std::string& text, size_t start_byte, size_t end_byte);` |
| `erase_utf8_substr` | function | `core/moonshine-tts/src/utf8-utils.h:27` | `inline void erase_utf8_substr(std::string& s, std::string_view sub)` |
| `is_ascii_whitespace` | function | `core/moonshine-tts/src/utf8-utils.h:45` | `inline bool is_ascii_whitespace(unsigned char c)` |
| `trim_ascii_ws_copy` | function | `core/moonshine-tts/src/utf8-utils.h:50` | `inline std::string trim_ascii_ws_copy(std::string_view s)` |
| `utf8_append_codepoint` | function | `core/moonshine-tts/src/utf8-utils.h:14` | `void utf8_append_codepoint(std::string& out, char32_t cp);` |
| `utf8_codepoint_at_index` | function | `core/moonshine-tts/src/utf8-utils.h:76` | `std::optional<char32_t> utf8_codepoint_at_index(const std::string& s, size_t byte_idx);` |
| `utf8_codepoint_before_index` | function | `core/moonshine-tts/src/utf8-utils.h:74` | `std::optional<char32_t> utf8_codepoint_before_index(const std::string& s, size_t byte_idx);` |
| `utf8_decode_at` | function | `core/moonshine-tts/src/utf8-utils.h:19` | `bool utf8_decode_at(const std::string& s, size_t i, char32_t& out_cp, size_t& out_len);` |
| `BiasNormJob` | struct | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:251` | `` |
| `BiasNormKernel` | struct | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:276` | `` |
| `BypassJob` | struct | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:303` | `` |
| `BypassKernel` | struct | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:322` | `` |
| `Compute` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:100` | `void Compute(OrtKernelContext* context)` |
| `Compute` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:147` | `void Compute(OrtKernelContext* context)` |
| `Compute` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:205` | `void Compute(OrtKernelContext* context)` |
| `Compute` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:277` | `void Compute(OrtKernelContext* context)` |
| `Compute` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:323` | `void Compute(OrtKernelContext* context)` |
| `ComputeBiasNormRow` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:259` | `void ComputeBiasNormRow(void* user_data, size_t r)` |
| `ComputeBypassRow` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:311` | `void ComputeBypassRow(void* user_data, size_t r)` |
| `ComputeConvRow` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:184` | `void ComputeConvRow(void* user_data, size_t row)` |
| `ComputeGluRow` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:132` | `void ComputeGluRow(void* user_data, size_t r)` |
| `ComputeTile` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:78` | `void ComputeTile(void* user_data, size_t idx)` |
| `CreateKernel` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:350` | `void* CreateKernel(const OrtApi& /*api*/,                      const OrtKernelInfo* /*info*/) const` |
| `CreateKernel` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:366` | `void* CreateKernel(const OrtApi& /*api*/,                      const OrtKernelInfo* /*info*/) const` |
| `CreateKernel` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:382` | `void* CreateKernel(const OrtApi& /*api*/,                      const OrtKernelInfo* /*info*/) const` |
| `CreateKernel` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:399` | `void* CreateKernel(const OrtApi& /*api*/,                      const OrtKernelInfo* /*info*/) const` |
| `CreateKernel` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:415` | `void* CreateKernel(const OrtApi& /*api*/,                      const OrtKernelInfo* /*info*/) const` |
| `CreateKernel` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:431` | `void* CreateKernel(const OrtApi& /*api*/,                      const OrtKernelInfo* /*info*/) const` |
| `DepthwiseConvKernel` | struct | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:204` | `` |
| `DwJob` | struct | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:176` | `` |
| `GetInputType` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:356` | `ONNXTensorElementDataType GetInputType(size_t /*index*/) const` |
| `GetInputType` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:372` | `ONNXTensorElementDataType GetInputType(size_t /*index*/) const` |
| `GetInputType` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:388` | `ONNXTensorElementDataType GetInputType(size_t /*index*/) const` |
| `GetInputType` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:405` | `ONNXTensorElementDataType GetInputType(size_t /*index*/) const` |
| `GetInputType` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:421` | `ONNXTensorElementDataType GetInputType(size_t /*index*/) const` |
| `GetInputType` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:437` | `ONNXTensorElementDataType GetInputType(size_t /*index*/) const` |
| `GetInputTypeCount` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:355` | `size_t GetInputTypeCount() const` |
| `GetInputTypeCount` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:371` | `size_t GetInputTypeCount() const` |
| `GetInputTypeCount` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:387` | `size_t GetInputTypeCount() const` |
| `GetInputTypeCount` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:404` | `size_t GetInputTypeCount() const` |
| `GetInputTypeCount` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:420` | `size_t GetInputTypeCount() const` |
| `GetInputTypeCount` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:436` | `size_t GetInputTypeCount() const` |
| `GetName` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:354` | `const char* GetName() const` |
| `GetName` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:370` | `const char* GetName() const` |
| `GetName` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:386` | `const char* GetName() const` |
| `GetName` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:403` | `const char* GetName() const` |
| `GetName` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:419` | `const char* GetName() const` |
| `GetName` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:435` | `const char* GetName() const` |
| `GetOutputType` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:360` | `ONNXTensorElementDataType GetOutputType(size_t /*index*/) const` |
| `GetOutputType` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:376` | `ONNXTensorElementDataType GetOutputType(size_t /*index*/) const` |
| `GetOutputType` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:392` | `ONNXTensorElementDataType GetOutputType(size_t /*index*/) const` |
| `GetOutputType` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:409` | `ONNXTensorElementDataType GetOutputType(size_t /*index*/) const` |
| `GetOutputType` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:425` | `ONNXTensorElementDataType GetOutputType(size_t /*index*/) const` |
| `GetOutputType` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:441` | `ONNXTensorElementDataType GetOutputType(size_t /*index*/) const` |
| `GetOutputTypeCount` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:359` | `size_t GetOutputTypeCount() const` |
| `GetOutputTypeCount` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:375` | `size_t GetOutputTypeCount() const` |
| `GetOutputTypeCount` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:391` | `size_t GetOutputTypeCount() const` |
| `GetOutputTypeCount` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:408` | `size_t GetOutputTypeCount() const` |
| `GetOutputTypeCount` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:424` | `size_t GetOutputTypeCount() const` |
| `GetOutputTypeCount` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:440` | `size_t GetOutputTypeCount() const` |
| `GluJob` | struct | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:126` | `` |
| `GluKernel` | struct | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:146` | `` |
| `SigmoidScalar` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:124` | `inline float SigmoidScalar(float v)` |
| `SoftplusPoly` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:52` | `inline float SoftplusPoly(float z)` |
| `SwooshJob` | struct | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:70` | `` |
| `SwooshKernel` | struct | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:95` | `` |
| `SwooshKernel` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:96` | `explicit SwooshKernel(bool is_left)       : offset_(is_left ? kLeftOffset : kRightOffset),       ...` |
| `wpacked` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:230` | `std::vector<float> wpacked(static_cast<size_t>(K * C));` |
| `zipvoice_domain` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:457` | `Ort::CustomOpDomain& zipvoice_domain()` |
| `zipvoice_register_custom_ops` | function | `core/moonshine-tts/src/zipvoice-custom-ops.cpp:473` | `void zipvoice_register_custom_ops(Ort::SessionOptions& opts)` |
| `MOONSHINE_TTS_ZIPVOICE_CUSTOM_OPS_H` | macro | `core/moonshine-tts/src/zipvoice-custom-ops.h:2` | `#define MOONSHINE_TTS_ZIPVOICE_CUSTOM_OPS_H` |
| `zipvoice_register_custom_ops` | function | `core/moonshine-tts/src/zipvoice-custom-ops.h:15` | `void zipvoice_register_custom_ops(Ort::SessionOptions& opts);` |
| `VocosFbank` | function | `core/moonshine-tts/src/zipvoice-mel.cpp:81` | `VocosFbank::VocosFbank()` |
| `all_freqs` | function | `core/moonshine-tts/src/zipvoice-mel.cpp:93` | `std::vector<double> all_freqs(static_cast<size_t>(n_freqs));` |
| `extract` | function | `core/moonshine-tts/src/zipvoice-mel.cpp:136` | `std::vector<float> VocosFbank::extract(const std::vector<float>& samples,                        ...` |
| `f_diff` | function | `core/moonshine-tts/src/zipvoice-mel.cpp:106` | `std::vector<double> f_diff(static_cast<size_t>(kNMels + 1));` |
| `f_pts` | function | `core/moonshine-tts/src/zipvoice-mel.cpp:100` | `std::vector<double> f_pts(static_cast<size_t>(kNMels + 2));` |
| `fft_radix2` | function | `core/moonshine-tts/src/zipvoice-mel.cpp:21` | `void fft_radix2(std::vector<double>& re, std::vector<double>& im)` |
| `hz_to_bin_count` | function | `core/moonshine-tts/src/zipvoice-mel.cpp:12` | `int hz_to_bin_count(int n_fft)` |
| `hz_to_mel_htk` | function | `core/moonshine-tts/src/zipvoice-mel.cpp:14` | `double hz_to_mel_htk(double f)` |
| `im` | function | `core/moonshine-tts/src/zipvoice-mel.cpp:152` | `std::vector<double> im(static_cast<size_t>(kNFft));` |
| `mag` | function | `core/moonshine-tts/src/zipvoice-mel.cpp:153` | `std::vector<double> mag(static_cast<size_t>(n_freqs));` |
| `mel_to_hz_htk` | function | `core/moonshine-tts/src/zipvoice-mel.cpp:15` | `double mel_to_hz_htk(double m)` |
| `num_frames_for` | function | `core/moonshine-tts/src/zipvoice-mel.cpp:132` | `int VocosFbank::num_frames_for(size_t num_samples)` |
| `out` | function | `core/moonshine-tts/src/zipvoice-mel.cpp:145` | `std::vector<float> out( static_cast<size_t>(frames) * static_cast<size_t>(kNMels), 0.F);` |
| `re` | function | `core/moonshine-tts/src/zipvoice-mel.cpp:151` | `std::vector<double> re(static_cast<size_t>(kNFft));` |
| `reflect_index` | function | `core/moonshine-tts/src/zipvoice-mel.cpp:64` | `size_t reflect_index(long idx, long len)` |
| `MOONSHINE_TTS_ZIPVOICE_MEL_H` | macro | `core/moonshine-tts/src/zipvoice-mel.h:2` | `#define MOONSHINE_TTS_ZIPVOICE_MEL_H` |
| `VocosFbank` | class | `core/moonshine-tts/src/zipvoice-mel.h:16` | `` |
| `extract` | function | `core/moonshine-tts/src/zipvoice-mel.h:32` | `std::vector<float> extract(const std::vector<float>& samples, int* out_frames) const;` |
| `num_frames_for` | function | `core/moonshine-tts/src/zipvoice-mel.h:27` | `static int num_frames_for(size_t num_samples);` |
| `Impl` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:306` | `explicit Impl(const ZipVoiceTTSOptions& opt)` |
| `Run` | struct | `core/moonshine-tts/src/zipvoice-tts.cpp:791` | `` |
| `ZipVoiceTTS` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:729` | `ZipVoiceTTS::ZipVoiceTTS(const ZipVoiceTTSOptions& opt)     : impl_(std::make_unique<Impl>(opt))` |
| `chunk_target_ids` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:601` | `std::vector<std::vector<int64_t>> chunk_target_ids(       const std::vector<int64_t>& ids)` |
| `cross_fade_concat` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:651` | `static std::vector<float> cross_fade_concat(       const std::vector<std::vector<float>>& chunks,...` |
| `dist` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:503` | `std::normal_distribution<float> dist(0.F, 1.F);` |
| `env` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:764` | `std::vector<float> env(wav.size(), 0.F);` |
| `get_time_steps` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:130` | `std::vector<float> get_time_steps(int num_step, float t_shift)` |
| `id_str` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:159` | `const std::string id_str(data + tab + 1, data + content_end);` |
| `ipa_text_to_token_ids` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:284` | `std::vector<int64_t> ipa_text_to_token_ids(const std::string& text)` |
| `ipa_to_token_ids` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:289` | `std::vector<int64_t> ipa_to_token_ids(const std::string& ipa)` |
| `k` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:225` | `const std::string k(key);` |
| `load_asset_bytes` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:256` | `std::vector<uint8_t> load_asset_bytes(std::string_view key)` |
| `load_session` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:218` | `Ort::Session load_session(std::string_view key, bool register_custom_ops,                        ...` |
| `mel` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:570` | `std::vector<float> mel(static_cast<size_t>(gen_frames) * feat);` |
| `normalize_audio` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:434` | `bool normalize_audio() const` |
| `normalize_audio` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:737` | `bool ZipVoiceTTS::normalize_audio() const` |
| `normalize_lang_key` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:34` | `std::string normalize_lang_key(std::string_view raw)` |
| `out` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:108` | `std::vector<float> out(wav.begin() + static_cast<std::ptrdiff_t>(start), wav.begin() +...` |
| `output_volume` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:436` | `float output_volume() const` |
| `output_volume` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:741` | `float ZipVoiceTTS::output_volume() const` |
| `pred` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:558` | `std::vector<float> pred(static_cast<size_t>(gen_frames) * feat);` |
| `resample_linear` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:60` | `std::vector<float> resample_linear(const std::vector<float>& x, int src_sr,                      ...` |
| `resolve_zipvoice_lang` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:49` | `void resolve_zipvoice_lang(const std::string& lang, std::string& g2p_dialect,                    ...` |
| `rms_of` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:117` | `float rms_of(const std::vector<float>& x)` |
| `run_text_encoder` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:441` | `std::vector<float> run_text_encoder(const std::vector<int64_t>& tokens,                          ...` |
| `run_vocoder` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:566` | `std::vector<float> run_vocoder(const std::vector<float>& pred,                                  i...` |
| `sample_chunk` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:489` | `std::vector<float> sample_chunk(const std::vector<int64_t>& tokens,                              ...` |
| `set_normalize_audio` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:435` | `void set_normalize_audio(bool on)` |
| `set_normalize_audio` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:738` | `void ZipVoiceTTS::set_normalize_audio(bool on)` |
| `set_output_volume` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:437` | `void set_output_volume(float v)` |
| `set_output_volume` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:742` | `void ZipVoiceTTS::set_output_volume(float volume)` |
| `set_speed` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:427` | `void set_speed(double s)` |
| `set_speed` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:735` | `void ZipVoiceTTS::set_speed(double speed)` |
| `speech_condition` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:508` | `std::vector<float> speech_condition(total, 0.F);` |
| `speed` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:426` | `double speed() const` |
| `speed` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:736` | `double ZipVoiceTTS::speed() const` |
| `synthesize` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:691` | `std::vector<float> synthesize(std::string_view text)` |
| `synthesize` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:746` | `std::vector<float> ZipVoiceTTS::synthesize(std::string_view text)` |
| `synthesize_from_ipa` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:695` | `std::vector<float> synthesize_from_ipa(std::string_view ipa)` |
| `synthesize_from_ipa` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:750` | `std::vector<float> ZipVoiceTTS::synthesize_from_ipa(std::string_view ipa)` |
| `synthesize_from_token_ids` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:699` | `std::vector<float> synthesize_from_token_ids(std::vector<int64_t> ids)` |
| `token` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:158` | `const std::string token(data + i, data + tab);` |
| `trim_edge_silence` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:87` | `std::vector<float> trim_edge_silence(const std::vector<float>& wav,                              ...` |
| `ts` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:131` | `std::vector<float> ts(static_cast<size_t>(num_step + 1));` |
| `wav` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:591` | `std::vector<float> wav(n);` |
| `x` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:501` | `std::vector<float> x(total);` |
| `y` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:69` | `std::vector<float> y(n_out);` |
| `zipvoice_compress_long_pauses` | function | `core/moonshine-tts/src/zipvoice-tts.cpp:754` | `std::vector<float> zipvoice_compress_long_pauses(const std::vector<float>& wav,                  ...` |
| `Impl` | struct | `core/moonshine-tts/src/zipvoice-tts.h:93` | `` |
| `MOONSHINE_TTS_ZIPVOICE_TTS_H` | macro | `core/moonshine-tts/src/zipvoice-tts.h:2` | `#define MOONSHINE_TTS_ZIPVOICE_TTS_H` |
| `ZipVoiceTTS` | class | `core/moonshine-tts/src/zipvoice-tts.h:65` | `` |
| `ZipVoiceTTSOptions` | struct | `core/moonshine-tts/src/zipvoice-tts.h:20` | `` |
| `normalize_audio` | function | `core/moonshine-tts/src/zipvoice-tts.h:78` | `bool normalize_audio() const;` |
| `output_volume` | function | `core/moonshine-tts/src/zipvoice-tts.h:80` | `float output_volume() const;` |
| `set_normalize_audio` | function | `core/moonshine-tts/src/zipvoice-tts.h:79` | `void set_normalize_audio(bool on);` |
| `set_output_volume` | function | `core/moonshine-tts/src/zipvoice-tts.h:81` | `void set_output_volume(float volume);` |
| `set_speed` | function | `core/moonshine-tts/src/zipvoice-tts.h:76` | `void set_speed(double speed);` |
| `speed` | function | `core/moonshine-tts/src/zipvoice-tts.h:77` | `double speed() const;` |
| `synthesize` | function | `core/moonshine-tts/src/zipvoice-tts.h:86` | `std::vector<float> synthesize(std::string_view text);` |
| `synthesize_from_ipa` | function | `core/moonshine-tts/src/zipvoice-tts.h:90` | `std::vector<float> synthesize_from_ipa(std::string_view ipa);` |
| `zipvoice_compress_long_pauses` | function | `core/moonshine-tts/src/zipvoice-tts.h:100` | `std::vector<float> zipvoice_compress_long_pauses(const std::vector<float>& wav, int sample_rate, float...` |
| `out` | function | `core/moonshine-tts/src/zipvoice-voices.cpp:20` | `std::vector<float> out(voice.num_samples);` |
| `zipvoice_builtin_voice_pcm_to_float` | function | `core/moonshine-tts/src/zipvoice-voices.cpp:18` | `std::vector<float> zipvoice_builtin_voice_pcm_to_float(     const ZipVoiceBuiltinVoice& voice)` |
| `zipvoice_find_builtin_voice` | function | `core/moonshine-tts/src/zipvoice-voices.cpp:7` | `const ZipVoiceBuiltinVoice* zipvoice_find_builtin_voice(std::string_view id)` |
| `MOONSHINE_TTS_ZIPVOICE_VOICES_H` | macro | `core/moonshine-tts/src/zipvoice-voices.h:2` | `#define MOONSHINE_TTS_ZIPVOICE_VOICES_H` |
| `ZipVoiceBuiltinVoice` | struct | `core/moonshine-tts/src/zipvoice-voices.h:17` | `` |
| `zipvoice_builtin_voice_pcm_to_float` | function | `core/moonshine-tts/src/zipvoice-voices.h:38` | `std::vector<float> zipvoice_builtin_voice_pcm_to_float( const ZipVoiceBuiltinVoice& voice);` |
| `zipvoice_builtin_voices` | function | `core/moonshine-tts/src/zipvoice-voices.h:30` | `const ZipVoiceBuiltinVoice* zipvoice_builtin_voices(size_t* count);` |
| `zipvoice_find_builtin_voice` | function | `core/moonshine-tts/src/zipvoice-voices.h:34` | `const ZipVoiceBuiltinVoice* zipvoice_find_builtin_voice(std::string_view id);` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/arabic-rule-g2p-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/arabic-rule-g2p-test.cpp:9` | `TEST_CASE(     "arabic rule g2p: first 100 wiki lines match reference IPA when assets and "     "...` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/chinese-rule-g2p-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/chinese-rule-g2p-test.cpp:33` | `TEST_CASE("chinese: dialect_resolves_to_chinese_rules")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/chinese-rule-g2p-test.cpp:44` | `TEST_CASE(     "chinese: lexicon lookup and Arabic numeral expansion via per-char Han "     "IPA")` |
| `make_temp_tsv` | function | `core/moonshine-tts/tests/chinese-rule-g2p-test.cpp:21` | `std::filesystem::path make_temp_tsv(const char* contents)` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/chinese-tok-pos-onnx-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/chinese-tok-pos-onnx-test.cpp:10` | `TEST_CASE("chinese tok pos: single sentence matches reference file")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/chinese-tok-pos-onnx-test.cpp:27` | `TEST_CASE(     "chinese tok pos: first 100 wiki lines match reference when assets and "     "gold...` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/cmudict-tsv-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/cmudict-tsv-test.cpp:11` | `TEST_CASE("cmudict-tsv load and lookup")` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp:29` | `TEST_CASE("dutch: lowercase homograph overrides capitalized")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp:38` | `TEST_CASE(     "dutch: lexicon stress not shifted by vocoder (unlike German policy)")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp:50` | `TEST_CASE("dutch: rule IPA gets vocoder stress when enabled")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp:59` | `TEST_CASE("dutch: normalize_ipa_stress_for_vocoder idempotent")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp:70` | `TEST_CASE("dutch: dialect_resolves_to_dutch_rules")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp:79` | `TEST_CASE("dutch: optional real dict fiets matches Python when data present")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp:93` | `TEST_CASE(     "dutch: wiki-text first 100 lines match reference IPA when data and golden "     "...` |
| `make_temp_tsv` | function | `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp:17` | `std::filesystem::path make_temp_tsv(const char* contents)` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/english-hand-oov-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/english-hand-oov-test.cpp:13` | `TEST_CASE("english_number_token_ipa")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/english-hand-oov-test.cpp:20` | `TEST_CASE("english_hand_oov_rules_ipa nonempty")` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/english-rule-g2p-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/english-rule-g2p-test.cpp:22` | `TEST_CASE("english: dialect_resolves_to_english_rules")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/english-rule-g2p-test.cpp:38` | `TEST_CASE("english: tomato heteronym picks US vs British by dialect flag")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/english-rule-g2p-test.cpp:51` | `TEST_CASE(     "english: wiki-text first 100 lines match reference IPA when data and "     "golde...` |
| `resolve_en_dict` | function | `core/moonshine-tts/tests/english-rule-g2p-test.cpp:15` | `std::filesystem::path resolve_en_dict()` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/file-information-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/file-information-test.cpp:11` | `TEST_CASE("FileInformation default memory fields")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/file-information-test.cpp:18` | `TEST_CASE("FileInformationMap set_path and contains")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/file-information-test.cpp:28` | `TEST_CASE("FileInformationMap erase_key")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/file-information-test.cpp:35` | `TEST_CASE("FileInformationMap::parse_file_list")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/file-information-test.cpp:60` | `TEST_CASE("FileInformationMap::parse_file_list null key_list throws")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/file-information-test.cpp:66` | `TEST_CASE("FileInformationMap::parse_file_list memory size mismatch throws")` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/french-rule-g2p-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/french-rule-g2p-test.cpp:43` | `TEST_CASE("french: dialect_resolves_to_french_rules")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/french-rule-g2p-test.cpp:52` | `TEST_CASE("french: ensure_french_nuclear_stress")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/french-rule-g2p-test.cpp:58` | `TEST_CASE("french: liaison les amis" * doctest::skip(!french_dict_present()))` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/french-rule-g2p-test.cpp:70` | `TEST_CASE("french: En 1891 cardinal expansion" *           doctest::skip(!french_dict_present()))` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/french-rule-g2p-test.cpp:83` | `TEST_CASE("french: punctuation keeps space before next word" *           doctest::skip(!french_di...` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/french-rule-g2p-test.cpp:94` | `TEST_CASE(     "french: hyphenated OOV allez-vous matches Python (UTF-8 trim + stress)" *     doc...` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/french-rule-g2p-test.cpp:105` | `TEST_CASE("french: uppercase accented letters in words (Saint-Étienne)" *           doctest::skip...` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/french-rule-g2p-test.cpp:115` | `TEST_CASE(     "french: wiki-text first 100 lines match reference IPA when data and "     "golden...` |
| `french_dict_present` | function | `core/moonshine-tts/tests/french-rule-g2p-test.cpp:36` | `bool french_dict_present()` |
| `strip_stress` | function | `core/moonshine-tts/tests/french-rule-g2p-test.cpp:16` | `std::string strip_stress(std::string s)` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/german-rule-g2p-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/german-rule-g2p-test.cpp:29` | `TEST_CASE("german: lowercase homograph overrides capitalized")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/german-rule-g2p-test.cpp:38` | `TEST_CASE(     "german: lexicon entry with syllable-initial stress gets vocoder shift")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/german-rule-g2p-test.cpp:46` | `TEST_CASE(     "german: syllable-initial stress preserved when vocoder_stress false")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/german-rule-g2p-test.cpp:56` | `TEST_CASE("german: OOV rules machen")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/german-rule-g2p-test.cpp:68` | `TEST_CASE("german: normalize_ipa_stress_for_vocoder idempotent")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/german-rule-g2p-test.cpp:76` | `TEST_CASE("german: dialect_resolves_to_german_rules")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/german-rule-g2p-test.cpp:85` | `TEST_CASE("german: text token preserves comma")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/german-rule-g2p-test.cpp:93` | `TEST_CASE(     "german: Im Jahr 1891 matches reference IPA when data and golden exist")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/german-rule-g2p-test.cpp:109` | `TEST_CASE(     "german: wiki-text first 100 lines match reference IPA when data and "     "golden...` |
| `make_temp_tsv` | function | `core/moonshine-tts/tests/german-rule-g2p-test.cpp:17` | `std::filesystem::path make_temp_tsv(const char* contents)` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/heteronym-context-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/heteronym-context-test.cpp:10` | `TEST_CASE("heteronym_centered_context_window_cells short pad")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/heteronym-context-test.cpp:20` | `TEST_CASE("heteronym_centered_context_window_cells crop")` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/hindi-rule-g2p-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/hindi-rule-g2p-test.cpp:37` | `TEST_CASE("hindi: dialect_resolves_to_hindi_rules")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/hindi-rule-g2p-test.cpp:45` | `TEST_CASE("hindi: कमल and मैं match reference IPA when golden exists")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/hindi-rule-g2p-test.cpp:60` | `TEST_CASE("hindi: expand_cardinal_digits_to_hindi_words")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/hindi-rule-g2p-test.cpp:66` | `TEST_CASE(     "hindi: wiki-text first 100 lines match reference IPA when data and golden "     "...` |
| `check_wiki_parity` | function | `core/moonshine-tts/tests/hindi-rule-g2p-test.cpp:17` | `void check_wiki_parity(const std::filesystem::path& wiki,                        const std::files...` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:10` | `TEST_CASE("levenshtein_distance")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:17` | `TEST_CASE("pick_closest_cmudict_ipa single")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:22` | `TEST_CASE("match_prediction_to_cmudict_ipa")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:29` | `TEST_CASE("normalize_g2p_ipa_for_piper_engines")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:45` | `TEST_CASE("repair_ascii_c_combining_cedilla_to_ccedilla_utf8")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:57` | `TEST_CASE("normalize_g2p_ipa_for_piper NFC plus shared rules")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:66` | `TEST_CASE("coerce_unknown_ipa_chars_to_piper_inventory toy map")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:78` | `TEST_CASE("ipa_to_piper_ready without coercion")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:89` | `TEST_CASE("normalize_g2p_ipa_for_piper Korean rule IPA toward eSpeak-ng")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:111` | `TEST_CASE("normalize_russian_ipa_piper_style")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:167` | `TEST_CASE("normalize_german_ipa_piper_style")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:190` | `TEST_CASE("normalize_g2p_ipa_for_piper German applies piper-style pass")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:198` | `TEST_CASE("normalize_chinese_ipa_piper_style full pipeline single syllables")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:223` | `TEST_CASE("normalize_chinese_ipa_piper_style retroflexes")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:240` | `TEST_CASE("normalize_chinese_ipa_piper_style dental sibilants")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:247` | `TEST_CASE("normalize_chinese_ipa_piper_style velar fricative")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:254` | `TEST_CASE("normalize_chinese_ipa_piper_style er/erhua")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:261` | `TEST_CASE("normalize_chinese_ipa_piper_style mid vowel")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:274` | `TEST_CASE("normalize_chinese_ipa_piper_style -ong and -uo finals")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:287` | `TEST_CASE("normalize_chinese_ipa_piper_style ü-finals")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:301` | `TEST_CASE(     "normalize_chinese_ipa_piper_style tone repositioning before nasals")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:321` | `TEST_CASE("normalize_chinese_ipa_piper_style aspiration")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:334` | `TEST_CASE("normalize_g2p_ipa_for_piper Chinese wired up for zh keys")` |
| `expected` | function | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:337` | `const std::string expected( "m\xcb\x88" "a5");` |
| `kBar` | function | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:168` | `static const std::string kBar("\xcd\xa1");` |
| `ma_in` | function | `core/moonshine-tts/tests/ipa-postprocess-test.cpp:336` | `const std::string ma_in("ma\xcb\xa5\xcb\xa5");` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/italian-rule-g2p-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/italian-rule-g2p-test.cpp:29` | `TEST_CASE("italian: dialect_resolves_to_italian_rules")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/italian-rule-g2p-test.cpp:38` | `TEST_CASE("italian: lowercase homograph overrides capitalized")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/italian-rule-g2p-test.cpp:47` | `TEST_CASE("italian: lexicon stress not shifted by vocoder")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/italian-rule-g2p-test.cpp:56` | `TEST_CASE("italian: c'è matches reference IPA when data and golden exist")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/italian-rule-g2p-test.cpp:74` | `TEST_CASE(     "italian: wiki-text first 100 lines match reference IPA when data and "     "golde...` |
| `make_temp_tsv` | function | `core/moonshine-tts/tests/italian-rule-g2p-test.cpp:17` | `std::filesystem::path make_temp_tsv(const char* contents)` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/japanese-onnx-g2p-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/japanese-onnx-g2p-test.cpp:10` | `TEST_CASE(     "japanese onnx g2p: first 100 wiki IPA lines match reference when assets "     "an...` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/japanese-tok-pos-onnx-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/japanese-tok-pos-onnx-test.cpp:10` | `TEST_CASE("japanese tok pos: single sentence matches reference file")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/japanese-tok-pos-onnx-test.cpp:28` | `TEST_CASE(     "japanese tok pos: long input is split and does not exceed model length")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/japanese-tok-pos-onnx-test.cpp:48` | `TEST_CASE(     "japanese tok pos: first 100 wiki lines match reference when assets and "     "gol...` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/json-config-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/json-config-test.cpp:11` | `TEST_CASE("load_oov_tables from onnx-config.json")` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/korean-rule-g2p-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/korean-rule-g2p-test.cpp:25` | `TEST_CASE("korean: dialect_resolves_to_korean_rules")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/korean-rule-g2p-test.cpp:34` | `TEST_CASE(     "korean: normalize strips all combining marks including tense and "     "unreleased")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/korean-rule-g2p-test.cpp:67` | `TEST_CASE("korean: int_to_sino_korean_hangul")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/korean-rule-g2p-test.cpp:79` | `TEST_CASE("korean: korean_reading_fragments_from_ascii_numeral_token")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/korean-rule-g2p-test.cpp:103` | `TEST_CASE("korean: G2P examples with data/ko/dict.tsv")` |
| `ko_dict_path` | function | `core/moonshine-tts/tests/korean-rule-g2p-test.cpp:19` | `std::filesystem::path ko_dict_path()` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/korean-tok-pos-onnx-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/korean-tok-pos-onnx-test.cpp:10` | `TEST_CASE("korean tok pos: single sentence matches reference file")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/korean-tok-pos-onnx-test.cpp:27` | `TEST_CASE(     "korean tok pos: first 100 wiki lines match reference when assets and "     "golde...` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/moonshine-g2p-options-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/moonshine-g2p-options-test.cpp:19` | `TEST_CASE("MoonshineG2POptions default constructor seeds canonical file keys")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/moonshine-g2p-options-test.cpp:35` | `TEST_CASE(     "MoonshineG2POptions relative_asset_path falls back when key absent")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/moonshine-g2p-options-test.cpp:43` | `TEST_CASE("MoonshineG2POptions parse_options rejects unknown keys")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/moonshine-g2p-options-test.cpp:49` | `TEST_CASE("MoonshineG2POptions parse_options accepts every known option")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/moonshine-g2p-options-test.cpp:125` | `TEST_CASE(     "MoonshineG2POptions parse_options empty path clears canonical entry")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/moonshine-g2p-options-test.cpp:134` | `TEST_CASE("MoonshineG2POptions option names are case-insensitive")` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/moonshine-tts-options-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/moonshine-tts-options-test.cpp:12` | `TEST_CASE("MoonshineTTSOptions parse_options ort_providers")` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/moonshine-tts-speed-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/moonshine-tts-speed-test.cpp:24` | `TEST_CASE(     "MoonshineTTS Kokoro: per-call speed changes duration and restores "     "default")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/moonshine-tts-speed-test.cpp:47` | `TEST_CASE("MoonshineTTS Piper: per-call speed reduces duration vs baseline")` |
| `bundled_tts_data_present` | function | `core/moonshine-tts/tests/moonshine-tts-speed-test.cpp:14` | `bool bundled_tts_data_present(const std::filesystem::path& root)` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/onnx-g2p-smoke-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/onnx-g2p-smoke-test.cpp:13` | `TEST_CASE(     "MoonshineG2P en_us rule-based when MOONSHINE_TTS_MODELS_ROOT is set")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/onnx-g2p-smoke-test.cpp:33` | `TEST_CASE("MoonshineG2P ja-JP when data/ja assets exist under repo")` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp:29` | `TEST_CASE("portuguese: dialect flags")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp:40` | `TEST_CASE("portuguese: lowercase homograph overrides capitalized")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp:49` | `TEST_CASE("portuguese: lexicon stress not shifted by vocoder")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp:58` | `TEST_CASE("portuguese: casa matches reference IPA when data and golden exist")` |

Next: [SYMBOLS_p7.md](SYMBOLS_p7.md)
