# Index (page 2 of 2)
Previous: [INDEX.md](INDEX.md)

| File | Purpose | Subsystem | Symbols | Used by |
|------|---------|-----------|---------|---------|
| `python/src/moonshine_voice/dialog_flow.py` | Generator-based dialog flow runner for Moonshine Voice. | moonshine_voice | 94 | 0 |
| `python/src/moonshine_voice/download.py` | EmbeddingModelArch: Supported embedding model architectures. | moonshine_voice | 43 | 8 |
| `python/src/moonshine_voice/download_file.py` | get_cache_dir: Get the cache directory, respecting environment override. | moonshine_voice | 4 | 1 |
| `python/src/moonshine_voice/errors.py` | Error classes for Moonshine Voice. | moonshine_voice | 15 | 7 |
| `python/src/moonshine_voice/g2p.py` | Grapheme-to-phoneme (IPA) via the Moonshine C API. | moonshine_voice | 10 | 0 |
| `python/src/moonshine_voice/intent_recognizer.py` | Intent recognition module for Moonshine Voice. | moonshine_voice | 29 | 2 |
| `python/src/moonshine_voice/mic_transcriber.py` | MicTranscriber: MicTranscriber is a class that transcribes audio from a microphone. | moonshine_voice | 30 | 3 |
| `python/src/moonshine_voice/moonshine_api.py` | TranscriptWordC: C structure for transcript_word_t. | moonshine_voice | 37 | 8 |
| `python/src/moonshine_voice/tts.py` | Text-to-speech via the Moonshine C API. | moonshine_voice | 44 | 0 |
| `python/src/moonshine_voice/utils.py` | Utility functions for Moonshine Voice. | moonshine_voice | 3 | 4 |
| `python/tests/test_cli.py` | Tests the ``moonshine-voice`` console-script entry point. | python_tests | 8 | 0 |
| `python/tests/test_docs.py` | Tests that the code blocks in the documentation actually work. | python_tests | 10 | 0 |
| `python/tests/test_mic_transcriber_threading.py` | Regression test for issue #196. | python_tests | 22 | 0 |
| `python/tests/test_modules.py` | Runs the ``__main__`` sections of the most significant modules. | python_tests | 11 | 0 |
| `scripts/analyze_ko_phoneme_patterns.py` | Analyze systematic phoneme pattern differences between Moonshine and Piper Korean G2P. | scripts | 4 | 0 |
| `scripts/analyze_ko_stress.py` | Deep analysis of Korean stress placement: Moonshine vs Piper/eSpeak. | scripts | 8 | 0 |
| `scripts/check-banned-constructs.sh` | Guard against banned C++ constructs creeping into first-party core code. | scripts | 1 | 0 |
| `scripts/check-clang-tidy.sh` | Gate clang-tidy findings against a committed baseline so that only *newly introduced* problems... | scripts | 1 | 0 |
| `scripts/compare_ko_phonemes.py` | Compare Moonshine vs Piper Korean phonemes directly (no TTS/Whisper needed). | scripts | 5 | 0 |
| `scripts/convert_tokenizer.py` | Convert tokenizer files to the BinTokenizer format used by moonshine. | scripts | 4 | 0 |
| `scripts/eval-alphanumeric.py` | Evaluate AlphanumericListener on the test-assets/alphanumeric dataset. | scripts | 5 | 0 |
| `scripts/eval-librispeech.py` | Evaluate Moonshine English WER on LibriSpeech test-clean. | scripts | 10 | 0 |
| `scripts/eval-model-accuracy.py` | On a Mac you'll need to set up ffmpeg using: brew install ffmpeg@8 export... | scripts | 0 | 0 |
| `scripts/eval-speaker-id.py` | - | scripts | 0 | 0 |
| `scripts/export-decoder-with-attention.py` | Export a decoder_with_attention model for word-level timestamps. | scripts | 1 | 0 |
| `scripts/export_zipvoice_model.py` | Copyright 2026 Useful Sensors  Licensed under the Apache License, Version 2.0 (the "License")... | scripts | 4 | 0 |
| `scripts/export_zipvoice_voices_for_cpp.py` | Copyright 2026 Useful Sensors  Licensed under the Apache License, Version 2.0 (the "License")... | scripts | 10 | 0 |
| `scripts/format-core.sh` | Format (default) or check (--check) the first-party C++ in core/ against the repo's Google-based... | scripts | 0 | 0 |
| `scripts/generate-diarization-test-audio.py` | Copyright 2026 Moonshine AI (MIT License) | scripts | 4 | 0 |
| `scripts/generate-silero-vad-data.py` | Regenerate core/silero-vad-model-data.h from the Silero VAD model. | scripts | 4 | 0 |
| `scripts/patch-release.sh` | Fold one or more fixes into the current in-progress release by cherry-picking them onto its... | scripts | 1 | 0 |
| `scripts/prepare-release.sh` | main: All imperative work lives inside main() so bash parses the whole script before executing... | scripts | 1 | 0 |
| `scripts/publish-binary.sh` | - | scripts | 0 | 0 |
| `scripts/publish-examples.sh` | - | scripts | 0 | 0 |
| `scripts/publish-swift.sh` | - | scripts | 0 | 0 |
| `scripts/quantize-streaming-model.sh` | - | scripts | 0 | 0 |
| `scripts/reliability-remote.sh` | Runs the heavy reliability checks on a Linux x86 host with clang + libFuzzer. | scripts | 4 | 0 |
| `scripts/reliability.sh` | Periodic reliability driver. | scripts | 0 | 0 |
| `scripts/run-benchmarks.py` | Benchmark to compare Moonshine and Whisper model latency in live speech scenarios. | scripts | 3 | 0 |
| `scripts/setup-android-ci.sh` | One-time setup of the Android toolchain needed to run the moonshine-voice instrumentation tests... | scripts | 1 | 0 |
| `scripts/test-android.sh` | Run the moonshine-voice Android library's instrumentation tests on a real device or emulator... | scripts | 3 | 0 |
| `scripts/test-core.sh` | - | scripts | 0 | 0 |
| `scripts/test-docs.sh` | Tests that the code in the documentation still works, by executing the fenced code blocks in... | scripts | 1 | 0 |
| `scripts/test-examples.sh` | Verify iOS and Android examples build standalone: either from GitHub Release archives (default)... | scripts | 23 | 0 |
| `scripts/test-model-downloads.sh` | Download-and-run sampling tests for the native model catalog, plus the Swift and Android... | scripts | 3 | 0 |
| `scripts/test-python.sh` | Runs the Python module tests (python/tests/test_modules.py), which drive the __main__ sections... | scripts | 1 | 0 |
| `scripts/tts_g2p_intelligibility.py` | Evaluate TTS intelligibility: Moonshine synthesis (Kokoro / Piper vocoders) vs Whisper large-v3... | scripts | 62 | 0 |
| `scripts/update-version.sh` | - | scripts | 0 | 0 |
| `scripts/upload-tts-assets-to-gcs.sh` | Upload core/moonshine-tts/data to the Moonshine download bucket under tts/, using `gcloud... | scripts | 0 | 0 |
| `settings.gradle.kts` | - | root | 0 | 0 |
| `swift/Package.swift` | swift-tools-version: 6.1 | misc | 0 | 0 |
| `swift/Sources/MoonshineVoice/AssetDownloadError.swift` | - | MoonshineVoice | 0 | 0 |
| `swift/Sources/MoonshineVoice/AssetDownloader.swift` | - | MoonshineVoice | 0 | 0 |
| `swift/Sources/MoonshineVoice/EmbeddingModelArch.swift` | - | MoonshineVoice | 0 | 0 |
| `swift/Sources/MoonshineVoice/Errors.swift` | checkError: Helper function to check error codes and throw appropriate Swift errors | MoonshineVoice | 1 | 0 |
| `swift/Sources/MoonshineVoice/Events.swift` | - | MoonshineVoice | 0 | 0 |
| `swift/Sources/MoonshineVoice/IntentRecognizer.swift` | - | MoonshineVoice | 0 | 0 |
| `swift/Sources/MoonshineVoice/MicTranscriber.swift` | feedCapturedAudio: Sink for a single captured audio buffer. | MoonshineVoice | 1 | 0 |
| `swift/Sources/MoonshineVoice/ModelArch.swift` | - | MoonshineVoice | 0 | 0 |
| `swift/Sources/MoonshineVoice/MoonshineAPI.swift` | getVersion: Get the version of the loaded Moonshine library. | MoonshineVoice | 29 | 0 |
| `swift/Sources/MoonshineVoice/Stream.swift` | - | MoonshineVoice | 0 | 0 |
| `swift/Sources/MoonshineVoice/TextToSpeech.swift` | - | MoonshineVoice | 0 | 0 |
| `swift/Sources/MoonshineVoice/Transcriber.swift` | - | MoonshineVoice | 0 | 0 |
| `swift/Sources/MoonshineVoice/Transcript.swift` | - | MoonshineVoice | 0 | 0 |
| `swift/Sources/MoonshineVoice/TranscriptEventListener.swift` | onLineStarted: Called when a new transcription line starts. | MoonshineVoice | 12 | 0 |
| `swift/Sources/MoonshineVoice/TranscriptionStream.swift` | TranscriptionStream: The subset of ``Stream`` that ``MicTranscriber`` drives. | MoonshineVoice | 10 | 1 |
| `swift/Sources/MoonshineVoice/TtsSynthesisResult.swift` | - | MoonshineVoice | 0 | 0 |
| `swift/Sources/MoonshineVoice/WAVLoader.swift` | - | MoonshineVoice | 0 | 0 |
| `swift/Tests/MoonshineVoiceTests/AssetDownloaderNetworkTests.swift` | testDownloadsAndRunsSttModel: Downloads the tiny English STT model, loads it with... | MoonshineVoiceTests | 6 | 0 |
| `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift` | MockURLProtocol: Minimal in-process HTTP stub. | MoonshineVoiceTests | 18 | 0 |
| `swift/Tests/MoonshineVoiceTests/IntentRecognizerTests.swift` | - | MoonshineVoiceTests | 3 | 0 |
| `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift` | MicTranscriberThreadingTests: ``test_mic_transcriber_threading`` test. | MoonshineVoiceTests | 12 | 0 |
| `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift` | testCreateSynthesizer: MARK: - Creation Tests | MoonshineVoiceTests | 20 | 0 |
| `swift/Tests/MoonshineVoiceTests/TranscriberTests.swift` | testTranscribeWithoutStreaming_beckett: MARK: - Non-Streaming Tests | MoonshineVoiceTests | 12 | 0 |

