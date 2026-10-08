# Subsystem: misc

## android/java/test/java/ai/moonshine/voice/ExampleUnitTest.java
- Doc: ExampleUnitTest: Example local unit test, which will execute on the development machine (host)....
- Layer: testing
- Language: java
- Symbols:
  - `ExampleUnitTest` (class, line 12)
  - `addition_isCorrect` (method, line 13)

## android/moonshine-jni/moonshine-jni.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `get_class` (function, line 19) `static jclass get_class(JNIEnv *env, const char *className)`
  - `get_field` (function, line 27) `static jfieldID get_field(JNIEnv *env, jclass clazz, const char *fieldName,
                     ...`
  - `get_method` (function, line 36) `static jmethodID get_method(JNIEnv *env, jclass clazz, const char *methodName,
                  ...`
  - `c_transcript_from_jobject` (function, line 46) `static std::unique_ptr<transcript_t> c_transcript_from_jobject(
    JNIEnv *env, jobject javaTran...`
  - `c_transcript_to_jobject` (function, line 112) `static jobject c_transcript_to_jobject(JNIEnv *env, struct transcript_t *transcript)`
  - `fill_moonshine_options` (function, line 265) `static bool fill_moonshine_options(
    JNIEnv *env, jobjectArray joptions, std::vector<moonshine...`
  - `release_moonshine_options` (function, line 300) `static void release_moonshine_options(
    JNIEnv *env, const std::vector<moonshine_option_t> &co...`
  - `transcript` (function, line 77) `std::unique_ptr<transcript_t> transcript(new transcript_t());`
  - `copy` (function, line 673) `std::vector<uint8_t> copy(static_cast<size_t>(len));`
  - `MOONSHINE_ERROR_INVALID_ARGUMENT` (variable, line 514) `extern "C" JNIEXPORT int JNICALL Java_ai_moonshine_voice_JNI_moonshineAddAudioToStream( JNIEnv *env, jobject /* this...`
  - `nullptr` (variable, line 533) `extern "C" JNIEXPORT jobject JNICALL Java_ai_moonshine_voice_JNI_moonshineTranscribeStream(JNIEnv *env, jobject /*...`
  - `copts` (variable, line 557) `extern "C" JNIEXPORT jint JNICALL Java_ai_moonshine_voice_JNI_moonshineCreateTtsSynthesizerFromFiles( JNIEnv *env...`
  - `copts` (variable, line 610) `extern "C" JNIEXPORT jint JNICALL Java_ai_moonshine_voice_JNI_moonshineCreateTtsSynthesizerFromMemory( JNIEnv *env...`
  - `copts` (variable, line 712) `extern "C" JNIEXPORT jstring JNICALL Java_ai_moonshine_voice_JNI_moonshineGetG2pDependencies(JNIEnv *env, jobject /*...`
  - `copts` (variable, line 752) `extern "C" JNIEXPORT jstring JNICALL Java_ai_moonshine_voice_JNI_moonshineGetTtsDependencies(JNIEnv *env, jobject /*...`
  - `copts` (variable, line 792) `extern "C" JNIEXPORT jstring JNICALL Java_ai_moonshine_voice_JNI_moonshineGetSttDependencies(JNIEnv *env, jobject /*...`
  - `copts` (variable, line 832) `extern "C" JNIEXPORT jstring JNICALL Java_ai_moonshine_voice_JNI_moonshineGetIntentDependencies(JNIEnv *env, jobject...`
  - `copts` (variable, line 872) `extern "C" JNIEXPORT jstring JNICALL Java_ai_moonshine_voice_JNI_moonshineGetTtsVoices(JNIEnv *env, jobject /* this...`
  - `copts` (variable, line 911) `extern "C" JNIEXPORT jobject JNICALL Java_ai_moonshine_voice_JNI_moonshineTextToSpeech(JNIEnv *env, jobject /* this...`
  - `copts` (variable, line 961) `extern "C" JNIEXPORT jobject JNICALL Java_ai_moonshine_voice_JNI_moonshinePhonemesToSpeech( JNIEnv *env, jobject /*...`
  - `copts` (variable, line 1011) `extern "C" JNIEXPORT jint JNICALL Java_ai_moonshine_voice_JNI_moonshineCreateGraphemeToPhonemizerFromFiles( JNIEnv...`
  - `copts` (variable, line 1064) `extern "C" JNIEXPORT jint JNICALL Java_ai_moonshine_voice_JNI_moonshineCreateGraphemeToPhonemizerFromMemory( JNIEnv...`
  - `copts` (variable, line 1165) `extern "C" JNIEXPORT jstring JNICALL Java_ai_moonshine_voice_JNI_moonshineTextToPhonemes( JNIEnv *env, jobject /*...`
  - `MOONSHINE_ERROR_INVALID_ARGUMENT` (variable, line 1205) `extern "C" JNIEXPORT jint JNICALL Java_ai_moonshine_voice_JNI_moonshineCreateIntentRecognizer( JNIEnv *env, jobject...`
  - `MOONSHINE_ERROR_INVALID_ARGUMENT` (variable, line 1238) `extern "C" JNIEXPORT jint JNICALL Java_ai_moonshine_voice_JNI_moonshineRegisterIntent(JNIEnv *env, jobject /* this...`
  - `MOONSHINE_ERROR_INVALID_ARGUMENT` (variable, line 1268) `extern "C" JNIEXPORT jint JNICALL Java_ai_moonshine_voice_JNI_moonshineUnregisterIntent( JNIEnv *env, jobject /*...`
  - `nullptr` (variable, line 1286) `extern "C" JNIEXPORT jobjectArray JNICALL Java_ai_moonshine_voice_JNI_moonshineGetClosestIntents( JNIEnv *env...`
  - `nullptr` (variable, line 1355) `extern "C" JNIEXPORT jfloatArray JNICALL Java_ai_moonshine_voice_JNI_moonshineCalculateIntentEmbedding( JNIEnv *env...`
  - `LOG_TAG` (macro, line 13) `#define LOG_TAG`
- Depends on: `core/moonshine-c-api.h`

## examples/android/IntentRecognizer/settings.gradle.kts
- Layer: infrastructure
- Language: kts

## examples/android/TextToSpeech/settings.gradle.kts
- Layer: infrastructure
- Language: kts

## examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java
- Doc: MainActivity: Minimal microphone transcription sample.
- Layer: utility
- Language: java
- Symbols:
  - `MainActivity` (class, line 22)
  - `onCreate` (method, line 50)
  - `TranscriptEventListener` (method, line 62)
  - `onLineTextChanged` (method, line 64)
  - `onLineCompleted` (method, line 75)
  - `onDestroy` (method, line 133)
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`

## examples/android/Transcriber/settings.gradle.kts
- Layer: infrastructure
- Language: kts

## examples/c++/download-library.sh
- Layer: utility
- Language: sh

## examples/ios/IntentRecognizer/scripts/copy-moonshine-models.sh
- Layer: business_logic
- Language: sh

## examples/ios/Transcriber/TranscriberTests/TranscriberTests.swift
- Doc: TranscriberTests.swift TranscriberTests  Created by Pete Warden on 1/1/26.
- Layer: testing
- Language: swift
- Symbols:
  - `TranscriberTests` (struct, line 10)

## examples/macos/BasicTranscription/Package.swift
- Doc: swift-tools-version: 6.1
- Layer: utility
- Language: swift

## examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift
- Doc: Arguments: MARK: - Command Line Argument Parsing
- Layer: utility
- Language: swift
- Symbols:
  - `TestListener` (class, line 31)
  - `Arguments` (struct, line 76)
  - `transcribeWithoutStreaming` (function, line 5)
  - `transcribeWithStreaming` (function, line 26)
  - `onLineStarted` (function, line 33)
  - `onLineTextChanged` (function, line 39)
  - `onLineCompleted` (function, line 46)
  - `parseArguments` (function, line 82)
  - `main` (function, line 146)

## examples/macos/MicTranscription/Package.swift
- Doc: swift-tools-version: 6.1
- Layer: utility
- Language: swift

## examples/macos/MicTranscription/Sources/MicTranscription/main.swift
- Doc: main: MARK: - Main
- Layer: utility
- Language: swift
- Symbols:
  - `TestListener` (class, line 40)
  - `main` (function, line 5)
  - `onLineStarted` (function, line 42)
  - `onLineTextChanged` (function, line 48)
  - `onLineCompleted` (function, line 55)

## examples/macos/TextToSpeech/Package.swift
- Doc: swift-tools-version: 6.1
- Layer: utility
- Language: swift

## examples/macos/TextToSpeech/Sources/TextToSpeech/main.swift
- Doc: Arguments: MARK: - Command Line Argument Parsing
- Layer: utility
- Language: swift
- Symbols:
  - `Arguments` (struct, line 54)
  - `writeWav` (function, line 6)
  - `printUsage` (function, line 66)
  - `parseArguments` (function, line 86)
  - `resolveAssetRoot` (function, line 163)
  - `resolveDevice` (function, line 205)
  - `main` (function, line 246)

## examples/python/ollama-voice/ollama_voice.py
- Doc: Example of using the Moonshine Voice library to transcribe speech and send it to an Ollama LLM...
- Layer: utility
- Language: py
- Symbols:
  - `Spinner` (class, line 14) `class Spinner`
  - `OllamaVoice` (class, line 25) `class OllamaVoice(TranscriptEventListener)`
  - `__init__` (method, line 17) `def __init__(self)`
  - `spin` (method, line 20) `def spin(self)`
  - `__init__` (method, line 34) `def __init__(self, ollama_model, system_prompt)`
  - `on_line_text_changed` (method, line 59) `def on_line_text_changed(self, event)`
  - `on_line_completed` (method, line 69) `def on_line_completed(self, event)`

## examples/raspberry-pi/my-dalek/my-dalek.py
- Doc: TranscriptPrinter: Listener that prints transcript updates to the terminal.
- Layer: utility
- Language: py
- Symbols:
  - `on_intent_triggered_on` (function, line 38) `def on_intent_triggered_on(trigger, utterance, similarity)`
  - `TranscriptPrinter` (class, line 44) `class TranscriptPrinter(TranscriptEventListener)`
  - `on_move_forward` (method, line 92) `def on_move_forward(trigger, utterance, similarity)`
  - `on_move_backward` (method, line 94) `def on_move_backward(trigger, utterance, similarity)`
  - `on_turn_left` (method, line 96) `def on_turn_left(trigger, utterance, similarity)`
  - `on_turn_right` (method, line 98) `def on_turn_right(trigger, utterance, similarity)`
  - `on_exterminate` (method, line 100) `def on_exterminate(trigger, utterance, similarity)`
  - `__init__` (method, line 47) `def __init__(self)`
  - `update_last_terminal_line` (method, line 50) `def update_last_terminal_line(self, new_text)`
  - `on_line_started` (method, line 57) `def on_line_started(self, event)`
  - `on_line_text_changed` (method, line 60) `def on_line_text_changed(self, event)`
  - `on_line_completed` (method, line 63) `def on_line_completed(self, event)`

## examples/windows/cli-transcriber/cli-transcriber.cpp
- Doc: Helper class to manage COM initialization
- Layer: utility
- Language: cpp
- Symbols:
  - `COMInitializer` (class, line 24)
  - `MicrophoneCapture` (class, line 71)
  - `WavFileProducer` (class, line 324)
  - `COMInitializer` (function, line 26) `public:
  COMInitializer()`
  - `onLineStarted` (function, line 38) `public:
  void onLineStarted(const moonshine::LineStarted &event) override`
  - `onLineTextChanged` (function, line 44) `void onLineTextChanged(const moonshine::LineTextChanged &event) override`
  - `onLineCompleted` (function, line 52) `void onLineCompleted(const moonshine::LineCompleted &event) override`
  - `onError` (function, line 60) `void onError(const moonshine::Error &event) override`
  - `MicrophoneCapture` (function, line 73) `public:
  MicrophoneCapture() : is_capturing_(false), sample_rate_(16000)`
  - `Initialize` (function, line 95) `bool Initialize()`
  - `Start` (function, line 192) `void Start()`
  - `Stop` (function, line 208) `void Stop()`
  - `SetAudioCallback` (function, line 223) `void SetAudioCallback(
      std::function<void(const std::vector<float> &, int32_t)> callback)`
  - `CaptureLoop` (function, line 229) `private:
  void CaptureLoop()`
  - `WavFileProducer` (function, line 326) `public:
  explicit WavFileProducer(std::string wav_path,
                           float chunk_d...`
  - `getNextAudio` (function, line 336) `bool getNextAudio(std::vector<float> &out_audio_data)`
  - `sampleRate` (function, line 348) `int32_t sampleRate() const`
  - `loadWavData` (function, line 351) `private:
  void loadWavData(const std::string &wav_path)`
  - `runWavTranscription` (function, line 456) `int runWavTranscription(const std::string &model_path,
                        moonshine::ModelAr...`
  - `main` (function, line 489) `int main(int argc, char *argv[])`
  - `pcm_data` (function, line 428) `std::vector<int16_t> pcm_data(num_samples);`
  - `WIN32_LEAN_AND_MEAN` (macro, line 14) `#define WIN32_LEAN_AND_MEAN`
  - `NOMINMAX` (macro, line 15) `#define NOMINMAX`
- Depends on: `core/moonshine-cpp.h`

## micro/examples/rp2350/lwipopts.h
- Doc: Minimal lwIP configuration for the voice WiFi-setup app (moonshine_micro_echo_wifi).
- Layer: utility
- Language: h
- Symbols:
  - `SPELLING_LWIPOPTS_H_` (macro, line 17) `#define SPELLING_LWIPOPTS_H_`
  - `NO_SYS` (macro, line 20) `#define NO_SYS`
  - `LWIP_SOCKET` (macro, line 21) `#define LWIP_SOCKET`
  - `LWIP_NETCONN` (macro, line 22) `#define LWIP_NETCONN`
  - `SYS_LIGHTWEIGHT_PROT` (macro, line 23) `#define SYS_LIGHTWEIGHT_PROT`
  - `MEM_LIBC_MALLOC` (macro, line 26) `#define MEM_LIBC_MALLOC`
  - `MEM_ALIGNMENT` (macro, line 27) `#define MEM_ALIGNMENT`
  - `MEM_SIZE` (macro, line 28) `#define MEM_SIZE`
  - `MEMP_NUM_PBUF` (macro, line 29) `#define MEMP_NUM_PBUF`
  - `MEMP_NUM_UDP_PCB` (macro, line 30) `#define MEMP_NUM_UDP_PCB`
  - `MEMP_NUM_ARP_QUEUE` (macro, line 31) `#define MEMP_NUM_ARP_QUEUE`
  - `MEMP_NUM_SYS_TIMEOUT` (macro, line 32) `#define MEMP_NUM_SYS_TIMEOUT`
  - `PBUF_POOL_SIZE` (macro, line 33) `#define PBUF_POOL_SIZE`
  - `PBUF_POOL_BUFSIZE` (macro, line 34) `#define PBUF_POOL_BUFSIZE`
  - `LWIP_IPV4` (macro, line 37) `#define LWIP_IPV4`
  - `LWIP_IPV6` (macro, line 38) `#define LWIP_IPV6`
  - `LWIP_ARP` (macro, line 39) `#define LWIP_ARP`
  - `LWIP_ETHERNET` (macro, line 40) `#define LWIP_ETHERNET`
  - `LWIP_ICMP` (macro, line 41) `#define LWIP_ICMP`
  - `LWIP_RAW` (macro, line 42) `#define LWIP_RAW`
  - `LWIP_UDP` (macro, line 43) `#define LWIP_UDP`
  - `LWIP_TCP` (macro, line 44) `#define LWIP_TCP`
  - `LWIP_DNS` (macro, line 45) `#define LWIP_DNS`
  - `LWIP_DHCP` (macro, line 46) `#define LWIP_DHCP`
  - `DHCP_DOES_ARP_CHECK` (macro, line 47) `#define DHCP_DOES_ARP_CHECK`
  - `LWIP_DHCP_DOES_ACD_CHECK` (macro, line 48) `#define LWIP_DHCP_DOES_ACD_CHECK`
  - `LWIP_NETIF_STATUS_CALLBACK` (macro, line 51) `#define LWIP_NETIF_STATUS_CALLBACK`
  - `LWIP_NETIF_LINK_CALLBACK` (macro, line 52) `#define LWIP_NETIF_LINK_CALLBACK`
  - `LWIP_NETIF_HOSTNAME` (macro, line 53) `#define LWIP_NETIF_HOSTNAME`
  - `LWIP_NETIF_TX_SINGLE_PBUF` (macro, line 54) `#define LWIP_NETIF_TX_SINGLE_PBUF`
  - `LWIP_CHKSUM_ALGORITHM` (macro, line 57) `#define LWIP_CHKSUM_ALGORITHM`
  - `LWIP_STATS` (macro, line 60) `#define LWIP_STATS`
  - `MEM_STATS` (macro, line 61) `#define MEM_STATS`
  - `SYS_STATS` (macro, line 62) `#define SYS_STATS`
  - `MEMP_STATS` (macro, line 63) `#define MEMP_STATS`
  - `LINK_STATS` (macro, line 64) `#define LINK_STATS`
  - `ETHARP_STATS` (macro, line 65) `#define ETHARP_STATS`
  - `IP_STATS` (macro, line 66) `#define IP_STATS`
  - `UDP_STATS` (macro, line 67) `#define UDP_STATS`
  - `ICMP_STATS` (macro, line 68) `#define ICMP_STATS`
  - `LWIP_DEBUG` (macro, line 71) `#define LWIP_DEBUG`
  - `LWIP_STATS_DISPLAY` (macro, line 73) `#define LWIP_STATS_DISPLAY`

## micro/feature-generation/include/feature_generation/feature_generation.h
- Doc: feature-generation -- portable, heap-free log-mel spectrogram front-end.
- Layer: utility
- Language: h
- Symbols:
  - `kiss_fftr_state` (struct, line 38)
  - `LogMelParams` (struct, line 64)
  - `LogMelSpectrogram` (class, line 98)
  - `MelStreamer` (class, line 164)
  - `n_mels` (function, line 120) `int n_mels() const`
  - `target_frames` (function, line 121) `int target_frames() const`
  - `n_freq` (function, line 122) `int n_freq() const`
  - `params` (function, line 123) `const LogMelParams& params() const`
  - `filled` (function, line 186) `int filled() const`
  - `n_mels` (function, line 187) `int n_mels() const`
  - `window_frames` (function, line 188) `int window_frames() const`
  - `HannWindowPeriodic` (function, line 48) `std::vector<float> HannWindowPeriodic(int length);`
  - `HzToMelSlaney` (function, line 52) `float HzToMelSlaney(float hz);`
  - `MelToHzSlaney` (function, line 53) `float MelToHzSlaney(float mel);`
  - `MakeMelFilterbank` (function, line 57) `std::vector<float> MakeMelFilterbank(int n_freq, int n_mels, int sample_rate, float f_min, float f_max);`
  - `Compute` (function, line 117) `void Compute(const float* waveform, std::size_t n_samples, float* out) const;`
  - `ComputeImpl` (function, line 128) `template <typename SampleT> void ComputeImpl(const SampleT* waveform, std::size_t n_samples, float* out) const;`
  - `Reset` (function, line 174) `void Reset();`
  - `PushHop` (function, line 178) `void PushHop(const float* hop_samples);`
  - `BuildModelInput` (function, line 184) `void BuildModelInput(float* out) const;`
  - `FEATURE_GENERATION_FEATURE_GENERATION_H_` (macro, line 30) `#define FEATURE_GENERATION_FEATURE_GENERATION_H_`
- Imported by: `micro/examples/rp2350/src/audio_service.cc`, `micro/examples/rp2350/src/test_app.cc`, `micro/feature-generation/src/log_mel.cc`, `micro/feature-generation/src/mel_streamer.cc`, `micro/feature-generation/tests/feature_generation_test.cc`

## micro/feature-generation/scripts/generate_mel_tables.py
- Doc: Emit C++ flash tables (periodic Hann window + CSR Slaney mel filterbank) for the...
- Layer: utility
- Language: py
- Symbols:
  - `_include_guard` (function, line 28) `def _include_guard(stem)`
  - `hann_window_periodic` (function, line 32) `def hann_window_periodic(length)`
  - `hz_to_mel_slaney` (function, line 40) `def hz_to_mel_slaney(hz)`
  - `mel_to_hz_slaney` (function, line 50) `def mel_to_hz_slaney(mel)`
  - `make_csr_filterbank` (function, line 60) `def make_csr_filterbank(n_freq, n_mels, sample_rate, f_min, f_max)`
  - `fmt_floats` (function, line 89) `def fmt_floats(values, per_line)`
  - `fmt_ints` (function, line 97) `def fmt_ints(values, per_line)`
  - `main` (function, line 105) `def main()`

## micro/feature-generation/tests/feature_generation_test.cc
- Doc: Unit tests for the feature-generation module, using TFLM's micro_test.h.
- Layer: testing
- Language: cc
- Symbols:
  - `DenseToCsr` (function, line 24) `void DenseToCsr(const std::vector<float>& dense, int n_mels, int n_freq,
                std::vec...`
  - `TF_LITE_MICRO_TEST` (function, line 46) `TF_LITE_MICRO_TESTS_BEGIN

TF_LITE_MICRO_TEST(HannWindowPeriodicEndpoints)`
  - `TF_LITE_MICRO_TEST` (function, line 54) `TF_LITE_MICRO_TEST(MelScaleRoundTrip)`
  - `TF_LITE_MICRO_TEST` (function, line 61) `TF_LITE_MICRO_TEST(StreamerMatchesBatch)`
  - `buf` (function, line 70) `std::vector<float> buf(n_samples);`
  - `out_ref` (function, line 93) `std::vector<float> out_ref(static_cast<std::size_t>(n_mels) * window_frames);`
  - `out_stream` (function, line 111) `std::vector<float> out_stream(static_cast<std::size_t>(n_mels) * window_frames);`
- Depends on: `micro/feature-generation/include/feature_generation/feature_generation.h`

## micro/klatt-tts/tests/tts_test.cc
- Doc: Unit tests for the TTS synth core, using TFLM's micro_test.h.
- Layer: testing
- Language: cc
- Symbols:
  - `Contains` (function, line 17) `bool Contains(const std::vector<std::string>& toks, const char* needle)`
  - `TF_LITE_MICRO_TEST` (function, line 28) `TF_LITE_MICRO_TESTS_BEGIN

TF_LITE_MICRO_TEST(G2PProducesPhones)`
  - `TF_LITE_MICRO_TEST` (function, line 35) `TF_LITE_MICRO_TEST(G2PNumberNormalization)`
  - `TF_LITE_MICRO_TEST` (function, line 41) `TF_LITE_MICRO_TEST(StreamSynthProducesAudioInRange)`
- Depends on: `micro/g2p/include/g2p/g2p.h`, `micro/klatt-tts/include/tts/tts.h`

## micro/stt/include/stt/stt.h
- Doc: stt -- on-device speech-to-text (isolated-letter/digit) classifier.
- Layer: utility
- Language: h
- Symbols:
  - `TensorQuant` (struct, line 35)
  - `Impl` (struct, line 74)
  - `Classifier` (class, line 40)
  - `feature_scratch` (function, line 65) `float* feature_scratch() const`
  - `input_quant` (function, line 67) `TensorQuant input_quant() const`
  - `output_quant` (function, line 68) `TensorQuant output_quant() const`
  - `n_classes` (function, line 69) `int n_classes() const`
  - `input_count` (function, line 70) `std::size_t input_count() const`
  - `arena_used_bytes` (function, line 71) `std::size_t arena_used_bytes() const`
  - `Run` (function, line 60) `void Run(const float* features, float* logits_out) const;`
  - `Argmax` (function, line 90) `int Argmax(const float* logits, int n_logits);`
  - `SoftmaxProb` (function, line 93) `float SoftmaxProb(const float* logits, int n_logits, int index);`
  - `STT_STT_H_` (macro, line 19) `#define STT_STT_H_`
- Imported by: `micro/examples/rp2350/src/audio_service.cc`, `micro/examples/rp2350/src/test_app.cc`, `micro/stt/src/classifier.cc`, `micro/stt/src/predictor.cc`, `micro/stt/tests/predictor_test.cc`

## micro/stt/tests/predictor_test.cc
- Doc: Unit tests for the STT prediction helpers, using TFLM's micro_test.h.
- Layer: testing
- Language: cc
- Symbols:
  - `TF_LITE_MICRO_TEST` (function, line 14) `TF_LITE_MICRO_TESTS_BEGIN

TF_LITE_MICRO_TEST(ArgmaxPicksLargest)`
  - `TF_LITE_MICRO_TEST` (function, line 19) `TF_LITE_MICRO_TEST(ArgmaxTiesGoToLowestIndex)`
  - `TF_LITE_MICRO_TEST` (function, line 24) `TF_LITE_MICRO_TEST(SoftmaxProbsSumToOne)`
  - `TF_LITE_MICRO_TEST` (function, line 31) `TF_LITE_MICRO_TEST(SoftmaxProbMatchesHandComputed)`
  - `TF_LITE_MICRO_TEST` (function, line 37) `TF_LITE_MICRO_TEST(SoftmaxStableOnLargeLogits)`
- Depends on: `micro/stt/include/stt/stt.h`

## micro/test-support/host/tflm_host_stub.cc
- Doc: Host (desktop) implementations of the handful of TFLM platform hooks that the modules and the...
- Layer: testing
- Language: cc
- Symbols:
  - `MicroPrintf` (function, line 19) `void MicroPrintf(const char* format, ...)`
  - `VMicroPrintf` (function, line 27) `void VMicroPrintf(const char* format, va_list args)`
  - `MicroSnprintf` (function, line 32) `int MicroSnprintf(char* buffer, size_t buf_size, const char* format, ...)`
  - `MicroVsnprintf` (function, line 40) `int MicroVsnprintf(char* buffer, size_t buf_size, const char* format,
                   va_list ...`
  - `InitializeTarget` (function, line 46) `void InitializeTarget()`

## micro/test-support/run_micro_test.sh
- Doc: Run a TFLM micro_test.h binary and translate its output into an exit code.  micro_test.h wraps...
- Layer: testing
- Language: sh

## micro/vad/include/vad/vad.h
- Doc: vad -- on-device voice activity detection.
- Layer: utility
- Language: h
- Symbols:
  - `VadTensorQuant` (struct, line 38)
  - `Impl` (struct, line 72)
  - `VadEvent` (enum, line 85)
  - `Vad` (class, line 43)
  - `VadEvent` (class, line 85)
  - `VadSegmenter` (class, line 96)
  - `feature_scratch` (function, line 64) `float* feature_scratch() const`
  - `input_quant` (function, line 66) `VadTensorQuant input_quant() const`
  - `output_quant` (function, line 67) `VadTensorQuant output_quant() const`
  - `input_count` (function, line 68) `std::size_t input_count() const`
  - `arena_used_bytes` (function, line 69) `std::size_t arena_used_bytes() const`
  - `segment_start_sample` (function, line 113) `std::size_t segment_start_sample() const`
  - `segment_end_sample` (function, line 114) `std::size_t segment_end_sample() const`
  - `samples_processed` (function, line 115) `std::size_t samples_processed() const`
  - `Predict` (function, line 60) `float Predict(const float* features) const;`
  - `Start` (function, line 103) `void Start();`
  - `ExtractClipFrontAligned` (function, line 135) `void ExtractClipFrontAligned(const float* src, std::size_t src_len, std::size_t start, std::size_t end, float* out...`
  - `EnergyCentroidIndex` (function, line 145) `std::size_t EnergyCentroidIndex(const int16_t* buf, std::size_t start, std::size_t end);`
  - `VAD_VAD_H_` (macro, line 23) `#define VAD_VAD_H_`
- Imported by: `micro/examples/rp2350/src/audio_service.cc`, `micro/examples/rp2350/src/test_app.cc`, `micro/vad/src/vad.cc`, `micro/vad/src/vad_segmenter.cc`, `micro/vad/tests/vad_segmenter_test.cc`

## micro/vad/scripts/generate_vad_embedded_data.py
- Doc: Generate the compiled-in VAD data blobs for the moonshine-micro Pico build.
- Layer: data_access
- Language: py
- Symbols:
  - `_smooth_window_frames` (function, line 66) `def _smooth_window_frames()`
  - `_write_vad_config` (function, line 72) `def _write_vad_config(out_dir)`
  - `_write_vad_mel_tables` (function, line 117) `def _write_vad_mel_tables(out_dir)`
  - `_write_vad_model` (function, line 190) `def _write_vad_model(out_dir, tflite)`
  - `_auto_tflite` (function, line 224) `def _auto_tflite()`
  - `main` (function, line 229) `def main(argv)`
- Depends on: `micro/stt/scripts/generate_embedded_data.py`

## micro/vad/tests/vad_segmenter_test.cc
- Doc: Unit tests for the VAD segmenter, using TFLM's micro_test.h.
- Layer: testing
- Language: cc
- Symbols:
  - `Repeat` (function, line 20) `std::vector<float> Repeat(float v, int n)`
  - `Concat` (function, line 22) `std::vector<float> Concat(std::initializer_list<std::vector<float>> parts)`
  - `TF_LITE_MICRO_TEST` (function, line 50) `TF_LITE_MICRO_TESTS_BEGIN

TF_LITE_MICRO_TEST(SingleSegmentDetected)`
  - `TF_LITE_MICRO_TEST` (function, line 60) `TF_LITE_MICRO_TEST(TwoSegmentsDetected)`
  - `TF_LITE_MICRO_TEST` (function, line 68) `TF_LITE_MICRO_TEST(TrailingSegmentFlushed)`
  - `TF_LITE_MICRO_TEST` (function, line 75) `TF_LITE_MICRO_TEST(NoLookBehindStartsLater)`
  - `TF_LITE_MICRO_TEST` (function, line 86) `TF_LITE_MICRO_TEST(ExtractClipFrontAlignedZeroPads)`
  - `TF_LITE_MICRO_TEST` (function, line 96) `TF_LITE_MICRO_TEST(EnergyCentroidIndexWeightsByPower)`
- Depends on: `micro/vad/include/vad/vad.h`

## python/setup.py
- Doc: Setup script for moonshine-voice package.
- Layer: infrastructure
- Language: py
- Symbols:
  - `BinaryDistribution` (class, line 9) `class BinaryDistribution(Distribution)`
  - `PlatformWheel` (class, line 14) `class PlatformWheel(bdist_wheel)`
  - `read_readme` (method, line 26) `def read_readme()`
  - `read_license` (method, line 32) `def read_license()`
  - `read_requirements` (method, line 39) `def read_requirements()`
  - `has_ext_modules` (method, line 10) `def has_ext_modules(self)`
  - `finalize_options` (method, line 15) `def finalize_options(self)`
  - `get_tag` (method, line 20) `def get_tag(self)`

## swift/Package.swift
- Doc: swift-tools-version: 6.1
- Layer: utility
- Language: swift
