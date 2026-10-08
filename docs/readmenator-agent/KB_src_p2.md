# Subsystem: src (page 2 of 2)
Previous: [KB_src.md](KB_src.md)

## micro/examples/rp2350/src/test_app.h
- Doc: The embedded-clip accuracy sweep (the moonshine_micro_echo_test target): run the embedded clip...
- Layer: testing
- Language: h
- Symbols:
  - `SPELLING_TEST_APP_H_` (macro, line 9) `#define SPELLING_TEST_APP_H_`
- Imported by: `micro/examples/rp2350/src/main_test.cc`, `micro/examples/rp2350/src/test_app.cc`

## micro/examples/rp2350/src/tts_service.cc
- Doc: Flash-resident neural TTS pack (generated/neural_tts_pack.S).
- Layer: business_logic
- Language: cc
- Symbols:
  - `SetBootReport` (function, line 22) `void SetBootReport(const BootReport& report)`
  - `ReadLine` (function, line 34) `int ReadLine(char* buf, int maxlen)`
  - `EmitToUsb` (function, line 55) `void EmitToUsb(void* user, const int16_t* samples, int n)`
  - `RunTtsService` (function, line 63) `void RunTtsService(uint8_t* arena, std::size_t arena_size)`
  - `g_neural_tts_pack` (variable, line 12) `extern "C" const uint8_t g_neural_tts_pack[];`
- Depends on: `micro/examples/rp2350/src/tts_service.h`, `micro/neural-tts/include/neural_tts/neural_tts.h`

## micro/examples/rp2350/src/tts_service.h
- Doc: USB streaming text-to-speech service for the RP2350 firmware.
- Layer: business_logic
- Language: h
- Symbols:
  - `BootReport` (struct, line 32)
  - `SetBootReport` (function, line 39) `void SetBootReport(const BootReport& report);`
  - `SPELLING_TTS_SERVICE_H_` (macro, line 21) `#define SPELLING_TTS_SERVICE_H_`
- Imported by: `micro/examples/rp2350/src/main_tts.cc`, `micro/examples/rp2350/src/test_app.cc`, `micro/examples/rp2350/src/tts_service.cc`

## micro/examples/rp2350/src/usb_audio_io.cc
- Doc: ReadByteTimed: Read one byte, waiting up to ~timeout_ms.
- Layer: utility
- Language: cc
- Symbols:
  - `ReadByteTimed` (function, line 18) `int ReadByteTimed(int timeout_ms)`
  - `ReadHop` (function, line 25) `bool UsbAudioInput::ReadHop(int16_t* out, int n)`
  - `Drain` (function, line 60) `void UsbAudioInput::Drain()`
  - `Begin` (function, line 67) `void UsbAudioOutput::Begin(int sample_rate, int num_samples, const char* kind)`
  - `Write` (function, line 72) `void UsbAudioOutput::Write(const int16_t* samples, int n)`
  - `End` (function, line 76) `void UsbAudioOutput::End()`
- Depends on: `micro/examples/rp2350/src/usb_audio_io.h`

## micro/examples/rp2350/src/usb_audio_io.h
- Doc: USB CDC implementation of the AudioInput / AudioOutput interfaces: the laptop acts as the...
- Layer: utility
- Language: h
- Symbols:
  - `UsbAudioInput` (class, line 25)
  - `UsbAudioOutput` (class, line 31)
  - `SPELLING_USB_AUDIO_IO_H_` (macro, line 19) `#define SPELLING_USB_AUDIO_IO_H_`
- Depends on: `micro/examples/rp2350/src/audio_io.h`
- Imported by: `micro/examples/rp2350/src/echo_app.cc`, `micro/examples/rp2350/src/main_i2s_mic_test.cc`, `micro/examples/rp2350/src/main_wifi.cc`, `micro/examples/rp2350/src/usb_audio_io.cc`

## micro/examples/rp2350/src/wifi_app.cc
- Doc: Tok: What a recognized class label means during credential entry.
- Layer: utility
- Language: cc
- Symbols:
  - `State` (enum, line 30)
  - `Tok` (enum, line 38)
  - `State` (class, line 30)
  - `Tok` (class, line 38)
  - `DigitWord` (function, line 51) `const char* DigitWord(char c)`
  - `SymbolChar` (function, line 58) `bool SymbolChar(const char* label, char* out)`
  - `SymbolWord` (function, line 68) `const char* SymbolWord(char c)`
  - `Classify` (function, line 79) `Tok Classify(const char* label, char* out_char)`
  - `AppendSpokenForChar` (function, line 110) `void AppendSpokenForChar(char* dst, std::size_t cap, char c)`
  - `SpeakSpelled` (function, line 133) `void SpeakSpelled(const char* prefix, const char* text, AudioOutput& out,
                  Audio...`
  - `SpeakName` (function, line 147) `void SpeakName(const char* name, AudioOutput& out, AudioInput& in,
               uint8_t* arena,...`
  - `SpeakIp` (function, line 156) `void SpeakIp(AudioOutput& out, AudioInput& in, uint8_t* arena,
             std::size_t arena_size)`
  - `DoConnect` (function, line 190) `void DoConnect(const char* ssid, const char* pw, AudioOutput& out,
               AudioInput& in,...`
  - `AppendChar` (function, line 222) `std::size_t AppendChar(char* buf, std::size_t len, char c, bool* caps,
                       Aud...`
  - `ScanResultCb` (function, line 255) `int ScanResultCb(void* /*env*/, const cyw43_ev_scan_result_t* r)`
  - `ScanNetworks` (function, line 275) `void ScanNetworks(AudioInput& in)`
  - `LowerAscii` (function, line 300) `char LowerAscii(char c)`
  - `HasPrefixCi` (function, line 305) `bool HasPrefixCi(const char* name, const char* prefix, std::size_t plen)`
  - `EqualsCi` (function, line 314) `bool EqualsCi(const char* a, const char* b)`
  - `CountPrefixMatches` (function, line 323) `int CountPrefixMatches(const char* prefix, int* only_idx)`
  - `FindExactMatch` (function, line 336) `int FindExactMatch(const char* name)`
  - `AnnounceMatch` (function, line 345) `void AnnounceMatch(const char* name, char* ssid, std::size_t* ssid_len,
                   AudioO...`
  - `RunWifiAppWithIo` (function, line 359) `void RunWifiAppWithIo(AudioInput& in, AudioOutput& out)`
- Depends on: `micro/examples/rp2350/generated/audio_config.h`, `micro/examples/rp2350/generated/classes.h`, `micro/examples/rp2350/src/app_common.h`, `micro/examples/rp2350/src/audio_service.h`, `micro/examples/rp2350/src/spelling_labels.h`, `micro/examples/rp2350/src/wifi_app.h`

## micro/examples/rp2350/src/wifi_app.h
- Doc: Shared voice-driven WiFi setup state machine.
- Layer: utility
- Language: h
- Symbols:
  - `SPELLING_WIFI_APP_H_` (macro, line 15) `#define SPELLING_WIFI_APP_H_`
- Depends on: `micro/examples/rp2350/src/audio_io.h`
- Imported by: `micro/examples/rp2350/src/main_wifi.cc`, `micro/examples/rp2350/src/wifi_app.cc`, `micro/examples/rp2350/src/wifi_hardware_app.cc`

## micro/examples/rp2350/src/wifi_hardware_app.cc
- Layer: utility
- Language: cc
- Symbols:
  - `RunWifiHardwareApp` (function, line 13) `void RunWifiHardwareApp()`
- Depends on: `micro/examples/rp2350/generated/audio_config.h`, `micro/examples/rp2350/generated/vad_config.h`, `micro/examples/rp2350/src/i2s_audio_io.h`, `micro/examples/rp2350/src/i2s_audio_out.h`, `micro/examples/rp2350/src/wifi_app.h`, `micro/examples/rp2350/src/wifi_hardware_app.h`

## micro/examples/rp2350/src/wifi_hardware_app.h
- Doc: Voice-driven WiFi setup on the on-board hardware audio I/O (I2S mic + I2S amp) instead of the...
- Layer: utility
- Language: h
- Symbols:
  - `SPELLING_WIFI_HARDWARE_APP_H_` (macro, line 10) `#define SPELLING_WIFI_HARDWARE_APP_H_`
- Imported by: `micro/examples/rp2350/src/main_wifi_hardware.cc`, `micro/examples/rp2350/src/wifi_hardware_app.cc`

