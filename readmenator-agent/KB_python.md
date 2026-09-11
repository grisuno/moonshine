# Subsystem: python

## examples/python/basic_transcription.py
- Layer: utility
- Language: py
- Symbols:
  - `transcribe_without_streaming` (function, line 16) `def transcribe_without_streaming(transcriber, audio_data, sample_rate)`
  - `transcribe_with_streaming` (function, line 30) `def transcribe_with_streaming(transcriber, audio_data, sample_rate)`
  - `TestListener` (class, line 37) `class TestListener(TranscriptEventListener)`
  - `on_line_started` (method, line 38) `def on_line_started(self, event)`
  - `on_line_text_changed` (method, line 41) `def on_line_text_changed(self, event)`
  - `on_line_completed` (method, line 44) `def on_line_completed(self, event)`

## examples/python/dialog_flow.py
- Layer: infrastructure
- Language: py
- Symbols:
  - `setup_wifi` (function, line 46) `def setup_wifi(d)`
  - `set_timezone` (function, line 70) `def set_timezone(d)`
  - `full_onboarding` (function, line 80) `def full_onboarding(d)`
  - `_apply_wifi_config` (function, line 89) `def _apply_wifi_config(ssid, password)`
  - `TranscriptPrinter` (class, line 102) `class TranscriptPrinter(TranscriptEventListener)`
  - `run_live` (method, line 142) `def run_live(args)`
  - `run_interactive` (method, line 279) `def run_interactive(flow_name)`
  - `run_scripted` (method, line 347) `def run_scripted(flow_name, answers)`
  - `main` (method, line 411) `def main()`
  - `__init__` (method, line 112) `def __init__(self)`
  - `_overwrite` (method, line 116) `def _overwrite(self, text)`
  - `on_line_started` (method, line 122) `def on_line_started(self, event)`
  - `on_line_text_changed` (method, line 125) `def on_line_text_changed(self, event)`
  - `on_line_completed` (method, line 128) `def on_line_completed(self, event)`
  - `mute` (method, line 202) `def mute(should_mute)`
  - `set_spelling_mode` (method, line 206) `def set_spelling_mode(active)`
  - `speak` (method, line 212) `def speak(text)`
  - `speak` (method, line 293) `def speak(text)`
  - `speak` (method, line 363) `def speak(text)`

## examples/python/intent_recognition.py
- Layer: utility
- Language: py
- Symbols:
  - `on_lights_on` (function, line 26) `def on_lights_on(trigger, utterance, similarity)`
  - `on_lights_off` (function, line 31) `def on_lights_off(trigger, utterance, similarity)`
  - `on_weather` (function, line 36) `def on_weather(trigger, utterance, similarity)`
  - `on_timer` (function, line 41) `def on_timer(trigger, utterance, similarity)`
  - `on_music_play` (function, line 46) `def on_music_play(trigger, utterance, similarity)`
  - `on_music_stop` (function, line 51) `def on_music_stop(trigger, utterance, similarity)`
  - `TranscriptPrinter` (class, line 56) `class TranscriptPrinter(TranscriptEventListener)`
  - `main` (method, line 80) `def main()`
  - `__init__` (method, line 59) `def __init__(self)`
  - `update_last_terminal_line` (method, line 62) `def update_last_terminal_line(self, new_text)`
  - `on_line_started` (method, line 69) `def on_line_started(self, event)`
  - `on_line_text_changed` (method, line 72) `def on_line_text_changed(self, event)`
  - `on_line_completed` (method, line 75) `def on_line_completed(self, event)`

## examples/python/mic_transcription.py
- Layer: utility
- Language: py
- Symbols:
  - `TerminalListener` (class, line 14) `class TerminalListener(TranscriptEventListener)`
  - `FileListener` (class, line 44) `class FileListener(TranscriptEventListener)`
  - `__init__` (method, line 15) `def __init__(self)`
  - `update_last_terminal_line` (method, line 20) `def update_last_terminal_line(self, new_text)`
  - `on_line_started` (method, line 30) `def on_line_started(self, event)`
  - `on_line_text_changed` (method, line 33) `def on_line_text_changed(self, event)`
  - `on_line_completed` (method, line 36) `def on_line_completed(self, event)`
  - `on_line_completed` (method, line 45) `def on_line_completed(self, event)`
