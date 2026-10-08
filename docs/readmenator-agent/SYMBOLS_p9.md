# Symbols (page 9 of 12)
Previous: [SYMBOLS_p8.md](SYMBOLS_p8.md)

| Symbol | Kind | File:Line | Signature |
|--------|------|-----------|-----------|
| `I2sRemoveBufferDc` | function | `micro/examples/rp2350/src/i2s_mic_process.h:34` | `void I2sRemoveBufferDc(int16_t* samples, int n);` |
| `Process` | function | `micro/examples/rp2350/src/i2s_mic_process.h:24` | `int16_t Process(int16_t x);` |
| `Reset` | function | `micro/examples/rp2350/src/i2s_mic_process.h:25` | `void Reset();` |
| `SPELLING_I2S_MIC_PROCESS_H_` | macro | `micro/examples/rp2350/src/i2s_mic_process.h:7` | `#define SPELLING_I2S_MIC_PROCESS_H_` |
| `Play` | function | `micro/examples/rp2350/src/main_audio_loopback_test.cc:40` | `void Play(spelling::I2sAudioOutput& output)` |
| `Record` | function | `micro/examples/rp2350/src/main_audio_loopback_test.cc:27` | `void Record(spelling::I2sAudioInput& input)` |
| `main` | function | `micro/examples/rp2350/src/main_audio_loopback_test.cc:61` | `int main()` |
| `main` | function | `micro/examples/rp2350/src/main_echo_hardware.cc:10` | `int main()` |
| `BuildSineTable` | function | `micro/examples/rp2350/src/main_i2s_audio_test.cc:97` | `void BuildSineTable()` |
| `PlaySweep` | function | `micro/examples/rp2350/src/main_i2s_audio_test.cc:135` | `void PlaySweep(spelling::I2sAudioOutput& out, double f0, double f1, int ms)` |
| `PlayTone` | function | `micro/examples/rp2350/src/main_i2s_audio_test.cc:107` | `void PlayTone(spelling::I2sAudioOutput& out, double freq, int ms)` |
| `SpeakText` | function | `micro/examples/rp2350/src/main_i2s_audio_test.cc:190` | `void SpeakText(spelling::I2sAudioOutput& out, neural_tts::NeuralTts& tts,                const ch...` |
| `TtsEmit` | function | `micro/examples/rp2350/src/main_i2s_audio_test.cc:172` | `void TtsEmit(void* user, const int16_t* samples, int n)` |
| `TtsSink` | struct | `micro/examples/rp2350/src/main_i2s_audio_test.cc:167` | `` |
| `frame` | variable | `micro/examples/rp2350/src/main_i2s_audio_test.cc:59` | `extern "C" void HardFaultC(uint32_t* frame) { watchdog_hw->scratch[3] = frame[6];` |
| `g_neural_tts_pack` | variable | `micro/examples/rp2350/src/main_i2s_audio_test.cc:42` | `extern "C" const uint8_t g_neural_tts_pack[];` |
| `main` | function | `micro/examples/rp2350/src/main_i2s_audio_test.cc:224` | `int main()` |
| `v` | variable | `micro/examples/rp2350/src/main_i2s_audio_test.cc:51` | `extern "C" void tts_checkpoint(uint32_t v) { watchdog_hw->scratch[0] = v;` |
| `v` | variable | `micro/examples/rp2350/src/main_i2s_audio_test.cc:55` | `extern "C" void tts_checkpoint2(uint32_t v) { watchdog_hw->scratch[1] = v;` |
| `Add` | function | `micro/examples/rp2350/src/main_i2s_mic_test.cc:60` | `void Add(int32_t s, uint32_t raw)` |
| `ChannelRms` | function | `micro/examples/rp2350/src/main_i2s_mic_test.cc:86` | `double ChannelRms(const ChannelStats& st)` |
| `ChannelStats` | struct | `micro/examples/rp2350/src/main_i2s_mic_test.cc:51` | `` |
| `DrainUsbInput` | function | `micro/examples/rp2350/src/main_i2s_mic_test.cc:71` | `void DrainUsbInput()` |
| `DrawBar` | function | `micro/examples/rp2350/src/main_i2s_mic_test.cc:76` | `void DrawBar(double level, double full_scale)` |
| `RecordWindow` | function | `micro/examples/rp2350/src/main_i2s_mic_test.cc:113` | `void RecordWindow(PIO pio, uint sm, ChannelStats* a, ChannelStats* b,                   spelling:...` |
| `ReportChannel` | function | `micro/examples/rp2350/src/main_i2s_mic_test.cc:93` | `void ReportChannel(const char* name, const ChannelStats& st, bool active)` |
| `StreamToHost` | function | `micro/examples/rp2350/src/main_i2s_mic_test.cc:132` | `void StreamToHost(const int16_t* samples, int n)` |
| `WaitForClipAck` | function | `micro/examples/rp2350/src/main_i2s_mic_test.cc:144` | `bool WaitForClipAck(int timeout_ms)` |
| `main` | function | `micro/examples/rp2350/src/main_i2s_mic_test.cc:168` | `int main()` |
| `PlayStream` | function | `micro/examples/rp2350/src/main_i2s_relay.cc:140` | `int PlayStream(spelling::I2sAudioOutput& out, int rate, int total)` |
| `ReadByteTimed` | function | `micro/examples/rp2350/src/main_i2s_relay.cc:88` | `int ReadByteTimed(int timeout_ms)` |
| `ReadHop` | function | `micro/examples/rp2350/src/main_i2s_relay.cc:98` | `int ReadHop(int16_t* out, int n)` |
| `ReadLine` | function | `micro/examples/rp2350/src/main_i2s_relay.cc:71` | `int ReadLine(char* buf, int maxlen)` |
| `frame` | variable | `micro/examples/rp2350/src/main_i2s_relay.cc:165` | `extern "C" void HardFaultC(uint32_t* frame) { watchdog_hw->scratch[3] = frame[6];` |
| `main` | function | `micro/examples/rp2350/src/main_i2s_relay.cc:182` | `int main()` |
| `main` | function | `micro/examples/rp2350/src/main_live.cc:11` | `int main()` |
| `main` | function | `micro/examples/rp2350/src/main_step1_blinky.cc:11` | `int main()` |
| `main` | function | `micro/examples/rp2350/src/main_step1_blinky_w.cc:10` | `int main()` |
| `LedInit` | function | `micro/examples/rp2350/src/main_step2_printf.cc:17` | `bool LedInit()` |
| `LedPut` | function | `micro/examples/rp2350/src/main_step2_printf.cc:27` | `void LedPut(bool on)` |
| `main` | function | `micro/examples/rp2350/src/main_step2_printf.cc:37` | `int main()` |
| `LedInit` | function | `micro/examples/rp2350/src/main_step3_fft.cc:19` | `bool LedInit()` |
| `LedPut` | function | `micro/examples/rp2350/src/main_step3_fft.cc:29` | `void LedPut(bool on)` |
| `main` | function | `micro/examples/rp2350/src/main_step3_fft.cc:43` | `int main()` |
| `0` | variable | `micro/examples/rp2350/src/main_step5_synth.cc:17` | `extern "C" void tts_checkpoint(uint32_t) {} extern "C" void tts_checkpoint2(uint32_t) {} extern "C" void...` |
| `LedInit` | function | `micro/examples/rp2350/src/main_step5_synth.cc:23` | `bool LedInit()` |
| `LedPut` | function | `micro/examples/rp2350/src/main_step5_synth.cc:33` | `void LedPut(bool on)` |
| `main` | function | `micro/examples/rp2350/src/main_step5_synth.cc:43` | `int main()` |
| `0` | variable | `micro/examples/rp2350/src/main_step6_decoder.cc:22` | `extern "C" void tts_checkpoint(uint32_t) {} extern "C" void tts_checkpoint2(uint32_t) {} extern "C" void...` |
| `LedInit` | function | `micro/examples/rp2350/src/main_step6_decoder.cc:28` | `bool LedInit()` |
| `LedPut` | function | `micro/examples/rp2350/src/main_step6_decoder.cc:38` | `void LedPut(bool on)` |
| `STEP6_FLASH_DIV` | macro | `micro/examples/rp2350/src/main_step6_decoder.cc:59` | `#define STEP6_FLASH_DIV` |
| `STEP6_SYS_KHZ` | macro | `micro/examples/rp2350/src/main_step6_decoder.cc:56` | `#define STEP6_SYS_KHZ` |
| `decoder` | function | `micro/examples/rp2350/src/main_step6_decoder.cc:97` | `static neural_tts::PbDecoder decoder(cfg, g_arena, kArenaBytes);` |
| `main` | function | `micro/examples/rp2350/src/main_step6_decoder.cc:51` | `int main()` |
| `DiscardPcm` | function | `micro/examples/rp2350/src/main_step7_synthesize.cc:56` | `void DiscardPcm(void* user, const int16_t* samples, int n)` |
| `LedInit` | function | `micro/examples/rp2350/src/main_step7_synthesize.cc:35` | `bool LedInit()` |
| `LedPut` | function | `micro/examples/rp2350/src/main_step7_synthesize.cc:45` | `void LedPut(bool on)` |
| `PaintStack` | function | `micro/examples/rp2350/src/main_step7_synthesize.cc:66` | `void PaintStack()` |
| `StackFreeBytes` | function | `micro/examples/rp2350/src/main_step7_synthesize.cc:74` | `uint32_t StackFreeBytes()` |
| `__StackBottom` | variable | `micro/examples/rp2350/src/main_step7_synthesize.cc:63` | `extern "C" char __StackBottom;` |
| `decoder` | function | `micro/examples/rp2350/src/main_step7_synthesize.cc:122` | `static neural_tts::PbDecoder decoder(cfg, g_arena, kArenaBytes);` |
| `main` | function | `micro/examples/rp2350/src/main_step7_synthesize.cc:83` | `int main()` |
| `v` | variable | `micro/examples/rp2350/src/main_step7_synthesize.cc:24` | `extern "C" void tts_checkpoint(uint32_t v) { watchdog_hw->scratch[4] = v;` |
| `v` | variable | `micro/examples/rp2350/src/main_step7_synthesize.cc:28` | `extern "C" void tts_checkpoint2(uint32_t v) { watchdog_hw->scratch[5] = v;` |
| `0` | variable | `micro/examples/rp2350/src/main_step7b_framesweep.cc:19` | `extern "C" void tts_checkpoint(uint32_t) {} extern "C" void tts_checkpoint2(uint32_t) {} extern "C" void...` |
| `LedInit` | function | `micro/examples/rp2350/src/main_step7b_framesweep.cc:25` | `bool LedInit()` |
| `LedPut` | function | `micro/examples/rp2350/src/main_step7b_framesweep.cc:35` | `void LedPut(bool on)` |
| `PaintStack` | function | `micro/examples/rp2350/src/main_step7b_framesweep.cc:51` | `void PaintStack()` |
| `StackFreeBytes` | function | `micro/examples/rp2350/src/main_step7b_framesweep.cc:59` | `uint32_t StackFreeBytes()` |
| `__StackBottom` | variable | `micro/examples/rp2350/src/main_step7b_framesweep.cc:48` | `extern "C" char __StackBottom;` |
| `decoder` | function | `micro/examples/rp2350/src/main_step7b_framesweep.cc:96` | `static neural_tts::PbDecoder decoder(cfg, g_arena, kArenaBytes);` |
| `main` | function | `micro/examples/rp2350/src/main_step7b_framesweep.cc:68` | `int main()` |
| `0` | variable | `micro/examples/rp2350/src/main_step7c_synthonly.cc:23` | `extern "C" void tts_checkpoint(uint32_t) {} extern "C" void tts_checkpoint2(uint32_t) {} extern "C" void...` |
| `DiscardPcm` | function | `micro/examples/rp2350/src/main_step7c_synthonly.cc:64` | `void DiscardPcm(void* user, const int16_t* samples, int n)` |
| `LedInit` | function | `micro/examples/rp2350/src/main_step7c_synthonly.cc:29` | `bool LedInit()` |
| `LedPut` | function | `micro/examples/rp2350/src/main_step7c_synthonly.cc:39` | `void LedPut(bool on)` |
| `PaintStack` | function | `micro/examples/rp2350/src/main_step7c_synthonly.cc:74` | `void PaintStack()` |
| `StackFreeBytes` | function | `micro/examples/rp2350/src/main_step7c_synthonly.cc:82` | `uint32_t StackFreeBytes()` |
| `SynthFrame` | function | `micro/examples/rp2350/src/main_step7c_synthonly.cc:48` | `void SynthFrame(void* /*user*/, int t, neural_tts::WorldFrame* f)` |
| `__StackBottom` | variable | `micro/examples/rp2350/src/main_step7c_synthonly.cc:71` | `extern "C" char __StackBottom;` |
| `main` | function | `micro/examples/rp2350/src/main_step7c_synthonly.cc:91` | `int main()` |
| `main` | function | `micro/examples/rp2350/src/main_test.cc:12` | `int main()` |
| `0xFA17FA17u` | variable | `micro/examples/rp2350/src/main_tflm_invoke_test.cc:33` | `extern "C" void isr_hardfault_c(uint32_t* sp) { watchdog_hw->scratch[4] = 0xFA17FA17u;` |
| `BeginEvent` | function | `micro/examples/rp2350/src/main_tflm_invoke_test.cc:68` | `uint32_t BeginEvent(const char* tag) override` |
| `EndEvent` | function | `micro/examples/rp2350/src/main_tflm_invoke_test.cc:73` | `void EndEvent(uint32_t handle) override` |
| `FeedWatchdog` | function | `micro/examples/rp2350/src/main_tflm_invoke_test.cc:100` | `bool FeedWatchdog(repeating_timer_t*)` |
| `INVOKE_TEST_SYS_KHZ` | macro | `micro/examples/rp2350/src/main_tflm_invoke_test.cc:117` | `#define INVOKE_TEST_SYS_KHZ` |
| `Report` | function | `micro/examples/rp2350/src/main_tflm_invoke_test.cc:77` | `void Report()` |
| `Reset` | function | `micro/examples/rp2350/src/main_tflm_invoke_test.cc:76` | `void Reset()` |
| `TRACE` | macro | `micro/examples/rp2350/src/main_tflm_invoke_test.cc:53` | `#define TRACE(...)` |
| `__end__` | variable | `micro/examples/rp2350/src/main_tflm_invoke_test.cc:111` | `extern char __end__;` |
| `interp` | function | `micro/examples/rp2350/src/main_tflm_invoke_test.cc:158` | `static tflite::MicroInterpreter interp(model, resolver, g_arena, kArenaBytes, /*resource_variables=*/nullptr...` |
| `main` | function | `micro/examples/rp2350/src/main_tflm_invoke_test.cc:108` | `int main()` |
| `frame` | variable | `micro/examples/rp2350/src/main_tts.cc:49` | `extern "C" void HardFaultC(uint32_t* frame) { watchdog_hw->scratch[3] = frame[6];` |
| `main` | function | `micro/examples/rp2350/src/main_tts.cc:64` | `int main()` |
| `v` | variable | `micro/examples/rp2350/src/main_tts.cc:37` | `extern "C" void tts_checkpoint(uint32_t v) { watchdog_hw->scratch[0] = v;` |
| `v` | variable | `micro/examples/rp2350/src/main_tts.cc:41` | `extern "C" void tts_checkpoint2(uint32_t v) { watchdog_hw->scratch[1] = v;` |
| `0xFA17FA17u` | variable | `micro/examples/rp2350/src/main_tts_ladder_test.cc:47` | `extern "C" void isr_hardfault_c(uint32_t* sp) { watchdog_hw->scratch[4] = 0xFA17FA17u;` |
| `EmitPcm` | function | `micro/examples/rp2350/src/main_tts_ladder_test.cc:90` | `void EmitPcm(void* user, const int16_t* samples, int n)` |
| `TRACE` | macro | `micro/examples/rp2350/src/main_tts_ladder_test.cc:77` | `#define TRACE(...)` |
| `TTS_LADDER_EXECUTE` | macro | `micro/examples/rp2350/src/main_tts_ladder_test.cc:33` | `#define TTS_LADDER_EXECUTE` |
| `TTS_LADDER_STAGE` | macro | `micro/examples/rp2350/src/main_tts_ladder_test.cc:27` | `#define TTS_LADDER_STAGE` |
| `__end__` | variable | `micro/examples/rp2350/src/main_tts_ladder_test.cc:106` | `extern char __end__;` |
| `decoder` | function | `micro/examples/rp2350/src/main_tts_ladder_test.cc:186` | `static neural_tts::PbDecoder decoder(cfg, g_arena, kArenaBytes);` |
| `main` | function | `micro/examples/rp2350/src/main_tts_ladder_test.cc:104` | `int main()` |
| `main` | function | `micro/examples/rp2350/src/main_usb_banner_test.cc:29` | `int main()` |
| `sp` | variable | `micro/examples/rp2350/src/main_usb_banner_test.cc:18` | `extern "C" void isr_hardfault(void) { uint32_t* sp;` |
| `main` | function | `micro/examples/rp2350/src/main_wifi.cc:17` | `int main()` |
| `main` | function | `micro/examples/rp2350/src/main_wifi_hardware.cc:12` | `int main()` |
| `BeginEvent` | function | `micro/examples/rp2350/src/op_profiler.cc:11` | `uint32_t OpProfiler::BeginEvent(const char* tag)` |
| `EndEvent` | function | `micro/examples/rp2350/src/op_profiler.cc:24` | `void OpProfiler::EndEvent(uint32_t event_handle)` |
| `Report` | function | `micro/examples/rp2350/src/op_profiler.cc:29` | `void OpProfiler::Report(const char* label) const` |
| `TagAgg` | struct | `micro/examples/rp2350/src/op_profiler.cc:44` | `` |
| `Report` | function | `micro/examples/rp2350/src/op_profiler.h:55` | `void Report(const char* label) const;` |
| `Reset` | function | `micro/examples/rp2350/src/op_profiler.h:46` | `void Reset()` |
| `SPELLING_OP_PROFILER_H_` | macro | `micro/examples/rp2350/src/op_profiler.h:26` | `#define SPELLING_OP_PROFILER_H_` |
| `num_events` | function | `micro/examples/rp2350/src/op_profiler.h:51` | `int num_events() const` |
| `SPELLING_SPELLING_LABELS_H_` | macro | `micro/examples/rp2350/src/spelling_labels.h:19` | `#define SPELLING_SPELLING_LABELS_H_` |
| `SpokenForLabel` | function | `micro/examples/rp2350/src/spelling_labels.h:25` | `inline const char* SpokenForLabel(const char* label)` |
| `RunTestApp` | function | `micro/examples/rp2350/src/test_app.cc:147` | `void RunTestApp(unsigned led_pin)` |
| `RunVadDemo` | function | `micro/examples/rp2350/src/test_app.cc:66` | `void RunVadDemo(uint8_t* arena, std::size_t arena_size, kiss_fftr_state* fft)` |
| `SPELLING_TEST_APP_H_` | macro | `micro/examples/rp2350/src/test_app.h:9` | `#define SPELLING_TEST_APP_H_` |
| `EmitToUsb` | function | `micro/examples/rp2350/src/tts_service.cc:55` | `void EmitToUsb(void* user, const int16_t* samples, int n)` |
| `ReadLine` | function | `micro/examples/rp2350/src/tts_service.cc:34` | `int ReadLine(char* buf, int maxlen)` |
| `RunTtsService` | function | `micro/examples/rp2350/src/tts_service.cc:63` | `void RunTtsService(uint8_t* arena, std::size_t arena_size)` |
| `SetBootReport` | function | `micro/examples/rp2350/src/tts_service.cc:22` | `void SetBootReport(const BootReport& report)` |
| `g_neural_tts_pack` | variable | `micro/examples/rp2350/src/tts_service.cc:12` | `extern "C" const uint8_t g_neural_tts_pack[];` |
| `BootReport` | struct | `micro/examples/rp2350/src/tts_service.h:32` | `` |
| `SPELLING_TTS_SERVICE_H_` | macro | `micro/examples/rp2350/src/tts_service.h:21` | `#define SPELLING_TTS_SERVICE_H_` |
| `SetBootReport` | function | `micro/examples/rp2350/src/tts_service.h:39` | `void SetBootReport(const BootReport& report);` |
| `Begin` | function | `micro/examples/rp2350/src/usb_audio_io.cc:67` | `void UsbAudioOutput::Begin(int sample_rate, int num_samples, const char* kind)` |
| `Drain` | function | `micro/examples/rp2350/src/usb_audio_io.cc:60` | `void UsbAudioInput::Drain()` |
| `End` | function | `micro/examples/rp2350/src/usb_audio_io.cc:76` | `void UsbAudioOutput::End()` |
| `ReadByteTimed` | function | `micro/examples/rp2350/src/usb_audio_io.cc:18` | `int ReadByteTimed(int timeout_ms)` |
| `ReadHop` | function | `micro/examples/rp2350/src/usb_audio_io.cc:25` | `bool UsbAudioInput::ReadHop(int16_t* out, int n)` |
| `Write` | function | `micro/examples/rp2350/src/usb_audio_io.cc:72` | `void UsbAudioOutput::Write(const int16_t* samples, int n)` |
| `SPELLING_USB_AUDIO_IO_H_` | macro | `micro/examples/rp2350/src/usb_audio_io.h:19` | `#define SPELLING_USB_AUDIO_IO_H_` |
| `UsbAudioInput` | class | `micro/examples/rp2350/src/usb_audio_io.h:25` | `` |
| `UsbAudioOutput` | class | `micro/examples/rp2350/src/usb_audio_io.h:31` | `` |
| `AnnounceMatch` | function | `micro/examples/rp2350/src/wifi_app.cc:345` | `void AnnounceMatch(const char* name, char* ssid, std::size_t* ssid_len,                    AudioO...` |
| `AppendChar` | function | `micro/examples/rp2350/src/wifi_app.cc:222` | `std::size_t AppendChar(char* buf, std::size_t len, char c, bool* caps,                        Aud...` |
| `AppendSpokenForChar` | function | `micro/examples/rp2350/src/wifi_app.cc:110` | `void AppendSpokenForChar(char* dst, std::size_t cap, char c)` |
| `Classify` | function | `micro/examples/rp2350/src/wifi_app.cc:79` | `Tok Classify(const char* label, char* out_char)` |
| `CountPrefixMatches` | function | `micro/examples/rp2350/src/wifi_app.cc:323` | `int CountPrefixMatches(const char* prefix, int* only_idx)` |
| `DigitWord` | function | `micro/examples/rp2350/src/wifi_app.cc:51` | `const char* DigitWord(char c)` |
| `DoConnect` | function | `micro/examples/rp2350/src/wifi_app.cc:190` | `void DoConnect(const char* ssid, const char* pw, AudioOutput& out,                AudioInput& in,...` |
| `EqualsCi` | function | `micro/examples/rp2350/src/wifi_app.cc:314` | `bool EqualsCi(const char* a, const char* b)` |
| `FindExactMatch` | function | `micro/examples/rp2350/src/wifi_app.cc:336` | `int FindExactMatch(const char* name)` |
| `HasPrefixCi` | function | `micro/examples/rp2350/src/wifi_app.cc:305` | `bool HasPrefixCi(const char* name, const char* prefix, std::size_t plen)` |
| `LowerAscii` | function | `micro/examples/rp2350/src/wifi_app.cc:300` | `char LowerAscii(char c)` |
| `RunWifiAppWithIo` | function | `micro/examples/rp2350/src/wifi_app.cc:359` | `void RunWifiAppWithIo(AudioInput& in, AudioOutput& out)` |
| `ScanNetworks` | function | `micro/examples/rp2350/src/wifi_app.cc:275` | `void ScanNetworks(AudioInput& in)` |
| `ScanResultCb` | function | `micro/examples/rp2350/src/wifi_app.cc:255` | `int ScanResultCb(void* /*env*/, const cyw43_ev_scan_result_t* r)` |
| `SpeakIp` | function | `micro/examples/rp2350/src/wifi_app.cc:156` | `void SpeakIp(AudioOutput& out, AudioInput& in, uint8_t* arena,              std::size_t arena_size)` |
| `SpeakName` | function | `micro/examples/rp2350/src/wifi_app.cc:147` | `void SpeakName(const char* name, AudioOutput& out, AudioInput& in,                uint8_t* arena,...` |
| `SpeakSpelled` | function | `micro/examples/rp2350/src/wifi_app.cc:133` | `void SpeakSpelled(const char* prefix, const char* text, AudioOutput& out,                   Audio...` |
| `State` | enum | `micro/examples/rp2350/src/wifi_app.cc:30` | `` |
| `State` | class | `micro/examples/rp2350/src/wifi_app.cc:30` | `` |
| `SymbolChar` | function | `micro/examples/rp2350/src/wifi_app.cc:58` | `bool SymbolChar(const char* label, char* out)` |
| `SymbolWord` | function | `micro/examples/rp2350/src/wifi_app.cc:68` | `const char* SymbolWord(char c)` |
| `Tok` | enum | `micro/examples/rp2350/src/wifi_app.cc:38` | `` |
| `Tok` | class | `micro/examples/rp2350/src/wifi_app.cc:38` | `` |
| `SPELLING_WIFI_APP_H_` | macro | `micro/examples/rp2350/src/wifi_app.h:15` | `#define SPELLING_WIFI_APP_H_` |
| `RunWifiHardwareApp` | function | `micro/examples/rp2350/src/wifi_hardware_app.cc:13` | `void RunWifiHardwareApp()` |
| `SPELLING_WIFI_HARDWARE_APP_H_` | macro | `micro/examples/rp2350/src/wifi_hardware_app.h:10` | `#define SPELLING_WIFI_HARDWARE_APP_H_` |
| `BuildModelInput` | function | `micro/feature-generation/include/feature_generation/feature_generation.h:184` | `void BuildModelInput(float* out) const;` |
| `Compute` | function | `micro/feature-generation/include/feature_generation/feature_generation.h:117` | `void Compute(const float* waveform, std::size_t n_samples, float* out) const;` |
| `ComputeImpl` | function | `micro/feature-generation/include/feature_generation/feature_generation.h:128` | `template <typename SampleT> void ComputeImpl(const SampleT* waveform, std::size_t n_samples, float* out) const;` |
| `FEATURE_GENERATION_FEATURE_GENERATION_H_` | macro | `micro/feature-generation/include/feature_generation/feature_generation.h:30` | `#define FEATURE_GENERATION_FEATURE_GENERATION_H_` |
| `HannWindowPeriodic` | function | `micro/feature-generation/include/feature_generation/feature_generation.h:48` | `std::vector<float> HannWindowPeriodic(int length);` |
| `HzToMelSlaney` | function | `micro/feature-generation/include/feature_generation/feature_generation.h:52` | `float HzToMelSlaney(float hz);` |
| `LogMelParams` | struct | `micro/feature-generation/include/feature_generation/feature_generation.h:64` | `` |
| `LogMelSpectrogram` | class | `micro/feature-generation/include/feature_generation/feature_generation.h:98` | `` |
| `MakeMelFilterbank` | function | `micro/feature-generation/include/feature_generation/feature_generation.h:57` | `std::vector<float> MakeMelFilterbank(int n_freq, int n_mels, int sample_rate, float f_min, float f_max);` |
| `MelStreamer` | class | `micro/feature-generation/include/feature_generation/feature_generation.h:164` | `` |
| `MelToHzSlaney` | function | `micro/feature-generation/include/feature_generation/feature_generation.h:53` | `float MelToHzSlaney(float mel);` |
| `PushHop` | function | `micro/feature-generation/include/feature_generation/feature_generation.h:178` | `void PushHop(const float* hop_samples);` |
| `Reset` | function | `micro/feature-generation/include/feature_generation/feature_generation.h:174` | `void Reset();` |
| `filled` | function | `micro/feature-generation/include/feature_generation/feature_generation.h:186` | `int filled() const` |
| `kiss_fftr_state` | struct | `micro/feature-generation/include/feature_generation/feature_generation.h:38` | `` |
| `n_freq` | function | `micro/feature-generation/include/feature_generation/feature_generation.h:122` | `int n_freq() const` |
| `n_mels` | function | `micro/feature-generation/include/feature_generation/feature_generation.h:120` | `int n_mels() const` |
| `n_mels` | function | `micro/feature-generation/include/feature_generation/feature_generation.h:187` | `int n_mels() const` |
| `params` | function | `micro/feature-generation/include/feature_generation/feature_generation.h:123` | `const LogMelParams& params() const` |
| `target_frames` | function | `micro/feature-generation/include/feature_generation/feature_generation.h:121` | `int target_frames() const` |
| `window_frames` | function | `micro/feature-generation/include/feature_generation/feature_generation.h:188` | `int window_frames() const` |
| `_include_guard` | function | `micro/feature-generation/scripts/generate_mel_tables.py:28` | `def _include_guard(stem)` |
| `fmt_floats` | function | `micro/feature-generation/scripts/generate_mel_tables.py:89` | `def fmt_floats(values, per_line)` |
| `fmt_ints` | function | `micro/feature-generation/scripts/generate_mel_tables.py:97` | `def fmt_ints(values, per_line)` |
| `hann_window_periodic` | function | `micro/feature-generation/scripts/generate_mel_tables.py:32` | `def hann_window_periodic(length)` |
| `hz_to_mel_slaney` | function | `micro/feature-generation/scripts/generate_mel_tables.py:40` | `def hz_to_mel_slaney(hz)` |
| `main` | function | `micro/feature-generation/scripts/generate_mel_tables.py:105` | `def main()` |
| `make_csr_filterbank` | function | `micro/feature-generation/scripts/generate_mel_tables.py:60` | `def make_csr_filterbank(n_freq, n_mels, sample_rate, f_min, f_max)` |
| `mel_to_hz_slaney` | function | `micro/feature-generation/scripts/generate_mel_tables.py:50` | `def mel_to_hz_slaney(mel)` |
| `FEATURE_GENERATION_FFT_SCRATCH_H_` | macro | `micro/feature-generation/src/fft_scratch.h:21` | `#define FEATURE_GENERATION_FFT_SCRATCH_H_` |
| `g_fft_scratch_frame` | variable | `micro/feature-generation/src/fft_scratch.h:32` | `extern float g_fft_scratch_frame[kFftScratchNFft];` |
| `g_fft_scratch_pow` | variable | `micro/feature-generation/src/fft_scratch.h:34` | `extern float g_fft_scratch_pow[kFftScratchNFreq];` |
| `g_fft_scratch_spec` | variable | `micro/feature-generation/src/fft_scratch.h:33` | `extern kiss_fft_cpx g_fft_scratch_spec[kFftScratchNFreq];` |
| `Compute` | function | `micro/feature-generation/src/log_mel.cc:439` | `void LogMelSpectrogram::Compute(const float* waveform, std::size_t n_samples,                    ...` |
| `Compute` | function | `micro/feature-generation/src/log_mel.cc:444` | `void LogMelSpectrogram::Compute(const int16_t* waveform, std::size_t n_samples,                  ...` |
| `ComputeImpl` | function | `micro/feature-generation/src/log_mel.cc:313` | `template <typename SampleT> void LogMelSpectrogram::ComputeImpl(const SampleT* waveform,         ...` |
| `HannWindowPeriodic` | function | `micro/feature-generation/src/log_mel.cc:107` | `std::vector<float> HannWindowPeriodic(int length)` |
| `HzToMelSlaney` | function | `micro/feature-generation/src/log_mel.cc:93` | `float HzToMelSlaney(float hz)` |
| `LogMelSpectrogram` | function | `micro/feature-generation/src/log_mel.cc:163` | `LogMelSpectrogram::LogMelSpectrogram(const LogMelParams& params)     : params_(params), n_freq_(p...` |
| `MakeMelFilterbank` | function | `micro/feature-generation/src/log_mel.cc:121` | `std::vector<float> MakeMelFilterbank(int n_freq, int n_mels, int sample_rate,                    ...` |
| `MelToHzSlaney` | function | `micro/feature-generation/src/log_mel.cc:100` | `float MelToHzSlaney(float mel)` |
| `ReflectIndex` | function | `micro/feature-generation/src/log_mel.cc:69` | `inline int ReflectIndex(int i, int n)` |
| `ToFloatSample` | function | `micro/feature-generation/src/log_mel.cc:87` | `inline float ToFloatSample(float s)` |
| `ToFloatSample` | function | `micro/feature-generation/src/log_mel.cc:88` | `inline float ToFloatSample(int16_t s)` |
| `bin_hz` | function | `micro/feature-generation/src/log_mel.cc:136` | `std::vector<float> bin_hz(static_cast<std::size_t>(n_freq));` |
| `exp` | function | `micro/feature-generation/src/log_mel.cc:102` | `return kMinLogHz * std::exp(kLogStep * (mel - kMinLogMel));` |
| `fb` | function | `micro/feature-generation/src/log_mel.cc:142` | `std::vector<float> fb( static_cast<std::size_t>(n_mels) * static_cast<std::size_t>(n_freq), 0.0f);` |
| `hz_pts` | function | `micro/feature-generation/src/log_mel.cc:132` | `std::vector<float> hz_pts(mel_pts.size());` |
| `mel_pts` | function | `micro/feature-generation/src/log_mel.cc:126` | `std::vector<float> mel_pts(static_cast<std::size_t>(n_mels + 2));` |
| `w` | function | `micro/feature-generation/src/log_mel.cc:112` | `std::vector<float> w(length);` |
| `BuildModelInput` | function | `micro/feature-generation/src/mel_streamer.cc:93` | `void MelStreamer::BuildModelInput(float* out) const` |
| `MelStreamer` | function | `micro/feature-generation/src/mel_streamer.cc:10` | `MelStreamer::MelStreamer(int n_mels, int window_frames, int n_fft,                          const...` |
| `PushHop` | function | `micro/feature-generation/src/mel_streamer.cc:53` | `void MelStreamer::PushHop(const float* hop_samples)` |
| `Reset` | function | `micro/feature-generation/src/mel_streamer.cc:39` | `void MelStreamer::Reset()` |
| `DenseToCsr` | function | `micro/feature-generation/tests/feature_generation_test.cc:24` | `void DenseToCsr(const std::vector<float>& dense, int n_mels, int n_freq,                 std::vec...` |
| `TF_LITE_MICRO_TEST` | function | `micro/feature-generation/tests/feature_generation_test.cc:46` | `TF_LITE_MICRO_TESTS_BEGIN  TF_LITE_MICRO_TEST(HannWindowPeriodicEndpoints)` |
| `TF_LITE_MICRO_TEST` | function | `micro/feature-generation/tests/feature_generation_test.cc:54` | `TF_LITE_MICRO_TEST(MelScaleRoundTrip)` |
| `TF_LITE_MICRO_TEST` | function | `micro/feature-generation/tests/feature_generation_test.cc:61` | `TF_LITE_MICRO_TEST(StreamerMatchesBatch)` |
| `buf` | function | `micro/feature-generation/tests/feature_generation_test.cc:70` | `std::vector<float> buf(n_samples);` |
| `out_ref` | function | `micro/feature-generation/tests/feature_generation_test.cc:93` | `std::vector<float> out_ref(static_cast<std::size_t>(n_mels) * window_frames);` |
| `out_stream` | function | `micro/feature-generation/tests/feature_generation_test.cc:111` | `std::vector<float> out_stream(static_cast<std::size_t>(n_mels) * window_frames);` |
| `G2P_G2P_H_` | macro | `micro/g2p/include/g2p/g2p.h:18` | `#define G2P_G2P_H_` |
| `Add` | function | `micro/g2p/include/g2p/g2p_dict.h:38` | `void Add(std::string_view word, std::string_view ipa);` |
| `DictLookup` | function | `micro/g2p/include/g2p/g2p_dict.h:26` | `bool DictLookup(std::string_view word, std::string* ipa);` |
| `EnsureSorted` | function | `micro/g2p/include/g2p/g2p_dict.h:47` | `private: void EnsureSorted() const;` |
| `G2P_G2P_DICT_H_` | macro | `micro/g2p/include/g2p/g2p_dict.h:15` | `#define G2P_G2P_DICT_H_` |
| `Lexicon` | class | `micro/g2p/include/g2p/g2p_dict.h:30` | `` |
| `LoadFromFile` | function | `micro/g2p/include/g2p/g2p_dict.h:35` | `bool LoadFromFile(const std::string& path);` |
| `Lookup` | function | `micro/g2p/include/g2p/g2p_dict.h:41` | `bool Lookup(std::string_view word, std::string* ipa) const;` |
| `empty` | function | `micro/g2p/include/g2p/g2p_dict.h:44` | `bool empty() const` |
| `size` | function | `micro/g2p/include/g2p/g2p_dict.h:43` | `size_t size() const` |
| `G2P_G2P_PHONES_H_` | macro | `micro/g2p/include/g2p/g2p_phones.h:7` | `#define G2P_G2P_PHONES_H_` |
| `PhoneTokenList` | struct | `micro/g2p/include/g2p/g2p_phones.h:15` | `` |
| `TextToPhoneList` | function | `micro/g2p/include/g2p/g2p_phones.h:27` | `bool TextToPhoneList(const char* text, PhoneTokenList* out, const Lexicon* overrides = nullptr);` |
| `TokenizeIpaToList` | function | `micro/g2p/include/g2p/g2p_phones.h:31` | `bool TokenizeIpaToList(const char* ipa, PhoneTokenList* out);` |
| `push` | function | `micro/g2p/include/g2p/g2p_phones.h:21` | `bool push(const char* tok);` |
| `HasDigit` | function | `micro/g2p/src/g2p.cc:14` | `bool HasDigit(const std::string& s)` |
| `ResolveToken` | function | `micro/g2p/src/g2p.cc:22` | `std::string ResolveToken(const std::string& tok, const Lexicon* overrides)` |
| `TextToPhones` | function | `micro/g2p/src/g2p.cc:33` | `std::vector<std::string> TextToPhones(const std::string& text,                                   ...` |
| `Add` | function | `micro/g2p/src/g2p_dict.cc:106` | `void Lexicon::Add(std::string_view word, std::string_view ipa)` |
| `DecodeIpa` | function | `micro/g2p/src/g2p_dict.cc:16` | `std::string DecodeIpa(uint32_t start, unsigned count)` |
| `DictLookup` | function | `micro/g2p/src/g2p_dict.cc:51` | `bool DictLookup(std::string_view word, std::string* ipa)` |
| `EnsureSorted` | function | `micro/g2p/src/g2p_dict.cc:113` | `void Lexicon::EnsureSorted() const` |
| `LoadFromFile` | function | `micro/g2p/src/g2p_dict.cc:145` | `bool Lexicon::LoadFromFile(const std::string& path)` |
| `Lookup` | function | `micro/g2p/src/g2p_dict.cc:132` | `bool Lexicon::Lookup(std::string_view word, std::string* ipa) const` |
| `NormalizeWordKey` | function | `micro/g2p/src/g2p_dict.cc:35` | `std::string NormalizeWordKey(std::string_view word)` |
| `RestartKey` | function | `micro/g2p/src/g2p_dict.cc:27` | `std::string RestartKey(int block)` |
| `stable_sort` | function | `micro/g2p/src/g2p_dict.cc:115` | `std::stable_sort(       entries_.begin(), entries_.end(),       [](const auto& a, const auto& b)` |
| `G2P_DICT_DATA_H_` | macro | `micro/g2p/src/g2p_dict_data.h:13` | `#define G2P_DICT_DATA_H_` |
| `CardinalNonNegativeIpa` | function | `micro/g2p/src/g2p_numbers.cc:70` | `bool CardinalNonNegativeIpa(long long n, std::string* out)` |
| `DigitSequenceIpa` | function | `micro/g2p/src/g2p_numbers.cc:40` | `std::string DigitSequenceIpa(std::string_view digits)` |
| `IntegerDecimalStringIpa` | function | `micro/g2p/src/g2p_numbers.cc:108` | `bool IntegerDecimalStringIpa(std::string s, std::string* out)` |
| `NumberWordToIpa` | function | `micro/g2p/src/g2p_numbers.cc:184` | `bool NumberWordToIpa(std::string_view token, std::string* ipa)` |
| `Scale` | struct | `micro/g2p/src/g2p_numbers.cc:77` | `` |
| `Under1000Ipa` | function | `micro/g2p/src/g2p_numbers.cc:61` | `std::string Under1000Ipa(int n)` |
| `Under100Ipa` | function | `micro/g2p/src/g2p_numbers.cc:51` | `std::string Under100Ipa(int n)` |
| `G2P_NUMBERS_H_` | macro | `micro/g2p/src/g2p_numbers.h:8` | `#define G2P_NUMBERS_H_` |
| `NumberWordToIpa` | function | `micro/g2p/src/g2p_numbers.h:17` | `bool NumberWordToIpa(std::string_view token, std::string* ipa);` |
| `HasDigit` | function | `micro/g2p/src/g2p_phones.cc:16` | `bool HasDigit(const char* s)` |
| `ResolveTokenBuf` | function | `micro/g2p/src/g2p_phones.cc:27` | `bool ResolveTokenBuf(const char* tok, char* out, std::size_t cap,                      const Lexi...` |
| `TextToPhoneList` | function | `micro/g2p/src/g2p_phones.cc:61` | `bool TextToPhoneList(const char* text, PhoneTokenList* out,                      const Lexicon* o...` |
| `TokenizeIpaToList` | function | `micro/g2p/src/g2p_phones.cc:53` | `bool TokenizeIpaToList(const char* ipa, PhoneTokenList* out)` |
| `push` | function | `micro/g2p/src/g2p_phones.cc:45` | `bool PhoneTokenList::push(const char* tok)` |
| `AddPrimaryStressIfMissing` | function | `micro/g2p/src/g2p_rules.cc:352` | `std::string AddPrimaryStressIfMissing(std::string s)` |
| `GraphemeToIpa` | function | `micro/g2p/src/g2p_rules.cc:371` | `std::string GraphemeToIpa(std::string_view word)` |
| `IsConsonant` | function | `micro/g2p/src/g2p_rules.cc:51` | `constexpr bool IsConsonant(char c)` |
| `IsVowel` | function | `micro/g2p/src/g2p_rules.cc:47` | `constexpr bool IsVowel(char c)` |
| `LastIpaUnitIsVowel` | function | `micro/g2p/src/g2p_rules.cc:34` | `bool LastIpaUnitIsVowel(std::string_view prev)` |
| `LastUtf8Char` | function | `micro/g2p/src/g2p_rules.cc:23` | `std::string_view LastUtf8Char(std::string_view s)` |
| `LetterHomophoneToIpa` | function | `micro/g2p/src/g2p_rules.cc:467` | `bool LetterHomophoneToIpa(std::string_view word, std::string* ipa)` |
| `Literal` | struct | `micro/g2p/src/g2p_rules.cc:104` | `` |
| `MagicELengthens` | function | `micro/g2p/src/g2p_rules.cc:62` | `bool MagicELengthens(std::string_view w, int vowel_i)` |
| `NextVowelIndex` | function | `micro/g2p/src/g2p_rules.cc:55` | `int NextVowelIndex(std::string_view w, int start)` |
| `RulesWordToIpa` | function | `micro/g2p/src/g2p_rules.cc:451` | `std::string RulesWordToIpa(std::string_view word)` |
| `SingleConsonant` | function | `micro/g2p/src/g2p_rules.cc:207` | `std::string SingleConsonant(char c, std::string_view w, int i)` |
| `ThVoicedWord` | function | `micro/g2p/src/g2p_rules.cc:201` | `bool ThVoicedWord(std::string_view w)` |
| `Utf8StartsWith` | function | `micro/g2p/src/g2p_rules.cc:19` | `bool Utf8StartsWith(const std::string& s, std::string_view p)` |
| `p` | function | `micro/g2p/src/g2p_rules.cc:359` | `const std::string_view p(pref);` |
| `G2P_RULES_H_` | macro | `micro/g2p/src/g2p_rules.h:12` | `#define G2P_RULES_H_` |
| `LetterHomophoneToIpa` | function | `micro/g2p/src/g2p_rules.h:26` | `bool LetterHomophoneToIpa(std::string_view word, std::string* ipa);` |
| `IsDirectAscii` | function | `micro/g2p/src/ipa_tokens.cc:81` | `bool IsDirectAscii(char c)` |
| `Rule` | struct | `micro/g2p/src/ipa_tokens.cc:18` | `` |
| `TokenizeIpa` | function | `micro/g2p/src/ipa_tokens.cc:118` | `std::vector<std::string> TokenizeIpa(const std::string& ipa)` |
| `Utf8Len` | function | `micro/g2p/src/ipa_tokens.cc:108` | `size_t Utf8Len(unsigned char lead)` |
| `DumpVoiceConfig` | function | `micro/klatt-tts/include/tts/config.h:140` | `bool DumpVoiceConfig(const std::string& path, const VoiceParams& vp);` |
| `LoadVoiceConfig` | function | `micro/klatt-tts/include/tts/config.h:136` | `bool LoadVoiceConfig(const std::string& path, VoiceParams& vp);` |
| `Lookup` | function | `micro/klatt-tts/include/tts/config.h:128` | `const Phone* Lookup(const std::string& ipa) const;` |
| `TTS_CONFIG_H_` | macro | `micro/klatt-tts/include/tts/config.h:15` | `#define TTS_CONFIG_H_` |
| `VoiceParams` | struct | `micro/klatt-tts/include/tts/config.h:24` | `` |
| `Antiresonator` | struct | `micro/klatt-tts/include/tts/klatt.h:120` | `` |
| `Biquad` | struct | `micro/klatt-tts/include/tts/klatt.h:101` | `` |
| `EnsureLfShape` | function | `micro/klatt-tts/include/tts/klatt.h:157` | `void EnsureLfShape(float rd);` |
| `KlattParams` | struct | `micro/klatt-tts/include/tts/klatt.h:62` | `` |
| `KlattSynth` | class | `micro/klatt-tts/include/tts/klatt.h:134` | `` |
| `LfDeriv` | function | `micro/klatt-tts/include/tts/klatt.h:160` | `inline float LfDeriv(float phase) const;` |
| `NextNoise` | function | `micro/klatt-tts/include/tts/klatt.h:154` | `private: float NextNoise();` |
| `Render` | function | `micro/klatt-tts/include/tts/klatt.h:141` | `std::vector<float> Render(const std::vector<SynthFrame>& frames, int samples_per_frame);` |
| `RenderFrame` | function | `micro/klatt-tts/include/tts/klatt.h:150` | `void RenderFrame(const SynthFrame& cur, const SynthFrame& nxt, int samples_per_frame, float* out);` |
| `Reset` | function | `micro/klatt-tts/include/tts/klatt.h:57` | `void Reset()` |
| `Reset` | function | `micro/klatt-tts/include/tts/klatt.h:116` | `void Reset()` |
| `Reset` | function | `micro/klatt-tts/include/tts/klatt.h:131` | `void Reset()` |
| `Resonator` | struct | `micro/klatt-tts/include/tts/klatt.h:46` | `` |
| `SetBandpass` | function | `micro/klatt-tts/include/tts/klatt.h:107` | `void SetBandpass(float freq_hz, float q, float sample_rate);` |
| `SetParams` | function | `micro/klatt-tts/include/tts/klatt.h:50` | `void SetParams(float freq_hz, float bw_hz, float sample_rate);` |
| `Step` | function | `micro/klatt-tts/include/tts/klatt.h:51` | `inline float Step(float x)` |
| `Step` | function | `micro/klatt-tts/include/tts/klatt.h:108` | `inline float Step(float x)` |
| `Step` | function | `micro/klatt-tts/include/tts/klatt.h:125` | `inline float Step(float x)` |
| `SynthFrame` | struct | `micro/klatt-tts/include/tts/klatt.h:32` | `` |
| `TTS_KLATT_H_` | macro | `micro/klatt-tts/include/tts/klatt.h:22` | `#define TTS_KLATT_H_` |
| `LookupPhone` | function | `micro/klatt-tts/include/tts/phonemes.h:72` | `const Phone* LookupPhone(const std::string& ipa);` |
| `Phone` | struct | `micro/klatt-tts/include/tts/phonemes.h:45` | `` |
| `PhoneClass` | enum | `micro/klatt-tts/include/tts/phonemes.h:28` | `` |
| `Source` | enum | `micro/klatt-tts/include/tts/phonemes.h:38` | `` |
| `TTS_PHONEMES_H_` | macro | `micro/klatt-tts/include/tts/phonemes.h:20` | `#define TTS_PHONEMES_H_` |
| `BuildSegments` | function | `micro/klatt-tts/include/tts/synth_internal.h:56` | `int BuildSegments(const char* const* phones, int n_phones, const VoiceParams& vp, Segment* out, int max_out);` |
| `CountFrames` | function | `micro/klatt-tts/include/tts/synth_internal.h:60` | `size_t CountFrames(const std::vector<Segment>& segs, float dur_scale);` |
| `FillParamTracks` | function | `micro/klatt-tts/include/tts/synth_internal.h:88` | `void FillParamTracks(const std::vector<Segment>& segs, const VoiceParams& vp, float dur_scale, bool question...` |
| `ParamTracks` | struct | `micro/klatt-tts/include/tts/synth_internal.h:65` | `` |
| `Segment` | struct | `micro/klatt-tts/include/tts/synth_internal.h:28` | `` |
| `SmoothAsym` | function | `micro/klatt-tts/include/tts/synth_internal.h:47` | `void SmoothAsym(float* v, size_t n, float attack_ms, float release_ms);` |
| `SmoothBidir` | function | `micro/klatt-tts/include/tts/synth_internal.h:45` | `void SmoothBidir(float* v, size_t n, float tau_ms);` |
| `SmoothFwd` | function | `micro/klatt-tts/include/tts/synth_internal.h:46` | `void SmoothFwd(float* v, size_t n, float tau_ms);` |
| `TTS_SYNTH_INTERNAL_H_` | macro | `micro/klatt-tts/include/tts/synth_internal.h:9` | `#define TTS_SYNTH_INTERNAL_H_` |
| `ArenaBytes` | function | `micro/klatt-tts/include/tts/synth_stream.h:86` | `uint8_t* ArenaBytes(size_t count, size_t align);` |
| `ArenaFloats` | function | `micro/klatt-tts/include/tts/synth_stream.h:85` | `float* ArenaFloats(size_t count);` |
| `ArenaReset` | function | `micro/klatt-tts/include/tts/synth_stream.h:84` | `void ArenaReset()` |
| `BeginIpa` | function | `micro/klatt-tts/include/tts/synth_stream.h:66` | `int BeginIpa(const char* ipa, const StreamOptions& opts);` |
| `BeginPhones` | function | `micro/klatt-tts/include/tts/synth_stream.h:82` | `private: int BeginPhones(const std::vector<std::string>& phones, const StreamOptions& opts);` |
| `BeginText` | function | `micro/klatt-tts/include/tts/synth_stream.h:61` | `int BeginText(const char* text, const StreamOptions& opts, const g2p::Lexicon* overrides = nullptr);` |
| `Read` | function | `micro/klatt-tts/include/tts/synth_stream.h:71` | `int Read(float* out, int max_samples);` |
| `RenderNextFrame` | function | `micro/klatt-tts/include/tts/synth_stream.h:87` | `void RenderNextFrame();` |
| `StreamOptions` | struct | `micro/klatt-tts/include/tts/synth_stream.h:37` | `` |
| `StreamStatus` | enum | `micro/klatt-tts/include/tts/synth_stream.h:44` | `` |
| `StreamSynth` | class | `micro/klatt-tts/include/tts/synth_stream.h:51` | `` |
| `TTS_SYNTH_STREAM_H_` | macro | `micro/klatt-tts/include/tts/synth_stream.h:22` | `#define TTS_SYNTH_STREAM_H_` |
| `done` | function | `micro/klatt-tts/include/tts/synth_stream.h:73` | `bool done() const` |
| `sample_rate` | function | `micro/klatt-tts/include/tts/synth_stream.h:76` | `int sample_rate() const` |
| `total_samples` | function | `micro/klatt-tts/include/tts/synth_stream.h:77` | `int total_samples() const` |
| `TTS_TTS_H_` | macro | `micro/klatt-tts/include/tts/tts.h:26` | `#define TTS_TTS_H_` |
| `ClassName` | function | `micro/klatt-tts/src/config.cc:14` | `const char* ClassName(PhoneClass c)` |
| `DefaultVoiceParams` | function | `micro/klatt-tts/src/config.cc:146` | `VoiceParams DefaultVoiceParams()` |
| `DumpVoiceConfig` | function | `micro/klatt-tts/src/config.cc:216` | `bool DumpVoiceConfig(const std::string& path, const VoiceParams& vp)` |
| `LoadVoiceConfig` | function | `micro/klatt-tts/src/config.cc:152` | `bool LoadVoiceConfig(const std::string& path, VoiceParams& vp)` |
| `Lookup` | function | `micro/klatt-tts/src/config.cc:139` | `const Phone* VoiceParams::Lookup(const std::string& ipa) const` |
| `SetPhoneField` | function | `micro/klatt-tts/src/config.cc:105` | `bool SetPhoneField(Phone& p, const std::string& field, float v)` |
| `SourceName` | function | `micro/klatt-tts/src/config.cc:34` | `const char* SourceName(Source s)` |
| `EnsureLfShape` | function | `micro/klatt-tts/src/klatt.cc:94` | `void KlattSynth::EnsureLfShape(float rd)` |
| `GlottalPulse` | function | `micro/klatt-tts/src/klatt.cc:16` | `inline float GlottalPulse(float phase, float open, float close)` |
| `KlattSynth` | function | `micro/klatt-tts/src/klatt.cc:82` | `KlattSynth::KlattSynth(float sample_rate, const KlattParams& params)     : sample_rate_(sample_ra...` |
| `LfDeriv` | function | `micro/klatt-tts/src/klatt.cc:165` | `inline float KlattSynth::LfDeriv(float phase) const` |
| `NextNoise` | function | `micro/klatt-tts/src/klatt.cc:173` | `float KlattSynth::NextNoise()` |
| `Render` | function | `micro/klatt-tts/src/klatt.cc:296` | `std::vector<float> KlattSynth::Render(const std::vector<SynthFrame>& frames,                     ...` |
| `RenderFrame` | function | `micro/klatt-tts/src/klatt.cc:181` | `void KlattSynth::RenderFrame(const SynthFrame& cur, const SynthFrame& nxt,                       ...` |
| `SetBandpass` | function | `micro/klatt-tts/src/klatt.cc:55` | `void Biquad::SetBandpass(float freq_hz, float q, float sample_rate)` |
| `SetParams` | function | `micro/klatt-tts/src/klatt.cc:48` | `void Resonator::SetParams(float freq_hz, float bw_hz, float sample_rate)` |
| `SetParams` | function | `micro/klatt-tts/src/klatt.cc:70` | `void Antiresonator::SetParams(float freq_hz, float bw_hz, float sample_rate)` |
| `TiltCoef` | function | `micro/klatt-tts/src/klatt.cc:29` | `float TiltCoef(float tilt_db, float sample_rate)` |
| `DefaultPhoneTable` | function | `micro/klatt-tts/src/phonemes.cc:96` | `std::vector<Phone> DefaultPhoneTable()` |
| `LookupPhone` | function | `micro/klatt-tts/src/phonemes.cc:90` | `const Phone* LookupPhone(const std::string& ipa)` |
| `AppendStop` | function | `micro/klatt-tts/src/synth_internal.cc:38` | `void AppendStop(const Phone& p, const VoiceParams& vp, int src_token,                 Segment* ou...` |
| `BuildSegments` | function | `micro/klatt-tts/src/synth_internal.cc:75` | `int BuildSegments(const char* const* phones, int n_phones, const VoiceParams& vp,                ...` |
| `BuildSegments` | function | `micro/klatt-tts/src/synth_internal.cc:176` | `std::vector<Segment> BuildSegments(const std::vector<std::string>& phones,                       ...` |
| `CountFrames` | function | `micro/klatt-tts/src/synth_internal.cc:222` | `size_t CountFrames(const std::vector<Segment>& segs, float dur_scale)` |
| `FillParamTracks` | function | `micro/klatt-tts/src/synth_internal.cc:232` | `void FillParamTracks(const std::vector<Segment>& segs, const VoiceParams& vp,                    ...` |
| `FrameAt` | function | `micro/klatt-tts/src/synth_internal.cc:339` | `SynthFrame FrameAt(const ParamTracks& t, size_t i)` |
| `MakeKlattParams` | function | `micro/klatt-tts/src/synth_internal.cc:358` | `KlattParams MakeKlattParams(const VoiceParams& vp)` |
| `SegFromPhone` | function | `micro/klatt-tts/src/synth_internal.cc:15` | `Segment SegFromPhone(const Phone& p)` |
| `SmoothAsym` | function | `micro/klatt-tts/src/synth_internal.cc:209` | `void SmoothAsym(float* v, size_t n, float attack_ms, float release_ms)` |
| `SmoothBidir` | function | `micro/klatt-tts/src/synth_internal.cc:190` | `void SmoothBidir(float* v, size_t n, float tau_ms)` |
| `SmoothFwd` | function | `micro/klatt-tts/src/synth_internal.cc:201` | `void SmoothFwd(float* v, size_t n, float tau_ms)` |
| `ArenaBytes` | function | `micro/klatt-tts/src/synth_stream.cc:34` | `uint8_t* StreamSynth::ArenaBytes(size_t count, size_t align)` |
| `ArenaFloats` | function | `micro/klatt-tts/src/synth_stream.cc:41` | `float* StreamSynth::ArenaFloats(size_t count)` |
| `BeginIpa` | function | `micro/klatt-tts/src/synth_stream.cc:54` | `int StreamSynth::BeginIpa(const char* ipa, const StreamOptions& opts)` |
| `BeginPhones` | function | `micro/klatt-tts/src/synth_stream.cc:60` | `int StreamSynth::BeginPhones(const std::vector<std::string>& phones,                             ...` |
| `BeginText` | function | `micro/klatt-tts/src/synth_stream.cc:46` | `int StreamSynth::BeginText(const char* text, const StreamOptions& opts,                          ...` |
| `Read` | function | `micro/klatt-tts/src/synth_stream.cc:140` | `int StreamSynth::Read(float* out, int max_samples)` |
| `RenderNextFrame` | function | `micro/klatt-tts/src/synth_stream.cc:125` | `void StreamSynth::RenderNextFrame()` |
| `SoftClip` | function | `micro/klatt-tts/src/synth_stream.cc:18` | `inline float SoftClip(float x)` |
| `StreamSynth` | function | `micro/klatt-tts/src/synth_stream.cc:30` | `StreamSynth::StreamSynth(const VoiceParams& vp, uint8_t* arena,                          size_t a...` |
| `Contains` | function | `micro/klatt-tts/tests/tts_test.cc:17` | `bool Contains(const std::vector<std::string>& toks, const char* needle)` |
| `TF_LITE_MICRO_TEST` | function | `micro/klatt-tts/tests/tts_test.cc:28` | `TF_LITE_MICRO_TESTS_BEGIN  TF_LITE_MICRO_TEST(G2PProducesPhones)` |
| `TF_LITE_MICRO_TEST` | function | `micro/klatt-tts/tests/tts_test.cc:35` | `TF_LITE_MICRO_TEST(G2PNumberNormalization)` |
| `TF_LITE_MICRO_TEST` | function | `micro/klatt-tts/tests/tts_test.cc:41` | `TF_LITE_MICRO_TEST(StreamSynthProducesAudioInRange)` |
| `AddEval` | function | `micro/neural-tts/host/tflm_ref/add.cpp:168` | `TfLiteStatus AddEval(TfLiteContext* context, TfLiteNode* node)` |
| `AddInit` | function | `micro/neural-tts/host/tflm_ref/add.cpp:163` | `void* AddInit(TfLiteContext* context, const char* buffer, size_t length)` |
| `EvalAdd` | function | `micro/neural-tts/host/tflm_ref/add.cpp:35` | `TfLiteStatus EvalAdd(TfLiteContext* context, TfLiteNode* node,                      TfLiteAddPara...` |
| `EvalAddQuantized` | function | `micro/neural-tts/host/tflm_ref/add.cpp:91` | `TfLiteStatus EvalAddQuantized(TfLiteContext* context, TfLiteNode* node,                          ...` |
| `Register_ADD` | function | `micro/neural-tts/host/tflm_ref/add.cpp:196` | `TFLMRegistration Register_ADD()` |
| `ConvEval` | function | `micro/neural-tts/host/tflm_ref/conv.cpp:38` | `TfLiteStatus ConvEval(TfLiteContext* context, TfLiteNode* node)` |
| `Register_CONV_2D` | function | `micro/neural-tts/host/tflm_ref/conv.cpp:129` | `TFLMRegistration Register_CONV_2D()` |
| `GetCurrentTimeTicks` | function | `micro/neural-tts/host/tflm_ref/host_platform.cpp:30` | `uint32_t GetCurrentTimeTicks()` |
| `InitializeTarget` | function | `micro/neural-tts/host/tflm_ref/host_platform.cpp:26` | `void InitializeTarget()` |
| `ticks_per_second` | function | `micro/neural-tts/host/tflm_ref/host_platform.cpp:28` | `uint32_t ticks_per_second()` |
| `CalculateOpData` | function | `micro/neural-tts/host/tflm_ref/transpose_conv.cpp:72` | `TfLiteStatus CalculateOpData(TfLiteContext* context, TfLiteNode* node,                           ...` |
| `OpData` | struct | `micro/neural-tts/host/tflm_ref/transpose_conv.cpp:36` | `` |
| `Register_TRANSPOSE_CONV` | function | `micro/neural-tts/host/tflm_ref/transpose_conv.cpp:410` | `TFLMRegistration Register_TRANSPOSE_CONV()` |
| `RuntimePaddingType` | function | `micro/neural-tts/host/tflm_ref/transpose_conv.cpp:60` | `inline PaddingType RuntimePaddingType(TfLitePadding padding)` |
| `TransposeConvEval` | function | `micro/neural-tts/host/tflm_ref/transpose_conv.cpp:261` | `TfLiteStatus TransposeConvEval(TfLiteContext* context, TfLiteNode* node)` |
| `TransposeConvInit` | function | `micro/neural-tts/host/tflm_ref/transpose_conv.cpp:146` | `void* TransposeConvInit(TfLiteContext* context, const char* buffer,                         size_...` |
| `TransposeConvPrepare` | function | `micro/neural-tts/host/tflm_ref/transpose_conv.cpp:152` | `TfLiteStatus TransposeConvPrepare(TfLiteContext* context, TfLiteNode* node)` |
| `Emit` | function | `micro/neural-tts/host/tts_cli.cc:71` | `void Emit(void* user, const int16_t* samples, int n)` |
| `ReadFile` | function | `micro/neural-tts/host/tts_cli.cc:32` | `std::vector<uint8_t> ReadFile(const char* path)` |
| `Sink` | struct | `micro/neural-tts/host/tts_cli.cc:67` | `` |
| `WriteWavHeader` | function | `micro/neural-tts/host/tts_cli.cc:47` | `void WriteWavHeader(FILE* f, int rate, int nsamples)` |
| `arena` | function | `micro/neural-tts/host/tts_cli.cc:118` | `std::vector<uint8_t> arena(1u << 20);` |
| `main` | function | `micro/neural-tts/host/tts_cli.cc:78` | `int main(int argc, char** argv)` |
| `Ctx` | struct | `micro/neural-tts/host/worldlite_synth_cli.cc:39` | `` |
| `main` | function | `micro/neural-tts/host/worldlite_synth_cli.cc:15` | `int main(int argc, char** argv)` |
| `EstimateSamples` | function | `micro/neural-tts/include/neural_tts/neural_tts.h:65` | `int EstimateSamples(const char* text);` |
| `EstimateSamplesIpa` | function | `micro/neural-tts/include/neural_tts/neural_tts.h:66` | `int EstimateSamplesIpa(const char* ipa);` |
| `NEURAL_TTS_NEURAL_TTS_H_` | macro | `micro/neural-tts/include/neural_tts/neural_tts.h:31` | `#define NEURAL_TTS_NEURAL_TTS_H_` |
| `NeuralTts` | class | `micro/neural-tts/include/neural_tts/neural_tts.h:40` | `` |
| `Stats` | struct | `micro/neural-tts/include/neural_tts/neural_tts.h:70` | `` |
| `Synthesize` | function | `micro/neural-tts/include/neural_tts/neural_tts.h:57` | `int Synthesize(const char* text, EmitFn emit, void* user);` |
| `SynthesizeIpa` | function | `micro/neural-tts/include/neural_tts/neural_tts.h:60` | `int SynthesizeIpa(const char* ipa, EmitFn emit, void* user);` |
| `SynthesizeTokens` | function | `micro/neural-tts/include/neural_tts/neural_tts.h:87` | `private: int SynthesizeTokens(void* tokens_vec, EmitFn emit, void* user, bool plan_only);` |
| `ok` | function | `micro/neural-tts/include/neural_tts/neural_tts.h:49` | `bool ok() const` |
| `stats` | function | `micro/neural-tts/include/neural_tts/neural_tts.h:84` | `const Stats& stats() const` |
| `DiphoneTypeRec` | struct | `micro/neural-tts/include/neural_tts/pack_format.h:96` | `` |
| `DiphoneUnitRec` | struct | `micro/neural-tts/include/neural_tts/pack_format.h:105` | `` |
| `NEURAL_TTS_PACK_FORMAT_H_` | macro | `micro/neural-tts/include/neural_tts/pack_format.h:13` | `#define NEURAL_TTS_PACK_FORMAT_H_` |
| `Pack` | class | `micro/neural-tts/include/neural_tts/pack_format.h:141` | `` |
| `Pack` | function | `micro/neural-tts/include/neural_tts/pack_format.h:143` | `public:   explicit Pack(const uint8_t* base)       : base_(base),         h_(reinterpret_cast<con...` |
| `PackHeader` | struct | `micro/neural-tts/include/neural_tts/pack_format.h:46` | `` |
| `WordUnitRec` | struct | `micro/neural-tts/include/neural_tts/pack_format.h:120` | `` |
| `centroid` | function | `micro/neural-tts/include/neural_tts/pack_format.h:171` | `const int8_t* centroid(int type_idx) const` |
| `codebook` | function | `micro/neural-tts/include/neural_tts/pack_format.h:155` | `const int8_t* codebook(int s) const` |
| `codebook_scale` | function | `micro/neural-tts/include/neural_tts/pack_format.h:158` | `const float* codebook_scale(int s) const` |
| `codes` | function | `micro/neural-tts/include/neural_tts/pack_format.h:175` | `const uint8_t* codes(uint32_t off) const` |
| `dtypes` | function | `micro/neural-tts/include/neural_tts/pack_format.h:161` | `const DiphoneTypeRec* dtypes() const` |
| `dunits` | function | `micro/neural-tts/include/neural_tts/pack_format.h:164` | `const DiphoneUnitRec* dunits() const` |
| `dur_ratio` | function | `micro/neural-tts/include/neural_tts/pack_format.h:184` | `const float* dur_ratio() const` |
| `f0_stream` | function | `micro/neural-tts/include/neural_tts/pack_format.h:178` | `const uint8_t* f0_stream(uint32_t off) const` |
| `func_blob` | function | `micro/neural-tts/include/neural_tts/pack_format.h:191` | `const uint8_t* func_blob() const` |
| `func_idx` | function | `micro/neural-tts/include/neural_tts/pack_format.h:188` | `const uint16_t* func_idx() const` |
| `h` | function | `micro/neural-tts/include/neural_tts/pack_format.h:151` | `const PackHeader& h() const` |
| `model` | function | `micro/neural-tts/include/neural_tts/pack_format.h:154` | `const unsigned char* model() const` |
| `ok` | function | `micro/neural-tts/include/neural_tts/pack_format.h:147` | `bool ok() const` |
| `phone_class` | function | `micro/neural-tts/include/neural_tts/pack_format.h:187` | `const uint8_t* phone_class() const` |
| `phone_token` | function | `micro/neural-tts/include/neural_tts/pack_format.h:181` | `const char* phone_token(int id) const` |
| `raw` | function | `micro/neural-tts/include/neural_tts/pack_format.h:152` | `const uint8_t* raw(uint32_t off) const` |
| `wkeys` | function | `micro/neural-tts/include/neural_tts/pack_format.h:170` | `const uint8_t* wkeys() const` |
| `wunits` | function | `micro/neural-tts/include/neural_tts/pack_format.h:167` | `const WordUnitRec* wunits() const` |
| `BeginUtterance` | function | `micro/neural-tts/include/neural_tts/pb_decoder.h:58` | `void BeginUtterance(const PbCodedUtterance* utt);` |
| `Config` | struct | `micro/neural-tts/include/neural_tts/pb_decoder.h:40` | `` |
| `DecodeTileAt` | function | `micro/neural-tts/include/neural_tts/pb_decoder.h:81` | `bool DecodeTileAt(int latent_start);` |
| `GetFrame` | function | `micro/neural-tts/include/neural_tts/pb_decoder.h:62` | `void GetFrame(int t, WorldFrame* frame);` |
| `GetFrameThunk` | function | `micro/neural-tts/include/neural_tts/pb_decoder.h:61` | `static void GetFrameThunk(void* user, int t, WorldFrame* frame);` |
| `Model` | struct | `micro/neural-tts/include/neural_tts/pb_decoder.h:20` | `` |
| `NEURAL_TTS_PB_DECODER_H_` | macro | `micro/neural-tts/include/neural_tts/pb_decoder.h:11` | `#define NEURAL_TTS_PB_DECODER_H_` |
| `PbCodedUtterance` | struct | `micro/neural-tts/include/neural_tts/pb_decoder.h:31` | `` |
| `PbDecoder` | class | `micro/neural-tts/include/neural_tts/pb_decoder.h:38` | `` |
| `ReadRows` | function | `micro/neural-tts/include/neural_tts/pb_decoder.h:72` | `void ReadRows(int t0, int n, int16_t* out);` |
| `arena_used_bytes` | function | `micro/neural-tts/include/neural_tts/pb_decoder.h:56` | `size_t arena_used_bytes() const;` |
| `decode_us` | function | `micro/neural-tts/include/neural_tts/pb_decoder.h:75` | `uint64_t decode_us() const` |
| `ok` | function | `micro/neural-tts/include/neural_tts/pb_decoder.h:55` | `bool ok() const` |
| `tiles_decoded` | function | `micro/neural-tts/include/neural_tts/pb_decoder.h:76` | `int tiles_decoded() const` |
| `BinMap` | struct | `micro/neural-tts/include/neural_tts/worldlite_synth.h:92` | `` |
| `ExpandFrame` | function | `micro/neural-tts/include/neural_tts/worldlite_synth.h:98` | `void ExpandFrame(const WorldFrame& f, float* spec_pow, float* ap) const;` |
| `FftSelfTest` | function | `micro/neural-tts/include/neural_tts/worldlite_synth.h:89` | `float FftSelfTest();` |
| `FlushTo` | function | `micro/neural-tts/include/neural_tts/worldlite_synth.h:102` | `void FlushTo(int abs_pos, float gain, EmitFn emit, void* emit_user);` |
| `InitTables` | function | `micro/neural-tts/include/neural_tts/worldlite_synth.h:97` | `void InitTables();` |
| `KissFftrPairBytes` | function | `micro/neural-tts/include/neural_tts/worldlite_synth.h:46` | `inline size_t KissFftrPairBytes(int nfft)` |
| `KissFftrPlanBytes` | function | `micro/neural-tts/include/neural_tts/worldlite_synth.h:39` | `inline size_t KissFftrPlanBytes(int nfft, int inverse_fft)` |
| `MinimumPhase` | function | `micro/neural-tts/include/neural_tts/worldlite_synth.h:99` | `void MinimumPhase(const float* log_amp_half, kiss_fft_cpx* min_phase);` |
| `NEURAL_TTS_WORLDLITE_SYNTH_H_` | macro | `micro/neural-tts/include/neural_tts/worldlite_synth.h:23` | `#define NEURAL_TTS_WORLDLITE_SYNTH_H_` |
| `Randn` | function | `micro/neural-tts/include/neural_tts/worldlite_synth.h:103` | `float Randn();` |
| `RenderPulse` | function | `micro/neural-tts/include/neural_tts/worldlite_synth.h:100` | `void RenderPulse(const float* spec_pow, const float* ap, bool voiced, int noise_size, float frac_shift_s, float*...` |
| `Synthesize` | function | `micro/neural-tts/include/neural_tts/worldlite_synth.h:77` | `void Synthesize(GetFrameFn get_frame, void* frame_user, int num_frames, float gain, EmitFn emit, void* emit_user);` |
| `WorldFrame` | struct | `micro/neural-tts/include/neural_tts/worldlite_synth.h:51` | `` |
| `WorldLiteSynth` | class | `micro/neural-tts/include/neural_tts/worldlite_synth.h:57` | `` |
| `fwd_plan` | function | `micro/neural-tts/include/neural_tts/worldlite_synth.h:87` | `const void* fwd_plan() const` |
| `inv_plan` | function | `micro/neural-tts/include/neural_tts/worldlite_synth.h:88` | `const void* inv_plan() const` |
| `ok` | function | `micro/neural-tts/include/neural_tts/worldlite_synth.h:82` | `bool ok() const` |
| `AdvanceJoins` | function | `micro/neural-tts/src/neural_tts.cc:1547` | `void Engine::AdvanceJoins()` |
| `Alloc` | function | `micro/neural-tts/src/neural_tts.cc:237` | `void* Alloc(size_t bytes, size_t align = 4)` |
| `AllocArray` | function | `micro/neural-tts/src/neural_tts.cc:244` | `template <typename T>   T* AllocArray(size_t n, size_t align = 4)` |
| `BitReader` | class | `micro/neural-tts/src/neural_tts.cc:120` | `` |
| `BitReader` | function | `micro/neural-tts/src/neural_tts.cc:122` | `public:   explicit BitReader(const uint8_t* p) : p_(p)` |
| `BlendLenUnit` | function | `micro/neural-tts/src/neural_tts.cc:352` | `static int BlendLenUnit(int rule_n, int nat_n)` |
| `BuildParts` | function | `micro/neural-tts/src/neural_tts.cc:928` | `void Engine::BuildParts(int n)` |
| `BuildRanges` | function | `micro/neural-tts/src/neural_tts.cc:1167` | `int Engine::BuildRanges(const Part& p, int T, Range ranges[2]) const` |
| `BuildRuns` | function | `micro/neural-tts/src/neural_tts.cc:492` | `int Engine::BuildRuns(const std::vector<std::string>& tokens)` |
| `BuildRunsFromPtrs` | function | `micro/neural-tts/src/neural_tts.cc:447` | `int Engine::BuildRunsFromPtrs(const char* const* tokens, int n_tokens)` |
| `Bump` | class | `micro/neural-tts/src/neural_tts.cc:234` | `` |
| `Bump` | function | `micro/neural-tts/src/neural_tts.cc:236` | `public:   Bump(uint8_t* base, size_t size) : base_(base), size_(size)` |
| `Canon` | function | `micro/neural-tts/src/neural_tts.cc:299` | `int Canon(int pid) const` |

Next: [SYMBOLS_p10.md](SYMBOLS_p10.md)
