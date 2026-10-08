# Symbols (page 11 of 12)
Previous: [SYMBOLS_p10.md](SYMBOLS_p10.md)

| Symbol | Kind | File:Line | Signature |
|--------|------|-----------|-----------|
| `hash_file` | function | `python/src/moonshine_voice/download_file.py:19` | `def hash_file(path, algorithm)` |
| `MoonshineAudioOutputError` | class | `python/src/moonshine_voice/errors.py:54` | `class MoonshineAudioOutputError(MoonshineError)` |
| `MoonshineError` | class | `python/src/moonshine_voice/errors.py:6` | `class MoonshineError(Exception)` |
| `MoonshineInvalidArgumentError` | class | `python/src/moonshine_voice/errors.py:28` | `class MoonshineInvalidArgumentError(MoonshineError)` |
| `MoonshineInvalidHandleError` | class | `python/src/moonshine_voice/errors.py:21` | `class MoonshineInvalidHandleError(MoonshineError)` |
| `MoonshineTtsLanguageError` | class | `python/src/moonshine_voice/errors.py:35` | `class MoonshineTtsLanguageError(MoonshineInvalidArgumentError)` |
| `MoonshineTtsVoiceError` | class | `python/src/moonshine_voice/errors.py:72` | `class MoonshineTtsVoiceError(MoonshineInvalidArgumentError)` |
| `MoonshineUnknownError` | class | `python/src/moonshine_voice/errors.py:14` | `class MoonshineUnknownError(MoonshineError)` |
| `__init__` | method | `python/src/moonshine_voice/errors.py:9` | `def __init__(self, message, error_code)` |
| `__init__` | method | `python/src/moonshine_voice/errors.py:17` | `def __init__(self, message)` |
| `__init__` | method | `python/src/moonshine_voice/errors.py:24` | `def __init__(self, message)` |
| `__init__` | method | `python/src/moonshine_voice/errors.py:31` | `def __init__(self, message)` |
| `__init__` | method | `python/src/moonshine_voice/errors.py:38` | `def __init__(self, language, alternatives, message)` |
| `__init__` | method | `python/src/moonshine_voice/errors.py:57` | `def __init__(self, message)` |
| `__init__` | method | `python/src/moonshine_voice/errors.py:81` | `def __init__(self, voice, language, alternatives)` |
| `check_error` | method | `python/src/moonshine_voice/errors.py:107` | `def check_error(error_code)` |
| `GraphemeToPhonemizer` | class | `python/src/moonshine_voice/g2p.py:24` | `class GraphemeToPhonemizer` |
| `__del__` | method | `python/src/moonshine_voice/g2p.py:111` | `def __del__(self)` |
| `__enter__` | method | `python/src/moonshine_voice/g2p.py:105` | `def __enter__(self)` |
| `__exit__` | method | `python/src/moonshine_voice/g2p.py:108` | `def __exit__(self, exc_type, exc, tb)` |
| `__init__` | method | `python/src/moonshine_voice/g2p.py:30` | `def __init__(self, language)` |
| `asset_root` | method | `python/src/moonshine_voice/g2p.py:89` | `def asset_root(self)` |
| `close` | method | `python/src/moonshine_voice/g2p.py:100` | `def close(self)` |
| `language` | method | `python/src/moonshine_voice/g2p.py:85` | `def language(self)` |
| `main` | method | `python/src/moonshine_voice/g2p.py:118` | `def main()` |
| `to_ipa` | method | `python/src/moonshine_voice/g2p.py:92` | `def to_ipa(self, text, options)` |
| `IntentMatch` | class | `python/src/moonshine_voice/intent_recognizer.py:29` | `class IntentMatch` |
| `IntentRecognizer` | class | `python/src/moonshine_voice/intent_recognizer.py:42` | `class IntentRecognizer(TranscriptEventListener)` |
| `TranscriptPrinter` | class | `python/src/moonshine_voice/intent_recognizer.py:561` | `class TranscriptPrinter(TranscriptEventListener)` |
| `__del__` | method | `python/src/moonshine_voice/intent_recognizer.py:206` | `def __del__(self)` |
| `__enter__` | method | `python/src/moonshine_voice/intent_recognizer.py:191` | `def __enter__(self)` |
| `__exit__` | method | `python/src/moonshine_voice/intent_recognizer.py:195` | `def __exit__(self, exc_type, exc_val, exc_tb)` |
| `__init__` | method | `python/src/moonshine_voice/intent_recognizer.py:61` | `def __init__(self, model_path, model_arch, model_variant, threshold)` |
| `__init__` | method | `python/src/moonshine_voice/intent_recognizer.py:564` | `def __init__(self)` |
| `_setup_function_signatures` | method | `python/src/moonshine_voice/intent_recognizer.py:109` | `def _setup_function_signatures(self)` |
| `calculate_embedding` | method | `python/src/moonshine_voice/intent_recognizer.py:385` | `def calculate_embedding(self, sentence)` |
| `clear_intents` | method | `python/src/moonshine_voice/intent_recognizer.py:377` | `def clear_intents(self)` |
| `close` | method | `python/src/moonshine_voice/intent_recognizer.py:199` | `def close(self)` |
| `distance` | method | `python/src/moonshine_voice/intent_recognizer.py:421` | `def distance(self, embedding_a, embedding_b)` |
| `get_closest_intents` | method | `python/src/moonshine_voice/intent_recognizer.py:274` | `def get_closest_intents(self, utterance, tolerance_threshold)` |
| `intent_count` | method | `python/src/moonshine_voice/intent_recognizer.py:368` | `def intent_count(self)` |
| `on_error` | method | `python/src/moonshine_voice/intent_recognizer.py:485` | `def on_error(self, event)` |
| `on_intent_triggered_on` | method | `python/src/moonshine_voice/intent_recognizer.py:555` | `def on_intent_triggered_on(trigger, utterance, similarity)` |
| `on_line_completed` | method | `python/src/moonshine_voice/intent_recognizer.py:469` | `def on_line_completed(self, event)` |
| `on_line_completed` | method | `python/src/moonshine_voice/intent_recognizer.py:580` | `def on_line_completed(self, event)` |
| `on_line_started` | method | `python/src/moonshine_voice/intent_recognizer.py:574` | `def on_line_started(self, event)` |
| `on_line_text_changed` | method | `python/src/moonshine_voice/intent_recognizer.py:577` | `def on_line_text_changed(self, event)` |
| `process_utterance` | method | `python/src/moonshine_voice/intent_recognizer.py:331` | `def process_utterance(self, utterance)` |
| `register_intent` | method | `python/src/moonshine_voice/intent_recognizer.py:211` | `def register_intent(self, trigger_phrase, handler)` |
| `set_on_intent` | method | `python/src/moonshine_voice/intent_recognizer.py:454` | `def set_on_intent(self, callback)` |
| `threshold` | method | `python/src/moonshine_voice/intent_recognizer.py:358` | `def threshold(self)` |
| `threshold` | method | `python/src/moonshine_voice/intent_recognizer.py:363` | `def threshold(self, value)` |
| `trigger_phrase` | method | `python/src/moonshine_voice/intent_recognizer.py:37` | `def trigger_phrase(self)` |
| `unregister_intent` | method | `python/src/moonshine_voice/intent_recognizer.py:253` | `def unregister_intent(self, trigger_phrase)` |
| `update_last_terminal_line` | method | `python/src/moonshine_voice/intent_recognizer.py:567` | `def update_last_terminal_line(self, new_text)` |
| `FileListener` | class | `python/src/moonshine_voice/mic_transcriber.py:319` | `class FileListener(TranscriptEventListener)` |
| `MicTranscriber` | class | `python/src/moonshine_voice/mic_transcriber.py:19` | `class MicTranscriber` |
| `TerminalListener` | class | `python/src/moonshine_voice/mic_transcriber.py:280` | `class TerminalListener(TranscriptEventListener)` |
| `__init__` | method | `python/src/moonshine_voice/mic_transcriber.py:22` | `def __init__(self, model_path, model_arch, update_interval, device, samplerate, channels, blocksize, options...` |
| `__init__` | method | `python/src/moonshine_voice/mic_transcriber.py:281` | `def __init__(self)` |
| `_add_batch` | method | `python/src/moonshine_voice/mic_transcriber.py:163` | `def _add_batch(self, batch)` |
| `_add_run` | method | `python/src/moonshine_voice/mic_transcriber.py:176` | `def _add_run(self, chunks, sample_rate)` |
| `_open_input_stream` | method | `python/src/moonshine_voice/mic_transcriber.py:78` | `def _open_input_stream(self, samplerate, callback)` |
| `_process_audio_queue` | method | `python/src/moonshine_voice/mic_transcriber.py:128` | `def _process_audio_queue(self)` |
| `_query_device_default_samplerate` | method | `python/src/moonshine_voice/mic_transcriber.py:60` | `def _query_device_default_samplerate(self)` |
| `_start_listening` | method | `python/src/moonshine_voice/mic_transcriber.py:89` | `def _start_listening(self)` |
| `_start_worker` | method | `python/src/moonshine_voice/mic_transcriber.py:186` | `def _start_worker(self)` |
| `_stop_worker` | method | `python/src/moonshine_voice/mic_transcriber.py:195` | `def _stop_worker(self)` |
| `add_listener` | method | `python/src/moonshine_voice/mic_transcriber.py:236` | `def add_listener(self, listener)` |
| `audio_callback` | method | `python/src/moonshine_voice/mic_transcriber.py:95` | `def audio_callback(in_data, frames, time, status)` |
| `close` | method | `python/src/moonshine_voice/mic_transcriber.py:216` | `def close(self)` |
| `on_line_completed` | method | `python/src/moonshine_voice/mic_transcriber.py:314` | `def on_line_completed(self, event)` |
| `on_line_completed` | method | `python/src/moonshine_voice/mic_transcriber.py:320` | `def on_line_completed(self, event)` |
| `on_line_started` | method | `python/src/moonshine_voice/mic_transcriber.py:308` | `def on_line_started(self, event)` |
| `on_line_text_changed` | method | `python/src/moonshine_voice/mic_transcriber.py:311` | `def on_line_text_changed(self, event)` |
| `pop_all_listeners` | method | `python/src/moonshine_voice/mic_transcriber.py:253` | `def pop_all_listeners(self)` |
| `pop_listener` | method | `python/src/moonshine_voice/mic_transcriber.py:249` | `def pop_listener(self)` |
| `push_listener` | method | `python/src/moonshine_voice/mic_transcriber.py:245` | `def push_listener(self, listener)` |
| `remove_all_listeners` | method | `python/src/moonshine_voice/mic_transcriber.py:242` | `def remove_all_listeners(self)` |
| `remove_listener` | method | `python/src/moonshine_voice/mic_transcriber.py:239` | `def remove_listener(self, listener)` |
| `set_transcribe_flags` | method | `python/src/moonshine_voice/mic_transcriber.py:227` | `def set_transcribe_flags(self, flags)` |
| `start` | method | `python/src/moonshine_voice/mic_transcriber.py:202` | `def start(self)` |
| `stop` | method | `python/src/moonshine_voice/mic_transcriber.py:209` | `def stop(self)` |
| `transcribe_flags` | method | `python/src/moonshine_voice/mic_transcriber.py:223` | `def transcribe_flags(self)` |
| `update_last_terminal_line` | method | `python/src/moonshine_voice/mic_transcriber.py:286` | `def update_last_terminal_line(self, line)` |
| `ModelArch` | class | `python/src/moonshine_voice/moonshine_api.py:188` | `class ModelArch(IntEnum)` |
| `MoonshineIntentMatchC` | class | `python/src/moonshine_voice/moonshine_api.py:179` | `class MoonshineIntentMatchC(Structure)` |
| `SpeakerSpan` | class | `python/src/moonshine_voice/moonshine_api.py:249` | `class SpeakerSpan` |
| `SpeakerSpanC` | class | `python/src/moonshine_voice/moonshine_api.py:85` | `class SpeakerSpanC(Structure)` |
| `TranscriberOptionC` | class | `python/src/moonshine_voice/moonshine_api.py:166` | `class TranscriberOptionC(Structure)` |
| `Transcript` | class | `python/src/moonshine_voice/moonshine_api.py:312` | `class Transcript` |
| `TranscriptC` | class | `python/src/moonshine_voice/moonshine_api.py:121` | `class TranscriptC(Structure)` |
| `TranscriptLine` | class | `python/src/moonshine_voice/moonshine_api.py:285` | `class TranscriptLine` |
| `TranscriptLineC` | class | `python/src/moonshine_voice/moonshine_api.py:98` | `class TranscriptLineC(Structure)` |
| `TranscriptWordC` | class | `python/src/moonshine_voice/moonshine_api.py:74` | `class TranscriptWordC(Structure)` |
| `WordTiming` | class | `python/src/moonshine_voice/moonshine_api.py:236` | `class WordTiming` |
| `_MoonshineLib` | class | `python/src/moonshine_voice/moonshine_api.py:583` | `class _MoonshineLib` |
| `__new__` | method | `python/src/moonshine_voice/moonshine_api.py:589` | `def __new__(cls)` |
| `__str__` | method | `python/src/moonshine_voice/moonshine_api.py:244` | `def __str__(self)` |
| `__str__` | method | `python/src/moonshine_voice/moonshine_api.py:272` | `def __str__(self)` |
| `__str__` | method | `python/src/moonshine_voice/moonshine_api.py:302` | `def __str__(self)` |
| `__str__` | method | `python/src/moonshine_voice/moonshine_api.py:317` | `def __str__(self)` |
| `_decode_utf8_from_c` | function | `python/src/moonshine_voice/moonshine_api.py:34` | `def _decode_utf8_from_c(buf)` |
| `_get_libc` | function | `python/src/moonshine_voice/moonshine_api.py:56` | `def _get_libc()` |
| `_load_libc` | function | `python/src/moonshine_voice/moonshine_api.py:42` | `def _load_libc()` |
| `_load_library` | method | `python/src/moonshine_voice/moonshine_api.py:595` | `def _load_library(self)` |
| `_require_struct_size` | method | `python/src/moonshine_voice/moonshine_api.py:130` | `def _require_struct_size(name, struct, expected, note)` |
| `_setup_function_signatures` | method | `python/src/moonshine_voice/moonshine_api.py:642` | `def _setup_function_signatures(self)` |
| `lib` | method | `python/src/moonshine_voice/moonshine_api.py:888` | `def lib(self)` |
| `model_arch_to_string` | method | `python/src/moonshine_voice/moonshine_api.py:199` | `def model_arch_to_string(model_arch)` |
| `moonshine_c_string_array` | method | `python/src/moonshine_voice/moonshine_api.py:339` | `def moonshine_c_string_array(strings)` |
| `moonshine_free` | function | `python/src/moonshine_voice/moonshine_api.py:65` | `def moonshine_free(address)` |
| `moonshine_get_g2p_dependencies_string` | method | `python/src/moonshine_voice/moonshine_api.py:373` | `def moonshine_get_g2p_dependencies_string(languages, options)` |
| `moonshine_get_tts_dependencies_string` | method | `python/src/moonshine_voice/moonshine_api.py:398` | `def moonshine_get_tts_dependencies_string(languages, options)` |
| `moonshine_get_tts_voices_string` | method | `python/src/moonshine_voice/moonshine_api.py:452` | `def moonshine_get_tts_voices_string(languages, options)` |
| `moonshine_memory_arrays` | method | `python/src/moonshine_voice/moonshine_api.py:348` | `def moonshine_memory_arrays(buffers)` |
| `moonshine_options_array` | method | `python/src/moonshine_voice/moonshine_api.py:322` | `def moonshine_options_array(options)` |
| `moonshine_phonemes_to_speech_samples` | method | `python/src/moonshine_voice/moonshine_api.py:505` | `def moonshine_phonemes_to_speech_samples(tts_synthesizer_handle, phonemes, options)` |
| `moonshine_text_to_phonemes_string` | method | `python/src/moonshine_voice/moonshine_api.py:546` | `def moonshine_text_to_phonemes_string(grapheme_to_phonemizer_handle, text, options)` |
| `moonshine_text_to_speech_samples` | method | `python/src/moonshine_voice/moonshine_api.py:468` | `def moonshine_text_to_speech_samples(tts_synthesizer_handle, text, options)` |
| `moonshine_try_get_tts_voices` | method | `python/src/moonshine_voice/moonshine_api.py:423` | `def moonshine_try_get_tts_voices(languages, options)` |
| `string_to_model_arch` | method | `python/src/moonshine_voice/moonshine_api.py:217` | `def string_to_model_arch(model_arch_string)` |
| `TextToSpeech` | class | `python/src/moonshine_voice/tts.py:453` | `class TextToSpeech` |
| `_BeepRequest` | class | `python/src/moonshine_voice/tts.py:51` | `class _BeepRequest` |
| `_PlayItem` | class | `python/src/moonshine_voice/tts.py:43` | `class _PlayItem` |
| `_SayRequest` | class | `python/src/moonshine_voice/tts.py:33` | `class _SayRequest` |
| `__del__` | method | `python/src/moonshine_voice/tts.py:1326` | `def __del__(self)` |
| `__enter__` | method | `python/src/moonshine_voice/tts.py:1320` | `def __enter__(self)` |
| `__exit__` | method | `python/src/moonshine_voice/tts.py:1323` | `def __exit__(self, exc_type, exc, tb)` |
| `__init__` | method | `python/src/moonshine_voice/tts.py:477` | `def __init__(self, language)` |
| `_announce_resolved_device` | method | `python/src/moonshine_voice/tts.py:734` | `def _announce_resolved_device(self, sd, resolved)` |
| `_autotranscribe_clone_pcm` | method | `python/src/moonshine_voice/tts.py:389` | `def _autotranscribe_clone_pcm(pcm, sample_rate)` |
| `_c_options_for_create` | method | `python/src/moonshine_voice/tts.py:819` | `def _c_options_for_create(self)` |
| `_ensure_say_workers` | method | `python/src/moonshine_voice/tts.py:987` | `def _ensure_say_workers(self)` |
| `_import_say_audio_deps` | method | `python/src/moonshine_voice/tts.py:116` | `def _import_say_audio_deps()` |
| `_init_playback_state` | method | `python/src/moonshine_voice/tts.py:604` | `def _init_playback_state(self, output_device, volume, debug)` |
| `_init_zipvoice_from_clone` | method | `python/src/moonshine_voice/tts.py:636` | `def _init_zipvoice_from_clone(self, language)` |
| `_load_beep_samples` | method | `python/src/moonshine_voice/tts.py:88` | `def _load_beep_samples(np, kind)` |
| `_log` | method | `python/src/moonshine_voice/tts.py:793` | `def _log(self, msg)` |
| `_normalize_clone_argument` | method | `python/src/moonshine_voice/tts.py:360` | `def _normalize_clone_argument(clone)` |
| `_parse_options_cli` | method | `python/src/moonshine_voice/tts.py:1333` | `def _parse_options_cli(pairs)` |
| `_play_one` | method | `python/src/moonshine_voice/tts.py:1097` | `def _play_one(self, item, sd, np)` |
| `_play_worker` | method | `python/src/moonshine_voice/tts.py:1069` | `def _play_worker(self)` |
| `_resample_linear` | method | `python/src/moonshine_voice/tts.py:339` | `def _resample_linear(np, samples, source_sr, target_sr)` |
| `_resolve_default_output_index` | method | `python/src/moonshine_voice/tts.py:129` | `def _resolve_default_output_index(sd)` |
| `_say_device_lines` | method | `python/src/moonshine_voice/tts.py:241` | `def _say_device_lines(outs)` |
| `_say_device_spec_key` | method | `python/src/moonshine_voice/tts.py:245` | `def _say_device_spec_key(device)` |
| `_say_enumerate_output_devices` | method | `python/src/moonshine_voice/tts.py:219` | `def _say_enumerate_output_devices(sd)` |
| `_say_resolve_output_index` | method | `python/src/moonshine_voice/tts.py:423` | `def _say_resolve_output_index(spec_key, outs)` |
| `_select_output_sample_rate` | method | `python/src/moonshine_voice/tts.py:270` | `def _select_output_sample_rate(sd)` |
| `_synth_worker` | method | `python/src/moonshine_voice/tts.py:1005` | `def _synth_worker(self)` |
| `_synthesize_one` | method | `python/src/moonshine_voice/tts.py:1060` | `def _synthesize_one(self, req, np)` |
| `_try` | method | `python/src/moonshine_voice/tts.py:295` | `def _try(sr)` |
| `_write_wav_mono_pcm16` | method | `python/src/moonshine_voice/tts.py:1356` | `def _write_wav_mono_pcm16(path, samples, sample_rate_hz)` |
| `asset_root` | method | `python/src/moonshine_voice/tts.py:832` | `def asset_root(self)` |
| `close` | method | `python/src/moonshine_voice/tts.py:1288` | `def close(self)` |
| `is_talking` | method | `python/src/moonshine_voice/tts.py:1242` | `def is_talking(self)` |
| `language` | method | `python/src/moonshine_voice/tts.py:828` | `def language(self)` |
| `list_output_devices` | method | `python/src/moonshine_voice/tts.py:163` | `def list_output_devices()` |
| `play_error` | method | `python/src/moonshine_voice/tts.py:928` | `def play_error(self)` |
| `play_success` | method | `python/src/moonshine_voice/tts.py:962` | `def play_success(self)` |
| `say` | method | `python/src/moonshine_voice/tts.py:883` | `def say(self, text)` |
| `stop` | method | `python/src/moonshine_voice/tts.py:1260` | `def stop(self)` |
| `synthesize` | method | `python/src/moonshine_voice/tts.py:835` | `def synthesize(self, text)` |
| `synthesize_from_phonemes` | method | `python/src/moonshine_voice/tts.py:856` | `def synthesize_from_phonemes(self, phonemes)` |
| `wait` | method | `python/src/moonshine_voice/tts.py:1255` | `def wait(self)` |
| `get_assets_path` | function | `python/src/moonshine_voice/utils.py:9` | `def get_assets_path()` |
| `get_model_path` | function | `python/src/moonshine_voice/utils.py:27` | `def get_model_path(model_name)` |
| `load_wav_file` | function | `python/src/moonshine_voice/utils.py:47` | `def load_wav_file(file_path)` |
| `console_script` | function | `python/tests/test_cli.py:24` | `def console_script(name)` |
| `describe` | function | `python/tests/test_cli.py:49` | `def describe(result)` |
| `run` | function | `python/tests/test_cli.py:40` | `def run()` |
| `test_console_scripts_are_installed` | function | `python/tests/test_cli.py:58` | `def test_console_scripts_are_installed(name)` |
| `test_help_lists_every_command` | function | `python/tests/test_cli.py:65` | `def test_help_lists_every_command()` |
| `test_subcommand_help_parses` | function | `python/tests/test_cli.py:84` | `def test_subcommand_help_parses(command)` |
| `test_unknown_command_is_a_usage_error` | function | `python/tests/test_cli.py:78` | `def test_unknown_command_is_a_usage_error()` |
| `test_version_reports_package_name` | function | `python/tests/test_cli.py:72` | `def test_version_reports_package_name()` |
| `DocBlock` | class | `python/tests/test_docs.py:60` | `class DocBlock` |
| `check_python_syntax` | method | `python/tests/test_docs.py:158` | `def check_python_syntax(block)` |
| `collect_all_blocks` | method | `python/tests/test_docs.py:130` | `def collect_all_blocks()` |
| `describe` | method | `python/tests/test_docs.py:171` | `def describe(result)` |
| `extract_blocks` | method | `python/tests/test_docs.py:84` | `def extract_blocks(path)` |
| `parse_annotation` | method | `python/tests/test_docs.py:73` | `def parse_annotation(line)` |
| `resolve_mode` | method | `python/tests/test_docs.py:120` | `def resolve_mode(language, annotation)` |
| `run_bash_block` | method | `python/tests/test_docs.py:137` | `def run_bash_block(block, cwd, timeout)` |
| `test_doc_block` | method | `python/tests/test_docs.py:185` | `def test_doc_block(block, tmp_path)` |
| `test_id` | method | `python/tests/test_docs.py:68` | `def test_id(self)` |
| `FakeInputStream` | class | `python/tests/test_mic_transcriber_threading.py:116` | `class FakeInputStream` |
| `FakeStream` | class | `python/tests/test_mic_transcriber_threading.py:47` | `class FakeStream` |
| `FakeTranscriber` | class | `python/tests/test_mic_transcriber_threading.py:102` | `class FakeTranscriber` |
| `__init__` | method | `python/tests/test_mic_transcriber_threading.py:55` | `def __init__(self, update_interval)` |
| `__init__` | method | `python/tests/test_mic_transcriber_threading.py:105` | `def __init__(self)` |
| `__init__` | method | `python/tests/test_mic_transcriber_threading.py:125` | `def __init__(self, samplerate, blocksize, device, channels, dtype, callback)` |
| `_feed` | method | `python/tests/test_mic_transcriber_threading.py:145` | `def _feed(self)` |
| `_run_update` | method | `python/tests/test_mic_transcriber_threading.py:97` | `def _run_update(self)` |
| `add_audio` | method | `python/tests/test_mic_transcriber_threading.py:88` | `def add_audio(self, audio_data, sample_rate)` |
| `add_listener` | method | `python/tests/test_mic_transcriber_threading.py:79` | `def add_listener(self, listener)` |
| `close` | method | `python/tests/test_mic_transcriber_threading.py:73` | `def close(self)` |
| `close` | method | `python/tests/test_mic_transcriber_threading.py:112` | `def close(self)` |
| `close` | method | `python/tests/test_mic_transcriber_threading.py:142` | `def close(self)` |
| `create_stream` | method | `python/tests/test_mic_transcriber_threading.py:108` | `def create_stream(self, update_interval, flags, transcribe_flags)` |
| `remove_all_listeners` | method | `python/tests/test_mic_transcriber_threading.py:85` | `def remove_all_listeners(self)` |
| `remove_listener` | method | `python/tests/test_mic_transcriber_threading.py:82` | `def remove_listener(self, listener)` |
| `set_transcribe_flags` | method | `python/tests/test_mic_transcriber_threading.py:76` | `def set_transcribe_flags(self, flags)` |
| `start` | method | `python/tests/test_mic_transcriber_threading.py:66` | `def start(self)` |
| `start` | method | `python/tests/test_mic_transcriber_threading.py:135` | `def start(self)` |
| `stop` | method | `python/tests/test_mic_transcriber_threading.py:69` | `def stop(self)` |
| `stop` | method | `python/tests/test_mic_transcriber_threading.py:139` | `def stop(self)` |
| `test_capture_callback_is_not_blocked_by_transcription` | method | `python/tests/test_mic_transcriber_threading.py:165` | `def test_capture_callback_is_not_blocked_by_transcription(monkeypatch)` |
| `assets_path` | function | `python/tests/test_modules.py:47` | `def assets_path()` |
| `describe` | function | `python/tests/test_modules.py:39` | `def describe(result)` |
| `run_module` | function | `python/tests/test_modules.py:29` | `def run_module(module)` |
| `test_dialog_flow_lists_output_devices` | function | `python/tests/test_modules.py:150` | `def test_dialog_flow_lists_output_devices()` |
| `test_diarization_finds_two_speakers_on_endgame_clip` | function | `python/tests/test_modules.py:62` | `def test_diarization_finds_two_speakers_on_endgame_clip()` |
| `test_download_g2p_assets` | function | `python/tests/test_modules.py:143` | `def test_download_g2p_assets()` |
| `test_g2p_prints_ipa` | function | `python/tests/test_modules.py:124` | `def test_g2p_prints_ipa()` |
| `test_intent_recognizer_triggers_intents` | function | `python/tests/test_modules.py:130` | `def test_intent_recognizer_triggers_intents()` |
| `test_mic_module_arguments_parse` | function | `python/tests/test_modules.py:162` | `def test_mic_module_arguments_parse(module, args)` |
| `test_transcriber_transcribes_bundled_audio` | function | `python/tests/test_modules.py:52` | `def test_transcriber_transcribes_bundled_audio()` |
| `test_tts_synthesizes_wav` | function | `python/tests/test_modules.py:109` | `def test_tts_synthesizes_wav(tmp_path)` |
| `classify_phoneme` | function | `scripts/analyze_ko_phoneme_patterns.py:82` | `def classify_phoneme(ch)` |
| `extract_substitution_patterns` | function | `scripts/analyze_ko_phoneme_patterns.py:63` | `def extract_substitution_patterns(ops, context_size)` |
| `levenshtein_alignment` | function | `scripts/analyze_ko_phoneme_patterns.py:29` | `def levenshtein_alignment(s, t)` |
| `main` | function | `scripts/analyze_ko_phoneme_patterns.py:98` | `def main()` |
| `analyze_stress_position_type` | function | `scripts/analyze_ko_stress.py:140` | `def analyze_stress_position_type(ipa)` |
| `count_hangul_syllables` | function | `scripts/analyze_ko_stress.py:77` | `def count_hangul_syllables(word)` |
| `extract_stress_pattern` | function | `scripts/analyze_ko_stress.py:104` | `def extract_stress_pattern(ipa, num_syllables)` |
| `extract_stress_positions` | function | `scripts/analyze_ko_stress.py:82` | `def extract_stress_positions(ipa)` |
| `get_piper_ipa` | function | `scripts/analyze_ko_stress.py:188` | `def get_piper_ipa(phonemizer, word)` |
| `main` | function | `scripts/analyze_ko_stress.py:198` | `def main()` |
| `phonemize_nfc` | function | `scripts/analyze_ko_stress.py:163` | `def phonemize_nfc(self, voice, text)` |
| `setup_piper_phonemizer` | function | `scripts/analyze_ko_stress.py:158` | `def setup_piper_phonemizer()` |
| `scan` | function | `scripts/check-banned-constructs.sh:76` | `` |
| `extract_keys` | function | `scripts/check-clang-tidy.sh:60` | `` |
| `classify_char` | function | `scripts/compare_ko_phonemes.py:75` | `def classify_char(ch)` |
| `get_piper_phonemes` | function | `scripts/compare_ko_phonemes.py:28` | `def get_piper_phonemes(text, piper_voice)` |
| `levenshtein_alignment` | function | `scripts/compare_ko_phonemes.py:42` | `def levenshtein_alignment(s, t)` |
| `main` | function | `scripts/compare_ko_phonemes.py:87` | `def main()` |
| `phonemize_nfc` | function | `scripts/compare_ko_phonemes.py:136` | `def phonemize_nfc(self, voice, text)` |
| `convert_huggingface_json` | function | `scripts/convert_tokenizer.py:84` | `def convert_huggingface_json(input_path, output_path)` |
| `convert_sentencepiece` | function | `scripts/convert_tokenizer.py:51` | `def convert_sentencepiece(input_path, output_path)` |
| `main` | function | `scripts/convert_tokenizer.py:127` | `def main()` |
| `write_bin_tokenizer` | function | `scripts/convert_tokenizer.py:29` | `def write_bin_tokenizer(tokens, output_path)` |
| `folder_name_to_expected_char` | function | `scripts/eval-alphanumeric.py:46` | `def folder_name_to_expected_char(name, matcher)` |
| `main` | function | `scripts/eval-alphanumeric.py:138` | `def main()` |
| `on_event` | function | `scripts/eval-alphanumeric.py:79` | `def on_event(event)` |
| `predict_character` | function | `scripts/eval-alphanumeric.py:54` | `def predict_character(transcriber, audio, sample_rate, transcribe_flags)` |
| `print_confusion_matrix` | function | `scripts/eval-alphanumeric.py:106` | `def print_confusion_matrix(matrix, labels, title)` |
| `decode_audio` | function | `scripts/eval-librispeech.py:172` | `def decode_audio(audio_field)` |
| `detect_text_column` | function | `scripts/eval-librispeech.py:149` | `def detect_text_column(sample)` |
| `load_eval_dataset` | function | `scripts/eval-librispeech.py:158` | `def load_eval_dataset(args)` |
| `main` | function | `scripts/eval-librispeech.py:282` | `def main()` |
| `make_hf_backend` | function | `scripts/eval-librispeech.py:233` | `def make_hf_backend(args)` |
| `make_moonshine_c_backend` | function | `scripts/eval-librispeech.py:192` | `def make_moonshine_c_backend(args, streaming)` |
| `parse_args` | function | `scripts/eval-librispeech.py:87` | `def parse_args()` |
| `transcribe` | function | `scripts/eval-librispeech.py:268` | `def transcribe(audio, sample_rate)` |
| `transcribe_batch` | function | `scripts/eval-librispeech.py:211` | `def transcribe_batch(audio, sample_rate)` |
| `transcribe_streaming` | function | `scripts/eval-librispeech.py:217` | `def transcribe_streaming(audio, sample_rate)` |
| `main` | function | `scripts/export-decoder-with-attention.py:33` | `def main()` |
| `convert_to_ort` | function | `scripts/export_zipvoice_model.py:58` | `def convert_to_ort(python, onnx_path, custom_op_lib)` |
| `deploy` | function | `scripts/export_zipvoice_model.py:134` | `def deploy(src_onnx, canonical_stem)` |
| `main` | function | `scripts/export_zipvoice_model.py:72` | `def main()` |
| `run` | function | `scripts/export_zipvoice_model.py:53` | `def run(cmd, cwd)` |
| `_CloneTranscriber` | class | `scripts/export_zipvoice_voices_for_cpp.py:146` | `class _CloneTranscriber` |
| `__init__` | method | `scripts/export_zipvoice_voices_for_cpp.py:154` | `def __init__(self)` |
| `_clean_cut_index` | function | `scripts/export_zipvoice_voices_for_cpp.py:81` | `def _clean_cut_index(wav, sr, max_samples)` |
| `c_escape` | method | `scripts/export_zipvoice_voices_for_cpp.py:177` | `def c_escape(s)` |
| `close` | method | `scripts/export_zipvoice_voices_for_cpp.py:170` | `def close(self)` |
| `load_clip_pcm16` | function | `scripts/export_zipvoice_voices_for_cpp.py:127` | `def load_clip_pcm16(path)` |
| `main` | method | `scripts/export_zipvoice_voices_for_cpp.py:181` | `def main()` |
| `select_voices` | function | `scripts/export_zipvoice_voices_for_cpp.py:60` | `def select_voices(voices)` |
| `slug_from_voice_id` | function | `scripts/export_zipvoice_voices_for_cpp.py:55` | `def slug_from_voice_id(voice_id)` |
| `transcribe_pcm16` | method | `scripts/export_zipvoice_voices_for_cpp.py:165` | `def transcribe_pcm16(self, pcm)` |
| `_append_silence` | function | `scripts/generate-diarization-test-audio.py:78` | `def _append_silence(samples, sample_rate, seconds)` |
| `_synthesize_utterance` | function | `scripts/generate-diarization-test-audio.py:60` | `def _synthesize_utterance(voice, text, asset_root)` |
| `generate_dialogue_wav` | function | `scripts/generate-diarization-test-audio.py:84` | `def generate_dialogue_wav(asset_root)` |
| `main` | function | `scripts/generate-diarization-test-audio.py:97` | `def main()` |
| `convert_onnx_to_ort` | function | `scripts/generate-silero-vad-data.py:105` | `def convert_onnx_to_ort(onnx_path, out_dir, optimization)` |
| `fetch_source_onnx` | function | `scripts/generate-silero-vad-data.py:88` | `def fetch_source_onnx(dest_dir)` |
| `main` | function | `scripts/generate-silero-vad-data.py:159` | `def main()` |
| `render_header` | function | `scripts/generate-silero-vad-data.py:130` | `def render_header(data, source_name, optimization)` |
| `main` | function | `scripts/patch-release.sh:32` | `` |
| `main` | function | `scripts/prepare-release.sh:67` | `` |
| `record_failure` | function | `scripts/reliability-remote.sh:69` | `` |
| `require_tool` | function | `scripts/reliability-remote.sh:89` | `` |
| `run_fuzzer` | function | `scripts/reliability-remote.sh:439` | `` |
| `run_test` | function | `scripts/reliability-remote.sh:183` | `` |
| `WhisperListener` | class | `scripts/run-benchmarks.py:132` | `class WhisperListener(TranscriptEventListener)` |
| `__init__` | method | `scripts/run-benchmarks.py:133` | `def __init__(self)` |
| `on_line_completed` | method | `scripts/run-benchmarks.py:137` | `def on_line_completed(self, event)` |
| `log` | function | `scripts/setup-android-ci.sh:27` | `` |
| `cleanup` | function | `scripts/test-android.sh:82` | `` |
| `die` | function | `scripts/test-android.sh:38` | `` |
| `log` | function | `scripts/test-android.sh:37` | `` |
| `cleanup` | function | `scripts/test-docs.sh:31` | `` |
| `apply_local_library_overrides` | function | `scripts/test-examples.sh:299` | `` |
| `apply_local_library_overrides_ios` | function | `scripts/test-examples.sh:414` | `` |
| `cleanup` | function | `scripts/test-examples.sh:157` | `` |
| `copy_local_example_trees` | function | `scripts/test-examples.sh:230` | `` |
| `copy_local_swift_package` | function | `scripts/test-examples.sh:333` | `` |
| `die` | function | `scripts/test-examples.sh:98` | `` |
| `download_one` | function | `scripts/test-examples.sh:178` | `` |
| `download_platform_example_archives` | function | `scripts/test-examples.sh:213` | `` |
| `download_url_for` | function | `scripts/test-examples.sh:169` | `` |
| `ensure_local_swift_package` | function | `scripts/test-examples.sh:320` | `` |
| `extract_tgz` | function | `scripts/test-examples.sh:194` | `` |
| `list_example_project_names` | function | `scripts/test-examples.sh:204` | `` |
| `log` | function | `scripts/test-examples.sh:94` | `` |
| `main` | function | `scripts/test-examples.sh:552` | `` |
| `pick_xcode_scheme` | function | `scripts/test-examples.sh:430` | `` |
| `portable_sed_inplace` | function | `scripts/test-examples.sh:247` | `` |
| `publish_local_library` | function | `scripts/test-examples.sh:270` | `` |
| `read_library_version` | function | `scripts/test-examples.sh:260` | `` |
| `rewrite_pbxproj_to_local_package` | function | `scripts/test-examples.sh:346` | `` |
| `run_android_builds` | function | `scripts/test-examples.sh:474` | `` |
| `run_ios_builds` | function | `scripts/test-examples.sh:512` | `` |
| `usage` | function | `scripts/test-examples.sh:56` | `` |
| `write_local_library_init_script` | function | `scripts/test-examples.sh:279` | `` |
| `download_and_run` | function | `scripts/test-model-downloads.sh:103` | `` |
| `run_android_framework_tests` | function | `scripts/test-model-downloads.sh:223` | `` |
| `run_swift_framework_tests` | function | `scripts/test-model-downloads.sh:195` | `` |
| `cleanup` | function | `scripts/test-python.sh:28` | `` |
| `LineResult` | class | `scripts/tts_g2p_intelligibility.py:1162` | `class LineResult` |
| `VoicePair` | class | `scripts/tts_g2p_intelligibility.py:913` | `class VoicePair` |
| `_fmt_cer_percent` | method | `scripts/tts_g2p_intelligibility.py:1498` | `def _fmt_cer_percent(x)` |
| `_fmt_metric` | method | `scripts/tts_g2p_intelligibility.py:1494` | `def _fmt_metric(x)` |
| `_german_wikipedia_lead_penalty` | function | `scripts/tts_g2p_intelligibility.py:576` | `def _german_wikipedia_lead_penalty(line)` |
| `_kokoro_ja_text_for_misaki_cutlet` | method | `scripts/tts_g2p_intelligibility.py:989` | `def _kokoro_ja_text_for_misaki_cutlet(text)` |
| `_load_tts_wav_meta` | function | `scripts/tts_g2p_intelligibility.py:819` | `def _load_tts_wav_meta(meta_path)` |
| `_parse_datasets_version_tuple` | function | `scripts/tts_g2p_intelligibility.py:486` | `def _parse_datasets_version_tuple(version)` |
| `_prefers_natural_wikipedia_prose_for_tag` | function | `scripts/tts_g2p_intelligibility.py:569` | `def _prefers_natural_wikipedia_prose_for_tag(tag)` |
| `_read_nonempty_lines` | function | `scripts/tts_g2p_intelligibility.py:278` | `def _read_nonempty_lines(text)` |
| `_read_wav_int16_mono` | function | `scripts/tts_g2p_intelligibility.py:803` | `def _read_wav_int16_mono(path)` |
| `_reference_cer_from_upstream_averages` | method | `scripts/tts_g2p_intelligibility.py:1505` | `def _reference_cer_from_upstream_averages(kokoro, piper)` |
| `_save_tts_wav_meta` | function | `scripts/tts_g2p_intelligibility.py:832` | `def _save_tts_wav_meta(meta_path, phonemes)` |
| `_split_oversized_wiki_piece` | function | `scripts/tts_g2p_intelligibility.py:360` | `def _split_oversized_wiki_piece(s)` |
| `_try_read_tts_wav_cache` | function | `scripts/tts_g2p_intelligibility.py:845` | `def _try_read_tts_wav_cache(cache_root, lang, payload)` |
| `_tts_cache_key` | function | `scripts/tts_g2p_intelligibility.py:749` | `def _tts_cache_key(payload)` |
| `_tts_cache_stem` | function | `scripts/tts_g2p_intelligibility.py:778` | `def _tts_cache_stem(text, track, payload)` |
| `_tts_cache_wav_and_meta_paths` | function | `scripts/tts_g2p_intelligibility.py:785` | `def _tts_cache_wav_and_meta_paths(root, lang, stem)` |
| `_tts_sentence_prefix_for_cache` | function | `scripts/tts_g2p_intelligibility.py:766` | `def _tts_sentence_prefix_for_cache(text, max_chars)` |
| `_tts_track_to_engine_slug` | function | `scripts/tts_g2p_intelligibility.py:754` | `def _tts_track_to_engine_slug(track)` |
| `_wiki_max_graphemes_for_moonshine_tag` | function | `scripts/tts_g2p_intelligibility.py:325` | `def _wiki_max_graphemes_for_moonshine_tag(tag, base_max)` |
| `_write_tts_wav_cache` | function | `scripts/tts_g2p_intelligibility.py:872` | `def _write_tts_wav_cache(cache_root, lang, payload, samples, sample_rate, phonemes)` |
| `_write_wav_int16_mono` | function | `scripts/tts_g2p_intelligibility.py:792` | `def _write_wav_int16_mono(path, samples, sample_rate)` |
| `all_moonshine_tts_language_tags` | function | `scripts/tts_g2p_intelligibility.py:672` | `def all_moonshine_tts_language_tags()` |
| `build_upstream_kokoro_pipeline` | method | `scripts/tts_g2p_intelligibility.py:1086` | `def build_upstream_kokoro_pipeline(lang_code)` |
| `clean_wiki_text_line` | function | `scripts/tts_g2p_intelligibility.py:339` | `def clean_wiki_text_line(raw)` |
| `discover_voices` | method | `scripts/tts_g2p_intelligibility.py:918` | `def discover_voices(language, asset_root)` |
| `ensure_piper_espeak_phonemizer_uses_nfc_for_eval` | method | `scripts/tts_g2p_intelligibility.py:1023` | `def ensure_piper_espeak_phonemizer_uses_nfc_for_eval()` |
| `ensure_wiki_text_files` | function | `scripts/tts_g2p_intelligibility.py:682` | `def ensure_wiki_text_files(output_dir, languages)` |
| `fetch_lines_for_moonshine_language` | function | `scripts/tts_g2p_intelligibility.py:655` | `def fetch_lines_for_moonshine_language(lang_tag)` |
| `fetch_lines_wikipedia` | function | `scripts/tts_g2p_intelligibility.py:593` | `def fetch_lines_wikipedia(wiki_lang)` |
| `fetch_lines_wikitext2` | function | `scripts/tts_g2p_intelligibility.py:528` | `def fetch_lines_wikitext2()` |
| `flush` | method | `scripts/tts_g2p_intelligibility.py:295` | `def flush()` |
| `format_cer_summary_markdown_table` | method | `scripts/tts_g2p_intelligibility.py:1519` | `def format_cer_summary_markdown_table(languages_report)` |
| `levenshtein_distance` | function | `scripts/tts_g2p_intelligibility.py:102` | `def levenshtein_distance(s, t)` |
| `line_result_to_dict` | method | `scripts/tts_g2p_intelligibility.py:1474` | `def line_result_to_dict(r)` |
| `load_wiki_text_directory` | function | `scripts/tts_g2p_intelligibility.py:268` | `def load_wiki_text_directory(dir_path)` |
| `load_wiki_text_file` | function | `scripts/tts_g2p_intelligibility.py:288` | `def load_wiki_text_file(path)` |
| `load_wiki_texts` | function | `scripts/tts_g2p_intelligibility.py:319` | `def load_wiki_texts(path)` |
| `main` | method | `scripts/tts_g2p_intelligibility.py:1556` | `def main()` |
| `moonshine_kokoro_catalog_voice_to_package_voice` | method | `scripts/tts_g2p_intelligibility.py:995` | `def moonshine_kokoro_catalog_voice_to_package_voice(catalog_id)` |
| `moonshine_tag_to_upstream_kokoro_lang_code` | function | `scripts/tts_g2p_intelligibility.py:250` | `def moonshine_tag_to_upstream_kokoro_lang_code(tag)` |
| `moonshine_tag_to_whisper_language` | function | `scripts/tts_g2p_intelligibility.py:238` | `def moonshine_tag_to_whisper_language(tag)` |
| `moonshine_tag_to_wikipedia_lang` | function | `scripts/tts_g2p_intelligibility.py:226` | `def moonshine_tag_to_wikipedia_lang(tag)` |
| `normalize_eval_lines` | function | `scripts/tts_g2p_intelligibility.py:415` | `def normalize_eval_lines(raw_lines)` |
| `overlay_repo_tts_data_into_asset_root` | method | `scripts/tts_g2p_intelligibility.py:955` | `def overlay_repo_tts_data_into_asset_root(asset_root, tts_data_root, lang)` |
| `phonemize_nfc` | method | `scripts/tts_g2p_intelligibility.py:1041` | `def phonemize_nfc(self, voice, text)` |
| `prepare_asset_root` | method | `scripts/tts_g2p_intelligibility.py:931` | `def prepare_asset_root(language, voices, cache_root)` |
| `require_datasets_compatible_with_python` | function | `scripts/tts_g2p_intelligibility.py:506` | `def require_datasets_compatible_with_python()` |
| `resample_linear` | function | `scripts/tts_g2p_intelligibility.py:735` | `def resample_linear(samples, orig_sr, target_sr)` |
| `resolve_piper_onnx_path` | method | `scripts/tts_g2p_intelligibility.py:1074` | `def resolve_piper_onnx_path(asset_root, piper_voice_catalog_id)` |
| `run_language` | method | `scripts/tts_g2p_intelligibility.py:1197` | `def run_language(language, lines)` |
| `synthesize_upstream_kokoro_package` | method | `scripts/tts_g2p_intelligibility.py:1104` | `def synthesize_upstream_kokoro_package(pipeline, text, voice)` |
| `synthesize_upstream_piper_package` | method | `scripts/tts_g2p_intelligibility.py:1136` | `def synthesize_upstream_piper_package(piper_voice, text)` |
| `transcribe_whisper` | method | `scripts/tts_g2p_intelligibility.py:1180` | `def transcribe_whisper(model, samples, sample_rate, whisper_lang)` |
| `try_import_cer` | function | `scripts/tts_g2p_intelligibility.py:894` | `def try_import_cer()` |
| `try_import_datasets` | function | `scripts/tts_g2p_intelligibility.py:477` | `def try_import_datasets()` |
| `try_import_k_pipeline` | method | `scripts/tts_g2p_intelligibility.py:1002` | `def try_import_k_pipeline()` |
| `try_import_piper_voice` | method | `scripts/tts_g2p_intelligibility.py:1011` | `def try_import_piper_voice()` |
| `try_import_whisper_model` | function | `scripts/tts_g2p_intelligibility.py:903` | `def try_import_whisper_model()` |
| `uses_wikitext2_corpus` | function | `scripts/tts_g2p_intelligibility.py:218` | `def uses_wikitext2_corpus(tag)` |
| `wikipedia_paragraph_to_candidates` | function | `scripts/tts_g2p_intelligibility.py:446` | `def wikipedia_paragraph_to_candidates(para)` |
| `checkError` | function | `swift/Sources/MoonshineVoice/Errors.swift:40` | `` |
| `feedCapturedAudio` | function | `swift/Sources/MoonshineVoice/MicTranscriber.swift:262` | `` |
| `addAudioToStream` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:159` | `` |
| `calculateIntentEmbedding` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:838` | `` |
| `clearIntentRecognizerIntents` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:834` | `` |
| `createIntentRecognizer` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:744` | `` |
| `createStream` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:134` | `` |
| `createTtsSynthesizerFromFiles` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:305` | `` |
| `createTtsSynthesizerFromMemory` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:361` | `` |
| `errorToString` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:26` | `` |
| `freeIntentRecognizer` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:761` | `` |
| `freeStream` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:141` | `` |
| `freeTranscriber` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:93` | `` |
| `freeTtsSynthesizer` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:545` | `` |
| `getClosestIntents` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:787` | `` |
| `getG2pDependencies` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:650` | `` |
| `getIntentDependencies` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:685` | `` |
| `getIntentRecognizerIntentCount` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:826` | `` |
| `getSttDependencies` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:668` | `` |
| `getTtsDependencies` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:600` | `` |
| `getTtsVoices` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:550` | `` |
| `getVersion` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:21` | `` |
| `loadTranscriberFromFiles` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:34` | `` |
| `phonemesToSpeech` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:485` | `` |
| `registerIntentRecognizerIntent` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:765` | `` |
| `startStream` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:147` | `` |
| `stopStream` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:153` | `` |
| `textToSpeech` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:421` | `` |
| `transcribeStream` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:184` | `` |
| `transcribeWithoutStreaming` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:98` | `` |
| `unregisterIntentRecognizerIntent` | function | `swift/Sources/MoonshineVoice/MoonshineAPI.swift:775` | `` |
| `onError` | function | `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:26` | `` |
| `onError` | function | `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:36` | `` |
| `onLineCompleted` | function | `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:23` | `` |
| `onLineCompleted` | function | `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:35` | `` |
| `onLineSpeakersChanged` | function | `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:20` | `` |
| `onLineSpeakersChanged` | function | `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:34` | `` |
| `onLineStarted` | function | `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:10` | `` |
| `onLineStarted` | function | `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:31` | `` |
| `onLineTextChanged` | function | `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:16` | `` |
| `onLineTextChanged` | function | `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:33` | `` |
| `onLineUpdated` | function | `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:13` | `` |
| `onLineUpdated` | function | `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:32` | `` |
| `TranscriptionStream` | protocol | `swift/Sources/MoonshineVoice/TranscriptionStream.swift:9` | `` |
| `addAudio` | function | `swift/Sources/MoonshineVoice/TranscriptionStream.swift:13` | `` |
| `addListener` | function | `swift/Sources/MoonshineVoice/TranscriptionStream.swift:14` | `` |
| `addListener` | function | `swift/Sources/MoonshineVoice/TranscriptionStream.swift:15` | `` |
| `close` | function | `swift/Sources/MoonshineVoice/TranscriptionStream.swift:12` | `` |
| `removeAllListeners` | function | `swift/Sources/MoonshineVoice/TranscriptionStream.swift:18` | `` |
| `removeListener` | function | `swift/Sources/MoonshineVoice/TranscriptionStream.swift:16` | `` |
| `removeListener` | function | `swift/Sources/MoonshineVoice/TranscriptionStream.swift:17` | `` |
| `start` | function | `swift/Sources/MoonshineVoice/TranscriptionStream.swift:10` | `` |
| `stop` | function | `swift/Sources/MoonshineVoice/TranscriptionStream.swift:11` | `` |
| `AssetDownloaderNetworkTests` | class | `swift/Tests/MoonshineVoiceTests/AssetDownloaderNetworkTests.swift:16` | `` |
| `setUpWithError` | function | `swift/Tests/MoonshineVoiceTests/AssetDownloaderNetworkTests.swift:19` | `` |
| `tearDown` | function | `swift/Tests/MoonshineVoiceTests/AssetDownloaderNetworkTests.swift:27` | `` |
| `testDownloadsAndRunsIntentModel` | function | `swift/Tests/MoonshineVoiceTests/AssetDownloaderNetworkTests.swift:96` | `` |
| `testDownloadsAndRunsSttModel` | function | `swift/Tests/MoonshineVoiceTests/AssetDownloaderNetworkTests.swift:49` | `` |
| `testDownloadsAndRunsTtsVoice` | function | `swift/Tests/MoonshineVoiceTests/AssetDownloaderNetworkTests.swift:76` | `` |
| `AssetDownloaderTests` | class | `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:10` | `` |
| `MockURLProtocol` | class | `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:258` | `` |
| `RecordedRequest` | struct | `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:250` | `` |
| `canInit` | function | `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:285` | `` |
| `canonicalRequest` | function | `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:287` | `` |
| `record` | function | `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:237` | `` |
| `setUp` | function | `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:13` | `` |
| `startLoading` | function | `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:288` | `` |
| `stopLoading` | function | `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:306` | `` |
| `tearDown` | function | `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:22` | `` |
| `testDownloadsIntentModel` | function | `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:144` | `` |
| `testDownloadsSttModelIntoEmptyDirectory` | function | `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:93` | `` |
| `testDownloadsTtsAssetsIntoNestedPaths` | function | `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:153` | `` |
| `testHttpErrorSurfacesAsAssetDownloadError` | function | `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:177` | `` |
| `testIncludeSpellingAddsFilesForEnglish` | function | `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:122` | `` |
| `testReportsProgress` | function | `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:163` | `` |
| `testResumesFromPartialDownload` | function | `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:196` | `` |
| `testSkipsAlreadyPresentFiles` | function | `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:107` | `` |
| `IntentRecognizerTests` | class | `swift/Tests/MoonshineVoiceTests/IntentRecognizerTests.swift:5` | `` |
| `testCreateIntentRecognizer_invalidPath_throws` | function | `swift/Tests/MoonshineVoiceTests/IntentRecognizerTests.swift:7` | `` |
| `testIntentRecognizer_closestIntents_whenEmbeddingModelPresent` | function | `swift/Tests/MoonshineVoiceTests/IntentRecognizerTests.swift:21` | `` |
| `FakeStream` | class | `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift:35` | `` |
| `MicTranscriberThreadingTests` | class | `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift:21` | `` |
| `addAudio` | function | `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift:57` | `` |
| `addListener` | function | `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift:78` | `` |
| `addListener` | function | `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift:80` | `` |
| `close` | function | `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift:53` | `` |
| `removeAllListeners` | function | `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift:83` | `` |
| `removeListener` | function | `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift:81` | `` |
| `removeListener` | function | `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift:82` | `` |
| `start` | function | `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift:51` | `` |
| `stop` | function | `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift:56` | `` |
| `testCaptureCallbackIsNotBlockedByTranscription` | function | `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift:95` | `` |
| `TextToSpeechTests` | class | `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:5` | `` |
| `any` | function | `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:225` | `` |
| `testCloseIdempotent` | function | `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:296` | `` |
| `testCreateSynthesizer` | function | `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:36` | `` |
| `testCreateSynthesizerInvalidLanguage` | function | `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:56` | `` |
| `testCreateSynthesizerWithVoice` | function | `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:44` | `` |
| `testGetAudioOutputDevices` | function | `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:282` | `` |
| `testGetDependencies` | function | `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:207` | `` |
| `testGetVoices` | function | `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:194` | `` |
| `testGetVoicesListsZipVoice` | function | `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:233` | `` |
| `testSayDefaultDevice` | function | `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:169` | `` |
| `testSayMultipleCalls` | function | `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:180` | `` |
| `testSynthesizeBasic` | function | `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:68` | `` |
| `testSynthesizeLongerText` | function | `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:80` | `` |
| `testSynthesizeMultipleCalls` | function | `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:151` | `` |
| `testSynthesizeSampleRange` | function | `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:135` | `` |
| `testSynthesizeWithSpeedOption` | function | `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:115` | `` |

Next: [SYMBOLS_p12.md](SYMBOLS_p12.md)
