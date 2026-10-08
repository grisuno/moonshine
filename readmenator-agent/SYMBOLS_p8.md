# Symbols (page 8 of 12)
Previous: [SYMBOLS_p7.md](SYMBOLS_p7.md)

| Symbol | Kind | File:Line | Signature |
|--------|------|-----------|-----------|
| `SpellingMatch` | struct | `core/spelling-fusion.h:34` | `` |
| `SpellingMatchType` | enum | `core/spelling-fusion.h:26` | `` |
| `SpellingMatchType` | class | `core/spelling-fusion.h:26` | `` |
| `SpellingMatcher` | class | `core/spelling-fusion.h:53` | `` |
| `SpellingPrediction` | struct | `core/spelling-fusion.h:47` | `` |
| `is_character` | function | `core/spelling-fusion.h:41` | `bool is_character() const` |
| `is_character` | function | `core/spelling-fusion.h:91` | `bool is_character() const` |
| `is_recognized` | function | `core/spelling-fusion.h:42` | `bool is_recognized() const` |
| `is_weak_homonym` | function | `core/spelling-fusion.h:66` | `bool is_weak_homonym(const std::string &raw_text) const;` |
| `Clip` | struct | `core/spelling-model-test.cpp:99` | `` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/spelling-model-test.cpp:12` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/spelling-model-test.cpp:60` | `TEST_CASE("spelling-model: load from path")` |
| `TEST_CASE` | function | `core/spelling-model-test.cpp:73` | `TEST_CASE("spelling-model: load from memory")` |
| `TEST_CASE` | function | `core/spelling-model-test.cpp:86` | `TEST_CASE("spelling-model: predict on bundled clips")` |
| `TEST_CASE` | function | `core/spelling-model-test.cpp:133` | `TEST_CASE("spelling-model: invalid arguments are rejected")` |
| `buffer` | function | `core/spelling-model-test.cpp:53` | `std::vector<uint8_t> buffer(static_cast<size_t>(size));` |
| `dummy` | function | `core/spelling-model-test.cpp:143` | `std::vector<float> dummy(16000, 0.0f);` |
| `find_model_path` | function | `core/spelling-model-test.cpp:21` | `std::string find_model_path()` |
| `find_wav` | function | `core/spelling-model-test.cpp:33` | `std::string find_wav(const std::string &label, const std::string &filename)` |
| `read_file` | function | `core/spelling-model-test.cpp:47` | `std::vector<uint8_t> read_file(const std::string &path)` |
| `SpellingModel` | function | `core/spelling-model.cpp:95` | `SpellingModel::SpellingModel(bool log_ort_run,                              const std::vector<std...` |
| `apply_default_metadata` | function | `core/spelling-model.cpp:157` | `void SpellingModel::apply_default_metadata()` |
| `clip` | function | `core/spelling-model.cpp:260` | `std::vector<float> clip(target_samples_, 0.0f);` |
| `initialize_session_options` | function | `core/spelling-model.cpp:137` | `void SpellingModel::initialize_session_options()` |
| `load` | function | `core/spelling-model.cpp:169` | `int SpellingModel::load(const char *model_path)` |
| `load_from_memory` | function | `core/spelling-model.cpp:177` | `int SpellingModel::load_from_memory(const uint8_t *model_data,                                   ...` |
| `lookup_metadata` | function | `core/spelling-model.cpp:26` | `std::optional<std::string> lookup_metadata(const OrtApi *ort_api,                                ...` |
| `parse_class_list_json` | function | `core/spelling-model.cpp:59` | `std::vector<std::string> parse_class_list_json(const std::string &raw)` |
| `populate_metadata_from_session` | function | `core/spelling-model.cpp:186` | `int SpellingModel::populate_metadata_from_session()` |
| `predict` | function | `core/spelling-model.cpp:243` | `int SpellingModel::predict(const float *audio, size_t audio_size,                            int3...` |
| `probs` | function | `core/spelling-model.cpp:307` | `std::vector<float> probs(row_size);` |
| `trim` | function | `core/spelling-model.cpp:45` | `std::string trim(const std::string &s)` |
| `SPELLING_MODEL_H` | macro | `core/spelling-model.h:2` | `#define SPELLING_MODEL_H` |
| `SpellingModel` | class | `core/spelling-model.h:24` | `` |
| `apply_default_metadata` | function | `core/spelling-model.h:63` | `void apply_default_metadata();` |
| `classes` | function | `core/spelling-model.h:58` | `const std::vector<std::string> &classes() const` |
| `clip_seconds` | function | `core/spelling-model.h:57` | `float clip_seconds() const` |
| `initialize_session_options` | function | `core/spelling-model.h:61` | `private: void initialize_session_options();` |
| `load` | function | `core/spelling-model.h:39` | `int load(const char *model_path);` |
| `load_from_memory` | function | `core/spelling-model.h:43` | `int load_from_memory(const uint8_t *model_data, size_t model_data_size);` |
| `populate_metadata_from_session` | function | `core/spelling-model.h:62` | `int populate_metadata_from_session();` |
| `predict` | function | `core/spelling-model.h:52` | `int predict(const float *audio, size_t audio_size, int32_t sample_rate, SpellingPrediction *out_prediction);` |
| `sample_rate` | function | `core/spelling-model.h:56` | `int32_t sample_rate() const` |
| `DOCTEST_CONFIG_IMPLEMENT` | macro | `core/tts-repeated-memory-test.cpp:27` | `#define DOCTEST_CONFIG_IMPLEMENT` |
| `EngineSpec` | struct | `core/tts-repeated-memory-test.cpp:216` | `` |
| `TEST_CASE` | function | `core/tts-repeated-memory-test.cpp:407` | `TEST_CASE("tts-repeated-memory-kokoro")` |
| `TEST_CASE` | function | `core/tts-repeated-memory-test.cpp:416` | `TEST_CASE("tts-repeated-memory-piper")` |
| `TEST_CASE` | function | `core/tts-repeated-memory-test.cpp:426` | `TEST_CASE("tts-repeated-memory-zipvoice")` |
| `create_synth` | function | `core/tts-repeated-memory-test.cpp:223` | `int32_t create_synth(const EngineSpec &spec)` |
| `detect_continual_growth` | function | `core/tts-repeated-memory-test.cpp:117` | `bool detect_continual_growth(const std::vector<size_t> &samples,                              siz...` |
| `discover_data_root` | function | `core/tts-repeated-memory-test.cpp:439` | `std::optional<fs::path> discover_data_root()` |
| `env_size` | function | `core/tts-repeated-memory-test.cpp:99` | `size_t env_size(const char *name, size_t default_value)` |
| `exercise_engine` | function | `core/tts-repeated-memory-test.cpp:294` | `void exercise_engine(const EngineSpec &spec)` |
| `file_present` | function | `core/tts-repeated-memory-test.cpp:339` | `bool file_present(const fs::path &p)` |
| `kokoro_spec` | function | `core/tts-repeated-memory-test.cpp:344` | `std::optional<EngineSpec> kokoro_spec()` |
| `main` | function | `core/tts-repeated-memory-test.cpp:464` | `int main(int argc, char **argv)` |
| `median` | function | `core/tts-repeated-memory-test.cpp:90` | `size_t median(std::vector<size_t> values)` |
| `piper_spec` | function | `core/tts-repeated-memory-test.cpp:355` | `std::optional<EngineSpec> piper_spec()` |
| `read_rss_kb` | function | `core/tts-repeated-memory-test.cpp:54` | `size_t read_rss_kb()` |
| `reload_strict` | function | `core/tts-repeated-memory-test.cpp:248` | `bool reload_strict()` |
| `run_growth_phase` | function | `core/tts-repeated-memory-test.cpp:259` | `void run_growth_phase(const std::string &label, size_t iterations,                       const st...` |
| `run_growth_phase` | function | `core/tts-repeated-memory-test.cpp:306` | `run_growth_phase(         std::string(spec.name) + " synth", synth_iterations,         [handle](s...` |
| `run_growth_phase` | function | `core/tts-repeated-memory-test.cpp:322` | `run_growth_phase(       std::string(spec.name) + " reload", reload_iterations,       [&spec](size...` |
| `synth_once` | function | `core/tts-repeated-memory-test.cpp:236` | `bool synth_once(int32_t handle, size_t text_index)` |
| `zipvoice_spec` | function | `core/tts-repeated-memory-test.cpp:389` | `std::optional<EngineSpec> zipvoice_spec()` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/voice-activity-detector-test.cpp:8` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `SUBCASE` | function | `core/voice-activity-detector-test.cpp:15` | `SUBCASE("vad-block")` |
| `SUBCASE` | function | `core/voice-activity-detector-test.cpp:54` | `SUBCASE("vad-stream")` |
| `SUBCASE` | function | `core/voice-activity-detector-test.cpp:122` | `SUBCASE("vad-threshold-0")` |
| `TEST_CASE` | function | `core/voice-activity-detector-test.cpp:11` | `TEST_CASE("voice-activity-detector-test")` |
| `VoiceActivityDetector` | function | `core/voice-activity-detector.cpp:24` | `VoiceActivityDetector::VoiceActivityDetector(float threshold,                                    ...` |
| `audio_vec` | function | `core/voice-activity-detector.cpp:136` | `std::vector<float> audio_vec(audio_data, audio_data + audio_data_size);` |
| `clear_completed_segment_audio_data` | function | `core/voice-activity-detector.cpp:99` | `void VoiceActivityDetector::clear_completed_segment_audio_data()` |
| `completed_segment_audio_byte_count` | function | `core/voice-activity-detector.cpp:115` | `size_t VoiceActivityDetector::completed_segment_audio_byte_count() const` |
| `input_audio_vector` | function | `core/voice-activity-detector.cpp:79` | `std::vector<float> input_audio_vector(audio_data, audio_data + audio_data_size);` |
| `on_voice_continuing` | function | `core/voice-activity-detector.cpp:210` | `void VoiceActivityDetector::on_voice_continuing()` |
| `on_voice_end` | function | `core/voice-activity-detector.cpp:219` | `void VoiceActivityDetector::on_voice_end()` |
| `on_voice_start` | function | `core/voice-activity-detector.cpp:196` | `void VoiceActivityDetector::on_voice_start()` |
| `process_audio` | function | `core/voice-activity-detector.cpp:69` | `void VoiceActivityDetector::process_audio(const float *audio_data,                               ...` |
| `process_audio_chunk` | function | `core/voice-activity-detector.cpp:125` | `void VoiceActivityDetector::process_audio_chunk(const float *audio_data,                         ...` |
| `retained_segment_audio_byte_count` | function | `core/voice-activity-detector.cpp:107` | `size_t VoiceActivityDetector::retained_segment_audio_byte_count() const` |
| `seconds_from_sample_count` | function | `core/voice-activity-detector.cpp:15` | `float seconds_from_sample_count(size_t sample_count)` |
| `start` | function | `core/voice-activity-detector.cpp:50` | `void VoiceActivityDetector::start()` |
| `stop` | function | `core/voice-activity-detector.cpp:62` | `void VoiceActivityDetector::stop()` |
| `to_string` | function | `core/voice-activity-detector.cpp:228` | `std::string VoiceActivitySegment::to_string() const` |
| `to_string` | function | `core/voice-activity-detector.cpp:238` | `std::string VoiceActivityDetector::to_string() const` |
| `VOICE_ACTIVITY_DETECTOR_H` | macro | `core/voice-activity-detector.h:2` | `#define VOICE_ACTIVITY_DETECTOR_H` |
| `VoiceActivityDetector` | class | `core/voice-activity-detector.h:22` | `` |
| `VoiceActivitySegment` | struct | `core/voice-activity-detector.h:9` | `` |
| `clear` | function | `core/voice-activity-detector.h:65` | `private: void clear();` |
| `clear_completed_segment_audio_data` | function | `core/voice-activity-detector.h:61` | `void clear_completed_segment_audio_data();` |
| `completed_segment_audio_byte_count` | function | `core/voice-activity-detector.h:60` | `size_t completed_segment_audio_byte_count() const;` |
| `get_segments` | function | `core/voice-activity-detector.h:56` | `const std::vector<VoiceActivitySegment> *get_segments() const` |
| `is_active` | function | `core/voice-activity-detector.h:53` | `bool is_active() const` |
| `on_voice_continuing` | function | `core/voice-activity-detector.h:68` | `void on_voice_continuing();` |
| `on_voice_end` | function | `core/voice-activity-detector.h:67` | `void on_voice_end();` |
| `on_voice_start` | function | `core/voice-activity-detector.h:66` | `void on_voice_start();` |
| `process_audio` | function | `core/voice-activity-detector.h:54` | `void process_audio(const float *audio_data, size_t audio_data_size, int32_t sample_rate);` |
| `process_audio_chunk` | function | `core/voice-activity-detector.h:69` | `void process_audio_chunk(const float *audio_data, size_t audio_data_size);` |
| `retained_segment_audio_byte_count` | function | `core/voice-activity-detector.h:59` | `size_t retained_segment_audio_byte_count() const;` |
| `start` | function | `core/voice-activity-detector.h:51` | `void start();` |
| `stop` | function | `core/voice-activity-detector.h:52` | `void stop();` |
| `BenchResult` | struct | `core/word-alignment-benchmark.cpp:31` | `` |
| `load_wav` | function | `core/word-alignment-benchmark.cpp:10` | `static float* load_wav(const char* path, long* num_samples_out)` |
| `main` | function | `core/word-alignment-benchmark.cpp:97` | `int main(int argc, char** argv)` |
| `run_benchmark` | function | `core/word-alignment-benchmark.cpp:38` | `static BenchResult run_benchmark(const char* model_path, const char* wav_path,                   ...` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/word-alignment-test.cpp:9` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `SUBCASE` | function | `core/word-alignment-test.cpp:13` | `SUBCASE("non-streaming-transcribe-with-word-timestamps")` |
| `TEST_CASE` | function | `core/word-alignment-test.cpp:12` | `TEST_CASE("word-timestamps")` |
| `D` | function | `core/word-alignment.cpp:16` | `std::vector<float> D((N + 1) * (M + 1), std::numeric_limits<float>::infinity());` |
| `WordGroup` | struct | `core/word-alignment.cpp:304` | `` |
| `align_words` | function | `core/word-alignment.cpp:181` | `std::vector<TranscriberWord> align_words(const float* cross_attention_data,                      ...` |
| `compute_median` | function | `core/word-alignment.cpp:93` | `static float compute_median(std::vector<float>& window)` |
| `decode_tokens` | function | `core/word-alignment.cpp:174` | `static std::string decode_tokens(BinTokenizer* tokenizer,                                  const ...` |
| `dtw` | function | `core/word-alignment.cpp:12` | `void dtw(const std::vector<float>& cost_matrix, int N, int M,          std::vector<int>& text_ind...` |
| `matrix` | function | `core/word-alignment.cpp:250` | `std::vector<float> matrix(n_steps * encoder_frames, 0.0f);` |
| `median_filter` | function | `core/word-alignment.cpp:99` | `void median_filter(std::vector<float>& data, int channels, int height,                    int wid...` |
| `neg_matrix` | function | `core/word-alignment.cpp:270` | `std::vector<float> neg_matrix(matrix.size());` |
| `padded` | function | `core/word-alignment.cpp:114` | `std::vector<float> padded(padded_width);` |
| `result_row` | function | `core/word-alignment.cpp:116` | `std::vector<float> result_row(width);` |
| `token_starts_new_word` | function | `core/word-alignment.cpp:159` | `static bool token_starts_new_word(BinTokenizer* tokenizer, int token_id)` |
| `trace` | function | `core/word-alignment.cpp:22` | `std::vector<int> trace(N * M, 0);` |
| `weights` | function | `core/word-alignment.cpp:200` | `std::vector<float> weights(total_size);` |
| `window` | function | `core/word-alignment.cpp:115` | `std::vector<float> window(filter_width);` |
| `TranscriberWord` | struct | `core/word-alignment.h:9` | `` |
| `WORD_ALIGNMENT_H` | macro | `core/word-alignment.h:2` | `#define WORD_ALIGNMENT_H` |
| `dtw` | function | `core/word-alignment.h:18` | `void dtw(const std::vector<float>& cost_matrix, int N, int M, std::vector<int>& text_indices_out, std::vector<int>&...` |
| `median_filter` | function | `core/word-alignment.h:24` | `void median_filter(std::vector<float>& data, int channels, int height, int width, int filter_width);` |
| `copyDirIfNeeded` | function | `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/AssetDirectoryCopy.kt:10` | `` |
| `MainActivity` | class | `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/MainActivity.kt:19` | `` |
| `VH` | class | `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/PhraseAdapter.kt:86` | `` |
| `addEmptyRow` | function | `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/PhraseAdapter.kt:40` | `` |
| `bind` | function | `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/PhraseAdapter.kt:89` | `` |
| `currentPhrases` | function | `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/PhraseAdapter.kt:71` | `` |
| `flashHighlight` | function | `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/PhraseAdapter.kt:54` | `` |
| `removeRow` | function | `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/PhraseAdapter.kt:46` | `` |
| `resetToDefaults` | function | `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/PhraseAdapter.kt:27` | `` |
| `rowIdMatchingCanonical` | function | `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/PhraseAdapter.kt:72` | `` |
| `copyDirIfNeeded` | function | `examples/android/TextToSpeech/app/src/main/java/ai/moonshine/examples/texttospeech/AssetDirectoryCopy.kt:10` | `` |
| `MainActivity` | class | `examples/android/TextToSpeech/app/src/main/java/ai/moonshine/examples/texttospeech/MainActivity.kt:64` | `` |
| `MainActivity` | class | `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java:22` | `` |
| `TranscriptEventListener` | method | `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java:62` | `` |
| `onCreate` | method | `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java:50` | `` |
| `onDestroy` | method | `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java:133` | `` |
| `onLineCompleted` | method | `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java:75` | `` |
| `onLineTextChanged` | method | `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java:64` | `` |
| `ContentView` | struct | `examples/ios/IntentRecognizer/IntentRecognizer/ContentView.swift:3` | `` |
| `IntentRecognizerApp` | struct | `examples/ios/IntentRecognizer/IntentRecognizer/IntentRecognizerApp.swift:4` | `` |
| `IntentPhraseRow` | struct | `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:4` | `` |
| `IntentSessionModel` | class | `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:24` | `` |
| `addPhrase` | function | `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:132` | `` |
| `bootstrapIfNeeded` | function | `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:52` | `` |
| `handleCompletedTranscriptLine` | function | `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:168` | `` |
| `handleTranscriptLineCompleted` | function | `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:231` | `` |
| `handleTranscriptLineStarted` | function | `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:218` | `` |
| `handleTranscriptLineTextChanged` | function | `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:226` | `` |
| `pauseMicIfNeededForBackground` | function | `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:207` | `` |
| `phraseTextCommitted` | function | `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:119` | `` |
| `removePhrase` | function | `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:137` | `` |
| `scheduleDebouncedIntentSync` | function | `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:110` | `` |
| `toggleListening` | function | `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:143` | `` |
| `IntentTranscriptBridge` | class | `examples/ios/IntentRecognizer/IntentRecognizer/IntentTranscriptBridge.swift:5` | `` |
| `onLineCompleted` | function | `examples/ios/IntentRecognizer/IntentRecognizer/IntentTranscriptBridge.swift:20` | `` |
| `onLineStarted` | function | `examples/ios/IntentRecognizer/IntentRecognizer/IntentTranscriptBridge.swift:7` | `` |
| `onLineTextChanged` | function | `examples/ios/IntentRecognizer/IntentRecognizer/IntentTranscriptBridge.swift:13` | `` |
| `ContentView` | struct | `examples/ios/TextToSpeech/TextToSpeech/ContentView.swift:3` | `` |
| `DownloadStatus` | struct | `examples/ios/TextToSpeech/TextToSpeech/TextToSpeechApp.swift:71` | `` |
| `KokoroLanguage` | struct | `examples/ios/TextToSpeech/TextToSpeech/TextToSpeechApp.swift:6` | `` |
| `TTSModel` | class | `examples/ios/TextToSpeech/TextToSpeech/TextToSpeechApp.swift:81` | `` |
| `TextToSpeechApp` | struct | `examples/ios/TextToSpeech/TextToSpeech/TextToSpeechApp.swift:374` | `` |
| `TtsVoice` | struct | `examples/ios/TextToSpeech/TextToSpeech/TextToSpeechApp.swift:61` | `` |
| `changeLanguage` | function | `examples/ios/TextToSpeech/TextToSpeech/TextToSpeechApp.swift:173` | `` |
| `changeVoice` | function | `examples/ios/TextToSpeech/TextToSpeech/TextToSpeechApp.swift:189` | `` |
| `hash` | function | `examples/ios/TextToSpeech/TextToSpeech/TextToSpeechApp.swift:10` | `` |
| `hash` | function | `examples/ios/TextToSpeech/TextToSpeech/TextToSpeechApp.swift:65` | `` |
| `initialize` | function | `examples/ios/TextToSpeech/TextToSpeech/TextToSpeechApp.swift:95` | `` |
| `speak` | function | `examples/ios/TextToSpeech/TextToSpeech/TextToSpeechApp.swift:194` | `` |
| `ContentView` | struct | `examples/ios/Transcriber/Transcriber/ContentView.swift:11` | `` |
| `TranscriberApp` | struct | `examples/ios/Transcriber/Transcriber/TranscriberApp.swift:13` | `` |
| `addNewMessage` | function | `examples/ios/Transcriber/Transcriber/TranscriberApp.swift:65` | `` |
| `handleRecordingChanged` | function | `examples/ios/Transcriber/Transcriber/TranscriberApp.swift:73` | `` |
| `updateLatestMessage` | function | `examples/ios/Transcriber/Transcriber/TranscriberApp.swift:69` | `` |
| `TranscriberTests` | struct | `examples/ios/Transcriber/TranscriberTests/TranscriberTests.swift:10` | `` |
| `TranscriberUITests` | class | `examples/ios/Transcriber/TranscriberUITests/TranscriberUITests.swift:9` | `` |
| `setUpWithError` | function | `examples/ios/Transcriber/TranscriberUITests/TranscriberUITests.swift:11` | `` |
| `tearDownWithError` | function | `examples/ios/Transcriber/TranscriberUITests/TranscriberUITests.swift:20` | `` |
| `testExample` | function | `examples/ios/Transcriber/TranscriberUITests/TranscriberUITests.swift:26` | `` |
| `testLaunchPerformance` | function | `examples/ios/Transcriber/TranscriberUITests/TranscriberUITests.swift:35` | `` |
| `TranscriberUITestsLaunchTests` | class | `examples/ios/Transcriber/TranscriberUITests/TranscriberUITestsLaunchTests.swift:9` | `` |
| `setUpWithError` | function | `examples/ios/Transcriber/TranscriberUITests/TranscriberUITestsLaunchTests.swift:15` | `` |
| `testLaunch` | function | `examples/ios/Transcriber/TranscriberUITests/TranscriberUITestsLaunchTests.swift:21` | `` |
| `Arguments` | struct | `examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift:76` | `` |
| `TestListener` | class | `examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift:31` | `` |
| `main` | function | `examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift:146` | `` |
| `onLineCompleted` | function | `examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift:46` | `` |
| `onLineStarted` | function | `examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift:33` | `` |
| `onLineTextChanged` | function | `examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift:39` | `` |
| `parseArguments` | function | `examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift:82` | `` |
| `transcribeWithStreaming` | function | `examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift:26` | `` |
| `transcribeWithoutStreaming` | function | `examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift:5` | `` |
| `TestListener` | class | `examples/macos/MicTranscription/Sources/MicTranscription/main.swift:40` | `` |
| `main` | function | `examples/macos/MicTranscription/Sources/MicTranscription/main.swift:5` | `` |
| `onLineCompleted` | function | `examples/macos/MicTranscription/Sources/MicTranscription/main.swift:55` | `` |
| `onLineStarted` | function | `examples/macos/MicTranscription/Sources/MicTranscription/main.swift:42` | `` |
| `onLineTextChanged` | function | `examples/macos/MicTranscription/Sources/MicTranscription/main.swift:48` | `` |
| `Arguments` | struct | `examples/macos/TextToSpeech/Sources/TextToSpeech/main.swift:54` | `` |
| `main` | function | `examples/macos/TextToSpeech/Sources/TextToSpeech/main.swift:246` | `` |
| `parseArguments` | function | `examples/macos/TextToSpeech/Sources/TextToSpeech/main.swift:86` | `` |
| `printUsage` | function | `examples/macos/TextToSpeech/Sources/TextToSpeech/main.swift:66` | `` |
| `resolveAssetRoot` | function | `examples/macos/TextToSpeech/Sources/TextToSpeech/main.swift:163` | `` |
| `resolveDevice` | function | `examples/macos/TextToSpeech/Sources/TextToSpeech/main.swift:205` | `` |
| `writeWav` | function | `examples/macos/TextToSpeech/Sources/TextToSpeech/main.swift:6` | `` |
| `TestListener` | class | `examples/python/basic_transcription.py:37` | `class TestListener(TranscriptEventListener)` |
| `on_line_completed` | method | `examples/python/basic_transcription.py:44` | `def on_line_completed(self, event)` |
| `on_line_started` | method | `examples/python/basic_transcription.py:38` | `def on_line_started(self, event)` |
| `on_line_text_changed` | method | `examples/python/basic_transcription.py:41` | `def on_line_text_changed(self, event)` |
| `transcribe_with_streaming` | function | `examples/python/basic_transcription.py:30` | `def transcribe_with_streaming(transcriber, audio_data, sample_rate)` |
| `transcribe_without_streaming` | function | `examples/python/basic_transcription.py:16` | `def transcribe_without_streaming(transcriber, audio_data, sample_rate)` |
| `TranscriptPrinter` | class | `examples/python/dialog_flow.py:102` | `class TranscriptPrinter(TranscriptEventListener)` |
| `__init__` | method | `examples/python/dialog_flow.py:112` | `def __init__(self)` |
| `_apply_wifi_config` | function | `examples/python/dialog_flow.py:89` | `def _apply_wifi_config(ssid, password)` |
| `_overwrite` | method | `examples/python/dialog_flow.py:116` | `def _overwrite(self, text)` |
| `full_onboarding` | function | `examples/python/dialog_flow.py:80` | `def full_onboarding(d)` |
| `main` | method | `examples/python/dialog_flow.py:411` | `def main()` |
| `mute` | method | `examples/python/dialog_flow.py:202` | `def mute(should_mute)` |
| `on_line_completed` | method | `examples/python/dialog_flow.py:128` | `def on_line_completed(self, event)` |
| `on_line_started` | method | `examples/python/dialog_flow.py:122` | `def on_line_started(self, event)` |
| `on_line_text_changed` | method | `examples/python/dialog_flow.py:125` | `def on_line_text_changed(self, event)` |
| `run_interactive` | method | `examples/python/dialog_flow.py:279` | `def run_interactive(flow_name)` |
| `run_live` | method | `examples/python/dialog_flow.py:142` | `def run_live(args)` |
| `run_scripted` | method | `examples/python/dialog_flow.py:347` | `def run_scripted(flow_name, answers)` |
| `set_spelling_mode` | method | `examples/python/dialog_flow.py:206` | `def set_spelling_mode(active)` |
| `set_timezone` | function | `examples/python/dialog_flow.py:70` | `def set_timezone(d)` |
| `setup_wifi` | function | `examples/python/dialog_flow.py:46` | `def setup_wifi(d)` |
| `speak` | method | `examples/python/dialog_flow.py:212` | `def speak(text)` |
| `speak` | method | `examples/python/dialog_flow.py:293` | `def speak(text)` |
| `speak` | method | `examples/python/dialog_flow.py:363` | `def speak(text)` |
| `TranscriptPrinter` | class | `examples/python/intent_recognition.py:56` | `class TranscriptPrinter(TranscriptEventListener)` |
| `__init__` | method | `examples/python/intent_recognition.py:59` | `def __init__(self)` |
| `main` | method | `examples/python/intent_recognition.py:80` | `def main()` |
| `on_lights_off` | function | `examples/python/intent_recognition.py:31` | `def on_lights_off(trigger, utterance, similarity)` |
| `on_lights_on` | function | `examples/python/intent_recognition.py:26` | `def on_lights_on(trigger, utterance, similarity)` |
| `on_line_completed` | method | `examples/python/intent_recognition.py:75` | `def on_line_completed(self, event)` |
| `on_line_started` | method | `examples/python/intent_recognition.py:69` | `def on_line_started(self, event)` |
| `on_line_text_changed` | method | `examples/python/intent_recognition.py:72` | `def on_line_text_changed(self, event)` |
| `on_music_play` | function | `examples/python/intent_recognition.py:46` | `def on_music_play(trigger, utterance, similarity)` |
| `on_music_stop` | function | `examples/python/intent_recognition.py:51` | `def on_music_stop(trigger, utterance, similarity)` |
| `on_timer` | function | `examples/python/intent_recognition.py:41` | `def on_timer(trigger, utterance, similarity)` |
| `on_weather` | function | `examples/python/intent_recognition.py:36` | `def on_weather(trigger, utterance, similarity)` |
| `update_last_terminal_line` | method | `examples/python/intent_recognition.py:62` | `def update_last_terminal_line(self, new_text)` |
| `FileListener` | class | `examples/python/mic_transcription.py:44` | `class FileListener(TranscriptEventListener)` |
| `TerminalListener` | class | `examples/python/mic_transcription.py:14` | `class TerminalListener(TranscriptEventListener)` |
| `__init__` | method | `examples/python/mic_transcription.py:15` | `def __init__(self)` |
| `on_line_completed` | method | `examples/python/mic_transcription.py:36` | `def on_line_completed(self, event)` |
| `on_line_completed` | method | `examples/python/mic_transcription.py:45` | `def on_line_completed(self, event)` |
| `on_line_started` | method | `examples/python/mic_transcription.py:30` | `def on_line_started(self, event)` |
| `on_line_text_changed` | method | `examples/python/mic_transcription.py:33` | `def on_line_text_changed(self, event)` |
| `update_last_terminal_line` | method | `examples/python/mic_transcription.py:20` | `def update_last_terminal_line(self, new_text)` |
| `OllamaVoice` | class | `examples/python/ollama-voice/ollama_voice.py:25` | `class OllamaVoice(TranscriptEventListener)` |
| `Spinner` | class | `examples/python/ollama-voice/ollama_voice.py:14` | `class Spinner` |
| `__init__` | method | `examples/python/ollama-voice/ollama_voice.py:17` | `def __init__(self)` |
| `__init__` | method | `examples/python/ollama-voice/ollama_voice.py:34` | `def __init__(self, ollama_model, system_prompt)` |
| `on_line_completed` | method | `examples/python/ollama-voice/ollama_voice.py:69` | `def on_line_completed(self, event)` |
| `on_line_text_changed` | method | `examples/python/ollama-voice/ollama_voice.py:59` | `def on_line_text_changed(self, event)` |
| `spin` | method | `examples/python/ollama-voice/ollama_voice.py:20` | `def spin(self)` |
| `TranscriptPrinter` | class | `examples/raspberry-pi/my-dalek/my-dalek.py:44` | `class TranscriptPrinter(TranscriptEventListener)` |
| `__init__` | method | `examples/raspberry-pi/my-dalek/my-dalek.py:47` | `def __init__(self)` |
| `on_exterminate` | method | `examples/raspberry-pi/my-dalek/my-dalek.py:100` | `def on_exterminate(trigger, utterance, similarity)` |
| `on_intent_triggered_on` | function | `examples/raspberry-pi/my-dalek/my-dalek.py:38` | `def on_intent_triggered_on(trigger, utterance, similarity)` |
| `on_line_completed` | method | `examples/raspberry-pi/my-dalek/my-dalek.py:63` | `def on_line_completed(self, event)` |
| `on_line_started` | method | `examples/raspberry-pi/my-dalek/my-dalek.py:57` | `def on_line_started(self, event)` |
| `on_line_text_changed` | method | `examples/raspberry-pi/my-dalek/my-dalek.py:60` | `def on_line_text_changed(self, event)` |
| `on_move_backward` | method | `examples/raspberry-pi/my-dalek/my-dalek.py:94` | `def on_move_backward(trigger, utterance, similarity)` |
| `on_move_forward` | method | `examples/raspberry-pi/my-dalek/my-dalek.py:92` | `def on_move_forward(trigger, utterance, similarity)` |
| `on_turn_left` | method | `examples/raspberry-pi/my-dalek/my-dalek.py:96` | `def on_turn_left(trigger, utterance, similarity)` |
| `on_turn_right` | method | `examples/raspberry-pi/my-dalek/my-dalek.py:98` | `def on_turn_right(trigger, utterance, similarity)` |
| `update_last_terminal_line` | method | `examples/raspberry-pi/my-dalek/my-dalek.py:50` | `def update_last_terminal_line(self, new_text)` |
| `COMInitializer` | class | `examples/windows/cli-transcriber/cli-transcriber.cpp:24` | `` |
| `COMInitializer` | function | `examples/windows/cli-transcriber/cli-transcriber.cpp:26` | `public:   COMInitializer()` |
| `CaptureLoop` | function | `examples/windows/cli-transcriber/cli-transcriber.cpp:229` | `private:   void CaptureLoop()` |
| `Initialize` | function | `examples/windows/cli-transcriber/cli-transcriber.cpp:95` | `bool Initialize()` |
| `MicrophoneCapture` | class | `examples/windows/cli-transcriber/cli-transcriber.cpp:71` | `` |
| `MicrophoneCapture` | function | `examples/windows/cli-transcriber/cli-transcriber.cpp:73` | `public:   MicrophoneCapture() : is_capturing_(false), sample_rate_(16000)` |
| `NOMINMAX` | macro | `examples/windows/cli-transcriber/cli-transcriber.cpp:15` | `#define NOMINMAX` |
| `SetAudioCallback` | function | `examples/windows/cli-transcriber/cli-transcriber.cpp:223` | `void SetAudioCallback(       std::function<void(const std::vector<float> &, int32_t)> callback)` |
| `Start` | function | `examples/windows/cli-transcriber/cli-transcriber.cpp:192` | `void Start()` |
| `Stop` | function | `examples/windows/cli-transcriber/cli-transcriber.cpp:208` | `void Stop()` |
| `WIN32_LEAN_AND_MEAN` | macro | `examples/windows/cli-transcriber/cli-transcriber.cpp:14` | `#define WIN32_LEAN_AND_MEAN` |
| `WavFileProducer` | class | `examples/windows/cli-transcriber/cli-transcriber.cpp:324` | `` |
| `WavFileProducer` | function | `examples/windows/cli-transcriber/cli-transcriber.cpp:326` | `public:   explicit WavFileProducer(std::string wav_path,                            float chunk_d...` |
| `getNextAudio` | function | `examples/windows/cli-transcriber/cli-transcriber.cpp:336` | `bool getNextAudio(std::vector<float> &out_audio_data)` |
| `loadWavData` | function | `examples/windows/cli-transcriber/cli-transcriber.cpp:351` | `private:   void loadWavData(const std::string &wav_path)` |
| `main` | function | `examples/windows/cli-transcriber/cli-transcriber.cpp:489` | `int main(int argc, char *argv[])` |
| `onError` | function | `examples/windows/cli-transcriber/cli-transcriber.cpp:60` | `void onError(const moonshine::Error &event) override` |
| `onLineCompleted` | function | `examples/windows/cli-transcriber/cli-transcriber.cpp:52` | `void onLineCompleted(const moonshine::LineCompleted &event) override` |
| `onLineStarted` | function | `examples/windows/cli-transcriber/cli-transcriber.cpp:38` | `public:   void onLineStarted(const moonshine::LineStarted &event) override` |
| `onLineTextChanged` | function | `examples/windows/cli-transcriber/cli-transcriber.cpp:44` | `void onLineTextChanged(const moonshine::LineTextChanged &event) override` |
| `pcm_data` | function | `examples/windows/cli-transcriber/cli-transcriber.cpp:428` | `std::vector<int16_t> pcm_data(num_samples);` |
| `runWavTranscription` | function | `examples/windows/cli-transcriber/cli-transcriber.cpp:456` | `int runWavTranscription(const std::string &model_path,                         moonshine::ModelAr...` |
| `sampleRate` | function | `examples/windows/cli-transcriber/cli-transcriber.cpp:348` | `int32_t sampleRate() const` |
| `SPELLING_AUDIO_CONFIG_H_` | macro | `micro/examples/rp2350/generated/audio_config.h:9` | `#define SPELLING_AUDIO_CONFIG_H_` |
| `SPELLING_CLASSES_H_` | macro | `micro/examples/rp2350/generated/classes.h:5` | `#define SPELLING_CLASSES_H_` |
| `kClassLabels` | variable | `micro/examples/rp2350/generated/classes.h:10` | `extern const char* const kClassLabels[kNumClasses];` |
| `SPELLING_MEL_TABLES_H_` | macro | `micro/examples/rp2350/generated/mel_tables.h:17` | `#define SPELLING_MEL_TABLES_H_` |
| `kMelNzIdx` | variable | `micro/examples/rp2350/generated/mel_tables.h:36` | `extern const int kMelNzIdx[kMelNzTotal];` |
| `kMelNzOff` | variable | `micro/examples/rp2350/generated/mel_tables.h:35` | `extern const int kMelNzOff[kMelTableNMels + 1];` |
| `kMelNzVal` | variable | `micro/examples/rp2350/generated/mel_tables.h:37` | `extern const float kMelNzVal[kMelNzTotal];` |
| `kMelWindow` | variable | `micro/examples/rp2350/generated/mel_tables.h:29` | `extern const float kMelWindow[kMelTableNFft];` |
| `SPELLING_MODEL_DATA_H_` | macro | `micro/examples/rp2350/generated/model_data.h:9` | `#define SPELLING_MODEL_DATA_H_` |
| `g_spelling_model_data` | variable | `micro/examples/rp2350/generated/model_data.h:14` | `extern const unsigned char g_spelling_model_data[];` |
| `g_spelling_model_data_size` | variable | `micro/examples/rp2350/generated/model_data.h:12` | `extern const unsigned int g_spelling_model_data_size;` |
| `NEURAL_TTS_DEMO_DATA_H_` | macro | `micro/examples/rp2350/generated/neural_tts_demo_data.h:3` | `#define NEURAL_TTS_DEMO_DATA_H_` |
| `PbDemoUtterance` | struct | `micro/examples/rp2350/generated/neural_tts_demo_data.h:13` | `` |
| `g_pb_codebook0` | variable | `micro/examples/rp2350/generated/neural_tts_demo_data.h:26` | `extern const int8_t g_pb_codebook0[2048 * kPbLatentDim];` |
| `g_pb_codebook0_scale` | variable | `micro/examples/rp2350/generated/neural_tts_demo_data.h:27` | `extern const float g_pb_codebook0_scale[kPbLatentDim];` |
| `g_pb_codebook1` | variable | `micro/examples/rp2350/generated/neural_tts_demo_data.h:28` | `extern const int8_t g_pb_codebook1[1024 * kPbLatentDim];` |
| `g_pb_codebook1_scale` | variable | `micro/examples/rp2350/generated/neural_tts_demo_data.h:29` | `extern const float g_pb_codebook1_scale[kPbLatentDim];` |
| `g_pb_codebook2` | variable | `micro/examples/rp2350/generated/neural_tts_demo_data.h:30` | `extern const int8_t g_pb_codebook2[1024 * kPbLatentDim];` |
| `g_pb_codebook2_scale` | variable | `micro/examples/rp2350/generated/neural_tts_demo_data.h:31` | `extern const float g_pb_codebook2_scale[kPbLatentDim];` |
| `g_pb_decoder_model` | variable | `micro/examples/rp2350/generated/neural_tts_demo_data.h:24` | `extern const unsigned char g_pb_decoder_model[];` |
| `g_pb_decoder_model_len` | variable | `micro/examples/rp2350/generated/neural_tts_demo_data.h:25` | `extern const unsigned int g_pb_decoder_model_len;` |
| `kPbUtterances` | variable | `micro/examples/rp2350/generated/neural_tts_demo_data.h:23` | `extern const PbDemoUtterance kPbUtterances[kPbNumUtterances];` |
| `g_neural_tts_pack` | function | `micro/examples/rp2350/generated/neural_tts_pack.S:5` | `` |
| `g_neural_tts_pack_end` | function | `micro/examples/rp2350/generated/neural_tts_pack.S:8` | `` |
| `Clip` | struct | `micro/examples/rp2350/generated/speaker_test_clips.h:11` | `` |
| `SPELLING_SPEAKER_TEST_CLIPS_H_` | macro | `micro/examples/rp2350/generated/speaker_test_clips.h:5` | `#define SPELLING_SPEAKER_TEST_CLIPS_H_` |
| `kClips` | variable | `micro/examples/rp2350/generated/speaker_test_clips.h:19` | `extern const Clip kClips[kClipCount];` |
| `EmbeddedClip` | struct | `micro/examples/rp2350/generated/test_clips.h:13` | `` |
| `SPELLING_TEST_CLIPS_H_` | macro | `micro/examples/rp2350/generated/test_clips.h:8` | `#define SPELLING_TEST_CLIPS_H_` |
| `kEmbeddedClips` | variable | `micro/examples/rp2350/generated/test_clips.h:25` | `extern const EmbeddedClip kEmbeddedClips[kNumEmbeddedClips];` |
| `SPELLING_VAD_CONFIG_H_` | macro | `micro/examples/rp2350/generated/vad_config.h:9` | `#define SPELLING_VAD_CONFIG_H_` |
| `SPELLING_VAD_MEL_TABLES_H_` | macro | `micro/examples/rp2350/generated/vad_mel_tables.h:9` | `#define SPELLING_VAD_MEL_TABLES_H_` |
| `kVadMelNzIdx` | variable | `micro/examples/rp2350/generated/vad_mel_tables.h:20` | `extern const int kVadMelNzIdx[kVadMelNzTotal];` |
| `kVadMelNzOff` | variable | `micro/examples/rp2350/generated/vad_mel_tables.h:19` | `extern const int kVadMelNzOff[kVadMelTableNMels + 1];` |
| `kVadMelNzVal` | variable | `micro/examples/rp2350/generated/vad_mel_tables.h:21` | `extern const float kVadMelNzVal[kVadMelNzTotal];` |
| `kVadMelWindow` | variable | `micro/examples/rp2350/generated/vad_mel_tables.h:18` | `extern const float kVadMelWindow[kVadMelTableNFft];` |
| `SPELLING_VAD_MODEL_DATA_H_` | macro | `micro/examples/rp2350/generated/vad_model_data.h:8` | `#define SPELLING_VAD_MODEL_DATA_H_` |
| `g_vad_model_data` | variable | `micro/examples/rp2350/generated/vad_model_data.h:12` | `extern const unsigned char g_vad_model_data[];` |
| `g_vad_model_data_size` | variable | `micro/examples/rp2350/generated/vad_model_data.h:11` | `extern const unsigned int g_vad_model_data_size;` |
| `DHCP_DOES_ARP_CHECK` | macro | `micro/examples/rp2350/lwipopts.h:47` | `#define DHCP_DOES_ARP_CHECK` |
| `ETHARP_STATS` | macro | `micro/examples/rp2350/lwipopts.h:65` | `#define ETHARP_STATS` |
| `ICMP_STATS` | macro | `micro/examples/rp2350/lwipopts.h:68` | `#define ICMP_STATS` |
| `IP_STATS` | macro | `micro/examples/rp2350/lwipopts.h:66` | `#define IP_STATS` |
| `LINK_STATS` | macro | `micro/examples/rp2350/lwipopts.h:64` | `#define LINK_STATS` |
| `LWIP_ARP` | macro | `micro/examples/rp2350/lwipopts.h:39` | `#define LWIP_ARP` |
| `LWIP_CHKSUM_ALGORITHM` | macro | `micro/examples/rp2350/lwipopts.h:57` | `#define LWIP_CHKSUM_ALGORITHM` |
| `LWIP_DEBUG` | macro | `micro/examples/rp2350/lwipopts.h:71` | `#define LWIP_DEBUG` |
| `LWIP_DHCP` | macro | `micro/examples/rp2350/lwipopts.h:46` | `#define LWIP_DHCP` |
| `LWIP_DHCP_DOES_ACD_CHECK` | macro | `micro/examples/rp2350/lwipopts.h:48` | `#define LWIP_DHCP_DOES_ACD_CHECK` |
| `LWIP_DNS` | macro | `micro/examples/rp2350/lwipopts.h:45` | `#define LWIP_DNS` |
| `LWIP_ETHERNET` | macro | `micro/examples/rp2350/lwipopts.h:40` | `#define LWIP_ETHERNET` |
| `LWIP_ICMP` | macro | `micro/examples/rp2350/lwipopts.h:41` | `#define LWIP_ICMP` |
| `LWIP_IPV4` | macro | `micro/examples/rp2350/lwipopts.h:37` | `#define LWIP_IPV4` |
| `LWIP_IPV6` | macro | `micro/examples/rp2350/lwipopts.h:38` | `#define LWIP_IPV6` |
| `LWIP_NETCONN` | macro | `micro/examples/rp2350/lwipopts.h:22` | `#define LWIP_NETCONN` |
| `LWIP_NETIF_HOSTNAME` | macro | `micro/examples/rp2350/lwipopts.h:53` | `#define LWIP_NETIF_HOSTNAME` |
| `LWIP_NETIF_LINK_CALLBACK` | macro | `micro/examples/rp2350/lwipopts.h:52` | `#define LWIP_NETIF_LINK_CALLBACK` |
| `LWIP_NETIF_STATUS_CALLBACK` | macro | `micro/examples/rp2350/lwipopts.h:51` | `#define LWIP_NETIF_STATUS_CALLBACK` |
| `LWIP_NETIF_TX_SINGLE_PBUF` | macro | `micro/examples/rp2350/lwipopts.h:54` | `#define LWIP_NETIF_TX_SINGLE_PBUF` |
| `LWIP_RAW` | macro | `micro/examples/rp2350/lwipopts.h:42` | `#define LWIP_RAW` |
| `LWIP_SOCKET` | macro | `micro/examples/rp2350/lwipopts.h:21` | `#define LWIP_SOCKET` |
| `LWIP_STATS` | macro | `micro/examples/rp2350/lwipopts.h:60` | `#define LWIP_STATS` |
| `LWIP_STATS_DISPLAY` | macro | `micro/examples/rp2350/lwipopts.h:73` | `#define LWIP_STATS_DISPLAY` |
| `LWIP_TCP` | macro | `micro/examples/rp2350/lwipopts.h:44` | `#define LWIP_TCP` |
| `LWIP_UDP` | macro | `micro/examples/rp2350/lwipopts.h:43` | `#define LWIP_UDP` |
| `MEMP_NUM_ARP_QUEUE` | macro | `micro/examples/rp2350/lwipopts.h:31` | `#define MEMP_NUM_ARP_QUEUE` |
| `MEMP_NUM_PBUF` | macro | `micro/examples/rp2350/lwipopts.h:29` | `#define MEMP_NUM_PBUF` |
| `MEMP_NUM_SYS_TIMEOUT` | macro | `micro/examples/rp2350/lwipopts.h:32` | `#define MEMP_NUM_SYS_TIMEOUT` |
| `MEMP_NUM_UDP_PCB` | macro | `micro/examples/rp2350/lwipopts.h:30` | `#define MEMP_NUM_UDP_PCB` |
| `MEMP_STATS` | macro | `micro/examples/rp2350/lwipopts.h:63` | `#define MEMP_STATS` |
| `MEM_ALIGNMENT` | macro | `micro/examples/rp2350/lwipopts.h:27` | `#define MEM_ALIGNMENT` |
| `MEM_LIBC_MALLOC` | macro | `micro/examples/rp2350/lwipopts.h:26` | `#define MEM_LIBC_MALLOC` |
| `MEM_SIZE` | macro | `micro/examples/rp2350/lwipopts.h:28` | `#define MEM_SIZE` |
| `MEM_STATS` | macro | `micro/examples/rp2350/lwipopts.h:61` | `#define MEM_STATS` |
| `NO_SYS` | macro | `micro/examples/rp2350/lwipopts.h:20` | `#define NO_SYS` |
| `PBUF_POOL_BUFSIZE` | macro | `micro/examples/rp2350/lwipopts.h:34` | `#define PBUF_POOL_BUFSIZE` |
| `PBUF_POOL_SIZE` | macro | `micro/examples/rp2350/lwipopts.h:33` | `#define PBUF_POOL_SIZE` |
| `SPELLING_LWIPOPTS_H_` | macro | `micro/examples/rp2350/lwipopts.h:17` | `#define SPELLING_LWIPOPTS_H_` |
| `SYS_LIGHTWEIGHT_PROT` | macro | `micro/examples/rp2350/lwipopts.h:23` | `#define SYS_LIGHTWEIGHT_PROT` |
| `SYS_STATS` | macro | `micro/examples/rp2350/lwipopts.h:62` | `#define SYS_STATS` |
| `UDP_STATS` | macro | `micro/examples/rp2350/lwipopts.h:67` | `#define UDP_STATS` |
| `find_port` | function | `micro/examples/rp2350/scripts/capture_neural_tts.py:22` | `def find_port()` |
| `main` | function | `micro/examples/rp2350/scripts/capture_neural_tts.py:29` | `def main()` |
| `SerialReader` | class | `micro/examples/rp2350/scripts/capture_stt.py:71` | `class SerialReader` |
| `__init__` | method | `micro/examples/rp2350/scripts/capture_stt.py:74` | `def __init__(self, fd)` |
| `_fill` | method | `micro/examples/rp2350/scripts/capture_stt.py:78` | `def _fill(self)` |
| `_open_raw` | function | `micro/examples/rp2350/scripts/capture_stt.py:61` | `def _open_raw(dev)` |
| `_resolve_serial` | function | `micro/examples/rp2350/scripts/capture_stt.py:36` | `def _resolve_serial(explicit, timeout)` |
| `_save_wav` | method | `micro/examples/rp2350/scripts/capture_stt.py:109` | `def _save_wav(path, raw, rate)` |
| `main` | method | `micro/examples/rp2350/scripts/capture_stt.py:117` | `def main()` |
| `read_exact` | method | `micro/examples/rp2350/scripts/capture_stt.py:100` | `def read_exact(self, n)` |
| `readline` | method | `micro/examples/rp2350/scripts/capture_stt.py:92` | `def readline(self)` |
| `draw_bar` | function | `micro/examples/rp2350/scripts/flash.sh:259` | `` |
| `find_mounted_volume` | function | `micro/examples/rp2350/scripts/flash.sh:66` | `` |
| `usage` | function | `micro/examples/rp2350/scripts/flash.sh:78` | `` |
| `wait_volume_writable` | function | `micro/examples/rp2350/scripts/flash.sh:227` | `` |
| `_read_pcm` | function | `micro/examples/rp2350/scripts/generate_speaker_test_clips.py:27` | `def _read_pcm(path)` |
| `_write_header` | function | `micro/examples/rp2350/scripts/generate_speaker_test_clips.py:46` | `def _write_header()` |
| `main` | function | `micro/examples/rp2350/scripts/generate_speaker_test_clips.py:74` | `def main()` |
| `_wait_for_any_usbmodem` | function | `micro/examples/rp2350/scripts/monitor.sh:89` | `` |
| `_wait_for_specific_tty` | function | `micro/examples/rp2350/scripts/monitor.sh:113` | `` |
| `find_port` | function | `micro/examples/rp2350/scripts/tts_speak.py:36` | `def find_port()` |
| `main` | function | `micro/examples/rp2350/scripts/tts_speak.py:44` | `def main()` |
| `send_line` | function | `micro/examples/rp2350/scripts/tts_speak.py:71` | `def send_line(s)` |
| `SerialReader` | class | `micro/examples/rp2350/scripts/usb_audio_bridge.py:101` | `class SerialReader` |
| `__init__` | method | `micro/examples/rp2350/scripts/usb_audio_bridge.py:104` | `def __init__(self, fd)` |
| `_dev` | method | `micro/examples/rp2350/scripts/usb_audio_bridge.py:163` | `def _dev(arg)` |
| `_fill` | method | `micro/examples/rp2350/scripts/usb_audio_bridge.py:108` | `def _fill(self)` |
| `_on_signal` | method | `micro/examples/rp2350/scripts/usb_audio_bridge.py:404` | `def _on_signal(signum, frame)` |
| `_open_raw` | function | `micro/examples/rp2350/scripts/usb_audio_bridge.py:80` | `def _open_raw(dev)` |
| `_resolve_serial` | function | `micro/examples/rp2350/scripts/usb_audio_bridge.py:49` | `def _resolve_serial(explicit, timeout)` |
| `flush_mic` | method | `micro/examples/rp2350/scripts/usb_audio_bridge.py:260` | `def flush_mic()` |
| `main` | method | `micro/examples/rp2350/scripts/usb_audio_bridge.py:140` | `def main()` |
| `on_audio` | method | `micro/examples/rp2350/scripts/usb_audio_bridge.py:206` | `def on_audio(indata, frames, time_info, status)` |
| `read_exact` | method | `micro/examples/rp2350/scripts/usb_audio_bridge.py:131` | `def read_exact(self, n)` |
| `readline` | method | `micro/examples/rp2350/scripts/usb_audio_bridge.py:123` | `def readline(self)` |
| `receiver` | method | `micro/examples/rp2350/scripts/usb_audio_bridge.py:268` | `def receiver()` |
| `save_stream` | method | `micro/examples/rp2350/scripts/usb_audio_bridge.py:184` | `def save_stream(tag, samples, rate)` |
| `sender` | method | `micro/examples/rp2350/scripts/usb_audio_bridge.py:224` | `def sender()` |
| `BoardInit` | function | `micro/examples/rp2350/src/app_common.cc:42` | `unsigned BoardInit()` |
| `LedPulse` | function | `micro/examples/rp2350/src/app_common.cc:33` | `void LedPulse(unsigned pin, int count, int on_ms, int off_ms)` |
| `PrintBootBanner` | function | `micro/examples/rp2350/src/app_common.cc:84` | `void PrintBootBanner()` |
| `BoardInit` | function | `micro/examples/rp2350/src/app_common.h:48` | `unsigned BoardInit();` |
| `LedPulse` | function | `micro/examples/rp2350/src/app_common.h:55` | `void LedPulse(unsigned pin, int count, int on_ms, int off_ms);` |
| `PrintBootBanner` | function | `micro/examples/rp2350/src/app_common.h:52` | `void PrintBootBanner();` |
| `SPELLING_APP_COMMON_H_` | macro | `micro/examples/rp2350/src/app_common.h:8` | `#define SPELLING_APP_COMMON_H_` |
| `SPELLING_TINY_ARENA_BYTES` | macro | `micro/examples/rp2350/src/app_common.h:31` | `#define SPELLING_TINY_ARENA_BYTES` |
| `g_tensor_arena` | variable | `micro/examples/rp2350/src/app_common.h:42` | `extern uint8_t g_tensor_arena[kTensorArenaSize];` |
| `g_waveform` | variable | `micro/examples/rp2350/src/app_common.h:43` | `extern int16_t g_waveform[kClipNumSamples];` |
| `AudioInput` | class | `micro/examples/rp2350/src/audio_io.h:19` | `` |
| `AudioOutput` | class | `micro/examples/rp2350/src/audio_io.h:35` | `` |
| `SPELLING_AUDIO_IO_H_` | macro | `micro/examples/rp2350/src/audio_io.h:12` | `#define SPELLING_AUDIO_IO_H_` |
| `PlayCapturedClip` | function | `micro/examples/rp2350/src/audio_service.cc:386` | `void PlayCapturedClip(const int16_t* window, int num_samples,                       AudioOutput& ...` |
| `PopClause` | function | `micro/examples/rp2350/src/audio_service.cc:472` | `const char* PopClause(const char* text, char* out, size_t cap)` |
| `RecognizeOne` | function | `micro/examples/rp2350/src/audio_service.cc:103` | `int RecognizeOne(AudioInput& input, uint8_t* arena, std::size_t arena_size,                  int1...` |
| `RecognizerInit` | function | `micro/examples/rp2350/src/audio_service.cc:74` | `void RecognizerInit(kiss_fftr_state* fft)` |
| `RunAudioService` | function | `micro/examples/rp2350/src/audio_service.cc:547` | `void RunAudioService(AudioInput& input, AudioOutput& output, uint8_t* arena,                     ...` |
| `SetTtsVolume` | function | `micro/examples/rp2350/src/audio_service.cc:66` | `void SetTtsVolume(float volume)` |
| `SkipSpaces` | function | `micro/examples/rp2350/src/audio_service.cc:464` | `const char* SkipSpaces(const char* p)` |
| `Speak` | function | `micro/examples/rp2350/src/audio_service.cc:499` | `void Speak(const char* text, AudioOutput& output, AudioInput& input,            uint8_t* arena, s...` |
| `SpeakEmit` | function | `micro/examples/rp2350/src/audio_service.cc:440` | `void SpeakEmit(void* user, const int16_t* samples, int n)` |
| `SpeakSink` | struct | `micro/examples/rp2350/src/audio_service.cc:433` | `` |
| `TtsVolume` | function | `micro/examples/rp2350/src/audio_service.cc:72` | `float TtsVolume()` |
| `g_neural_tts_pack` | variable | `micro/examples/rp2350/src/audio_service.cc:53` | `extern "C" const uint8_t g_neural_tts_pack[];` |
| `RecognizeOne` | function | `micro/examples/rp2350/src/audio_service.h:46` | `int RecognizeOne(AudioInput& input, uint8_t* arena, std::size_t arena_size, int16_t* window, int window_samples...` |
| `RecognizerInit` | function | `micro/examples/rp2350/src/audio_service.h:38` | `void RecognizerInit(kiss_fftr_state* fft);` |
| `RunAudioService` | function | `micro/examples/rp2350/src/audio_service.h:77` | `void RunAudioService(AudioInput& input, AudioOutput& output, uint8_t* arena, std::size_t arena_size...` |
| `SPELLING_AUDIO_SERVICE_H_` | macro | `micro/examples/rp2350/src/audio_service.h:19` | `#define SPELLING_AUDIO_SERVICE_H_` |
| `SetTtsVolume` | function | `micro/examples/rp2350/src/audio_service.h:61` | `void SetTtsVolume(float volume);` |
| `Speak` | function | `micro/examples/rp2350/src/audio_service.h:68` | `void Speak(const char* text, AudioOutput& output, AudioInput& input, uint8_t* arena, std::size_t arena_size);` |
| `TtsVolume` | function | `micro/examples/rp2350/src/audio_service.h:62` | `float TtsVolume();` |
| `kiss_fftr_state` | struct | `micro/examples/rp2350/src/audio_service.h:26` | `` |
| `RunEchoApp` | function | `micro/examples/rp2350/src/echo_app.cc:28` | `void RunEchoApp()` |
| `SPELLING_ECHO_APP_H_` | macro | `micro/examples/rp2350/src/echo_app.h:8` | `#define SPELLING_ECHO_APP_H_` |
| `RunEchoHardwareApp` | function | `micro/examples/rp2350/src/echo_hardware_app.cc:24` | `void RunEchoHardwareApp()` |
| `SPELLING_ECHO_HARDWARE_APP_H_` | macro | `micro/examples/rp2350/src/echo_hardware_app.h:9` | `#define SPELLING_ECHO_HARDWARE_APP_H_` |
| `CaptureWriteIdx` | function | `micro/examples/rp2350/src/i2s_audio_io.cc:49` | `inline unsigned CaptureWriteIdx()` |
| `Drain` | function | `micro/examples/rp2350/src/i2s_audio_io.cc:114` | `void I2sAudioInput::Drain()` |
| `I2sAudioInput` | function | `micro/examples/rp2350/src/i2s_audio_io.cc:76` | `I2sAudioInput::I2sAudioInput(int sample_rate)     : sm_(0), dc_blocker_(sample_rate)` |
| `ReadHop` | function | `micro/examples/rp2350/src/i2s_audio_io.cc:96` | `bool I2sAudioInput::ReadHop(int16_t* out, int n)` |
| `StartCaptureDma` | function | `micro/examples/rp2350/src/i2s_audio_io.cc:55` | `void StartCaptureDma()` |
| `I2sAudioInput` | class | `micro/examples/rp2350/src/i2s_audio_io.h:20` | `` |
| `SPELLING_I2S_AUDIO_IO_H_` | macro | `micro/examples/rp2350/src/i2s_audio_io.h:13` | `#define SPELLING_I2S_AUDIO_IO_H_` |
| `ApplyClockDiv` | function | `micro/examples/rp2350/src/i2s_audio_out.cc:131` | `void I2sAudioOutput::ApplyClockDiv()` |
| `Begin` | function | `micro/examples/rp2350/src/i2s_audio_out.cc:140` | `void I2sAudioOutput::Begin(int sample_rate, int num_samples, const char* kind)` |
| `End` | function | `micro/examples/rp2350/src/i2s_audio_out.cc:167` | `void I2sAudioOutput::End()` |
| `I2sAudioOutput` | function | `micro/examples/rp2350/src/i2s_audio_out.cc:72` | `I2sAudioOutput::I2sAudioOutput(unsigned data_pin, unsigned clock_base,                           ...` |
| `PeakNormalizeGain` | function | `micro/examples/rp2350/src/i2s_audio_out.cc:43` | `float PeakNormalizeGain(const int16_t* samples, int n, float target,                         floa...` |
| `PeakNormalizeGain` | function | `micro/examples/rp2350/src/i2s_audio_out.cc:58` | `float PeakNormalizeGain(const float* samples, int n, float target,                         float ...` |
| `PushFrame` | function | `micro/examples/rp2350/src/i2s_audio_out.cc:118` | `void I2sAudioOutput::PushFrame(uint32_t frame)` |
| `ReadIdx` | function | `micro/examples/rp2350/src/i2s_audio_out.cc:101` | `unsigned I2sAudioOutput::ReadIdx() const` |
| `StartDma` | function | `micro/examples/rp2350/src/i2s_audio_out.cc:111` | `void I2sAudioOutput::StartDma()` |
| `StereoFrame` | function | `micro/examples/rp2350/src/i2s_audio_out.cc:20` | `inline uint32_t StereoFrame(int16_t s)` |
| `Used` | function | `micro/examples/rp2350/src/i2s_audio_out.cc:107` | `unsigned I2sAudioOutput::Used() const` |
| `Write` | function | `micro/examples/rp2350/src/i2s_audio_out.cc:158` | `void I2sAudioOutput::Write(const int16_t* samples, int n)` |
| `ApplyClockDiv` | function | `micro/examples/rp2350/src/i2s_audio_out.h:60` | `void ApplyClockDiv();` |
| `I2sAudioOutput` | class | `micro/examples/rp2350/src/i2s_audio_out.h:42` | `` |
| `PeakNormalizeGain` | function | `micro/examples/rp2350/src/i2s_audio_out.h:37` | `float PeakNormalizeGain(const int16_t* samples, int n, float target = 0.9f, float max_gain = 32.0f);` |
| `PushFrame` | function | `micro/examples/rp2350/src/i2s_audio_out.h:63` | `void PushFrame(uint32_t frame);` |
| `ReadIdx` | function | `micro/examples/rp2350/src/i2s_audio_out.h:68` | `unsigned ReadIdx() const;` |
| `SPELLING_I2S_AUDIO_OUT_H_` | macro | `micro/examples/rp2350/src/i2s_audio_out.h:23` | `#define SPELLING_I2S_AUDIO_OUT_H_` |
| `SetGain` | function | `micro/examples/rp2350/src/i2s_audio_out.h:56` | `void SetGain(float gain)` |
| `StartDma` | function | `micro/examples/rp2350/src/i2s_audio_out.h:66` | `void StartDma();` |
| `Used` | function | `micro/examples/rp2350/src/i2s_audio_out.h:69` | `unsigned Used() const;` |
| `I2sDcBlocker` | function | `micro/examples/rp2350/src/i2s_mic_process.cc:18` | `I2sDcBlocker::I2sDcBlocker(int sample_rate_hz, float cutoff_hz)     : r_(std::exp(-2.f * 3.141592...` |
| `I2sRawToInt16` | function | `micro/examples/rp2350/src/i2s_mic_process.cc:12` | `int16_t I2sRawToInt16(uint32_t raw)` |
| `I2sRawToInt32` | function | `micro/examples/rp2350/src/i2s_mic_process.cc:8` | `int32_t I2sRawToInt32(uint32_t raw)` |
| `I2sRemoveBufferDc` | function | `micro/examples/rp2350/src/i2s_mic_process.cc:37` | `void I2sRemoveBufferDc(int16_t* samples, int n)` |
| `Process` | function | `micro/examples/rp2350/src/i2s_mic_process.cc:22` | `int16_t I2sDcBlocker::Process(int16_t x)` |
| `Reset` | function | `micro/examples/rp2350/src/i2s_mic_process.cc:32` | `void I2sDcBlocker::Reset()` |
| `I2sDcBlocker` | class | `micro/examples/rp2350/src/i2s_mic_process.h:20` | `` |
| `I2sRawToInt16` | function | `micro/examples/rp2350/src/i2s_mic_process.h:17` | `int16_t I2sRawToInt16(uint32_t raw);` |
| `I2sRawToInt32` | function | `micro/examples/rp2350/src/i2s_mic_process.h:16` | `int32_t I2sRawToInt32(uint32_t raw);` |

Next: [SYMBOLS_p9.md](SYMBOLS_p9.md)
