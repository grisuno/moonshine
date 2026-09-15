# Subsystem: misc

## android/java/test/java/ai/moonshine/voice/ExampleUnitTest.java
- Layer: testing
- Language: java
- Symbols:
  - `ExampleUnitTest` (class, line 12)
  - `addition_isCorrect` (method, line 13)

## android/moonshine-jni/moonshine-jni.cpp
- Layer: utility
- Doc: include <jni.h>  include <cstdint> include <cstdlib> include <algorithm> include <memory> include <mutex> include <strin
- Language: cpp
- Symbols:
  - `get_class` (function, line 18) `static jclass get_class(JNIEnv *env, const char *className)`
  - `get_field` (function, line 26) `static jfieldID get_field(JNIEnv *env, jclass clazz, const char *fieldName,
                     ...`
  - `get_method` (function, line 35) `static jmethodID get_method(JNIEnv *env, jclass clazz, const char *methodName,
                  ...`
  - `c_transcript_from_jobject` (function, line 45) `static std::unique_ptr<transcript_t> c_transcript_from_jobject(
    JNIEnv *env, jobject javaTran...`
  - `c_transcript_to_jobject` (function, line 111) `static jobject c_transcript_to_jobject(JNIEnv *env, struct transcript_t *transcript)`
  - `fill_moonshine_options` (function, line 264) `static bool fill_moonshine_options(
    JNIEnv *env, jobjectArray joptions, std::vector<moonshine...`
  - `release_moonshine_options` (function, line 299) `static void release_moonshine_options(
    JNIEnv *env, const std::vector<moonshine_option_t> &co...`
  - `runtime_error` (function, line 22) `throw std::runtime_error(std::string("Failed to find class: ") + className);`
  - `transcript` (function, line 77) `std::unique_ptr<transcript_t> transcript(new transcript_t());`
  - `raw_text` (function, line 143) `std::string raw_text(line->text);`
  - `wtext` (function, line 228) `std::string wtext(w->text ? w->text : "");`
  - `moonshine_get_version` (function, line 324) `return moonshine_get_version();`
  - `moonshine_load_transcriber_from_files` (function, line 375) `return moonshine_load_transcriber_from_files( path_str, model_arch, coptions.data(), coptions.size(), MOONSHINE_HEADER_VERSION);`
  - `ALOGE` (function, line 379) `ALOGE("moonshineLoadTranscriberFromFiles: %s\n", e.what());`
  - `moonshine_load_transcriber_from_memory` (function, line 421) `return moonshine_load_transcriber_from_memory( encoder_model_data_ptr, encoder_model_data_size, decoder_model_data_ptr, decoder_model_data_size, tokenizer_data_ptr, tokenizer_data_size, spelling_model`
  - `moonshine_free_transcriber` (function, line 437) `moonshine_free_transcriber(transcriber_handle);`
  - `moonshine_create_stream` (function, line 469) `return moonshine_create_stream(transcriber_handle, 0);`
  - `moonshine_free_stream` (function, line 482) `moonshine_free_stream(transcriber_handle, stream_handle);`
  - `moonshine_start_stream` (function, line 494) `return moonshine_start_stream(transcriber_handle, stream_handle);`
  - `moonshine_stop_stream` (function, line 507) `return moonshine_stop_stream(transcriber_handle, stream_handle);`
  - `moonshine_transcribe_add_audio_to_stream` (function, line 524) `return moonshine_transcribe_add_audio_to_stream( transcriber_handle, stream_handle, audio_data_ptr, audio_data_size, sample_rate, flags);`
  - `ALOGD` (function, line 541) `ALOGD("moonshineTranscribeStream: start transcribe stream");`
  - `copy` (function, line 673) `std::vector<uint8_t> copy(static_cast<size_t>(len));`
  - `lock` (function, line 689) `std::lock_guard<std::mutex> lock(g_tts_memory_backing_mutex);`
  - `moonshine_free_tts_synthesizer` (function, line 704) `moonshine_free_tts_synthesizer(tts_handle);`
  - `free` (function, line 736) `std::free(out);`
  - `moonshine_free_grapheme_to_phonemizer` (function, line 1157) `moonshine_free_grapheme_to_phonemizer(g2p_handle);`
  - `ipa` (function, line 1195) `std::string ipa(out_ph);`
  - `moonshine_free_intent_recognizer` (function, line 1235) `moonshine_free_intent_recognizer(intent_handle);`
  - `moonshine_free_intent_matches` (function, line 1302) `moonshine_free_intent_matches(matches, count);`
  - `moonshine_get_intent_count` (function, line 1340) `return moonshine_get_intent_count(intent_handle);`
  - `moonshine_clear_intents` (function, line 1348) `return moonshine_clear_intents(intent_handle);`
  - `moonshine_free_intent_embedding` (function, line 1369) `moonshine_free_intent_embedding(out_embedding);`
  - `MOONSHINE_ERROR_INVALID_ARGUMENT` (variable, line 513) `extern "C" JNIEXPORT int JNICALL Java_ai_moonshine_voice_JNI_moonshineAddAudioToStream( JNIEnv *env, jobject /* this */, jint transcriber_handle, jint stream_handle, jfloatArray audio_data, jint sampl`
  - `nullptr` (variable, line 532) `extern "C" JNIEXPORT jobject JNICALL Java_ai_moonshine_voice_JNI_moonshineTranscribeStream(JNIEnv *env, jobject /* this */, jint transcriber_handle, jint stream_handle, jint flags) { try { struct tran`
  - `copts` (variable, line 556) `extern "C" JNIEXPORT jint JNICALL Java_ai_moonshine_voice_JNI_moonshineCreateTtsSynthesizerFromFiles( JNIEnv *env, jobject /* this */, jstring language, jobjectArray jfilenames, jobjectArray joptions)`
  - `copts` (variable, line 609) `extern "C" JNIEXPORT jint JNICALL Java_ai_moonshine_voice_JNI_moonshineCreateTtsSynthesizerFromMemory( JNIEnv *env, jobject /* this */, jstring language, jobjectArray jfilenames, jobjectArray jmemory,`
  - `copts` (variable, line 711) `extern "C" JNIEXPORT jstring JNICALL Java_ai_moonshine_voice_JNI_moonshineGetG2pDependencies(JNIEnv *env, jobject /* this */, jstring languages, jobjectArray joptions) { try { std::vector<moonshine_op`
  - `copts` (variable, line 751) `extern "C" JNIEXPORT jstring JNICALL Java_ai_moonshine_voice_JNI_moonshineGetTtsDependencies(JNIEnv *env, jobject /* this */, jstring languages, jobjectArray joptions) { try { std::vector<moonshine_op`
  - `copts` (variable, line 791) `extern "C" JNIEXPORT jstring JNICALL Java_ai_moonshine_voice_JNI_moonshineGetSttDependencies(JNIEnv *env, jobject /* this */, jstring language, jobjectArray joptions) { try { std::vector<moonshine_opt`
  - `copts` (variable, line 831) `extern "C" JNIEXPORT jstring JNICALL Java_ai_moonshine_voice_JNI_moonshineGetIntentDependencies(JNIEnv *env, jobject /* this */, jstring model_name, jobjectArray joptions) { try { std::vector<moonshin`
  - `copts` (variable, line 871) `extern "C" JNIEXPORT jstring JNICALL Java_ai_moonshine_voice_JNI_moonshineGetTtsVoices(JNIEnv *env, jobject /* this */, jstring languages, jobjectArray joptions) { try { std::vector<moonshine_option_t`
  - `copts` (variable, line 910) `extern "C" JNIEXPORT jobject JNICALL Java_ai_moonshine_voice_JNI_moonshineTextToSpeech(JNIEnv *env, jobject /* this */, jint tts_handle, jstring text, jobjectArray joptions) { try { std::vector<moonsh`
  - `copts` (variable, line 960) `extern "C" JNIEXPORT jobject JNICALL Java_ai_moonshine_voice_JNI_moonshinePhonemesToSpeech( JNIEnv *env, jobject /* this */, jint tts_handle, jstring phonemes, jobjectArray joptions) { try { std::vect`
  - `copts` (variable, line 1010) `extern "C" JNIEXPORT jint JNICALL Java_ai_moonshine_voice_JNI_moonshineCreateGraphemeToPhonemizerFromFiles( JNIEnv *env, jobject /* this */, jstring language, jobjectArray jfilenames, jobjectArray jop`
  - `copts` (variable, line 1063) `extern "C" JNIEXPORT jint JNICALL Java_ai_moonshine_voice_JNI_moonshineCreateGraphemeToPhonemizerFromMemory( JNIEnv *env, jobject /* this */, jstring language, jobjectArray jfilenames, jobjectArray jm`
  - `copts` (variable, line 1164) `extern "C" JNIEXPORT jstring JNICALL Java_ai_moonshine_voice_JNI_moonshineTextToPhonemes( JNIEnv *env, jobject /* this */, jint g2p_handle, jstring text, jobjectArray joptions) { try { std::vector<moo`
  - `MOONSHINE_ERROR_INVALID_ARGUMENT` (variable, line 1204) `extern "C" JNIEXPORT jint JNICALL Java_ai_moonshine_voice_JNI_moonshineCreateIntentRecognizer( JNIEnv *env, jobject /* this */, jstring model_path, jint embedding_arch, jstring model_variant) { try { `
  - `MOONSHINE_ERROR_INVALID_ARGUMENT` (variable, line 1237) `extern "C" JNIEXPORT jint JNICALL Java_ai_moonshine_voice_JNI_moonshineRegisterIntent(JNIEnv *env, jobject /* this */, jint intent_handle, jstring canonical_phrase, jfloatArray embedding, jint priorit`
  - `MOONSHINE_ERROR_INVALID_ARGUMENT` (variable, line 1267) `extern "C" JNIEXPORT jint JNICALL Java_ai_moonshine_voice_JNI_moonshineUnregisterIntent( JNIEnv *env, jobject /* this */, jint intent_handle, jstring canonical_phrase) { try { if (canonical_phrase == `
  - `nullptr` (variable, line 1285) `extern "C" JNIEXPORT jobjectArray JNICALL Java_ai_moonshine_voice_JNI_moonshineGetClosestIntents( JNIEnv *env, jobject /* this */, jint intent_handle, jstring utterance, jfloat tolerance) { try { if (`
  - `nullptr` (variable, line 1354) `extern "C" JNIEXPORT jfloatArray JNICALL Java_ai_moonshine_voice_JNI_moonshineCalculateIntentEmbedding( JNIEnv *env, jobject /* this */, jint intent_handle, jstring sentence) { try { if (sentence == n`
  - `LOG_TAG` (macro, line 12) `#define LOG_TAG`
- Depends on: `core/moonshine-c-api.h`

## examples/android/IntentRecognizer/settings.gradle.kts
- Layer: infrastructure
- Language: kts

## examples/android/TextToSpeech/settings.gradle.kts
- Layer: infrastructure
- Language: kts

## examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java
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
- Layer: testing
- Doc: TranscriberTests.swift TranscriberTests  Created by Pete Warden on 1/1/26.
- Language: swift
- Symbols:
  - `TranscriberTests` (struct, line 10)

## examples/macos/BasicTranscription/Package.swift
- Layer: utility
- Doc: swift-tools-version: 6.1
- Language: swift

## examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift
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
- Layer: utility
- Doc: swift-tools-version: 6.1
- Language: swift

## examples/macos/MicTranscription/Sources/MicTranscription/main.swift
- Layer: utility
- Language: swift
- Symbols:
  - `TestListener` (class, line 40)
  - `main` (function, line 5)
  - `onLineStarted` (function, line 42)
  - `onLineTextChanged` (function, line 48)
  - `onLineCompleted` (function, line 55)

## examples/macos/TextToSpeech/Package.swift
- Layer: utility
- Doc: swift-tools-version: 6.1
- Language: swift

## examples/macos/TextToSpeech/Sources/TextToSpeech/main.swift
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
- Layer: data_access
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
- Layer: utility
- Doc: include <atomic> include <algorithm> include <cstdio> include <cstring> include <iostream> include <memory> include <mut
- Language: cpp
- Symbols:
  - `COMInitializer` (class, line 24)
  - `MicrophoneCapture` (class, line 71)
  - `WavFileProducer` (class, line 324)
  - `COMInitializer` (function, line 25) `public:
  COMInitializer()`
  - `onLineStarted` (function, line 37) `public:
  void onLineStarted(const moonshine::LineStarted &event) override`
  - `onLineTextChanged` (function, line 43) `void onLineTextChanged(const moonshine::LineTextChanged &event) override`
  - `onLineCompleted` (function, line 51) `void onLineCompleted(const moonshine::LineCompleted &event) override`
  - `onError` (function, line 59) `void onError(const moonshine::Error &event) override`
  - `MicrophoneCapture` (function, line 72) `public:
  MicrophoneCapture() : is_capturing_(false), sample_rate_(16000)`
  - `Initialize` (function, line 94) `bool Initialize()`
  - `Start` (function, line 191) `void Start()`
  - `Stop` (function, line 207) `void Stop()`
  - `SetAudioCallback` (function, line 222) `void SetAudioCallback(
      std::function<void(const std::vector<float> &, int32_t)> callback)`
  - `CaptureLoop` (function, line 227) `private:
  void CaptureLoop()`
  - `WavFileProducer` (function, line 325) `public:
  explicit WavFileProducer(std::string wav_path,
                           float chunk_d...`
  - `getNextAudio` (function, line 335) `bool getNextAudio(std::vector<float> &out_audio_data)`
  - `sampleRate` (function, line 347) `int32_t sampleRate() const`
  - `loadWavData` (function, line 349) `private:
  void loadWavData(const std::string &wav_path)`
  - `runWavTranscription` (function, line 455) `int runWavTranscription(const std::string &model_path,
                        moonshine::ModelAr...`
  - `main` (function, line 488) `int main(int argc, char *argv[])`
  - `runtime_error` (function, line 29) `throw std::runtime_error("Failed to initialize COM");`
  - `lock` (function, line 39) `std::lock_guard<std::mutex> lock(output_mutex_);`
  - `__uuidof` (function, line 100) `__uuidof(IMMDeviceEnumerator), (void **)&device_enumerator_);`
  - `CoTaskMemFree` (function, line 155) `CoTaskMemFree(pwfx);`
  - `Sleep` (function, line 237) `Sleep( (DWORD)((1000.0 * buffer_frame_count_) / (2 * actual_sample_rate_)));`
  - `audio_callback_` (function, line 302) `audio_callback_(audio_data, sample_rate_);`
  - `min` (function, line 341) `std::min(current_index_ + chunk_size_, audio_data_.size());`
  - `fclose` (function, line 363) `std::fclose(file);`
  - `fseek` (function, line 366) `std::fseek(file, 4, SEEK_CUR);`
  - `fread` (function, line 397) `std::fread(&audio_format, sizeof(uint16_t), 1, file);`
  - `pcm_data` (function, line 428) `std::vector<int16_t> pcm_data(num_samples);`
  - `audio_producer` (function, line 459) `WavFileProducer audio_producer(wav_path);`
  - `transcriber` (function, line 460) `moonshine::Transcriber transcriber(model_path, model_arch, 0.5f);`
  - `sleep_for` (function, line 572) `std::this_thread::sleep_for(std::chrono::milliseconds(100));`
  - `WIN32_LEAN_AND_MEAN` (macro, line 13) `#define WIN32_LEAN_AND_MEAN`
  - `NOMINMAX` (macro, line 15) `#define NOMINMAX`
- Depends on: `core/moonshine-cpp.h`

## micro/examples/rp2350/lwipopts.h
- Layer: utility
- Doc: Minimal lwIP configuration for the voice WiFi-setup app (moonshine_micro_echo_wifi).  This firmware only needs to ASSOCI
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
- Layer: utility
- Doc: feature-generation -- portable, heap-free log-mel spectrogram front-end.  This is the single public header for the modul
- Language: h
- Symbols:
  - `kiss_fftr_state` (struct, line 38)
  - `LogMelParams` (struct, line 64)
  - `LogMelSpectrogram` (class, line 98)
  - `MelStreamer` (class, line 164)
  - `n_mels` (function, line 119) `int n_mels() const`
  - `target_frames` (function, line 121) `int target_frames() const`
  - `n_freq` (function, line 122) `int n_freq() const`
  - `params` (function, line 123) `const LogMelParams& params() const`
  - `filled` (function, line 185) `int filled() const`
  - `n_mels` (function, line 187) `int n_mels() const`
  - `window_frames` (function, line 188) `int window_frames() const`
  - `HannWindowPeriodic` (function, line 48) `std::vector<float> HannWindowPeriodic(int length);`
  - `HzToMelSlaney` (function, line 52) `float HzToMelSlaney(float hz);`
  - `MelToHzSlaney` (function, line 53) `float MelToHzSlaney(float mel);`
  - `MakeMelFilterbank` (function, line 57) `std::vector<float> MakeMelFilterbank(int n_freq, int n_mels, int sample_rate, float f_min, float f_max);`
  - `LogMelSpectrogram` (function, line 99) `public: explicit LogMelSpectrogram(const LogMelParams& params);`
  - `Compute` (function, line 117) `void Compute(const float* waveform, std::size_t n_samples, float* out) const;`
  - `ComputeImpl` (function, line 127) `template <typename SampleT> void ComputeImpl(const SampleT* waveform, std::size_t n_samples, float* out) const;`
  - `MelStreamer` (function, line 169) `MelStreamer(int n_mels, int window_frames, int n_fft, const float* window, const int* nz_off, const int* nz_idx, const float* nz_val, kiss_fftr_state* fft, float eps = 1e-6f);`
  - `Reset` (function, line 174) `void Reset();`
  - `PushHop` (function, line 178) `void PushHop(const float* hop_samples);`
  - `BuildModelInput` (function, line 184) `void BuildModelInput(float* out) const;`
  - `FEATURE_GENERATION_FEATURE_GENERATION_H_` (macro, line 30) `#define FEATURE_GENERATION_FEATURE_GENERATION_H_`
- Imported by: `micro/examples/rp2350/src/audio_service.cc`, `micro/examples/rp2350/src/test_app.cc`, `micro/feature-generation/src/log_mel.cc`, `micro/feature-generation/src/mel_streamer.cc`, `micro/feature-generation/tests/feature_generation_test.cc`

## micro/feature-generation/scripts/generate_mel_tables.py
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
- Layer: testing
- Doc: Unit tests for the feature-generation module, using TFLM's micro_test.h.  Covers the shared building blocks (periodic Ha
- Language: cc
- Symbols:
  - `DenseToCsr` (function, line 24) `void DenseToCsr(const std::vector<float>& dense, int n_mels, int n_freq,
                std::vec...`
  - `TF_LITE_MICRO_TEST` (function, line 43) `TF_LITE_MICRO_TESTS_BEGIN

TF_LITE_MICRO_TEST(HannWindowPeriodicEndpoints)`
  - `TF_LITE_MICRO_TEST` (function, line 53) `TF_LITE_MICRO_TEST(MelScaleRoundTrip)`
  - `TF_LITE_MICRO_TEST` (function, line 60) `TF_LITE_MICRO_TEST(StreamerMatchesBatch)`
  - `TF_LITE_MICRO_EXPECT_EQ` (function, line 48) `TF_LITE_MICRO_EXPECT_EQ(static_cast<int>(w.size()), 512);`
  - `TF_LITE_MICRO_EXPECT_NEAR` (function, line 50) `TF_LITE_MICRO_EXPECT_NEAR(w[0], 0.0f, 1e-6f);`
  - `TF_LITE_MICRO_EXPECT_GT` (function, line 51) `TF_LITE_MICRO_EXPECT_GT(w[256], 0.99f);`
  - `buf` (function, line 70) `std::vector<float> buf(n_samples);`
  - `ref` (function, line 92) `spelling::LogMelSpectrogram ref(p);`
  - `out_ref` (function, line 93) `std::vector<float> out_ref(static_cast<std::size_t>(n_mels) * window_frames);`
  - `MakeMelFilterbank` (function, line 99) `spelling::MakeMelFilterbank(n_freq, n_mels, sr, f_min, f_max);`
  - `streamer` (function, line 105) `spelling::MelStreamer streamer(n_mels, window_frames, n_fft, window.data(), nz_off.data(), nz_idx.data(), nz_val.data(), fft, 1e-6f);`
  - `out_stream` (function, line 111) `std::vector<float> out_stream(static_cast<std::size_t>(n_mels) * window_frames);`
  - `kiss_fftr_free` (function, line 120) `kiss_fftr_free(fft);`
  - `TF_LITE_MICRO_EXPECT_LT` (function, line 124) `TF_LITE_MICRO_EXPECT_LT(max_abs, 1e-3);`
- Depends on: `micro/feature-generation/include/feature_generation/feature_generation.h`

## micro/klatt-tts/tests/tts_test.cc
- Layer: testing
- Doc: Unit tests for the TTS synth core, using TFLM's micro_test.h.  Covers the English G2P front-end (text -> phone tokens, n
- Language: cc
- Symbols:
  - `Contains` (function, line 16) `bool Contains(const std::vector<std::string>& toks, const char* needle)`
  - `TF_LITE_MICRO_TEST` (function, line 25) `TF_LITE_MICRO_TESTS_BEGIN

TF_LITE_MICRO_TEST(G2PProducesPhones)`
  - `TF_LITE_MICRO_TEST` (function, line 34) `TF_LITE_MICRO_TEST(G2PNumberNormalization)`
  - `TF_LITE_MICRO_TEST` (function, line 40) `TF_LITE_MICRO_TEST(StreamSynthProducesAudioInRange)`
  - `TF_LITE_MICRO_EXPECT_GT` (function, line 30) `TF_LITE_MICRO_EXPECT_GT(static_cast<int>(toks.size()), 0);`
  - `TF_LITE_MICRO_EXPECT_TRUE` (function, line 32) `TF_LITE_MICRO_EXPECT_TRUE(Contains(toks, " "));`
  - `synth` (function, line 44) `tts::StreamSynth synth(voice, arena, sizeof(arena));`
  - `TF_LITE_MICRO_EXPECT_EQ` (function, line 47) `TF_LITE_MICRO_EXPECT_EQ(synth.BeginText("a", opts), tts::kStreamOk);`
  - `TF_LITE_MICRO_EXPECT_LE` (function, line 62) `TF_LITE_MICRO_EXPECT_LE(peak, 1.5f);`
- Depends on: `micro/g2p/include/g2p/g2p.h`, `micro/klatt-tts/include/tts/tts.h`

## micro/stt/include/stt/stt.h
- Layer: utility
- Doc: stt -- on-device speech-to-text (isolated-letter/digit) classifier.  Single public header for the module. It exposes:  *
- Language: h
- Symbols:
  - `TensorQuant` (struct, line 35)
  - `Impl` (struct, line 74)
  - `Classifier` (class, line 40)
  - `feature_scratch` (function, line 65) `float* feature_scratch() const`
  - `input_quant` (function, line 66) `TensorQuant input_quant() const`
  - `output_quant` (function, line 68) `TensorQuant output_quant() const`
  - `n_classes` (function, line 69) `int n_classes() const`
  - `input_count` (function, line 70) `std::size_t input_count() const`
  - `arena_used_bytes` (function, line 71) `std::size_t arena_used_bytes() const`
  - `Classifier` (function, line 47) `Classifier(const unsigned char* model_data, unsigned int model_size, uint8_t* tensor_arena, std::size_t tensor_arena_size, int expected_n_mels, int expected_target_frames, int expected_n_classes, tfli`
  - `Run` (function, line 60) `void Run(const float* features, float* logits_out) const;`
  - `Argmax` (function, line 90) `int Argmax(const float* logits, int n_logits);`
  - `SoftmaxProb` (function, line 93) `float SoftmaxProb(const float* logits, int n_logits, int index);`
  - `STT_STT_H_` (macro, line 19) `#define STT_STT_H_`
- Imported by: `micro/examples/rp2350/src/audio_service.cc`, `micro/examples/rp2350/src/test_app.cc`, `micro/stt/src/classifier.cc`, `micro/stt/src/predictor.cc`, `micro/stt/tests/predictor_test.cc`

## micro/stt/tests/predictor_test.cc
- Layer: testing
- Doc: Unit tests for the STT prediction helpers, using TFLM's micro_test.h.  Argmax + stable-softmax are the post-processing t
- Language: cc
- Symbols:
  - `TF_LITE_MICRO_TEST` (function, line 11) `TF_LITE_MICRO_TESTS_BEGIN

TF_LITE_MICRO_TEST(ArgmaxPicksLargest)`
  - `TF_LITE_MICRO_TEST` (function, line 18) `TF_LITE_MICRO_TEST(ArgmaxTiesGoToLowestIndex)`
  - `TF_LITE_MICRO_TEST` (function, line 23) `TF_LITE_MICRO_TEST(SoftmaxProbsSumToOne)`
  - `TF_LITE_MICRO_TEST` (function, line 30) `TF_LITE_MICRO_TEST(SoftmaxProbMatchesHandComputed)`
  - `TF_LITE_MICRO_TEST` (function, line 36) `TF_LITE_MICRO_TEST(SoftmaxStableOnLargeLogits)`
  - `TF_LITE_MICRO_EXPECT_EQ` (function, line 16) `TF_LITE_MICRO_EXPECT_EQ(spelling::Argmax(logits, 5), 2);`
  - `TF_LITE_MICRO_EXPECT_NEAR` (function, line 28) `TF_LITE_MICRO_EXPECT_NEAR(sum, 1.0f, 1e-5f);`
  - `TF_LITE_MICRO_EXPECT_GT` (function, line 42) `TF_LITE_MICRO_EXPECT_GT(p, 0.999f);`
  - `TF_LITE_MICRO_EXPECT_LE` (function, line 43) `TF_LITE_MICRO_EXPECT_LE(p, 1.0f);`
- Depends on: `micro/stt/include/stt/stt.h`

## micro/test-support/host/tflm_host_stub.cc
- Layer: testing
- Doc: Host (desktop) implementations of the handful of TFLM platform hooks that the modules and the micro_test.h harness refer
- Language: cc
- Symbols:
  - `MicroPrintf` (function, line 18) `void MicroPrintf(const char* format, ...)`
  - `VMicroPrintf` (function, line 26) `void VMicroPrintf(const char* format, va_list args)`
  - `MicroSnprintf` (function, line 31) `int MicroSnprintf(char* buffer, size_t buf_size, const char* format, ...)`
  - `MicroVsnprintf` (function, line 39) `int MicroVsnprintf(char* buffer, size_t buf_size, const char* format,
                   va_list ...`
  - `InitializeTarget` (function, line 46) `void InitializeTarget()`
  - `va_start` (function, line 21) `va_start(args, format);`
  - `vfprintf` (function, line 22) `vfprintf(stderr, format, args);`
  - `va_end` (function, line 23) `va_end(args);`
  - `fputc` (function, line 24) `fputc('\n', stderr);`
  - `vsnprintf` (function, line 42) `return vsnprintf(buffer, buf_size, format, vlist);`

## micro/test-support/run_micro_test.sh
- Layer: testing
- Doc: Run a TFLM micro_test.h binary and translate its output into an exit code.  micro_test.h wraps the suite in `while (true
- Language: sh

## micro/vad/include/vad/vad.h
- Layer: utility
- Doc: vad -- on-device voice activity detection.  Single public header for the module. It exposes the two halves of the VAD:  
- Language: h
- Symbols:
  - `VadTensorQuant` (struct, line 38)
  - `Impl` (struct, line 72)
  - `VadEvent` (enum, line 85)
  - `Vad` (class, line 43)
  - `VadEvent` (class, line 85)
  - `VadSegmenter` (class, line 96)
  - `feature_scratch` (function, line 64) `float* feature_scratch() const`
  - `input_quant` (function, line 65) `VadTensorQuant input_quant() const`
  - `output_quant` (function, line 67) `VadTensorQuant output_quant() const`
  - `input_count` (function, line 68) `std::size_t input_count() const`
  - `arena_used_bytes` (function, line 69) `std::size_t arena_used_bytes() const`
  - `segment_start_sample` (function, line 113) `std::size_t segment_start_sample() const`
  - `segment_end_sample` (function, line 114) `std::size_t segment_end_sample() const`
  - `samples_processed` (function, line 115) `std::size_t samples_processed() const`
  - `Vad` (function, line 49) `Vad(const unsigned char* model_data, unsigned int model_size, uint8_t* tensor_arena, std::size_t tensor_arena_size, int expected_n_mels, int expected_window_frames, tflite::MicroProfilerInterface* pro`
  - `Predict` (function, line 60) `float Predict(const float* features) const;`
  - `VadSegmenter` (function, line 97) `public: VadSegmenter(float threshold, int window_frames, int hop, std::size_t look_behind_samples, std::size_t max_segment_samples);`
  - `Start` (function, line 103) `void Start();`
  - `ProcessFrame` (function, line 107) `VadEvent ProcessFrame(float raw_probability);`
  - `Finish` (function, line 110) `VadEvent Finish();`
  - `ExtractClipFrontAligned` (function, line 135) `void ExtractClipFrontAligned(const float* src, std::size_t src_len, std::size_t start, std::size_t end, float* out, std::size_t clip_len);`
  - `EnergyCentroidIndex` (function, line 145) `std::size_t EnergyCentroidIndex(const int16_t* buf, std::size_t start, std::size_t end);`
  - `VAD_VAD_H_` (macro, line 23) `#define VAD_VAD_H_`
- Imported by: `micro/examples/rp2350/src/audio_service.cc`, `micro/examples/rp2350/src/test_app.cc`, `micro/vad/src/vad.cc`, `micro/vad/src/vad_segmenter.cc`, `micro/vad/tests/vad_segmenter_test.cc`

## micro/vad/scripts/generate_vad_embedded_data.py
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
- Layer: testing
- Doc: Unit tests for the VAD segmenter, using TFLM's micro_test.h.  These cases exercise segment boundaries (look-behind pre-r
- Language: cc
- Symbols:
  - `Repeat` (function, line 19) `std::vector<float> Repeat(float v, int n)`
  - `Concat` (function, line 21) `std::vector<float> Concat(std::initializer_list<std::vector<float>> parts)`
  - `TF_LITE_MICRO_TEST` (function, line 47) `TF_LITE_MICRO_TESTS_BEGIN

TF_LITE_MICRO_TEST(SingleSegmentDetected)`
  - `TF_LITE_MICRO_TEST` (function, line 59) `TF_LITE_MICRO_TEST(TwoSegmentsDetected)`
  - `TF_LITE_MICRO_TEST` (function, line 67) `TF_LITE_MICRO_TEST(TrailingSegmentFlushed)`
  - `TF_LITE_MICRO_TEST` (function, line 74) `TF_LITE_MICRO_TEST(NoLookBehindStartsLater)`
  - `TF_LITE_MICRO_TEST` (function, line 85) `TF_LITE_MICRO_TEST(ExtractClipFrontAlignedZeroPads)`
  - `TF_LITE_MICRO_TEST` (function, line 95) `TF_LITE_MICRO_TEST(EnergyCentroidIndexWeightsByPower)`
  - `seg` (function, line 32) `spelling::VadSegmenter seg(0.5f, 16, kHop, look_behind, kMaxSeg);`
  - `TF_LITE_MICRO_EXPECT_EQ` (function, line 54) `TF_LITE_MICRO_EXPECT_EQ(static_cast<int>(segs.size()), 1);`
  - `TF_LITE_MICRO_EXPECT_LT` (function, line 57) `TF_LITE_MICRO_EXPECT_LT(segs[0].first, segs[0].second);`
  - `TF_LITE_MICRO_EXPECT_GE` (function, line 83) `TF_LITE_MICRO_EXPECT_GE(no_lb[0].first, with_lb[0].first);`
  - `ExtractClipFrontAligned` (function, line 89) `spelling::ExtractClipFrontAligned(src, 8, /*start=*/2, /*end=*/5, out, 6);`
  - `TF_LITE_MICRO_EXPECT_NEAR` (function, line 90) `TF_LITE_MICRO_EXPECT_NEAR(out[0], 3.0f, 1e-6f);`
- Depends on: `micro/vad/include/vad/vad.h`

## python/setup.py
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
- Layer: utility
- Doc: swift-tools-version: 6.1
- Language: swift
