# Subsystem: core (page 3 of 3)
Previous: [KB_core_p2.md](KB_core_p2.md)

## core/moonshine-streaming-model.h
- Doc: Streaming model configuration (matches streaming_config.json)
- Layer: business_logic
- Language: h
- Symbols:
  - `MoonshineStreamingConfig` (struct, line 17)
  - `MoonshineStreamingState` (struct, line 35)
  - `MoonshineStreamingModel` (struct, line 72)
  - `reset` (function, line 69) `void reset(const MoonshineStreamingConfig &cfg);`
  - `load` (function, line 117) `int load(const char *model_dir, const char *tokenizer_path, int32_t model_type);`
  - `load_from_memory` (function, line 120) `int load_from_memory( const uint8_t *frontend_model_data, size_t frontend_model_data_size, const uint8_t...`
  - `load_from_assets` (function, line 130) `int load_from_assets(const char *model_dir, const char *tokenizer_path, int32_t model_type, AAssetManager...`
  - `transcribe` (function, line 135) `int transcribe(const float *input_audio_data, size_t input_audio_data_size, char **out_text);`
  - `process_audio_chunk` (function, line 139) `int process_audio_chunk(MoonshineStreamingState *state, const float *audio_chunk, size_t chunk_len, int *features_out);`
  - `encode` (function, line 143) `int encode(MoonshineStreamingState *state, bool is_final, int *new_frames_out);`
  - `decode_step` (function, line 147) `int decode_step(MoonshineStreamingState *state, int token, float *logits_out);`
  - `decode_full` (function, line 161) `int decode_full(MoonshineStreamingState *state, const int *speculative_tokens, int speculative_len, int...`
  - `decoder_reset` (function, line 164) `void decoder_reset(MoonshineStreamingState *state);`
  - `create_state` (function, line 167) `MoonshineStreamingState *create_state();`
  - `load_config` (function, line 173) `private: int load_config(const char *config_path);`
  - `load_config_from_string` (function, line 174) `int load_config_from_string(const std::string &json);`
  - `run_decoder_with_cross_kv` (function, line 177) `int run_decoder_with_cross_kv(MoonshineStreamingState *state, const std::vector<int64_t> &tokens, std::vector<float>...`
  - `compute_cross_kv` (function, line 182) `int compute_cross_kv(MoonshineStreamingState *state);`
  - `MOONSHINE_STREAMING_MODEL_H` (macro, line 2) `#define MOONSHINE_STREAMING_MODEL_H`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/ort-utils/moonshine-ort-allocator.h`, `core/word-alignment.h`
- Imported by: `core/moonshine-streaming-model.cpp`

## core/resampler-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `test_resample_audio` (function, line 13) `void test_resample_audio(const std::vector<float> &input_audio,
                         int32_t ...`
  - `TEST_CASE` (function, line 44) `TEST_CASE("resampler-test")`
  - `SUBCASE` (function, line 45) `SUBCASE("resample-audio")`
  - `max_element` (function, line 20) `*std::max_element(input_audio.begin(), input_audio.end());`
  - `min_element` (function, line 27) `*std::min_element(input_audio.begin(), input_audio.end());`
  - `wav_data_vector` (function, line 55) `const std::vector<float> wav_data_vector(wav_data, wav_data + wav_data_size);`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 9) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-utils/debug-utils.h`, `core/resampler.h`

## core/resampler.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `resample_audio` (function, line 5) `const std::vector<float> resample_audio(const std::vector<float> &audio,
                        ...`
  - `downsample_audio` (function, line 17) `const std::vector<float> downsample_audio(const std::vector<float> &audio,
                      ...`
  - `upsample_audio` (function, line 56) `const std::vector<float> upsample_audio(const std::vector<float> &audio,
                        ...`
  - `output_audio` (function, line 23) `std::vector<float> output_audio(output_audio_size);`
- Depends on: `core/moonshine-utils/debug-utils.h`, `core/resampler.h`

## core/resampler.h
- Layer: utility
- Language: h
- Symbols:
  - `resample_audio` (function, line 6) `const std::vector<float> resample_audio(const std::vector<float> &audio, float input_sample_rate, float...`
  - `downsample_audio` (function, line 10) `const std::vector<float> downsample_audio(const std::vector<float> &audio, float input_sample_rate, float...`
  - `upsample_audio` (function, line 14) `const std::vector<float> upsample_audio(const std::vector<float> &audio, float input_sample_rate, float...`
  - `RESAMPLER_H` (macro, line 2) `#define RESAMPLER_H`
- Imported by: `core/reliability/fuzz-resampler.cpp`, `core/resampler-test.cpp`, `core/resampler.cpp`, `core/voice-activity-detector.cpp`

## core/silero-vad.cpp
- Doc: init_engine_threads: Initializes threading settings.
- Layer: utility
- Language: cpp
- Symbols:
  - `init_onnx_env` (function, line 6) `void SileroVad::init_onnx_env()`
  - `init_engine_threads` (function, line 21) `void SileroVad::init_engine_threads(int inter_threads, int intra_threads)`
  - `SileroVad` (function, line 30) `SileroVad::SileroVad(int sample_rate, int windows_frame_size, float threshold,
                  ...`
  - `load_from_memory` (function, line 60) `int SileroVad::load_from_memory(const uint8_t *model_data,
                                size_t...`
  - `predict` (function, line 78) `void SileroVad::predict(const std::vector<float> &data_chunk,
                        float *out_...`
- Depends on: `core/ort-utils/ort-utils.h`, `core/silero-vad.h`

## core/silero-vad.h
- Doc: init_onnx_env: Initializes the common ONNX runtime environment (env, session_options...
- Layer: utility
- Language: h
- Symbols:
  - `SileroVad` (class, line 22)
  - `is_loaded` (function, line 85) `bool is_loaded() const`
  - `init_onnx_env` (function, line 68) `void init_onnx_env();`
  - `init_engine_threads` (function, line 71) `void init_engine_threads(int inter_threads, int intra_threads);`
  - `load_from_memory` (function, line 83) `int load_from_memory(const uint8_t *model_data, size_t model_data_size);`
  - `predict` (function, line 87) `void predict(const std::vector<float> &data_chunk, float *out_probability, int *out_flag);`
- Imported by: `core/silero-vad.cpp`, `core/voice-activity-detector.h`

## core/speaker-diarizer.cpp
- Doc: turn_overlap_seconds: Total seconds of overlap between the spans of two turn lists.
- Layer: utility
- Language: cpp
- Symbols:
  - `StreamState` (struct, line 43)
  - `turn_overlap_seconds` (function, line 17) `double turn_overlap_seconds(
    const std::vector<cppannote::StreamingDiarizationTurn> &a, int32...`
  - `Impl` (function, line 67) `explicit Impl(const SpeakerDiarizerOptions &options_in)
      : engine(), options(options_in)`
  - `session_config` (function, line 75) `cppannote::StreamingDiarizationConfig session_config() const`
  - `get_stream` (function, line 83) `StreamState &get_stream(int32_t stream_id)`
  - `allocate_stable_id` (function, line 92) `uint64_t allocate_stable_id()`
  - `map_snapshot_to_stable_ids` (function, line 102) `void map_snapshot_to_stable_ids(
      StreamState &state,
      const cppannote::StreamingDiariz...`
  - `sort` (function, line 135) `std::sort(candidates.begin(), candidates.end(),
              [](const auto &a, const auto &b)`
  - `SpeakerDiarizer` (function, line 171) `SpeakerDiarizer::SpeakerDiarizer(const SpeakerDiarizerOptions &options)
    : impl(std::make_uniq...`
  - `create_stream` (function, line 176) `int32_t SpeakerDiarizer::create_stream()`
  - `free_stream` (function, line 186) `void SpeakerDiarizer::free_stream(int32_t stream_id)`
  - `start_stream` (function, line 191) `void SpeakerDiarizer::start_stream(int32_t stream_id)`
  - `add_audio_to_stream` (function, line 201) `void SpeakerDiarizer::add_audio_to_stream(int32_t stream_id,
                                    ...`
  - `get_turns` (function, line 218) `std::vector<SpeakerTurn> SpeakerDiarizer::get_turns(int32_t stream_id)`
  - `finish_stream` (function, line 225) `std::vector<SpeakerTurn> SpeakerDiarizer::finish_stream(int32_t stream_id)`
  - `diarize` (function, line 236) `std::vector<SpeakerTurn> SpeakerDiarizer::diarize(const float *audio_data,
                      ...`
- Depends on: `core/cpp-annote/src/cpp-annote-engine.h`, `core/cpp-annote/src/cpp-annote-streaming.h`, `core/moonshine-utils/debug-utils.h`, `core/speaker-diarizer.h`

## core/speaker-diarizer.h
- Doc: One contiguous span of speech attributed to a single speaker on the stream timeline.
- Layer: utility
- Language: h
- Symbols:
  - `SpeakerTurn` (struct, line 10)
  - `SpeakerDiarizerOptions` (struct, line 24)
  - `Impl` (struct, line 74)
  - `SpeakerDiarizer` (class, line 42)
  - `create_stream` (function, line 51) `int32_t create_stream();`
  - `free_stream` (function, line 52) `void free_stream(int32_t stream_id);`
  - `start_stream` (function, line 53) `void start_stream(int32_t stream_id);`
  - `add_audio_to_stream` (function, line 58) `void add_audio_to_stream(int32_t stream_id, const float *audio_data, uint64_t audio_length, int32_t sample_rate);`
  - `SPEAKER_DIARIZER_H` (macro, line 2) `#define SPEAKER_DIARIZER_H`
- Imported by: `core/speaker-diarizer.cpp`

## core/spelling-fusion-data.cpp
- Layer: data_access
- Language: cpp
- Symbols:
  - `build_set` (function, line 28) `std::unordered_set<std::string> build_set(
    std::initializer_list<const char *> phrases)`
  - `upper_modifiers` (function, line 268) `const std::unordered_set<std::string> &upper_modifiers()`
  - `upper_modifiers_by_length` (function, line 281) `const std::vector<std::string> &upper_modifiers_by_length()`
  - `sort` (function, line 287) `std::sort(v.begin(), v.end(),
              [](const std::string &a, const std::string &b)`
  - `undo_words` (function, line 296) `const std::unordered_set<std::string> &undo_words()`
  - `clear_words` (function, line 309) `const std::unordered_set<std::string> &clear_words()`
  - `stop_words` (function, line 319) `const std::unordered_set<std::string> &stop_words()`
  - `default_weak_homonyms` (function, line 338) `const std::unordered_set<std::string> &default_weak_homonyms()`
  - `default_meta` (function, line 356) `const DefaultSpellingMeta &default_meta()`
- Depends on: `core/spelling-fusion-data.h`, `core/spelling-fusion.h`

## core/spelling-fusion-data.h
- Doc: Compiled-in tables for the spelling matcher.
- Layer: data_access
- Language: h
- Symbols:
  - `DefaultSpellingMeta` (struct, line 53)
  - `upper_modifiers` (function, line 27) `const std::unordered_set<std::string> &upper_modifiers();`
  - `upper_modifiers_by_length` (function, line 28) `const std::vector<std::string> &upper_modifiers_by_length();`
  - `undo_words` (function, line 32) `const std::unordered_set<std::string> &undo_words();`
  - `clear_words` (function, line 33) `const std::unordered_set<std::string> &clear_words();`
  - `stop_words` (function, line 34) `const std::unordered_set<std::string> &stop_words();`
  - `default_weak_homonyms` (function, line 40) `const std::unordered_set<std::string> &default_weak_homonyms();`
  - `default_meta` (function, line 60) `const DefaultSpellingMeta &default_meta();`
  - `SPELLING_FUSION_DATA_H` (macro, line 2) `#define SPELLING_FUSION_DATA_H`
- Imported by: `core/spelling-fusion-data.cpp`, `core/spelling-fusion-test.cpp`, `core/spelling-fusion.cpp`, `core/spelling-model.cpp`

## core/spelling-fusion-test.cpp
- Doc: char_match: Helper: shorthand for "matcher said this character".
- Layer: testing
- Language: cpp
- Symbols:
  - `char_match` (function, line 13) `SpellingMatch char_match(const std::string &c)`
  - `no_match` (function, line 21) `SpellingMatch no_match()`
  - `TEST_CASE` (function, line 25) `TEST_CASE("spelling-fusion: normalize")`
  - `TEST_CASE` (function, line 39) `TEST_CASE("spelling-fusion: matcher classifies plain letters")`
  - `TEST_CASE` (function, line 50) `TEST_CASE("spelling-fusion: matcher classifies NATO codewords")`
  - `TEST_CASE` (function, line 61) `TEST_CASE("spelling-fusion: matcher classifies digits")`
  - `TEST_CASE` (function, line 73) `TEST_CASE("spelling-fusion: matcher parses 10..1000 number words")`
  - `TEST_CASE` (function, line 85) `TEST_CASE("spelling-fusion: matcher applies upper-case modifier")`
  - `TEST_CASE` (function, line 94) `TEST_CASE("spelling-fusion: matcher recognizes speller patterns")`
  - `TEST_CASE` (function, line 103) `TEST_CASE("spelling-fusion: matcher classifies command words")`
  - `TEST_CASE` (function, line 114) `TEST_CASE("spelling-fusion: matcher classifies special characters")`
  - `TEST_CASE` (function, line 149) `TEST_CASE("spelling-fusion: weak-homonym detection")`
  - `TEST_CASE` (function, line 158) `TEST_CASE("spelling-fusion: fuse without prediction")`
  - `TEST_CASE` (function, line 166) `TEST_CASE("spelling-fusion: fuse drops unrecognized + no prediction")`
  - `TEST_CASE` (function, line 173) `TEST_CASE("spelling-fusion: fuse passes through command words")`
  - `TEST_CASE` (function, line 183) `TEST_CASE(
    "spelling-fusion: special-character match is preserved when the "
    "spelling mo...`
  - `TEST_CASE` (function, line 204) `TEST_CASE("spelling-fusion: weak-homonym demotion")`
  - `TEST_CASE` (function, line 225) `TEST_CASE("spelling-fusion: cross-class routing")`
  - `TEST_CASE` (function, line 238) `TEST_CASE("spelling-fusion: same-class disagreement uses threshold")`
  - `TEST_CASE` (function, line 251) `TEST_CASE("spelling-fusion: multi-digit ASR vs single-digit spelling")`
  - `TEST_CASE` (function, line 275) `TEST_CASE("spelling-fusion: agreement preserves matcher casing")`
  - `TEST_CASE` (function, line 284) `TEST_CASE("spelling-fusion: spelling-only when matcher misses")`
  - `TEST_CASE` (function, line 293) `TEST_CASE("spelling-fusion: data tables are non-empty")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 7) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/spelling-fusion-data.h`, `core/spelling-fusion.h`

## core/spelling-fusion.cpp
- Doc: consume_curly_quote: Try to consume a 3-byte UTF-8 curly quote starting at ``input[i]``.
- Layer: utility
- Language: cpp
- Symbols:
  - `is_ascii_drop` (function, line 25) `bool is_ascii_drop(char c)`
  - `is_ascii_letter` (function, line 35) `bool is_ascii_letter(char c)`
  - `ascii_to_lower` (function, line 39) `char ascii_to_lower(char c)`
  - `consume_curly_quote` (function, line 46) `size_t consume_curly_quote(const std::string &input, size_t i)`
  - `split_on_whitespace` (function, line 62) `std::vector<std::string> split_on_whitespace(const std::string &s)`
  - `parse_number_words` (function, line 108) `std::optional<int> parse_number_words(const std::string &text)`
  - `is_ascii_digit_string` (function, line 181) `bool is_ascii_digit_string(const std::string &s)`
  - `is_printable_ascii` (function, line 189) `bool is_printable_ascii(char c)`
  - `spelling_normalize` (function, line 195) `std::string spelling_normalize(const std::string &text)`
  - `SpellingMatcher` (function, line 234) `SpellingMatcher::SpellingMatcher()
    : lookup_(&spelling_fusion_data::lookup_table()),
      up...`
  - `classify` (function, line 244) `SpellingMatch SpellingMatcher::classify(const std::string &raw_text) const`
  - `is_weak_homonym` (function, line 300) `bool SpellingMatcher::is_weak_homonym(const std::string &raw_text) const`
  - `resolve` (function, line 305) `std::optional<std::string> SpellingMatcher::resolve(
    const std::string &text) const`
  - `resolve_spelled_letter` (function, line 326) `std::optional<std::string> SpellingMatcher::resolve_spelled_letter(
    const std::string &text) ...`
  - `string_is_letter` (function, line 373) `bool string_is_letter(const std::string &c)`
  - `string_is_digit` (function, line 381) `bool string_is_digit(const std::string &c)`
  - `single_char_is_letter` (function, line 389) `bool single_char_is_letter(const std::string &c)`
  - `apply_case` (function, line 393) `std::string apply_case(const std::string &ch, const std::string &hint)`
  - `fuse_default` (function, line 407) `FusedResult fuse_default(const std::string &raw_text,
                         const SpellingMatc...`
- Depends on: `core/spelling-fusion-data.h`, `core/spelling-fusion.h`

## core/spelling-fusion.h
- Doc: C++ port of the matcher / fusion logic from
- Layer: utility
- Language: h
- Symbols:
  - `SpellingMatch` (struct, line 34)
  - `SpellingPrediction` (struct, line 47)
  - `FusedResult` (struct, line 88)
  - `SpellingMatchType` (enum, line 26)
  - `SpellingMatchType` (class, line 26)
  - `SpellingMatcher` (class, line 53)
  - `is_character` (function, line 41) `bool is_character() const`
  - `is_recognized` (function, line 42) `bool is_recognized() const`
  - `is_character` (function, line 91) `bool is_character() const`
  - `is_weak_homonym` (function, line 66) `bool is_weak_homonym(const std::string &raw_text) const;`
  - `SPELLING_FUSION_H` (macro, line 2) `#define SPELLING_FUSION_H`
- Imported by: `core/spelling-fusion-data.cpp`, `core/spelling-fusion-test.cpp`, `core/spelling-fusion.cpp`, `core/spelling-model-test.cpp`, `core/spelling-model.h`

## core/spelling-model-test.cpp
- Doc: Clip: (label_dir, expected canonical char).
- Layer: business_logic
- Language: cpp
- Symbols:
  - `Clip` (struct, line 99)
  - `find_model_path` (function, line 21) `std::string find_model_path()`
  - `find_wav` (function, line 33) `std::string find_wav(const std::string &label, const std::string &filename)`
  - `read_file` (function, line 47) `std::vector<uint8_t> read_file(const std::string &path)`
  - `TEST_CASE` (function, line 60) `TEST_CASE("spelling-model: load from path")`
  - `TEST_CASE` (function, line 73) `TEST_CASE("spelling-model: load from memory")`
  - `TEST_CASE` (function, line 86) `TEST_CASE("spelling-model: predict on bundled clips")`
  - `TEST_CASE` (function, line 133) `TEST_CASE("spelling-model: invalid arguments are rejected")`
  - `buffer` (function, line 53) `std::vector<uint8_t> buffer(static_cast<size_t>(size));`
  - `dummy` (function, line 143) `std::vector<float> dummy(16000, 0.0f);`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 12) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-utils/debug-utils.h`, `core/spelling-fusion.h`, `core/spelling-model.h`

## core/spelling-model.cpp
- Doc: lookup_metadata: Read a single key from the model's custom_metadata_map, returning nullopt when...
- Layer: business_logic
- Language: cpp
- Symbols:
  - `lookup_metadata` (function, line 26) `std::optional<std::string> lookup_metadata(const OrtApi *ort_api,
                               ...`
  - `trim` (function, line 45) `std::string trim(const std::string &s)`
  - `parse_class_list_json` (function, line 59) `std::vector<std::string> parse_class_list_json(const std::string &raw)`
  - `SpellingModel` (function, line 95) `SpellingModel::SpellingModel(bool log_ort_run,
                             const std::vector<std...`
  - `initialize_session_options` (function, line 137) `void SpellingModel::initialize_session_options()`
  - `apply_default_metadata` (function, line 157) `void SpellingModel::apply_default_metadata()`
  - `load` (function, line 169) `int SpellingModel::load(const char *model_path)`
  - `load_from_memory` (function, line 177) `int SpellingModel::load_from_memory(const uint8_t *model_data,
                                  ...`
  - `populate_metadata_from_session` (function, line 186) `int SpellingModel::populate_metadata_from_session()`
  - `predict` (function, line 243) `int SpellingModel::predict(const float *audio, size_t audio_size,
                           int3...`
  - `clip` (function, line 260) `std::vector<float> clip(target_samples_, 0.0f);`
  - `probs` (function, line 307) `std::vector<float> probs(row_size);`
- Depends on: `core/moonshine-utils/debug-utils.h`, `core/ort-utils/moonshine-tensor-view.h`, `core/ort-utils/ort-utils.h`, `core/spelling-fusion-data.h`, `core/spelling-model.h`

## core/spelling-model.h
- Doc: Wraps the SpellingCNN ``.ort`` model.
- Layer: business_logic
- Language: h
- Symbols:
  - `SpellingModel` (class, line 24)
  - `sample_rate` (function, line 56) `int32_t sample_rate() const`
  - `clip_seconds` (function, line 57) `float clip_seconds() const`
  - `classes` (function, line 58) `const std::vector<std::string> &classes() const`
  - `load` (function, line 39) `int load(const char *model_path);`
  - `load_from_memory` (function, line 43) `int load_from_memory(const uint8_t *model_data, size_t model_data_size);`
  - `predict` (function, line 52) `int predict(const float *audio, size_t audio_size, int32_t sample_rate, SpellingPrediction *out_prediction);`
  - `initialize_session_options` (function, line 61) `private: void initialize_session_options();`
  - `populate_metadata_from_session` (function, line 62) `int populate_metadata_from_session();`
  - `apply_default_metadata` (function, line 63) `void apply_default_metadata();`
  - `SPELLING_MODEL_H` (macro, line 2) `#define SPELLING_MODEL_H`
- Depends on: `core/spelling-fusion.h`
- Imported by: `core/spelling-model-test.cpp`, `core/spelling-model.cpp`

## core/tts-repeated-memory-test.cpp
- Doc: Repeated-use memory regression test for the text-to-speech synthesizers.
- Layer: testing
- Language: cpp
- Symbols:
  - `EngineSpec` (struct, line 216)
  - `read_rss_kb` (function, line 54) `size_t read_rss_kb()`
  - `median` (function, line 90) `size_t median(std::vector<size_t> values)`
  - `env_size` (function, line 99) `size_t env_size(const char *name, size_t default_value)`
  - `detect_continual_growth` (function, line 117) `bool detect_continual_growth(const std::vector<size_t> &samples,
                             siz...`
  - `create_synth` (function, line 223) `int32_t create_synth(const EngineSpec &spec)`
  - `synth_once` (function, line 236) `bool synth_once(int32_t handle, size_t text_index)`
  - `reload_strict` (function, line 248) `bool reload_strict()`
  - `run_growth_phase` (function, line 259) `void run_growth_phase(const std::string &label, size_t iterations,
                      const st...`
  - `exercise_engine` (function, line 294) `void exercise_engine(const EngineSpec &spec)`
  - `run_growth_phase` (function, line 306) `run_growth_phase(
        std::string(spec.name) + " synth", synth_iterations,
        [handle](s...`
  - `run_growth_phase` (function, line 322) `run_growth_phase(
      std::string(spec.name) + " reload", reload_iterations,
      [&spec](size...`
  - `file_present` (function, line 339) `bool file_present(const fs::path &p)`
  - `kokoro_spec` (function, line 344) `std::optional<EngineSpec> kokoro_spec()`
  - `piper_spec` (function, line 355) `std::optional<EngineSpec> piper_spec()`
  - `zipvoice_spec` (function, line 389) `std::optional<EngineSpec> zipvoice_spec()`
  - `TEST_CASE` (function, line 407) `TEST_CASE("tts-repeated-memory-kokoro")`
  - `TEST_CASE` (function, line 416) `TEST_CASE("tts-repeated-memory-piper")`
  - `TEST_CASE` (function, line 426) `TEST_CASE("tts-repeated-memory-zipvoice")`
  - `discover_data_root` (function, line 439) `std::optional<fs::path> discover_data_root()`
  - `main` (function, line 464) `int main(int argc, char **argv)`
  - `DOCTEST_CONFIG_IMPLEMENT` (macro, line 27) `#define DOCTEST_CONFIG_IMPLEMENT`
- Depends on: `core/moonshine-c-api.h`

## core/voice-activity-detector-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 11) `TEST_CASE("voice-activity-detector-test")`
  - `SUBCASE` (function, line 15) `SUBCASE("vad-block")`
  - `SUBCASE` (function, line 54) `SUBCASE("vad-stream")`
  - `SUBCASE` (function, line 122) `SUBCASE("vad-threshold-0")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 8) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-utils/debug-utils.h`, `core/voice-activity-detector.h`

## core/voice-activity-detector.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `seconds_from_sample_count` (function, line 15) `float seconds_from_sample_count(size_t sample_count)`
  - `VoiceActivityDetector` (function, line 24) `VoiceActivityDetector::VoiceActivityDetector(float threshold,
                                   ...`
  - `start` (function, line 50) `void VoiceActivityDetector::start()`
  - `stop` (function, line 62) `void VoiceActivityDetector::stop()`
  - `process_audio` (function, line 69) `void VoiceActivityDetector::process_audio(const float *audio_data,
                              ...`
  - `clear_completed_segment_audio_data` (function, line 99) `void VoiceActivityDetector::clear_completed_segment_audio_data()`
  - `retained_segment_audio_byte_count` (function, line 107) `size_t VoiceActivityDetector::retained_segment_audio_byte_count() const`
  - `completed_segment_audio_byte_count` (function, line 115) `size_t VoiceActivityDetector::completed_segment_audio_byte_count() const`
  - `process_audio_chunk` (function, line 125) `void VoiceActivityDetector::process_audio_chunk(const float *audio_data,
                        ...`
  - `on_voice_start` (function, line 196) `void VoiceActivityDetector::on_voice_start()`
  - `on_voice_continuing` (function, line 210) `void VoiceActivityDetector::on_voice_continuing()`
  - `on_voice_end` (function, line 219) `void VoiceActivityDetector::on_voice_end()`
  - `to_string` (function, line 228) `std::string VoiceActivitySegment::to_string() const`
  - `to_string` (function, line 238) `std::string VoiceActivityDetector::to_string() const`
  - `input_audio_vector` (function, line 79) `std::vector<float> input_audio_vector(audio_data, audio_data + audio_data_size);`
  - `audio_vec` (function, line 136) `std::vector<float> audio_vec(audio_data, audio_data + audio_data_size);`
- Depends on: `core/moonshine-utils/debug-utils.h`, `core/resampler.h`, `core/voice-activity-detector.h`

## core/voice-activity-detector.h
- Layer: utility
- Language: h
- Symbols:
  - `VoiceActivitySegment` (struct, line 9)
  - `VoiceActivityDetector` (class, line 22)
  - `is_active` (function, line 53) `bool is_active() const`
  - `get_segments` (function, line 56) `const std::vector<VoiceActivitySegment> *get_segments() const`
  - `start` (function, line 51) `void start();`
  - `stop` (function, line 52) `void stop();`
  - `process_audio` (function, line 54) `void process_audio(const float *audio_data, size_t audio_data_size, int32_t sample_rate);`
  - `retained_segment_audio_byte_count` (function, line 59) `size_t retained_segment_audio_byte_count() const;`
  - `completed_segment_audio_byte_count` (function, line 60) `size_t completed_segment_audio_byte_count() const;`
  - `clear_completed_segment_audio_data` (function, line 61) `void clear_completed_segment_audio_data();`
  - `clear` (function, line 65) `private: void clear();`
  - `on_voice_start` (function, line 66) `void on_voice_start();`
  - `on_voice_end` (function, line 67) `void on_voice_end();`
  - `on_voice_continuing` (function, line 68) `void on_voice_continuing();`
  - `process_audio_chunk` (function, line 69) `void process_audio_chunk(const float *audio_data, size_t audio_data_size);`
  - `VOICE_ACTIVITY_DETECTOR_H` (macro, line 2) `#define VOICE_ACTIVITY_DETECTOR_H`
- Depends on: `core/silero-vad.h`
- Imported by: `core/voice-activity-detector-test.cpp`, `core/voice-activity-detector.cpp`

## core/word-alignment-benchmark.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `BenchResult` (struct, line 31)
  - `load_wav` (function, line 10) `static float* load_wav(const char* path, long* num_samples_out)`
  - `run_benchmark` (function, line 38) `static BenchResult run_benchmark(const char* model_path, const char* wav_path,
                  ...`
  - `main` (function, line 97) `int main(int argc, char** argv)`
- Depends on: `core/moonshine-c-api.h`, `core/moonshine-utils/file-utils.h`

## core/word-alignment-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 12) `TEST_CASE("word-timestamps")`
  - `SUBCASE` (function, line 13) `SUBCASE("non-streaming-transcribe-with-word-timestamps")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 9) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-c-api.h`, `core/moonshine-utils/debug-utils.h`

## core/word-alignment.cpp
- Doc: DTW (Dynamic Time Warping)
- Layer: utility
- Language: cpp
- Symbols:
  - `WordGroup` (struct, line 304)
  - `dtw` (function, line 12) `void dtw(const std::vector<float>& cost_matrix, int N, int M,
         std::vector<int>& text_ind...`
  - `compute_median` (function, line 93) `static float compute_median(std::vector<float>& window)`
  - `median_filter` (function, line 99) `void median_filter(std::vector<float>& data, int channels, int height,
                   int wid...`
  - `token_starts_new_word` (function, line 159) `static bool token_starts_new_word(BinTokenizer* tokenizer, int token_id)`
  - `decode_tokens` (function, line 174) `static std::string decode_tokens(BinTokenizer* tokenizer,
                                 const ...`
  - `align_words` (function, line 181) `std::vector<TranscriberWord> align_words(const float* cross_attention_data,
                     ...`
  - `D` (function, line 16) `std::vector<float> D((N + 1) * (M + 1), std::numeric_limits<float>::infinity());`
  - `trace` (function, line 22) `std::vector<int> trace(N * M, 0);`
  - `padded` (function, line 114) `std::vector<float> padded(padded_width);`
  - `window` (function, line 115) `std::vector<float> window(filter_width);`
  - `result_row` (function, line 116) `std::vector<float> result_row(width);`
  - `weights` (function, line 200) `std::vector<float> weights(total_size);`
  - `matrix` (function, line 250) `std::vector<float> matrix(n_steps * encoder_frames, 0.0f);`
  - `neg_matrix` (function, line 270) `std::vector<float> neg_matrix(matrix.size());`
- Depends on: `core/word-alignment.h`

## core/word-alignment.h
- Doc: dtw: Dynamic Time Warping on a cost matrix [N x M] Returns aligned (text_indices, time_indices)...
- Layer: utility
- Language: h
- Symbols:
  - `TranscriberWord` (struct, line 9)
  - `dtw` (function, line 18) `void dtw(const std::vector<float>& cost_matrix, int N, int M, std::vector<int>& text_indices_out, std::vector<int>&...`
  - `median_filter` (function, line 24) `void median_filter(std::vector<float>& data, int channels, int height, int width, int filter_width);`
  - `WORD_ALIGNMENT_H` (macro, line 2) `#define WORD_ALIGNMENT_H`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`
- Imported by: `core/moonshine-model.h`, `core/moonshine-streaming-model.h`, `core/word-alignment.cpp`

