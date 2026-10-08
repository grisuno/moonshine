# API (page 3 of 10)
Previous: [API_p2.md](API_p2.md)

## core/moonshine-cpp.h
Depends on: `core/moonshine-c-api.h`
Imported by: `core/benchmark.cpp`, `core/moonshine-cpp-test.cpp`, `examples/windows/cli-transcriber/cli-transcriber.cpp`
- `onLineStarted` (function) `core/moonshine-cpp.h:16` `* public:
 *     void onLineStarted(const moonshine::LineStarted& event) override`
- `onLineCompleted` (function) `core/moonshine-cpp.h:19` `*     void onLineCompleted(const moonshine::LineCompleted& event) override`
- `main` (function) `core/moonshine-cpp.h:24` `*
 * int main()`
- `transcriber` (function) `core/moonshine-cpp.h:25` `* moonshine::Transcriber transcriber("path/to/models", * moonshine::ModelArch::BASE);`
- `WordTiming` (function) `core/moonshine-cpp.h:93` `WordTiming() : start(0.0f), end(0.0f), confidence(0.0f)`
- `WordTiming` (function) `core/moonshine-cpp.h:94` `WordTiming(const std::string &word, float start, float end, float confidence)
      : word(word),...`
- `SpeakerSpan` (function) `core/moonshine-cpp.h:120` `SpeakerSpan()
      : startTime(0.0f),
        duration(0.0f),
        speakerId(0),
        spea...`
- `SpeakerSpan` (function) `core/moonshine-cpp.h:127` `SpeakerSpan(float startTime, float duration, uint64_t speakerId,
              uint32_t speakerIn...`
- `TranscriptLine` (function) `core/moonshine-cpp.h:186` `TranscriptLine()
      : startTime(0.0f),
        duration(0.0f),
        lineId(0),
        isCo...` -- Default constructor
- `TranscriptLine` (function) `core/moonshine-cpp.h:198` `TranscriptLine(const transcript_line_t &line_c)
      : startTime(line_c.start_time),
        dur...` -- Construct from C API structure
- `toString` (function) `core/moonshine-cpp.h:233` `std::string toString() const`
- `Transcript` (function) `core/moonshine-cpp.h:269` `Transcript()` -- Default constructor
- `Transcript` (function) `core/moonshine-cpp.h:272` `Transcript(const transcript_t *transcript_c)` -- Construct from C API structure
- `toString` (function) `core/moonshine-cpp.h:283` `std::string toString() const`
- `TranscriptEvent` (function) `core/moonshine-cpp.h:320` `protected:
  TranscriptEvent(const TranscriptLine &line, int32_t streamHandle, Type type)
      :...`
- `LineStarted` (function) `core/moonshine-cpp.h:327` `public:
  LineStarted(const TranscriptLine &line, int32_t streamHandle)
      : TranscriptEvent(l...`
- `LineUpdated` (function) `core/moonshine-cpp.h:334` `public:
  LineUpdated(const TranscriptLine &line, int32_t streamHandle)
      : TranscriptEvent(l...`
- `LineTextChanged` (function) `core/moonshine-cpp.h:341` `public:
  LineTextChanged(const TranscriptLine &line, int32_t streamHandle)
      : TranscriptEve...`
- `LineSpeakersChanged` (function) `core/moonshine-cpp.h:351` `public:
  LineSpeakersChanged(const TranscriptLine &line, int32_t streamHandle)
      : Transcrip...`
- `LineCompleted` (function) `core/moonshine-cpp.h:358` `public:
  LineCompleted(const TranscriptLine &line, int32_t streamHandle)
      : TranscriptEvent...`
- `Error` (function) `core/moonshine-cpp.h:368` `Error(const std::string &errorMessage, int32_t streamHandle)
      : TranscriptEvent(TranscriptLi...`
- `Error` (function) `core/moonshine-cpp.h:372` `Error(const std::string &errorMessage, const TranscriptLine &line,
        int32_t streamHandle)
...`
- `onLineStarted` (function) `core/moonshine-cpp.h:390` `virtual void onLineStarted(const LineStarted &)` -- Called when a new transcription line starts
- `onLineUpdated` (function) `core/moonshine-cpp.h:393` `virtual void onLineUpdated(const LineUpdated &)` -- Called when an existing transcription line is updated
- `onLineTextChanged` (function) `core/moonshine-cpp.h:396` `virtual void onLineTextChanged(const LineTextChanged &)` -- Called when the text of a transcription line changes
- `onLineSpeakersChanged` (function) `core/moonshine-cpp.h:400` `virtual void onLineSpeakersChanged(const LineSpeakersChanged &)` -- Called when the speaker spans of a transcription line change.
- `onLineCompleted` (function) `core/moonshine-cpp.h:403` `virtual void onLineCompleted(const LineCompleted &)` -- Called when a transcription line is completed
- `onError` (function) `core/moonshine-cpp.h:406` `virtual void onError(const Error &)` -- Called when an error occurs
- `MoonshineException` (function) `core/moonshine-cpp.h:414` `public:
  MoonshineException(const std::string &message)
      : std::runtime_error(message)`
- `getHandle` (function) `core/moonshine-cpp.h:489` `int32_t getHandle() const` -- Get the stream handle (for internal use)
- `getHandle` (function) `core/moonshine-cpp.h:641` `int32_t getHandle() const` -- Get the transcriber handle (for internal use)
- `Transcriber` (function) `core/moonshine-cpp.h:646` `Transcriber(int32_t handle, ModelArch modelArch, double updateInterval)
      : handle_(handle),
...` -- Internal constructor used by ``loadFromMemory`` to wrap an already-acquired C handle without re-running the...
- `TtsSynthesisResult` (function) `core/moonshine-cpp.h:673` `TtsSynthesisResult() : sampleRateHz(0)`
- `TtsSynthesisResult` (function) `core/moonshine-cpp.h:674` `TtsSynthesisResult(std::vector<float> samples, int32_t sampleRateHz)
      : samples(std::move(sa...`
- `getLanguage` (function) `core/moonshine-cpp.h:748` `const std::string &getLanguage() const` -- Get the language tag
- `getHandle` (function) `core/moonshine-cpp.h:751` `int32_t getHandle() const` -- Get the synthesizer handle (for internal use)
- `getLanguage` (function) `core/moonshine-cpp.h:834` `const std::string &getLanguage() const` -- Get the language tag
- `getHandle` (function) `core/moonshine-cpp.h:837` `int32_t getHandle() const` -- Get the phonemizer handle (for internal use)
- `IntentMatch` (function) `core/moonshine-cpp.h:863` `IntentMatch(std::string phrase, float sim)
      : canonicalPhrase(std::move(phrase)), similarity...`
- `getHandle` (function) `core/moonshine-cpp.h:920` `int32_t getHandle() const`
- `Stream` (function) `core/moonshine-cpp.h:932` `inline Stream::Stream(Transcriber *transcriber, double updateInterval,
                      uint...` -- Stream implementation
- `Stream` (function) `core/moonshine-cpp.h:945` `inline Stream::Stream(Stream &&other)
    : transcriber_(other.transcriber_),
      handle_(other...`
- `start` (function) `core/moonshine-cpp.h:971` `inline void Stream::start()`
- `stop` (function) `core/moonshine-cpp.h:975` `inline void Stream::stop()`
- `addAudio` (function) `core/moonshine-cpp.h:986` `inline void Stream::addAudio(const std::vector<float> &audioData,
                             in...`
- `updateTranscription` (function) `core/moonshine-cpp.h:1002` `inline Transcript Stream::updateTranscription(uint32_t flags)`
- `addListener` (function) `core/moonshine-cpp.h:1011` `inline void Stream::addListener(TranscriptEventListener *listener)`
- `addListener` (function) `core/moonshine-cpp.h:1017` `inline void Stream::addListener(
    std::function<void(const TranscriptEvent &)> listener)`
- `removeListener` (function) `core/moonshine-cpp.h:1022` `inline void Stream::removeListener(TranscriptEventListener *listener)`
- `removeListener` (function) `core/moonshine-cpp.h:1028` `inline void Stream::removeListener(
    std::function<void(const TranscriptEvent &)> listener)`
- `remove_if` (function) `core/moonshine-cpp.h:1034` `std::remove_if(
          functionListeners_.begin(), functionListeners_.end(),
          [&liste...`
- `removeAllListeners` (function) `core/moonshine-cpp.h:1051` `inline void Stream::removeAllListeners()`
- `close` (function) `core/moonshine-cpp.h:1056` `inline void Stream::close()`
- `notifyFromTranscript` (function) `core/moonshine-cpp.h:1064` `inline void Stream::notifyFromTranscript(const Transcript &transcript)`
- `emit` (function) `core/moonshine-cpp.h:1084` `inline void Stream::emit(const TranscriptEvent &event)`
- `emitError` (function) `core/moonshine-cpp.h:1168` `inline void Stream::emitError(const std::string &errorMessage)`
- `buildOptions` (function) `core/moonshine-cpp.h:1187` `inline OptionsBuffer buildOptions(
    const std::string &spellingModelPath,
    const std::vecto...`
- `Transcriber` (function) `core/moonshine-cpp.h:1214` `inline Transcriber::Transcriber(const std::string &modelPath,
                                Mod...`
- `Transcriber` (function) `core/moonshine-cpp.h:1226` `inline Transcriber::Transcriber(
    const std::string &modelPath, ModelArch modelArch, double up...`
- `loadFromMemory` (function) `core/moonshine-cpp.h:1242` `inline Transcriber Transcriber::loadFromMemory(
    const uint8_t *encoderData, size_t encoderDat...`
- `Transcriber` (function) `core/moonshine-cpp.h:1267` `inline Transcriber::Transcriber(Transcriber &&other)
    : handle_(other.handle_),
      modelPat...`
- `close` (function) `core/moonshine-cpp.h:1295` `inline void Transcriber::close()`
- `transcribeWithoutStreaming` (function) `core/moonshine-cpp.h:1303` `inline Transcript Transcriber::transcribeWithoutStreaming(
    const std::vector<float> &audioDat...`
- `getVersion` (function) `core/moonshine-cpp.h:1318` `inline int32_t Transcriber::getVersion() const`
- `createStream` (function) `core/moonshine-cpp.h:1322` `inline Stream Transcriber::createStream(double updateInterval, uint32_t flags)`
- `getDefaultStream` (function) `core/moonshine-cpp.h:1326` `inline Stream &Transcriber::getDefaultStream()`
- `start` (function) `core/moonshine-cpp.h:1333` `inline void Transcriber::start()`
- `stop` (function) `core/moonshine-cpp.h:1335` `inline void Transcriber::stop()`
- `addAudio` (function) `core/moonshine-cpp.h:1341` `inline void Transcriber::addAudio(const std::vector<float> &audioData,
                          ...`
- `updateTranscription` (function) `core/moonshine-cpp.h:1346` `inline Transcript Transcriber::updateTranscription(uint32_t flags)`
- `addListener` (function) `core/moonshine-cpp.h:1350` `inline void Transcriber::addListener(TranscriptEventListener *listener)`
- `addListener` (function) `core/moonshine-cpp.h:1354` `inline void Transcriber::addListener(
    std::function<void(const TranscriptEvent &)> listener)`
- `removeListener` (function) `core/moonshine-cpp.h:1359` `inline void Transcriber::removeListener(TranscriptEventListener *listener)`
- `removeListener` (function) `core/moonshine-cpp.h:1365` `inline void Transcriber::removeListener(
    std::function<void(const TranscriptEvent &)> listener)`
- `removeAllListeners` (function) `core/moonshine-cpp.h:1372` `inline void Transcriber::removeAllListeners()`
- `parseTranscript` (function) `core/moonshine-cpp.h:1378` `inline Transcript Transcriber::parseTranscript(
    const transcript_t *transcript_c)`
- `checkError` (function) `core/moonshine-cpp.h:1383` `inline void Transcriber::checkError(int32_t error) const`
- `checkError` (function) `core/moonshine-cpp.h:1391` `inline void Stream::checkError(int32_t error) const`
- `TextToSpeech` (function) `core/moonshine-cpp.h:1400` `inline TextToSpeech::TextToSpeech(
    const std::string &language, const std::vector<moonshine_o...` -- TextToSpeech implementation
- `TextToSpeech` (function) `core/moonshine-cpp.h:1411` `inline TextToSpeech::TextToSpeech(TextToSpeech &&other)
    : handle_(other.handle_), language_(s...`
- `synthesize` (function) `core/moonshine-cpp.h:1426` `inline TtsSynthesisResult TextToSpeech::synthesize(
    const std::string &text, const std::vecto...`
- `synthesizeFromPhonemes` (function) `core/moonshine-cpp.h:1446` `inline TtsSynthesisResult TextToSpeech::synthesizeFromPhonemes(
    const std::string &phonemes,
...`
- `close` (function) `core/moonshine-cpp.h:1467` `inline void TextToSpeech::close()`
- `getVoices` (function) `core/moonshine-cpp.h:1474` `inline std::string TextToSpeech::getVoices(
    const std::string &languages,
    const std::vect...`
- `getDependencies` (function) `core/moonshine-cpp.h:1494` `inline std::string TextToSpeech::getDependencies(
    const std::string &languages,
    const std...`
- `checkError` (function) `core/moonshine-cpp.h:1514` `inline void TextToSpeech::checkError(int32_t error) const`
- `GraphemeToPhonemizer` (function) `core/moonshine-cpp.h:1523` `inline GraphemeToPhonemizer::GraphemeToPhonemizer(
    const std::string &language, const std::ve...` -- GraphemeToPhonemizer implementation
- `GraphemeToPhonemizer` (function) `core/moonshine-cpp.h:1534` `inline GraphemeToPhonemizer::GraphemeToPhonemizer(GraphemeToPhonemizer &&other)
    : handle_(oth...`
- `toIpa` (function) `core/moonshine-cpp.h:1550` `inline std::string GraphemeToPhonemizer::toIpa(
    const std::string &text, const std::vector<mo...`
- `close` (function) `core/moonshine-cpp.h:1566` `inline void GraphemeToPhonemizer::close()`
- `getDependencies` (function) `core/moonshine-cpp.h:1573` `inline std::string GraphemeToPhonemizer::getDependencies(
    const std::string &languages,
    c...`
- `checkError` (function) `core/moonshine-cpp.h:1593` `inline void GraphemeToPhonemizer::checkError(int32_t error) const`
- `IntentRecognizer` (function) `core/moonshine-cpp.h:1601` `inline IntentRecognizer::IntentRecognizer(const std::string &model_path,
                        ...`
- `IntentRecognizer` (function) `core/moonshine-cpp.h:1612` `inline IntentRecognizer::IntentRecognizer(IntentRecognizer &&other) noexcept
    : handle_(other....`
- `registerIntent` (function) `core/moonshine-cpp.h:1627` `inline void IntentRecognizer::registerIntent(
    const std::string &canonical_phrase, float *emb...`
- `unregisterIntent` (function) `core/moonshine-cpp.h:1634` `inline bool IntentRecognizer::unregisterIntent(
    const std::string &canonical_phrase)`
- `getClosestIntents` (function) `core/moonshine-cpp.h:1647` `inline std::vector<IntentMatch> IntentRecognizer::getClosestIntents(
    const std::string &utter...`
- `intentCount` (function) `core/moonshine-cpp.h:1671` `inline int32_t IntentRecognizer::intentCount() const`
- `clearIntents` (function) `core/moonshine-cpp.h:1681` `inline void IntentRecognizer::clearIntents()`
- `calculateEmbedding` (function) `core/moonshine-cpp.h:1685` `inline std::vector<float> IntentRecognizer::calculateEmbedding(
    const std::string &sentence, ...`
- `close` (function) `core/moonshine-cpp.h:1699` `inline void IntentRecognizer::close()`
- `checkError` (function) `core/moonshine-cpp.h:1706` `inline void IntentRecognizer::checkError(int32_t error) const`

## core/moonshine-download-smoke.cpp
Depends on: `core/moonshine-c-api.h`, `core/moonshine-utils/debug-utils.h`
- `print_usage` (function) `core/moonshine-download-smoke.cpp:45` `void print_usage()`
- `url_encode_path` (function) `core/moonshine-download-smoke.cpp:53` `std::string url_encode_path(const std::string& key)`
- `fail` (function) `core/moonshine-download-smoke.cpp:73` `int fail(const std::string& message)`
- `print_group_manifest` (function) `core/moonshine-download-smoke.cpp:82` `void print_group_manifest(const std::string& json_text)` -- Emits "<url>\t<relative_path>" for every file in a {"groups":[...]} manifest produced by...
- `manifest_stt` (function) `core/moonshine-download-smoke.cpp:93` `int manifest_stt(const std::vector<std::string>& spec)`
- `manifest_intent` (function) `core/moonshine-download-smoke.cpp:115` `int manifest_intent(const std::vector<std::string>& spec)`
- `manifest_tts` (function) `core/moonshine-download-smoke.cpp:135` `int manifest_tts(const std::vector<std::string>& spec)`
- `manifest_g2p` (function) `core/moonshine-download-smoke.cpp:166` `int manifest_g2p(const std::vector<std::string>& spec)`
- `csv` (function) `core/moonshine-download-smoke.cpp:176` `const std::string csv(out);`
- `load_speech_or_tone` (function) `core/moonshine-download-smoke.cpp:197` `std::vector<float> load_speech_or_tone()`
- `audio` (function) `core/moonshine-download-smoke.cpp:218` `std::vector<float> audio(data, data + used);`
- `is_streaming_arch` (function) `core/moonshine-download-smoke.cpp:234` `bool is_streaming_arch(uint32_t arch)`
- `run_stt` (function) `core/moonshine-download-smoke.cpp:241` `int run_stt(const std::string& root, const std::vector<std::string>& spec)`
- `run_intent` (function) `core/moonshine-download-smoke.cpp:295` `int run_intent(const std::string& root, const std::vector<std::string>& spec)`
- `run_tts` (function) `core/moonshine-download-smoke.cpp:323` `int run_tts(const std::string& root, const std::vector<std::string>& spec)`
- `run_g2p` (function) `core/moonshine-download-smoke.cpp:361` `int run_g2p(const std::string& root, const std::vector<std::string>& spec)`
- `main` (function) `core/moonshine-download-smoke.cpp:388` `int main(int argc, char** argv)`

## core/moonshine-model-catalog.cpp
Depends on: `core/moonshine-c-api.h`, `core/moonshine-model-catalog.h`
- `to_lower` (function) `core/moonshine-model-catalog.cpp:40` `std::string to_lower(std::string s)`
- `transform` (function) `core/moonshine-model-catalog.cpp:41` `std::transform(s.begin(), s.end(), s.begin(), [](unsigned char c)`
- `is_streaming_arch` (function) `core/moonshine-model-catalog.cpp:47` `bool is_streaming_arch(int32_t model_arch)`
- `stt_catalog` (function) `core/moonshine-model-catalog.cpp:56` `const std::vector<SttLanguageEntry>& stt_catalog()` -- Port of MODEL_INFO from python/src/moonshine_voice/download.py.
- `embedding_catalog` (function) `core/moonshine-model-catalog.cpp:123` `const std::vector<EmbeddingModelEntry>& embedding_catalog()` -- Port of EMBEDDING_MODEL_INFO.
- `find_stt_language` (function) `core/moonshine-model-catalog.cpp:133` `const SttLanguageEntry* find_stt_language(const std::string& language)`
- `stt_component_files` (function) `core/moonshine-model-catalog.cpp:148` `std::vector<std::string> stt_component_files(const std::string& language_code,
                  ...`
- `find_spelling_model` (function) `core/moonshine-model-catalog.cpp:170` `const SpellingModelEntry* find_spelling_model(const std::string& language_code)`
- `find_embedding_model` (function) `core/moonshine-model-catalog.cpp:179` `const EmbeddingModelEntry* find_embedding_model(const std::string& model_name)`
- `embedding_component_files` (function) `core/moonshine-model-catalog.cpp:194` `std::vector<std::string> embedding_component_files(const std::string& variant)` -- The C++ embedding loader (gemma-embedding-model.cpp) maps each variant to a specific ONNX filename.
- `stt_model_dependencies` (function) `core/moonshine-model-catalog.cpp:214` `std::optional<ModelDependencies> stt_model_dependencies(
    const std::string& language, std::op...`
- `intent_model_dependencies` (function) `core/moonshine-model-catalog.cpp:251` `std::optional<ModelDependencies> intent_model_dependencies(
    const std::string& model_name, co...`
- `stt_supported_languages` (function) `core/moonshine-model-catalog.cpp:273` `std::vector<std::string> stt_supported_languages()`
- `intent_supported_models` (function) `core/moonshine-model-catalog.cpp:281` `std::vector<std::string> intent_supported_models()`
- `intent_supported_variants` (function) `core/moonshine-model-catalog.cpp:289` `std::vector<std::string> intent_supported_variants(
    const std::string& model_name)`

## core/moonshine-model.cpp
Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/moonshine-model.h`, `core/moonshine-utils/debug-utils.h`, `core/moonshine-utils/string-utils.h`, `core/ort-utils/moonshine-ort-allocator.h`, `core/ort-utils/moonshine-tensor-view.h`, `core/ort-utils/ort-utils.h`
- `set_model_options_from_arch` (function) `core/moonshine-model.cpp:60` `int set_model_options_from_arch(MoonshineModel *model, int32_t model_arch)`
- `MoonshineModel` (function) `core/moonshine-model.cpp:82` `MoonshineModel::MoonshineModel(
    bool log_ort_run, float max_tokens_per_second,
    const std:...`
- `load` (function) `core/moonshine-model.cpp:145` `int MoonshineModel::load(const char *encoder_model_path,
                         const char *dec...`
- `load_from_memory` (function) `core/moonshine-model.cpp:163` `int MoonshineModel::load_from_memory(const uint8_t *encoder_model_data,
                         ...`
- `load_from_assets` (function) `core/moonshine-model.cpp:186` `int MoonshineModel::load_from_assets(const char *encoder_model_path,
                            ...` -- if defined(ANDROID)
- `transcribe` (function) `core/moonshine-model.cpp:216` `int MoonshineModel::transcribe(const float *input_audio_data,
                               size...`
- `encoder_input_names` (function) `core/moonshine-model.cpp:231` `std::vector<char *> encoder_input_names(encoder_input_count);`
- `encoder_output_names` (function) `core/moonshine-model.cpp:232` `std::vector<char *> encoder_output_names(encoder_output_count);`
- `encoder_outputs` (function) `core/moonshine-model.cpp:268` `std::vector<OrtValue *> encoder_outputs(encoder_output_count);`
- `decoder_input_names` (function) `core/moonshine-model.cpp:326` `std::vector<const char *> decoder_input_names(decoder_input_count);`
- `decoder_output_names` (function) `core/moonshine-model.cpp:338` `std::vector<const char *> decoder_output_names(decoder_output_count);`
- `decoder_inputs_data` (function) `core/moonshine-model.cpp:382` `std::vector<MoonshineTensorView *> decoder_inputs_data(decoder_input_count);`
- `decoder_outputs` (function) `core/moonshine-model.cpp:442` `std::vector<OrtValue *> decoder_outputs(decoder_output_count);` -- TIMER_START(moonshine_decoder_run);
- `transcribe_wav` (function) `core/moonshine-model.cpp:565` `int MoonshineModel::transcribe_wav(const char *wav_path, char **out_text)`
- `load_alignment_model` (function) `core/moonshine-model.cpp:580` `int MoonshineModel::load_alignment_model(const char *alignment_model_path)`
- `compute_word_timestamps` (function) `core/moonshine-model.cpp:591` `int MoonshineModel::compute_word_timestamps(
    float audio_duration, std::vector<TranscriberWor...`
- `tokens_int` (function) `core/moonshine-model.cpp:601` `std::vector<int> tokens_int(last_tokens.begin(), last_tokens.end());`
- `rearranged` (function) `core/moonshine-model.cpp:613` `std::vector<float> rearranged(L * H * total_steps * E);`
- `output_names_alloc` (function) `core/moonshine-model.cpp:679` `std::vector<char *> output_names_alloc(align_output_count);`
- `output_names` (function) `core/moonshine-model.cpp:686` `std::vector<const char *> output_names(align_output_count);`
- `outputs` (function) `core/moonshine-model.cpp:692` `std::vector<OrtValue *> outputs(align_output_count, nullptr);`
- `attn_shape` (function) `core/moonshine-model.cpp:732` `std::vector<int64_t> attn_shape(attn_ndims);`
- `cross_attention_data` (function) `core/moonshine-model.cpp:744` `std::vector<float> cross_attention_data(attn_layers * per_layer);`

## core/moonshine-model.h
Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/moonshine-c-api.h`, `core/ort-utils/moonshine-ort-allocator.h`, `core/word-alignment.h`
Imported by: `core/moonshine-c-api.cpp`, `core/moonshine-model.cpp`
- `load` (function) `core/moonshine-model.h:72` `int load(const char *encoder_model_path, const char *decoder_model_path, const char *tokenizer_path, int32_t...`
- `load_alignment_model` (function) `core/moonshine-model.h:75` `int load_alignment_model(const char *alignment_model_path);`
- `load_from_memory` (function) `core/moonshine-model.h:77` `int load_from_memory(const uint8_t *encoder_model_data, size_t encoder_model_data_size, const uint8_t...`
- `load_from_assets` (function) `core/moonshine-model.h:85` `int load_from_assets(const char *encoder_model_path, const char *decoder_model_path, const char *tokenizer_path...` -- if defined(ANDROID)
- `transcribe` (function) `core/moonshine-model.h:91` `int transcribe(const float *input_audio_data, size_t input_audio_data_size, char **out_text);`
- `transcribe_wav` (function) `core/moonshine-model.h:94` `int transcribe_wav(const char *wav_path, char **out_text);`
- `compute_word_timestamps` (function) `core/moonshine-model.h:101` `int compute_word_timestamps(float audio_duration, std::vector<TranscriberWord> &words_out);` -- Compute word-level timestamps using the alignment model and saved encoder states / tokens from the last transcribe()...

## core/moonshine-streaming-model.cpp
Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/moonshine-streaming-model.h`, `core/moonshine-utils/debug-utils.h`, `core/moonshine-utils/string-utils.h`, `core/ort-utils/moonshine-ort-allocator.h`, `core/ort-utils/ort-utils.h`
- `read_file_to_string` (function) `core/moonshine-streaming-model.cpp:49` `static std::string read_file_to_string(const std::string &path)`
- `parse_config_json` (function) `core/moonshine-streaming-model.cpp:58` `static bool parse_config_json(const std::string &json,
                              MoonshineStr...` -- TODO Use constants instead of loading config JSON
- `reset` (function) `core/moonshine-streaming-model.cpp:107` `void MoonshineStreamingState::reset(const MoonshineStreamingConfig &cfg)`
- `MoonshineStreamingModel` (function) `core/moonshine-streaming-model.cpp:146` `MoonshineStreamingModel::MoonshineStreamingModel(
    bool log_ort_run, const std::vector<std::st...`
- `load_config` (function) `core/moonshine-streaming-model.cpp:200` `int MoonshineStreamingModel::load_config(const char *config_path)`
- `load_config_from_string` (function) `core/moonshine-streaming-model.cpp:209` `int MoonshineStreamingModel::load_config_from_string(const std::string &json)`
- `load` (function) `core/moonshine-streaming-model.cpp:217` `int MoonshineStreamingModel::load(const char *model_dir,
                                  const ...`
- `load_from_memory` (function) `core/moonshine-streaming-model.cpp:290` `int MoonshineStreamingModel::load_from_memory(
    const uint8_t *frontend_model_data, size_t fro...`
- `load_from_assets` (function) `core/moonshine-streaming-model.cpp:332` `int MoonshineStreamingModel::load_from_assets(const char *model_dir,
                            ...` -- if defined(ANDROID)
- `create_state` (function) `core/moonshine-streaming-model.cpp:405` `MoonshineStreamingState *MoonshineStreamingModel::create_state()`
- `tokens_to_text` (function) `core/moonshine-streaming-model.cpp:411` `std::string MoonshineStreamingModel::tokens_to_text(
    const std::vector<int64_t> &tokens)`
- `process_audio_chunk` (function) `core/moonshine-streaming-model.cpp:421` `int MoonshineStreamingModel::process_audio_chunk(MoonshineStreamingState *state,
                ...`
- `audio_vec` (function) `core/moonshine-streaming-model.cpp:442` `std::vector<float> audio_vec(audio_chunk, audio_chunk + chunk_len);` -- Prepare input tensors
- `feat_shape` (function) `core/moonshine-streaming-model.cpp:529` `std::vector<int64_t> feat_shape(num_dims);`
- `encode` (function) `core/moonshine-streaming-model.cpp:584` `int MoonshineStreamingModel::encode(MoonshineStreamingState *state,
                             ...`
- `enc_shape` (function) `core/moonshine-streaming-model.cpp:667` `std::vector<int64_t> enc_shape(num_dims);`
- `new_encoded` (function) `core/moonshine-streaming-model.cpp:686` `std::vector<float> new_encoded(new_frames * config.encoder_dim);`
- `compute_cross_kv` (function) `core/moonshine-streaming-model.cpp:759` `int MoonshineStreamingModel::compute_cross_kv(MoonshineStreamingState *state)`
- `k_shape` (function) `core/moonshine-streaming-model.cpp:803` `std::vector<int64_t> k_shape(num_dims);`
- `run_decoder_with_cross_kv` (function) `core/moonshine-streaming-model.cpp:847` `int MoonshineStreamingModel::run_decoder_with_cross_kv(
    MoonshineStreamingState *state, const...`
- `token_data` (function) `core/moonshine-streaming-model.cpp:865` `std::vector<int64_t> token_data(tokens.begin(), tokens.end());`
- `output_names_alloc` (function) `core/moonshine-streaming-model.cpp:932` `std::vector<char *> output_names_alloc(decoder_output_count);`
- `outputs` (function) `core/moonshine-streaming-model.cpp:945` `std::vector<OrtValue *> outputs(decoder_output_count, nullptr);`
- `attn_shape` (function) `core/moonshine-streaming-model.cpp:1022` `std::vector<int64_t> attn_shape(attn_ndims);`
- `decode_step` (function) `core/moonshine-streaming-model.cpp:1069` `int MoonshineStreamingModel::decode_step(MoonshineStreamingState *state,
                        ...`
- `decode_tokens` (function) `core/moonshine-streaming-model.cpp:1116` `int MoonshineStreamingModel::decode_tokens(MoonshineStreamingState *state,
                      ...`
- `token_vec` (function) `core/moonshine-streaming-model.cpp:1138` `std::vector<int64_t> token_vec(tokens_len);`
- `decode_full` (function) `core/moonshine-streaming-model.cpp:1172` `int MoonshineStreamingModel::decode_full(MoonshineStreamingState *state,
                        ...`
- `decoder_reset` (function) `core/moonshine-streaming-model.cpp:1344` `void MoonshineStreamingModel::decoder_reset(MoonshineStreamingState *state)`

## core/moonshine-streaming-model.h
Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/ort-utils/moonshine-ort-allocator.h`, `core/word-alignment.h`
Imported by: `core/moonshine-streaming-model.cpp`
- `reset` (function) `core/moonshine-streaming-model.h:69` `void reset(const MoonshineStreamingConfig &cfg);`
- `load` (function) `core/moonshine-streaming-model.h:117` `int load(const char *model_dir, const char *tokenizer_path, int32_t model_type);`
- `load_from_memory` (function) `core/moonshine-streaming-model.h:120` `int load_from_memory( const uint8_t *frontend_model_data, size_t frontend_model_data_size, const uint8_t...`
- `load_from_assets` (function) `core/moonshine-streaming-model.h:130` `int load_from_assets(const char *model_dir, const char *tokenizer_path, int32_t model_type, AAssetManager...` -- if defined(ANDROID)
- `transcribe` (function) `core/moonshine-streaming-model.h:135` `int transcribe(const float *input_audio_data, size_t input_audio_data_size, char **out_text);` -- const uint8_t *frontend_model_data, size_t frontend_model_data_size, const uint8_t *encoder_model_data, size_t...
- `process_audio_chunk` (function) `core/moonshine-streaming-model.h:139` `int process_audio_chunk(MoonshineStreamingState *state, const float *audio_chunk, size_t chunk_len, int *features_out);` -- const uint8_t *decoder_kv_model_data, size_t decoder_kv_model_data_size, const uint8_t *tokenizer_data, size_t...
- `encode` (function) `core/moonshine-streaming-model.h:143` `int encode(MoonshineStreamingState *state, bool is_final, int *new_frames_out);`
- `decode_step` (function) `core/moonshine-streaming-model.h:147` `int decode_step(MoonshineStreamingState *state, int token, float *logits_out);` -- /* Batch transcription - processes all audio at once int transcribe(const float *input_audio_data, size_t...
- `decode_full` (function) `core/moonshine-streaming-model.h:161` `int decode_full(MoonshineStreamingState *state, const int *speculative_tokens, int speculative_len, int...` -- Full decode with optional speculative tokens.
- `decoder_reset` (function) `core/moonshine-streaming-model.h:164` `void decoder_reset(MoonshineStreamingState *state);`
- `create_state` (function) `core/moonshine-streaming-model.h:167` `MoonshineStreamingState *create_state();` -- Full decode with optional speculative tokens.
- `load_config` (function) `core/moonshine-streaming-model.h:173` `private: int load_config(const char *config_path);`
- `load_config_from_string` (function) `core/moonshine-streaming-model.h:174` `int load_config_from_string(const std::string &json);`
- `run_decoder_with_cross_kv` (function) `core/moonshine-streaming-model.h:177` `int run_decoder_with_cross_kv(MoonshineStreamingState *state, const std::vector<int64_t> &tokens, std::vector<float>...` -- void decoder_reset(MoonshineStreamingState *state); /* Create a new streaming state MoonshineStreamingState...
- `compute_cross_kv` (function) `core/moonshine-streaming-model.h:182` `int compute_cross_kv(MoonshineStreamingState *state);` -- /* Decode tokens to text using the tokenizer std::string tokens_to_text(const std::vector<int64_t> &tokens)...

## core/moonshine-tts/src/file-information.cpp
Depends on: `core/moonshine-tts/src/file-information.h`
- `FileInformation` (function) `core/moonshine-tts/src/file-information.cpp:8` `FileInformation::FileInformation(const FileInformation& o)
    : path(o.path), owned_storage_(o.o...`
- `load` (function) `core/moonshine-tts/src/file-information.cpp:35` `void FileInformation::load(const uint8_t** out_memory, size_t* out_size)`
- `free` (function) `core/moonshine-tts/src/file-information.cpp:81` `void FileInformation::free()`
- `set_memory` (function) `core/moonshine-tts/src/file-information.cpp:90` `void FileInformationMap::set_memory(std::string_view key, const uint8_t* mem,
                   ...`
- `parse_file_list` (function) `core/moonshine-tts/src/file-information.cpp:99` `void FileInformationMap::parse_file_list(
    const std::vector<std::pair<std::string, std::strin...`

## core/moonshine-tts/src/file-information.h
Imported by: `core/moonshine-tts/src/file-information.cpp`, `core/moonshine-tts/src/moonshine-asset-catalog.h`, `core/moonshine-tts/src/moonshine-g2p-options.h`, `core/moonshine-tts/src/moonshine-tts-options.h`, `core/moonshine-tts/src/ort-onnx-external-data.h`, `core/moonshine-tts/src/piper-tts.h`, `core/moonshine-tts/src/zipvoice-tts.h`, `core/moonshine-tts/tests/file-information-test.cpp`
- `FileInformation` (function) `core/moonshine-tts/src/file-information.h:24` `FileInformation(std::filesystem::path p, const uint8_t* mem, size_t sz)
      : path(std::move(p)...`
- `load` (function) `core/moonshine-tts/src/file-information.h:35` `void load(const uint8_t** out_memory, size_t* out_size);` -- If ``memory`` / ``memory_size`` are set (client buffer), returns them.
- `free` (function) `core/moonshine-tts/src/file-information.h:40` `void free();` -- Drops bytes read by ``load()`` from disk.
- `set_path` (function) `core/moonshine-tts/src/file-information.h:54` `void set_path(std::string_view key, std::filesystem::path path)`
- `erase_key` (function) `core/moonshine-tts/src/file-information.h:63` `void erase_key(std::string_view key)`
- `contains` (function) `core/moonshine-tts/src/file-information.h:65` `bool contains(std::string_view key) const`
- `parse_file_list` (function) `core/moonshine-tts/src/file-information.h:71` `void parse_file_list( const std::vector<std::pair<std::string, std::string>>* key_list, const std::vector<uint8_t*>*...` -- Fills ``entries`` from ``(*key_list)[i].first`` → path ``root_path / (*key_list)[i].second``, with optional...

## core/moonshine-tts/src/g2p-path.h
Imported by: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp`, `core/moonshine-tts/src/lang-specific/arabic.cpp`, `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp`, `core/moonshine-tts/src/lang-specific/chinese.cpp`, `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp`, `core/moonshine-tts/src/lang-specific/japanese.cpp`, `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp`, `core/moonshine-tts/src/moonshine-g2p-options.cpp`, `core/moonshine-tts/src/moonshine-tts.cpp`, `core/moonshine-tts/src/piper-tts.cpp`, `core/moonshine-tts/src/rule-based-g2p-factory.cpp`, `core/moonshine-tts/src/zipvoice-tts.cpp`
- `resolve_path_under_root` (function) `core/moonshine-tts/src/g2p-path.h:13` `inline std::filesystem::path resolve_path_under_root(
    const std::filesystem::path& root, cons...` -- If ``path`` is absolute, returns it unchanged.
- `resolve_prefer_ort_model` (function) `core/moonshine-tts/src/g2p-path.h:30` `inline std::filesystem::path resolve_prefer_ort_model(
    const std::filesystem::path& dir, std:...` -- Prefer ``stem.ort`` when present, else ``stem.onnx`` (``basename`` may end with ``.ort`` or ``.onnx``).
- `b` (function) `core/moonshine-tts/src/g2p-path.h:33` `const std::string b(basename);`
- `resolve_disk_model_file_path` (function) `core/moonshine-tts/src/g2p-path.h:56` `inline void resolve_disk_model_file_path(std::filesystem::path& path)` -- For a path whose basename ends with ``.ort`` or ``.onnx``, set ``path`` to the existing sibling preferring...

## core/moonshine-tts/src/g2p-word-log.cpp
Depends on: `core/moonshine-tts/src/g2p-word-log.h`
- `g2p_word_path_tag` (function) `core/moonshine-tts/src/g2p-word-log.cpp:7` `const char* g2p_word_path_tag(G2pWordPath path)`
- `format_g2p_word_log_line` (function) `core/moonshine-tts/src/g2p-word-log.cpp:35` `std::string format_g2p_word_log_line(const G2pWordLog& e)`

## core/moonshine-tts/src/g2p-word-log.h
Imported by: `core/moonshine-tts/src/g2p-word-log.cpp`, `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp`, `core/moonshine-tts/src/lang-specific/chinese.cpp`, `core/moonshine-tts/src/lang-specific/dutch.cpp`, `core/moonshine-tts/src/lang-specific/english.cpp`, `core/moonshine-tts/src/lang-specific/french.cpp`, `core/moonshine-tts/src/lang-specific/german.cpp`, `core/moonshine-tts/src/lang-specific/hindi.cpp`, `core/moonshine-tts/src/lang-specific/italian.cpp`, `core/moonshine-tts/src/lang-specific/japanese.cpp`, `core/moonshine-tts/src/lang-specific/korean.cpp`, `core/moonshine-tts/src/lang-specific/portuguese.cpp`, `core/moonshine-tts/src/lang-specific/russian.cpp`, `core/moonshine-tts/src/lang-specific/spanish.cpp`, `core/moonshine-tts/src/lang-specific/turkish.cpp`, `core/moonshine-tts/src/lang-specific/ukrainian.cpp`, `core/moonshine-tts/src/lang-specific/vietnamese.cpp`, `core/moonshine-tts/src/moonshine-g2p.h`, `core/moonshine-tts/tools/moonshine-g2p-cli.cpp`
- `g2p_word_path_tag` (function) `core/moonshine-tts/src/g2p-word-log.h:27` `const char* g2p_word_path_tag(G2pWordPath path);`

## core/moonshine-tts/src/ipa-postprocess.cpp
Depends on: `core/moonshine-tts/src/ipa-postprocess.h`, `core/moonshine-tts/src/utf8-utils.h`
- `replace_utf8_all` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:21` `void replace_utf8_all(std::string& s, std::string_view old_utf8,
                      std::strin...`
- `trim_copy` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:30` `std::string trim_copy(std::string t)`
- `strip_length_markers_copy` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:37` `std::string strip_length_markers_copy(std::string t)`
- `apply_shared_g2p_to_piper_replacements` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:46` `void apply_shared_g2p_to_piper_replacements(std::string& s)`
- `apply_korean_post_normalize_ipa` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:54` `void apply_korean_post_normalize_ipa(std::string& s)`
- `apply_german_ipa_piper_style` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:76` `void apply_german_ipa_piper_style(std::string& s)` -- U+0361 COMBINING DOUBLE INVERTED BREVE between consonants (narrow IPA tie bar) → espeak digraph.
- `kBar` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:77` `static const std::string kBar("\xcd\xa1");`
- `kTurnedACombBreve` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:92` `static const std::string kTurnedACombBreve("\xc9\x90\xcc\xaf");` -- Non-syllabic turned-a (common for post-vocalic /ɐ/ in German narrow IPA) → alveolar tap like Piper.
- `kAlveolarTap` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:93` `static const std::string kAlveolarTap("\xc9\xbe");`
- `kUvuR` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:97` `static const std::string kUvuR("\xca\x81");` -- Uvular fricative/approximant ʁ (U+0281) → ɾ for Piper/de voice inventory overlap.
- `apply_lang_specific_replacements` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:106` `void apply_lang_specific_replacements(std::string& s,
                                      std::...`
- `key` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:141` `const std::string key(eff);`
- `py_isspace_one_utf8_char` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:151` `bool py_isspace_one_utf8_char(std::string_view ch)`
- `unicode_category_first_char_is_p_or_s` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:170` `bool unicode_category_first_char_is_p_or_s(char32_t cp)`
- `category_is_mn_or_me` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:175` `bool category_is_mn_or_me(char32_t cp)`
- `is_ipa_like_inventory_char` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:181` `bool is_ipa_like_inventory_char(char32_t cp)`
- `utf8_singleton_codepoint` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:206` `char32_t utf8_singleton_codepoint(std::string_view token)`
- `utf8_prev_codepoint_start` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:216` `size_t utf8_prev_codepoint_start(const std::string& s, size_t char_start)`
- `rewrite_russian_combining_acute_to_primary_stress` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:230` `void rewrite_russian_combining_acute_to_primary_stress(std::string& s)` -- Map combining acute (U+0301) after a nucleus onto U+02C8 ˈ (Piper-style modifier stress).
- `kAcute` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:231` `static const std::string kAcute("\xcc\x81");`
- `kPri` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:232` `static const std::string kPri("\xcb\x88");`
- `kSec` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:233` `static const std::string kSec( "\xcb\x8c");`
- `apply_russian_ipa_piper_style` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:276` `void apply_russian_ipa_piper_style(std::string& s)` -- Russian G2P uses narrow-IPA tie bars and retroflex letters; Piper / Kokoro / espeak-ng expect digraph affricates...
- `kZhd` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:336` `static const std::string kZhd("\xca\x90");`
- `kZhj` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:337` `static const std::string kZhj("\xca\x92");`
- `kIsp` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:356` `static const std::string kIsp("\xc9\xaa ");`
- `repair_ascii_c_combining_cedilla_to_ccedilla_utf8` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:368` `void repair_ascii_c_combining_cedilla_to_ccedilla_utf8(std::string& s)`
- `kPrecomposedCcedilla` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:371` `static const std::string kPrecomposedCcedilla("\xc3\xa7");`
- `normalize_russian_ipa_piper_style` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:379` `std::string normalize_russian_ipa_piper_style(std::string ipa)`
- `normalize_german_ipa_piper_style` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:384` `std::string normalize_german_ipa_piper_style(std::string ipa)`
- `is_cmn_vowel_cp` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:394` `bool is_cmn_vowel_cp(char32_t cp)` -- True for IPA vowel codepoints used in Mandarin (after mapping).
- `is_cmn_tone_marker` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:416` `bool is_cmn_tone_marker(char32_t cp)` -- True for espeak-ng Mandarin tone markers (single characters placed in syllables).
- `normalize_chinese_ipa_piper_style` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:421` `std::string normalize_chinese_ipa_piper_style(std::string ipa)`
- `kEng` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:515` `static const std::string kEng("\xc5\x8b");`
- `kStress` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:602` `static const std::string kStress("\xcb\x88");`
- `utf8_nfc_copy` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:660` `std::string utf8_nfc_copy(std::string_view s)`
- `tmp` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:661` `const std::string tmp(s);`
- `normalize_g2p_ipa_for_piper` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:672` `std::string normalize_g2p_ipa_for_piper(std::string_view ipa_utf8,
                              ...`
- `coerce_unknown_ipa_chars_to_piper_inventory` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:690` `std::string coerce_unknown_ipa_chars_to_piper_inventory(
    std::string_view ipa_utf8,
    const...`
- `ipa_to_piper_ready` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:762` `std::string ipa_to_piper_ready(
    std::string_view ipa_utf8, std::string_view piper_lang_key,
 ...`
- `normalize_g2p_ipa_for_piper_engines` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:774` `std::string normalize_g2p_ipa_for_piper_engines(std::string_view ipa_utf8)`
- `ipa_string_to_phoneme_tokens` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:780` `std::vector<std::string> ipa_string_to_phoneme_tokens(const std::string& s)`
- `levenshtein_distance` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:806` `int levenshtein_distance(const std::vector<std::string>& a,
                         const std::v...`
- `prev` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:816` `std::vector<int> prev(static_cast<size_t>(lb + 1));`
- `cur` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:817` `std::vector<int> cur(static_cast<size_t>(lb + 1));`
- `pick_closest_alternative_index` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:837` `int pick_closest_alternative_index(
    const std::vector<std::string>& predicted_phoneme_tokens,...`
- `pick_closest_cmudict_ipa` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:866` `std::string pick_closest_cmudict_ipa(
    const std::vector<std::string>& predicted_phoneme_token...`
- `match_prediction_to_cmudict_ipa` (function) `core/moonshine-tts/src/ipa-postprocess.cpp:882` `std::optional<std::string> match_prediction_to_cmudict_ipa(
    const std::string& predicted, con...`

## core/moonshine-tts/src/ipa-postprocess.h
Imported by: `core/moonshine-tts/src/ipa-postprocess.cpp`, `core/moonshine-tts/src/lang-specific/german.cpp`, `core/moonshine-tts/src/lang-specific/russian.cpp`, `core/moonshine-tts/src/piper-tts.cpp`, `core/moonshine-tts/src/zipvoice-tts.cpp`, `core/moonshine-tts/tests/ipa-postprocess-test.cpp`, `core/moonshine-tts/tools/piper-ipa-normalize-cli.cpp`
- `repair_ascii_c_combining_cedilla_to_ccedilla_utf8` (function) `core/moonshine-tts/src/ipa-postprocess.h:19` `void repair_ascii_c_combining_cedilla_to_ccedilla_utf8(std::string& ipa_utf8);` -- Replace ASCII ``c`` + U+0327 COMBINING CEDILLA with precomposed ``ç`` (espeak NFD quirk) before Piper...
- `levenshtein_distance` (function) `core/moonshine-tts/src/ipa-postprocess.h:68` `int levenshtein_distance(const std::vector<std::string>& a, const std::vector<std::string>& b);`
- `pick_closest_alternative_index` (function) `core/moonshine-tts/src/ipa-postprocess.h:71` `int pick_closest_alternative_index( const std::vector<std::string>& predicted_phoneme_tokens, const...`

## core/moonshine-tts/src/json-config.cpp
Depends on: `core/moonshine-tts/src/constants.h`, `core/moonshine-tts/src/json-config.h`
- `read_json_file` (function) `core/moonshine-tts/src/json-config.cpp:14` `nlohmann::json read_json_file(const std::filesystem::path& p)`
- `validate_header` (function) `core/moonshine-tts/src/json-config.cpp:24` `void validate_header(const nlohmann::json& cfg, const std::string& expect_kind,
                 ...`
- `stoi_to_itos` (function) `core/moonshine-tts/src/json-config.cpp:47` `std::vector<std::string> stoi_to_itos(
    const std::unordered_map<std::string, int64_t>& stoi)`
- `load_oov_tables_from_json` (function) `core/moonshine-tts/src/json-config.cpp:64` `OovOnnxTables load_oov_tables_from_json(const nlohmann::json& cfg,
                              ...`
- `load_oov_tables` (function) `core/moonshine-tts/src/json-config.cpp:88` `OovOnnxTables load_oov_tables(const std::filesystem::path& model_onnx_path)`

## core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp
Depends on: `core/moonshine-tts/src/constants.h`, `core/moonshine-tts/src/lang-specific/onnx-g2p-models.h`, `core/moonshine-tts/src/ort-session-options.h`, `core/moonshine-tts/src/utf8-utils.h`
- `open_session` (function) `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:21` `Ort::Session open_session(Ort::Env& env,
                          const std::filesystem::path& m...`
- `open_session_memory` (function) `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:38` `Ort::Session open_session_memory(Ort::Env& env, const void* data, size_t len,
                   ...`
- `encode_chars_for_model` (function) `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:46` `std::vector<int64_t> encode_chars_for_model(
    const std::string& text,
    const std::unordere...`
- `decoder_io_padded` (function) `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:58` `void decoder_io_padded(const std::vector<int64_t>& cur, int max_phoneme_len,
                    ...`
- `argmax_vocab_row` (function) `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:73` `int argmax_vocab_row(const float* logits, int64_t vocab, int time_index)`
- `OnnxOovG2p` (function) `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:90` `OnnxOovG2p::OnnxOovG2p(Ort::Env& env, const std::filesystem::path& model_onnx,
                  ...`
- `OnnxOovG2p` (function) `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:97` `OnnxOovG2p::OnnxOovG2p(Ort::Env& env, const void* model_onnx_bytes,
                       size_t...`
- `predict_phonemes` (function) `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:106` `std::vector<std::string> OnnxOovG2p::predict_phonemes(const std::string& word)`
- `enc_ids` (function) `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:115` `std::vector<int64_t> enc_ids(static_cast<size_t>(tab_.max_seq_len), tab_.pad_id);`
- `enc_mask` (function) `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:117` `std::vector<int64_t> enc_mask(static_cast<size_t>(tab_.max_seq_len), 0);`


Next: [API_p4.md](API_p4.md)
