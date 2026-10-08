# Subsystem: core (page 2 of 3)
Previous: [KB_core.md](KB_core.md)

## core/moonshine-c-api.h
- Doc: Moonshine is a library for building interactive voice applications.
- Layer: presentation
- Language: h
- Symbols:
  - `moonshine_option_t` (struct, line 137)
  - `transcript_word_t` (struct, line 194)
  - `speaker_span_t` (struct, line 212)
  - `transcript_line_t` (struct, line 231)
  - `transcript_t` (struct, line 276)
  - `moonshine_intent_match_t` (struct, line 611)
  - `main` (function, line 38) `int main(int argc, char *argv[])`
  - `moonshine_get_version` (function, line 286) `MOONSHINE_EXPORT int32_t moonshine_get_version(void);`
  - `moonshine_error_to_string` (function, line 290) `MOONSHINE_EXPORT const char *moonshine_error_to_string(int32_t error);`
  - `moonshine_transcript_to_string` (function, line 295) `MOONSHINE_EXPORT const char *moonshine_transcript_to_string( const struct transcript_t *transcript);`
  - `moonshine_load_transcriber_from_files` (function, line 357) `MOONSHINE_EXPORT int32_t moonshine_load_transcriber_from_files( const char *path, uint32_t model_arch, const struct...`
  - `moonshine_free_transcriber` (function, line 388) `MOONSHINE_EXPORT void moonshine_free_transcriber(int32_t transcriber_handle);`
  - `moonshine_transcribe_without_streaming` (function, line 425) `MOONSHINE_EXPORT int32_t moonshine_transcribe_without_streaming( int32_t transcriber_handle, float *audio_data...`
  - `moonshine_create_stream` (function, line 507) `MOONSHINE_EXPORT int32_t moonshine_create_stream(int32_t transcriber_handle, uint32_t flags);`
  - `moonshine_free_stream` (function, line 513) `MOONSHINE_EXPORT int32_t moonshine_free_stream(int32_t transcriber_handle, int32_t stream_handle);`
  - `moonshine_start_stream` (function, line 524) `MOONSHINE_EXPORT int32_t moonshine_start_stream(int32_t transcriber_handle, int32_t stream_handle);`
  - `moonshine_stop_stream` (function, line 531) `MOONSHINE_EXPORT int32_t moonshine_stop_stream(int32_t transcriber_handle, int32_t stream_handle);`
  - `moonshine_transcribe_add_audio_to_stream` (function, line 564) `MOONSHINE_EXPORT int32_t moonshine_transcribe_add_audio_to_stream( int32_t transcriber_handle, int32_t...`
  - `moonshine_transcribe_stream` (function, line 597) `MOONSHINE_EXPORT int32_t moonshine_transcribe_stream( int32_t transcriber_handle, int32_t stream_handle, uint32_t...`
  - `moonshine_free_intent_recognizer` (function, line 638) `MOONSHINE_EXPORT void moonshine_free_intent_recognizer( int32_t intent_recognizer_handle);`
  - `moonshine_register_intent` (function, line 652) `MOONSHINE_EXPORT int32_t moonshine_register_intent( int32_t intent_recognizer_handle, const char *canonical_phrase...`
  - `moonshine_unregister_intent` (function, line 659) `MOONSHINE_EXPORT int32_t moonshine_unregister_intent( int32_t intent_recognizer_handle, const char *canonical_phrase);`
  - `moonshine_free_intent_matches` (function, line 685) `MOONSHINE_EXPORT void moonshine_free_intent_matches( struct moonshine_intent_match_t *matches, uint64_t count);`
  - `moonshine_clear_intents` (function, line 698) `MOONSHINE_EXPORT int32_t moonshine_clear_intents(int32_t intent_recognizer_handle);`
  - `moonshine_calculate_intent_embedding` (function, line 708) `MOONSHINE_EXPORT int32_t moonshine_calculate_intent_embedding( int32_t intent_recognizer_handle, const char...`
  - `moonshine_free_intent_embedding` (function, line 715) `MOONSHINE_EXPORT void moonshine_free_intent_embedding(float *embedding);`
  - `moonshine_calculate_embedding_distance` (function, line 725) `MOONSHINE_EXPORT int32_t moonshine_calculate_embedding_distance( int32_t intent_recognizer_handle, const float...`
  - `moonshine_create_tts_synthesizer_from_memory` (function, line 784) `MOONSHINE_EXPORT int32_t moonshine_create_tts_synthesizer_from_memory( const char *language, const char **filenames...`
  - `moonshine_free_tts_synthesizer` (function, line 793) `MOONSHINE_EXPORT void moonshine_free_tts_synthesizer( int32_t tts_synthesizer_handle);`
  - `moonshine_get_g2p_dependencies` (function, line 813) `MOONSHINE_EXPORT int32_t moonshine_get_g2p_dependencies( const char *languages, const struct moonshine_option_t...`
  - `moonshine_get_tts_dependencies` (function, line 830) `MOONSHINE_EXPORT int32_t moonshine_get_tts_dependencies( const char *languages, const struct moonshine_option_t...`
  - `moonshine_get_tts_voices` (function, line 858) `MOONSHINE_EXPORT int32_t moonshine_get_tts_voices( const char *languages, const struct moonshine_option_t *options...`
  - `moonshine_get_stt_dependencies` (function, line 892) `MOONSHINE_EXPORT int32_t moonshine_get_stt_dependencies( const char *language, const struct moonshine_option_t...`
  - `moonshine_get_intent_dependencies` (function, line 915) `MOONSHINE_EXPORT int32_t moonshine_get_intent_dependencies( const char *model_name, const struct moonshine_option_t...`
  - `moonshine_text_to_speech` (function, line 929) `MOONSHINE_EXPORT int32_t moonshine_text_to_speech( int32_t tts_synthesizer_handle, const char *text, const struct...`
  - `moonshine_phonemes_to_speech` (function, line 953) `MOONSHINE_EXPORT int32_t moonshine_phonemes_to_speech( int32_t tts_synthesizer_handle, const char *phonemes, const...`
  - `moonshine_free_grapheme_to_phonemizer` (function, line 1013) `MOONSHINE_EXPORT void moonshine_free_grapheme_to_phonemizer( int32_t grapheme_to_phonemizer_handle);`
  - `moonshine_text_to_phonemes` (function, line 1019) `MOONSHINE_EXPORT int32_t moonshine_text_to_phonemes( int32_t grapheme_to_phonemizer_handle, const char *text, const...`
  - `effect` (variable, line 84) `extern "C" { #endif /* ------------------------------ CONSTANTS -------------------------------- */ /* What version...`
  - `MOONSHINE_C_API_H` (macro, line 2) `#define MOONSHINE_C_API_H`
  - `MOONSHINE_EXPORT` (macro, line 78) `#define MOONSHINE_EXPORT`
  - `MOONSHINE_EXPORT` (macro, line 80) `#define MOONSHINE_EXPORT`
  - `MOONSHINE_HEADER_VERSION` (macro, line 95) `#define MOONSHINE_HEADER_VERSION`
  - `MOONSHINE_MODEL_ARCH_TINY` (macro, line 98) `#define MOONSHINE_MODEL_ARCH_TINY`
  - `MOONSHINE_MODEL_ARCH_BASE` (macro, line 99) `#define MOONSHINE_MODEL_ARCH_BASE`
  - `MOONSHINE_MODEL_ARCH_TINY_STREAMING` (macro, line 100) `#define MOONSHINE_MODEL_ARCH_TINY_STREAMING`
  - `MOONSHINE_MODEL_ARCH_BASE_STREAMING` (macro, line 101) `#define MOONSHINE_MODEL_ARCH_BASE_STREAMING`
  - `MOONSHINE_MODEL_ARCH_SMALL_STREAMING` (macro, line 102) `#define MOONSHINE_MODEL_ARCH_SMALL_STREAMING`
  - `MOONSHINE_MODEL_ARCH_MEDIUM_STREAMING` (macro, line 103) `#define MOONSHINE_MODEL_ARCH_MEDIUM_STREAMING`
  - `MOONSHINE_ERROR_NONE` (macro, line 106) `#define MOONSHINE_ERROR_NONE`
  - `MOONSHINE_ERROR_UNKNOWN` (macro, line 107) `#define MOONSHINE_ERROR_UNKNOWN`
  - `MOONSHINE_ERROR_INVALID_HANDLE` (macro, line 108) `#define MOONSHINE_ERROR_INVALID_HANDLE`
  - `MOONSHINE_ERROR_INVALID_ARGUMENT` (macro, line 109) `#define MOONSHINE_ERROR_INVALID_ARGUMENT`
  - `MOONSHINE_FLAG_FORCE_UPDATE` (macro, line 112) `#define MOONSHINE_FLAG_FORCE_UPDATE`
  - `MOONSHINE_FLAG_SPELLING_MODE` (macro, line 126) `#define MOONSHINE_FLAG_SPELLING_MODE`
  - `MOONSHINE_EMBEDDING_MODEL_ARCH_GEMMA_300M` (macro, line 604) `#define MOONSHINE_EMBEDDING_MODEL_ARCH_GEMMA_300M`
  - `MOONSHINE_INTENT_MAX_MATCHES` (macro, line 608) `#define MOONSHINE_INTENT_MAX_MATCHES`
- Imported by: `android/moonshine-jni/moonshine-jni.cpp`, `core/intent-recognizer-test.cpp`, `core/moonshine-c-api-memory-test.cpp`, `core/moonshine-c-api-test.cpp`, `core/moonshine-c-api.cpp`, `core/moonshine-cpp.h`, `core/moonshine-download-smoke.cpp`, `core/moonshine-model-catalog.cpp`, `core/moonshine-model.h`, `core/tts-repeated-memory-test.cpp`, `core/word-alignment-benchmark.cpp`, `core/word-alignment-test.cpp`

## core/moonshine-cpp-test.cpp
- Doc: load_wav_data: Duplicate of load_wav_data in debug-utils.cpp to avoid depending on internal...
- Layer: testing
- Language: cpp
- Symbols:
  - `load_wav_data` (function, line 13) `bool load_wav_data(const char *path, float **out_float_data,
                   size_t *out_num_s...`
  - `file_exists` (function, line 132) `bool file_exists(const std::string &path)`
  - `onLineStarted` (function, line 147) `void onLineStarted(const moonshine::LineStarted &) override`
  - `onLineUpdated` (function, line 150) `void onLineUpdated(const moonshine::LineUpdated &) override`
  - `onLineTextChanged` (function, line 153) `void onLineTextChanged(const moonshine::LineTextChanged &) override`
  - `onLineCompleted` (function, line 156) `void onLineCompleted(const moonshine::LineCompleted &) override`
  - `TEST_CASE` (function, line 163) `TEST_CASE("moonshine-cpp-test")`
  - `SUBCASE` (function, line 164) `SUBCASE("transcribe-without-streaming")`
  - `SUBCASE` (function, line 193) `SUBCASE("transcribe-with-streaming")`
  - `SUBCASE` (function, line 288) `SUBCASE("g2p")`
  - `SUBCASE` (function, line 306) `SUBCASE("intent recognizer invalid model path throws")`
  - `SUBCASE` (function, line 312) `SUBCASE("spelling-mode-replaces-line-text-via-cpp-ctor")`
  - `SUBCASE` (function, line 347) `SUBCASE("loadFromMemory-with-spelling-buffer")`
  - `SUBCASE` (function, line 395) `SUBCASE("intent recognizer closest intents when embedding model present")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 7) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-cpp.h`

## core/moonshine-cpp.h
- Doc: Moonshine C++ API - Header-only library
- Layer: utility
- Language: h
- Symbols:
  - `WordTiming` (struct, line 83)
  - `SpeakerSpan` (struct, line 104)
  - `TranscriptLine` (struct, line 139)
  - `Transcript` (struct, line 264)
  - `TtsSynthesisResult` (struct, line 667)
  - `IntentMatch` (struct, line 858)
  - `OptionsBuffer` (struct, line 1181)
  - `ModelArch` (enum, line 66)
  - `EmbeddingModelArch` (enum, line 76)
  - `Type` (enum, line 299)
  - `ModelArch` (class, line 66)
  - `TranscriptEvent` (class, line 296)
  - `LineStarted` (class, line 325)
  - `LineUpdated` (class, line 332)
  - `LineTextChanged` (class, line 339)
  - `LineSpeakersChanged` (class, line 349)
  - `LineCompleted` (class, line 356)
  - `Error` (class, line 363)
  - `TranscriptEventListener` (class, line 385)
  - `Stream` (class, line 421)
  - `Transcriber` (class, line 514)
  - `TextToSpeech` (class, line 702)
  - `GraphemeToPhonemizer` (class, line 800)
  - `IntentRecognizer` (class, line 868)
  - `onLineStarted` (function, line 16) `* public:
 *     void onLineStarted(const moonshine::LineStarted& event) override`
  - `onLineCompleted` (function, line 19) `*     void onLineCompleted(const moonshine::LineCompleted& event) override`
  - `main` (function, line 24) `*
 * int main()`
  - `WordTiming` (function, line 93) `WordTiming() : start(0.0f), end(0.0f), confidence(0.0f)`
  - `WordTiming` (function, line 94) `WordTiming(const std::string &word, float start, float end, float confidence)
      : word(word),...`
  - `SpeakerSpan` (function, line 120) `SpeakerSpan()
      : startTime(0.0f),
        duration(0.0f),
        speakerId(0),
        spea...`
  - `SpeakerSpan` (function, line 127) `SpeakerSpan(float startTime, float duration, uint64_t speakerId,
              uint32_t speakerIn...`
  - `TranscriptLine` (function, line 186) `TranscriptLine()
      : startTime(0.0f),
        duration(0.0f),
        lineId(0),
        isCo...`
  - `TranscriptLine` (function, line 198) `TranscriptLine(const transcript_line_t &line_c)
      : startTime(line_c.start_time),
        dur...`
  - `toString` (function, line 233) `std::string toString() const`
  - `Transcript` (function, line 269) `Transcript()`
  - `Transcript` (function, line 272) `Transcript(const transcript_t *transcript_c)`
  - `toString` (function, line 283) `std::string toString() const`
  - `TranscriptEvent` (function, line 320) `protected:
  TranscriptEvent(const TranscriptLine &line, int32_t streamHandle, Type type)
      :...`
  - `LineStarted` (function, line 327) `public:
  LineStarted(const TranscriptLine &line, int32_t streamHandle)
      : TranscriptEvent(l...`
  - `LineUpdated` (function, line 334) `public:
  LineUpdated(const TranscriptLine &line, int32_t streamHandle)
      : TranscriptEvent(l...`
  - `LineTextChanged` (function, line 341) `public:
  LineTextChanged(const TranscriptLine &line, int32_t streamHandle)
      : TranscriptEve...`
  - `LineSpeakersChanged` (function, line 351) `public:
  LineSpeakersChanged(const TranscriptLine &line, int32_t streamHandle)
      : Transcrip...`
  - `LineCompleted` (function, line 358) `public:
  LineCompleted(const TranscriptLine &line, int32_t streamHandle)
      : TranscriptEvent...`
  - `Error` (function, line 368) `Error(const std::string &errorMessage, int32_t streamHandle)
      : TranscriptEvent(TranscriptLi...`
  - `Error` (function, line 372) `Error(const std::string &errorMessage, const TranscriptLine &line,
        int32_t streamHandle)
...`
  - `onLineStarted` (function, line 390) `virtual void onLineStarted(const LineStarted &)`
  - `onLineUpdated` (function, line 393) `virtual void onLineUpdated(const LineUpdated &)`
  - `onLineTextChanged` (function, line 396) `virtual void onLineTextChanged(const LineTextChanged &)`
  - `onLineSpeakersChanged` (function, line 400) `virtual void onLineSpeakersChanged(const LineSpeakersChanged &)`
  - `onLineCompleted` (function, line 403) `virtual void onLineCompleted(const LineCompleted &)`
  - `onError` (function, line 406) `virtual void onError(const Error &)`
  - `MoonshineException` (function, line 414) `public:
  MoonshineException(const std::string &message)
      : std::runtime_error(message)`
  - `getHandle` (function, line 489) `int32_t getHandle() const`
  - `getHandle` (function, line 641) `int32_t getHandle() const`
  - `Transcriber` (function, line 646) `Transcriber(int32_t handle, ModelArch modelArch, double updateInterval)
      : handle_(handle),
...`
  - `TtsSynthesisResult` (function, line 673) `TtsSynthesisResult() : sampleRateHz(0)`
  - `TtsSynthesisResult` (function, line 674) `TtsSynthesisResult(std::vector<float> samples, int32_t sampleRateHz)
      : samples(std::move(sa...`
  - `getLanguage` (function, line 748) `const std::string &getLanguage() const`
  - `getHandle` (function, line 751) `int32_t getHandle() const`
  - `getLanguage` (function, line 834) `const std::string &getLanguage() const`
  - `getHandle` (function, line 837) `int32_t getHandle() const`
  - `IntentMatch` (function, line 863) `IntentMatch(std::string phrase, float sim)
      : canonicalPhrase(std::move(phrase)), similarity...`
  - `getHandle` (function, line 920) `int32_t getHandle() const`
  - `Stream` (function, line 932) `inline Stream::Stream(Transcriber *transcriber, double updateInterval,
                      uint...`
  - `Stream` (function, line 945) `inline Stream::Stream(Stream &&other)
    : transcriber_(other.transcriber_),
      handle_(other...`
  - `start` (function, line 971) `inline void Stream::start()`
  - `stop` (function, line 975) `inline void Stream::stop()`
  - `addAudio` (function, line 986) `inline void Stream::addAudio(const std::vector<float> &audioData,
                             in...`
  - `updateTranscription` (function, line 1002) `inline Transcript Stream::updateTranscription(uint32_t flags)`
  - `addListener` (function, line 1011) `inline void Stream::addListener(TranscriptEventListener *listener)`
  - `addListener` (function, line 1017) `inline void Stream::addListener(
    std::function<void(const TranscriptEvent &)> listener)`
  - `removeListener` (function, line 1022) `inline void Stream::removeListener(TranscriptEventListener *listener)`
  - `removeListener` (function, line 1028) `inline void Stream::removeListener(
    std::function<void(const TranscriptEvent &)> listener)`
  - `remove_if` (function, line 1034) `std::remove_if(
          functionListeners_.begin(), functionListeners_.end(),
          [&liste...`
  - `removeAllListeners` (function, line 1051) `inline void Stream::removeAllListeners()`
  - `close` (function, line 1056) `inline void Stream::close()`
  - `notifyFromTranscript` (function, line 1064) `inline void Stream::notifyFromTranscript(const Transcript &transcript)`
  - `emit` (function, line 1084) `inline void Stream::emit(const TranscriptEvent &event)`
  - `emitError` (function, line 1168) `inline void Stream::emitError(const std::string &errorMessage)`
  - `buildOptions` (function, line 1187) `inline OptionsBuffer buildOptions(
    const std::string &spellingModelPath,
    const std::vecto...`
  - `Transcriber` (function, line 1214) `inline Transcriber::Transcriber(const std::string &modelPath,
                                Mod...`
  - `Transcriber` (function, line 1226) `inline Transcriber::Transcriber(
    const std::string &modelPath, ModelArch modelArch, double up...`
  - `loadFromMemory` (function, line 1242) `inline Transcriber Transcriber::loadFromMemory(
    const uint8_t *encoderData, size_t encoderDat...`
  - `Transcriber` (function, line 1267) `inline Transcriber::Transcriber(Transcriber &&other)
    : handle_(other.handle_),
      modelPat...`
  - `close` (function, line 1295) `inline void Transcriber::close()`
  - `transcribeWithoutStreaming` (function, line 1303) `inline Transcript Transcriber::transcribeWithoutStreaming(
    const std::vector<float> &audioDat...`
  - `getVersion` (function, line 1318) `inline int32_t Transcriber::getVersion() const`
  - `createStream` (function, line 1322) `inline Stream Transcriber::createStream(double updateInterval, uint32_t flags)`
  - `getDefaultStream` (function, line 1326) `inline Stream &Transcriber::getDefaultStream()`
  - `start` (function, line 1333) `inline void Transcriber::start()`
  - `stop` (function, line 1335) `inline void Transcriber::stop()`
  - `addAudio` (function, line 1341) `inline void Transcriber::addAudio(const std::vector<float> &audioData,
                          ...`
  - `updateTranscription` (function, line 1346) `inline Transcript Transcriber::updateTranscription(uint32_t flags)`
  - `addListener` (function, line 1350) `inline void Transcriber::addListener(TranscriptEventListener *listener)`
  - `addListener` (function, line 1354) `inline void Transcriber::addListener(
    std::function<void(const TranscriptEvent &)> listener)`
  - `removeListener` (function, line 1359) `inline void Transcriber::removeListener(TranscriptEventListener *listener)`
  - `removeListener` (function, line 1365) `inline void Transcriber::removeListener(
    std::function<void(const TranscriptEvent &)> listener)`
  - `removeAllListeners` (function, line 1372) `inline void Transcriber::removeAllListeners()`
  - `parseTranscript` (function, line 1378) `inline Transcript Transcriber::parseTranscript(
    const transcript_t *transcript_c)`
  - `checkError` (function, line 1383) `inline void Transcriber::checkError(int32_t error) const`
  - `checkError` (function, line 1391) `inline void Stream::checkError(int32_t error) const`
  - `TextToSpeech` (function, line 1400) `inline TextToSpeech::TextToSpeech(
    const std::string &language, const std::vector<moonshine_o...`
  - `TextToSpeech` (function, line 1411) `inline TextToSpeech::TextToSpeech(TextToSpeech &&other)
    : handle_(other.handle_), language_(s...`
  - `synthesize` (function, line 1426) `inline TtsSynthesisResult TextToSpeech::synthesize(
    const std::string &text, const std::vecto...`
  - `synthesizeFromPhonemes` (function, line 1446) `inline TtsSynthesisResult TextToSpeech::synthesizeFromPhonemes(
    const std::string &phonemes,
...`
  - `close` (function, line 1467) `inline void TextToSpeech::close()`
  - `getVoices` (function, line 1474) `inline std::string TextToSpeech::getVoices(
    const std::string &languages,
    const std::vect...`
  - `getDependencies` (function, line 1494) `inline std::string TextToSpeech::getDependencies(
    const std::string &languages,
    const std...`
  - `checkError` (function, line 1514) `inline void TextToSpeech::checkError(int32_t error) const`
  - `GraphemeToPhonemizer` (function, line 1523) `inline GraphemeToPhonemizer::GraphemeToPhonemizer(
    const std::string &language, const std::ve...`
  - `GraphemeToPhonemizer` (function, line 1534) `inline GraphemeToPhonemizer::GraphemeToPhonemizer(GraphemeToPhonemizer &&other)
    : handle_(oth...`
  - `toIpa` (function, line 1550) `inline std::string GraphemeToPhonemizer::toIpa(
    const std::string &text, const std::vector<mo...`
  - `close` (function, line 1566) `inline void GraphemeToPhonemizer::close()`
  - `getDependencies` (function, line 1573) `inline std::string GraphemeToPhonemizer::getDependencies(
    const std::string &languages,
    c...`
  - `checkError` (function, line 1593) `inline void GraphemeToPhonemizer::checkError(int32_t error) const`
  - `IntentRecognizer` (function, line 1601) `inline IntentRecognizer::IntentRecognizer(const std::string &model_path,
                        ...`
  - `IntentRecognizer` (function, line 1612) `inline IntentRecognizer::IntentRecognizer(IntentRecognizer &&other) noexcept
    : handle_(other....`
  - `registerIntent` (function, line 1627) `inline void IntentRecognizer::registerIntent(
    const std::string &canonical_phrase, float *emb...`
  - `unregisterIntent` (function, line 1634) `inline bool IntentRecognizer::unregisterIntent(
    const std::string &canonical_phrase)`
  - `getClosestIntents` (function, line 1647) `inline std::vector<IntentMatch> IntentRecognizer::getClosestIntents(
    const std::string &utter...`
  - `intentCount` (function, line 1671) `inline int32_t IntentRecognizer::intentCount() const`
  - `clearIntents` (function, line 1681) `inline void IntentRecognizer::clearIntents()`
  - `calculateEmbedding` (function, line 1685) `inline std::vector<float> IntentRecognizer::calculateEmbedding(
    const std::string &sentence, ...`
  - `close` (function, line 1699) `inline void IntentRecognizer::close()`
  - `checkError` (function, line 1706) `inline void IntentRecognizer::checkError(int32_t error) const`
  - `transcriber` (function, line 25) `* moonshine::Transcriber transcriber("path/to/models", * moonshine::ModelArch::BASE);`
  - `MOONSHINE_CPP_H` (macro, line 2) `#define MOONSHINE_CPP_H`
- Depends on: `core/moonshine-c-api.h`
- Imported by: `core/benchmark.cpp`, `core/moonshine-cpp-test.cpp`, `examples/windows/cli-transcriber/cli-transcriber.cpp`

## core/moonshine-download-smoke.cpp
- Doc: moonshine-download-smoke: a tiny CLI used by scripts/test-model-downloads.sh to verify that the...
- Layer: utility
- Language: cpp
- Symbols:
  - `print_usage` (function, line 45) `void print_usage()`
  - `url_encode_path` (function, line 53) `std::string url_encode_path(const std::string& key)`
  - `fail` (function, line 73) `int fail(const std::string& message)`
  - `print_group_manifest` (function, line 82) `void print_group_manifest(const std::string& json_text)`
  - `manifest_stt` (function, line 93) `int manifest_stt(const std::vector<std::string>& spec)`
  - `manifest_intent` (function, line 115) `int manifest_intent(const std::vector<std::string>& spec)`
  - `manifest_tts` (function, line 135) `int manifest_tts(const std::vector<std::string>& spec)`
  - `manifest_g2p` (function, line 166) `int manifest_g2p(const std::vector<std::string>& spec)`
  - `load_speech_or_tone` (function, line 197) `std::vector<float> load_speech_or_tone()`
  - `is_streaming_arch` (function, line 234) `bool is_streaming_arch(uint32_t arch)`
  - `run_stt` (function, line 241) `int run_stt(const std::string& root, const std::vector<std::string>& spec)`
  - `run_intent` (function, line 295) `int run_intent(const std::string& root, const std::vector<std::string>& spec)`
  - `run_tts` (function, line 323) `int run_tts(const std::string& root, const std::vector<std::string>& spec)`
  - `run_g2p` (function, line 361) `int run_g2p(const std::string& root, const std::vector<std::string>& spec)`
  - `main` (function, line 388) `int main(int argc, char** argv)`
  - `csv` (function, line 176) `const std::string csv(out);`
  - `audio` (function, line 218) `std::vector<float> audio(data, data + used);`
- Depends on: `core/moonshine-c-api.h`, `core/moonshine-utils/debug-utils.h`

## core/moonshine-model-catalog.cpp
- Doc: stt_catalog: Port of MODEL_INFO from python/src/moonshine_voice/download.py.
- Layer: business_logic
- Language: cpp
- Symbols:
  - `SttModelEntry` (struct, line 17)
  - `SttLanguageEntry` (struct, line 22)
  - `SpellingModelEntry` (struct, line 28)
  - `EmbeddingModelEntry` (struct, line 33)
  - `to_lower` (function, line 40) `std::string to_lower(std::string s)`
  - `transform` (function, line 41) `std::transform(s.begin(), s.end(), s.begin(), [](unsigned char c)`
  - `is_streaming_arch` (function, line 47) `bool is_streaming_arch(int32_t model_arch)`
  - `stt_catalog` (function, line 56) `const std::vector<SttLanguageEntry>& stt_catalog()`
  - `embedding_catalog` (function, line 123) `const std::vector<EmbeddingModelEntry>& embedding_catalog()`
  - `find_stt_language` (function, line 133) `const SttLanguageEntry* find_stt_language(const std::string& language)`
  - `stt_component_files` (function, line 148) `std::vector<std::string> stt_component_files(const std::string& language_code,
                  ...`
  - `find_spelling_model` (function, line 170) `const SpellingModelEntry* find_spelling_model(const std::string& language_code)`
  - `find_embedding_model` (function, line 179) `const EmbeddingModelEntry* find_embedding_model(const std::string& model_name)`
  - `embedding_component_files` (function, line 194) `std::vector<std::string> embedding_component_files(const std::string& variant)`
  - `stt_model_dependencies` (function, line 214) `std::optional<ModelDependencies> stt_model_dependencies(
    const std::string& language, std::op...`
  - `intent_model_dependencies` (function, line 251) `std::optional<ModelDependencies> intent_model_dependencies(
    const std::string& model_name, co...`
  - `stt_supported_languages` (function, line 273) `std::vector<std::string> stt_supported_languages()`
  - `intent_supported_models` (function, line 281) `std::vector<std::string> intent_supported_models()`
  - `intent_supported_variants` (function, line 289) `std::vector<std::string> intent_supported_variants(
    const std::string& model_name)`
- Depends on: `core/moonshine-c-api.h`, `core/moonshine-model-catalog.h`

## core/moonshine-model-catalog.h
- Doc: Native catalog of downloadable model assets (speech-to-text transcription, the optional...
- Layer: business_logic
- Language: h
- Symbols:
  - `ModelDependencyGroup` (struct, line 24)
  - `ModelDependencies` (struct, line 29)
  - `MOONSHINE_MODEL_CATALOG_H` (macro, line 2) `#define MOONSHINE_MODEL_CATALOG_H`
- Imported by: `core/moonshine-c-api.cpp`, `core/moonshine-model-catalog.cpp`

## core/moonshine-model.cpp
- Doc: load_from_assets: if defined(ANDROID)
- Layer: business_logic
- Language: cpp
- Symbols:
  - `set_model_options_from_arch` (function, line 60) `int set_model_options_from_arch(MoonshineModel *model, int32_t model_arch)`
  - `MoonshineModel` (function, line 82) `MoonshineModel::MoonshineModel(
    bool log_ort_run, float max_tokens_per_second,
    const std:...`
  - `load` (function, line 145) `int MoonshineModel::load(const char *encoder_model_path,
                         const char *dec...`
  - `load_from_memory` (function, line 163) `int MoonshineModel::load_from_memory(const uint8_t *encoder_model_data,
                         ...`
  - `load_from_assets` (function, line 186) `int MoonshineModel::load_from_assets(const char *encoder_model_path,
                            ...`
  - `transcribe` (function, line 216) `int MoonshineModel::transcribe(const float *input_audio_data,
                               size...`
  - `transcribe_wav` (function, line 565) `int MoonshineModel::transcribe_wav(const char *wav_path, char **out_text)`
  - `load_alignment_model` (function, line 580) `int MoonshineModel::load_alignment_model(const char *alignment_model_path)`
  - `compute_word_timestamps` (function, line 591) `int MoonshineModel::compute_word_timestamps(
    float audio_duration, std::vector<TranscriberWor...`
  - `encoder_input_names` (function, line 231) `std::vector<char *> encoder_input_names(encoder_input_count);`
  - `encoder_output_names` (function, line 232) `std::vector<char *> encoder_output_names(encoder_output_count);`
  - `encoder_outputs` (function, line 268) `std::vector<OrtValue *> encoder_outputs(encoder_output_count);`
  - `decoder_input_names` (function, line 326) `std::vector<const char *> decoder_input_names(decoder_input_count);`
  - `decoder_output_names` (function, line 338) `std::vector<const char *> decoder_output_names(decoder_output_count);`
  - `decoder_inputs_data` (function, line 382) `std::vector<MoonshineTensorView *> decoder_inputs_data(decoder_input_count);`
  - `decoder_outputs` (function, line 442) `std::vector<OrtValue *> decoder_outputs(decoder_output_count);`
  - `tokens_int` (function, line 601) `std::vector<int> tokens_int(last_tokens.begin(), last_tokens.end());`
  - `rearranged` (function, line 613) `std::vector<float> rearranged(L * H * total_steps * E);`
  - `output_names_alloc` (function, line 679) `std::vector<char *> output_names_alloc(align_output_count);`
  - `output_names` (function, line 686) `std::vector<const char *> output_names(align_output_count);`
  - `outputs` (function, line 692) `std::vector<OrtValue *> outputs(align_output_count, nullptr);`
  - `attn_shape` (function, line 732) `std::vector<int64_t> attn_shape(attn_ndims);`
  - `cross_attention_data` (function, line 744) `std::vector<float> cross_attention_data(attn_layers * per_layer);`
  - `DEBUG_ALLOC_ENABLED` (macro, line 36) `#define DEBUG_ALLOC_ENABLED`
  - `MOONSHINE_TINY_NUM_LAYERS` (macro, line 41) `#define MOONSHINE_TINY_NUM_LAYERS`
  - `MOONSHINE_TINY_NUM_KV_HEADS` (macro, line 42) `#define MOONSHINE_TINY_NUM_KV_HEADS`
  - `MOONSHINE_TINY_HEAD_DIM` (macro, line 43) `#define MOONSHINE_TINY_HEAD_DIM`
  - `MOONSHINE_TINY_PAST_ELEMENT_COUNT` (macro, line 45) `#define MOONSHINE_TINY_PAST_ELEMENT_COUNT`
  - `MOONSHINE_BASE_NUM_LAYERS` (macro, line 49) `#define MOONSHINE_BASE_NUM_LAYERS`
  - `MOONSHINE_BASE_NUM_KV_HEADS` (macro, line 50) `#define MOONSHINE_BASE_NUM_KV_HEADS`
  - `MOONSHINE_BASE_HEAD_DIM` (macro, line 51) `#define MOONSHINE_BASE_HEAD_DIM`
  - `MOONSHINE_BASE_PAST_ELEMENT_COUNT` (macro, line 53) `#define MOONSHINE_BASE_PAST_ELEMENT_COUNT`
  - `MOONSHINE_DECODER_START_TOKEN_ID` (macro, line 56) `#define MOONSHINE_DECODER_START_TOKEN_ID`
  - `MOONSHINE_EOS_TOKEN_ID` (macro, line 57) `#define MOONSHINE_EOS_TOKEN_ID`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/moonshine-model.h`, `core/moonshine-utils/debug-utils.h`, `core/moonshine-utils/string-utils.h`, `core/ort-utils/moonshine-ort-allocator.h`, `core/ort-utils/moonshine-tensor-view.h`, `core/ort-utils/ort-utils.h`

## core/moonshine-model.h
- Doc: load_from_assets: if defined(ANDROID)
- Layer: business_logic
- Language: h
- Symbols:
  - `MoonshineModel` (struct, line 17)
  - `load` (function, line 72) `int load(const char *encoder_model_path, const char *decoder_model_path, const char *tokenizer_path, int32_t...`
  - `load_alignment_model` (function, line 75) `int load_alignment_model(const char *alignment_model_path);`
  - `load_from_memory` (function, line 77) `int load_from_memory(const uint8_t *encoder_model_data, size_t encoder_model_data_size, const uint8_t...`
  - `load_from_assets` (function, line 85) `int load_from_assets(const char *encoder_model_path, const char *decoder_model_path, const char *tokenizer_path...`
  - `transcribe` (function, line 91) `int transcribe(const float *input_audio_data, size_t input_audio_data_size, char **out_text);`
  - `transcribe_wav` (function, line 94) `int transcribe_wav(const char *wav_path, char **out_text);`
  - `compute_word_timestamps` (function, line 101) `int compute_word_timestamps(float audio_duration, std::vector<TranscriberWord> &words_out);`
  - `MOONSHINE_MODEL_H` (macro, line 2) `#define MOONSHINE_MODEL_H`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/moonshine-c-api.h`, `core/ort-utils/moonshine-ort-allocator.h`, `core/word-alignment.h`
- Imported by: `core/moonshine-c-api.cpp`, `core/moonshine-model.cpp`

## core/moonshine-streaming-model.cpp
- Doc: Streaming model constants
- Layer: business_logic
- Language: cpp
- Symbols:
  - `read_file_to_string` (function, line 49) `static std::string read_file_to_string(const std::string &path)`
  - `parse_config_json` (function, line 58) `static bool parse_config_json(const std::string &json,
                              MoonshineStr...`
  - `reset` (function, line 107) `void MoonshineStreamingState::reset(const MoonshineStreamingConfig &cfg)`
  - `MoonshineStreamingModel` (function, line 146) `MoonshineStreamingModel::MoonshineStreamingModel(
    bool log_ort_run, const std::vector<std::st...`
  - `load_config` (function, line 200) `int MoonshineStreamingModel::load_config(const char *config_path)`
  - `load_config_from_string` (function, line 209) `int MoonshineStreamingModel::load_config_from_string(const std::string &json)`
  - `load` (function, line 217) `int MoonshineStreamingModel::load(const char *model_dir,
                                  const ...`
  - `load_from_memory` (function, line 290) `int MoonshineStreamingModel::load_from_memory(
    const uint8_t *frontend_model_data, size_t fro...`
  - `load_from_assets` (function, line 332) `int MoonshineStreamingModel::load_from_assets(const char *model_dir,
                            ...`
  - `create_state` (function, line 405) `MoonshineStreamingState *MoonshineStreamingModel::create_state()`
  - `tokens_to_text` (function, line 411) `std::string MoonshineStreamingModel::tokens_to_text(
    const std::vector<int64_t> &tokens)`
  - `process_audio_chunk` (function, line 421) `int MoonshineStreamingModel::process_audio_chunk(MoonshineStreamingState *state,
                ...`
  - `encode` (function, line 584) `int MoonshineStreamingModel::encode(MoonshineStreamingState *state,
                             ...`
  - `compute_cross_kv` (function, line 759) `int MoonshineStreamingModel::compute_cross_kv(MoonshineStreamingState *state)`
  - `run_decoder_with_cross_kv` (function, line 847) `int MoonshineStreamingModel::run_decoder_with_cross_kv(
    MoonshineStreamingState *state, const...`
  - `decode_step` (function, line 1069) `int MoonshineStreamingModel::decode_step(MoonshineStreamingState *state,
                        ...`
  - `decode_tokens` (function, line 1116) `int MoonshineStreamingModel::decode_tokens(MoonshineStreamingState *state,
                      ...`
  - `decode_full` (function, line 1172) `int MoonshineStreamingModel::decode_full(MoonshineStreamingState *state,
                        ...`
  - `decoder_reset` (function, line 1344) `void MoonshineStreamingModel::decoder_reset(MoonshineStreamingState *state)`
  - `audio_vec` (function, line 442) `std::vector<float> audio_vec(audio_chunk, audio_chunk + chunk_len);`
  - `feat_shape` (function, line 529) `std::vector<int64_t> feat_shape(num_dims);`
  - `enc_shape` (function, line 667) `std::vector<int64_t> enc_shape(num_dims);`
  - `new_encoded` (function, line 686) `std::vector<float> new_encoded(new_frames * config.encoder_dim);`
  - `k_shape` (function, line 803) `std::vector<int64_t> k_shape(num_dims);`
  - `token_data` (function, line 865) `std::vector<int64_t> token_data(tokens.begin(), tokens.end());`
  - `output_names_alloc` (function, line 932) `std::vector<char *> output_names_alloc(decoder_output_count);`
  - `outputs` (function, line 945) `std::vector<OrtValue *> outputs(decoder_output_count, nullptr);`
  - `attn_shape` (function, line 1022) `std::vector<int64_t> attn_shape(attn_ndims);`
  - `token_vec` (function, line 1138) `std::vector<int64_t> token_vec(tokens_len);`
  - `DEBUG_ALLOC_ENABLED` (macro, line 24) `#define DEBUG_ALLOC_ENABLED`
  - `MOONSHINE_STREAMING_TINY_ENCODER_DIM` (macro, line 29) `#define MOONSHINE_STREAMING_TINY_ENCODER_DIM`
  - `MOONSHINE_STREAMING_TINY_DECODER_DIM` (macro, line 30) `#define MOONSHINE_STREAMING_TINY_DECODER_DIM`
  - `MOONSHINE_STREAMING_TINY_DEPTH` (macro, line 31) `#define MOONSHINE_STREAMING_TINY_DEPTH`
  - `MOONSHINE_STREAMING_TINY_NHEADS` (macro, line 32) `#define MOONSHINE_STREAMING_TINY_NHEADS`
  - `MOONSHINE_STREAMING_TINY_HEAD_DIM` (macro, line 33) `#define MOONSHINE_STREAMING_TINY_HEAD_DIM`
  - `MOONSHINE_STREAMING_BASE_ENCODER_DIM` (macro, line 35) `#define MOONSHINE_STREAMING_BASE_ENCODER_DIM`
  - `MOONSHINE_STREAMING_BASE_DECODER_DIM` (macro, line 36) `#define MOONSHINE_STREAMING_BASE_DECODER_DIM`
  - `MOONSHINE_STREAMING_BASE_DEPTH` (macro, line 37) `#define MOONSHINE_STREAMING_BASE_DEPTH`
  - `MOONSHINE_STREAMING_BASE_NHEADS` (macro, line 38) `#define MOONSHINE_STREAMING_BASE_NHEADS`
  - `MOONSHINE_STREAMING_BASE_HEAD_DIM` (macro, line 39) `#define MOONSHINE_STREAMING_BASE_HEAD_DIM`
  - `MOONSHINE_DECODER_START_TOKEN_ID` (macro, line 41) `#define MOONSHINE_DECODER_START_TOKEN_ID`
  - `MOONSHINE_EOS_TOKEN_ID` (macro, line 42) `#define MOONSHINE_EOS_TOKEN_ID`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/moonshine-streaming-model.h`, `core/moonshine-utils/debug-utils.h`, `core/moonshine-utils/string-utils.h`, `core/ort-utils/moonshine-ort-allocator.h`, `core/ort-utils/ort-utils.h`


Next: [KB_core_p3.md](KB_core_p3.md)
