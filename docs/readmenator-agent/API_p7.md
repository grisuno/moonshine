# API (page 7 of 10)
Previous: [API_p6.md](API_p6.md)

## examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift
- `bootstrapIfNeeded` (function) `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:52`
- `scheduleDebouncedIntentSync` (function) `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:110`
- `phraseTextCommitted` (function) `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:119`
- `addPhrase` (function) `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:132`
- `removePhrase` (function) `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:137`
- `toggleListening` (function) `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:143`
- `handleCompletedTranscriptLine` (function) `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:168`
- `pauseMicIfNeededForBackground` (function) `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:207`
- `handleTranscriptLineStarted` (function) `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:218`
- `handleTranscriptLineTextChanged` (function) `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:226`
- `handleTranscriptLineCompleted` (function) `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:231`

## examples/ios/IntentRecognizer/IntentRecognizer/IntentTranscriptBridge.swift
- `onLineStarted` (function) `examples/ios/IntentRecognizer/IntentRecognizer/IntentTranscriptBridge.swift:7`
- `onLineTextChanged` (function) `examples/ios/IntentRecognizer/IntentRecognizer/IntentTranscriptBridge.swift:13`
- `onLineCompleted` (function) `examples/ios/IntentRecognizer/IntentRecognizer/IntentTranscriptBridge.swift:20`

## examples/ios/TextToSpeech/TextToSpeech/TextToSpeechApp.swift
- `hash` (function) `examples/ios/TextToSpeech/TextToSpeech/TextToSpeechApp.swift:10`
- `hash` (function) `examples/ios/TextToSpeech/TextToSpeech/TextToSpeechApp.swift:65`
- `initialize` (function) `examples/ios/TextToSpeech/TextToSpeech/TextToSpeechApp.swift:95`
- `changeLanguage` (function) `examples/ios/TextToSpeech/TextToSpeech/TextToSpeechApp.swift:173` -- MARK: - Public language / voice switching
- `changeVoice` (function) `examples/ios/TextToSpeech/TextToSpeech/TextToSpeechApp.swift:189`
- `speak` (function) `examples/ios/TextToSpeech/TextToSpeech/TextToSpeechApp.swift:194`

## examples/ios/Transcriber/Transcriber/TranscriberApp.swift
- `addNewMessage` (function) `examples/ios/Transcriber/Transcriber/TranscriberApp.swift:65`
- `updateLatestMessage` (function) `examples/ios/Transcriber/Transcriber/TranscriberApp.swift:69`
- `handleRecordingChanged` (function) `examples/ios/Transcriber/Transcriber/TranscriberApp.swift:73`

## examples/ios/Transcriber/TranscriberUITests/TranscriberUITests.swift
- `setUpWithError` (function) `examples/ios/Transcriber/TranscriberUITests/TranscriberUITests.swift:11`
- `tearDownWithError` (function) `examples/ios/Transcriber/TranscriberUITests/TranscriberUITests.swift:20`
- `testExample` (function) `examples/ios/Transcriber/TranscriberUITests/TranscriberUITests.swift:26`
- `testLaunchPerformance` (function) `examples/ios/Transcriber/TranscriberUITests/TranscriberUITests.swift:35`

## examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift
- `transcribeWithoutStreaming` (function) `examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift:5` -- Transcribe audio data offline without streaming
- `transcribeWithStreaming` (function) `examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift:26` -- Example of streaming transcription
- `onLineStarted` (function) `examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift:33`
- `onLineTextChanged` (function) `examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift:39`
- `onLineCompleted` (function) `examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift:46`
- `parseArguments` (function) `examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift:82`
- `main` (function) `examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift:146` -- MARK: - Main

## examples/macos/MicTranscription/Sources/MicTranscription/main.swift
- `main` (function) `examples/macos/MicTranscription/Sources/MicTranscription/main.swift:5` -- MARK: - Main
- `onLineStarted` (function) `examples/macos/MicTranscription/Sources/MicTranscription/main.swift:42`
- `onLineTextChanged` (function) `examples/macos/MicTranscription/Sources/MicTranscription/main.swift:48`
- `onLineCompleted` (function) `examples/macos/MicTranscription/Sources/MicTranscription/main.swift:55`

## examples/macos/TextToSpeech/Sources/TextToSpeech/main.swift
- `writeWav` (function) `examples/macos/TextToSpeech/Sources/TextToSpeech/main.swift:6` -- MARK: - WAV Writing
- `printUsage` (function) `examples/macos/TextToSpeech/Sources/TextToSpeech/main.swift:66`
- `parseArguments` (function) `examples/macos/TextToSpeech/Sources/TextToSpeech/main.swift:86`
- `resolveAssetRoot` (function) `examples/macos/TextToSpeech/Sources/TextToSpeech/main.swift:163` -- MARK: - Asset Root Resolution
- `resolveDevice` (function) `examples/macos/TextToSpeech/Sources/TextToSpeech/main.swift:205` -- MARK: - Device Resolution
- `main` (function) `examples/macos/TextToSpeech/Sources/TextToSpeech/main.swift:246` -- MARK: - Main

## examples/python/basic_transcription.py
- `transcribe_without_streaming` (function) `examples/python/basic_transcription.py:16` `def transcribe_without_streaming(transcriber, audio_data, sample_rate)` -- Transcribe audio data offline without streaming.
- `transcribe_with_streaming` (function) `examples/python/basic_transcription.py:30` `def transcribe_with_streaming(transcriber, audio_data, sample_rate)` -- Example of streaming transcription.
- `TestListener.on_line_started` (method) `examples/python/basic_transcription.py:38` `def on_line_started(self, event)`
- `TestListener.on_line_text_changed` (method) `examples/python/basic_transcription.py:41` `def on_line_text_changed(self, event)`
- `TestListener.on_line_completed` (method) `examples/python/basic_transcription.py:44` `def on_line_completed(self, event)`

## examples/python/dialog_flow.py
- `setup_wifi` (function) `examples/python/dialog_flow.py:46` `def setup_wifi(d)` -- Classic slot-filling flow: network name, password, confirm, apply.
- `set_timezone` (function) `examples/python/dialog_flow.py:70` `def set_timezone(d)` -- Sub-flow that can be composed with ``yield from``.
- `full_onboarding` (function) `examples/python/dialog_flow.py:80` `def full_onboarding(d)` -- Compose sub-flows with ``yield from``.
- `TranscriptPrinter.__init__` (method) `examples/python/dialog_flow.py:112` `def __init__(self)`
- `TranscriptPrinter.on_line_started` (method) `examples/python/dialog_flow.py:122` `def on_line_started(self, event)`
- `TranscriptPrinter.on_line_text_changed` (method) `examples/python/dialog_flow.py:125` `def on_line_text_changed(self, event)`
- `TranscriptPrinter.on_line_completed` (method) `examples/python/dialog_flow.py:128` `def on_line_completed(self, event)`
- `TranscriptPrinter.run_live` (method) `examples/python/dialog_flow.py:142` `def run_live(args)`
- `TranscriptPrinter.mute` (method) `examples/python/dialog_flow.py:202` `def mute(should_mute)`
- `TranscriptPrinter.set_spelling_mode` (method) `examples/python/dialog_flow.py:206` `def set_spelling_mode(active)` -- Toggle the C++ spelling-CNN fusion path on the live mic stream.
- `TranscriptPrinter.speak` (method) `examples/python/dialog_flow.py:212` `def speak(text)` -- Log every spoken prompt and (optionally) pass it through TTS.
- `TranscriptPrinter.run_interactive` (method) `examples/python/dialog_flow.py:279` `def run_interactive(flow_name)` -- Keyboard-driven demo – prompts go to stdout, replies come from stdin.
- `TranscriptPrinter.speak` (method) `examples/python/dialog_flow.py:293` `def speak(text)`
- `TranscriptPrinter.run_scripted` (method) `examples/python/dialog_flow.py:347` `def run_scripted(flow_name, answers)` -- Drive a flow from a pre-canned list of utterances.
- `TranscriptPrinter.speak` (method) `examples/python/dialog_flow.py:363` `def speak(text)`
- `TranscriptPrinter.main` (method) `examples/python/dialog_flow.py:411` `def main()`

## examples/python/intent_recognition.py
- `on_lights_on` (function) `examples/python/intent_recognition.py:26` `def on_lights_on(trigger, utterance, similarity)` -- Handler for turning lights on.
- `on_lights_off` (function) `examples/python/intent_recognition.py:31` `def on_lights_off(trigger, utterance, similarity)` -- Handler for turning lights off.
- `on_weather` (function) `examples/python/intent_recognition.py:36` `def on_weather(trigger, utterance, similarity)` -- Handler for weather queries.
- `on_timer` (function) `examples/python/intent_recognition.py:41` `def on_timer(trigger, utterance, similarity)` -- Handler for timer requests.
- `on_music_play` (function) `examples/python/intent_recognition.py:46` `def on_music_play(trigger, utterance, similarity)` -- Handler for playing music.
- `on_music_stop` (function) `examples/python/intent_recognition.py:51` `def on_music_stop(trigger, utterance, similarity)` -- Handler for stopping music.
- `TranscriptPrinter.__init__` (method) `examples/python/intent_recognition.py:59` `def __init__(self)`
- `TranscriptPrinter.update_last_terminal_line` (method) `examples/python/intent_recognition.py:62` `def update_last_terminal_line(self, new_text)`
- `TranscriptPrinter.on_line_started` (method) `examples/python/intent_recognition.py:69` `def on_line_started(self, event)`
- `TranscriptPrinter.on_line_text_changed` (method) `examples/python/intent_recognition.py:72` `def on_line_text_changed(self, event)`
- `TranscriptPrinter.on_line_completed` (method) `examples/python/intent_recognition.py:75` `def on_line_completed(self, event)`
- `TranscriptPrinter.main` (method) `examples/python/intent_recognition.py:80` `def main()`

## examples/python/mic_transcription.py
- `TerminalListener.__init__` (method) `examples/python/mic_transcription.py:15` `def __init__(self)`
- `TerminalListener.update_last_terminal_line` (method) `examples/python/mic_transcription.py:20` `def update_last_terminal_line(self, new_text)`
- `TerminalListener.on_line_started` (method) `examples/python/mic_transcription.py:30` `def on_line_started(self, event)`
- `TerminalListener.on_line_text_changed` (method) `examples/python/mic_transcription.py:33` `def on_line_text_changed(self, event)`
- `TerminalListener.on_line_completed` (method) `examples/python/mic_transcription.py:36` `def on_line_completed(self, event)`
- `FileListener.on_line_completed` (method) `examples/python/mic_transcription.py:45` `def on_line_completed(self, event)`

## examples/python/ollama-voice/ollama_voice.py
- `Spinner.__init__` (method) `examples/python/ollama-voice/ollama_voice.py:17` `def __init__(self)`
- `Spinner.spin` (method) `examples/python/ollama-voice/ollama_voice.py:20` `def spin(self)`
- `OllamaVoice.__init__` (method) `examples/python/ollama-voice/ollama_voice.py:34` `def __init__(self, ollama_model, system_prompt)` -- Initialize the OllamaVoice listener.
- `OllamaVoice.on_line_text_changed` (method) `examples/python/ollama-voice/ollama_voice.py:59` `def on_line_text_changed(self, event)` -- Called whenever the transcription of the current line changes (live updates).
- `OllamaVoice.on_line_completed` (method) `examples/python/ollama-voice/ollama_voice.py:69` `def on_line_completed(self, event)` -- Called when a line (segment) of speech has been fully transcribed.

## examples/raspberry-pi/my-dalek/my-dalek.py
- `on_intent_triggered_on` (function) `examples/raspberry-pi/my-dalek/my-dalek.py:38` `def on_intent_triggered_on(trigger, utterance, similarity)` -- Handler for when an intent is triggered.
- `TranscriptPrinter.__init__` (method) `examples/raspberry-pi/my-dalek/my-dalek.py:47` `def __init__(self)`
- `TranscriptPrinter.update_last_terminal_line` (method) `examples/raspberry-pi/my-dalek/my-dalek.py:50` `def update_last_terminal_line(self, new_text)`
- `TranscriptPrinter.on_line_started` (method) `examples/raspberry-pi/my-dalek/my-dalek.py:57` `def on_line_started(self, event)`
- `TranscriptPrinter.on_line_text_changed` (method) `examples/raspberry-pi/my-dalek/my-dalek.py:60` `def on_line_text_changed(self, event)`
- `TranscriptPrinter.on_line_completed` (method) `examples/raspberry-pi/my-dalek/my-dalek.py:63` `def on_line_completed(self, event)`
- `TranscriptPrinter.on_move_forward` (method) `examples/raspberry-pi/my-dalek/my-dalek.py:92` `def on_move_forward(trigger, utterance, similarity)`
- `TranscriptPrinter.on_move_backward` (method) `examples/raspberry-pi/my-dalek/my-dalek.py:94` `def on_move_backward(trigger, utterance, similarity)`
- `TranscriptPrinter.on_turn_left` (method) `examples/raspberry-pi/my-dalek/my-dalek.py:96` `def on_turn_left(trigger, utterance, similarity)`
- `TranscriptPrinter.on_turn_right` (method) `examples/raspberry-pi/my-dalek/my-dalek.py:98` `def on_turn_right(trigger, utterance, similarity)`
- `TranscriptPrinter.on_exterminate` (method) `examples/raspberry-pi/my-dalek/my-dalek.py:100` `def on_exterminate(trigger, utterance, similarity)`

## examples/windows/cli-transcriber/cli-transcriber.cpp
Depends on: `core/moonshine-cpp.h`
- `COMInitializer` (function) `examples/windows/cli-transcriber/cli-transcriber.cpp:26` `public:
  COMInitializer()`
- `onLineStarted` (function) `examples/windows/cli-transcriber/cli-transcriber.cpp:38` `public:
  void onLineStarted(const moonshine::LineStarted &event) override`
- `onLineTextChanged` (function) `examples/windows/cli-transcriber/cli-transcriber.cpp:44` `void onLineTextChanged(const moonshine::LineTextChanged &event) override`
- `onLineCompleted` (function) `examples/windows/cli-transcriber/cli-transcriber.cpp:52` `void onLineCompleted(const moonshine::LineCompleted &event) override`
- `onError` (function) `examples/windows/cli-transcriber/cli-transcriber.cpp:60` `void onError(const moonshine::Error &event) override`
- `MicrophoneCapture` (function) `examples/windows/cli-transcriber/cli-transcriber.cpp:73` `public:
  MicrophoneCapture() : is_capturing_(false), sample_rate_(16000)`
- `Initialize` (function) `examples/windows/cli-transcriber/cli-transcriber.cpp:95` `bool Initialize()`
- `Start` (function) `examples/windows/cli-transcriber/cli-transcriber.cpp:192` `void Start()`
- `Stop` (function) `examples/windows/cli-transcriber/cli-transcriber.cpp:208` `void Stop()`
- `SetAudioCallback` (function) `examples/windows/cli-transcriber/cli-transcriber.cpp:223` `void SetAudioCallback(
      std::function<void(const std::vector<float> &, int32_t)> callback)`
- `CaptureLoop` (function) `examples/windows/cli-transcriber/cli-transcriber.cpp:229` `private:
  void CaptureLoop()`
- `WavFileProducer` (function) `examples/windows/cli-transcriber/cli-transcriber.cpp:326` `public:
  explicit WavFileProducer(std::string wav_path,
                           float chunk_d...`
- `getNextAudio` (function) `examples/windows/cli-transcriber/cli-transcriber.cpp:336` `bool getNextAudio(std::vector<float> &out_audio_data)`
- `sampleRate` (function) `examples/windows/cli-transcriber/cli-transcriber.cpp:348` `int32_t sampleRate() const`
- `loadWavData` (function) `examples/windows/cli-transcriber/cli-transcriber.cpp:351` `private:
  void loadWavData(const std::string &wav_path)`
- `pcm_data` (function) `examples/windows/cli-transcriber/cli-transcriber.cpp:428` `std::vector<int16_t> pcm_data(num_samples);`
- `runWavTranscription` (function) `examples/windows/cli-transcriber/cli-transcriber.cpp:456` `int runWavTranscription(const std::string &model_path,
                        moonshine::ModelAr...`
- `main` (function) `examples/windows/cli-transcriber/cli-transcriber.cpp:489` `int main(int argc, char *argv[])`

## micro/examples/rp2350/generated/neural_tts_pack.S
- `g_neural_tts_pack` (function) `micro/examples/rp2350/generated/neural_tts_pack.S:5`
- `g_neural_tts_pack_end` (function) `micro/examples/rp2350/generated/neural_tts_pack.S:8`

## micro/examples/rp2350/scripts/capture_neural_tts.py
- `find_port` (function) `micro/examples/rp2350/scripts/capture_neural_tts.py:22` `def find_port()`
- `main` (function) `micro/examples/rp2350/scripts/capture_neural_tts.py:29` `def main()`

## micro/examples/rp2350/scripts/capture_stt.py
- `SerialReader.__init__` (method) `micro/examples/rp2350/scripts/capture_stt.py:74` `def __init__(self, fd)`
- `SerialReader.readline` (method) `micro/examples/rp2350/scripts/capture_stt.py:92` `def readline(self)`
- `SerialReader.read_exact` (method) `micro/examples/rp2350/scripts/capture_stt.py:100` `def read_exact(self, n)`
- `SerialReader.main` (method) `micro/examples/rp2350/scripts/capture_stt.py:117` `def main()`

## micro/examples/rp2350/scripts/flash.sh
- `find_mounted_volume` (function) `micro/examples/rp2350/scripts/flash.sh:66` -- Echo the first currently-mounted candidate (empty if none are mounted yet).
- `usage` (function) `micro/examples/rp2350/scripts/flash.sh:78` -- Require a variant argument and map it to the firmware artifact name.
- `wait_volume_writable` (function) `micro/examples/rp2350/scripts/flash.sh:227` -- macOS sometimes reports the BOOTSEL volume before it's actually writable (Permission denied on the first cp).
- `draw_bar` (function) `micro/examples/rp2350/scripts/flash.sh:259` -- 2.

## micro/examples/rp2350/scripts/tts_speak.py
- `find_port` (function) `micro/examples/rp2350/scripts/tts_speak.py:36` `def find_port()`
- `main` (function) `micro/examples/rp2350/scripts/tts_speak.py:44` `def main()`
- `send_line` (function) `micro/examples/rp2350/scripts/tts_speak.py:71` `def send_line(s)`

## micro/examples/rp2350/scripts/usb_audio_bridge.py
- `SerialReader.__init__` (method) `micro/examples/rp2350/scripts/usb_audio_bridge.py:104` `def __init__(self, fd)`
- `SerialReader.readline` (method) `micro/examples/rp2350/scripts/usb_audio_bridge.py:123` `def readline(self)`
- `SerialReader.read_exact` (method) `micro/examples/rp2350/scripts/usb_audio_bridge.py:131` `def read_exact(self, n)`
- `SerialReader.main` (method) `micro/examples/rp2350/scripts/usb_audio_bridge.py:140` `def main()`
- `SerialReader.save_stream` (method) `micro/examples/rp2350/scripts/usb_audio_bridge.py:184` `def save_stream(tag, samples, rate)`
- `SerialReader.on_audio` (method) `micro/examples/rp2350/scripts/usb_audio_bridge.py:206` `def on_audio(indata, frames, time_info, status)`
- `SerialReader.sender` (method) `micro/examples/rp2350/scripts/usb_audio_bridge.py:224` `def sender()`
- `SerialReader.flush_mic` (method) `micro/examples/rp2350/scripts/usb_audio_bridge.py:260` `def flush_mic()`
- `SerialReader.receiver` (method) `micro/examples/rp2350/scripts/usb_audio_bridge.py:268` `def receiver()`

## micro/examples/rp2350/src/app_common.cc
Depends on: `micro/examples/rp2350/generated/classes.h`, `micro/examples/rp2350/generated/mel_tables.h`, `micro/examples/rp2350/generated/model_data.h`, `micro/examples/rp2350/src/app_common.h`
- `LedPulse` (function) `micro/examples/rp2350/src/app_common.cc:33` `void LedPulse(unsigned pin, int count, int on_ms, int off_ms)`
- `BoardInit` (function) `micro/examples/rp2350/src/app_common.cc:42` `unsigned BoardInit()`
- `PrintBootBanner` (function) `micro/examples/rp2350/src/app_common.cc:84` `void PrintBootBanner()`

## micro/examples/rp2350/src/app_common.h
Depends on: `micro/examples/rp2350/generated/audio_config.h`
Imported by: `micro/examples/rp2350/src/app_common.cc`, `micro/examples/rp2350/src/echo_app.cc`, `micro/examples/rp2350/src/echo_hardware_app.cc`, `micro/examples/rp2350/src/main_echo_hardware.cc`, `micro/examples/rp2350/src/main_live.cc`, `micro/examples/rp2350/src/main_test.cc`, `micro/examples/rp2350/src/main_wifi.cc`, `micro/examples/rp2350/src/main_wifi_hardware.cc`, `micro/examples/rp2350/src/test_app.cc`, `micro/examples/rp2350/src/wifi_app.cc`
- `BoardInit` (function) `micro/examples/rp2350/src/app_common.h:48` `unsigned BoardInit();` -- Bring up the board: overclock to 250 MHz (core voltage bumped first), LED POST pulses, USB CDC stdio, and wait up to...
- `PrintBootBanner` (function) `micro/examples/rp2350/src/app_common.h:52` `void PrintBootBanner();` -- Print the boot banner shared by both paths (clock, cores, model size, classes, mel config, arena size).
- `LedPulse` (function) `micro/examples/rp2350/src/app_common.h:55` `void LedPulse(unsigned pin, int count, int on_ms, int off_ms);` -- Pulse the LED `count` times (POST / fault / heartbeat signaling).

## micro/examples/rp2350/src/audio_service.cc
Depends on: `micro/examples/rp2350/generated/audio_config.h`, `micro/examples/rp2350/generated/classes.h`, `micro/examples/rp2350/generated/mel_tables.h`, `micro/examples/rp2350/generated/model_data.h`, `micro/examples/rp2350/generated/vad_config.h`, `micro/examples/rp2350/generated/vad_mel_tables.h`, `micro/examples/rp2350/generated/vad_model_data.h`, `micro/examples/rp2350/src/audio_service.h`, `micro/examples/rp2350/src/spelling_labels.h`, `micro/feature-generation/include/feature_generation/feature_generation.h`, `micro/neural-tts/include/neural_tts/neural_tts.h`, `micro/stt/include/stt/stt.h`, `micro/vad/include/vad/vad.h`
- `SetTtsVolume` (function) `micro/examples/rp2350/src/audio_service.cc:66` `void SetTtsVolume(float volume)`
- `TtsVolume` (function) `micro/examples/rp2350/src/audio_service.cc:72` `float TtsVolume()`
- `RecognizerInit` (function) `micro/examples/rp2350/src/audio_service.cc:74` `void RecognizerInit(kiss_fftr_state* fft)`
- `RecognizeOne` (function) `micro/examples/rp2350/src/audio_service.cc:103` `int RecognizeOne(AudioInput& input, uint8_t* arena, std::size_t arena_size,
                 int1...`
- `PlayCapturedClip` (function) `micro/examples/rp2350/src/audio_service.cc:386` `void PlayCapturedClip(const int16_t* window, int num_samples,
                      AudioOutput& ...` -- Play back the front-aligned capture window (what the classifier saw) before the TTS reply so mic wiring/gain issues...
- `SpeakEmit` (function) `micro/examples/rp2350/src/audio_service.cc:440` `void SpeakEmit(void* user, const int16_t* samples, int n)`
- `SkipSpaces` (function) `micro/examples/rp2350/src/audio_service.cc:464` `const char* SkipSpaces(const char* p)`
- `PopClause` (function) `micro/examples/rp2350/src/audio_service.cc:472` `const char* PopClause(const char* text, char* out, size_t cap)` -- Copy one clause from `text` into `out` (cap bytes).
- `Speak` (function) `micro/examples/rp2350/src/audio_service.cc:499` `void Speak(const char* text, AudioOutput& output, AudioInput& input,
           uint8_t* arena, s...`
- `RunAudioService` (function) `micro/examples/rp2350/src/audio_service.cc:547` `void RunAudioService(AudioInput& input, AudioOutput& output, uint8_t* arena,
                    ...`

## micro/examples/rp2350/src/audio_service.h
Depends on: `micro/examples/rp2350/src/audio_io.h`
Imported by: `micro/examples/rp2350/src/audio_service.cc`, `micro/examples/rp2350/src/echo_app.cc`, `micro/examples/rp2350/src/echo_hardware_app.cc`, `micro/examples/rp2350/src/wifi_app.cc`
- `RecognizerInit` (function) `micro/examples/rp2350/src/audio_service.h:38` `void RecognizerInit(kiss_fftr_state* fft);` -- Build the persistent recognizer front-end (the streaming VAD mel front-end, the STT log-mel, and their shared 512-pt...
- `RecognizeOne` (function) `micro/examples/rp2350/src/audio_service.h:46` `int RecognizeOne(AudioInput& input, uint8_t* arena, std::size_t arena_size, int16_t* window, int window_samples...` -- Listen on `input` until the streaming VAD reports a completed speech segment, front-align the 1 s clip into...
- `SetTtsVolume` (function) `micro/examples/rp2350/src/audio_service.h:61` `void SetTtsVolume(float volume);` -- Playback volume for the spoken reply, as a linear multiplier on the TTS PCM.
- `TtsVolume` (function) `micro/examples/rp2350/src/audio_service.h:62` `float TtsVolume();`
- `Speak` (function) `micro/examples/rp2350/src/audio_service.h:68` `void Speak(const char* text, AudioOutput& output, AudioInput& input, uint8_t* arena, std::size_t arena_size);` -- Synthesize `text` with the formant TTS and stream it to `output`, draining `input` while we speak so our own audio...
- `RunAudioService` (function) `micro/examples/rp2350/src/audio_service.h:77` `void RunAudioService(AudioInput& input, AudioOutput& output, uint8_t* arena, std::size_t arena_size...` -- Never returns: runs the live recognition loop forever.

## micro/examples/rp2350/src/echo_app.cc
Depends on: `micro/examples/rp2350/generated/audio_config.h`, `micro/examples/rp2350/generated/mel_tables.h`, `micro/examples/rp2350/generated/vad_config.h`, `micro/examples/rp2350/generated/vad_mel_tables.h`, `micro/examples/rp2350/src/app_common.h`, `micro/examples/rp2350/src/audio_service.h`, `micro/examples/rp2350/src/echo_app.h`, `micro/examples/rp2350/src/usb_audio_io.h`
- `RunEchoApp` (function) `micro/examples/rp2350/src/echo_app.cc:28` `void RunEchoApp()`

## micro/examples/rp2350/src/echo_hardware_app.cc
Depends on: `micro/examples/rp2350/generated/audio_config.h`, `micro/examples/rp2350/generated/mel_tables.h`, `micro/examples/rp2350/generated/vad_config.h`, `micro/examples/rp2350/generated/vad_mel_tables.h`, `micro/examples/rp2350/src/app_common.h`, `micro/examples/rp2350/src/audio_service.h`, `micro/examples/rp2350/src/echo_hardware_app.h`, `micro/examples/rp2350/src/i2s_audio_io.h`, `micro/examples/rp2350/src/i2s_audio_out.h`
- `RunEchoHardwareApp` (function) `micro/examples/rp2350/src/echo_hardware_app.cc:24` `void RunEchoHardwareApp()`

## micro/examples/rp2350/src/i2s_audio_io.cc
Depends on: `micro/examples/rp2350/src/i2s_audio_io.h`, `micro/examples/rp2350/src/i2s_mic_process.h`
- `CaptureWriteIdx` (function) `micro/examples/rp2350/src/i2s_audio_io.cc:49` `inline unsigned CaptureWriteIdx()` -- Current DMA write position as a ring word index (0..kRingWords-1).
- `StartCaptureDma` (function) `micro/examples/rp2350/src/i2s_audio_io.cc:55` `void StartCaptureDma()`
- `I2sAudioInput` (function) `micro/examples/rp2350/src/i2s_audio_io.cc:76` `I2sAudioInput::I2sAudioInput(int sample_rate)
    : sm_(0), dc_blocker_(sample_rate)`
- `ReadHop` (function) `micro/examples/rp2350/src/i2s_audio_io.cc:96` `bool I2sAudioInput::ReadHop(int16_t* out, int n)`
- `Drain` (function) `micro/examples/rp2350/src/i2s_audio_io.cc:114` `void I2sAudioInput::Drain()`

## micro/examples/rp2350/src/i2s_audio_out.cc
Depends on: `micro/examples/rp2350/src/i2s_audio_out.h`
- `StereoFrame` (function) `micro/examples/rp2350/src/i2s_audio_out.cc:20` `inline uint32_t StereoFrame(int16_t s)` -- Pack one mono int16 sample into a 32-bit stereo I2S frame: MSB-first shift means [31:16] is the ws=0 slot and [15:0]...
- `PeakNormalizeGain` (function) `micro/examples/rp2350/src/i2s_audio_out.cc:43` `float PeakNormalizeGain(const int16_t* samples, int n, float target,
                        floa...`
- `PeakNormalizeGain` (function) `micro/examples/rp2350/src/i2s_audio_out.cc:58` `float PeakNormalizeGain(const float* samples, int n, float target,
                        float ...`
- `I2sAudioOutput` (function) `micro/examples/rp2350/src/i2s_audio_out.cc:72` `I2sAudioOutput::I2sAudioOutput(unsigned data_pin, unsigned clock_base,
                          ...`
- `ReadIdx` (function) `micro/examples/rp2350/src/i2s_audio_out.cc:101` `unsigned I2sAudioOutput::ReadIdx() const`
- `Used` (function) `micro/examples/rp2350/src/i2s_audio_out.cc:107` `unsigned I2sAudioOutput::Used() const`
- `StartDma` (function) `micro/examples/rp2350/src/i2s_audio_out.cc:111` `void I2sAudioOutput::StartDma()`
- `PushFrame` (function) `micro/examples/rp2350/src/i2s_audio_out.cc:118` `void I2sAudioOutput::PushFrame(uint32_t frame)`
- `ApplyClockDiv` (function) `micro/examples/rp2350/src/i2s_audio_out.cc:131` `void I2sAudioOutput::ApplyClockDiv()`
- `Begin` (function) `micro/examples/rp2350/src/i2s_audio_out.cc:140` `void I2sAudioOutput::Begin(int sample_rate, int num_samples, const char* kind)`
- `Write` (function) `micro/examples/rp2350/src/i2s_audio_out.cc:158` `void I2sAudioOutput::Write(const int16_t* samples, int n)`
- `End` (function) `micro/examples/rp2350/src/i2s_audio_out.cc:167` `void I2sAudioOutput::End()`

## micro/examples/rp2350/src/i2s_audio_out.h
Depends on: `micro/examples/rp2350/src/audio_io.h`
Imported by: `micro/examples/rp2350/src/echo_hardware_app.cc`, `micro/examples/rp2350/src/i2s_audio_out.cc`, `micro/examples/rp2350/src/main_audio_loopback_test.cc`, `micro/examples/rp2350/src/main_i2s_audio_test.cc`, `micro/examples/rp2350/src/main_i2s_relay.cc`, `micro/examples/rp2350/src/wifi_hardware_app.cc`
- `PeakNormalizeGain` (function) `micro/examples/rp2350/src/i2s_audio_out.h:37` `float PeakNormalizeGain(const int16_t* samples, int n, float target = 0.9f, float max_gain = 32.0f);` -- Peak-normalization gain so the loudest sample maps to `target` of full scale.
- `SetGain` (function) `micro/examples/rp2350/src/i2s_audio_out.h:56` `void SetGain(float gain)` -- Linear playback gain applied before I2S conversion.
- `ApplyClockDiv` (function) `micro/examples/rp2350/src/i2s_audio_out.h:60` `void ApplyClockDiv();` -- (Re)configure the SM clock divider for the current sample rate.
- `PushFrame` (function) `micro/examples/rp2350/src/i2s_audio_out.h:63` `void PushFrame(uint32_t frame);` -- Push one packed stereo frame into the ring, blocking (spin) while the ring is full so the DMA's real-time drain sets...
- `StartDma` (function) `micro/examples/rp2350/src/i2s_audio_out.h:66` `void StartDma();` -- Kick the drain DMA (read from the ring base, DREQ-paced) once enough has been pre-buffered.
- `ReadIdx` (function) `micro/examples/rp2350/src/i2s_audio_out.h:68` `unsigned ReadIdx() const;` -- DMA read cursor and buffered-frame count, as ring-word indices.
- `Used` (function) `micro/examples/rp2350/src/i2s_audio_out.h:69` `unsigned Used() const;`

## micro/examples/rp2350/src/i2s_mic_process.cc
Depends on: `micro/examples/rp2350/src/i2s_mic_process.h`
- `I2sRawToInt32` (function) `micro/examples/rp2350/src/i2s_mic_process.cc:8` `int32_t I2sRawToInt32(uint32_t raw)`
- `I2sRawToInt16` (function) `micro/examples/rp2350/src/i2s_mic_process.cc:12` `int16_t I2sRawToInt16(uint32_t raw)`
- `I2sDcBlocker` (function) `micro/examples/rp2350/src/i2s_mic_process.cc:18` `I2sDcBlocker::I2sDcBlocker(int sample_rate_hz, float cutoff_hz)
    : r_(std::exp(-2.f * 3.141592...`
- `Process` (function) `micro/examples/rp2350/src/i2s_mic_process.cc:22` `int16_t I2sDcBlocker::Process(int16_t x)`
- `Reset` (function) `micro/examples/rp2350/src/i2s_mic_process.cc:32` `void I2sDcBlocker::Reset()`
- `I2sRemoveBufferDc` (function) `micro/examples/rp2350/src/i2s_mic_process.cc:37` `void I2sRemoveBufferDc(int16_t* samples, int n)`

## micro/examples/rp2350/src/i2s_mic_process.h
Imported by: `micro/examples/rp2350/src/i2s_audio_io.cc`, `micro/examples/rp2350/src/i2s_audio_io.h`, `micro/examples/rp2350/src/i2s_mic_process.cc`, `micro/examples/rp2350/src/main_i2s_mic_test.cc`
- `I2sRawToInt32` (function) `micro/examples/rp2350/src/i2s_mic_process.h:16` `int32_t I2sRawToInt32(uint32_t raw);`
- `I2sRawToInt16` (function) `micro/examples/rp2350/src/i2s_mic_process.h:17` `int16_t I2sRawToInt16(uint32_t raw);`
- `Process` (function) `micro/examples/rp2350/src/i2s_mic_process.h:24` `int16_t Process(int16_t x);`
- `Reset` (function) `micro/examples/rp2350/src/i2s_mic_process.h:25` `void Reset();`
- `I2sRemoveBufferDc` (function) `micro/examples/rp2350/src/i2s_mic_process.h:34` `void I2sRemoveBufferDc(int16_t* samples, int n);` -- Subtract the buffer mean (quick residual DC trim before host playback).

## micro/examples/rp2350/src/main_echo_hardware.cc
Depends on: `micro/examples/rp2350/src/app_common.h`, `micro/examples/rp2350/src/echo_hardware_app.h`
- `main` (function) `micro/examples/rp2350/src/main_echo_hardware.cc:10` `int main()`

## micro/examples/rp2350/src/main_i2s_relay.cc
Depends on: `micro/examples/rp2350/src/i2s_audio_out.h`
- `ReadLine` (function) `micro/examples/rp2350/src/main_i2s_relay.cc:71` `int ReadLine(char* buf, int maxlen)` -- Read one newline-terminated line into `buf` (NUL-terminated), blocking until a non-empty line arrives.
- `ReadByteTimed` (function) `micro/examples/rp2350/src/main_i2s_relay.cc:88` `int ReadByteTimed(int timeout_ms)` -- Read one byte, waiting up to ~timeout_ms.
- `ReadHop` (function) `micro/examples/rp2350/src/main_i2s_relay.cc:98` `int ReadHop(int16_t* out, int n)` -- Scan for the 0xA5 0x5A sync, then read up to `n` int16 LE samples into `out`.
- `PlayStream` (function) `micro/examples/rp2350/src/main_i2s_relay.cc:140` `int PlayStream(spelling::I2sAudioOutput& out, int rate, int total)` -- Receive `total` samples from the host into RAM, then play them to the I2S amp at `rate` Hz.
- `main` (function) `micro/examples/rp2350/src/main_i2s_relay.cc:182` `int main()`

## micro/examples/rp2350/src/main_live.cc
Depends on: `micro/examples/rp2350/src/app_common.h`, `micro/examples/rp2350/src/echo_app.h`
- `main` (function) `micro/examples/rp2350/src/main_live.cc:11` `int main()`

## micro/examples/rp2350/src/main_step1_blinky.cc
- `main` (function) `micro/examples/rp2350/src/main_step1_blinky.cc:11` `int main()`

## micro/examples/rp2350/src/main_step1_blinky_w.cc
- `main` (function) `micro/examples/rp2350/src/main_step1_blinky_w.cc:10` `int main()`

## micro/examples/rp2350/src/main_step2_printf.cc
- `LedInit` (function) `micro/examples/rp2350/src/main_step2_printf.cc:17` `bool LedInit()`
- `LedPut` (function) `micro/examples/rp2350/src/main_step2_printf.cc:27` `void LedPut(bool on)`
- `main` (function) `micro/examples/rp2350/src/main_step2_printf.cc:37` `int main()`

## micro/examples/rp2350/src/main_step3_fft.cc
- `LedInit` (function) `micro/examples/rp2350/src/main_step3_fft.cc:19` `bool LedInit()`
- `LedPut` (function) `micro/examples/rp2350/src/main_step3_fft.cc:29` `void LedPut(bool on)`
- `main` (function) `micro/examples/rp2350/src/main_step3_fft.cc:43` `int main()`

## micro/examples/rp2350/src/main_step5_synth.cc
Depends on: `micro/neural-tts/include/neural_tts/worldlite_synth.h`
- `LedInit` (function) `micro/examples/rp2350/src/main_step5_synth.cc:23` `bool LedInit()`
- `LedPut` (function) `micro/examples/rp2350/src/main_step5_synth.cc:33` `void LedPut(bool on)`
- `main` (function) `micro/examples/rp2350/src/main_step5_synth.cc:43` `int main()`

## micro/examples/rp2350/src/main_step6_decoder.cc
Depends on: `micro/examples/rp2350/generated/neural_tts_demo_data.h`, `micro/neural-tts/include/neural_tts/pb_decoder.h`, `micro/neural-tts/include/neural_tts/worldlite_synth.h`
- `LedInit` (function) `micro/examples/rp2350/src/main_step6_decoder.cc:28` `bool LedInit()`
- `LedPut` (function) `micro/examples/rp2350/src/main_step6_decoder.cc:38` `void LedPut(bool on)`
- `main` (function) `micro/examples/rp2350/src/main_step6_decoder.cc:51` `int main()`
- `decoder` (function) `micro/examples/rp2350/src/main_step6_decoder.cc:97` `static neural_tts::PbDecoder decoder(cfg, g_arena, kArenaBytes);`

## micro/examples/rp2350/src/main_step7_synthesize.cc
Depends on: `micro/examples/rp2350/generated/neural_tts_demo_data.h`, `micro/neural-tts/include/neural_tts/pb_decoder.h`, `micro/neural-tts/include/neural_tts/worldlite_synth.h`
- `LedInit` (function) `micro/examples/rp2350/src/main_step7_synthesize.cc:35` `bool LedInit()`
- `LedPut` (function) `micro/examples/rp2350/src/main_step7_synthesize.cc:45` `void LedPut(bool on)`
- `DiscardPcm` (function) `micro/examples/rp2350/src/main_step7_synthesize.cc:56` `void DiscardPcm(void* user, const int16_t* samples, int n)`
- `PaintStack` (function) `micro/examples/rp2350/src/main_step7_synthesize.cc:66` `void PaintStack()`
- `StackFreeBytes` (function) `micro/examples/rp2350/src/main_step7_synthesize.cc:74` `uint32_t StackFreeBytes()`
- `main` (function) `micro/examples/rp2350/src/main_step7_synthesize.cc:83` `int main()`
- `decoder` (function) `micro/examples/rp2350/src/main_step7_synthesize.cc:122` `static neural_tts::PbDecoder decoder(cfg, g_arena, kArenaBytes);`

## micro/examples/rp2350/src/main_step7b_framesweep.cc
Depends on: `micro/examples/rp2350/generated/neural_tts_demo_data.h`, `micro/neural-tts/include/neural_tts/pb_decoder.h`
- `LedInit` (function) `micro/examples/rp2350/src/main_step7b_framesweep.cc:25` `bool LedInit()`
- `LedPut` (function) `micro/examples/rp2350/src/main_step7b_framesweep.cc:35` `void LedPut(bool on)`
- `PaintStack` (function) `micro/examples/rp2350/src/main_step7b_framesweep.cc:51` `void PaintStack()`
- `StackFreeBytes` (function) `micro/examples/rp2350/src/main_step7b_framesweep.cc:59` `uint32_t StackFreeBytes()`
- `main` (function) `micro/examples/rp2350/src/main_step7b_framesweep.cc:68` `int main()`
- `decoder` (function) `micro/examples/rp2350/src/main_step7b_framesweep.cc:96` `static neural_tts::PbDecoder decoder(cfg, g_arena, kArenaBytes);`

## micro/examples/rp2350/src/main_step7c_synthonly.cc
Depends on: `micro/neural-tts/include/neural_tts/worldlite_synth.h`
- `LedInit` (function) `micro/examples/rp2350/src/main_step7c_synthonly.cc:29` `bool LedInit()`
- `LedPut` (function) `micro/examples/rp2350/src/main_step7c_synthonly.cc:39` `void LedPut(bool on)`
- `SynthFrame` (function) `micro/examples/rp2350/src/main_step7c_synthonly.cc:48` `void SynthFrame(void* /*user*/, int t, neural_tts::WorldFrame* f)` -- 100-frame voiced spans alternating with 30-frame unvoiced spans.
- `DiscardPcm` (function) `micro/examples/rp2350/src/main_step7c_synthonly.cc:64` `void DiscardPcm(void* user, const int16_t* samples, int n)`
- `PaintStack` (function) `micro/examples/rp2350/src/main_step7c_synthonly.cc:74` `void PaintStack()`
- `StackFreeBytes` (function) `micro/examples/rp2350/src/main_step7c_synthonly.cc:82` `uint32_t StackFreeBytes()`
- `main` (function) `micro/examples/rp2350/src/main_step7c_synthonly.cc:91` `int main()`

## micro/examples/rp2350/src/main_tts.cc
Depends on: `micro/examples/rp2350/src/tts_service.h`
- `main` (function) `micro/examples/rp2350/src/main_tts.cc:64` `int main()`

## micro/examples/rp2350/src/main_wifi.cc
Depends on: `micro/examples/rp2350/src/app_common.h`, `micro/examples/rp2350/src/usb_audio_io.h`, `micro/examples/rp2350/src/wifi_app.h`
- `main` (function) `micro/examples/rp2350/src/main_wifi.cc:17` `int main()`

## micro/examples/rp2350/src/main_wifi_hardware.cc
Depends on: `micro/examples/rp2350/src/app_common.h`, `micro/examples/rp2350/src/wifi_hardware_app.h`
- `main` (function) `micro/examples/rp2350/src/main_wifi_hardware.cc:12` `int main()`

## micro/examples/rp2350/src/op_profiler.cc
Depends on: `micro/examples/rp2350/src/op_profiler.h`
- `BeginEvent` (function) `micro/examples/rp2350/src/op_profiler.cc:11` `uint32_t OpProfiler::BeginEvent(const char* tag)`
- `EndEvent` (function) `micro/examples/rp2350/src/op_profiler.cc:24` `void OpProfiler::EndEvent(uint32_t event_handle)`
- `Report` (function) `micro/examples/rp2350/src/op_profiler.cc:29` `void OpProfiler::Report(const char* label) const`

## micro/examples/rp2350/src/op_profiler.h
Imported by: `micro/examples/rp2350/src/op_profiler.cc`, `micro/examples/rp2350/src/test_app.cc`
- `Reset` (function) `micro/examples/rp2350/src/op_profiler.h:46` `void Reset()` -- Drop all recorded events (call before each Invoke you want to measure in isolation).
- `num_events` (function) `micro/examples/rp2350/src/op_profiler.h:51` `int num_events() const`
- `Report` (function) `micro/examples/rp2350/src/op_profiler.h:55` `void Report(const char* label) const;` -- Print the per-instance and per-tag breakdown over USB stdio.

## micro/examples/rp2350/src/spelling_labels.h
Imported by: `micro/examples/rp2350/src/audio_service.cc`, `micro/examples/rp2350/src/main_i2s_audio_test.cc`, `micro/examples/rp2350/src/wifi_app.cc`
- `SpokenForLabel` (function) `micro/examples/rp2350/src/spelling_labels.h:25` `inline const char* SpokenForLabel(const char* label)` -- Map a class label to the text the TTS should speak.

## micro/examples/rp2350/src/tts_service.cc
Depends on: `micro/examples/rp2350/src/tts_service.h`, `micro/neural-tts/include/neural_tts/neural_tts.h`
- `SetBootReport` (function) `micro/examples/rp2350/src/tts_service.cc:22` `void SetBootReport(const BootReport& report)`
- `ReadLine` (function) `micro/examples/rp2350/src/tts_service.cc:34` `int ReadLine(char* buf, int maxlen)` -- Read one newline-terminated line from USB CDC into `buf` (NUL-terminated), blocking until a non-empty line arrives.
- `EmitToUsb` (function) `micro/examples/rp2350/src/tts_service.cc:55` `void EmitToUsb(void* user, const int16_t* samples, int n)` -- PCM chunks stream straight to the CDC byte pipe as they render.
- `RunTtsService` (function) `micro/examples/rp2350/src/tts_service.cc:63` `void RunTtsService(uint8_t* arena, std::size_t arena_size)`

## micro/examples/rp2350/src/tts_service.h
Imported by: `micro/examples/rp2350/src/main_tts.cc`, `micro/examples/rp2350/src/test_app.cc`, `micro/examples/rp2350/src/tts_service.cc`
- `SetBootReport` (function) `micro/examples/rp2350/src/tts_service.h:39` `void SetBootReport(const BootReport& report);`

## micro/examples/rp2350/src/usb_audio_io.cc
Depends on: `micro/examples/rp2350/src/usb_audio_io.h`
- `ReadByteTimed` (function) `micro/examples/rp2350/src/usb_audio_io.cc:18` `int ReadByteTimed(int timeout_ms)` -- Read one byte, waiting up to ~timeout_ms.
- `ReadHop` (function) `micro/examples/rp2350/src/usb_audio_io.cc:25` `bool UsbAudioInput::ReadHop(int16_t* out, int n)`
- `Drain` (function) `micro/examples/rp2350/src/usb_audio_io.cc:60` `void UsbAudioInput::Drain()`
- `Begin` (function) `micro/examples/rp2350/src/usb_audio_io.cc:67` `void UsbAudioOutput::Begin(int sample_rate, int num_samples, const char* kind)`
- `Write` (function) `micro/examples/rp2350/src/usb_audio_io.cc:72` `void UsbAudioOutput::Write(const int16_t* samples, int n)`
- `End` (function) `micro/examples/rp2350/src/usb_audio_io.cc:76` `void UsbAudioOutput::End()`

## micro/examples/rp2350/src/wifi_app.cc
Depends on: `micro/examples/rp2350/generated/audio_config.h`, `micro/examples/rp2350/generated/classes.h`, `micro/examples/rp2350/src/app_common.h`, `micro/examples/rp2350/src/audio_service.h`, `micro/examples/rp2350/src/spelling_labels.h`, `micro/examples/rp2350/src/wifi_app.h`
- `DigitWord` (function) `micro/examples/rp2350/src/wifi_app.cc:51` `const char* DigitWord(char c)`
- `SymbolChar` (function) `micro/examples/rp2350/src/wifi_app.cc:58` `bool SymbolChar(const char* label, char* out)` -- Symbol class label -> the character it inserts.
- `SymbolWord` (function) `micro/examples/rp2350/src/wifi_app.cc:68` `const char* SymbolWord(char c)` -- Symbol character -> the word the TTS should say for it.
- `Classify` (function) `micro/examples/rp2350/src/wifi_app.cc:79` `Tok Classify(const char* label, char* out_char)`
- `AppendSpokenForChar` (function) `micro/examples/rp2350/src/wifi_app.cc:110` `void AppendSpokenForChar(char* dst, std::size_t cap, char c)` -- Append the spoken word(s) for one credential character to `dst` (a phrase builder), separated by a leading space...
- `SpeakSpelled` (function) `micro/examples/rp2350/src/wifi_app.cc:133` `void SpeakSpelled(const char* prefix, const char* text, AudioOutput& out,
                  Audio...` -- Speak a credential back, spelled out ("see ay tee one"), with an optional prefix ("the name is ...").
- `SpeakName` (function) `micro/examples/rp2350/src/wifi_app.cc:147` `void SpeakName(const char* name, AudioOutput& out, AudioInput& in,
               uint8_t* arena,...` -- Announce a network name: first say it as whole words (letting the TTS g2p pronounce the raw text), then spell it out...
- `SpeakIp` (function) `micro/examples/rp2350/src/wifi_app.cc:156` `void SpeakIp(AudioOutput& out, AudioInput& in, uint8_t* arena,
             std::size_t arena_size)` -- Speak the current STA IPv4 address digit-by-digit ("one nine two dot ...").
- `DoConnect` (function) `micro/examples/rp2350/src/wifi_app.cc:190` `void DoConnect(const char* ssid, const char* pw, AudioOutput& out,
               AudioInput& in,...` -- Join `ssid`/`pw` (WPA2-PSK), waiting for the link and a DHCP lease, pumping the CYW43 poll context throughout.
- `AppendChar` (function) `micro/examples/rp2350/src/wifi_app.cc:222` `std::size_t AppendChar(char* buf, std::size_t len, char c, bool* caps,
                       Aud...` -- Append one recognized credential character to `buf`, applying a pending caps flag, and echo it back.
- `ScanResultCb` (function) `micro/examples/rp2350/src/wifi_app.cc:255` `int ScanResultCb(void* /*env*/, const cyw43_ev_scan_result_t* r)`
- `ScanNetworks` (function) `micro/examples/rp2350/src/wifi_app.cc:275` `void ScanNetworks(AudioInput& in)` -- Scan for nearby networks into g_scan_ssids.
- `LowerAscii` (function) `micro/examples/rp2350/src/wifi_app.cc:300` `char LowerAscii(char c)`
- `HasPrefixCi` (function) `micro/examples/rp2350/src/wifi_app.cc:305` `bool HasPrefixCi(const char* name, const char* prefix, std::size_t plen)` -- Case-insensitive: does `name` begin with the `plen`-char `prefix`?
- `EqualsCi` (function) `micro/examples/rp2350/src/wifi_app.cc:314` `bool EqualsCi(const char* a, const char* b)`
- `CountPrefixMatches` (function) `micro/examples/rp2350/src/wifi_app.cc:323` `int CountPrefixMatches(const char* prefix, int* only_idx)` -- Count scanned SSIDs starting (case-insensitively) with `prefix`; on a single match, write its index to *only_idx.
- `FindExactMatch` (function) `micro/examples/rp2350/src/wifi_app.cc:336` `int FindExactMatch(const char* name)`
- `AnnounceMatch` (function) `micro/examples/rp2350/src/wifi_app.cc:345` `void AnnounceMatch(const char* name, char* ssid, std::size_t* ssid_len,
                   AudioO...` -- Adopt `name` as the chosen SSID (copied into `ssid`), say it back spelled out, and ask for confirmation.
- `RunWifiAppWithIo` (function) `micro/examples/rp2350/src/wifi_app.cc:359` `void RunWifiAppWithIo(AudioInput& in, AudioOutput& out)`

## micro/examples/rp2350/src/wifi_hardware_app.cc
Depends on: `micro/examples/rp2350/generated/audio_config.h`, `micro/examples/rp2350/generated/vad_config.h`, `micro/examples/rp2350/src/i2s_audio_io.h`, `micro/examples/rp2350/src/i2s_audio_out.h`, `micro/examples/rp2350/src/wifi_app.h`, `micro/examples/rp2350/src/wifi_hardware_app.h`
- `RunWifiHardwareApp` (function) `micro/examples/rp2350/src/wifi_hardware_app.cc:13` `void RunWifiHardwareApp()`

## micro/feature-generation/include/feature_generation/feature_generation.h
Imported by: `micro/examples/rp2350/src/audio_service.cc`, `micro/examples/rp2350/src/test_app.cc`, `micro/feature-generation/src/log_mel.cc`, `micro/feature-generation/src/mel_streamer.cc`, `micro/feature-generation/tests/feature_generation_test.cc`
- `HannWindowPeriodic` (function) `micro/feature-generation/include/feature_generation/feature_generation.h:48` `std::vector<float> HannWindowPeriodic(int length);` -- Periodic Hann window of length L (matches torch.hann_window(L, periodic=True)).
- `HzToMelSlaney` (function) `micro/feature-generation/include/feature_generation/feature_generation.h:52` `float HzToMelSlaney(float hz);` -- Slaney's auditory-toolbox mel scale (matches torchaudio _hz_to_mel("slaney")).
- `MelToHzSlaney` (function) `micro/feature-generation/include/feature_generation/feature_generation.h:53` `float MelToHzSlaney(float mel);`
- `MakeMelFilterbank` (function) `micro/feature-generation/include/feature_generation/feature_generation.h:57` `std::vector<float> MakeMelFilterbank(int n_freq, int n_mels, int sample_rate, float f_min, float f_max);` -- Dense (n_mels, n_freq) Slaney-normalised triangular mel filterbank, row-major.
- `Compute` (function) `micro/feature-generation/include/feature_generation/feature_generation.h:117` `void Compute(const float* waveform, std::size_t n_samples, float* out) const;` -- Heap-free streaming compute.
- `n_mels` (function) `micro/feature-generation/include/feature_generation/feature_generation.h:120` `int n_mels() const`
- `target_frames` (function) `micro/feature-generation/include/feature_generation/feature_generation.h:121` `int target_frames() const`
- `n_freq` (function) `micro/feature-generation/include/feature_generation/feature_generation.h:122` `int n_freq() const`
- `params` (function) `micro/feature-generation/include/feature_generation/feature_generation.h:123` `const LogMelParams& params() const`
- `ComputeImpl` (function) `micro/feature-generation/include/feature_generation/feature_generation.h:128` `template <typename SampleT> void ComputeImpl(const SampleT* waveform, std::size_t n_samples, float* out) const;`
- `Reset` (function) `micro/feature-generation/include/feature_generation/feature_generation.h:174` `void Reset();` -- Reset the ring (call at stream start / between independent clips).
- `PushHop` (function) `micro/feature-generation/include/feature_generation/feature_generation.h:178` `void PushHop(const float* hop_samples);` -- Push one hop == n_fft samples (a non-overlapping block).
- `BuildModelInput` (function) `micro/feature-generation/include/feature_generation/feature_generation.h:184` `void BuildModelInput(float* out) const;` -- Write the current window as a row-major (n_mels x window_frames) fp32 tensor into `out` (t=0 oldest .....
- `filled` (function) `micro/feature-generation/include/feature_generation/feature_generation.h:186` `int filled() const`
- `n_mels` (function) `micro/feature-generation/include/feature_generation/feature_generation.h:187` `int n_mels() const`
- `window_frames` (function) `micro/feature-generation/include/feature_generation/feature_generation.h:188` `int window_frames() const`

## micro/feature-generation/scripts/generate_mel_tables.py
- `hann_window_periodic` (function) `micro/feature-generation/scripts/generate_mel_tables.py:32` `def hann_window_periodic(length)`
- `hz_to_mel_slaney` (function) `micro/feature-generation/scripts/generate_mel_tables.py:40` `def hz_to_mel_slaney(hz)`
- `mel_to_hz_slaney` (function) `micro/feature-generation/scripts/generate_mel_tables.py:50` `def mel_to_hz_slaney(mel)`
- `make_csr_filterbank` (function) `micro/feature-generation/scripts/generate_mel_tables.py:60` `def make_csr_filterbank(n_freq, n_mels, sample_rate, f_min, f_max)`
- `fmt_floats` (function) `micro/feature-generation/scripts/generate_mel_tables.py:89` `def fmt_floats(values, per_line)`
- `fmt_ints` (function) `micro/feature-generation/scripts/generate_mel_tables.py:97` `def fmt_ints(values, per_line)`
- `main` (function) `micro/feature-generation/scripts/generate_mel_tables.py:105` `def main()`


Next: [API_p8.md](API_p8.md)
