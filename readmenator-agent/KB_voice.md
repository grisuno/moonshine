# Subsystem: voice

## android/java/androidTest/java/ai/moonshine/voice/AssetDownloaderTest.java
- Layer: testing
- Language: java
- Symbols:
  - `AssetDownloaderTest` (class, line 35)
  - `setUp` (method, line 39)
  - `downloadsEnabled` (method, line 49)
  - `testDownloadsAndRunsSttModel` (method, line 61)
  - `testDownloadsAndRunsTtsVoice` (method, line 91)
  - `testDownloadsAndRunsIntentModel` (method, line 112)

## android/java/androidTest/java/ai/moonshine/voice/IntentRecognizerTest.java
- Layer: testing
- Language: java
- Symbols:
  - `IntentRecognizerTest` (class, line 13)
  - `testCreateIntentRecognizer_invalidPath_throws` (method, line 15)
  - `testGetClosestIntents_whenModelPresent` (method, line 22)

## android/java/androidTest/java/ai/moonshine/voice/JNITest.java
- Layer: testing
- Language: java
- Symbols:
  - `JNITest` (class, line 28)
  - `setUp` (method, line 32)
  - `testMoonshineGetVersion` (method, line 43)
  - `testMoonshineGetG2pDependencies` (method, line 48)
  - `testMoonshineErrorToString` (method, line 55)
  - `testMoonshineTranscriptToString` (method, line 60)
  - `testMoonshineLoadTranscriber` (method, line 81)
  - `testMoonshineTranscribe` (method, line 112)
  - `testMoonshineStreaming` (method, line 148)
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

## android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java
- Layer: testing
- Language: java
- Symbols:
  - `NoTranscriptionTest` (class, line 29)
  - `setUp` (method, line 37)
  - `testMoonshineNoTranscription` (method, line 47)
  - `TranscriptEventListener` (method, line 70)
  - `onLineStarted` (method, line 71)
  - `onLineUpdated` (method, line 76)
  - `onLineTextChanged` (method, line 81)
  - `onLineCompleted` (method, line 86)
  - `onError` (method, line 91)
  - `onLineStartedEvent` (method, line 111)
  - `onLineUpdatedEvent` (method, line 120)
  - `onLineTextChangedEvent` (method, line 128)
  - `onLineCompletedEvent` (method, line 134)
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

## android/java/androidTest/java/ai/moonshine/voice/TextToSpeechTest.java
- Layer: testing
- Language: java
- Symbols:
  - `TextToSpeechTest` (class, line 27)
  - `setUp` (method, line 28)
  - `testZipVoiceDependencies` (method, line 33)
  - `testZipVoiceVoicesListing` (method, line 49)
  - `findZipVoiceRoot` (method, line 63)
  - `testZipVoiceBuiltinVoiceSynthesizes` (method, line 97)
  - `testZipVoiceClonePcmSynthesizes` (method, line 114)

## android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java
- Layer: testing
- Language: java
- Symbols:
  - `TranscriberTest` (class, line 33)
  - `setUp` (method, line 43)
  - `testMoonshineTranscriberStreaming` (method, line 53)
  - `TranscriptEventListener` (method, line 82)
  - `onLineStarted` (method, line 83)
  - `onLineUpdated` (method, line 88)
  - `onLineTextChanged` (method, line 93)
  - `onLineCompleted` (method, line 98)
  - `onError` (method, line 103)
  - `onLineStartedEvent` (method, line 126)
  - `onLineUpdatedEvent` (method, line 134)
  - `onLineTextChangedEvent` (method, line 141)
  - `onLineCompletedEvent` (method, line 153)
  - `testMoonshineTranscriberWithoutStreaming` (method, line 165)
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

## android/java/androidTest/java/ai/moonshine/voice/Utils.java
- Layer: testing
- Language: java
- Symbols:
  - `Utils` (class, line 18)
  - `WavData` (class, line 116)
  - `logStats` (method, line 22)
  - `removePunctuation` (method, line 58)
  - `normalizedEditDistance` (method, line 80)
  - `WavData` (method, line 118)
  - `loadWavFromAssets` (method, line 128)
  - `loadAsset` (method, line 174)
  - `copyAssetToTempDir` (method, line 186)
