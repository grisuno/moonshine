# Subsystem: MoonshineVoice

## swift/Sources/MoonshineVoice/AssetDownloadError.swift
- Layer: utility
- Language: swift

## swift/Sources/MoonshineVoice/AssetDownloader.swift
- Layer: utility
- Language: swift

## swift/Sources/MoonshineVoice/EmbeddingModelArch.swift
- Layer: business_logic
- Language: swift

## swift/Sources/MoonshineVoice/Errors.swift
- Doc: checkError: Helper function to check error codes and throw appropriate Swift errors
- Layer: utility
- Language: swift
- Symbols:
  - `checkError` (function, line 40)

## swift/Sources/MoonshineVoice/Events.swift
- Layer: infrastructure
- Language: swift

## swift/Sources/MoonshineVoice/IntentRecognizer.swift
- Layer: utility
- Language: swift

## swift/Sources/MoonshineVoice/MicTranscriber.swift
- Doc: feedCapturedAudio: Sink for a single captured audio buffer.
- Layer: utility
- Language: swift
- Symbols:
  - `feedCapturedAudio` (function, line 262)

## swift/Sources/MoonshineVoice/ModelArch.swift
- Layer: business_logic
- Language: swift

## swift/Sources/MoonshineVoice/MoonshineAPI.swift
- Doc: getVersion: Get the version of the loaded Moonshine library.
- Layer: presentation
- Language: swift
- Symbols:
  - `getVersion` (function, line 21)
  - `errorToString` (function, line 26)
  - `loadTranscriberFromFiles` (function, line 34)
  - `freeTranscriber` (function, line 93)
  - `transcribeWithoutStreaming` (function, line 98)
  - `createStream` (function, line 134)
  - `freeStream` (function, line 141)
  - `startStream` (function, line 147)
  - `stopStream` (function, line 153)
  - `addAudioToStream` (function, line 159)
  - `transcribeStream` (function, line 184)
  - `createTtsSynthesizerFromFiles` (function, line 305)
  - `createTtsSynthesizerFromMemory` (function, line 361)
  - `textToSpeech` (function, line 421)
  - `phonemesToSpeech` (function, line 485)
  - `freeTtsSynthesizer` (function, line 545)
  - `getTtsVoices` (function, line 550)
  - `getTtsDependencies` (function, line 600)
  - `getG2pDependencies` (function, line 650)
  - `getSttDependencies` (function, line 668)
  - `getIntentDependencies` (function, line 685)
  - `createIntentRecognizer` (function, line 744)
  - `freeIntentRecognizer` (function, line 761)
  - `registerIntentRecognizerIntent` (function, line 765)
  - `unregisterIntentRecognizerIntent` (function, line 775)
  - `getClosestIntents` (function, line 787)
  - `getIntentRecognizerIntentCount` (function, line 826)
  - `clearIntentRecognizerIntents` (function, line 834)
  - `calculateIntentEmbedding` (function, line 838)

## swift/Sources/MoonshineVoice/Stream.swift
- Layer: utility
- Language: swift

## swift/Sources/MoonshineVoice/TextToSpeech.swift
- Layer: utility
- Language: swift

## swift/Sources/MoonshineVoice/Transcriber.swift
- Layer: utility
- Language: swift

## swift/Sources/MoonshineVoice/Transcript.swift
- Layer: utility
- Language: swift

## swift/Sources/MoonshineVoice/TranscriptEventListener.swift
- Doc: onLineStarted: Called when a new transcription line starts.
- Layer: infrastructure
- Language: swift
- Symbols:
  - `onLineStarted` (function, line 10)
  - `onLineUpdated` (function, line 13)
  - `onLineTextChanged` (function, line 16)
  - `onLineSpeakersChanged` (function, line 20)
  - `onLineCompleted` (function, line 23)
  - `onError` (function, line 26)
  - `onLineStarted` (function, line 31)
  - `onLineUpdated` (function, line 32)
  - `onLineTextChanged` (function, line 33)
  - `onLineSpeakersChanged` (function, line 34)
  - `onLineCompleted` (function, line 35)
  - `onError` (function, line 36)

## swift/Sources/MoonshineVoice/TranscriptionStream.swift
- Doc: TranscriptionStream: The subset of ``Stream`` that ``MicTranscriber`` drives.
- Layer: utility
- Language: swift
- Symbols:
  - `TranscriptionStream` (protocol, line 9)
  - `start` (function, line 10)
  - `stop` (function, line 11)
  - `close` (function, line 12)
  - `addAudio` (function, line 13)
  - `addListener` (function, line 14)
  - `addListener` (function, line 15)
  - `removeListener` (function, line 16)
  - `removeListener` (function, line 17)
  - `removeAllListeners` (function, line 18)
- Imported by: `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift::FakeStream`

## swift/Sources/MoonshineVoice/TtsSynthesisResult.swift
- Layer: utility
- Language: swift

## swift/Sources/MoonshineVoice/WAVLoader.swift
- Layer: utility
- Language: swift
