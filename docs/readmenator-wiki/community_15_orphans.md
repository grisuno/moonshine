# orphans

*Community 15 | 137 files | cohesion 0.00*

## Definition

This community groups 137 file(s) rooted at `scripts` with dominant language swift (cohesion 0.00). Central symbols: `AddEval`, `AddInit`, `Arguments`, `AssetDownloader`, `AssetDownloaderNetworkTests`, `AssetDownloaderTest`, `AssetDownloaderTests`, `BinaryDistribution`. Core file: `micro/examples/rp2350/lwipopts.h` (42 symbols). Documented purpose: ContentView.swift Transcriber  Created by Pete Warden on 1/1/26..

## Files

### `scripts` (31 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `scripts/analyze_ko_phoneme_patterns.py` | py | utility | 4 | yes |

### `swift/Sources/MoonshineVoice` (17 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `swift/Sources/MoonshineVoice/AssetDownloadError.swift` | swift | utility | 0 | no |

### `android/java/main/java/ai/moonshine/voice` (13 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `android/java/main/java/ai/moonshine/voice/AssetDownloader.java` | java | utility | 14 | no |

### `micro/examples/rp2350/scripts` (7 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `micro/examples/rp2350/scripts/capture_neural_tts.py` | py | utility | 2 | yes |

### `swift/Tests/MoonshineVoiceTests` (6 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `swift/Tests/MoonshineVoiceTests/AssetDownloaderNetworkTests.swift` | swift | testing | 6 | no |

### `micro/examples/rp2350/src` (5 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `micro/examples/rp2350/src/main_step1_blinky.cc` | cc | utility | 1 | yes |

### `android/java/androidTest/java/ai/moonshine/voice` (4 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `android/java/androidTest/java/ai/moonshine/voice/AssetDownloaderTest.java` | java | testing | 6 | no |

### `examples/ios/IntentRecognizer/IntentRecognizer` (4 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `examples/ios/IntentRecognizer/IntentRecognizer/ContentView.swift` | swift | presentation | 1 | no |

### `examples/python` (4 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `examples/python/basic_transcription.py` | py | utility | 6 | yes |

### `micro/neural-tts/host/tflm_ref` (4 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `micro/neural-tts/host/tflm_ref/add.cpp` | cpp | utility | 5 | yes |

### `.` (2 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `clang-format.sh` | sh | utility | 0 | no |

### `core/cpp-annote/src` (2 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `core/cpp-annote/src/community1_cpp_annote_embedded.cpp` | cpp | utility | 0 | no |

### `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer` (2 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/AssetDirectoryCopy.kt` | kt | utility | 1 | no |

### `examples/ios/TextToSpeech/TextToSpeech` (2 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `examples/ios/TextToSpeech/TextToSpeech/ContentView.swift` | swift | presentation | 1 | no |

### `examples/ios/Transcriber/Transcriber` (2 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `examples/ios/Transcriber/Transcriber/ContentView.swift` | swift | presentation | 1 | yes |

### `examples/ios/Transcriber/TranscriberUITests` (2 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `examples/ios/Transcriber/TranscriberUITests/TranscriberUITests.swift` | swift | utility | 5 | yes |

### `micro/stt-training` (2 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `micro/stt-training/config.sh` | sh | infrastructure | 0 | yes |

### `python/tests` (2 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `python/tests/test_docs.py` | py | testing | 10 | yes |

### `android/java/test/java/ai/moonshine/voice` (1 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `android/java/test/java/ai/moonshine/voice/ExampleUnitTest.java` | java | testing | 2 | no |

### `core/moonshine-tts/src` (1 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `core/moonshine-tts/src/zipvoice-voices-data.cpp` | cpp | data_access | 0 | no |

*... and 117 more files in this community.*


## Key Symbols

- `AssetDownloaderTest` (class, `android/java/androidTest/java/ai/moonshine/voice/AssetDownloaderTest.java:35`) - End-to-end tests that exercise {@link AssetDownloader} against the <b>real</b> CDN (https://download
- `setUp` (method, `android/java/androidTest/java/ai/moonshine/voice/AssetDownloaderTest.java:39`)
- `downloadsEnabled` (method, `android/java/androidTest/java/ai/moonshine/voice/AssetDownloaderTest.java:49`)
- `testDownloadsAndRunsSttModel` (method, `android/java/androidTest/java/ai/moonshine/voice/AssetDownloaderTest.java:61`)
- `testDownloadsAndRunsTtsVoice` (method, `android/java/androidTest/java/ai/moonshine/voice/AssetDownloaderTest.java:91`)
- `testDownloadsAndRunsIntentModel` (method, `android/java/androidTest/java/ai/moonshine/voice/AssetDownloaderTest.java:112`)
- `IntentRecognizerTest` (class, `android/java/androidTest/java/ai/moonshine/voice/IntentRecognizerTest.java:13`)
- `testCreateIntentRecognizer_invalidPath_throws` (method, `android/java/androidTest/java/ai/moonshine/voice/IntentRecognizerTest.java:15`)
- `testGetClosestIntents_whenModelPresent` (method, `android/java/androidTest/java/ai/moonshine/voice/IntentRecognizerTest.java:22`)
- `TextToSpeechTest` (class, `android/java/androidTest/java/ai/moonshine/voice/TextToSpeechTest.java:27`) - ZipVoice TTS coverage for the Android JNI binding.  <p>The catalog / engine-selection tests need no
- `setUp` (method, `android/java/androidTest/java/ai/moonshine/voice/TextToSpeechTest.java:28`)
- `testZipVoiceDependencies` (method, `android/java/androidTest/java/ai/moonshine/voice/TextToSpeechTest.java:33`)
- `testZipVoiceVoicesListing` (method, `android/java/androidTest/java/ai/moonshine/voice/TextToSpeechTest.java:49`)
- `findZipVoiceRoot` (method, `android/java/androidTest/java/ai/moonshine/voice/TextToSpeechTest.java:63`)
- `testZipVoiceBuiltinVoiceSynthesizes` (method, `android/java/androidTest/java/ai/moonshine/voice/TextToSpeechTest.java:97`)
- `testZipVoiceClonePcmSynthesizes` (method, `android/java/androidTest/java/ai/moonshine/voice/TextToSpeechTest.java:114`)
- `Utils` (class, `android/java/androidTest/java/ai/moonshine/voice/Utils.java:18`)
- `logStats` (method, `android/java/androidTest/java/ai/moonshine/voice/Utils.java:22`)
- `removePunctuation` (method, `android/java/androidTest/java/ai/moonshine/voice/Utils.java:58`)
- `normalizedEditDistance` (method, `android/java/androidTest/java/ai/moonshine/voice/Utils.java:80`)
- `WavData` (class, `android/java/androidTest/java/ai/moonshine/voice/Utils.java:116`)
- `WavData` (method, `android/java/androidTest/java/ai/moonshine/voice/Utils.java:118`)
- `loadWavFromAssets` (method, `android/java/androidTest/java/ai/moonshine/voice/Utils.java:128`)
- `loadAsset` (method, `android/java/androidTest/java/ai/moonshine/voice/Utils.java:174`)
- `copyAssetToTempDir` (method, `android/java/androidTest/java/ai/moonshine/voice/Utils.java:186`)
- `AssetDownloader` (class, `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:37`) - Downloads the model/data files a Moonshine engine needs into an app-chosen directory, then hands bac
- `ProgressListener` (class, `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:46`) - and report progress through an optional listener.  <p>{@link #ensureModelPresent} performs blocking
- `AssetDownloader` (method, `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:59`)
- `AssetDownloader` (method, `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:69`)
- `isModelPresent` (method, `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:74`)

## Internal vs External Edges

- Internal resolved imports (EXTRACTED): 0
- Cross-boundary resolved imports (EXTRACTED): 1

## Connections

- No cross-community bridges recorded. This community is self-contained.

## Risks

- [taint medium] `android/java/androidTest/java/ai/moonshine/voice/Utils.java` -> `android/java/androidTest/java/ai/moonshine/voice/Utils.java` via `input` (0 hops)
- [taint medium] `android/java/main/java/ai/moonshine/voice/AssetDownloader.java` -> `android/java/main/java/ai/moonshine/voice/AssetDownloader.java` via `input` (0 hops)
- [taint medium] `micro/stt-training/tools/download_musan_rirs.py` -> `micro/stt-training/tools/download_musan_rirs.py` via `urllib.request` (0 hops)
- [dataflow UNCHECKED_ALLOC] `android/java/androidTest/java/ai/moonshine/voice/Utils.java:131` `loadWavFromAssets` `is`: Result of allocator stored in `is` is never checked against NULL.
- [dataflow UNCHECKED_ALLOC] `android/java/androidTest/java/ai/moonshine/voice/Utils.java:177` `loadAsset` `is`: Result of allocator stored in `is` is never checked against NULL.
- [dataflow UNCHECKED_ALLOC] `android/java/androidTest/java/ai/moonshine/voice/Utils.java:190` `copyAssetToTempDir` `is`: Result of allocator stored in `is` is never checked against NULL.

## Open Questions

- Why do 71 file(s) lack file-level docs (e.g. `android/java/androidTest/java/ai/moonshine/voice/AssetDownloaderTest.java`)? What purpose do they serve?
- Is the dangerous import `input` in `android/java/androidTest/java/ai/moonshine/voice/Utils.java` still required, or can it be isolated?
- What would break if the most connected file in orphans changed?
- Should orphans be split, given cohesion 0.00?

## Sources

- `android/java/androidTest/java/ai/moonshine/voice/AssetDownloaderTest.java`
- `android/java/androidTest/java/ai/moonshine/voice/IntentRecognizerTest.java`
- `android/java/androidTest/java/ai/moonshine/voice/TextToSpeechTest.java`
- `android/java/androidTest/java/ai/moonshine/voice/Utils.java`
- `android/java/main/java/ai/moonshine/voice/AssetDownloader.java`
- `android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java`
- `android/java/main/java/ai/moonshine/voice/IntentMatch.java`
- `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java`
- `android/java/main/java/ai/moonshine/voice/MicCaptureProcessor.java`
- `android/java/main/java/ai/moonshine/voice/MicTranscriber.java`
- `android/java/main/java/ai/moonshine/voice/MoonshineDownloadWorker.java`
- `android/java/main/java/ai/moonshine/voice/SpeakerSpan.java`
- `android/java/main/java/ai/moonshine/voice/TextToSpeech.java`
- `android/java/main/java/ai/moonshine/voice/Transcript.java`
- `android/java/main/java/ai/moonshine/voice/TranscriptEventListener.java`
- `android/java/main/java/ai/moonshine/voice/TtsSynthesisResult.java`
- `android/java/main/java/ai/moonshine/voice/WordTiming.java`
- `android/java/test/java/ai/moonshine/voice/ExampleUnitTest.java`
- `clang-format.sh`
- `core/cpp-annote/src/community1_cpp_annote_embedded.cpp`
- *... and 117 more*
