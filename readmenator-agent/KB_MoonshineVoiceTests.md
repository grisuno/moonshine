# Subsystem: MoonshineVoiceTests

## swift/Tests/MoonshineVoiceTests/AssetDownloaderNetworkTests.swift
- Layer: testing
- Language: swift
- Symbols:
  - `AssetDownloaderNetworkTests` (class, line 16)
  - `setUpWithError` (function, line 19)
  - `tearDown` (function, line 27)
  - `testDownloadsAndRunsSttModel` (function, line 49)
  - `testDownloadsAndRunsTtsVoice` (function, line 76)
  - `testDownloadsAndRunsIntentModel` (function, line 96)

## swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift
- Layer: testing
- Language: swift
- Symbols:
  - `AssetDownloaderTests` (class, line 10)
  - `MockURLProtocol` (class, line 258)
  - `RecordedRequest` (struct, line 250)
  - `setUp` (function, line 13)
  - `tearDown` (function, line 22)
  - `testDownloadsSttModelIntoEmptyDirectory` (function, line 93)
  - `testSkipsAlreadyPresentFiles` (function, line 107)
  - `testIncludeSpellingAddsFilesForEnglish` (function, line 122)
  - `testDownloadsIntentModel` (function, line 144)
  - `testDownloadsTtsAssetsIntoNestedPaths` (function, line 153)
  - `testReportsProgress` (function, line 163)
  - `testHttpErrorSurfacesAsAssetDownloadError` (function, line 177)
  - `testResumesFromPartialDownload` (function, line 196)
  - `record` (function, line 237)
  - `canInit` (function, line 285)
  - `canonicalRequest` (function, line 287)
  - `startLoading` (function, line 288)
  - `stopLoading` (function, line 306)

## swift/Tests/MoonshineVoiceTests/IntentRecognizerTests.swift
- Layer: testing
- Language: swift
- Symbols:
  - `IntentRecognizerTests` (class, line 5)
  - `testCreateIntentRecognizer_invalidPath_throws` (function, line 7)
  - `testIntentRecognizer_closestIntents_whenEmbeddingModelPresent` (function, line 21)

## swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift
- Layer: infrastructure
- Language: swift
- Symbols:
  - `MicTranscriberThreadingTests` (class, line 21)
  - `FakeStream` (class, line 35)
  - `start` (function, line 51)
  - `close` (function, line 53)
  - `stop` (function, line 56)
  - `addAudio` (function, line 57)
  - `addListener` (function, line 78)
  - `addListener` (function, line 80)
  - `removeListener` (function, line 81)
  - `removeListener` (function, line 82)
  - `removeAllListeners` (function, line 83)
  - `testCaptureCallbackIsNotBlockedByTranscription` (function, line 95)

## swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift
- Layer: testing
- Language: swift
- Symbols:
  - `TextToSpeechTests` (class, line 5)
  - `testCreateSynthesizer` (function, line 36)
  - `testCreateSynthesizerWithVoice` (function, line 44)
  - `testCreateSynthesizerInvalidLanguage` (function, line 56)
  - `testSynthesizeBasic` (function, line 68)
  - `testSynthesizeLongerText` (function, line 80)
  - `testSynthesizeWithVoiceOption` (function, line 100)
  - `testSynthesizeWithSpeedOption` (function, line 115)
  - `testSynthesizeSampleRange` (function, line 135)
  - `testSynthesizeMultipleCalls` (function, line 151)
  - `testSayDefaultDevice` (function, line 169)
  - `testSayMultipleCalls` (function, line 180)
  - `testGetVoices` (function, line 194)
  - `testGetDependencies` (function, line 207)
  - `any` (function, line 225)
  - `testGetVoicesListsZipVoice` (function, line 233)
  - `testZipVoiceBuiltinVoiceSynthesizes` (function, line 246)
  - `testZipVoiceClonePCMSynthesizes` (function, line 258)
  - `testGetAudioOutputDevices` (function, line 282)
  - `testCloseIdempotent` (function, line 296)

## swift/Tests/MoonshineVoiceTests/TranscriberTests.swift
- Layer: testing
- Language: swift
- Symbols:
  - `TranscriberTests` (class, line 5)
  - `testTranscribeWithoutStreaming_beckett` (function, line 52)
  - `testTranscribeWithoutStreaming_twoCities` (function, line 80)
  - `testTranscribeWithoutStreaming_emptyAudio` (function, line 108)
  - `testTranscribeWithStreaming` (function, line 126)
  - `testTranscribeWithStreamingAll` (function, line 200)
  - `testTranscribeWithStreaming_manualUpdates` (function, line 205)
  - `testTranscribeWithStreaming_emptyAudio` (function, line 233)
  - `testGetVersion` (function, line 256)
  - `testFrameworkBundle` (function, line 267)
  - `testSpellingModeApiSurface` (function, line 276)
  - `testTranscribeWithDebugWAV_twoCities` (function, line 311)
