# Subsystem: scripts

## scripts/analyze_ko_phoneme_patterns.py
- Doc: Analyze systematic phoneme pattern differences between Moonshine and Piper Korean G2P.
- Layer: utility
- Language: py
- Symbols:
  - `levenshtein_alignment` (function, line 29) `def levenshtein_alignment(s, t)`
  - `extract_substitution_patterns` (function, line 63) `def extract_substitution_patterns(ops, context_size)`
  - `classify_phoneme` (function, line 82) `def classify_phoneme(ch)`
  - `main` (function, line 98) `def main()`

## scripts/analyze_ko_stress.py
- Doc: Deep analysis of Korean stress placement: Moonshine vs Piper/eSpeak.
- Layer: utility
- Language: py
- Symbols:
  - `count_hangul_syllables` (function, line 77) `def count_hangul_syllables(word)`
  - `extract_stress_positions` (function, line 82) `def extract_stress_positions(ipa)`
  - `extract_stress_pattern` (function, line 104) `def extract_stress_pattern(ipa, num_syllables)`
  - `analyze_stress_position_type` (function, line 140) `def analyze_stress_position_type(ipa)`
  - `setup_piper_phonemizer` (function, line 158) `def setup_piper_phonemizer()`
  - `get_piper_ipa` (function, line 188) `def get_piper_ipa(phonemizer, word)`
  - `main` (function, line 198) `def main()`
  - `phonemize_nfc` (function, line 163) `def phonemize_nfc(self, voice, text)`
- Depends on: `python/src/moonshine_voice/download.py`

## scripts/check-banned-constructs.sh
- Doc: Guard against banned C++ constructs creeping into first-party core code.
- Layer: utility
- Language: sh
- Symbols:
  - `scan` (function, line 76)

## scripts/check-clang-tidy.sh
- Doc: Gate clang-tidy findings against a committed baseline so that only *newly introduced* problems...
- Layer: utility
- Language: sh
- Symbols:
  - `extract_keys` (function, line 60)

## scripts/compare_ko_phonemes.py
- Doc: Compare Moonshine vs Piper Korean phonemes directly (no TTS/Whisper needed).
- Layer: utility
- Language: py
- Symbols:
  - `get_piper_phonemes` (function, line 28) `def get_piper_phonemes(text, piper_voice)`
  - `levenshtein_alignment` (function, line 42) `def levenshtein_alignment(s, t)`
  - `classify_char` (function, line 75) `def classify_char(ch)`
  - `main` (function, line 87) `def main()`
  - `phonemize_nfc` (function, line 136) `def phonemize_nfc(self, voice, text)`
- Depends on: `python/src/moonshine_voice/download.py`

## scripts/convert_tokenizer.py
- Doc: Convert tokenizer files to the BinTokenizer format used by moonshine.
- Layer: utility
- Language: py
- Symbols:
  - `write_bin_tokenizer` (function, line 29) `def write_bin_tokenizer(tokens, output_path)`
  - `convert_sentencepiece` (function, line 51) `def convert_sentencepiece(input_path, output_path)`
  - `convert_huggingface_json` (function, line 84) `def convert_huggingface_json(input_path, output_path)`
  - `main` (function, line 127) `def main()`

## scripts/eval-alphanumeric.py
- Doc: Evaluate AlphanumericListener on the test-assets/alphanumeric dataset.
- Layer: utility
- Language: py
- Symbols:
  - `folder_name_to_expected_char` (function, line 46) `def folder_name_to_expected_char(name, matcher)`
  - `predict_character` (function, line 54) `def predict_character(transcriber, audio, sample_rate, transcribe_flags)`
  - `print_confusion_matrix` (function, line 106) `def print_confusion_matrix(matrix, labels, title)`
  - `main` (function, line 138) `def main()`
  - `on_event` (function, line 79) `def on_event(event)`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/moonshine_api.py`

## scripts/eval-librispeech.py
- Doc: Evaluate Moonshine English WER on LibriSpeech test-clean.
- Layer: utility
- Language: py
- Symbols:
  - `parse_args` (function, line 87) `def parse_args()`
  - `detect_text_column` (function, line 149) `def detect_text_column(sample)`
  - `load_eval_dataset` (function, line 158) `def load_eval_dataset(args)`
  - `decode_audio` (function, line 172) `def decode_audio(audio_field)`
  - `make_moonshine_c_backend` (function, line 192) `def make_moonshine_c_backend(args, streaming)`
  - `make_hf_backend` (function, line 233) `def make_hf_backend(args)`
  - `main` (function, line 282) `def main()`
  - `transcribe_batch` (function, line 211) `def transcribe_batch(audio, sample_rate)`
  - `transcribe_streaming` (function, line 217) `def transcribe_streaming(audio, sample_rate)`
  - `transcribe` (function, line 268) `def transcribe(audio, sample_rate)`

## scripts/eval-model-accuracy.py
- Doc: On a Mac you'll need to set up ffmpeg using: brew install ffmpeg@8 export...
- Layer: business_logic
- Language: py

## scripts/eval-speaker-id.py
- Layer: utility
- Language: py

## scripts/export-decoder-with-attention.py
- Doc: Export a decoder_with_attention model for word-level timestamps.
- Layer: utility
- Language: py
- Symbols:
  - `main` (function, line 33) `def main()`

## scripts/export_zipvoice_model.py
- Doc: Copyright 2026 Useful Sensors  Licensed under the Apache License, Version 2.0 (the "License")...
- Layer: business_logic
- Language: py
- Symbols:
  - `run` (function, line 53) `def run(cmd, cwd)`
  - `convert_to_ort` (function, line 58) `def convert_to_ort(python, onnx_path, custom_op_lib)`
  - `main` (function, line 72) `def main()`
  - `deploy` (function, line 134) `def deploy(src_onnx, canonical_stem)`

## scripts/export_zipvoice_voices_for_cpp.py
- Doc: Copyright 2026 Useful Sensors  Licensed under the Apache License, Version 2.0 (the "License")...
- Layer: utility
- Language: py
- Symbols:
  - `slug_from_voice_id` (function, line 55) `def slug_from_voice_id(voice_id)`
  - `select_voices` (function, line 60) `def select_voices(voices)`
  - `_clean_cut_index` (function, line 81) `def _clean_cut_index(wav, sr, max_samples)`
  - `load_clip_pcm16` (function, line 127) `def load_clip_pcm16(path)`
  - `_CloneTranscriber` (class, line 146) `class _CloneTranscriber`
  - `c_escape` (method, line 177) `def c_escape(s)`
  - `main` (method, line 181) `def main()`
  - `__init__` (method, line 154) `def __init__(self)`
  - `transcribe_pcm16` (method, line 165) `def transcribe_pcm16(self, pcm)`
  - `close` (method, line 170) `def close(self)`

## scripts/format-core.sh
- Doc: Format (default) or check (--check) the first-party C++ in core/ against the repo's Google-based...
- Layer: utility
- Language: sh

## scripts/generate-diarization-test-audio.py
- Doc: Copyright 2026 Moonshine AI (MIT License)
- Layer: testing
- Language: py
- Symbols:
  - `_synthesize_utterance` (function, line 60) `def _synthesize_utterance(voice, text, asset_root)`
  - `_append_silence` (function, line 78) `def _append_silence(samples, sample_rate, seconds)`
  - `generate_dialogue_wav` (function, line 84) `def generate_dialogue_wav(asset_root)`
  - `main` (function, line 97) `def main()`

## scripts/generate-silero-vad-data.py
- Doc: Regenerate core/silero-vad-model-data.h from the Silero VAD model.
- Layer: data_access
- Language: py
- Symbols:
  - `fetch_source_onnx` (function, line 88) `def fetch_source_onnx(dest_dir)`
  - `convert_onnx_to_ort` (function, line 105) `def convert_onnx_to_ort(onnx_path, out_dir, optimization)`
  - `render_header` (function, line 130) `def render_header(data, source_name, optimization)`
  - `main` (function, line 159) `def main()`

## scripts/patch-release.sh
- Doc: Fold one or more fixes into the current in-progress release by cherry-picking them onto its...
- Layer: utility
- Language: sh
- Symbols:
  - `main` (function, line 32)

## scripts/prepare-release.sh
- Doc: main: All imperative work lives inside main() so bash parses the whole script before executing...
- Layer: utility
- Language: sh
- Symbols:
  - `main` (function, line 67)

## scripts/publish-binary.sh
- Layer: utility
- Language: sh

## scripts/publish-examples.sh
- Layer: utility
- Language: sh

## scripts/publish-swift.sh
- Layer: utility
- Language: sh

## scripts/quantize-streaming-model.sh
- Layer: business_logic
- Language: sh

## scripts/reliability-remote.sh
- Doc: Runs the heavy reliability checks on a Linux x86 host with clang + libFuzzer.
- Layer: utility
- Language: sh
- Symbols:
  - `record_failure` (function, line 69)
  - `require_tool` (function, line 89)
  - `run_test` (function, line 183)
  - `run_fuzzer` (function, line 439)

## scripts/reliability.sh
- Doc: Periodic reliability driver.
- Layer: utility
- Language: sh

## scripts/run-benchmarks.py
- Doc: Benchmark to compare Moonshine and Whisper model latency in live speech scenarios.
- Layer: utility
- Language: py
- Symbols:
  - `WhisperListener` (class, line 132) `class WhisperListener(TranscriptEventListener)`
  - `__init__` (method, line 133) `def __init__(self)`
  - `on_line_completed` (method, line 137) `def on_line_completed(self, event)`

## scripts/setup-android-ci.sh
- Doc: One-time setup of the Android toolchain needed to run the moonshine-voice instrumentation tests...
- Layer: infrastructure
- Language: sh
- Symbols:
  - `log` (function, line 27)

## scripts/test-android.sh
- Doc: Run the moonshine-voice Android library's instrumentation tests on a real device or emulator...
- Layer: testing
- Language: sh
- Symbols:
  - `log` (function, line 37)
  - `die` (function, line 38)
  - `cleanup` (function, line 82)

## scripts/test-core.sh
- Layer: testing
- Language: sh

## scripts/test-docs.sh
- Doc: Tests that the code in the documentation still works, by executing the fenced code blocks in...
- Layer: testing
- Language: sh
- Symbols:
  - `cleanup` (function, line 31)

## scripts/test-examples.sh
- Doc: Verify iOS and Android examples build standalone: either from GitHub Release archives (default)...
- Layer: testing
- Language: sh
- Symbols:
  - `usage` (function, line 56)
  - `log` (function, line 94)
  - `die` (function, line 98)
  - `cleanup` (function, line 157)
  - `download_url_for` (function, line 169)
  - `download_one` (function, line 178)
  - `extract_tgz` (function, line 194)
  - `list_example_project_names` (function, line 204)
  - `download_platform_example_archives` (function, line 213)
  - `copy_local_example_trees` (function, line 230)
  - `portable_sed_inplace` (function, line 247)
  - `read_library_version` (function, line 260)
  - `publish_local_library` (function, line 270)
  - `write_local_library_init_script` (function, line 279)
  - `apply_local_library_overrides` (function, line 299)
  - `ensure_local_swift_package` (function, line 320)
  - `copy_local_swift_package` (function, line 333)
  - `rewrite_pbxproj_to_local_package` (function, line 346)
  - `apply_local_library_overrides_ios` (function, line 414)
  - `pick_xcode_scheme` (function, line 430)
  - `run_android_builds` (function, line 474)
  - `run_ios_builds` (function, line 512)
  - `main` (function, line 552)

## scripts/test-model-downloads.sh
- Doc: Download-and-run sampling tests for the native model catalog, plus the Swift and Android...
- Layer: testing
- Language: sh
- Symbols:
  - `download_and_run` (function, line 103)
  - `run_swift_framework_tests` (function, line 195)
  - `run_android_framework_tests` (function, line 223)

## scripts/test-python.sh
- Doc: Runs the Python module tests (python/tests/test_modules.py), which drive the __main__ sections...
- Layer: testing
- Language: sh
- Symbols:
  - `cleanup` (function, line 28)

## scripts/tts_g2p_intelligibility.py
- Doc: Evaluate TTS intelligibility: Moonshine synthesis (Kokoro / Piper vocoders) vs Whisper large-v3...
- Layer: utility
- Language: py
- Symbols:
  - `levenshtein_distance` (function, line 102) `def levenshtein_distance(s, t)`
  - `uses_wikitext2_corpus` (function, line 218) `def uses_wikitext2_corpus(tag)`
  - `moonshine_tag_to_wikipedia_lang` (function, line 226) `def moonshine_tag_to_wikipedia_lang(tag)`
  - `moonshine_tag_to_whisper_language` (function, line 238) `def moonshine_tag_to_whisper_language(tag)`
  - `moonshine_tag_to_upstream_kokoro_lang_code` (function, line 250) `def moonshine_tag_to_upstream_kokoro_lang_code(tag)`
  - `load_wiki_text_directory` (function, line 268) `def load_wiki_text_directory(dir_path)`
  - `_read_nonempty_lines` (function, line 278) `def _read_nonempty_lines(text)`
  - `load_wiki_text_file` (function, line 288) `def load_wiki_text_file(path)`
  - `load_wiki_texts` (function, line 319) `def load_wiki_texts(path)`
  - `_wiki_max_graphemes_for_moonshine_tag` (function, line 325) `def _wiki_max_graphemes_for_moonshine_tag(tag, base_max)`
  - `clean_wiki_text_line` (function, line 339) `def clean_wiki_text_line(raw)`
  - `_split_oversized_wiki_piece` (function, line 360) `def _split_oversized_wiki_piece(s)`
  - `normalize_eval_lines` (function, line 415) `def normalize_eval_lines(raw_lines)`
  - `wikipedia_paragraph_to_candidates` (function, line 446) `def wikipedia_paragraph_to_candidates(para)`
  - `try_import_datasets` (function, line 477) `def try_import_datasets()`
  - `_parse_datasets_version_tuple` (function, line 486) `def _parse_datasets_version_tuple(version)`
  - `require_datasets_compatible_with_python` (function, line 506) `def require_datasets_compatible_with_python()`
  - `fetch_lines_wikitext2` (function, line 528) `def fetch_lines_wikitext2()`
  - `_prefers_natural_wikipedia_prose_for_tag` (function, line 569) `def _prefers_natural_wikipedia_prose_for_tag(tag)`
  - `_german_wikipedia_lead_penalty` (function, line 576) `def _german_wikipedia_lead_penalty(line)`
  - `fetch_lines_wikipedia` (function, line 593) `def fetch_lines_wikipedia(wiki_lang)`
  - `fetch_lines_for_moonshine_language` (function, line 655) `def fetch_lines_for_moonshine_language(lang_tag)`
  - `all_moonshine_tts_language_tags` (function, line 672) `def all_moonshine_tts_language_tags()`
  - `ensure_wiki_text_files` (function, line 682) `def ensure_wiki_text_files(output_dir, languages)`
  - `resample_linear` (function, line 735) `def resample_linear(samples, orig_sr, target_sr)`
  - `_tts_cache_key` (function, line 749) `def _tts_cache_key(payload)`
  - `_tts_track_to_engine_slug` (function, line 754) `def _tts_track_to_engine_slug(track)`
  - `_tts_sentence_prefix_for_cache` (function, line 766) `def _tts_sentence_prefix_for_cache(text, max_chars)`
  - `_tts_cache_stem` (function, line 778) `def _tts_cache_stem(text, track, payload)`
  - `_tts_cache_wav_and_meta_paths` (function, line 785) `def _tts_cache_wav_and_meta_paths(root, lang, stem)`
  - `_write_wav_int16_mono` (function, line 792) `def _write_wav_int16_mono(path, samples, sample_rate)`
  - `_read_wav_int16_mono` (function, line 803) `def _read_wav_int16_mono(path)`
  - `_load_tts_wav_meta` (function, line 819) `def _load_tts_wav_meta(meta_path)`
  - `_save_tts_wav_meta` (function, line 832) `def _save_tts_wav_meta(meta_path, phonemes)`
  - `_try_read_tts_wav_cache` (function, line 845) `def _try_read_tts_wav_cache(cache_root, lang, payload)`
  - `_write_tts_wav_cache` (function, line 872) `def _write_tts_wav_cache(cache_root, lang, payload, samples, sample_rate, phonemes)`
  - `try_import_cer` (function, line 894) `def try_import_cer()`
  - `try_import_whisper_model` (function, line 903) `def try_import_whisper_model()`
  - `VoicePair` (class, line 913) `class VoicePair`
  - `discover_voices` (method, line 918) `def discover_voices(language, asset_root)`
  - `prepare_asset_root` (method, line 931) `def prepare_asset_root(language, voices, cache_root)`
  - `overlay_repo_tts_data_into_asset_root` (method, line 955) `def overlay_repo_tts_data_into_asset_root(asset_root, tts_data_root, lang)`
  - `_kokoro_ja_text_for_misaki_cutlet` (method, line 989) `def _kokoro_ja_text_for_misaki_cutlet(text)`
  - `moonshine_kokoro_catalog_voice_to_package_voice` (method, line 995) `def moonshine_kokoro_catalog_voice_to_package_voice(catalog_id)`
  - `try_import_k_pipeline` (method, line 1002) `def try_import_k_pipeline()`
  - `try_import_piper_voice` (method, line 1011) `def try_import_piper_voice()`
  - `ensure_piper_espeak_phonemizer_uses_nfc_for_eval` (method, line 1023) `def ensure_piper_espeak_phonemizer_uses_nfc_for_eval()`
  - `resolve_piper_onnx_path` (method, line 1074) `def resolve_piper_onnx_path(asset_root, piper_voice_catalog_id)`
  - `build_upstream_kokoro_pipeline` (method, line 1086) `def build_upstream_kokoro_pipeline(lang_code)`
  - `synthesize_upstream_kokoro_package` (method, line 1104) `def synthesize_upstream_kokoro_package(pipeline, text, voice)`
  - `synthesize_upstream_piper_package` (method, line 1136) `def synthesize_upstream_piper_package(piper_voice, text)`
  - `LineResult` (class, line 1162) `class LineResult`
  - `transcribe_whisper` (method, line 1180) `def transcribe_whisper(model, samples, sample_rate, whisper_lang)`
  - `run_language` (method, line 1197) `def run_language(language, lines)`
  - `line_result_to_dict` (method, line 1474) `def line_result_to_dict(r)`
  - `_fmt_metric` (method, line 1494) `def _fmt_metric(x)`
  - `_fmt_cer_percent` (method, line 1498) `def _fmt_cer_percent(x)`
  - `_reference_cer_from_upstream_averages` (method, line 1505) `def _reference_cer_from_upstream_averages(kokoro, piper)`
  - `format_cer_summary_markdown_table` (method, line 1519) `def format_cer_summary_markdown_table(languages_report)`
  - `main` (method, line 1556) `def main()`
  - `flush` (method, line 295) `def flush()`
  - `phonemize_nfc` (method, line 1041) `def phonemize_nfc(self, voice, text)`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

## scripts/update-version.sh
- Layer: utility
- Language: sh

## scripts/upload-tts-assets-to-gcs.sh
- Doc: Upload core/moonshine-tts/data to the Moonshine download bucket under tts/, using `gcloud...
- Layer: utility
- Language: sh
