# Subsystem: voice

## android/java/main/java/ai/moonshine/voice/AssetDownloader.java
- Doc: AssetDownloader: Downloads the model/data files a Moonshine engine needs into an app-chosen...
- Layer: utility
- Language: java
- Symbols:
  - `AssetDownloader` (class, line 37)
  - `ProgressListener` (class, line 46)
  - `ResolvedFile` (class, line 118)
  - `AssetDownloader` (method, line 59)
  - `AssetDownloader` (method, line 69)
  - `isModelPresent` (method, line 74)
  - `ensureModelPresent` (method, line 97)
  - `resolveFiles` (method, line 126)
  - `filesFromGroupManifest` (method, line 158)
  - `filesFromKeyArray` (method, line 179)
  - `filesFromKeyList` (method, line 191)
  - `encodeKey` (method, line 205)
  - `downloadOne` (method, line 222)
  - `ensureSpaceAvailable` (method, line 305)

## android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java
- Doc: GraphemeToPhonemizer: Grapheme-to-phoneme (IPA) via the Moonshine native API.  <p>Aligns with...
- Layer: utility
- Language: java
- Symbols:
  - `GraphemeToPhonemizer` (class, line 12)
  - `GraphemeToPhonemizer` (method, line 22)
  - `GraphemeToPhonemizer` (method, line 38)
  - `fromMemory` (method, line 42)
  - `GraphemeToPhonemizer` (method, line 58)
  - `getG2pDependencies` (method, line 65)
  - `toArray` (method, line 68)
  - `getLanguage` (method, line 75)
  - `toIpa` (method, line 81)
  - `toIpa` (method, line 88)
  - `close` (method, line 92)
  - `finalize` (method, line 101)

## android/java/main/java/ai/moonshine/voice/IntentMatch.java
- Doc: IntentMatch: package ai.moonshine.voice; /** One ranked intent from {@link...
- Layer: utility
- Language: java
- Symbols:
  - `IntentMatch` (class, line 4)
  - `IntentMatch` (method, line 6)

## android/java/main/java/ai/moonshine/voice/IntentRecognizer.java
- Doc: IntentRecognizer: Semantic intent recognizer: registers canonical phrases and ranks them against...
- Layer: utility
- Language: java
- Symbols:
  - `IntentRecognizer` (class, line 11)
  - `IntentRecognizer` (method, line 18)
  - `IntentRecognizer` (method, line 26)
  - `getIntentDependencies` (method, line 42)
  - `finalize` (method, line 57)
  - `close` (method, line 64)
  - `registerIntent` (method, line 71)
  - `registerIntent` (method, line 83)
  - `calculateEmbedding` (method, line 97)
  - `unregisterIntent` (method, line 107)
  - `getClosestIntents` (method, line 118)
  - `getIntentCount` (method, line 128)
  - `clearIntents` (method, line 137)
  - `checkHandle` (method, line 145)

## android/java/main/java/ai/moonshine/voice/JNI.java
- Layer: utility
- Language: java
- Symbols:
  - `JNI` (class, line 3)
  - `ensureLibraryLoaded` (method, line 160)
- Imported by: `android/java/androidTest/java/ai/moonshine/voice/JNITest.java`, `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java`, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java`, `android/java/main/java/ai/moonshine/voice/Transcriber.java`, `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/MainActivity.kt`, `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java`

## android/java/main/java/ai/moonshine/voice/MicCaptureProcessor.java
- Doc: MicCaptureProcessor: Reads a stream of audio data from the microphone on a separate thread...
- Layer: business_logic
- Language: java
- Symbols:
  - `MicCaptureProcessor` (class, line 17)
  - `consumeAudio` (method, line 20)
  - `run` (method, line 40)

## android/java/main/java/ai/moonshine/voice/MicTranscriber.java
- Doc: loadFromAssets: These load* methods are overridden to complete the CompletableFuture when the...
- Layer: utility
- Language: java
- Symbols:
  - `MicTranscriber` (class, line 14)
  - `MicTranscriber` (method, line 20)
  - `loadFromAssets` (method, line 32)
  - `loadFromAssets` (method, line 37)
  - `loadFromFiles` (method, line 45)
  - `loadFromMemory` (method, line 50)
  - `loadFromMemory` (method, line 57)
  - `onMicPermissionGranted` (method, line 65)
  - `startProcessing` (method, line 69)
  - `startAudioProcessingLoop` (method, line 74)
  - `Thread` (method, line 77)
  - `run` (method, line 78)
  - `startMicCaptureLoop` (method, line 85)
  - `stop` (method, line 95)
  - `start` (method, line 100)
  - `audioProcessingLoop` (method, line 105)

## android/java/main/java/ai/moonshine/voice/ModelSpec.java
- Doc: ModelSpec: Describes which model's files {@link AssetDownloader} (or {@link...
- Layer: business_logic
- Language: java
- Symbols:
  - `ModelSpec` (class, line 16)
  - `ModelSpec` (method, line 30)
  - `stt` (method, line 42)
  - `stt` (method, line 47)
  - `tts` (method, line 53)
  - `intent` (method, line 58)
  - `g2p` (method, line 63)
  - `toOptions` (method, line 73)
- Imported by: `examples/android/TextToSpeech/app/src/main/java/ai/moonshine/examples/texttospeech/MainActivity.kt`

## android/java/main/java/ai/moonshine/voice/MoonshineDownloadWorker.java
- Doc: MoonshineDownloadWorker: Runs {@link AssetDownloader#ensureModelPresent} under WorkManager so...
- Layer: utility
- Language: java
- Symbols:
  - `MoonshineDownloadWorker` (class, line 32)
  - `MoonshineDownloadWorker` (method, line 55)
  - `buildRequest` (method, line 65)
  - `toInputData` (method, line 80)
  - `specFromData` (method, line 97)
  - `doWork` (method, line 119)

## android/java/main/java/ai/moonshine/voice/SpeakerSpan.java
- Doc: SpeakerSpan: One contiguous span of speech within a line attributed to a single speaker.
- Layer: utility
- Language: java
- Symbols:
  - `SpeakerSpan` (class, line 12)
  - `toString` (method, line 24)

## android/java/main/java/ai/moonshine/voice/TextToSpeech.java
- Doc: TextToSpeech: On-device text-to-speech via the Moonshine native API (Kokoro / Piper / ZipVoice...
- Layer: utility
- Language: java
- Symbols:
  - `TextToSpeech` (class, line 34)
  - `SayRequest` (class, line 49)
  - `PlayItem` (class, line 64)
  - `TextToSpeech` (method, line 98)
  - `TextToSpeech` (method, line 118)
  - `fromMemory` (method, line 126)
  - `fromZipVoiceClone` (method, line 153)
  - `floatPcmToLeBytes` (method, line 167)
  - `TextToSpeech` (method, line 176)
  - `getLanguage` (method, line 181)
  - `getG2pDependencies` (method, line 187)
  - `getTtsDependencies` (method, line 197)
  - `getTtsVoices` (method, line 207)
  - `toArray` (method, line 215)
  - `synthesize` (method, line 227)
  - `synthesize` (method, line 234)
  - `synthesizeFromPhonemes` (method, line 249)
  - `synthesizeFromPhonemes` (method, line 256)
  - `say` (method, line 270)
  - `say` (method, line 278)
  - `say` (method, line 286)
  - `say` (method, line 302)
  - `say` (method, line 309)
  - `waitUntilDone` (method, line 327)
  - `stop` (method, line 346)
  - `isTalking` (method, line 368)
  - `ensureWorkers` (method, line 373)
  - `synthWorker` (method, line 391)
  - `playWorker` (method, line 434)
  - `playOneItem` (method, line 459)
  - `playPcmFloat` (method, line 469)
  - `decrementPending` (method, line 508)
  - `drainQueue` (method, line 519)
  - `joinWorkers` (method, line 522)
  - `getAudioOutputDevices` (method, line 549)
  - `obtainSayTrackLocked` (method, line 560)
  - `buildAudioTrack` (method, line 604)
  - `releaseSayTrackLocked` (method, line 646)
  - `close` (method, line 659)
  - `finalize` (method, line 676)

## android/java/main/java/ai/moonshine/voice/Transcriber.java
- Doc: getTranscribeFlags: Sets the flags applied to subsequent transcription calls.
- Layer: utility
- Language: java
- Symbols:
  - `Transcriber` (class, line 28)
  - `Transcriber` (method, line 46)
  - `Transcriber` (method, line 48)
  - `setTranscribeFlags` (method, line 60)
  - `getTranscribeFlags` (method, line 61)
  - `getSttDependencies` (method, line 75)
  - `loadFromFiles` (method, line 88)
  - `loadFromMemory` (method, line 99)
  - `loadFromMemory` (method, line 113)
  - `loadFromAssets` (method, line 125)
  - `loadFromAssets` (method, line 140)
  - `finalize` (method, line 162)
  - `transcribeWithoutStreaming` (method, line 174)
  - `transcribeWithoutStreaming` (method, line 180)
  - `createStream` (method, line 186)
  - `freeStream` (method, line 190)
  - `startStream` (method, line 194)
  - `stopStream` (method, line 198)
  - `start` (method, line 210)
  - `stop` (method, line 212)
  - `addListener` (method, line 214)
  - `removeListener` (method, line 218)
  - `removeAllListeners` (method, line 222)
  - `addAudio` (method, line 224)
  - `addAudioToStream` (method, line 229)
  - `notifyFromTranscript` (method, line 242)
  - `emit` (method, line 276)
  - `getDefaultStreamHandle` (method, line 282)
  - `readAllBytes` (method, line 290)
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

## android/java/main/java/ai/moonshine/voice/TranscriberOption.java
- Layer: utility
- Language: java
- Symbols:
  - `TranscriberOption` (class, line 3)
  - `TranscriberOption` (method, line 5)
  - `name` (method, line 10)
  - `value` (method, line 14)
- Imported by: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java`, `android/java/main/java/ai/moonshine/voice/Transcriber.java`, `examples/android/TextToSpeech/app/src/main/java/ai/moonshine/examples/texttospeech/MainActivity.kt`

## android/java/main/java/ai/moonshine/voice/Transcript.java
- Layer: utility
- Language: java
- Symbols:
  - `Transcript` (class, line 5)
  - `text` (method, line 6)

## android/java/main/java/ai/moonshine/voice/TranscriptEvent.java
- Layer: infrastructure
- Language: java
- Symbols:
  - `TranscriptEvent` (class, line 3)
  - `Visitor` (class, line 4)
  - `LineStarted` (class, line 13)
  - `LineUpdated` (class, line 28)
  - `LineTextChanged` (class, line 43)
  - `LineSpeakersChanged` (class, line 65)
  - `LineCompleted` (class, line 79)
  - `Error` (class, line 94)
  - `LineStarted` (method, line 17)
  - `accept` (method, line 24)
  - `LineUpdated` (method, line 32)
  - `accept` (method, line 39)
  - `LineTextChanged` (method, line 47)
  - `accept` (method, line 54)
  - `LineSpeakersChanged` (method, line 68)
  - `accept` (method, line 75)
  - `LineCompleted` (method, line 83)
  - `accept` (method, line 90)
  - `Error` (method, line 98)
  - `accept` (method, line 105)
- Imported by: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java`, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java`, `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/MainActivity.kt`, `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java`

## android/java/main/java/ai/moonshine/voice/TranscriptEventListener.java
- Layer: infrastructure
- Language: java
- Symbols:
  - `TranscriptEventListener` (class, line 3)
  - `onLineStarted` (method, line 4)
  - `onLineUpdated` (method, line 5)
  - `onLineTextChanged` (method, line 6)
  - `onLineSpeakersChanged` (method, line 7)
  - `onLineCompleted` (method, line 8)
  - `onError` (method, line 9)

## android/java/main/java/ai/moonshine/voice/TranscriptLine.java
- Layer: utility
- Language: java
- Symbols:
  - `TranscriptLine` (class, line 5)
  - `toString` (method, line 29)
- Imported by: `android/java/androidTest/java/ai/moonshine/voice/JNITest.java`, `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java`, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java`

## android/java/main/java/ai/moonshine/voice/TtsSynthesisResult.java
- Doc: TtsSynthesisResult: package ai.moonshine.voice; /** PCM float samples (~-1..1) and sample rate...
- Layer: utility
- Language: java
- Symbols:
  - `TtsSynthesisResult` (class, line 4)
  - `TtsSynthesisResult` (method, line 6)
  - `TtsSynthesisResult` (method, line 8)

## android/java/main/java/ai/moonshine/voice/WordTiming.java
- Layer: utility
- Language: java
- Symbols:
  - `WordTiming` (class, line 3)
  - `toString` (method, line 7)
