# Symbols (page 3 of 12)
Previous: [SYMBOLS_p2.md](SYMBOLS_p2.md)

| Symbol | Kind | File:Line | Signature |
|--------|------|-----------|-----------|
| `Stream` | class | `core/moonshine-cpp.h:421` | `` |
| `Stream` | function | `core/moonshine-cpp.h:932` | `inline Stream::Stream(Transcriber *transcriber, double updateInterval,                       uint...` |
| `Stream` | function | `core/moonshine-cpp.h:945` | `inline Stream::Stream(Stream &&other)     : transcriber_(other.transcriber_),       handle_(other...` |
| `TextToSpeech` | class | `core/moonshine-cpp.h:702` | `` |
| `TextToSpeech` | function | `core/moonshine-cpp.h:1400` | `inline TextToSpeech::TextToSpeech(     const std::string &language, const std::vector<moonshine_o...` |
| `TextToSpeech` | function | `core/moonshine-cpp.h:1411` | `inline TextToSpeech::TextToSpeech(TextToSpeech &&other)     : handle_(other.handle_), language_(s...` |
| `Transcriber` | class | `core/moonshine-cpp.h:514` | `` |
| `Transcriber` | function | `core/moonshine-cpp.h:646` | `Transcriber(int32_t handle, ModelArch modelArch, double updateInterval)       : handle_(handle), ...` |
| `Transcriber` | function | `core/moonshine-cpp.h:1214` | `inline Transcriber::Transcriber(const std::string &modelPath,                                 Mod...` |
| `Transcriber` | function | `core/moonshine-cpp.h:1226` | `inline Transcriber::Transcriber(     const std::string &modelPath, ModelArch modelArch, double up...` |
| `Transcriber` | function | `core/moonshine-cpp.h:1267` | `inline Transcriber::Transcriber(Transcriber &&other)     : handle_(other.handle_),       modelPat...` |
| `Transcript` | struct | `core/moonshine-cpp.h:264` | `` |
| `Transcript` | function | `core/moonshine-cpp.h:269` | `Transcript()` |
| `Transcript` | function | `core/moonshine-cpp.h:272` | `Transcript(const transcript_t *transcript_c)` |
| `TranscriptEvent` | class | `core/moonshine-cpp.h:296` | `` |
| `TranscriptEvent` | function | `core/moonshine-cpp.h:320` | `protected:   TranscriptEvent(const TranscriptLine &line, int32_t streamHandle, Type type)       :...` |
| `TranscriptEventListener` | class | `core/moonshine-cpp.h:385` | `` |
| `TranscriptLine` | struct | `core/moonshine-cpp.h:139` | `` |
| `TranscriptLine` | function | `core/moonshine-cpp.h:186` | `TranscriptLine()       : startTime(0.0f),         duration(0.0f),         lineId(0),         isCo...` |
| `TranscriptLine` | function | `core/moonshine-cpp.h:198` | `TranscriptLine(const transcript_line_t &line_c)       : startTime(line_c.start_time),         dur...` |
| `TtsSynthesisResult` | struct | `core/moonshine-cpp.h:667` | `` |
| `TtsSynthesisResult` | function | `core/moonshine-cpp.h:673` | `TtsSynthesisResult() : sampleRateHz(0)` |
| `TtsSynthesisResult` | function | `core/moonshine-cpp.h:674` | `TtsSynthesisResult(std::vector<float> samples, int32_t sampleRateHz)       : samples(std::move(sa...` |
| `Type` | enum | `core/moonshine-cpp.h:299` | `` |
| `WordTiming` | struct | `core/moonshine-cpp.h:83` | `` |
| `WordTiming` | function | `core/moonshine-cpp.h:93` | `WordTiming() : start(0.0f), end(0.0f), confidence(0.0f)` |
| `WordTiming` | function | `core/moonshine-cpp.h:94` | `WordTiming(const std::string &word, float start, float end, float confidence)       : word(word),...` |
| `addAudio` | function | `core/moonshine-cpp.h:986` | `inline void Stream::addAudio(const std::vector<float> &audioData,                              in...` |
| `addAudio` | function | `core/moonshine-cpp.h:1341` | `inline void Transcriber::addAudio(const std::vector<float> &audioData,                           ...` |
| `addListener` | function | `core/moonshine-cpp.h:1011` | `inline void Stream::addListener(TranscriptEventListener *listener)` |
| `addListener` | function | `core/moonshine-cpp.h:1017` | `inline void Stream::addListener(     std::function<void(const TranscriptEvent &)> listener)` |
| `addListener` | function | `core/moonshine-cpp.h:1350` | `inline void Transcriber::addListener(TranscriptEventListener *listener)` |
| `addListener` | function | `core/moonshine-cpp.h:1354` | `inline void Transcriber::addListener(     std::function<void(const TranscriptEvent &)> listener)` |
| `buildOptions` | function | `core/moonshine-cpp.h:1187` | `inline OptionsBuffer buildOptions(     const std::string &spellingModelPath,     const std::vecto...` |
| `calculateEmbedding` | function | `core/moonshine-cpp.h:1685` | `inline std::vector<float> IntentRecognizer::calculateEmbedding(     const std::string &sentence, ...` |
| `checkError` | function | `core/moonshine-cpp.h:1383` | `inline void Transcriber::checkError(int32_t error) const` |
| `checkError` | function | `core/moonshine-cpp.h:1391` | `inline void Stream::checkError(int32_t error) const` |
| `checkError` | function | `core/moonshine-cpp.h:1514` | `inline void TextToSpeech::checkError(int32_t error) const` |
| `checkError` | function | `core/moonshine-cpp.h:1593` | `inline void GraphemeToPhonemizer::checkError(int32_t error) const` |
| `checkError` | function | `core/moonshine-cpp.h:1706` | `inline void IntentRecognizer::checkError(int32_t error) const` |
| `clearIntents` | function | `core/moonshine-cpp.h:1681` | `inline void IntentRecognizer::clearIntents()` |
| `close` | function | `core/moonshine-cpp.h:1056` | `inline void Stream::close()` |
| `close` | function | `core/moonshine-cpp.h:1295` | `inline void Transcriber::close()` |
| `close` | function | `core/moonshine-cpp.h:1467` | `inline void TextToSpeech::close()` |
| `close` | function | `core/moonshine-cpp.h:1566` | `inline void GraphemeToPhonemizer::close()` |
| `close` | function | `core/moonshine-cpp.h:1699` | `inline void IntentRecognizer::close()` |
| `createStream` | function | `core/moonshine-cpp.h:1322` | `inline Stream Transcriber::createStream(double updateInterval, uint32_t flags)` |
| `emit` | function | `core/moonshine-cpp.h:1084` | `inline void Stream::emit(const TranscriptEvent &event)` |
| `emitError` | function | `core/moonshine-cpp.h:1168` | `inline void Stream::emitError(const std::string &errorMessage)` |
| `getClosestIntents` | function | `core/moonshine-cpp.h:1647` | `inline std::vector<IntentMatch> IntentRecognizer::getClosestIntents(     const std::string &utter...` |
| `getDefaultStream` | function | `core/moonshine-cpp.h:1326` | `inline Stream &Transcriber::getDefaultStream()` |
| `getDependencies` | function | `core/moonshine-cpp.h:1494` | `inline std::string TextToSpeech::getDependencies(     const std::string &languages,     const std...` |
| `getDependencies` | function | `core/moonshine-cpp.h:1573` | `inline std::string GraphemeToPhonemizer::getDependencies(     const std::string &languages,     c...` |
| `getHandle` | function | `core/moonshine-cpp.h:489` | `int32_t getHandle() const` |
| `getHandle` | function | `core/moonshine-cpp.h:641` | `int32_t getHandle() const` |
| `getHandle` | function | `core/moonshine-cpp.h:751` | `int32_t getHandle() const` |
| `getHandle` | function | `core/moonshine-cpp.h:837` | `int32_t getHandle() const` |
| `getHandle` | function | `core/moonshine-cpp.h:920` | `int32_t getHandle() const` |
| `getLanguage` | function | `core/moonshine-cpp.h:748` | `const std::string &getLanguage() const` |
| `getLanguage` | function | `core/moonshine-cpp.h:834` | `const std::string &getLanguage() const` |
| `getVersion` | function | `core/moonshine-cpp.h:1318` | `inline int32_t Transcriber::getVersion() const` |
| `getVoices` | function | `core/moonshine-cpp.h:1474` | `inline std::string TextToSpeech::getVoices(     const std::string &languages,     const std::vect...` |
| `intentCount` | function | `core/moonshine-cpp.h:1671` | `inline int32_t IntentRecognizer::intentCount() const` |
| `loadFromMemory` | function | `core/moonshine-cpp.h:1242` | `inline Transcriber Transcriber::loadFromMemory(     const uint8_t *encoderData, size_t encoderDat...` |
| `main` | function | `core/moonshine-cpp.h:24` | `*  * int main()` |
| `notifyFromTranscript` | function | `core/moonshine-cpp.h:1064` | `inline void Stream::notifyFromTranscript(const Transcript &transcript)` |
| `onError` | function | `core/moonshine-cpp.h:406` | `virtual void onError(const Error &)` |
| `onLineCompleted` | function | `core/moonshine-cpp.h:19` | `*     void onLineCompleted(const moonshine::LineCompleted& event) override` |
| `onLineCompleted` | function | `core/moonshine-cpp.h:403` | `virtual void onLineCompleted(const LineCompleted &)` |
| `onLineSpeakersChanged` | function | `core/moonshine-cpp.h:400` | `virtual void onLineSpeakersChanged(const LineSpeakersChanged &)` |
| `onLineStarted` | function | `core/moonshine-cpp.h:16` | `* public:  *     void onLineStarted(const moonshine::LineStarted& event) override` |
| `onLineStarted` | function | `core/moonshine-cpp.h:390` | `virtual void onLineStarted(const LineStarted &)` |
| `onLineTextChanged` | function | `core/moonshine-cpp.h:396` | `virtual void onLineTextChanged(const LineTextChanged &)` |
| `onLineUpdated` | function | `core/moonshine-cpp.h:393` | `virtual void onLineUpdated(const LineUpdated &)` |
| `parseTranscript` | function | `core/moonshine-cpp.h:1378` | `inline Transcript Transcriber::parseTranscript(     const transcript_t *transcript_c)` |
| `registerIntent` | function | `core/moonshine-cpp.h:1627` | `inline void IntentRecognizer::registerIntent(     const std::string &canonical_phrase, float *emb...` |
| `removeAllListeners` | function | `core/moonshine-cpp.h:1051` | `inline void Stream::removeAllListeners()` |
| `removeAllListeners` | function | `core/moonshine-cpp.h:1372` | `inline void Transcriber::removeAllListeners()` |
| `removeListener` | function | `core/moonshine-cpp.h:1022` | `inline void Stream::removeListener(TranscriptEventListener *listener)` |
| `removeListener` | function | `core/moonshine-cpp.h:1028` | `inline void Stream::removeListener(     std::function<void(const TranscriptEvent &)> listener)` |
| `removeListener` | function | `core/moonshine-cpp.h:1359` | `inline void Transcriber::removeListener(TranscriptEventListener *listener)` |
| `removeListener` | function | `core/moonshine-cpp.h:1365` | `inline void Transcriber::removeListener(     std::function<void(const TranscriptEvent &)> listener)` |
| `remove_if` | function | `core/moonshine-cpp.h:1034` | `std::remove_if(           functionListeners_.begin(), functionListeners_.end(),           [&liste...` |
| `start` | function | `core/moonshine-cpp.h:971` | `inline void Stream::start()` |
| `start` | function | `core/moonshine-cpp.h:1333` | `inline void Transcriber::start()` |
| `stop` | function | `core/moonshine-cpp.h:975` | `inline void Stream::stop()` |
| `stop` | function | `core/moonshine-cpp.h:1335` | `inline void Transcriber::stop()` |
| `synthesize` | function | `core/moonshine-cpp.h:1426` | `inline TtsSynthesisResult TextToSpeech::synthesize(     const std::string &text, const std::vecto...` |
| `synthesizeFromPhonemes` | function | `core/moonshine-cpp.h:1446` | `inline TtsSynthesisResult TextToSpeech::synthesizeFromPhonemes(     const std::string &phonemes, ...` |
| `toIpa` | function | `core/moonshine-cpp.h:1550` | `inline std::string GraphemeToPhonemizer::toIpa(     const std::string &text, const std::vector<mo...` |
| `toString` | function | `core/moonshine-cpp.h:233` | `std::string toString() const` |
| `toString` | function | `core/moonshine-cpp.h:283` | `std::string toString() const` |
| `transcribeWithoutStreaming` | function | `core/moonshine-cpp.h:1303` | `inline Transcript Transcriber::transcribeWithoutStreaming(     const std::vector<float> &audioDat...` |
| `transcriber` | function | `core/moonshine-cpp.h:25` | `* moonshine::Transcriber transcriber("path/to/models", * moonshine::ModelArch::BASE);` |
| `unregisterIntent` | function | `core/moonshine-cpp.h:1634` | `inline bool IntentRecognizer::unregisterIntent(     const std::string &canonical_phrase)` |
| `updateTranscription` | function | `core/moonshine-cpp.h:1002` | `inline Transcript Stream::updateTranscription(uint32_t flags)` |
| `updateTranscription` | function | `core/moonshine-cpp.h:1346` | `inline Transcript Transcriber::updateTranscription(uint32_t flags)` |
| `audio` | function | `core/moonshine-download-smoke.cpp:218` | `std::vector<float> audio(data, data + used);` |
| `csv` | function | `core/moonshine-download-smoke.cpp:176` | `const std::string csv(out);` |
| `fail` | function | `core/moonshine-download-smoke.cpp:73` | `int fail(const std::string& message)` |
| `is_streaming_arch` | function | `core/moonshine-download-smoke.cpp:234` | `bool is_streaming_arch(uint32_t arch)` |
| `load_speech_or_tone` | function | `core/moonshine-download-smoke.cpp:197` | `std::vector<float> load_speech_or_tone()` |
| `main` | function | `core/moonshine-download-smoke.cpp:388` | `int main(int argc, char** argv)` |
| `manifest_g2p` | function | `core/moonshine-download-smoke.cpp:166` | `int manifest_g2p(const std::vector<std::string>& spec)` |
| `manifest_intent` | function | `core/moonshine-download-smoke.cpp:115` | `int manifest_intent(const std::vector<std::string>& spec)` |
| `manifest_stt` | function | `core/moonshine-download-smoke.cpp:93` | `int manifest_stt(const std::vector<std::string>& spec)` |
| `manifest_tts` | function | `core/moonshine-download-smoke.cpp:135` | `int manifest_tts(const std::vector<std::string>& spec)` |
| `print_group_manifest` | function | `core/moonshine-download-smoke.cpp:82` | `void print_group_manifest(const std::string& json_text)` |
| `print_usage` | function | `core/moonshine-download-smoke.cpp:45` | `void print_usage()` |
| `run_g2p` | function | `core/moonshine-download-smoke.cpp:361` | `int run_g2p(const std::string& root, const std::vector<std::string>& spec)` |
| `run_intent` | function | `core/moonshine-download-smoke.cpp:295` | `int run_intent(const std::string& root, const std::vector<std::string>& spec)` |
| `run_stt` | function | `core/moonshine-download-smoke.cpp:241` | `int run_stt(const std::string& root, const std::vector<std::string>& spec)` |
| `run_tts` | function | `core/moonshine-download-smoke.cpp:323` | `int run_tts(const std::string& root, const std::vector<std::string>& spec)` |
| `url_encode_path` | function | `core/moonshine-download-smoke.cpp:53` | `std::string url_encode_path(const std::string& key)` |
| `EmbeddingModelEntry` | struct | `core/moonshine-model-catalog.cpp:33` | `` |
| `SpellingModelEntry` | struct | `core/moonshine-model-catalog.cpp:28` | `` |
| `SttLanguageEntry` | struct | `core/moonshine-model-catalog.cpp:22` | `` |
| `SttModelEntry` | struct | `core/moonshine-model-catalog.cpp:17` | `` |
| `embedding_catalog` | function | `core/moonshine-model-catalog.cpp:123` | `const std::vector<EmbeddingModelEntry>& embedding_catalog()` |
| `embedding_component_files` | function | `core/moonshine-model-catalog.cpp:194` | `std::vector<std::string> embedding_component_files(const std::string& variant)` |
| `find_embedding_model` | function | `core/moonshine-model-catalog.cpp:179` | `const EmbeddingModelEntry* find_embedding_model(const std::string& model_name)` |
| `find_spelling_model` | function | `core/moonshine-model-catalog.cpp:170` | `const SpellingModelEntry* find_spelling_model(const std::string& language_code)` |
| `find_stt_language` | function | `core/moonshine-model-catalog.cpp:133` | `const SttLanguageEntry* find_stt_language(const std::string& language)` |
| `intent_model_dependencies` | function | `core/moonshine-model-catalog.cpp:251` | `std::optional<ModelDependencies> intent_model_dependencies(     const std::string& model_name, co...` |
| `intent_supported_models` | function | `core/moonshine-model-catalog.cpp:281` | `std::vector<std::string> intent_supported_models()` |
| `intent_supported_variants` | function | `core/moonshine-model-catalog.cpp:289` | `std::vector<std::string> intent_supported_variants(     const std::string& model_name)` |
| `is_streaming_arch` | function | `core/moonshine-model-catalog.cpp:47` | `bool is_streaming_arch(int32_t model_arch)` |
| `stt_catalog` | function | `core/moonshine-model-catalog.cpp:56` | `const std::vector<SttLanguageEntry>& stt_catalog()` |
| `stt_component_files` | function | `core/moonshine-model-catalog.cpp:148` | `std::vector<std::string> stt_component_files(const std::string& language_code,                   ...` |
| `stt_model_dependencies` | function | `core/moonshine-model-catalog.cpp:214` | `std::optional<ModelDependencies> stt_model_dependencies(     const std::string& language, std::op...` |
| `stt_supported_languages` | function | `core/moonshine-model-catalog.cpp:273` | `std::vector<std::string> stt_supported_languages()` |
| `to_lower` | function | `core/moonshine-model-catalog.cpp:40` | `std::string to_lower(std::string s)` |
| `transform` | function | `core/moonshine-model-catalog.cpp:41` | `std::transform(s.begin(), s.end(), s.begin(), [](unsigned char c)` |
| `MOONSHINE_MODEL_CATALOG_H` | macro | `core/moonshine-model-catalog.h:2` | `#define MOONSHINE_MODEL_CATALOG_H` |
| `ModelDependencies` | struct | `core/moonshine-model-catalog.h:29` | `` |
| `ModelDependencyGroup` | struct | `core/moonshine-model-catalog.h:24` | `` |
| `DEBUG_ALLOC_ENABLED` | macro | `core/moonshine-model.cpp:36` | `#define DEBUG_ALLOC_ENABLED` |
| `MOONSHINE_BASE_HEAD_DIM` | macro | `core/moonshine-model.cpp:51` | `#define MOONSHINE_BASE_HEAD_DIM` |
| `MOONSHINE_BASE_NUM_KV_HEADS` | macro | `core/moonshine-model.cpp:50` | `#define MOONSHINE_BASE_NUM_KV_HEADS` |
| `MOONSHINE_BASE_NUM_LAYERS` | macro | `core/moonshine-model.cpp:49` | `#define MOONSHINE_BASE_NUM_LAYERS` |
| `MOONSHINE_BASE_PAST_ELEMENT_COUNT` | macro | `core/moonshine-model.cpp:53` | `#define MOONSHINE_BASE_PAST_ELEMENT_COUNT` |
| `MOONSHINE_DECODER_START_TOKEN_ID` | macro | `core/moonshine-model.cpp:56` | `#define MOONSHINE_DECODER_START_TOKEN_ID` |
| `MOONSHINE_EOS_TOKEN_ID` | macro | `core/moonshine-model.cpp:57` | `#define MOONSHINE_EOS_TOKEN_ID` |
| `MOONSHINE_TINY_HEAD_DIM` | macro | `core/moonshine-model.cpp:43` | `#define MOONSHINE_TINY_HEAD_DIM` |
| `MOONSHINE_TINY_NUM_KV_HEADS` | macro | `core/moonshine-model.cpp:42` | `#define MOONSHINE_TINY_NUM_KV_HEADS` |
| `MOONSHINE_TINY_NUM_LAYERS` | macro | `core/moonshine-model.cpp:41` | `#define MOONSHINE_TINY_NUM_LAYERS` |
| `MOONSHINE_TINY_PAST_ELEMENT_COUNT` | macro | `core/moonshine-model.cpp:45` | `#define MOONSHINE_TINY_PAST_ELEMENT_COUNT` |
| `MoonshineModel` | function | `core/moonshine-model.cpp:82` | `MoonshineModel::MoonshineModel(     bool log_ort_run, float max_tokens_per_second,     const std:...` |
| `attn_shape` | function | `core/moonshine-model.cpp:732` | `std::vector<int64_t> attn_shape(attn_ndims);` |
| `compute_word_timestamps` | function | `core/moonshine-model.cpp:591` | `int MoonshineModel::compute_word_timestamps(     float audio_duration, std::vector<TranscriberWor...` |
| `cross_attention_data` | function | `core/moonshine-model.cpp:744` | `std::vector<float> cross_attention_data(attn_layers * per_layer);` |
| `decoder_input_names` | function | `core/moonshine-model.cpp:326` | `std::vector<const char *> decoder_input_names(decoder_input_count);` |
| `decoder_inputs_data` | function | `core/moonshine-model.cpp:382` | `std::vector<MoonshineTensorView *> decoder_inputs_data(decoder_input_count);` |
| `decoder_output_names` | function | `core/moonshine-model.cpp:338` | `std::vector<const char *> decoder_output_names(decoder_output_count);` |
| `decoder_outputs` | function | `core/moonshine-model.cpp:442` | `std::vector<OrtValue *> decoder_outputs(decoder_output_count);` |
| `encoder_input_names` | function | `core/moonshine-model.cpp:231` | `std::vector<char *> encoder_input_names(encoder_input_count);` |
| `encoder_output_names` | function | `core/moonshine-model.cpp:232` | `std::vector<char *> encoder_output_names(encoder_output_count);` |
| `encoder_outputs` | function | `core/moonshine-model.cpp:268` | `std::vector<OrtValue *> encoder_outputs(encoder_output_count);` |
| `load` | function | `core/moonshine-model.cpp:145` | `int MoonshineModel::load(const char *encoder_model_path,                          const char *dec...` |
| `load_alignment_model` | function | `core/moonshine-model.cpp:580` | `int MoonshineModel::load_alignment_model(const char *alignment_model_path)` |
| `load_from_assets` | function | `core/moonshine-model.cpp:186` | `int MoonshineModel::load_from_assets(const char *encoder_model_path,                             ...` |
| `load_from_memory` | function | `core/moonshine-model.cpp:163` | `int MoonshineModel::load_from_memory(const uint8_t *encoder_model_data,                          ...` |
| `output_names` | function | `core/moonshine-model.cpp:686` | `std::vector<const char *> output_names(align_output_count);` |
| `output_names_alloc` | function | `core/moonshine-model.cpp:679` | `std::vector<char *> output_names_alloc(align_output_count);` |
| `outputs` | function | `core/moonshine-model.cpp:692` | `std::vector<OrtValue *> outputs(align_output_count, nullptr);` |
| `rearranged` | function | `core/moonshine-model.cpp:613` | `std::vector<float> rearranged(L * H * total_steps * E);` |
| `set_model_options_from_arch` | function | `core/moonshine-model.cpp:60` | `int set_model_options_from_arch(MoonshineModel *model, int32_t model_arch)` |
| `tokens_int` | function | `core/moonshine-model.cpp:601` | `std::vector<int> tokens_int(last_tokens.begin(), last_tokens.end());` |
| `transcribe` | function | `core/moonshine-model.cpp:216` | `int MoonshineModel::transcribe(const float *input_audio_data,                                size...` |
| `transcribe_wav` | function | `core/moonshine-model.cpp:565` | `int MoonshineModel::transcribe_wav(const char *wav_path, char **out_text)` |
| `MOONSHINE_MODEL_H` | macro | `core/moonshine-model.h:2` | `#define MOONSHINE_MODEL_H` |
| `MoonshineModel` | struct | `core/moonshine-model.h:17` | `` |
| `compute_word_timestamps` | function | `core/moonshine-model.h:101` | `int compute_word_timestamps(float audio_duration, std::vector<TranscriberWord> &words_out);` |
| `load` | function | `core/moonshine-model.h:72` | `int load(const char *encoder_model_path, const char *decoder_model_path, const char *tokenizer_path, int32_t...` |
| `load_alignment_model` | function | `core/moonshine-model.h:75` | `int load_alignment_model(const char *alignment_model_path);` |
| `load_from_assets` | function | `core/moonshine-model.h:85` | `int load_from_assets(const char *encoder_model_path, const char *decoder_model_path, const char *tokenizer_path...` |
| `load_from_memory` | function | `core/moonshine-model.h:77` | `int load_from_memory(const uint8_t *encoder_model_data, size_t encoder_model_data_size, const uint8_t...` |
| `transcribe` | function | `core/moonshine-model.h:91` | `int transcribe(const float *input_audio_data, size_t input_audio_data_size, char **out_text);` |
| `transcribe_wav` | function | `core/moonshine-model.h:94` | `int transcribe_wav(const char *wav_path, char **out_text);` |
| `DEBUG_ALLOC_ENABLED` | macro | `core/moonshine-streaming-model.cpp:24` | `#define DEBUG_ALLOC_ENABLED` |
| `MOONSHINE_DECODER_START_TOKEN_ID` | macro | `core/moonshine-streaming-model.cpp:41` | `#define MOONSHINE_DECODER_START_TOKEN_ID` |
| `MOONSHINE_EOS_TOKEN_ID` | macro | `core/moonshine-streaming-model.cpp:42` | `#define MOONSHINE_EOS_TOKEN_ID` |
| `MOONSHINE_STREAMING_BASE_DECODER_DIM` | macro | `core/moonshine-streaming-model.cpp:36` | `#define MOONSHINE_STREAMING_BASE_DECODER_DIM` |
| `MOONSHINE_STREAMING_BASE_DEPTH` | macro | `core/moonshine-streaming-model.cpp:37` | `#define MOONSHINE_STREAMING_BASE_DEPTH` |
| `MOONSHINE_STREAMING_BASE_ENCODER_DIM` | macro | `core/moonshine-streaming-model.cpp:35` | `#define MOONSHINE_STREAMING_BASE_ENCODER_DIM` |
| `MOONSHINE_STREAMING_BASE_HEAD_DIM` | macro | `core/moonshine-streaming-model.cpp:39` | `#define MOONSHINE_STREAMING_BASE_HEAD_DIM` |
| `MOONSHINE_STREAMING_BASE_NHEADS` | macro | `core/moonshine-streaming-model.cpp:38` | `#define MOONSHINE_STREAMING_BASE_NHEADS` |
| `MOONSHINE_STREAMING_TINY_DECODER_DIM` | macro | `core/moonshine-streaming-model.cpp:30` | `#define MOONSHINE_STREAMING_TINY_DECODER_DIM` |
| `MOONSHINE_STREAMING_TINY_DEPTH` | macro | `core/moonshine-streaming-model.cpp:31` | `#define MOONSHINE_STREAMING_TINY_DEPTH` |
| `MOONSHINE_STREAMING_TINY_ENCODER_DIM` | macro | `core/moonshine-streaming-model.cpp:29` | `#define MOONSHINE_STREAMING_TINY_ENCODER_DIM` |
| `MOONSHINE_STREAMING_TINY_HEAD_DIM` | macro | `core/moonshine-streaming-model.cpp:33` | `#define MOONSHINE_STREAMING_TINY_HEAD_DIM` |
| `MOONSHINE_STREAMING_TINY_NHEADS` | macro | `core/moonshine-streaming-model.cpp:32` | `#define MOONSHINE_STREAMING_TINY_NHEADS` |
| `MoonshineStreamingModel` | function | `core/moonshine-streaming-model.cpp:146` | `MoonshineStreamingModel::MoonshineStreamingModel(     bool log_ort_run, const std::vector<std::st...` |
| `attn_shape` | function | `core/moonshine-streaming-model.cpp:1022` | `std::vector<int64_t> attn_shape(attn_ndims);` |
| `audio_vec` | function | `core/moonshine-streaming-model.cpp:442` | `std::vector<float> audio_vec(audio_chunk, audio_chunk + chunk_len);` |
| `compute_cross_kv` | function | `core/moonshine-streaming-model.cpp:759` | `int MoonshineStreamingModel::compute_cross_kv(MoonshineStreamingState *state)` |
| `create_state` | function | `core/moonshine-streaming-model.cpp:405` | `MoonshineStreamingState *MoonshineStreamingModel::create_state()` |
| `decode_full` | function | `core/moonshine-streaming-model.cpp:1172` | `int MoonshineStreamingModel::decode_full(MoonshineStreamingState *state,                         ...` |
| `decode_step` | function | `core/moonshine-streaming-model.cpp:1069` | `int MoonshineStreamingModel::decode_step(MoonshineStreamingState *state,                         ...` |
| `decode_tokens` | function | `core/moonshine-streaming-model.cpp:1116` | `int MoonshineStreamingModel::decode_tokens(MoonshineStreamingState *state,                       ...` |
| `decoder_reset` | function | `core/moonshine-streaming-model.cpp:1344` | `void MoonshineStreamingModel::decoder_reset(MoonshineStreamingState *state)` |
| `enc_shape` | function | `core/moonshine-streaming-model.cpp:667` | `std::vector<int64_t> enc_shape(num_dims);` |
| `encode` | function | `core/moonshine-streaming-model.cpp:584` | `int MoonshineStreamingModel::encode(MoonshineStreamingState *state,                              ...` |
| `feat_shape` | function | `core/moonshine-streaming-model.cpp:529` | `std::vector<int64_t> feat_shape(num_dims);` |
| `k_shape` | function | `core/moonshine-streaming-model.cpp:803` | `std::vector<int64_t> k_shape(num_dims);` |
| `load` | function | `core/moonshine-streaming-model.cpp:217` | `int MoonshineStreamingModel::load(const char *model_dir,                                   const ...` |
| `load_config` | function | `core/moonshine-streaming-model.cpp:200` | `int MoonshineStreamingModel::load_config(const char *config_path)` |
| `load_config_from_string` | function | `core/moonshine-streaming-model.cpp:209` | `int MoonshineStreamingModel::load_config_from_string(const std::string &json)` |
| `load_from_assets` | function | `core/moonshine-streaming-model.cpp:332` | `int MoonshineStreamingModel::load_from_assets(const char *model_dir,                             ...` |
| `load_from_memory` | function | `core/moonshine-streaming-model.cpp:290` | `int MoonshineStreamingModel::load_from_memory(     const uint8_t *frontend_model_data, size_t fro...` |
| `new_encoded` | function | `core/moonshine-streaming-model.cpp:686` | `std::vector<float> new_encoded(new_frames * config.encoder_dim);` |
| `output_names_alloc` | function | `core/moonshine-streaming-model.cpp:932` | `std::vector<char *> output_names_alloc(decoder_output_count);` |
| `outputs` | function | `core/moonshine-streaming-model.cpp:945` | `std::vector<OrtValue *> outputs(decoder_output_count, nullptr);` |
| `parse_config_json` | function | `core/moonshine-streaming-model.cpp:58` | `static bool parse_config_json(const std::string &json,                               MoonshineStr...` |
| `process_audio_chunk` | function | `core/moonshine-streaming-model.cpp:421` | `int MoonshineStreamingModel::process_audio_chunk(MoonshineStreamingState *state,                 ...` |
| `read_file_to_string` | function | `core/moonshine-streaming-model.cpp:49` | `static std::string read_file_to_string(const std::string &path)` |
| `reset` | function | `core/moonshine-streaming-model.cpp:107` | `void MoonshineStreamingState::reset(const MoonshineStreamingConfig &cfg)` |
| `run_decoder_with_cross_kv` | function | `core/moonshine-streaming-model.cpp:847` | `int MoonshineStreamingModel::run_decoder_with_cross_kv(     MoonshineStreamingState *state, const...` |
| `token_data` | function | `core/moonshine-streaming-model.cpp:865` | `std::vector<int64_t> token_data(tokens.begin(), tokens.end());` |
| `token_vec` | function | `core/moonshine-streaming-model.cpp:1138` | `std::vector<int64_t> token_vec(tokens_len);` |
| `tokens_to_text` | function | `core/moonshine-streaming-model.cpp:411` | `std::string MoonshineStreamingModel::tokens_to_text(     const std::vector<int64_t> &tokens)` |
| `MOONSHINE_STREAMING_MODEL_H` | macro | `core/moonshine-streaming-model.h:2` | `#define MOONSHINE_STREAMING_MODEL_H` |
| `MoonshineStreamingConfig` | struct | `core/moonshine-streaming-model.h:17` | `` |
| `MoonshineStreamingModel` | struct | `core/moonshine-streaming-model.h:72` | `` |
| `MoonshineStreamingState` | struct | `core/moonshine-streaming-model.h:35` | `` |
| `compute_cross_kv` | function | `core/moonshine-streaming-model.h:182` | `int compute_cross_kv(MoonshineStreamingState *state);` |
| `create_state` | function | `core/moonshine-streaming-model.h:167` | `MoonshineStreamingState *create_state();` |
| `decode_full` | function | `core/moonshine-streaming-model.h:161` | `int decode_full(MoonshineStreamingState *state, const int *speculative_tokens, int speculative_len, int...` |
| `decode_step` | function | `core/moonshine-streaming-model.h:147` | `int decode_step(MoonshineStreamingState *state, int token, float *logits_out);` |
| `decoder_reset` | function | `core/moonshine-streaming-model.h:164` | `void decoder_reset(MoonshineStreamingState *state);` |
| `encode` | function | `core/moonshine-streaming-model.h:143` | `int encode(MoonshineStreamingState *state, bool is_final, int *new_frames_out);` |
| `load` | function | `core/moonshine-streaming-model.h:117` | `int load(const char *model_dir, const char *tokenizer_path, int32_t model_type);` |
| `load_config` | function | `core/moonshine-streaming-model.h:173` | `private: int load_config(const char *config_path);` |
| `load_config_from_string` | function | `core/moonshine-streaming-model.h:174` | `int load_config_from_string(const std::string &json);` |
| `load_from_assets` | function | `core/moonshine-streaming-model.h:130` | `int load_from_assets(const char *model_dir, const char *tokenizer_path, int32_t model_type, AAssetManager...` |
| `load_from_memory` | function | `core/moonshine-streaming-model.h:120` | `int load_from_memory( const uint8_t *frontend_model_data, size_t frontend_model_data_size, const uint8_t...` |
| `process_audio_chunk` | function | `core/moonshine-streaming-model.h:139` | `int process_audio_chunk(MoonshineStreamingState *state, const float *audio_chunk, size_t chunk_len, int *features_out);` |
| `reset` | function | `core/moonshine-streaming-model.h:69` | `void reset(const MoonshineStreamingConfig &cfg);` |
| `run_decoder_with_cross_kv` | function | `core/moonshine-streaming-model.h:177` | `int run_decoder_with_cross_kv(MoonshineStreamingState *state, const std::vector<int64_t> &tokens, std::vector<float>...` |
| `transcribe` | function | `core/moonshine-streaming-model.h:135` | `int transcribe(const float *input_audio_data, size_t input_audio_data_size, char **out_text);` |
| `MOONSHINE_TTS_CONSTANTS_H` | macro | `core/moonshine-tts/src/constants.h:2` | `#define MOONSHINE_TTS_CONSTANTS_H` |
| `FileInformation` | function | `core/moonshine-tts/src/file-information.cpp:8` | `FileInformation::FileInformation(const FileInformation& o)     : path(o.path), owned_storage_(o.o...` |
| `free` | function | `core/moonshine-tts/src/file-information.cpp:81` | `void FileInformation::free()` |
| `load` | function | `core/moonshine-tts/src/file-information.cpp:35` | `void FileInformation::load(const uint8_t** out_memory, size_t* out_size)` |
| `parse_file_list` | function | `core/moonshine-tts/src/file-information.cpp:99` | `void FileInformationMap::parse_file_list(     const std::vector<std::pair<std::string, std::strin...` |
| `set_memory` | function | `core/moonshine-tts/src/file-information.cpp:90` | `void FileInformationMap::set_memory(std::string_view key, const uint8_t* mem,                    ...` |
| `FileInformation` | struct | `core/moonshine-tts/src/file-information.h:18` | `` |
| `FileInformation` | function | `core/moonshine-tts/src/file-information.h:24` | `FileInformation(std::filesystem::path p, const uint8_t* mem, size_t sz)       : path(std::move(p)...` |
| `FileInformationMap` | struct | `core/moonshine-tts/src/file-information.h:51` | `` |
| `MOONSHINE_TTS_FILE_INFORMATION_H` | macro | `core/moonshine-tts/src/file-information.h:2` | `#define MOONSHINE_TTS_FILE_INFORMATION_H` |
| `contains` | function | `core/moonshine-tts/src/file-information.h:65` | `bool contains(std::string_view key) const` |
| `erase_key` | function | `core/moonshine-tts/src/file-information.h:63` | `void erase_key(std::string_view key)` |
| `free` | function | `core/moonshine-tts/src/file-information.h:40` | `void free();` |
| `load` | function | `core/moonshine-tts/src/file-information.h:35` | `void load(const uint8_t** out_memory, size_t* out_size);` |
| `parse_file_list` | function | `core/moonshine-tts/src/file-information.h:71` | `void parse_file_list( const std::vector<std::pair<std::string, std::string>>* key_list, const std::vector<uint8_t*>*...` |
| `set_path` | function | `core/moonshine-tts/src/file-information.h:54` | `void set_path(std::string_view key, std::filesystem::path path)` |
| `MOONSHINE_TTS_G2P_PATH_H` | macro | `core/moonshine-tts/src/g2p-path.h:2` | `#define MOONSHINE_TTS_G2P_PATH_H` |
| `b` | function | `core/moonshine-tts/src/g2p-path.h:33` | `const std::string b(basename);` |
| `resolve_disk_model_file_path` | function | `core/moonshine-tts/src/g2p-path.h:56` | `inline void resolve_disk_model_file_path(std::filesystem::path& path)` |
| `resolve_path_under_root` | function | `core/moonshine-tts/src/g2p-path.h:13` | `inline std::filesystem::path resolve_path_under_root(     const std::filesystem::path& root, cons...` |
| `resolve_prefer_ort_model` | function | `core/moonshine-tts/src/g2p-path.h:30` | `inline std::filesystem::path resolve_prefer_ort_model(     const std::filesystem::path& dir, std:...` |
| `format_g2p_word_log_line` | function | `core/moonshine-tts/src/g2p-word-log.cpp:35` | `std::string format_g2p_word_log_line(const G2pWordLog& e)` |
| `g2p_word_path_tag` | function | `core/moonshine-tts/src/g2p-word-log.cpp:7` | `const char* g2p_word_path_tag(G2pWordPath path)` |
| `G2pWordLog` | struct | `core/moonshine-tts/src/g2p-word-log.h:29` | `` |
| `G2pWordPath` | enum | `core/moonshine-tts/src/g2p-word-log.h:11` | `` |
| `G2pWordPath` | class | `core/moonshine-tts/src/g2p-word-log.h:11` | `` |
| `MOONSHINE_TTS_G2P_WORD_LOG_H` | macro | `core/moonshine-tts/src/g2p-word-log.h:2` | `#define MOONSHINE_TTS_G2P_WORD_LOG_H` |
| `g2p_word_path_tag` | function | `core/moonshine-tts/src/g2p-word-log.h:27` | `const char* g2p_word_path_tag(G2pWordPath path);` |
| `0` | variable | `core/moonshine-tts/src/ipa-postprocess.cpp:5` | `extern "C" { #include <utf8proc.h> } #include <algorithm> #include <cctype> #include <cstddef> #include <cstdlib>...` |
| `apply_german_ipa_piper_style` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:76` | `void apply_german_ipa_piper_style(std::string& s)` |
| `apply_korean_post_normalize_ipa` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:54` | `void apply_korean_post_normalize_ipa(std::string& s)` |
| `apply_lang_specific_replacements` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:106` | `void apply_lang_specific_replacements(std::string& s,                                       std::...` |
| `apply_russian_ipa_piper_style` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:276` | `void apply_russian_ipa_piper_style(std::string& s)` |
| `apply_shared_g2p_to_piper_replacements` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:46` | `void apply_shared_g2p_to_piper_replacements(std::string& s)` |
| `category_is_mn_or_me` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:175` | `bool category_is_mn_or_me(char32_t cp)` |
| `coerce_unknown_ipa_chars_to_piper_inventory` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:690` | `std::string coerce_unknown_ipa_chars_to_piper_inventory(     std::string_view ipa_utf8,     const...` |
| `cur` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:817` | `std::vector<int> cur(static_cast<size_t>(lb + 1));` |
| `ipa_string_to_phoneme_tokens` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:780` | `std::vector<std::string> ipa_string_to_phoneme_tokens(const std::string& s)` |
| `ipa_to_piper_ready` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:762` | `std::string ipa_to_piper_ready(     std::string_view ipa_utf8, std::string_view piper_lang_key,  ...` |
| `is_cmn_tone_marker` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:416` | `bool is_cmn_tone_marker(char32_t cp)` |
| `is_cmn_vowel_cp` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:394` | `bool is_cmn_vowel_cp(char32_t cp)` |
| `is_ipa_like_inventory_char` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:181` | `bool is_ipa_like_inventory_char(char32_t cp)` |
| `kAcute` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:231` | `static const std::string kAcute("\xcc\x81");` |
| `kAlveolarTap` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:93` | `static const std::string kAlveolarTap("\xc9\xbe");` |
| `kBar` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:77` | `static const std::string kBar("\xcd\xa1");` |
| `kEng` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:515` | `static const std::string kEng("\xc5\x8b");` |
| `kIsp` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:356` | `static const std::string kIsp("\xc9\xaa ");` |
| `kPrecomposedCcedilla` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:371` | `static const std::string kPrecomposedCcedilla("\xc3\xa7");` |
| `kPri` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:232` | `static const std::string kPri("\xcb\x88");` |
| `kSec` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:233` | `static const std::string kSec( "\xcb\x8c");` |
| `kStress` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:602` | `static const std::string kStress("\xcb\x88");` |
| `kTurnedACombBreve` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:92` | `static const std::string kTurnedACombBreve("\xc9\x90\xcc\xaf");` |
| `kUvuR` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:97` | `static const std::string kUvuR("\xca\x81");` |
| `kZhd` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:336` | `static const std::string kZhd("\xca\x90");` |
| `kZhj` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:337` | `static const std::string kZhj("\xca\x92");` |
| `key` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:141` | `const std::string key(eff);` |
| `levenshtein_distance` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:806` | `int levenshtein_distance(const std::vector<std::string>& a,                          const std::v...` |
| `match_prediction_to_cmudict_ipa` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:882` | `std::optional<std::string> match_prediction_to_cmudict_ipa(     const std::string& predicted, con...` |
| `normalize_chinese_ipa_piper_style` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:421` | `std::string normalize_chinese_ipa_piper_style(std::string ipa)` |
| `normalize_g2p_ipa_for_piper` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:672` | `std::string normalize_g2p_ipa_for_piper(std::string_view ipa_utf8,                               ...` |
| `normalize_g2p_ipa_for_piper_engines` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:774` | `std::string normalize_g2p_ipa_for_piper_engines(std::string_view ipa_utf8)` |
| `normalize_german_ipa_piper_style` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:384` | `std::string normalize_german_ipa_piper_style(std::string ipa)` |
| `normalize_russian_ipa_piper_style` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:379` | `std::string normalize_russian_ipa_piper_style(std::string ipa)` |
| `pick_closest_alternative_index` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:837` | `int pick_closest_alternative_index(     const std::vector<std::string>& predicted_phoneme_tokens,...` |
| `pick_closest_cmudict_ipa` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:866` | `std::string pick_closest_cmudict_ipa(     const std::vector<std::string>& predicted_phoneme_token...` |
| `prev` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:816` | `std::vector<int> prev(static_cast<size_t>(lb + 1));` |
| `py_isspace_one_utf8_char` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:151` | `bool py_isspace_one_utf8_char(std::string_view ch)` |
| `repair_ascii_c_combining_cedilla_to_ccedilla_utf8` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:368` | `void repair_ascii_c_combining_cedilla_to_ccedilla_utf8(std::string& s)` |
| `replace_utf8_all` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:21` | `void replace_utf8_all(std::string& s, std::string_view old_utf8,                       std::strin...` |
| `rewrite_russian_combining_acute_to_primary_stress` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:230` | `void rewrite_russian_combining_acute_to_primary_stress(std::string& s)` |
| `strip_length_markers_copy` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:37` | `std::string strip_length_markers_copy(std::string t)` |
| `tmp` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:661` | `const std::string tmp(s);` |
| `trim_copy` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:30` | `std::string trim_copy(std::string t)` |
| `unicode_category_first_char_is_p_or_s` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:170` | `bool unicode_category_first_char_is_p_or_s(char32_t cp)` |
| `utf8_nfc_copy` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:660` | `std::string utf8_nfc_copy(std::string_view s)` |
| `utf8_prev_codepoint_start` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:216` | `size_t utf8_prev_codepoint_start(const std::string& s, size_t char_start)` |
| `utf8_singleton_codepoint` | function | `core/moonshine-tts/src/ipa-postprocess.cpp:206` | `char32_t utf8_singleton_codepoint(std::string_view token)` |
| `MOONSHINE_TTS_IPA_POSTPROCESS_H` | macro | `core/moonshine-tts/src/ipa-postprocess.h:2` | `#define MOONSHINE_TTS_IPA_POSTPROCESS_H` |
| `levenshtein_distance` | function | `core/moonshine-tts/src/ipa-postprocess.h:68` | `int levenshtein_distance(const std::vector<std::string>& a, const std::vector<std::string>& b);` |
| `pick_closest_alternative_index` | function | `core/moonshine-tts/src/ipa-postprocess.h:71` | `int pick_closest_alternative_index( const std::vector<std::string>& predicted_phoneme_tokens, const...` |
| `repair_ascii_c_combining_cedilla_to_ccedilla_utf8` | function | `core/moonshine-tts/src/ipa-postprocess.h:19` | `void repair_ascii_c_combining_cedilla_to_ccedilla_utf8(std::string& ipa_utf8);` |
| `load_oov_tables` | function | `core/moonshine-tts/src/json-config.cpp:88` | `OovOnnxTables load_oov_tables(const std::filesystem::path& model_onnx_path)` |
| `load_oov_tables_from_json` | function | `core/moonshine-tts/src/json-config.cpp:64` | `OovOnnxTables load_oov_tables_from_json(const nlohmann::json& cfg,                               ...` |
| `read_json_file` | function | `core/moonshine-tts/src/json-config.cpp:14` | `nlohmann::json read_json_file(const std::filesystem::path& p)` |
| `stoi_to_itos` | function | `core/moonshine-tts/src/json-config.cpp:47` | `std::vector<std::string> stoi_to_itos(     const std::unordered_map<std::string, int64_t>& stoi)` |
| `validate_header` | function | `core/moonshine-tts/src/json-config.cpp:24` | `void validate_header(const nlohmann::json& cfg, const std::string& expect_kind,                  ...` |
| `MOONSHINE_TTS_JSON_CONFIG_H` | macro | `core/moonshine-tts/src/json-config.h:2` | `#define MOONSHINE_TTS_JSON_CONFIG_H` |
| `OovOnnxTables` | struct | `core/moonshine-tts/src/json-config.h:15` | `` |
| `ArabicDiacOnnx` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:726` | `ArabicDiacOnnx::ArabicDiacOnnx(const MoonshineG2POptions* opt,                                std...` |
| `BasicTokCfg` | struct | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:315` | `` |
| `EncodedWp` | struct | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:427` | `` |
| `Idx` | struct | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:517` | `` |
| `align_basic_tokens_u32` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:362` | `void align_basic_tokens_u32(const std::u32string& ref,                             const std::vec...` |
| `anchor_index_for_span` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:686` | `std::optional<int> anchor_index_for_span(const std::u32string& ref, int s,                       ...` |
| `basic_tokenize_u32` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:330` | `std::vector<std::u32string> basic_tokenize_u32(     const std::u32string& original_text_u32, cons...` |
| `buf` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:628` | `const std::string buf(utf8);` |
| `bundle_load_binary_ar` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:94` | `bool bundle_load_binary_ar(const MoonshineG2POptions* opt,                            std::string...` |
| `bundle_load_utf8_ar` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:75` | `bool bundle_load_utf8_ar(const MoonshineG2POptions* opt,                          std::string_vie...` |
| `chars` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:389` | `std::vector<char32_t> chars(wt.begin(), wt.end());` |
| `clean_text_u32` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:234` | `std::u32string clean_text_u32(const std::u32string& text)` |
| `diacritize` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:787` | `std::string ArabicDiacOnnx::diacritize(std::string_view text_utf8) const` |
| `encode_bert_wordpiece` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:434` | `EncodedWp encode_bert_wordpiece(     const std::u32string& text_u32,     const std::unordered_map...` |
| `inner` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:821` | `std::vector<int64_t> inner(enc.input_ids.begin() + 1, enc.input_ids.end() - 1);` |
| `is_arabic_anchor_char` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:672` | `bool is_arabic_anchor_char(char32_t c)` |
| `is_chinese_char` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:184` | `bool is_chinese_char(std::uint32_t cp)` |
| `is_control_u32` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:157` | `bool is_control_u32(char32_t c)` |
| `is_punct_char_word_group_u32` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:179` | `bool is_punct_char_word_group_u32(char32_t c)` |
| `is_punctuation_u32` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:166` | `bool is_punctuation_u32(char32_t c)` |
| `is_space_u32` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:148` | `bool is_space_u32(char32_t c)` |
| `mask` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:844` | `std::vector<int64_t> mask(static_cast<size_t>(T), 1);` |
| `normalization_ref_u32` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:321` | `std::u32string normalization_ref_u32(const std::u32string& text_u32,                             ...` |
| `open_ar_session` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:34` | `std::unique_ptr<Ort::Session> open_ar_session(     Ort::Env& env, const std::filesystem::path& mo...` |
| `open_ar_session_memory` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:51` | `std::unique_ptr<Ort::Session> open_ar_session_memory(     Ort::Env& env, const void* data, size_t...` |
| `run_split_on_punc_u32` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:285` | `std::vector<std::u32string> run_split_on_punc_u32(const std::u32string& text)` |
| `slurp_utf8_file_ar` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:65` | `std::string slurp_utf8_file_ar(const std::filesystem::path& p)` |
| `split_u32_whitespace` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:260` | `std::vector<std::u32string> split_u32_whitespace(std::u32string_view s)` |
| `strip_arabic_diacritics_u32` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:700` | `std::u32string strip_arabic_diacritics_u32(const std::u32string& s)` |
| `strip_mn_nfd` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:205` | `std::u32string strip_mn_nfd(const std::u32string& s)` |
| `to_lower_u32` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:225` | `std::u32string to_lower_u32(const std::u32string& s)` |
| `tokenize_chinese_chars_u32` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:246` | `std::u32string tokenize_chinese_chars_u32(const std::u32string& text)` |
| `u32_nfc` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:193` | `std::u32string u32_nfc(const std::u32string& s)` |
| `u32_to_utf8` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:140` | `std::string u32_to_utf8(const std::u32string& s)` |
| `utf8_to_u32` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:127` | `std::u32string utf8_to_u32(std::string_view utf8)` |
| `wordpiece_tokenize_u32` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:379` | `std::vector<std::u32string> wordpiece_tokenize_u32(     const std::u32string& token,     const st...` |
| `ArabicDiacOnnx` | class | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.h:20` | `` |
| `MOONSHINE_TTS_ARABIC_DIAC_ONNX_H` | macro | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.h:2` | `#define MOONSHINE_TTS_ARABIC_DIAC_ONNX_H` |
| `MoonshineG2POptions` | struct | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.h:16` | `` |
| `model_dir` | function | `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.h:39` | `const std::filesystem::path& model_dir() const` |
| `apply_default_fatha_u32` | function | `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:160` | `std::u32string apply_default_fatha_u32(const std::u32string& w)` |
| `arabic_msa_apply_onnx_partial_postprocess_utf8` | function | `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:407` | `std::string arabic_msa_apply_onnx_partial_postprocess_utf8(     std::string_view utf8)` |
| `arabic_msa_strip_diacritics_utf8` | function | `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:402` | `std::string arabic_msa_strip_diacritics_utf8(std::string_view utf8)` |
| `arabic_msa_word_to_ipa_with_assimilation_utf8` | function | `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:415` | `std::string arabic_msa_word_to_ipa_with_assimilation_utf8(     std::string_view filled_diac_utf8,...` |
| `diac_word_to_ipa_u32` | function | `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:320` | `std::string diac_word_to_ipa_u32(const std::u32string& word)` |
| `gem_ipa` | function | `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:309` | `std::string gem_ipa(const std::string& onset)` |
| `has_vowel_mark_u32` | function | `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:87` | `bool has_vowel_mark_u32(const std::u32string& marks)` |
| `is_ar_base_letter` | function | `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:36` | `bool is_ar_base_letter(char32_t ch)` |
| `is_ar_combining` | function | `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:23` | `bool is_ar_combining(char32_t ch)` |
| `onset_ipa` | function | `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:203` | `std::string onset_ipa(char32_t base)` |
| `strip_ar_diac_u32` | function | `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:68` | `std::u32string strip_ar_diac_u32(const std::u32string& s)` |
| `strip_spurious_tatweil_u32` | function | `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:136` | `std::u32string strip_spurious_tatweil_u32(const std::u32string& w)` |
| `u32_nfc_u32` | function | `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:53` | `std::u32string u32_nfc_u32(const std::u32string& s)` |
| `u32_to_utf8_str` | function | `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:79` | `std::string u32_to_utf8_str(const std::u32string& s)` |
| `vowel_from_marks` | function | `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:273` | `std::string vowel_from_marks(const std::u32string& marks)` |
| `MOONSHINE_TTS_LANG_SPECIFIC_ARABIC_IPA_H` | macro | `core/moonshine-tts/src/lang-specific/arabic-ipa.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_ARABIC_IPA_H` |
| `ArabicRuleG2p` | function | `core/moonshine-tts/src/lang-specific/arabic.cpp:100` | `ArabicRuleG2p::ArabicRuleG2p(std::filesystem::path onnx_model_dir,                              s...` |
| `ArabicRuleG2p` | function | `core/moonshine-tts/src/lang-specific/arabic.cpp:106` | `ArabicRuleG2p::ArabicRuleG2p(std::filesystem::path onnx_model_dir,                              s...` |
| `ArabicRuleG2p` | function | `core/moonshine-tts/src/lang-specific/arabic.cpp:115` | `ArabicRuleG2p::ArabicRuleG2p(const MoonshineG2POptions& opt,                              std::fi...` |
| `ArabicRuleG2p` | function | `core/moonshine-tts/src/lang-specific/arabic.cpp:122` | `ArabicRuleG2p::ArabicRuleG2p(const MoonshineG2POptions& opt,                              std::fi...` |
| `absolute_model_root_ar` | function | `core/moonshine-tts/src/lang-specific/arabic.cpp:19` | `std::filesystem::path absolute_model_root_ar(     const std::filesystem::path& model_root)` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/arabic.cpp:132` | `std::vector<std::string> ArabicRuleG2p::dialect_ids()` |
| `dialect_resolves_to_arabic_rules` | function | `core/moonshine-tts/src/lang-specific/arabic.cpp:137` | `bool dialect_resolves_to_arabic_rules(std::string_view dialect_id)` |
| `g2p_word` | function | `core/moonshine-tts/src/lang-specific/arabic.cpp:158` | `std::string ArabicRuleG2p::g2p_word(std::string_view word_utf8)` |
| `has_arabic_script` | function | `core/moonshine-tts/src/lang-specific/arabic.cpp:33` | `bool has_arabic_script(std::string_view s)` |
| `resolve_arabic_dict_path` | function | `core/moonshine-tts/src/lang-specific/arabic.cpp:146` | `std::filesystem::path resolve_arabic_dict_path(     const std::filesystem::path& model_root)` |
| `resolve_arabic_onnx_model_dir` | function | `core/moonshine-tts/src/lang-specific/arabic.cpp:152` | `std::filesystem::path resolve_arabic_onnx_model_dir(     const std::filesystem::path& model_root)` |
| `strip_lex_ipa_segment_dots` | function | `core/moonshine-tts/src/lang-specific/arabic.cpp:93` | `std::string strip_lex_ipa_segment_dots(std::string ipa)` |
| `text_to_ipa` | function | `core/moonshine-tts/src/lang-specific/arabic.cpp:174` | `std::string ArabicRuleG2p::text_to_ipa(std::string text,                                        s...` |
| `ArabicRuleG2p` | class | `core/moonshine-tts/src/lang-specific/arabic.h:21` | `` |
| `G2pWordLog` | struct | `core/moonshine-tts/src/lang-specific/arabic.h:16` | `` |
| `MOONSHINE_TTS_LANG_SPECIFIC_ARABIC_H` | macro | `core/moonshine-tts/src/lang-specific/arabic.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_ARABIC_H` |
| `MoonshineG2POptions` | struct | `core/moonshine-tts/src/lang-specific/arabic.h:17` | `` |
| `dialect_id` | function | `core/moonshine-tts/src/lang-specific/arabic.h:45` | `const std::string& dialect_id() const` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/arabic.h:39` | `static std::vector<std::string> dialect_ids();` |
| `dialect_resolves_to_arabic_rules` | function | `core/moonshine-tts/src/lang-specific/arabic.h:54` | `bool dialect_resolves_to_arabic_rules(std::string_view dialect_id);` |
| `arabic_numeral_token_to_han` | function | `core/moonshine-tts/src/lang-specific/chinese-numbers.cpp:170` | `std::optional<std::string> arabic_numeral_token_to_han(     std::string_view token_sv)` |
| `ascii_digit_string` | function | `core/moonshine-tts/src/lang-specific/chinese-numbers.cpp:146` | `bool ascii_digit_string(std::string_view t, std::uint64_t& out_val)` |
| `cn_digit` | function | `core/moonshine-tts/src/lang-specific/chinese-numbers.cpp:27` | `std::string cn_digit(unsigned d)` |
| `digit_cp` | function | `core/moonshine-tts/src/lang-specific/chinese-numbers.cpp:17` | `char32_t digit_cp(unsigned d)` |
| `ends_with_ling_utf8` | function | `core/moonshine-tts/src/lang-specific/chinese-numbers.cpp:33` | `bool ends_with_ling_utf8(const std::string& s)` |
| `gs` | function | `core/moonshine-tts/src/lang-specific/chinese-numbers.cpp:116` | `std::vector<unsigned> gs(low_first.rbegin(), low_first.rend());` |
| `int_to_han_u64` | function | `core/moonshine-tts/src/lang-specific/chinese-numbers.cpp:96` | `std::string int_to_han_u64(std::uint64_t n)` |
| `int_to_mandarin_cardinal_han` | function | `core/moonshine-tts/src/lang-specific/chinese-numbers.cpp:166` | `std::string int_to_mandarin_cardinal_han(std::uint64_t n)` |
| `section_under_10000` | function | `core/moonshine-tts/src/lang-specific/chinese-numbers.cpp:41` | `std::string section_under_10000(unsigned n)` |
| `MOONSHINE_TTS_LANG_SPECIFIC_CHINESE_NUMBERS_H` | macro | `core/moonshine-tts/src/lang-specific/chinese-numbers.h:2` | `#define MOONSHINE_TTS_LANG_SPECIFIC_CHINESE_NUMBERS_H` |
| `ChineseOnnxG2p` | function | `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp:30` | `ChineseOnnxG2p::ChineseOnnxG2p(std::filesystem::path model_dir,                                st...` |
| `ChineseOnnxG2p` | function | `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp:34` | `ChineseOnnxG2p::ChineseOnnxG2p(std::filesystem::path model_dir,                                st...` |
| `ChineseOnnxG2p` | function | `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp:38` | `ChineseOnnxG2p::ChineseOnnxG2p(const MoonshineG2POptions& opt,                                std...` |
| `ChineseOnnxG2p` | function | `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp:44` | `ChineseOnnxG2p::ChineseOnnxG2p(const MoonshineG2POptions& opt,                                std...` |
| `ChineseOnnxRuleG2p` | function | `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp:76` | `ChineseOnnxRuleG2p::ChineseOnnxRuleG2p(std::filesystem::path onnx_model_dir,                     ...` |
| `ChineseOnnxRuleG2p` | function | `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp:82` | `ChineseOnnxRuleG2p::ChineseOnnxRuleG2p(std::filesystem::path onnx_model_dir,                     ...` |
| `ChineseOnnxRuleG2p` | function | `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp:87` | `ChineseOnnxRuleG2p::ChineseOnnxRuleG2p(const MoonshineG2POptions& opt,                           ...` |
| `ChineseOnnxRuleG2p` | function | `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp:94` | `ChineseOnnxRuleG2p::ChineseOnnxRuleG2p(const MoonshineG2POptions& opt,                           ...` |
| `text_to_ipa` | function | `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp:50` | `std::string ChineseOnnxG2p::text_to_ipa(std::string text_utf8,                                   ...` |
| `text_to_ipa` | function | `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp:101` | `std::string ChineseOnnxRuleG2p::text_to_ipa(     std::string text, std::vector<G2pWordLog>* per_w...` |
| `tmp` | function | `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp:17` | `const std::string tmp(s);` |
| `utf8_nfc_utf8proc` | function | `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp:16` | `std::string utf8_nfc_utf8proc(std::string_view s)` |
| `ChineseOnnxG2p` | class | `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h:20` | `` |
| `ChineseOnnxRuleG2p` | class | `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h:46` | `` |
| `G2pWordLog` | struct | `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h:15` | `` |
| `MOONSHINE_TTS_CHINESE_ONNX_G2P_H` | macro | `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h:2` | `#define MOONSHINE_TTS_CHINESE_ONNX_G2P_H` |
| `MoonshineG2POptions` | struct | `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h:16` | `` |
| `tok` | function | `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h:37` | `const ChineseTokPosOnnx& tok() const` |
| `BasicTokCfg` | struct | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:311` | `` |
| `ChineseTokPosOnnx` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:714` | `ChineseTokPosOnnx::ChineseTokPosOnnx(const MoonshineG2POptions* opt,                             ...` |
| `EncodedWp` | struct | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:435` | `` |
| `Idx` | struct | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:525` | `` |
| `align_basic_tokens_u32` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:370` | `void align_basic_tokens_u32(const std::u32string& ref,                             const std::vec...` |
| `basic_tokenize_u32` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:338` | `std::vector<std::u32string> basic_tokenize_u32(     const std::u32string& original_text_u32, cons...` |
| `buf` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:627` | `const std::string buf(utf8);` |
| `bundle_load_binary` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:90` | `bool bundle_load_binary(const MoonshineG2POptions* opt,                         std::string_view ...` |
| `bundle_load_utf8` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:72` | `bool bundle_load_utf8(const MoonshineG2POptions* opt,                       std::string_view bund...` |
| `chars` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:397` | `std::vector<char32_t> chars(wt.begin(), wt.end());` |
| `cjk_tokpos_chunk_exclusive_end` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:666` | `template <typename EncodeFn> std::size_t cjk_tokpos_chunk_exclusive_end(const std::u32string& ful...` |
| `cjk_tokpos_preferred_chunk_break_cp` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:632` | `bool cjk_tokpos_preferred_chunk_break_cp(char32_t c)` |
| `clean_text_u32` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:230` | `std::u32string clean_text_u32(const std::u32string& text)` |
| `default_chinese_tok_pos_model_dir` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:704` | `std::filesystem::path default_chinese_tok_pos_model_dir(     const std::filesystem::path& g2p_dat...` |
| `encode_bert_wordpiece` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:442` | `EncodedWp encode_bert_wordpiece(     const std::u32string& text_u32,     const std::unordered_map...` |
| `format_annotated_line` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:775` | `std::string ChineseTokPosOnnx::format_annotated_line(     const std::vector<std::pair<std::string...` |
| `is_chinese_char` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:180` | `bool is_chinese_char(std::uint32_t cp)` |
| `is_control_u32` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:153` | `bool is_control_u32(char32_t c)` |
| `is_punct_char_word_group_u32` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:175` | `bool is_punct_char_word_group_u32(char32_t c)` |
| `is_punctuation_u32` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:162` | `bool is_punctuation_u32(char32_t c)` |
| `is_space_u32` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:144` | `bool is_space_u32(char32_t c)` |
| `mask` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:831` | `std::vector<int64_t> mask(static_cast<size_t>(T), 1);` |
| `normalization_ref_u32` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:317` | `std::u32string normalization_ref_u32(const std::u32string& text_u32,                             ...` |
| `open_session` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:31` | `std::unique_ptr<Ort::Session> open_session(     Ort::Env& env, const std::filesystem::path& model...` |
| `open_session_memory` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:48` | `std::unique_ptr<Ort::Session> open_session_memory(     Ort::Env& env, const void* data, size_t le...` |
| `run_split_on_punc_u32` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:281` | `std::vector<std::u32string> run_split_on_punc_u32(const std::u32string& text)` |
| `slurp_utf8_file` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:62` | `std::string slurp_utf8_file(const std::filesystem::path& p)` |
| `split_u32_whitespace` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:256` | `std::vector<std::u32string> split_u32_whitespace(std::u32string_view s)` |
| `strip_mn_nfd` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:201` | `std::u32string strip_mn_nfd(const std::u32string& s)` |
| `to_lower_u32` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:221` | `std::u32string to_lower_u32(const std::u32string& s)` |
| `tokenize_chinese_chars_u32` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:242` | `std::u32string tokenize_chinese_chars_u32(const std::u32string& text)` |
| `u32_nfc` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:189` | `std::u32string u32_nfc(const std::u32string& s)` |
| `u32_to_utf8` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:136` | `std::string u32_to_utf8(const std::u32string& s)` |
| `utf8_to_u32` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:123` | `std::u32string utf8_to_u32(std::string_view utf8)` |
| `wordpiece_tokenize_u32` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:387` | `std::vector<std::u32string> wordpiece_tokenize_u32(     const std::u32string& token,     const st...` |
| `ChineseTokPosOnnx` | class | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.h:22` | `` |
| `MOONSHINE_TTS_CHINESE_TOK_POS_ONNX_H` | macro | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.h:2` | `#define MOONSHINE_TTS_CHINESE_TOK_POS_ONNX_H` |
| `MoonshineG2POptions` | struct | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.h:16` | `` |
| `format_annotated_line` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.h:39` | `static std::string format_annotated_line( const std::vector<std::pair<std::string, std::string>>& pairs);` |
| `model_dir` | function | `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.h:42` | `const std::filesystem::path& model_dir() const` |
| `ChineseRuleG2p` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:215` | `ChineseRuleG2p::ChineseRuleG2p(std::filesystem::path dict_tsv)` |
| `ChineseRuleG2p` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:232` | `ChineseRuleG2p::ChineseRuleG2p(std::string dict_tsv_utf8)` |
| `char_fallback_ipa` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:426` | `std::string ChineseRuleG2p::char_fallback_ipa(std::string_view word) const` |
| `dialect_ids` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:556` | `std::vector<std::string> ChineseRuleG2p::dialect_ids()` |
| `dialect_resolves_to_chinese_rules` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:547` | `bool dialect_resolves_to_chinese_rules(std::string_view dialect_id)` |
| `disambiguate_heteronym` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:240` | `std::string ChineseRuleG2p::disambiguate_heteronym(     std::string_view word, std::string_view p...` |
| `g2p_word_impl` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:441` | `std::string ChineseRuleG2p::g2p_word_impl(std::string_view word,                                 ...` |
| `h` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:402` | `const std::string h(han);` |
| `han_reading_to_ipa` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:401` | `std::string ChineseRuleG2p::han_reading_to_ipa(std::string_view han) const` |
| `ipa_contains` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:92` | `bool ipa_contains(const std::string& ipa, std::string_view sub)` |
| `is_ascii_digit_cp` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:44` | `bool is_ascii_digit_cp(char32_t cp)` |
| `is_cjk_cp` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:37` | `bool is_cjk_cp(char32_t cp)` |
| `is_fullwidth_digit_cp` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:46` | `bool is_fullwidth_digit_cp(char32_t cp)` |
| `load_chinese_lexicon_stream` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:191` | `void load_chinese_lexicon_stream(     std::istream& in,     std::unordered_map<std::string, std::...` |
| `noun_like_pos` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:85` | `const std::unordered_set<std::string>& noun_like_pos()` |
| `p` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:250` | `const std::string p(pos);` |
| `pos_in_set` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:68` | `bool pos_in_set(std::string_view p, const std::unordered_set<std::string>& s)` |
| `resolve_chinese_dict_path` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:561` | `std::filesystem::path resolve_chinese_dict_path(     const std::filesystem::path& model_root)` |
| `resolve_chinese_onnx_model_dir` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:566` | `std::filesystem::path resolve_chinese_onnx_model_dir(     const std::filesystem::path& model_root)` |
| `skip_phonetic_pos` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:72` | `const std::unordered_set<std::string>& skip_phonetic_pos()` |
| `text_to_ipa` | function | `core/moonshine-tts/src/lang-specific/chinese.cpp:497` | `std::string ChineseRuleG2p::text_to_ipa(std::string text,                                        ...` |

Next: [SYMBOLS_p4.md](SYMBOLS_p4.md)
