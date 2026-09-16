# Subsystem: tests

## python/tests/test_cli.py
- Layer: testing
- Language: py
- Symbols:
  - `console_script` (function, line 24) `def console_script(name)`
  - `run` (function, line 40) `def run()`
  - `describe` (function, line 49) `def describe(result)`
  - `test_console_scripts_are_installed` (function, line 58) `def test_console_scripts_are_installed(name)`
  - `test_help_lists_every_command` (function, line 65) `def test_help_lists_every_command()`
  - `test_version_reports_package_name` (function, line 72) `def test_version_reports_package_name()`
  - `test_unknown_command_is_a_usage_error` (function, line 78) `def test_unknown_command_is_a_usage_error()`
  - `test_subcommand_help_parses` (function, line 84) `def test_subcommand_help_parses(command)`
- Depends on: `python/src/moonshine_voice/cli.py`

## python/tests/test_docs.py
- Layer: testing
- Language: py
- Symbols:
  - `DocBlock` (class, line 60) `class DocBlock`
  - `parse_annotation` (method, line 73) `def parse_annotation(line)`
  - `extract_blocks` (method, line 84) `def extract_blocks(path)`
  - `resolve_mode` (method, line 120) `def resolve_mode(language, annotation)`
  - `collect_all_blocks` (method, line 130) `def collect_all_blocks()`
  - `run_bash_block` (method, line 137) `def run_bash_block(block, cwd, timeout)`
  - `check_python_syntax` (method, line 158) `def check_python_syntax(block)`
  - `describe` (method, line 171) `def describe(result)`
  - `test_doc_block` (method, line 185) `def test_doc_block(block, tmp_path)`
  - `test_id` (method, line 68) `def test_id(self)`

## python/tests/test_mic_transcriber_threading.py
- Layer: testing
- Language: py
- Symbols:
  - `FakeStream` (class, line 47) `class FakeStream`
  - `FakeTranscriber` (class, line 102) `class FakeTranscriber`
  - `FakeInputStream` (class, line 116) `class FakeInputStream`
  - `test_capture_callback_is_not_blocked_by_transcription` (method, line 165) `def test_capture_callback_is_not_blocked_by_transcription(monkeypatch)`
  - `__init__` (method, line 55) `def __init__(self, update_interval)`
  - `start` (method, line 66) `def start(self)`
  - `stop` (method, line 69) `def stop(self)`
  - `close` (method, line 73) `def close(self)`
  - `set_transcribe_flags` (method, line 76) `def set_transcribe_flags(self, flags)`
  - `add_listener` (method, line 79) `def add_listener(self, listener)`
  - `remove_listener` (method, line 82) `def remove_listener(self, listener)`
  - `remove_all_listeners` (method, line 85) `def remove_all_listeners(self)`
  - `add_audio` (method, line 88) `def add_audio(self, audio_data, sample_rate)`
  - `_run_update` (method, line 97) `def _run_update(self)`
  - `__init__` (method, line 105) `def __init__(self)`
  - `create_stream` (method, line 108) `def create_stream(self, update_interval, flags, transcribe_flags)`
  - `close` (method, line 112) `def close(self)`
  - `__init__` (method, line 125) `def __init__(self, samplerate, blocksize, device, channels, dtype, callback)`
  - `start` (method, line 135) `def start(self)`
  - `stop` (method, line 139) `def stop(self)`
  - `close` (method, line 142) `def close(self)`
  - `_feed` (method, line 145) `def _feed(self)`

## python/tests/test_modules.py
- Layer: testing
- Language: py
- Symbols:
  - `run_module` (function, line 29) `def run_module(module)`
  - `describe` (function, line 39) `def describe(result)`
  - `assets_path` (function, line 47) `def assets_path()`
  - `test_transcriber_transcribes_bundled_audio` (function, line 52) `def test_transcriber_transcribes_bundled_audio()`
  - `test_diarization_finds_two_speakers_on_endgame_clip` (function, line 62) `def test_diarization_finds_two_speakers_on_endgame_clip()`
  - `test_tts_synthesizes_wav` (function, line 109) `def test_tts_synthesizes_wav(tmp_path)`
  - `test_g2p_prints_ipa` (function, line 124) `def test_g2p_prints_ipa()`
  - `test_intent_recognizer_triggers_intents` (function, line 130) `def test_intent_recognizer_triggers_intents()`
  - `test_download_g2p_assets` (function, line 143) `def test_download_g2p_assets()`
  - `test_dialog_flow_lists_output_devices` (function, line 150) `def test_dialog_flow_lists_output_devices()`
  - `test_mic_module_arguments_parse` (function, line 162) `def test_mic_module_arguments_parse(module, args)`
- Depends on: `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`
