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
  - `LOG_TAG` (macro, line 12)

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
  - `WIN32_LEAN_AND_MEAN` (macro, line 13)
  - `NOMINMAX` (macro, line 15)

## micro/examples/rp2350/lwipopts.h
- Layer: utility
- Doc: Minimal lwIP configuration for the voice WiFi-setup app (moonshine_micro_echo_wifi).  This firmware only needs to ASSOCI
- Language: h
- Symbols:
  - `SPELLING_LWIPOPTS_H_` (macro, line 17)
  - `NO_SYS` (macro, line 20)
  - `LWIP_SOCKET` (macro, line 21)
  - `LWIP_NETCONN` (macro, line 22)
  - `SYS_LIGHTWEIGHT_PROT` (macro, line 23)
  - `MEM_LIBC_MALLOC` (macro, line 26)
  - `MEM_ALIGNMENT` (macro, line 27)
  - `MEM_SIZE` (macro, line 28)
  - `MEMP_NUM_PBUF` (macro, line 29)
  - `MEMP_NUM_UDP_PCB` (macro, line 30)
  - `MEMP_NUM_ARP_QUEUE` (macro, line 31)
  - `MEMP_NUM_SYS_TIMEOUT` (macro, line 32)
  - `PBUF_POOL_SIZE` (macro, line 33)
  - `PBUF_POOL_BUFSIZE` (macro, line 34)
  - `LWIP_IPV4` (macro, line 37)
  - `LWIP_IPV6` (macro, line 38)
  - `LWIP_ARP` (macro, line 39)
  - `LWIP_ETHERNET` (macro, line 40)
  - `LWIP_ICMP` (macro, line 41)
  - `LWIP_RAW` (macro, line 42)
  - `LWIP_UDP` (macro, line 43)
  - `LWIP_TCP` (macro, line 44)
  - `LWIP_DNS` (macro, line 45)
  - `LWIP_DHCP` (macro, line 46)
  - `DHCP_DOES_ARP_CHECK` (macro, line 47)
  - `LWIP_DHCP_DOES_ACD_CHECK` (macro, line 48)
  - `LWIP_NETIF_STATUS_CALLBACK` (macro, line 51)
  - `LWIP_NETIF_LINK_CALLBACK` (macro, line 52)
  - `LWIP_NETIF_HOSTNAME` (macro, line 53)
  - `LWIP_NETIF_TX_SINGLE_PBUF` (macro, line 54)
  - `LWIP_CHKSUM_ALGORITHM` (macro, line 57)
  - `LWIP_STATS` (macro, line 60)
  - `MEM_STATS` (macro, line 61)
  - `SYS_STATS` (macro, line 62)
  - `MEMP_STATS` (macro, line 63)
  - `LINK_STATS` (macro, line 64)
  - `ETHARP_STATS` (macro, line 65)
  - `IP_STATS` (macro, line 66)
  - `UDP_STATS` (macro, line 67)
  - `ICMP_STATS` (macro, line 68)
  - `LWIP_DEBUG` (macro, line 71)
  - `LWIP_STATS_DISPLAY` (macro, line 73)

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
  - `FEATURE_GENERATION_FEATURE_GENERATION_H_` (macro, line 30)

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
  - `STT_STT_H_` (macro, line 19)

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
  - `VAD_VAD_H_` (macro, line 23)

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
