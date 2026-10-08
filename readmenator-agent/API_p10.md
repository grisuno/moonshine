# API (page 10 of 10)
Previous: [API_p9.md](API_p9.md)

## scripts/tts_g2p_intelligibility.py
Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`
- `levenshtein_distance` (function) `scripts/tts_g2p_intelligibility.py:102` `def levenshtein_distance(s, t)` -- Character-level Levenshtein (edit) distance between two strings.
- `uses_wikitext2_corpus` (function) `scripts/tts_g2p_intelligibility.py:218` `def uses_wikitext2_corpus(tag)` -- WikiText-2 on Hugging Face is English-only; use it for US/UK (and generic ``en``) tags.
- `moonshine_tag_to_wikipedia_lang` (function) `scripts/tts_g2p_intelligibility.py:226` `def moonshine_tag_to_wikipedia_lang(tag)`
- `moonshine_tag_to_whisper_language` (function) `scripts/tts_g2p_intelligibility.py:238` `def moonshine_tag_to_whisper_language(tag)`
- `moonshine_tag_to_upstream_kokoro_lang_code` (function) `scripts/tts_g2p_intelligibility.py:250` `def moonshine_tag_to_upstream_kokoro_lang_code(tag)` -- Locale supported by ``pip install kokoro`` / ``KPipeline`` (not all Moonshine TTS languages).
- `load_wiki_text_directory` (function) `scripts/tts_g2p_intelligibility.py:268` `def load_wiki_text_directory(dir_path)`
- `load_wiki_text_file` (function) `scripts/tts_g2p_intelligibility.py:288` `def load_wiki_text_file(path)`
- `flush` (method) `scripts/tts_g2p_intelligibility.py:295` `def flush()`
- `load_wiki_texts` (function) `scripts/tts_g2p_intelligibility.py:319` `def load_wiki_texts(path)`
- `clean_wiki_text_line` (function) `scripts/tts_g2p_intelligibility.py:339` `def clean_wiki_text_line(raw)`
- `normalize_eval_lines` (function) `scripts/tts_g2p_intelligibility.py:415` `def normalize_eval_lines(raw_lines)` -- Chunk or filter lines so each fits Moonshine G2P / TTS (same bounds as wiki download).
- `wikipedia_paragraph_to_candidates` (function) `scripts/tts_g2p_intelligibility.py:446` `def wikipedia_paragraph_to_candidates(para)`
- `try_import_datasets` (function) `scripts/tts_g2p_intelligibility.py:477` `def try_import_datasets()`
- `require_datasets_compatible_with_python` (function) `scripts/tts_g2p_intelligibility.py:506` `def require_datasets_compatible_with_python()` -- ``datasets`` before 4.4.0 breaks on Python 3.14 inside dill/pickle (Hasher.hash / load_dataset).
- `fetch_lines_wikitext2` (function) `scripts/tts_g2p_intelligibility.py:528` `def fetch_lines_wikitext2()`
- `fetch_lines_wikipedia` (function) `scripts/tts_g2p_intelligibility.py:593` `def fetch_lines_wikipedia(wiki_lang)`
- `fetch_lines_for_moonshine_language` (function) `scripts/tts_g2p_intelligibility.py:655` `def fetch_lines_for_moonshine_language(lang_tag)`
- `all_moonshine_tts_language_tags` (function) `scripts/tts_g2p_intelligibility.py:672` `def all_moonshine_tts_language_tags()`
- `ensure_wiki_text_files` (function) `scripts/tts_g2p_intelligibility.py:682` `def ensure_wiki_text_files(output_dir, languages)` -- Ensure ``output_dir/<lang>.txt`` exists for each language.
- `resample_linear` (function) `scripts/tts_g2p_intelligibility.py:735` `def resample_linear(samples, orig_sr, target_sr)`
- `try_import_cer` (function) `scripts/tts_g2p_intelligibility.py:894` `def try_import_cer()`
- `try_import_whisper_model` (function) `scripts/tts_g2p_intelligibility.py:903` `def try_import_whisper_model()`
- `VoicePair.discover_voices` (method) `scripts/tts_g2p_intelligibility.py:918` `def discover_voices(language, asset_root)`
- `VoicePair.prepare_asset_root` (method) `scripts/tts_g2p_intelligibility.py:931` `def prepare_asset_root(language, voices, cache_root)`
- `VoicePair.overlay_repo_tts_data_into_asset_root` (method) `scripts/tts_g2p_intelligibility.py:955` `def overlay_repo_tts_data_into_asset_root(asset_root, tts_data_root, lang)` -- Copy files from ``tts_data_root/<lang>/`` onto the downloaded asset tree so repo ``dict.tsv`` and other linguistic...
- `VoicePair.moonshine_kokoro_catalog_voice_to_package_voice` (method) `scripts/tts_g2p_intelligibility.py:995` `def moonshine_kokoro_catalog_voice_to_package_voice(catalog_id)`
- `VoicePair.try_import_k_pipeline` (method) `scripts/tts_g2p_intelligibility.py:1002` `def try_import_k_pipeline()`
- `VoicePair.try_import_piper_voice` (method) `scripts/tts_g2p_intelligibility.py:1011` `def try_import_piper_voice()`
- `VoicePair.ensure_piper_espeak_phonemizer_uses_nfc_for_eval` (method) `scripts/tts_g2p_intelligibility.py:1023` `def ensure_piper_espeak_phonemizer_uses_nfc_for_eval()` -- ``piper-tts`` decomposes espeak IPA with Unicode NFD, so combining marks (e.g.
- `VoicePair.phonemize_nfc` (method) `scripts/tts_g2p_intelligibility.py:1041` `def phonemize_nfc(self, voice, text)`
- `VoicePair.resolve_piper_onnx_path` (method) `scripts/tts_g2p_intelligibility.py:1074` `def resolve_piper_onnx_path(asset_root, piper_voice_catalog_id)`
- `VoicePair.build_upstream_kokoro_pipeline` (method) `scripts/tts_g2p_intelligibility.py:1086` `def build_upstream_kokoro_pipeline(lang_code)`
- `VoicePair.synthesize_upstream_kokoro_package` (method) `scripts/tts_g2p_intelligibility.py:1104` `def synthesize_upstream_kokoro_package(pipeline, text, voice)` -- hexgrad/kokoro ``KPipeline`` (misaki + espeak-ng G2P inside the package).
- `VoicePair.synthesize_upstream_piper_package` (method) `scripts/tts_g2p_intelligibility.py:1136` `def synthesize_upstream_piper_package(piper_voice, text)` -- ``piper-tts`` ``PiperVoice`` (phonemize + espeak-ng data bundled with the package).
- `LineResult.transcribe_whisper` (method) `scripts/tts_g2p_intelligibility.py:1180` `def transcribe_whisper(model, samples, sample_rate, whisper_lang)`
- `LineResult.run_language` (method) `scripts/tts_g2p_intelligibility.py:1197` `def run_language(language, lines)`
- `LineResult.line_result_to_dict` (method) `scripts/tts_g2p_intelligibility.py:1474` `def line_result_to_dict(r)`
- `LineResult.format_cer_summary_markdown_table` (method) `scripts/tts_g2p_intelligibility.py:1519` `def format_cer_summary_markdown_table(languages_report)` -- GitHub-flavored markdown table: Language, Moonshine CER, Reference CER (min Kokoro/Piper).
- `LineResult.main` (method) `scripts/tts_g2p_intelligibility.py:1556` `def main()`

## swift/Sources/MoonshineVoice/Errors.swift
- `checkError` (function) `swift/Sources/MoonshineVoice/Errors.swift:40` -- Helper function to check error codes and throw appropriate Swift errors

## swift/Sources/MoonshineVoice/MicTranscriber.swift
- `feedCapturedAudio` (function) `swift/Sources/MoonshineVoice/MicTranscriber.swift:262` -- Sink for a single captured audio buffer.

## swift/Sources/MoonshineVoice/MoonshineAPI.swift
- `getVersion` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:21` -- Get the version of the loaded Moonshine library.
- `errorToString` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:26` -- Convert an error code to a human-readable string.
- `loadTranscriberFromFiles` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:34` -- Load a transcriber from files on disk.
- `freeTranscriber` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:93` -- Free a transcriber handle.
- `transcribeWithoutStreaming` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:98` -- Transcribe audio without streaming.
- `createStream` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:134` -- Create a stream for real-time transcription.
- `freeStream` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:141` -- Free a stream handle.
- `startStream` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:147` -- Start a stream.
- `stopStream` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:153` -- Stop a stream.
- `addAudioToStream` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:159` -- Add audio data to a stream.
- `transcribeStream` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:184` -- Transcribe a stream and get updated results.
- `createTtsSynthesizerFromFiles` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:305` -- Create a TTS synthesizer from files on disk.
- `createTtsSynthesizerFromMemory` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:361` -- Create a TTS synthesizer from in-memory asset buffers keyed by canonical filename.
- `textToSpeech` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:421` -- Synthesize text to speech, returning PCM float samples and sample rate.
- `phonemesToSpeech` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:485` -- Synthesize speech from IPA phonemes, returning PCM float samples and sample rate.
- `freeTtsSynthesizer` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:545` -- Free a TTS synthesizer handle.
- `getTtsVoices` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:550` -- Get TTS voices JSON for the given languages.
- `getTtsDependencies` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:600` -- Get TTS dependencies JSON for the given languages.
- `getG2pDependencies` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:650` -- Get G2P-only asset dependency keys as a comma-separated string.
- `getSttDependencies` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:668` -- Get the speech-to-text model download manifest as a JSON object string.  - Parameters: - language: Language code (e.g.
- `getIntentDependencies` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:685` -- Get the intent-recognition embedding model download manifest as a JSON object string.  - Parameters: - modelName...
- `createIntentRecognizer` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:744` -- MARK: - Intent recognition
- `freeIntentRecognizer` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:761`
- `registerIntentRecognizerIntent` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:765`
- `unregisterIntentRecognizerIntent` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:775` -- Returns: `true` if an intent was removed, `false` if the phrase was not registered.
- `getClosestIntents` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:787`
- `getIntentRecognizerIntentCount` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:826`
- `clearIntentRecognizerIntents` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:834`
- `calculateIntentEmbedding` (function) `swift/Sources/MoonshineVoice/MoonshineAPI.swift:838`

## swift/Sources/MoonshineVoice/TranscriptEventListener.swift
- `onLineStarted` (function) `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:10` -- Called when a new transcription line starts.
- `onLineUpdated` (function) `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:13` -- Called when an existing transcription line is updated.
- `onLineTextChanged` (function) `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:16` -- Called when the text of a transcription line changes.
- `onLineSpeakersChanged` (function) `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:20` -- Called when the speaker spans of a transcription line change.
- `onLineCompleted` (function) `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:23` -- Called when a transcription line is completed.
- `onError` (function) `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:26` -- Called when an error occurs.
- `onLineStarted` (function) `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:31`
- `onLineUpdated` (function) `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:32`
- `onLineTextChanged` (function) `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:33`
- `onLineSpeakersChanged` (function) `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:34`
- `onLineCompleted` (function) `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:35`
- `onError` (function) `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:36`

## swift/Sources/MoonshineVoice/TranscriptionStream.swift
Imported by: `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift::FakeStream`
- `start` (function) `swift/Sources/MoonshineVoice/TranscriptionStream.swift:10`
- `stop` (function) `swift/Sources/MoonshineVoice/TranscriptionStream.swift:11`
- `close` (function) `swift/Sources/MoonshineVoice/TranscriptionStream.swift:12`
- `addAudio` (function) `swift/Sources/MoonshineVoice/TranscriptionStream.swift:13`
- `addListener` (function) `swift/Sources/MoonshineVoice/TranscriptionStream.swift:14`
- `addListener` (function) `swift/Sources/MoonshineVoice/TranscriptionStream.swift:15`
- `removeListener` (function) `swift/Sources/MoonshineVoice/TranscriptionStream.swift:16`
- `removeListener` (function) `swift/Sources/MoonshineVoice/TranscriptionStream.swift:17`
- `removeAllListeners` (function) `swift/Sources/MoonshineVoice/TranscriptionStream.swift:18`

