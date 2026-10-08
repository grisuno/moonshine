# Subsystem: src (page 1 of 2)
Pages: [KB_src.md](KB_src.md), [KB_src_p2.md](KB_src_p2.md)

## micro/examples/rp2350/src/app_common.cc
- Layer: utility
- Language: cc
- Symbols:
  - `LedPulse` (function, line 33) `void LedPulse(unsigned pin, int count, int on_ms, int off_ms)`
  - `BoardInit` (function, line 42) `unsigned BoardInit()`
  - `PrintBootBanner` (function, line 84) `void PrintBootBanner()`
- Depends on: `micro/examples/rp2350/generated/classes.h`, `micro/examples/rp2350/generated/mel_tables.h`, `micro/examples/rp2350/generated/model_data.h`, `micro/examples/rp2350/src/app_common.h`

## micro/examples/rp2350/src/app_common.h
- Doc: Shared boot + state for the RP2350 example, used by both app paths: * echo_app -- the live...
- Layer: utility
- Language: h
- Symbols:
  - `BoardInit` (function, line 48) `unsigned BoardInit();`
  - `PrintBootBanner` (function, line 52) `void PrintBootBanner();`
  - `LedPulse` (function, line 55) `void LedPulse(unsigned pin, int count, int on_ms, int off_ms);`
  - `g_tensor_arena` (variable, line 42) `extern uint8_t g_tensor_arena[kTensorArenaSize];`
  - `g_waveform` (variable, line 43) `extern int16_t g_waveform[kClipNumSamples];`
  - `SPELLING_APP_COMMON_H_` (macro, line 8) `#define SPELLING_APP_COMMON_H_`
  - `SPELLING_TINY_ARENA_BYTES` (macro, line 31) `#define SPELLING_TINY_ARENA_BYTES`
- Depends on: `micro/examples/rp2350/generated/audio_config.h`
- Imported by: `micro/examples/rp2350/src/app_common.cc`, `micro/examples/rp2350/src/echo_app.cc`, `micro/examples/rp2350/src/echo_hardware_app.cc`, `micro/examples/rp2350/src/main_echo_hardware.cc`, `micro/examples/rp2350/src/main_live.cc`, `micro/examples/rp2350/src/main_test.cc`, `micro/examples/rp2350/src/main_wifi.cc`, `micro/examples/rp2350/src/main_wifi_hardware.cc`, `micro/examples/rp2350/src/test_app.cc`, `micro/examples/rp2350/src/wifi_app.cc`

## micro/examples/rp2350/src/audio_io.h
- Doc: Audio input/output abstraction for the live recognition service.
- Layer: utility
- Language: h
- Symbols:
  - `AudioInput` (class, line 19)
  - `AudioOutput` (class, line 35)
  - `SPELLING_AUDIO_IO_H_` (macro, line 12) `#define SPELLING_AUDIO_IO_H_`
- Imported by: `micro/examples/rp2350/src/audio_service.h`, `micro/examples/rp2350/src/i2s_audio_io.h`, `micro/examples/rp2350/src/i2s_audio_out.h`, `micro/examples/rp2350/src/usb_audio_io.h`, `micro/examples/rp2350/src/wifi_app.h`

## micro/examples/rp2350/src/audio_service.cc
- Doc: SPELLING_AUDIO_DIAG gates the verbose recognizer diagnostics: per-hop "listening" heartbeats...
- Layer: business_logic
- Language: cc
- Symbols:
  - `SpeakSink` (struct, line 433)
  - `SetTtsVolume` (function, line 66) `void SetTtsVolume(float volume)`
  - `TtsVolume` (function, line 72) `float TtsVolume()`
  - `RecognizerInit` (function, line 74) `void RecognizerInit(kiss_fftr_state* fft)`
  - `RecognizeOne` (function, line 103) `int RecognizeOne(AudioInput& input, uint8_t* arena, std::size_t arena_size,
                 int1...`
  - `PlayCapturedClip` (function, line 386) `void PlayCapturedClip(const int16_t* window, int num_samples,
                      AudioOutput& ...`
  - `SpeakEmit` (function, line 440) `void SpeakEmit(void* user, const int16_t* samples, int n)`
  - `SkipSpaces` (function, line 464) `const char* SkipSpaces(const char* p)`
  - `PopClause` (function, line 472) `const char* PopClause(const char* text, char* out, size_t cap)`
  - `Speak` (function, line 499) `void Speak(const char* text, AudioOutput& output, AudioInput& input,
           uint8_t* arena, s...`
  - `RunAudioService` (function, line 547) `void RunAudioService(AudioInput& input, AudioOutput& output, uint8_t* arena,
                    ...`
  - `g_neural_tts_pack` (variable, line 53) `extern "C" const uint8_t g_neural_tts_pack[];`
- Depends on: `micro/examples/rp2350/generated/audio_config.h`, `micro/examples/rp2350/generated/classes.h`, `micro/examples/rp2350/generated/mel_tables.h`, `micro/examples/rp2350/generated/model_data.h`, `micro/examples/rp2350/generated/vad_config.h`, `micro/examples/rp2350/generated/vad_mel_tables.h`, `micro/examples/rp2350/generated/vad_model_data.h`, `micro/examples/rp2350/src/audio_service.h`, `micro/examples/rp2350/src/spelling_labels.h`, `micro/feature-generation/include/feature_generation/feature_generation.h`, `micro/neural-tts/include/neural_tts/neural_tts.h`, `micro/stt/include/stt/stt.h`, `micro/vad/include/vad/vad.h`

## micro/examples/rp2350/src/audio_service.h
- Doc: Live USB audio service: turns the laptop into the RP2350's mic + speaker.
- Layer: business_logic
- Language: h
- Symbols:
  - `kiss_fftr_state` (struct, line 26)
  - `RecognizerInit` (function, line 38) `void RecognizerInit(kiss_fftr_state* fft);`
  - `RecognizeOne` (function, line 46) `int RecognizeOne(AudioInput& input, uint8_t* arena, std::size_t arena_size, int16_t* window, int window_samples...`
  - `SetTtsVolume` (function, line 61) `void SetTtsVolume(float volume);`
  - `TtsVolume` (function, line 62) `float TtsVolume();`
  - `Speak` (function, line 68) `void Speak(const char* text, AudioOutput& output, AudioInput& input, uint8_t* arena, std::size_t arena_size);`
  - `RunAudioService` (function, line 77) `void RunAudioService(AudioInput& input, AudioOutput& output, uint8_t* arena, std::size_t arena_size...`
  - `SPELLING_AUDIO_SERVICE_H_` (macro, line 19) `#define SPELLING_AUDIO_SERVICE_H_`
- Depends on: `micro/examples/rp2350/src/audio_io.h`
- Imported by: `micro/examples/rp2350/src/audio_service.cc`, `micro/examples/rp2350/src/echo_app.cc`, `micro/examples/rp2350/src/echo_hardware_app.cc`, `micro/examples/rp2350/src/wifi_app.cc`

## micro/examples/rp2350/src/echo_app.cc
- Layer: utility
- Language: cc
- Symbols:
  - `RunEchoApp` (function, line 28) `void RunEchoApp()`
- Depends on: `micro/examples/rp2350/generated/audio_config.h`, `micro/examples/rp2350/generated/mel_tables.h`, `micro/examples/rp2350/generated/vad_config.h`, `micro/examples/rp2350/generated/vad_mel_tables.h`, `micro/examples/rp2350/src/app_common.h`, `micro/examples/rp2350/src/audio_service.h`, `micro/examples/rp2350/src/echo_app.h`, `micro/examples/rp2350/src/usb_audio_io.h`

## micro/examples/rp2350/src/echo_app.h
- Doc: The default app path: the live mic/speaker recognition service.
- Layer: utility
- Language: h
- Symbols:
  - `SPELLING_ECHO_APP_H_` (macro, line 8) `#define SPELLING_ECHO_APP_H_`
- Imported by: `micro/examples/rp2350/src/echo_app.cc`, `micro/examples/rp2350/src/main_live.cc`

## micro/examples/rp2350/src/echo_hardware_app.cc
- Layer: utility
- Language: cc
- Symbols:
  - `RunEchoHardwareApp` (function, line 24) `void RunEchoHardwareApp()`
- Depends on: `micro/examples/rp2350/generated/audio_config.h`, `micro/examples/rp2350/generated/mel_tables.h`, `micro/examples/rp2350/generated/vad_config.h`, `micro/examples/rp2350/generated/vad_mel_tables.h`, `micro/examples/rp2350/src/app_common.h`, `micro/examples/rp2350/src/audio_service.h`, `micro/examples/rp2350/src/echo_hardware_app.h`, `micro/examples/rp2350/src/i2s_audio_io.h`, `micro/examples/rp2350/src/i2s_audio_out.h`

## micro/examples/rp2350/src/echo_hardware_app.h
- Doc: On-board hardware echo service (I2S mic + I2S amp).
- Layer: utility
- Language: h
- Symbols:
  - `SPELLING_ECHO_HARDWARE_APP_H_` (macro, line 9) `#define SPELLING_ECHO_HARDWARE_APP_H_`
- Imported by: `micro/examples/rp2350/src/echo_hardware_app.cc`, `micro/examples/rp2350/src/main_echo_hardware.cc`

## micro/examples/rp2350/src/i2s_audio_io.cc
- Doc: CaptureWriteIdx: Current DMA write position as a ring word index (0..kRingWords-1).
- Layer: utility
- Language: cc
- Symbols:
  - `CaptureWriteIdx` (function, line 49) `inline unsigned CaptureWriteIdx()`
  - `StartCaptureDma` (function, line 55) `void StartCaptureDma()`
  - `I2sAudioInput` (function, line 76) `I2sAudioInput::I2sAudioInput(int sample_rate)
    : sm_(0), dc_blocker_(sample_rate)`
  - `ReadHop` (function, line 96) `bool I2sAudioInput::ReadHop(int16_t* out, int n)`
  - `Drain` (function, line 114) `void I2sAudioInput::Drain()`
- Depends on: `micro/examples/rp2350/src/i2s_audio_io.h`, `micro/examples/rp2350/src/i2s_mic_process.h`

## micro/examples/rp2350/src/i2s_audio_io.h
- Doc: I2S microphone input for the on-board echo service (SPH0645 / Adafruit 3421).
- Layer: utility
- Language: h
- Symbols:
  - `I2sAudioInput` (class, line 20)
  - `SPELLING_I2S_AUDIO_IO_H_` (macro, line 13) `#define SPELLING_I2S_AUDIO_IO_H_`
- Depends on: `micro/examples/rp2350/src/audio_io.h`, `micro/examples/rp2350/src/i2s_mic_process.h`
- Imported by: `micro/examples/rp2350/src/echo_hardware_app.cc`, `micro/examples/rp2350/src/i2s_audio_io.cc`, `micro/examples/rp2350/src/main_audio_loopback_test.cc`, `micro/examples/rp2350/src/wifi_hardware_app.cc`

## micro/examples/rp2350/src/i2s_audio_out.cc
- Doc: StereoFrame: Pack one mono int16 sample into a 32-bit stereo I2S frame: MSB-first shift means...
- Layer: utility
- Language: cc
- Symbols:
  - `StereoFrame` (function, line 20) `inline uint32_t StereoFrame(int16_t s)`
  - `PeakNormalizeGain` (function, line 43) `float PeakNormalizeGain(const int16_t* samples, int n, float target,
                        floa...`
  - `PeakNormalizeGain` (function, line 58) `float PeakNormalizeGain(const float* samples, int n, float target,
                        float ...`
  - `I2sAudioOutput` (function, line 72) `I2sAudioOutput::I2sAudioOutput(unsigned data_pin, unsigned clock_base,
                          ...`
  - `ReadIdx` (function, line 101) `unsigned I2sAudioOutput::ReadIdx() const`
  - `Used` (function, line 107) `unsigned I2sAudioOutput::Used() const`
  - `StartDma` (function, line 111) `void I2sAudioOutput::StartDma()`
  - `PushFrame` (function, line 118) `void I2sAudioOutput::PushFrame(uint32_t frame)`
  - `ApplyClockDiv` (function, line 131) `void I2sAudioOutput::ApplyClockDiv()`
  - `Begin` (function, line 140) `void I2sAudioOutput::Begin(int sample_rate, int num_samples, const char* kind)`
  - `Write` (function, line 158) `void I2sAudioOutput::Write(const int16_t* samples, int n)`
  - `End` (function, line 167) `void I2sAudioOutput::End()`
- Depends on: `micro/examples/rp2350/src/i2s_audio_out.h`

## micro/examples/rp2350/src/i2s_audio_out.h
- Doc: I2S speaker output for the on-board echo service (MAX98357A / Adafruit 3006).
- Layer: utility
- Language: h
- Symbols:
  - `I2sAudioOutput` (class, line 42)
  - `SetGain` (function, line 56) `void SetGain(float gain)`
  - `PeakNormalizeGain` (function, line 37) `float PeakNormalizeGain(const int16_t* samples, int n, float target = 0.9f, float max_gain = 32.0f);`
  - `ApplyClockDiv` (function, line 60) `void ApplyClockDiv();`
  - `PushFrame` (function, line 63) `void PushFrame(uint32_t frame);`
  - `StartDma` (function, line 66) `void StartDma();`
  - `ReadIdx` (function, line 68) `unsigned ReadIdx() const;`
  - `Used` (function, line 69) `unsigned Used() const;`
  - `SPELLING_I2S_AUDIO_OUT_H_` (macro, line 23) `#define SPELLING_I2S_AUDIO_OUT_H_`
- Depends on: `micro/examples/rp2350/src/audio_io.h`
- Imported by: `micro/examples/rp2350/src/echo_hardware_app.cc`, `micro/examples/rp2350/src/i2s_audio_out.cc`, `micro/examples/rp2350/src/main_audio_loopback_test.cc`, `micro/examples/rp2350/src/main_i2s_audio_test.cc`, `micro/examples/rp2350/src/main_i2s_relay.cc`, `micro/examples/rp2350/src/wifi_hardware_app.cc`

## micro/examples/rp2350/src/i2s_mic_process.cc
- Layer: business_logic
- Language: cc
- Symbols:
  - `I2sRawToInt32` (function, line 8) `int32_t I2sRawToInt32(uint32_t raw)`
  - `I2sRawToInt16` (function, line 12) `int16_t I2sRawToInt16(uint32_t raw)`
  - `I2sDcBlocker` (function, line 18) `I2sDcBlocker::I2sDcBlocker(int sample_rate_hz, float cutoff_hz)
    : r_(std::exp(-2.f * 3.141592...`
  - `Process` (function, line 22) `int16_t I2sDcBlocker::Process(int16_t x)`
  - `Reset` (function, line 32) `void I2sDcBlocker::Reset()`
  - `I2sRemoveBufferDc` (function, line 37) `void I2sRemoveBufferDc(int16_t* samples, int n)`
- Depends on: `micro/examples/rp2350/src/i2s_mic_process.h`

## micro/examples/rp2350/src/i2s_mic_process.h
- Doc: SPH0645 / Adafruit 3421 I2S sample conversion and DC removal.
- Layer: business_logic
- Language: h
- Symbols:
  - `I2sDcBlocker` (class, line 20)
  - `I2sRawToInt32` (function, line 16) `int32_t I2sRawToInt32(uint32_t raw);`
  - `I2sRawToInt16` (function, line 17) `int16_t I2sRawToInt16(uint32_t raw);`
  - `Process` (function, line 24) `int16_t Process(int16_t x);`
  - `Reset` (function, line 25) `void Reset();`
  - `I2sRemoveBufferDc` (function, line 34) `void I2sRemoveBufferDc(int16_t* samples, int n);`
  - `SPELLING_I2S_MIC_PROCESS_H_` (macro, line 7) `#define SPELLING_I2S_MIC_PROCESS_H_`
- Imported by: `micro/examples/rp2350/src/i2s_audio_io.cc`, `micro/examples/rp2350/src/i2s_audio_io.h`, `micro/examples/rp2350/src/i2s_mic_process.cc`, `micro/examples/rp2350/src/main_i2s_mic_test.cc`

## micro/examples/rp2350/src/main_audio_loopback_test.cc
- Doc: Standalone mic -> speaker loopback test (the `moonshine_micro_audio_loopback_test` target).
- Layer: testing
- Language: cc
- Symbols:
  - `Record` (function, line 27) `void Record(spelling::I2sAudioInput& input)`
  - `Play` (function, line 40) `void Play(spelling::I2sAudioOutput& output)`
  - `main` (function, line 61) `int main()`
- Depends on: `micro/examples/rp2350/src/i2s_audio_io.h`, `micro/examples/rp2350/src/i2s_audio_out.h`

## micro/examples/rp2350/src/main_echo_hardware.cc
- Doc: Entry point for the on-board hardware echo service (the `moonshine_micro_echo_hardware` target).
- Layer: utility
- Language: cc
- Symbols:
  - `main` (function, line 10) `int main()`
- Depends on: `micro/examples/rp2350/src/app_common.h`, `micro/examples/rp2350/src/echo_hardware_app.h`

## micro/examples/rp2350/src/main_i2s_audio_test.cc
- Doc: Standalone speaker / audio-output bring-up test (the `moonshine_micro_i2s_audio_test` target).
- Layer: testing
- Language: cc
- Symbols:
  - `TtsSink` (struct, line 167)
  - `BuildSineTable` (function, line 97) `void BuildSineTable()`
  - `PlayTone` (function, line 107) `void PlayTone(spelling::I2sAudioOutput& out, double freq, int ms)`
  - `PlaySweep` (function, line 135) `void PlaySweep(spelling::I2sAudioOutput& out, double f0, double f1, int ms)`
  - `TtsEmit` (function, line 172) `void TtsEmit(void* user, const int16_t* samples, int n)`
  - `SpeakText` (function, line 190) `void SpeakText(spelling::I2sAudioOutput& out, neural_tts::NeuralTts& tts,
               const ch...`
  - `main` (function, line 224) `int main()`
  - `g_neural_tts_pack` (variable, line 42) `extern "C" const uint8_t g_neural_tts_pack[];`
  - `v` (variable, line 51) `extern "C" void tts_checkpoint(uint32_t v) { watchdog_hw->scratch[0] = v;`
  - `v` (variable, line 55) `extern "C" void tts_checkpoint2(uint32_t v) { watchdog_hw->scratch[1] = v;`
  - `frame` (variable, line 59) `extern "C" void HardFaultC(uint32_t* frame) { watchdog_hw->scratch[3] = frame[6];`
- Depends on: `micro/examples/rp2350/generated/speaker_test_clips.h`, `micro/examples/rp2350/src/i2s_audio_out.h`, `micro/examples/rp2350/src/spelling_labels.h`, `micro/neural-tts/include/neural_tts/neural_tts.h`

## micro/examples/rp2350/src/main_i2s_mic_test.cc
- Doc: Standalone I2S microphone bring-up test (the `moonshine_micro_i2s_mic_test` target).
- Layer: testing
- Language: cc
- Symbols:
  - `ChannelStats` (struct, line 51)
  - `Add` (function, line 60) `void Add(int32_t s, uint32_t raw)`
  - `DrainUsbInput` (function, line 71) `void DrainUsbInput()`
  - `DrawBar` (function, line 76) `void DrawBar(double level, double full_scale)`
  - `ChannelRms` (function, line 86) `double ChannelRms(const ChannelStats& st)`
  - `ReportChannel` (function, line 93) `void ReportChannel(const char* name, const ChannelStats& st, bool active)`
  - `RecordWindow` (function, line 113) `void RecordWindow(PIO pio, uint sm, ChannelStats* a, ChannelStats* b,
                  spelling:...`
  - `StreamToHost` (function, line 132) `void StreamToHost(const int16_t* samples, int n)`
  - `WaitForClipAck` (function, line 144) `bool WaitForClipAck(int timeout_ms)`
  - `main` (function, line 168) `int main()`
- Depends on: `micro/examples/rp2350/src/i2s_mic_process.h`, `micro/examples/rp2350/src/usb_audio_io.h`

## micro/examples/rp2350/src/main_i2s_relay.cc
- Doc: Dumb PCM -> I2S relay (the `moonshine_micro_i2s_relay` target).
- Layer: utility
- Language: cc
- Symbols:
  - `ReadLine` (function, line 71) `int ReadLine(char* buf, int maxlen)`
  - `ReadByteTimed` (function, line 88) `int ReadByteTimed(int timeout_ms)`
  - `ReadHop` (function, line 98) `int ReadHop(int16_t* out, int n)`
  - `PlayStream` (function, line 140) `int PlayStream(spelling::I2sAudioOutput& out, int rate, int total)`
  - `main` (function, line 182) `int main()`
  - `frame` (variable, line 165) `extern "C" void HardFaultC(uint32_t* frame) { watchdog_hw->scratch[3] = frame[6];`
- Depends on: `micro/examples/rp2350/src/i2s_audio_out.h`

## micro/examples/rp2350/src/main_live.cc
- Doc: Entry point for the live mic/speaker echo service (the `moonshine_micro_echo` target).
- Layer: utility
- Language: cc
- Symbols:
  - `main` (function, line 11) `int main()`
- Depends on: `micro/examples/rp2350/src/app_common.h`, `micro/examples/rp2350/src/echo_app.h`

## micro/examples/rp2350/src/main_step1_blinky.cc
- Doc: Step 1 of the minimal bring-up ladder: blink the LED, nothing else.
- Layer: utility
- Language: cc
- Symbols:
  - `main` (function, line 11) `int main()`

## micro/examples/rp2350/src/main_step1_blinky_w.cc
- Doc: Step 1b of the minimal bring-up ladder: blink the LED on a Pico 2 W.
- Layer: utility
- Language: cc
- Symbols:
  - `main` (function, line 10) `int main()`

## micro/examples/rp2350/src/main_step2_printf.cc
- Doc: Step 2 of the minimal bring-up ladder: blink the LED AND print one line per second over USB CDC.
- Layer: utility
- Language: cc
- Symbols:
  - `LedInit` (function, line 17) `bool LedInit()`
  - `LedPut` (function, line 27) `void LedPut(bool on)`
  - `main` (function, line 37) `int main()`

## micro/examples/rp2350/src/main_step3_fft.cc
- Doc: Step 3 of the minimal bring-up ladder: step 2 + heap probe + one kissfft plan + one 1024-point...
- Layer: utility
- Language: cc
- Symbols:
  - `LedInit` (function, line 19) `bool LedInit()`
  - `LedPut` (function, line 29) `void LedPut(bool on)`
  - `main` (function, line 43) `int main()`

## micro/examples/rp2350/src/main_step5_synth.cc
- Doc: Step 5 of the minimal bring-up ladder: step 4 + the real WorldLiteSynth (constructor allocates...
- Layer: utility
- Language: cc
- Symbols:
  - `LedInit` (function, line 23) `bool LedInit()`
  - `LedPut` (function, line 33) `void LedPut(bool on)`
  - `main` (function, line 43) `int main()`
  - `0` (variable, line 17) `extern "C" void tts_checkpoint(uint32_t) {} extern "C" void tts_checkpoint2(uint32_t) {} extern "C" void...`
- Depends on: `micro/neural-tts/include/neural_tts/worldlite_synth.h`

## micro/examples/rp2350/src/main_step6_decoder.cc
- Doc: Step 6 of the minimal bring-up ladder: step 5 + the TFLM decoder.
- Layer: utility
- Language: cc
- Symbols:
  - `LedInit` (function, line 28) `bool LedInit()`
  - `LedPut` (function, line 38) `void LedPut(bool on)`
  - `main` (function, line 51) `int main()`
  - `decoder` (function, line 97) `static neural_tts::PbDecoder decoder(cfg, g_arena, kArenaBytes);`
  - `0` (variable, line 22) `extern "C" void tts_checkpoint(uint32_t) {} extern "C" void tts_checkpoint2(uint32_t) {} extern "C" void...`
  - `STEP6_SYS_KHZ` (macro, line 56) `#define STEP6_SYS_KHZ`
  - `STEP6_FLASH_DIV` (macro, line 59) `#define STEP6_FLASH_DIV`
- Depends on: `micro/examples/rp2350/generated/neural_tts_demo_data.h`, `micro/neural-tts/include/neural_tts/pb_decoder.h`, `micro/neural-tts/include/neural_tts/worldlite_synth.h`

## micro/examples/rp2350/src/main_step7_synthesize.cc
- Doc: Step 7 of the minimal bring-up ladder: step 6 + full WORLD-lite synthesis of each demo utterance...
- Layer: utility
- Language: cc
- Symbols:
  - `LedInit` (function, line 35) `bool LedInit()`
  - `LedPut` (function, line 45) `void LedPut(bool on)`
  - `DiscardPcm` (function, line 56) `void DiscardPcm(void* user, const int16_t* samples, int n)`
  - `PaintStack` (function, line 66) `void PaintStack()`
  - `StackFreeBytes` (function, line 74) `uint32_t StackFreeBytes()`
  - `main` (function, line 83) `int main()`
  - `decoder` (function, line 122) `static neural_tts::PbDecoder decoder(cfg, g_arena, kArenaBytes);`
  - `v` (variable, line 24) `extern "C" void tts_checkpoint(uint32_t v) { watchdog_hw->scratch[4] = v;`
  - `v` (variable, line 28) `extern "C" void tts_checkpoint2(uint32_t v) { watchdog_hw->scratch[5] = v;`
  - `__StackBottom` (variable, line 63) `extern "C" char __StackBottom;`
- Depends on: `micro/examples/rp2350/generated/neural_tts_demo_data.h`, `micro/neural-tts/include/neural_tts/pb_decoder.h`, `micro/neural-tts/include/neural_tts/worldlite_synth.h`

## micro/examples/rp2350/src/main_step7b_framesweep.cc
- Doc: Step 7b of the minimal bring-up ladder: step 6 + sweep GetFrame through EVERY frame of each...
- Layer: utility
- Language: cc
- Symbols:
  - `LedInit` (function, line 25) `bool LedInit()`
  - `LedPut` (function, line 35) `void LedPut(bool on)`
  - `PaintStack` (function, line 51) `void PaintStack()`
  - `StackFreeBytes` (function, line 59) `uint32_t StackFreeBytes()`
  - `main` (function, line 68) `int main()`
  - `decoder` (function, line 96) `static neural_tts::PbDecoder decoder(cfg, g_arena, kArenaBytes);`
  - `0` (variable, line 19) `extern "C" void tts_checkpoint(uint32_t) {} extern "C" void tts_checkpoint2(uint32_t) {} extern "C" void...`
  - `__StackBottom` (variable, line 48) `extern "C" char __StackBottom;`
- Depends on: `micro/examples/rp2350/generated/neural_tts_demo_data.h`, `micro/neural-tts/include/neural_tts/pb_decoder.h`

## micro/examples/rp2350/src/main_step7c_synthonly.cc
- Doc: Step 7c of the minimal bring-up ladder: the mirror image of step 7b.
- Layer: utility
- Language: cc
- Symbols:
  - `LedInit` (function, line 29) `bool LedInit()`
  - `LedPut` (function, line 39) `void LedPut(bool on)`
  - `SynthFrame` (function, line 48) `void SynthFrame(void* /*user*/, int t, neural_tts::WorldFrame* f)`
  - `DiscardPcm` (function, line 64) `void DiscardPcm(void* user, const int16_t* samples, int n)`
  - `PaintStack` (function, line 74) `void PaintStack()`
  - `StackFreeBytes` (function, line 82) `uint32_t StackFreeBytes()`
  - `main` (function, line 91) `int main()`
  - `0` (variable, line 23) `extern "C" void tts_checkpoint(uint32_t) {} extern "C" void tts_checkpoint2(uint32_t) {} extern "C" void...`
  - `__StackBottom` (variable, line 71) `extern "C" char __StackBottom;`
- Depends on: `micro/neural-tts/include/neural_tts/worldlite_synth.h`

## micro/examples/rp2350/src/main_test.cc
- Doc: Entry point for the embedded-clip accuracy sweep (the `moonshine_micro_echo_test` target).
- Layer: testing
- Language: cc
- Symbols:
  - `main` (function, line 12) `int main()`
- Depends on: `micro/examples/rp2350/src/app_common.h`, `micro/examples/rp2350/src/test_app.h`

## micro/examples/rp2350/src/main_tflm_invoke_test.cc
- Doc: Rung-2 bring-up firmware: banner + TFLM interpreter init + ONE Invoke() of the s16x8 neural-TTS...
- Layer: testing
- Language: cc
- Symbols:
  - `BeginEvent` (function, line 68) `uint32_t BeginEvent(const char* tag) override`
  - `EndEvent` (function, line 73) `void EndEvent(uint32_t handle) override`
  - `Reset` (function, line 76) `void Reset()`
  - `Report` (function, line 77) `void Report()`
  - `FeedWatchdog` (function, line 100) `bool FeedWatchdog(repeating_timer_t*)`
  - `main` (function, line 108) `int main()`
  - `interp` (function, line 158) `static tflite::MicroInterpreter interp(model, resolver, g_arena, kArenaBytes, /*resource_variables=*/nullptr...`
  - `0xFA17FA17u` (variable, line 33) `extern "C" void isr_hardfault_c(uint32_t* sp) { watchdog_hw->scratch[4] = 0xFA17FA17u;`
  - `__end__` (variable, line 111) `extern char __end__;`
  - `TRACE` (macro, line 53) `#define TRACE(...)`
  - `INVOKE_TEST_SYS_KHZ` (macro, line 117) `#define INVOKE_TEST_SYS_KHZ`
- Depends on: `micro/examples/rp2350/generated/neural_tts_demo_data.h`

## micro/examples/rp2350/src/main_tts.cc
- Doc: Entry point for the standalone TTS service (`moonshine_micro_tts`).
- Layer: utility
- Language: cc
- Symbols:
  - `main` (function, line 64) `int main()`
  - `v` (variable, line 37) `extern "C" void tts_checkpoint(uint32_t v) { watchdog_hw->scratch[0] = v;`
  - `v` (variable, line 41) `extern "C" void tts_checkpoint2(uint32_t v) { watchdog_hw->scratch[1] = v;`
  - `frame` (variable, line 49) `extern "C" void HardFaultC(uint32_t* frame) { watchdog_hw->scratch[3] = frame[6];`
- Depends on: `micro/examples/rp2350/src/tts_service.h`

## micro/examples/rp2350/src/main_tts_ladder_test.cc
- Doc: Incremental bring-up ladder for the neural-TTS stack.
- Layer: testing
- Language: cc
- Symbols:
  - `EmitPcm` (function, line 90) `void EmitPcm(void* user, const int16_t* samples, int n)`
  - `main` (function, line 104) `int main()`
  - `decoder` (function, line 186) `static neural_tts::PbDecoder decoder(cfg, g_arena, kArenaBytes);`
  - `0xFA17FA17u` (variable, line 47) `extern "C" void isr_hardfault_c(uint32_t* sp) { watchdog_hw->scratch[4] = 0xFA17FA17u;`
  - `__end__` (variable, line 106) `extern char __end__;`
  - `TTS_LADDER_STAGE` (macro, line 27) `#define TTS_LADDER_STAGE`
  - `TTS_LADDER_EXECUTE` (macro, line 33) `#define TTS_LADDER_EXECUTE`
  - `TRACE` (macro, line 77) `#define TRACE(...)`
- Depends on: `micro/examples/rp2350/generated/neural_tts_demo_data.h`, `micro/neural-tts/include/neural_tts/pb_decoder.h`, `micro/neural-tts/include/neural_tts/worldlite_synth.h`

## micro/examples/rp2350/src/main_usb_banner_test.cc
- Doc: Minimal USB CDC stdio soak test (the `moonshine_micro_usb_banner_test` target).
- Layer: testing
- Language: cc
- Symbols:
  - `main` (function, line 29) `int main()`
  - `sp` (variable, line 18) `extern "C" void isr_hardfault(void) { uint32_t* sp;`

## micro/examples/rp2350/src/main_wifi.cc
- Doc: Entry point for the voice-driven WiFi setup app (the `moonshine_micro_echo_wifi` target; needs a...
- Layer: utility
- Language: cc
- Symbols:
  - `main` (function, line 17) `int main()`
- Depends on: `micro/examples/rp2350/src/app_common.h`, `micro/examples/rp2350/src/usb_audio_io.h`, `micro/examples/rp2350/src/wifi_app.h`

## micro/examples/rp2350/src/main_wifi_hardware.cc
- Doc: Entry point for the voice-driven WiFi setup app on the on-board hardware audio I/O (the...
- Layer: utility
- Language: cc
- Symbols:
  - `main` (function, line 12) `int main()`
- Depends on: `micro/examples/rp2350/src/app_common.h`, `micro/examples/rp2350/src/wifi_hardware_app.h`

## micro/examples/rp2350/src/op_profiler.cc
- Doc: See op_profiler.h for the rationale (why not tflite::MicroProfiler).
- Layer: utility
- Language: cc
- Symbols:
  - `TagAgg` (struct, line 44)
  - `BeginEvent` (function, line 11) `uint32_t OpProfiler::BeginEvent(const char* tag)`
  - `EndEvent` (function, line 24) `void OpProfiler::EndEvent(uint32_t event_handle)`
  - `Report` (function, line 29) `void OpProfiler::Report(const char* label) const`
- Depends on: `micro/examples/rp2350/src/op_profiler.h`

## micro/examples/rp2350/src/op_profiler.h
- Doc: Lightweight per-op profiler for the moonshine-micro SpellingCNN build.
- Layer: utility
- Language: h
- Symbols:
  - `Reset` (function, line 46) `void Reset()`
  - `num_events` (function, line 51) `int num_events() const`
  - `Report` (function, line 55) `void Report(const char* label) const;`
  - `SPELLING_OP_PROFILER_H_` (macro, line 26) `#define SPELLING_OP_PROFILER_H_`
- Imported by: `micro/examples/rp2350/src/op_profiler.cc`, `micro/examples/rp2350/src/test_app.cc`

## micro/examples/rp2350/src/spelling_labels.h
- Doc: Spoken "sound-alike" word for each recognized class label, so the readback TTS says "bee" for...
- Layer: utility
- Language: h
- Symbols:
  - `SpokenForLabel` (function, line 25) `inline const char* SpokenForLabel(const char* label)`
  - `SPELLING_SPELLING_LABELS_H_` (macro, line 19) `#define SPELLING_SPELLING_LABELS_H_`
- Imported by: `micro/examples/rp2350/src/audio_service.cc`, `micro/examples/rp2350/src/main_i2s_audio_test.cc`, `micro/examples/rp2350/src/wifi_app.cc`

## micro/examples/rp2350/src/test_app.cc
- Doc: RunVadDemo: Streaming VAD demo over the embedded clips (each treated as a 1 s stream): one FFT...
- Layer: testing
- Language: cc
- Symbols:
  - `RunVadDemo` (function, line 66) `void RunVadDemo(uint8_t* arena, std::size_t arena_size, kiss_fftr_state* fft)`
  - `RunTestApp` (function, line 147) `void RunTestApp(unsigned led_pin)`
- Depends on: `micro/examples/rp2350/generated/audio_config.h`, `micro/examples/rp2350/generated/classes.h`, `micro/examples/rp2350/generated/mel_tables.h`, `micro/examples/rp2350/generated/model_data.h`, `micro/examples/rp2350/generated/test_clips.h`, `micro/examples/rp2350/generated/vad_config.h`, `micro/examples/rp2350/generated/vad_mel_tables.h`, `micro/examples/rp2350/generated/vad_model_data.h`, `micro/examples/rp2350/src/app_common.h`, `micro/examples/rp2350/src/op_profiler.h`, `micro/examples/rp2350/src/test_app.h`, `micro/examples/rp2350/src/tts_service.h`, `micro/feature-generation/include/feature_generation/feature_generation.h`, `micro/stt/include/stt/stt.h`, `micro/vad/include/vad/vad.h`


Next: [KB_src_p2.md](KB_src_p2.md)
