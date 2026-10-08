# Subsystem: micro_examples_rp2350_scripts

## micro/examples/rp2350/scripts/capture_neural_tts.py
- Doc: Capture the neural_tts_test app's USB output: logs + AUDIO frames -> wavs.
- Layer: utility
- Language: py
- Symbols:
  - `find_port` (function, line 22) `def find_port()`
  - `main` (function, line 29) `def main()`

## micro/examples/rp2350/scripts/capture_stt.py
- Doc: Capture the exact audio the on-device STT receives, over USB CDC.
- Layer: utility
- Language: py
- Symbols:
  - `_resolve_serial` (function, line 36) `def _resolve_serial(explicit, timeout)`
  - `_open_raw` (function, line 61) `def _open_raw(dev)`
  - `SerialReader` (class, line 71) `class SerialReader`
  - `_save_wav` (method, line 109) `def _save_wav(path, raw, rate)`
  - `main` (method, line 117) `def main()`
  - `__init__` (method, line 74) `def __init__(self, fd)`
  - `_fill` (method, line 78) `def _fill(self)`
  - `readline` (method, line 92) `def readline(self)`
  - `read_exact` (method, line 100) `def read_exact(self, n)`

## micro/examples/rp2350/scripts/flash.sh
- Doc: Flash a moonshine-micro moonshine_micro_echo*.uf2 to a Raspberry Pi Pico 2 (RP2350) that's been...
- Layer: utility
- Language: sh
- Symbols:
  - `find_mounted_volume` (function, line 66)
  - `usage` (function, line 78)
  - `wait_volume_writable` (function, line 227)
  - `draw_bar` (function, line 259)

## micro/examples/rp2350/scripts/generate_speaker_test_clips.py
- Doc: Embed 1 s int16 PCM clips for the I2S speaker bring-up test.
- Layer: testing
- Language: py
- Symbols:
  - `_read_pcm` (function, line 27) `def _read_pcm(path)`
  - `_write_header` (function, line 46) `def _write_header()`
  - `main` (function, line 74) `def main()`

## micro/examples/rp2350/scripts/monitor.sh
- Doc: Robust USB CDC monitor for the Pico 2 boot log.
- Layer: utility
- Language: sh
- Symbols:
  - `_wait_for_any_usbmodem` (function, line 89)
  - `_wait_for_specific_tty` (function, line 113)

## micro/examples/rp2350/scripts/tts_speak.py
- Doc: Speak text on the RP2350 firmware and save the streamed PCM as a WAV.
- Layer: utility
- Language: py
- Symbols:
  - `find_port` (function, line 36) `def find_port()`
  - `main` (function, line 44) `def main()`
  - `send_line` (function, line 71) `def send_line(s)`

## micro/examples/rp2350/scripts/usb_audio_bridge.py
- Doc: Bridge the laptop mic + speaker to the RP2350 over USB (audio peripheral sim).
- Layer: utility
- Language: py
- Symbols:
  - `_resolve_serial` (function, line 49) `def _resolve_serial(explicit, timeout)`
  - `_open_raw` (function, line 80) `def _open_raw(dev)`
  - `SerialReader` (class, line 101) `class SerialReader`
  - `main` (method, line 140) `def main()`
  - `__init__` (method, line 104) `def __init__(self, fd)`
  - `_fill` (method, line 108) `def _fill(self)`
  - `readline` (method, line 123) `def readline(self)`
  - `read_exact` (method, line 131) `def read_exact(self, n)`
  - `_dev` (method, line 163) `def _dev(arg)`
  - `save_stream` (method, line 184) `def save_stream(tag, samples, rate)`
  - `on_audio` (method, line 206) `def on_audio(indata, frames, time_info, status)`
  - `sender` (method, line 224) `def sender()`
  - `flush_mic` (method, line 260) `def flush_mic()`
  - `receiver` (method, line 268) `def receiver()`
  - `_on_signal` (method, line 404) `def _on_signal(signum, frame)`
