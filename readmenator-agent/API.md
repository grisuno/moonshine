# API

## android/java/androidTest/java/ai/moonshine/voice/AssetDownloaderTest.java

### setUp
- Defined: `android/java/androidTest/java/ai/moonshine/voice/AssetDownloaderTest.java:39`

### downloadsEnabled
- Defined: `android/java/androidTest/java/ai/moonshine/voice/AssetDownloaderTest.java:49`

### testDownloadsAndRunsSttModel
- Defined: `android/java/androidTest/java/ai/moonshine/voice/AssetDownloaderTest.java:61`

### testDownloadsAndRunsTtsVoice
- Defined: `android/java/androidTest/java/ai/moonshine/voice/AssetDownloaderTest.java:91`

### testDownloadsAndRunsIntentModel
- Defined: `android/java/androidTest/java/ai/moonshine/voice/AssetDownloaderTest.java:112`

## android/java/androidTest/java/ai/moonshine/voice/IntentRecognizerTest.java

### testCreateIntentRecognizer_invalidPath_throws
- Defined: `android/java/androidTest/java/ai/moonshine/voice/IntentRecognizerTest.java:15`

### testGetClosestIntents_whenModelPresent
- Defined: `android/java/androidTest/java/ai/moonshine/voice/IntentRecognizerTest.java:22`

## android/java/androidTest/java/ai/moonshine/voice/JNITest.java

### setUp
- Defined: `android/java/androidTest/java/ai/moonshine/voice/JNITest.java:32`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### testMoonshineGetVersion
- Defined: `android/java/androidTest/java/ai/moonshine/voice/JNITest.java:43`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### testMoonshineGetG2pDependencies
- Defined: `android/java/androidTest/java/ai/moonshine/voice/JNITest.java:48`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### testMoonshineErrorToString
- Defined: `android/java/androidTest/java/ai/moonshine/voice/JNITest.java:55`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### testMoonshineTranscriptToString
- Defined: `android/java/androidTest/java/ai/moonshine/voice/JNITest.java:60`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### testMoonshineLoadTranscriber
- Defined: `android/java/androidTest/java/ai/moonshine/voice/JNITest.java:81`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### testMoonshineTranscribe
- Defined: `android/java/androidTest/java/ai/moonshine/voice/JNITest.java:112`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### testMoonshineStreaming
- Defined: `android/java/androidTest/java/ai/moonshine/voice/JNITest.java:148`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

## android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java

### setUp
- Defined: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java:37`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### testMoonshineNoTranscription
- Defined: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java:47`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### TranscriptEventListener
- Defined: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java:70`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### onLineStarted
- Defined: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java:71`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### onLineUpdated
- Defined: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java:76`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### onLineTextChanged
- Defined: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java:81`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### onLineCompleted
- Defined: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java:86`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### onError
- Defined: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java:91`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### onLineStartedEvent
- Defined: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java:111`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### onLineUpdatedEvent
- Defined: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java:120`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### onLineTextChangedEvent
- Defined: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java:128`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### onLineCompletedEvent
- Defined: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java:134`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

## android/java/androidTest/java/ai/moonshine/voice/TextToSpeechTest.java

### setUp
- Defined: `android/java/androidTest/java/ai/moonshine/voice/TextToSpeechTest.java:28`

### testZipVoiceDependencies
- Defined: `android/java/androidTest/java/ai/moonshine/voice/TextToSpeechTest.java:33`

### testZipVoiceVoicesListing
- Defined: `android/java/androidTest/java/ai/moonshine/voice/TextToSpeechTest.java:49`

### findZipVoiceRoot
- Defined: `android/java/androidTest/java/ai/moonshine/voice/TextToSpeechTest.java:63`

### testZipVoiceBuiltinVoiceSynthesizes
- Defined: `android/java/androidTest/java/ai/moonshine/voice/TextToSpeechTest.java:97`

### testZipVoiceClonePcmSynthesizes
- Defined: `android/java/androidTest/java/ai/moonshine/voice/TextToSpeechTest.java:114`

## android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java

### setUp
- Defined: `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java:43`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### testMoonshineTranscriberStreaming
- Defined: `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java:53`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### TranscriptEventListener
- Defined: `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java:82`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### onLineStarted
- Defined: `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java:83`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### onLineUpdated
- Defined: `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java:88`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### onLineTextChanged
- Defined: `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java:93`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### onLineCompleted
- Defined: `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java:98`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### onError
- Defined: `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java:103`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### onLineStartedEvent
- Defined: `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java:126`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### onLineUpdatedEvent
- Defined: `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java:134`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### onLineTextChangedEvent
- Defined: `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java:141`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### onLineCompletedEvent
- Defined: `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java:153`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

### testMoonshineTranscriberWithoutStreaming
- Defined: `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java:165`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`, `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`

## android/java/androidTest/java/ai/moonshine/voice/Utils.java

### logStats
- Defined: `android/java/androidTest/java/ai/moonshine/voice/Utils.java:22`

### removePunctuation
- Defined: `android/java/androidTest/java/ai/moonshine/voice/Utils.java:58`

### normalizedEditDistance
- Defined: `android/java/androidTest/java/ai/moonshine/voice/Utils.java:80`

### WavData
- Defined: `android/java/androidTest/java/ai/moonshine/voice/Utils.java:118`

### loadWavFromAssets
- Defined: `android/java/androidTest/java/ai/moonshine/voice/Utils.java:128`

### loadAsset
- Defined: `android/java/androidTest/java/ai/moonshine/voice/Utils.java:174`

### copyAssetToTempDir
- Defined: `android/java/androidTest/java/ai/moonshine/voice/Utils.java:186`

## android/java/main/java/ai/moonshine/voice/AssetDownloader.java

### AssetDownloader
- Defined: `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:59`

### AssetDownloader
- Defined: `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:69`

### isModelPresent
- Defined: `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:74`

### ensureModelPresent
- Defined: `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:97`

### resolveFiles
- Defined: `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:126`

### filesFromGroupManifest
- Defined: `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:158`

### filesFromKeyArray
- Defined: `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:179`

### filesFromKeyList
- Defined: `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:191`

### encodeKey
- Defined: `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:205`

### downloadOne
- Defined: `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:222`

### ensureSpaceAvailable
- Defined: `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:305`

## android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java

### GraphemeToPhonemizer
- Defined: `android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java:22`

### GraphemeToPhonemizer
- Defined: `android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java:38`

### fromMemory
- Defined: `android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java:42`

### GraphemeToPhonemizer
- Defined: `android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java:58`

### getG2pDependencies
- Defined: `android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java:65`

### toArray
- Defined: `android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java:68`

### getLanguage
- Defined: `android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java:75`

### toIpa
- Defined: `android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java:81`

### toIpa
- Defined: `android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java:88`

### close
- Defined: `android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java:92`

### finalize
- Defined: `android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java:101`

## android/java/main/java/ai/moonshine/voice/IntentMatch.java

### IntentMatch
- Defined: `android/java/main/java/ai/moonshine/voice/IntentMatch.java:6`

## android/java/main/java/ai/moonshine/voice/IntentRecognizer.java

### IntentRecognizer
- Defined: `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java:18`

### IntentRecognizer
- Defined: `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java:26`

### getIntentDependencies
- Defined: `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java:42`

### finalize
- Defined: `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java:57`

### close
- Defined: `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java:64`

### registerIntent
- Defined: `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java:71`

### registerIntent
- Defined: `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java:83`

### calculateEmbedding
- Defined: `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java:97`

### unregisterIntent
- Defined: `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java:107`

### getClosestIntents
- Defined: `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java:118`

### getIntentCount
- Defined: `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java:128`

### clearIntents
- Defined: `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java:137`

### checkHandle
- Defined: `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java:145`

## android/java/main/java/ai/moonshine/voice/JNI.java

### ensureLibraryLoaded
- Defined: `android/java/main/java/ai/moonshine/voice/JNI.java:160`
- Imported by: `android/java/androidTest/java/ai/moonshine/voice/JNITest.java`, `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java`, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java`, `android/java/main/java/ai/moonshine/voice/Transcriber.java`, `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/MainActivity.kt`, `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java`

## android/java/main/java/ai/moonshine/voice/MicCaptureProcessor.java

### consumeAudio
- Defined: `android/java/main/java/ai/moonshine/voice/MicCaptureProcessor.java:20`

### run
- Defined: `android/java/main/java/ai/moonshine/voice/MicCaptureProcessor.java:40`

## android/java/main/java/ai/moonshine/voice/MicTranscriber.java

### MicTranscriber
- Defined: `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:20`

### loadFromAssets
- Defined: `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:32`
- Doc: These load* methods are overridden to complete the CompletableFuture when the transcriber is loaded, so we can continue 

### loadFromAssets
- Defined: `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:37`

### loadFromFiles
- Defined: `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:45`

### loadFromMemory
- Defined: `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:50`

### loadFromMemory
- Defined: `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:57`

### onMicPermissionGranted
- Defined: `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:65`

### startProcessing
- Defined: `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:69`

### startAudioProcessingLoop
- Defined: `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:74`

### Thread
- Defined: `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:77`

### run
- Defined: `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:78`

### startMicCaptureLoop
- Defined: `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:85`

### stop
- Defined: `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:95`

### start
- Defined: `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:100`

### audioProcessingLoop
- Defined: `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:105`

## android/java/main/java/ai/moonshine/voice/ModelSpec.java

### ModelSpec
- Defined: `android/java/main/java/ai/moonshine/voice/ModelSpec.java:30`
- Doc: public final class ModelSpec { public enum Type { STT, TTS, INTENT, G2P } public final Type type; /** Language code / En
- Imported by: `examples/android/TextToSpeech/app/src/main/java/ai/moonshine/examples/texttospeech/MainActivity.kt`

### stt
- Defined: `android/java/main/java/ai/moonshine/voice/ModelSpec.java:42`
- Imported by: `examples/android/TextToSpeech/app/src/main/java/ai/moonshine/examples/texttospeech/MainActivity.kt`

### stt
- Defined: `android/java/main/java/ai/moonshine/voice/ModelSpec.java:47`
- Imported by: `examples/android/TextToSpeech/app/src/main/java/ai/moonshine/examples/texttospeech/MainActivity.kt`

### tts
- Defined: `android/java/main/java/ai/moonshine/voice/ModelSpec.java:53`
- Imported by: `examples/android/TextToSpeech/app/src/main/java/ai/moonshine/examples/texttospeech/MainActivity.kt`

### intent
- Defined: `android/java/main/java/ai/moonshine/voice/ModelSpec.java:58`
- Imported by: `examples/android/TextToSpeech/app/src/main/java/ai/moonshine/examples/texttospeech/MainActivity.kt`

### g2p
- Defined: `android/java/main/java/ai/moonshine/voice/ModelSpec.java:63`
- Imported by: `examples/android/TextToSpeech/app/src/main/java/ai/moonshine/examples/texttospeech/MainActivity.kt`

### toOptions
- Defined: `android/java/main/java/ai/moonshine/voice/ModelSpec.java:73`
- Imported by: `examples/android/TextToSpeech/app/src/main/java/ai/moonshine/examples/texttospeech/MainActivity.kt`

## android/java/main/java/ai/moonshine/voice/MoonshineDownloadWorker.java

### MoonshineDownloadWorker
- Defined: `android/java/main/java/ai/moonshine/voice/MoonshineDownloadWorker.java:55`

### buildRequest
- Defined: `android/java/main/java/ai/moonshine/voice/MoonshineDownloadWorker.java:65`

### toInputData
- Defined: `android/java/main/java/ai/moonshine/voice/MoonshineDownloadWorker.java:80`

### specFromData
- Defined: `android/java/main/java/ai/moonshine/voice/MoonshineDownloadWorker.java:97`

### doWork
- Defined: `android/java/main/java/ai/moonshine/voice/MoonshineDownloadWorker.java:119`

## android/java/main/java/ai/moonshine/voice/SpeakerSpan.java

### toString
- Defined: `android/java/main/java/ai/moonshine/voice/SpeakerSpan.java:24`
- Doc: TranscriptLine.haveSpeakersChanged to detect revisions.  public class SpeakerSpan { /** Time offset from the start of th

## android/java/main/java/ai/moonshine/voice/TextToSpeech.java

### TextToSpeech
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:98`

### TextToSpeech
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:118`

### fromMemory
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:126`

### fromZipVoiceClone
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:153`

### floatPcmToLeBytes
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:167`

### TextToSpeech
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:176`

### getLanguage
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:181`

### getG2pDependencies
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:187`

### getTtsDependencies
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:197`

### getTtsVoices
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:207`

### toArray
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:215`

### synthesize
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:227`

### synthesize
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:234`

### synthesizeFromPhonemes
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:249`

### synthesizeFromPhonemes
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:256`

### say
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:270`

### say
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:278`

### say
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:286`
- Doc: Queue {@code text} for synthesis and playback with options, returning immediately.

### say
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:302`

### say
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:309`

### waitUntilDone
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:327`

### stop
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:346`

### isTalking
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:368`

### ensureWorkers
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:373`

### synthWorker
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:391`

### playWorker
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:434`

### playOneItem
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:459`

### playPcmFloat
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:469`

### decrementPending
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:508`

### drainQueue
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:519`

### joinWorkers
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:522`

### getAudioOutputDevices
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:549`

### obtainSayTrackLocked
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:560`

### buildAudioTrack
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:604`

### releaseSayTrackLocked
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:646`

### close
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:659`

### finalize
- Defined: `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:676`

## android/java/main/java/ai/moonshine/voice/Transcriber.java

### Transcriber
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:46`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### Transcriber
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:48`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### setTranscribeFlags
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:60`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### getTranscribeFlags
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:61`
- Doc: Sets the flags applied to subsequent transcription calls. Callers can {@code OR} {@link JNI#MOONSHINE_FLAG_SPELLING_MODE
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### getSttDependencies
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:75`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### loadFromFiles
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:88`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### loadFromMemory
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:99`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### loadFromMemory
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:113`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### loadFromAssets
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:125`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### loadFromAssets
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:140`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### finalize
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:162`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### transcribeWithoutStreaming
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:174`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### transcribeWithoutStreaming
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:180`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### createStream
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:186`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### freeStream
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:190`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### startStream
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:194`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### stopStream
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:198`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### start
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:210`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### stop
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:212`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### addListener
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:214`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### removeListener
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:218`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### removeAllListeners
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:222`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### addAudio
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:224`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### addAudioToStream
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:229`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### notifyFromTranscript
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:242`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### emit
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:276`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### getDefaultStreamHandle
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:282`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

### readAllBytes
- Defined: `android/java/main/java/ai/moonshine/voice/Transcriber.java:290`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`

## android/java/main/java/ai/moonshine/voice/TranscriberOption.java

### TranscriberOption
- Defined: `android/java/main/java/ai/moonshine/voice/TranscriberOption.java:5`
- Imported by: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java`, `android/java/main/java/ai/moonshine/voice/Transcriber.java`, `examples/android/TextToSpeech/app/src/main/java/ai/moonshine/examples/texttospeech/MainActivity.kt`

### name
- Defined: `android/java/main/java/ai/moonshine/voice/TranscriberOption.java:10`
- Imported by: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java`, `android/java/main/java/ai/moonshine/voice/Transcriber.java`, `examples/android/TextToSpeech/app/src/main/java/ai/moonshine/examples/texttospeech/MainActivity.kt`

### value
- Defined: `android/java/main/java/ai/moonshine/voice/TranscriberOption.java:14`
- Imported by: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java`, `android/java/main/java/ai/moonshine/voice/Transcriber.java`, `examples/android/TextToSpeech/app/src/main/java/ai/moonshine/examples/texttospeech/MainActivity.kt`

## android/java/main/java/ai/moonshine/voice/Transcript.java

### text
- Defined: `android/java/main/java/ai/moonshine/voice/Transcript.java:6`

## android/java/main/java/ai/moonshine/voice/TranscriptEvent.java

### LineStarted
- Defined: `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java:17`
- Imported by: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java`, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java`, `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/MainActivity.kt`, `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java`

### accept
- Defined: `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java:24`
- Imported by: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java`, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java`, `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/MainActivity.kt`, `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java`

### LineUpdated
- Defined: `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java:32`
- Imported by: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java`, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java`, `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/MainActivity.kt`, `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java`

### accept
- Defined: `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java:39`
- Imported by: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java`, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java`, `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/MainActivity.kt`, `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java`

### LineTextChanged
- Defined: `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java:47`
- Imported by: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java`, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java`, `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/MainActivity.kt`, `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java`

### accept
- Defined: `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java:54`
- Imported by: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java`, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java`, `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/MainActivity.kt`, `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java`

### LineSpeakersChanged
- Defined: `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java:68`
- Imported by: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java`, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java`, `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/MainActivity.kt`, `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java`

### accept
- Defined: `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java:75`
- Imported by: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java`, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java`, `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/MainActivity.kt`, `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java`

### LineCompleted
- Defined: `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java:83`
- Imported by: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java`, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java`, `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/MainActivity.kt`, `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java`

### accept
- Defined: `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java:90`
- Imported by: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java`, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java`, `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/MainActivity.kt`, `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java`

### Error
- Defined: `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java:98`
- Imported by: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java`, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java`, `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/MainActivity.kt`, `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java`

### accept
- Defined: `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java:105`
- Imported by: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java`, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java`, `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/MainActivity.kt`, `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java`

## android/java/main/java/ai/moonshine/voice/TranscriptEventListener.java

### onLineStarted
- Defined: `android/java/main/java/ai/moonshine/voice/TranscriptEventListener.java:4`

### onLineUpdated
- Defined: `android/java/main/java/ai/moonshine/voice/TranscriptEventListener.java:5`

### onLineTextChanged
- Defined: `android/java/main/java/ai/moonshine/voice/TranscriptEventListener.java:6`

### onLineSpeakersChanged
- Defined: `android/java/main/java/ai/moonshine/voice/TranscriptEventListener.java:7`

### onLineCompleted
- Defined: `android/java/main/java/ai/moonshine/voice/TranscriptEventListener.java:8`

### onError
- Defined: `android/java/main/java/ai/moonshine/voice/TranscriptEventListener.java:9`

## android/java/main/java/ai/moonshine/voice/TranscriptLine.java

### toString
- Defined: `android/java/main/java/ai/moonshine/voice/TranscriptLine.java:29`
- Imported by: `android/java/androidTest/java/ai/moonshine/voice/JNITest.java`, `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java`, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java`

## android/java/main/java/ai/moonshine/voice/TtsSynthesisResult.java

### TtsSynthesisResult
- Defined: `android/java/main/java/ai/moonshine/voice/TtsSynthesisResult.java:6`

### TtsSynthesisResult
- Defined: `android/java/main/java/ai/moonshine/voice/TtsSynthesisResult.java:8`

## android/java/main/java/ai/moonshine/voice/WordTiming.java

### toString
- Defined: `android/java/main/java/ai/moonshine/voice/WordTiming.java:7`

## android/java/test/java/ai/moonshine/voice/ExampleUnitTest.java

### addition_isCorrect
- Defined: `android/java/test/java/ai/moonshine/voice/ExampleUnitTest.java:13`

## android/moonshine-jni/moonshine-jni.cpp

### get_class `static jclass get_class(JNIEnv *env, const char *className)`
- Defined: `android/moonshine-jni/moonshine-jni.cpp:18`
- Doc: include "moonshine-c-api.h" include "utf8.h"

### get_field `static jfieldID get_field(JNIEnv *env, jclass clazz, const char *fieldName,
                     ...`
- Defined: `android/moonshine-jni/moonshine-jni.cpp:26`

### get_method `static jmethodID get_method(JNIEnv *env, jclass clazz, const char *methodName,
                  ...`
- Defined: `android/moonshine-jni/moonshine-jni.cpp:35`

### c_transcript_from_jobject `static std::unique_ptr<transcript_t> c_transcript_from_jobject(
    JNIEnv *env, jobject javaTran...`
- Defined: `android/moonshine-jni/moonshine-jni.cpp:45`

### c_transcript_to_jobject `static jobject c_transcript_to_jobject(JNIEnv *env, struct transcript_t *transcript)`
- Defined: `android/moonshine-jni/moonshine-jni.cpp:111`

### fill_moonshine_options `static bool fill_moonshine_options(
    JNIEnv *env, jobjectArray joptions, std::vector<moonshine...`
- Defined: `android/moonshine-jni/moonshine-jni.cpp:264`

### release_moonshine_options `static void release_moonshine_options(
    JNIEnv *env, const std::vector<moonshine_option_t> &co...`
- Defined: `android/moonshine-jni/moonshine-jni.cpp:299`

## core/benchmark.cpp

### AudioProducer `public:
  AudioProducer(std::string wav_path, float chunk_duration_seconds = 0.0214f)
      : cur...`
- Defined: `core/benchmark.cpp:12`

### getNextAudio `bool getNextAudio(std::vector<float> &out_audio_data)`
- Defined: `core/benchmark.cpp:18`

### sample_rate `int32_t sample_rate() const`
- Defined: `core/benchmark.cpp:30`

### audio_data_size `size_t audio_data_size() const`
- Defined: `core/benchmark.cpp:31`

### main `int main(int argc, char *argv[])`
- Defined: `core/benchmark.cpp:42`

### loadWavData `void AudioProducer::loadWavData(std::string wav_path)`
- Defined: `core/benchmark.cpp:108`

## core/bin-tokenizer/bin-tokenizer-test.cpp

### TEST_CASE `TEST_CASE("bin-tokenizer")`
- Defined: `core/bin-tokenizer/bin-tokenizer-test.cpp:10`
- Doc: define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN include <doctest.h>

### SUBCASE `SUBCASE("constructor-from-path")`
- Defined: `core/bin-tokenizer/bin-tokenizer-test.cpp:12`

### SUBCASE `SUBCASE("constructor-from-data")`
- Defined: `core/bin-tokenizer/bin-tokenizer-test.cpp:26`

## core/bin-tokenizer/bin-tokenizer.cpp

### BinTokenizer `BinTokenizer::BinTokenizer(const char *tokenizer_path,
                           const char *spa...`
- Defined: `core/bin-tokenizer/bin-tokenizer.cpp:11`
- Doc: include "debug-utils.h" include "file-utils.h" include "string-utils.h"

### BinTokenizer `BinTokenizer::BinTokenizer(const uint8_t *tokenizer_data,
                           size_t token...`
- Defined: `core/bin-tokenizer/bin-tokenizer.cpp:49`

### BinTokenizer `BinTokenizer::BinTokenizer(const char *tokenizer_path,
                           AAssetManager *...`
- Defined: `core/bin-tokenizer/bin-tokenizer.cpp:106`
- Doc: if defined(ANDROID)

### text_to_special_token `template <typename T>
T BinTokenizer::text_to_special_token(const std::string &text)`
- Defined: `core/bin-tokenizer/bin-tokenizer.cpp:146`
- Doc: endif

### text_to_tokens `template <typename T>
std::vector<T> BinTokenizer::text_to_tokens(const std::string &text)`
- Defined: `core/bin-tokenizer/bin-tokenizer.cpp:172`
- Doc: Uses a naive algorithm to encode text into tokens. This is not the most efficient way to do it, but it's functional and 

### tokens_to_text `template <typename T>
std::string BinTokenizer::tokens_to_text(const std::vector<T> &tokens,
    ...`
- Defined: `core/bin-tokenizer/bin-tokenizer.cpp:220`

## core/cosine-distance-test.cpp

### TEST_CASE `TEST_CASE("cosine-distance")`
- Defined: `core/cosine-distance-test.cpp:7`
- Doc: define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN include <doctest.h>

### SUBCASE `SUBCASE("identical vectors give zero distance")`
- Defined: `core/cosine-distance-test.cpp:9`

### SUBCASE `SUBCASE("orthogonal vectors give distance one")`
- Defined: `core/cosine-distance-test.cpp:14`

### SUBCASE `SUBCASE("opposite vectors give distance two")`
- Defined: `core/cosine-distance-test.cpp:20`

### SUBCASE `SUBCASE("mismatched length throws")`
- Defined: `core/cosine-distance-test.cpp:26`

### SUBCASE `SUBCASE("zero vector gives zero distance")`
- Defined: `core/cosine-distance-test.cpp:32`

### SUBCASE `SUBCASE("matches scipy implementation")`
- Defined: `core/cosine-distance-test.cpp:38`

## core/cosine-distance.cpp

### cosine_distance `float cosine_distance(const std::vector<float>& a,
                      const std::vector<float>...`
- Defined: `core/cosine-distance.cpp:5`
- Doc: include <cmath> include <stdexcept>

## core/cpp-annote/src/annotation_support.h

### empty `bool empty() const`
- Defined: `core/cpp-annote/src/annotation_support.h:27`

### duration `double duration() const`
- Defined: `core/cpp-annote/src/annotation_support.h:29`

### segment_union `inline Segment segment_union(const Segment& a, const Segment& b)`
- Defined: `core/cpp-annote/src/annotation_support.h:37`
- Doc: Union (|): covers both segments including any gap between them.

### segment_gap `inline Segment segment_gap(const Segment& self_, const Segment& other)`
- Defined: `core/cpp-annote/src/annotation_support.h:49`
- Doc: Gap (^): self is first operand, other is second (matches Python `self ^ other`).

### timeline_support_sorted `inline std::vector<Segment> timeline_support_sorted(
    const std::vector<Segment>& segments, do...`
- Defined: `core/cpp-annote/src/annotation_support.h:60`
- Doc: Timeline.support_iter / Timeline.support(collar) `segments` must be sorted by increasing start (Timeline order).

### sort `std::sort(segs.begin(), segs.end(), [](const Segment& x, const Segment& y)`
- Defined: `core/cpp-annote/src/annotation_support.h:66`

## core/cpp-annote/src/clustering_vbx.cpp

### row_normalize `void row_normalize(Eigen::MatrixXd& M)`
- Defined: `core/cpp-annote/src/clustering_vbx.cpp:21`

### cdist_cosine `void cdist_cosine(const Eigen::MatrixXd& X, const Eigen::MatrixXd& C,
                  Eigen::Ma...`
- Defined: `core/cpp-annote/src/clustering_vbx.cpp:30`

### kmeans_fit_predict `std::vector<int> kmeans_fit_predict(const Eigen::MatrixXd& Xnorm, int k,
                        ...`
- Defined: `core/cpp-annote/src/clustering_vbx.cpp:49`

### centroids_from_labels `Eigen::MatrixXd centroids_from_labels(const Eigen::MatrixXd& train,
                             ...`
- Defined: `core/cpp-annote/src/clustering_vbx.cpp:114`

### hungarian_maximize `void hungarian_maximize(const Eigen::MatrixXd& score,
                        std::vector<int>& a...`
- Defined: `core/cpp-annote/src/clustering_vbx.cpp:132`

### vbx_clustering_hard `void vbx_clustering_hard(const plda_vbx::PldaModel& plda,
                         const VbxClust...`
- Defined: `core/cpp-annote/src/clustering_vbx.cpp:165`

## core/cpp-annote/src/compute_fbank.cpp

### wespeaker_like_fbank `void wespeaker_like_fbank(float sample_hz, int num_mel_bins,
                          float fram...`
- Defined: `core/cpp-annote/src/compute_fbank.cpp:12`

## core/cpp-annote/src/cpp-annote-engine.h

### print `void print(std::ostream& os, const char* prefix = "  ") const`
- Defined: `core/cpp-annote/src/cpp-annote-engine.h:32`

### accumulate `void accumulate(const DiarizationProfile& o)`
- Defined: `core/cpp-annote/src/cpp-annote-engine.h:48`

### segmentation_model_sample_rate `int segmentation_model_sample_rate() const`
- Defined: `core/cpp-annote/src/cpp-annote-engine.h:88`

### segmentation_num_channels `int segmentation_num_channels() const`
- Defined: `core/cpp-annote/src/cpp-annote-engine.h:90`

### segmentation_chunk_num_samples `int segmentation_chunk_num_samples() const`
- Defined: `core/cpp-annote/src/cpp-annote-engine.h:91`

### segmentation_chunk_step_sec `double segmentation_chunk_step_sec() const`
- Defined: `core/cpp-annote/src/cpp-annote-engine.h:92`

### segmentation_chunk_duration_sec `double segmentation_chunk_duration_sec() const`
- Defined: `core/cpp-annote/src/cpp-annote-engine.h:93`

### seg_frames_per_chunk `int seg_frames_per_chunk() const`
- Defined: `core/cpp-annote/src/cpp-annote-engine.h:94`

### seg_classes `int seg_classes() const`
- Defined: `core/cpp-annote/src/cpp-annote-engine.h:95`

### embedding_dimension `int embedding_dimension() const`
- Defined: `core/cpp-annote/src/cpp-annote-engine.h:96`

## core/cpp-annote/src/cpp-annote-streaming.cpp

### segment_iou `double segment_iou(double a0, double a1, double b0, double b1)`
- Defined: `core/cpp-annote/src/cpp-annote-streaming.cpp:21`

### turns_match `bool turns_match(const StreamingDiarizationTurn& a,
                 const StreamingDiarizationTu...`
- Defined: `core/cpp-annote/src/cpp-annote-streaming.cpp:30`

### StreamingDiarizationSession `StreamingDiarizationSession::StreamingDiarizationSession(
    CppAnnoteEngine& engine, StreamingD...`
- Defined: `core/cpp-annote/src/cpp-annote-streaming.cpp:39`

### start_session `void StreamingDiarizationSession::start_session()`
- Defined: `core/cpp-annote/src/cpp-annote-streaming.cpp:62`

### cluster_overlap_margin_sec `double StreamingDiarizationSession::cluster_overlap_margin_sec() const`
- Defined: `core/cpp-annote/src/cpp-annote-streaming.cpp:78`

### cluster_decode_margin_sec `double StreamingDiarizationSession::cluster_decode_margin_sec() const`
- Defined: `core/cpp-annote/src/cpp-annote-streaming.cpp:82`

### active_cluster_window_start_sec `double StreamingDiarizationSession::active_cluster_window_start_sec() const`
- Defined: `core/cpp-annote/src/cpp-annote-streaming.cpp:92`

### cluster_decode_window_start_sec `double StreamingDiarizationSession::cluster_decode_window_start_sec() const`
- Defined: `core/cpp-annote/src/cpp-annote-streaming.cpp:99`

### abs_sample_offset_for_sec `int64_t StreamingDiarizationSession::abs_sample_offset_for_sec(double sec) const`
- Defined: `core/cpp-annote/src/cpp-annote-streaming.cpp:112`

### evict_chunk_cache_if_needed `void StreamingDiarizationSession::evict_chunk_cache_if_needed()`
- Defined: `core/cpp-annote/src/cpp-annote-streaming.cpp:120`

### trim_buffer_if_needed `void StreamingDiarizationSession::trim_buffer_if_needed()`
- Defined: `core/cpp-annote/src/cpp-annote-streaming.cpp:136`

### cache_new_chunks `void StreamingDiarizationSession::cache_new_chunks()`
- Defined: `core/cpp-annote/src/cpp-annote-streaming.cpp:167`

### add_audio_chunk `void StreamingDiarizationSession::add_audio_chunk(const float* pcm,
                             ...`
- Defined: `core/cpp-annote/src/cpp-annote-streaming.cpp:199`

### carry_last_updated_times `void StreamingDiarizationSession::carry_last_updated_times(
    std::vector<StreamingDiarizationT...`
- Defined: `core/cpp-annote/src/cpp-annote-streaming.cpp:225`

### append_frozen_turn_if_new `void StreamingDiarizationSession::append_frozen_turn_if_new(
    std::vector<StreamingDiarization...`
- Defined: `core/cpp-annote/src/cpp-annote-streaming.cpp:249`

### relabel_active_turns `void StreamingDiarizationSession::relabel_active_turns(
    std::vector<StreamingDiarizationTurn>...`
- Defined: `core/cpp-annote/src/cpp-annote-streaming.cpp:260`

### sort `std::sort(candidates.begin(), candidates.end(),
              [](const auto& a, const auto& b)`
- Defined: `core/cpp-annote/src/cpp-annote-streaming.cpp:314`

### merge_frozen_and_active_turns `void StreamingDiarizationSession::merge_frozen_and_active_turns(
    std::vector<StreamingDiariza...`
- Defined: `core/cpp-annote/src/cpp-annote-streaming.cpp:342`

### sort `std::sort(merged.begin(), merged.end(),
            [](const StreamingDiarizationTurn& a,
       ...`
- Defined: `core/cpp-annote/src/cpp-annote-streaming.cpp:381`

### maybe_refresh `void StreamingDiarizationSession::maybe_refresh(bool force)`
- Defined: `core/cpp-annote/src/cpp-annote-streaming.cpp:394`

### snapshot `StreamingDiarizationSnapshot StreamingDiarizationSession::snapshot() const`
- Defined: `core/cpp-annote/src/cpp-annote-streaming.cpp:548`

### refresh_and_snapshot `StreamingDiarizationSnapshot
StreamingDiarizationSession::refresh_and_snapshot()`
- Defined: `core/cpp-annote/src/cpp-annote-streaming.cpp:552`

### end_session `StreamingDiarizationSnapshot StreamingDiarizationSession::end_session()`
- Defined: `core/cpp-annote/src/cpp-annote-streaming.cpp:560`

## core/cpp-annote/src/cpp-annote.cpp

### json_double `double json_double(const std::string &json, const char *key)`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:39`

### json_bool `bool json_bool(const std::string &json, const char *key)`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:49`

### closest_frame `int closest_frame(double t, double sw_start, double sw_duration,
                  double sw_step)`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:59`

### trim_warmup_inplace `void trim_warmup_inplace(std::vector<float> &data, size_t num_chunks,
                         si...`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:65`

### inference_aggregate `void inference_aggregate(const std::vector<float> &scores, size_t num_chunks,
                   ...`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:92`

### speaker_count_initial_uint8 `std::vector<std::uint8_t> speaker_count_initial_uint8(
    std::vector<float> binarized, size_t n...`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:165`

### cap_count `std::vector<std::int8_t> cap_count(const std::vector<std::uint8_t> &u8,
                         ...`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:197`

### crop_loose_frame_range `void crop_loose_frame_range(double focus_start, double focus_end,
                            dou...`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:207`

### extent_of_frames `void extent_of_frames(double sw_start, double sw_step, size_t n_rows,
                      doubl...`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:218`

### crop_feature_loose `void crop_feature_loose(const std::vector<float> &data, int n_samples,
                        in...`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:224`

### argsort_desc_stable `std::vector<int> argsort_desc_stable(const float *row, int k)`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:255`

### stable_sort `std::stable_sort(idx.begin(), idx.end(), [row](int a, int b)`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:259`

### reconstruct_to_diarization `std::vector<float> reconstruct_to_diarization(
    const std::vector<float> &segmentations, int C...`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:267`

### binarize_column `void binarize_column(const float *k_scores, int num_frames, double sw_start,
                    ...`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:400`

### try_regex_double `bool try_regex_double(const std::string &json, const std::string &key_esc,
                      ...`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:436`

### filter_min_duration_on `void filter_min_duration_on(std::vector<std::pair<double, double>> &regs,
                       ...`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:448`

### try_json_bool_field `bool try_json_bool_field(const std::string &json, const char *key_esc,
                         b...`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:462`

### try_regex_int `bool try_regex_int(const std::string &json, const std::string &key_esc,
                   int &out)`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:475`

### make_segmentation_session `Ort::Session make_segmentation_session(Ort::Env &env,
                                       Ort:...`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:489`

### make_embedding_session `std::unique_ptr<Ort::Session> make_embedding_session(
    Ort::Env &env, Ort::SessionOptions &opt...`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:503`

### init_config_and_models `void CppAnnoteEngine::init_config_and_models(
    const std::string &embedding_onnx_path)`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:514`

### in_name_ `in_name_(session_.GetInputNameAllocated(0, alloc_)),
      out_name_(session_.GetOutputNameAlloca...`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:611`

### in_name_ `in_name_(session_.GetInputNameAllocated(0, alloc_)),
      out_name_(session_.GetOutputNameAlloca...`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:624`

### extract_chunk_audio `std::vector<float> CppAnnoteEngine::extract_chunk_audio(const float *audio,
                     ...`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:632`
- Doc: -------------------------------------------------------------------------- Per-chunk building blocks -------------------

### run_segmentation_ort_single `std::vector<float> CppAnnoteEngine::run_segmentation_ort_single(
    const float *chunk_buf)`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:652`

### run_embedding_ort_single `std::vector<float> CppAnnoteEngine::run_embedding_ort_single(
    const float *chunk_mono, const ...`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:681`

### cluster_and_decode `std::vector<DiarizationTurn> CppAnnoteEngine::cluster_and_decode(
    const std::vector<float> &s...`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:752`

### sort `std::sort(turns.begin(), turns.end(),
            [](const DiarizationTurn &a, const DiarizationT...`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:893`

### write_json `void DiarizationResults::write_json(std::ostream &os) const`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:914`
- Doc: -------------------------------------------------------------------------- DiarizationResults::write_json --------------

### write_json `void DiarizationResults::write_json(const std::string &path) const`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:930`

### Impl `Impl() : engine()`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:949`

### Impl `Impl(const std::string& seg_path, const std::string& emb_path)
      : engine(seg_path, emb_path)`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:951`

### get_stream `StreamingDiarizationSession &get_stream(int32_t id)`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:953`

### to_results `static DiarizationResults to_results(
      const StreamingDiarizationSnapshot &snap)`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:962`

### CppAnnote `CppAnnote::CppAnnote() : impl_(std::make_unique<Impl>())`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:973`

### CppAnnote `CppAnnote::CppAnnote(const std::string& segmentation_onnx_path,
                      const std::...`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:975`

### create_stream `int32_t CppAnnote::create_stream(double cluster_cadence,
                                 double ...`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:984`

### free_stream `void CppAnnote::free_stream(int32_t stream_id)`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:996`

### start_stream `void CppAnnote::start_stream(int32_t stream_id)`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:1001`

### stop_stream `DiarizationResults CppAnnote::stop_stream(int32_t stream_id)`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:1005`

### add_audio_to_stream `void CppAnnote::add_audio_to_stream(int32_t stream_id, const float *audio_data,
                 ...`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:1010`

### diarize `DiarizationResults CppAnnote::diarize(const float *audio_data,
                                  ...`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:1018`

### diarize_stream `DiarizationResults CppAnnote::diarize_stream(int32_t stream_id)`
- Defined: `core/cpp-annote/src/cpp-annote.cpp:1032`

## core/cpp-annote/src/embedding_ort_infer.cpp

### any_non_finite_embedding `bool any_non_finite_embedding(const float* e, int dim)`
- Defined: `core/cpp-annote/src/embedding_ort_infer.cpp:15`

### embedding_json_inputs_fbank_first `bool embedding_json_inputs_fbank_first(const std::string& emb_json)`
- Defined: `core/cpp-annote/src/embedding_ort_infer.cpp:26`

### run_embedding_ort `void run_embedding_ort(Ort::Session& sess, Ort::MemoryInfo& mem,
                       Ort::Allo...`
- Defined: `core/cpp-annote/src/embedding_ort_infer.cpp:39`

### discover_min_num_samples_embedding `int discover_min_num_samples_embedding(Ort::Session& sess, Ort::MemoryInfo& mem,
                ...`
- Defined: `core/cpp-annote/src/embedding_ort_infer.cpp:77`

### fbank_num_frames_for_samples `int fbank_num_frames_for_samples(int embed_sr, int mel_bins, float fl_ms,
                       ...`
- Defined: `core/cpp-annote/src/embedding_ort_infer.cpp:114`

### seg_to_fbank_nearest_index `int seg_to_fbank_nearest_index(int tf, int num_seg_frames,
                               int num...`
- Defined: `core/cpp-annote/src/embedding_ort_infer.cpp:129`

## core/cpp-annote/src/filter_train.cpp

### filter_embeddings_train `void filter_embeddings_train(int num_chunks, int num_frames, int num_speakers,
                  ...`
- Defined: `core/cpp-annote/src/filter_train.cpp:9`

## core/cpp-annote/src/parity_log.cpp

### env_parity_level `int env_parity_level()`
- Defined: `core/cpp-annote/src/parity_log.cpp:18`

### env_parity_out_dir `const char* env_parity_out_dir()`
- Defined: `core/cpp-annote/src/parity_log.cpp:32`

### log_light `void log_light(const std::string& line)`
- Defined: `core/cpp-annote/src/parity_log.cpp:40`

### heavy_dumps_enabled `bool heavy_dumps_enabled()`
- Defined: `core/cpp-annote/src/parity_log.cpp:46`

### ensure_parity_out_dir `void ensure_parity_out_dir()`
- Defined: `core/cpp-annote/src/parity_log.cpp:50`

### parity_clustering_npz_path `std::string parity_clustering_npz_path()`
- Defined: `core/cpp-annote/src/parity_log.cpp:63`

### fingerprint_float32 `std::string fingerprint_float32(const float* data, std::size_t n,
                               ...`
- Defined: `core/cpp-annote/src/parity_log.cpp:73`

## core/cpp-annote/src/plda_vbx.cpp

### align_eigen_evecs_to_scipy_wccn_row0_for_community1_plda `void align_eigen_evecs_to_scipy_wccn_row0_for_community1_plda(
    const RowMatrixXd& tr_file, Ei...`
- Defined: `core/cpp-annote/src/plda_vbx.cpp:66`

### row_l2_normalize `void row_l2_normalize(Eigen::MatrixXd& M)`
- Defined: `core/cpp-annote/src/plda_vbx.cpp:87`

### logsumexp_rowwise `void logsumexp_rowwise(const Eigen::MatrixXd& M, Eigen::VectorXd& lse,
                       Eig...`
- Defined: `core/cpp-annote/src/plda_vbx.cpp:96`

### load_from_arrays `void PldaModel::load_from_arrays(const double* mean1_p, int n_mean1,
                            ...`
- Defined: `core/cpp-annote/src/plda_vbx.cpp:117`

### load `void PldaModel::load(const std::string& xvec_transform_npz,
                     const std::strin...`
- Defined: `core/cpp-annote/src/plda_vbx.cpp:161`
- Doc: The upstream file-based PldaModel::load() (cnpy NPZ loading) is removed in this vendored copy; see plda_vbx.h. if 0

### xvec_tf `Eigen::MatrixXd PldaModel::xvec_tf(const Eigen::MatrixXd& embeddings) const`
- Defined: `core/cpp-annote/src/plda_vbx.cpp:256`
- Doc: endif  // 0 (file-based load removed)

### plda_tf `Eigen::MatrixXd PldaModel::plda_tf(const Eigen::MatrixXd& x0,
                                   ...`
- Defined: `core/cpp-annote/src/plda_vbx.cpp:271`

### operator `Eigen::MatrixXd PldaModel::operator()(const Eigen::MatrixXd& embeddings) const`
- Defined: `core/cpp-annote/src/plda_vbx.cpp:281`

### softmax_rows `void softmax_rows(const Eigen::MatrixXd& logits, Eigen::MatrixXd& out)`
- Defined: `core/cpp-annote/src/plda_vbx.cpp:285`

### cluster_vbx `void cluster_vbx(const std::vector<int>& ahc_init, const Eigen::MatrixXd& fea,
                 c...`
- Defined: `core/cpp-annote/src/plda_vbx.cpp:298`

## core/cpp-annote/src/scipy_linkage.cpp

### centroid_update `inline double centroid_update(double d_xi, double d_yi, double d_xy, int size_x,
                ...`
- Defined: `core/cpp-annote/src/scipy_linkage.cpp:15`

### is_visited `inline bool is_visited(const std::vector<unsigned char>& bitset, int i)`
- Defined: `core/cpp-annote/src/scipy_linkage.cpp:33`
- Doc: SciPy ``fcluster(..., criterion='distance')`` uses ``get_max_dist_for_each_cluster`` then ``cluster_monocrit`` (see ``sc

### set_visited `inline void set_visited(std::vector<unsigned char>& bitset, int i)`
- Defined: `core/cpp-annote/src/scipy_linkage.cpp:38`

### visited_bytes `inline int visited_bytes(int n)`
- Defined: `core/cpp-annote/src/scipy_linkage.cpp:43`

### get_max_dist_for_each_cluster `void get_max_dist_for_each_cluster(const double* Z, int n,
                                   std...`
- Defined: `core/cpp-annote/src/scipy_linkage.cpp:45`

### cluster_monocrit `void cluster_monocrit(const double* Z, int n, const std::vector<double>& MC,
                    ...`
- Defined: `core/cpp-annote/src/scipy_linkage.cpp:92`

### pdist_euclidean `void pdist_euclidean(const std::vector<double>& X, int n, int d,
                     std::vector...`
- Defined: `core/cpp-annote/src/scipy_linkage.cpp:150`

### linkage_centroid_naive `void linkage_centroid_naive(const std::vector<double>& dist, int n,
                            s...`
- Defined: `core/cpp-annote/src/scipy_linkage.cpp:168`

### fcluster_distance `void fcluster_distance(const std::vector<double>& Z, int n, double cutoff,
                      ...`
- Defined: `core/cpp-annote/src/scipy_linkage.cpp:236`

### remap_labels_contiguous `void remap_labels_contiguous(const std::vector<int>& labels_one_based,
                          ...`
- Defined: `core/cpp-annote/src/scipy_linkage.cpp:243`

## core/cpp-annote/src/scipy_linkage.h

### condensed_index `inline std::size_t condensed_index(int n, int i, int j)`
- Defined: `core/cpp-annote/src/scipy_linkage.h:13`

## core/cpp-annote/src/wav_pcm_float32.h

### read_file_bytes `inline std::vector<std::uint8_t> read_file_bytes(const std::string& path)`
- Defined: `core/cpp-annote/src/wav_pcm_float32.h:17`

### u32 `inline std::uint32_t u32(const std::uint8_t* p)`
- Defined: `core/cpp-annote/src/wav_pcm_float32.h:36`

### u16 `inline std::uint16_t u16(const std::uint8_t* p)`
- Defined: `core/cpp-annote/src/wav_pcm_float32.h:43`

### load_wav_pcm16_mono_float32 `inline std::vector<float> load_wav_pcm16_mono_float32(const std::string& path,
                  ...`
- Defined: `core/cpp-annote/src/wav_pcm_float32.h:51`
- Doc: PCM 16 LE mono or stereo (mean to mono) → float32 mono, sample_rate_out set from header.

### linear_resample `inline std::vector<float> linear_resample(const std::vector<float>& x,
                          ...`
- Defined: `core/cpp-annote/src/wav_pcm_float32.h:119`

## core/embedding-model.h

### get_similarity `float get_similarity(const std::string &a, const std::string &b)`
- Defined: `core/embedding-model.h:29`
- Doc: Compute the similarity between two text strings. @param a The first text string. @param b The second text string. @retur

### get_similarity `float get_similarity(const std::string &text,
                       const std::vector<float> &em...`
- Defined: `core/embedding-model.h:41`
- Doc: Compute the similarity between a text string and a precomputed embedding. @param text The text string to compare. @param

### get_similarity `float get_similarity(const std::vector<float> &embedding_a,
                       const std::vec...`
- Defined: `core/embedding-model.h:53`
- Doc: Compute the similarity between two precomputed embeddings. @param embedding_a The first embedding vector. @param embeddi

### cosine_similarity `float cosine_similarity(const std::vector<float> &a,
                          const std::vector<...`
- Defined: `core/embedding-model.h:65`
- Doc: Compute the cosine similarity between two vectors. @param a The first vector. @param b The second vector. @return The co

## core/gemma-embedding-model-test.cpp

### TEST_CASE `TEST_CASE("gemma-embedding-model")`
- Defined: `core/gemma-embedding-model-test.cpp:9`
- Doc: define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN include <doctest.h>

### SUBCASE `SUBCASE("load model")`
- Defined: `core/gemma-embedding-model-test.cpp:17`

### SUBCASE `SUBCASE("get embeddings")`
- Defined: `core/gemma-embedding-model-test.cpp:25`

### SUBCASE `SUBCASE("identical strings have similarity 1.0")`
- Defined: `core/gemma-embedding-model-test.cpp:45`

### SUBCASE `SUBCASE("similar strings have high similarity")`
- Defined: `core/gemma-embedding-model-test.cpp:54`

### SUBCASE `SUBCASE("different strings have lower similarity")`
- Defined: `core/gemma-embedding-model-test.cpp:66`

### SUBCASE `SUBCASE("query and document embeddings")`
- Defined: `core/gemma-embedding-model-test.cpp:78`

### SUBCASE `SUBCASE("truncate embedding with MRL")`
- Defined: `core/gemma-embedding-model-test.cpp:98`

### SUBCASE `SUBCASE("config values")`
- Defined: `core/gemma-embedding-model-test.cpp:125`

### TEST_CASE `TEST_CASE("gemma-embedding-model error handling")`
- Defined: `core/gemma-embedding-model-test.cpp:137`

### SUBCASE `SUBCASE("load nonexistent model")`
- Defined: `core/gemma-embedding-model-test.cpp:139`

### SUBCASE `SUBCASE("get embeddings without loading")`
- Defined: `core/gemma-embedding-model-test.cpp:145`

### SUBCASE `SUBCASE("load invalid variant")`
- Defined: `core/gemma-embedding-model-test.cpp:151`

## core/gemma-embedding-model.cpp

### GemmaEmbeddingModel `GemmaEmbeddingModel::GemmaEmbeddingModel()
    : ort_api_(nullptr),
      ort_env_(nullptr),
    ...`
- Defined: `core/gemma-embedding-model.cpp:20`
- Doc: define DEBUG_ALLOC_ENABLED 1 include "debug-utils.h" include "ort-utils.h"

### load `int GemmaEmbeddingModel::load(const char *model_dir,
                              const char *mo...`
- Defined: `core/gemma-embedding-model.cpp:66`

### load_from_memory `int GemmaEmbeddingModel::load_from_memory(const uint8_t *model_data,
                            ...`
- Defined: `core/gemma-embedding-model.cpp:110`

### load_tokenizer `int GemmaEmbeddingModel::load_tokenizer(const char *tokenizer_path)`
- Defined: `core/gemma-embedding-model.cpp:130`

### load_tokenizer_from_memory `int GemmaEmbeddingModel::load_tokenizer_from_memory(const uint8_t *data,
                        ...`
- Defined: `core/gemma-embedding-model.cpp:141`

### tokenize `std::vector<int64_t> GemmaEmbeddingModel::tokenize(const std::string &text)`
- Defined: `core/gemma-embedding-model.cpp:160`

### run_inference `std::vector<float> GemmaEmbeddingModel::run_inference(
    const std::vector<int64_t> &input_ids,...`
- Defined: `core/gemma-embedding-model.cpp:185`

### get_embeddings `std::vector<float> GemmaEmbeddingModel::get_embeddings(
    const std::string &text)`
- Defined: `core/gemma-embedding-model.cpp:297`

### get_embeddings_with_prefix `std::vector<float> GemmaEmbeddingModel::get_embeddings_with_prefix(
    const std::string &text, ...`
- Defined: `core/gemma-embedding-model.cpp:314`

### get_query_embeddings `std::vector<float> GemmaEmbeddingModel::get_query_embeddings(
    const std::string &query)`
- Defined: `core/gemma-embedding-model.cpp:319`

### get_document_embeddings `std::vector<float> GemmaEmbeddingModel::get_document_embeddings(
    const std::string &document)`
- Defined: `core/gemma-embedding-model.cpp:324`

### truncate_embedding `std::vector<float> GemmaEmbeddingModel::truncate_embedding(
    const std::vector<float> &embeddi...`
- Defined: `core/gemma-embedding-model.cpp:329`

### normalize_embedding `void GemmaEmbeddingModel::normalize_embedding(std::vector<float> &embedding)`
- Defined: `core/gemma-embedding-model.cpp:345`

### is_loaded `bool GemmaEmbeddingModel::is_loaded() const`
- Defined: `core/gemma-embedding-model.cpp:361`

### get_config `const GemmaEmbeddingConfig &GemmaEmbeddingModel::get_config() const`
- Defined: `core/gemma-embedding-model.cpp:363`

## core/intent-recognizer-test.cpp

### make_options `IntentRecognizerOptions make_options()`
- Defined: `core/intent-recognizer-test.cpp:18`

### embedding_model_available `bool embedding_model_available()`
- Defined: `core/intent-recognizer-test.cpp:26`

### TEST_CASE `TEST_CASE("intent-recognizer unit tests")`
- Defined: `core/intent-recognizer-test.cpp:30`

### SUBCASE `SUBCASE("register and count intents")`
- Defined: `core/intent-recognizer-test.cpp:39`

### SUBCASE `SUBCASE("unregister intent")`
- Defined: `core/intent-recognizer-test.cpp:49`

### SUBCASE `SUBCASE("unregister nonexistent intent")`
- Defined: `core/intent-recognizer-test.cpp:58`

### SUBCASE `SUBCASE("clear intents")`
- Defined: `core/intent-recognizer-test.cpp:63`

### SUBCASE `SUBCASE("rank_intents returns empty for empty utterance")`
- Defined: `core/intent-recognizer-test.cpp:72`

### SUBCASE `SUBCASE("rank_intents sorts by similarity descending and respects max")`
- Defined: `core/intent-recognizer-test.cpp:77`

### SUBCASE `SUBCASE("rank_intents with max_results limit")`
- Defined: `core/intent-recognizer-test.cpp:95`

### precision `float precision() const`
- Defined: `core/intent-recognizer-test.cpp:121`

### recall `float recall() const`
- Defined: `core/intent-recognizer-test.cpp:126`

### f1_score `float f1_score() const`
- Defined: `core/intent-recognizer-test.cpp:131`

### accuracy `float accuracy() const`
- Defined: `core/intent-recognizer-test.cpp:137`

### TEST_CASE `TEST_CASE("intent-recognizer precision/recall with GemmaEmbeddingModel")`
- Defined: `core/intent-recognizer-test.cpp:146`

### SUBCASE `SUBCASE("basic intent matching")`
- Defined: `core/intent-recognizer-test.cpp:173`

### SUBCASE `SUBCASE("precision/recall evaluation")`
- Defined: `core/intent-recognizer-test.cpp:187`

### SUBCASE `SUBCASE("intent discrimination")`
- Defined: `core/intent-recognizer-test.cpp:282`

### SUBCASE `SUBCASE("similarity scores for exact matches")`
- Defined: `core/intent-recognizer-test.cpp:325`

### TEST_CASE `TEST_CASE("intent-recognizer register with pre-computed embedding")`
- Defined: `core/intent-recognizer-test.cpp:346`

### SUBCASE `SUBCASE("register with NULL embedding auto-computes")`
- Defined: `core/intent-recognizer-test.cpp:355`

### SUBCASE `SUBCASE("register with pre-computed embedding")`
- Defined: `core/intent-recognizer-test.cpp:365`

### SUBCASE `SUBCASE("update existing intent preserves count")`
- Defined: `core/intent-recognizer-test.cpp:379`

### TEST_CASE `TEST_CASE("intent-recognizer priority ranking")`
- Defined: `core/intent-recognizer-test.cpp:388`

### SUBCASE `SUBCASE("higher priority intent ranks first regardless of similarity")`
- Defined: `core/intent-recognizer-test.cpp:397`

### SUBCASE `SUBCASE("equal priority falls back to similarity ordering")`
- Defined: `core/intent-recognizer-test.cpp:407`

### TEST_CASE `TEST_CASE("intent-recognizer calculate_embedding")`
- Defined: `core/intent-recognizer-test.cpp:418`

### SUBCASE `SUBCASE("returns non-empty embedding")`
- Defined: `core/intent-recognizer-test.cpp:427`

### SUBCASE `SUBCASE("get_embedding_size returns correct dimension")`
- Defined: `core/intent-recognizer-test.cpp:433`

### SUBCASE `SUBCASE("same text produces same embedding")`
- Defined: `core/intent-recognizer-test.cpp:440`

### TEST_CASE `TEST_CASE("C API intent registration with embedding and priority")`
- Defined: `core/intent-recognizer-test.cpp:450`

### SUBCASE `SUBCASE("register with NULL embedding succeeds")`
- Defined: `core/intent-recognizer-test.cpp:462`

### SUBCASE `SUBCASE("register with nullptr canonical_phrase fails")`
- Defined: `core/intent-recognizer-test.cpp:468`

### SUBCASE `SUBCASE("register multiple intents with different priorities")`
- Defined: `core/intent-recognizer-test.cpp:473`

### SUBCASE `SUBCASE("unregister and clear work")`
- Defined: `core/intent-recognizer-test.cpp:481`

### TEST_CASE `TEST_CASE("C API moonshine_calculate_intent_embedding")`
- Defined: `core/intent-recognizer-test.cpp:496`

### SUBCASE `SUBCASE("basic embedding calculation")`
- Defined: `core/intent-recognizer-test.cpp:508`

### SUBCASE `SUBCASE("null sentence returns error")`
- Defined: `core/intent-recognizer-test.cpp:528`

### SUBCASE `SUBCASE("null out_embedding returns error")`
- Defined: `core/intent-recognizer-test.cpp:536`

### SUBCASE `SUBCASE("null out_embedding_size returns error")`
- Defined: `core/intent-recognizer-test.cpp:543`

### SUBCASE `SUBCASE("invalid handle returns error")`
- Defined: `core/intent-recognizer-test.cpp:550`

### SUBCASE `SUBCASE("round-trip: compute embedding then register with it")`
- Defined: `core/intent-recognizer-test.cpp:558`

### TEST_CASE `TEST_CASE("C API moonshine_free_intent_embedding")`
- Defined: `core/intent-recognizer-test.cpp:588`

### SUBCASE `SUBCASE("safe on nullptr")`
- Defined: `core/intent-recognizer-test.cpp:590`

### SUBCASE `SUBCASE("frees malloc-allocated buffer")`
- Defined: `core/intent-recognizer-test.cpp:591`

### TEST_CASE `TEST_CASE("C API moonshine_calculate_embedding_distance")`
- Defined: `core/intent-recognizer-test.cpp:598`

### SUBCASE `SUBCASE("identical embeddings have similarity ~1.0")`
- Defined: `core/intent-recognizer-test.cpp:610`

### SUBCASE `SUBCASE("similar sentences have high similarity")`
- Defined: `core/intent-recognizer-test.cpp:626`

### SUBCASE `SUBCASE("dissimilar sentences have low similarity")`
- Defined: `core/intent-recognizer-test.cpp:647`

### SUBCASE `SUBCASE("null embedding_a returns error")`
- Defined: `core/intent-recognizer-test.cpp:668`

### SUBCASE `SUBCASE("null embedding_b returns error")`
- Defined: `core/intent-recognizer-test.cpp:676`

### SUBCASE `SUBCASE("null out_similarity returns error")`
- Defined: `core/intent-recognizer-test.cpp:684`

### SUBCASE `SUBCASE("zero embedding_size returns error")`
- Defined: `core/intent-recognizer-test.cpp:691`

### SUBCASE `SUBCASE("invalid handle returns error")`
- Defined: `core/intent-recognizer-test.cpp:699`

### TEST_CASE `TEST_CASE("C API moonshine_get_closest_intents with priority")`
- Defined: `core/intent-recognizer-test.cpp:710`

## core/intent-recognizer.cpp

### create_embedding_model `std::unique_ptr<EmbeddingModel> create_embedding_model(
    const IntentRecognizerOptions &options)`
- Defined: `core/intent-recognizer.cpp:10`

### IntentRecognizer `IntentRecognizer::IntentRecognizer(const IntentRecognizerOptions &options)
    : embedding_model_...`
- Defined: `core/intent-recognizer.cpp:30`

### register_intent `void IntentRecognizer::register_intent(const std::string &trigger_phrase)`
- Defined: `core/intent-recognizer.cpp:35`

### register_intent `void IntentRecognizer::register_intent(const std::string &trigger_phrase,
                       ...`
- Defined: `core/intent-recognizer.cpp:39`

### unregister_intent `bool IntentRecognizer::unregister_intent(const std::string &trigger_phrase)`
- Defined: `core/intent-recognizer.cpp:67`

### sort `std::sort(entries.begin(), entries.end(), [](const auto &a, const auto &b)`
- Defined: `core/intent-recognizer.cpp:114`

### get_intent_count `size_t IntentRecognizer::get_intent_count() const`
- Defined: `core/intent-recognizer.cpp:129`

### clear_intents `void IntentRecognizer::clear_intents()`
- Defined: `core/intent-recognizer.cpp:134`

### calculate_embedding `std::vector<float> IntentRecognizer::calculate_embedding(
    const std::string &sentence) const`
- Defined: `core/intent-recognizer.cpp:139`

### calculate_similarity `float IntentRecognizer::calculate_similarity(
    const std::vector<float> &a, const std::vector<...`
- Defined: `core/intent-recognizer.cpp:145`

### get_embedding_size `size_t IntentRecognizer::get_embedding_size() const`
- Defined: `core/intent-recognizer.cpp:151`

## core/moonshine-c-api-memory-test.cpp

### read_binary_file `std::vector<uint8_t> read_binary_file(const std::filesystem::path& p)`
- Defined: `core/moonshine-c-api-memory-test.cpp:33`

### kokoro_lang_for_voice_stem `const char* kokoro_lang_for_voice_stem(std::string_view stem)`
- Defined: `core/moonshine-c-api-memory-test.cpp:44`
- Doc: Kokoro voice ids use a two-letter family prefix (e.g. af_alloy -> en_us).

### sample_text_for_kokoro_lang `const char* sample_text_for_kokoro_lang(const char* lang)`
- Defined: `core/moonshine-c-api-memory-test.cpp:78`

### append_files_under `void append_files_under(
    const std::filesystem::path& root, const std::filesystem::path& sub,...`
- Defined: `core/moonshine-c-api-memory-test.cpp:110`
- Doc: Subtrees needed for Kokoro + rule G2P (Spanish is rule-only; no lexicon files).

### build_kokoro_g2p_memory_bundle `void build_kokoro_g2p_memory_bundle(
    const std::filesystem::path& data_root,
    std::vector<...`
- Defined: `core/moonshine-c-api-memory-test.cpp:139`

### main `int main(int argc, char** argv)`
- Defined: `core/moonshine-c-api-memory-test.cpp:265`

## core/moonshine-c-api-test.cpp

### find_de_piper_voices_dir `std::filesystem::path find_de_piper_voices_dir()`
- Defined: `core/moonshine-c-api-test.cpp:21`

### read_binary_file `std::vector<uint8_t> read_binary_file(const std::filesystem::path& p)`
- Defined: `core/moonshine-c-api-test.cpp:36`

### find_moonshine_tts_data_dir `std::optional<std::filesystem::path> find_moonshine_tts_data_dir()`
- Defined: `core/moonshine-c-api-test.cpp:48`
- Doc: Resolve ``moonshine-tts/data`` for tests run from ``test-assets/``, repo root, or ``core/build``.

### free_phonemes_output `void free_phonemes_output(const char* ipa)`
- Defined: `core/moonshine-c-api-test.cpp:71`

### grapheme_phonemizer_smoke `void grapheme_phonemizer_smoke(const std::filesystem::path& data_root,
                          ...`
- Defined: `core/moonshine-c-api-test.cpp:78`
- Doc: Creates a phonemizer with ``g2p_root`` = *data_root*, runs ``text`` → IPA, frees output.

### TEST_CASE `TEST_CASE("moonshine-test-v2")`
- Defined: `core/moonshine-c-api-test.cpp:109`

### SUBCASE `SUBCASE("transcribe-complete")`
- Defined: `core/moonshine-c-api-test.cpp:111`

### SUBCASE `SUBCASE("transcribe-stream")`
- Defined: `core/moonshine-c-api-test.cpp:154`

### SUBCASE `SUBCASE("transcribe-complete-from-memory")`
- Defined: `core/moonshine-c-api-test.cpp:247`

### SUBCASE `SUBCASE("transcribe-without-streaming-skip-transcription")`
- Defined: `core/moonshine-c-api-test.cpp:313`

### SUBCASE `SUBCASE("transcribe-without-streaming-vad-threshold-0")`
- Defined: `core/moonshine-c-api-test.cpp:357`

### SUBCASE `SUBCASE("transcribe-valid-options")`
- Defined: `core/moonshine-c-api-test.cpp:407`

### SUBCASE `SUBCASE("transcribe-invalid-option")`
- Defined: `core/moonshine-c-api-test.cpp:438`

### SUBCASE `SUBCASE("spelling-mode-flag-noop-without-model")`
- Defined: `core/moonshine-c-api-test.cpp:451`

### SUBCASE `SUBCASE("spelling-mode-replaces-line-text")`
- Defined: `core/moonshine-c-api-test.cpp:478`

### SUBCASE `SUBCASE("tts-synthesizer-valid-options")`
- Defined: `core/moonshine-c-api-test.cpp:524`

### SUBCASE `SUBCASE("tts-synthesizer-per-call-speed-kokoro")`
- Defined: `core/moonshine-c-api-test.cpp:548`

### SUBCASE `SUBCASE("tts-piper-german-from-memory")`
- Defined: `core/moonshine-c-api-test.cpp:597`

### TEST_CASE `TEST_CASE("moonshine-phonemes-to-speech-c-api")`
- Defined: `core/moonshine-c-api-test.cpp:656`

### SUBCASE `SUBCASE("invalid-handle")`
- Defined: `core/moonshine-c-api-test.cpp:658`

### SUBCASE `SUBCASE("invalid-arguments")`
- Defined: `core/moonshine-c-api-test.cpp:666`

### SUBCASE `SUBCASE("kokoro-matches-text-to-speech")`
- Defined: `core/moonshine-c-api-test.cpp:695`

### TEST_CASE `TEST_CASE("grapheme-to-phonemizer-c-api")`
- Defined: `core/moonshine-c-api-test.cpp:783`

### SUBCASE `SUBCASE("create-invalid-filenames-pointer")`
- Defined: `core/moonshine-c-api-test.cpp:785`

### SUBCASE `SUBCASE("text-to-phonemes-invalid-handle")`
- Defined: `core/moonshine-c-api-test.cpp:794`

### SUBCASE `SUBCASE("text-to-phonemes-invalid-arguments")`
- Defined: `core/moonshine-c-api-test.cpp:801`

### SUBCASE `SUBCASE("rule-based-languages-smoke")`
- Defined: `core/moonshine-c-api-test.cpp:828`

### SUBCASE `SUBCASE("chinese-when-onnx-bundle-present")`
- Defined: `core/moonshine-c-api-test.cpp:867`

### SUBCASE `SUBCASE("japanese-when-onnx-bundle-present")`
- Defined: `core/moonshine-c-api-test.cpp:884`

### SUBCASE `SUBCASE("arabic-when-onnx-bundle-present")`
- Defined: `core/moonshine-c-api-test.cpp:903`

### TEST_CASE `TEST_CASE("moonshine-tts-g2p-dependency-api")`
- Defined: `core/moonshine-c-api-test.cpp:922`

### SUBCASE `SUBCASE("null-output-pointer")`
- Defined: `core/moonshine-c-api-test.cpp:924`

### SUBCASE `SUBCASE("options-count-without-options-pointer")`
- Defined: `core/moonshine-c-api-test.cpp:932`

### SUBCASE `SUBCASE("g2p-empty-means-all-languages")`
- Defined: `core/moonshine-c-api-test.cpp:942`

### SUBCASE `SUBCASE("g2p-arabic-onnx-model-key-matches-meta-onnx-filename")`
- Defined: `core/moonshine-c-api-test.cpp:960`

### SUBCASE `SUBCASE("g2p-french-lists-pos-csv-files-not-directory-prefix")`
- Defined: `core/moonshine-c-api-test.cpp:973`

### SUBCASE `SUBCASE("g2p-single-language")`
- Defined: `core/moonshine-c-api-test.cpp:987`

### SUBCASE `SUBCASE("g2p-unsupported-language")`
- Defined: `core/moonshine-c-api-test.cpp:996`

### SUBCASE `SUBCASE("g2p-multiple-languages")`
- Defined: `core/moonshine-c-api-test.cpp:1004`

### SUBCASE `SUBCASE("g2p-appends-override-key-when-option-set")`
- Defined: `core/moonshine-c-api-test.cpp:1016`

### SUBCASE `SUBCASE("tts-json-single-language")`
- Defined: `core/moonshine-c-api-test.cpp:1028`

### SUBCASE `SUBCASE("tts-empty-all-languages-json")`
- Defined: `core/moonshine-c-api-test.cpp:1043`

### SUBCASE `SUBCASE("tts-unsupported-language")`
- Defined: `core/moonshine-c-api-test.cpp:1054`

### SUBCASE `SUBCASE("tts-multiple-languages")`
- Defined: `core/moonshine-c-api-test.cpp:1062`

### SUBCASE `SUBCASE("tts-piper-engine-on-en_us")`
- Defined: `core/moonshine-c-api-test.cpp:1075`

### SUBCASE `SUBCASE("tts-kokoro-engine-on-fr")`
- Defined: `core/moonshine-c-api-test.cpp:1089`

### SUBCASE `SUBCASE("tts-explicit-piper-onnx-map-keys")`
- Defined: `core/moonshine-c-api-test.cpp:1103`

### SUBCASE `SUBCASE("tts-piper-voice-selects-onnx-basename")`
- Defined: `core/moonshine-c-api-test.cpp:1118`

### SUBCASE `SUBCASE("tts-voices-json-object-en_us")`
- Defined: `core/moonshine-c-api-test.cpp:1131`

### SUBCASE `SUBCASE("tts-voices-kokoro-reports-missing-without-assets")`
- Defined: `core/moonshine-c-api-test.cpp:1154`

### SUBCASE `SUBCASE("tts-voices-unsupported-language")`
- Defined: `core/moonshine-c-api-test.cpp:1168`

### SUBCASE `SUBCASE("tts-voices-piper-de-includes-thorsten-stem")`
- Defined: `core/moonshine-c-api-test.cpp:1175`

### SUBCASE `SUBCASE("tts-voices-piper-en_us-includes-saikat-stem")`
- Defined: `core/moonshine-c-api-test.cpp:1195`

### SUBCASE `SUBCASE("tts-zipvoice-dependencies")`
- Defined: `core/moonshine-c-api-test.cpp:1215`

### SUBCASE `SUBCASE("tts-zipvoice-voices-listing")`
- Defined: `core/moonshine-c-api-test.cpp:1233`

### TEST_CASE `TEST_CASE("moonshine-stt-intent-dependency-api")`
- Defined: `core/moonshine-c-api-test.cpp:1252`

### SUBCASE `SUBCASE("null-output-pointer")`
- Defined: `core/moonshine-c-api-test.cpp:1254`

### SUBCASE `SUBCASE("options-count-without-options-pointer")`
- Defined: `core/moonshine-c-api-test.cpp:1261`

### SUBCASE `SUBCASE("stt-empty-language-is-invalid")`
- Defined: `core/moonshine-c-api-test.cpp:1270`

### SUBCASE `SUBCASE("stt-english-default-is-medium-streaming")`
- Defined: `core/moonshine-c-api-test.cpp:1277`

### SUBCASE `SUBCASE("stt-english-tiny-non-streaming")`
- Defined: `core/moonshine-c-api-test.cpp:1295`

### SUBCASE `SUBCASE("stt-non-english-omits-attention-extra")`
- Defined: `core/moonshine-c-api-test.cpp:1316`

### SUBCASE `SUBCASE("stt-english-name-lookup")`
- Defined: `core/moonshine-c-api-test.cpp:1333`

### SUBCASE `SUBCASE("stt-include-spelling-adds-group-for-english")`
- Defined: `core/moonshine-c-api-test.cpp:1341`

### SUBCASE `SUBCASE("stt-include-spelling-noop-for-non-english")`
- Defined: `core/moonshine-c-api-test.cpp:1358`

### SUBCASE `SUBCASE("stt-unknown-language")`
- Defined: `core/moonshine-c-api-test.cpp:1372`

### SUBCASE `SUBCASE("stt-unknown-arch-for-language")`
- Defined: `core/moonshine-c-api-test.cpp:1380`

### SUBCASE `SUBCASE("stt-invalid-arch-value")`
- Defined: `core/moonshine-c-api-test.cpp:1390`

### SUBCASE `SUBCASE("intent-default-variant-is-q4")`
- Defined: `core/moonshine-c-api-test.cpp:1400`

### SUBCASE `SUBCASE("intent-null-model-name-uses-default")`
- Defined: `core/moonshine-c-api-test.cpp:1414`

### SUBCASE `SUBCASE("intent-q8-maps-to-model-quantized")`
- Defined: `core/moonshine-c-api-test.cpp:1423`

### SUBCASE `SUBCASE("intent-fp32-uses-bare-model-onnx")`
- Defined: `core/moonshine-c-api-test.cpp:1440`

### SUBCASE `SUBCASE("intent-unknown-model")`
- Defined: `core/moonshine-c-api-test.cpp:1454`

### SUBCASE `SUBCASE("intent-unknown-variant")`
- Defined: `core/moonshine-c-api-test.cpp:1461`

### SUBCASE `SUBCASE("builtin-voice-synthesizes-audio")`
- Defined: `core/moonshine-c-api-test.cpp:1497`

### SUBCASE `SUBCASE("user-pcm-with-explicit-transcript")`
- Defined: `core/moonshine-c-api-test.cpp:1521`

## core/moonshine-c-api.cpp

### parse_option_vector `OptionVector parse_option_vector(const moonshine_option_t *options,
                             ...`
- Defined: `core/moonshine-c-api.cpp:82`

### parse_common_options `OptionVector parse_common_options(const OptionVector &options)`
- Defined: `core/moonshine-c-api.cpp:98`
- Doc: Handles common options that are not specific to any particular API.

### parse_transcriber_options `void parse_transcriber_options(const OptionVector &options,
                               Transc...`
- Defined: `core/moonshine-c-api.cpp:109`

### allocate_transcriber_handle `int32_t allocate_transcriber_handle(Transcriber *transcriber)`
- Defined: `core/moonshine-c-api.cpp:170`

### free_transcriber_handle `void free_transcriber_handle(int32_t handle)`
- Defined: `core/moonshine-c-api.cpp:177`

### moonshine_load_transcriber_from_memory `int32_t moonshine_load_transcriber_from_memory(
    const uint8_t *encoder_model_data, size_t enc...`
- Defined: `core/moonshine-c-api.cpp:239`

### moonshine_free_transcriber `void moonshine_free_transcriber(int32_t transcriber_handle)`
- Defined: `core/moonshine-c-api.cpp:290`

### moonshine_transcribe_without_streaming `int32_t moonshine_transcribe_without_streaming(
    int32_t transcriber_handle, float *audio_data...`
- Defined: `core/moonshine-c-api.cpp:298`

### moonshine_create_stream `int32_t moonshine_create_stream(int32_t transcriber_handle, uint32_t flags)`
- Defined: `core/moonshine-c-api.cpp:321`

### moonshine_free_stream `int32_t moonshine_free_stream(int32_t transcriber_handle,
                              int32_t s...`
- Defined: `core/moonshine-c-api.cpp:335`

### moonshine_start_stream `int32_t moonshine_start_stream(int32_t transcriber_handle,
                               int32_t...`
- Defined: `core/moonshine-c-api.cpp:351`

### moonshine_stop_stream `int32_t moonshine_stop_stream(int32_t transcriber_handle,
                              int32_t s...`
- Defined: `core/moonshine-c-api.cpp:367`

### moonshine_transcript_to_string `const char *moonshine_transcript_to_string(
    const struct transcript_t *transcript)`
- Defined: `core/moonshine-c-api.cpp:383`

### moonshine_transcribe_add_audio_to_stream `int32_t moonshine_transcribe_add_audio_to_stream(int32_t transcriber_handle,
                    ...`
- Defined: `core/moonshine-c-api.cpp:393`

### moonshine_transcribe_stream `int32_t moonshine_transcribe_stream(int32_t transcriber_handle,
                                 ...`
- Defined: `core/moonshine-c-api.cpp:419`

### allocate_intent_recognizer_handle `int32_t allocate_intent_recognizer_handle(IntentRecognizer *recognizer)`
- Defined: `core/moonshine-c-api.cpp:447`

### free_intent_recognizer_handle `void free_intent_recognizer_handle(int32_t handle)`
- Defined: `core/moonshine-c-api.cpp:454`

### duplicate_c_string `char *duplicate_c_string(const char *s)`
- Defined: `core/moonshine-c-api.cpp:470`

### moonshine_create_intent_recognizer `int32_t moonshine_create_intent_recognizer(const char *model_path,
                              ...`
- Defined: `core/moonshine-c-api.cpp:484`

### moonshine_free_intent_recognizer `void moonshine_free_intent_recognizer(int32_t intent_recognizer_handle)`
- Defined: `core/moonshine-c-api.cpp:515`

### moonshine_register_intent `int32_t moonshine_register_intent(int32_t intent_recognizer_handle,
                             ...`
- Defined: `core/moonshine-c-api.cpp:526`

### moonshine_unregister_intent `int32_t moonshine_unregister_intent(int32_t intent_recognizer_handle,
                           ...`
- Defined: `core/moonshine-c-api.cpp:552`

### moonshine_get_closest_intents `int32_t moonshine_get_closest_intents(int32_t intent_recognizer_handle,
                         ...`
- Defined: `core/moonshine-c-api.cpp:577`

### moonshine_free_intent_matches `void moonshine_free_intent_matches(moonshine_intent_match_t *matches,
                           ...`
- Defined: `core/moonshine-c-api.cpp:635`

### moonshine_get_intent_count `int32_t moonshine_get_intent_count(int32_t intent_recognizer_handle)`
- Defined: `core/moonshine-c-api.cpp:646`

### moonshine_clear_intents `int32_t moonshine_clear_intents(int32_t intent_recognizer_handle)`
- Defined: `core/moonshine-c-api.cpp:658`

### moonshine_calculate_intent_embedding `int32_t moonshine_calculate_intent_embedding(int32_t intent_recognizer_handle,
                  ...`
- Defined: `core/moonshine-c-api.cpp:672`

### moonshine_free_intent_embedding `void moonshine_free_intent_embedding(float *embedding)`
- Defined: `core/moonshine-c-api.cpp:713`

### moonshine_calculate_embedding_distance `int32_t moonshine_calculate_embedding_distance(int32_t intent_recognizer_handle,
                ...`
- Defined: `core/moonshine-c-api.cpp:715`

### allocate_text_to_speech_synthesizer_handle `int32_t allocate_text_to_speech_synthesizer_handle(
    moonshine_tts::MoonshineTTS *synthesizer)`
- Defined: `core/moonshine-c-api.cpp:754`

### parse_tts_options `void parse_tts_options(const OptionVector &options,
                       moonshine_tts::Moonshi...`
- Defined: `core/moonshine-c-api.cpp:762`

### maybe_autotranscribe_zipvoice_clone `void maybe_autotranscribe_zipvoice_clone(
    const OptionVector &options,
    moonshine_tts::Moo...`
- Defined: `core/moonshine-c-api.cpp:778`
- Doc: When the ZipVoice engine is selected with a caller-supplied clone reference clip (memory key ``zipvoice/clone_audio``) b

### moonshine_create_tts_synthesizer_from_files `int32_t moonshine_create_tts_synthesizer_from_files(
    const char *language, const char **filen...`
- Defined: `core/moonshine-c-api.cpp:869`

### moonshine_create_tts_synthesizer_from_memory `int32_t moonshine_create_tts_synthesizer_from_memory(
    const char *language, const char **file...`
- Defined: `core/moonshine-c-api.cpp:910`

### moonshine_free_tts_synthesizer `void moonshine_free_tts_synthesizer(int32_t tts_synthesizer_handle)`
- Defined: `core/moonshine-c-api.cpp:1000`
- Doc: Releases the resources used by a text to speech synthesizer. Returns zero on success, or a non-zero error code on failur

### moonshine_text_to_speech `int32_t moonshine_text_to_speech(int32_t tts_synthesizer_handle,
                                ...`
- Defined: `core/moonshine-c-api.cpp:1041`
- Doc: Synthesizes text to speech. Returns zero on success, or a non-zero error code on failure.

### moonshine_phonemes_to_speech `int32_t moonshine_phonemes_to_speech(int32_t tts_synthesizer_handle,
                            ...`
- Defined: `core/moonshine-c-api.cpp:1088`

### malloc_string_copy `char *malloc_string_copy(const std::string &s)`
- Defined: `core/moonshine-c-api.cpp:1143`

### split_comma_nonempty_language_tokens `std::vector<std::string> split_comma_nonempty_language_tokens(const char *s)`
- Defined: `core/moonshine-c-api.cpp:1152`

### append_unique_in_order `void append_unique_in_order(std::vector<std::string> &acc,
                            const std:...`
- Defined: `core/moonshine-c-api.cpp:1177`

### json_utf8_string_literal `std::string json_utf8_string_literal(const std::string &s)`
- Defined: `core/moonshine-c-api.cpp:1187`

### json_flat_string_array `std::string json_flat_string_array(const std::vector<std::string> &items)`
- Defined: `core/moonshine-c-api.cpp:1229`

### json_model_dependencies `std::string json_model_dependencies(const moonshine::ModelDependencies &deps)`
- Defined: `core/moonshine-c-api.cpp:1247`
- Doc: Serializes a model download manifest as a JSON object with a "groups" array. Each group is { "base_url": "...", "files":

### json_tts_voice_entry `std::string json_tts_voice_entry(
    const moonshine_tts::MoonshineTtsVoiceAvailability &v)`
- Defined: `core/moonshine-c-api.cpp:1263`

### json_tts_voices_lang_array `std::string json_tts_voices_lang_array(
    const std::vector<moonshine_tts::MoonshineTtsVoiceAva...`
- Defined: `core/moonshine-c-api.cpp:1273`

### json_tts_voices_root_object `std::string json_tts_voices_root_object(
    const std::vector<std::pair<
        std::string, st...`
- Defined: `core/moonshine-c-api.cpp:1287`

### apply_g2p_dependency_query_c_options `void apply_g2p_dependency_query_c_options(
    const moonshine_option_t *options, uint64_t option...`
- Defined: `core/moonshine-c-api.cpp:1305`

### append_g2p_explicit_override_keys_from_c_options `void append_g2p_explicit_override_keys_from_c_options(
    const moonshine_option_t *options, uin...`
- Defined: `core/moonshine-c-api.cpp:1355`

### moonshine_get_g2p_dependencies `int32_t moonshine_get_g2p_dependencies(const char *languages,
                                   ...`
- Defined: `core/moonshine-c-api.cpp:1386`

### moonshine_get_tts_dependencies `int32_t moonshine_get_tts_dependencies(const char *languages,
                                   ...`
- Defined: `core/moonshine-c-api.cpp:1450`

### moonshine_get_tts_voices `int32_t moonshine_get_tts_voices(const char *languages,
                                 const mo...`
- Defined: `core/moonshine-c-api.cpp:1547`

### normalize_option_key `std::string normalize_option_key(const char *name)`
- Defined: `core/moonshine-c-api.cpp:1653`

### parse_int_option `std::optional<int32_t> parse_int_option(const std::string &value)`
- Defined: `core/moonshine-c-api.cpp:1662`
- Doc: Parses an integer option value; returns std::nullopt on empty/invalid input.

### moonshine_get_stt_dependencies `int32_t moonshine_get_stt_dependencies(const char *language,
                                    ...`
- Defined: `core/moonshine-c-api.cpp:1680`

### moonshine_get_intent_dependencies `int32_t moonshine_get_intent_dependencies(const char *model_name,
                               ...`
- Defined: `core/moonshine-c-api.cpp:1742`

### allocate_grapheme_phonemizer_handle `int32_t allocate_grapheme_phonemizer_handle(moonshine_tts::MoonshineG2P *g2p)`
- Defined: `core/moonshine-c-api.cpp:1801`

### parse_grapheme_phonemizer_options `void parse_grapheme_phonemizer_options(
    const moonshine_option_t *in_options, uint64_t in_opt...`
- Defined: `core/moonshine-c-api.cpp:1808`

### finalize_g2p_options_for_phonemizer_create `void finalize_g2p_options_for_phonemizer_create(
    moonshine_tts::MoonshineG2POptions &g2p_opt)`
- Defined: `core/moonshine-c-api.cpp:1845`

### moonshine_create_grapheme_to_phonemizer_from_files `int32_t moonshine_create_grapheme_to_phonemizer_from_files(
    const char *language, const char ...`
- Defined: `core/moonshine-c-api.cpp:1869`
- Doc: Creates a grapheme to phonemizer from files on disk. Returns a non-negative handle on success, or a negative error code 

### moonshine_create_grapheme_to_phonemizer_from_memory `int32_t moonshine_create_grapheme_to_phonemizer_from_memory(
    const char *language, const char...`
- Defined: `core/moonshine-c-api.cpp:1928`
- Doc: Creates a grapheme to phonemizer from memory. Returns a non-negative handle on success, or a negative error code on fail

### moonshine_free_grapheme_to_phonemizer `void moonshine_free_grapheme_to_phonemizer(
    int32_t grapheme_to_phonemizer_handle)`
- Defined: `core/moonshine-c-api.cpp:1995`
- Doc: Releases the resources used by a grapheme to phonemizer. Returns zero on success, or a non-zero error code on failure.

### moonshine_text_to_phonemes `int32_t moonshine_text_to_phonemes(int32_t grapheme_to_phonemizer_handle,
                       ...`
- Defined: `core/moonshine-c-api.cpp:2012`
- Doc: Converts a text into the equivalent International Phonetic Alphabet (IPA) phonemes. Returns zero on success, or a non-ze

## core/moonshine-c-api.h

### main `int main(int argc, char *argv[])`
- Defined: `core/moonshine-c-api.h:37`
- Doc: include "moonshine-c-api.h"

## core/moonshine-cpp-test.cpp

### load_wav_data `bool load_wav_data(const char *path, float **out_float_data,
                   size_t *out_num_s...`
- Defined: `core/moonshine-cpp-test.cpp:13`
- Doc: Duplicate of load_wav_data in debug-utils.cpp to avoid depending on internal library code.

### file_exists `bool file_exists(const std::string &path)`
- Defined: `core/moonshine-cpp-test.cpp:132`
- Doc: Would use std::filesystem::exists, but it's not available in C++11.

### onLineStarted `void onLineStarted(const moonshine::LineStarted &) override`
- Defined: `core/moonshine-cpp-test.cpp:147`

### onLineUpdated `void onLineUpdated(const moonshine::LineUpdated &) override`
- Defined: `core/moonshine-cpp-test.cpp:150`

### onLineTextChanged `void onLineTextChanged(const moonshine::LineTextChanged &) override`
- Defined: `core/moonshine-cpp-test.cpp:153`

### onLineCompleted `void onLineCompleted(const moonshine::LineCompleted &) override`
- Defined: `core/moonshine-cpp-test.cpp:156`

### TEST_CASE `TEST_CASE("moonshine-cpp-test")`
- Defined: `core/moonshine-cpp-test.cpp:162`

### SUBCASE `SUBCASE("transcribe-without-streaming")`
- Defined: `core/moonshine-cpp-test.cpp:164`

### SUBCASE `SUBCASE("transcribe-with-streaming")`
- Defined: `core/moonshine-cpp-test.cpp:193`

### SUBCASE `SUBCASE("g2p")`
- Defined: `core/moonshine-cpp-test.cpp:288`

### SUBCASE `SUBCASE("intent recognizer invalid model path throws")`
- Defined: `core/moonshine-cpp-test.cpp:306`

### SUBCASE `SUBCASE("spelling-mode-replaces-line-text-via-cpp-ctor")`
- Defined: `core/moonshine-cpp-test.cpp:312`

### SUBCASE `SUBCASE("loadFromMemory-with-spelling-buffer")`
- Defined: `core/moonshine-cpp-test.cpp:347`

### SUBCASE `SUBCASE("intent recognizer closest intents when embedding model present")`
- Defined: `core/moonshine-cpp-test.cpp:395`

## core/moonshine-cpp.h

### onLineStarted `* public:
 *     void onLineStarted(const moonshine::LineStarted& event) override`
- Defined: `core/moonshine-cpp.h:15`

### onLineCompleted `*     void onLineCompleted(const moonshine::LineCompleted& event) override`
- Defined: `core/moonshine-cpp.h:19`

### main `*
 * int main()`
- Defined: `core/moonshine-cpp.h:23`

### WordTiming `WordTiming() : start(0.0f), end(0.0f), confidence(0.0f)`
- Defined: `core/moonshine-cpp.h:92`

### WordTiming `WordTiming(const std::string &word, float start, float end, float confidence)
      : word(word),...`
- Defined: `core/moonshine-cpp.h:94`

### SpeakerSpan `SpeakerSpan()
      : startTime(0.0f),
        duration(0.0f),
        speakerId(0),
        spea...`
- Defined: `core/moonshine-cpp.h:119`

### SpeakerSpan `SpeakerSpan(float startTime, float duration, uint64_t speakerId,
              uint32_t speakerIn...`
- Defined: `core/moonshine-cpp.h:127`

### TranscriptLine `TranscriptLine()
      : startTime(0.0f),
        duration(0.0f),
        lineId(0),
        isCo...`
- Defined: `core/moonshine-cpp.h:186`
- Doc: Default constructor

### TranscriptLine `TranscriptLine(const transcript_line_t &line_c)
      : startTime(line_c.start_time),
        dur...`
- Defined: `core/moonshine-cpp.h:198`
- Doc: Construct from C API structure

### toString `std::string toString() const`
- Defined: `core/moonshine-cpp.h:232`

### Transcript `Transcript()`
- Defined: `core/moonshine-cpp.h:269`
- Doc: Default constructor

### Transcript `Transcript(const transcript_t *transcript_c)`
- Defined: `core/moonshine-cpp.h:272`
- Doc: Construct from C API structure

### toString `std::string toString() const`
- Defined: `core/moonshine-cpp.h:282`

### TranscriptEvent `protected:
  TranscriptEvent(const TranscriptLine &line, int32_t streamHandle, Type type)
      :...`
- Defined: `core/moonshine-cpp.h:318`

### LineStarted `public:
  LineStarted(const TranscriptLine &line, int32_t streamHandle)
      : TranscriptEvent(l...`
- Defined: `core/moonshine-cpp.h:326`

### LineUpdated `public:
  LineUpdated(const TranscriptLine &line, int32_t streamHandle)
      : TranscriptEvent(l...`
- Defined: `core/moonshine-cpp.h:333`

### LineTextChanged `public:
  LineTextChanged(const TranscriptLine &line, int32_t streamHandle)
      : TranscriptEve...`
- Defined: `core/moonshine-cpp.h:340`

### LineSpeakersChanged `public:
  LineSpeakersChanged(const TranscriptLine &line, int32_t streamHandle)
      : Transcrip...`
- Defined: `core/moonshine-cpp.h:350`

### LineCompleted `public:
  LineCompleted(const TranscriptLine &line, int32_t streamHandle)
      : TranscriptEvent...`
- Defined: `core/moonshine-cpp.h:357`

### Error `Error(const std::string &errorMessage, int32_t streamHandle)
      : TranscriptEvent(TranscriptLi...`
- Defined: `core/moonshine-cpp.h:367`

### Error `Error(const std::string &errorMessage, const TranscriptLine &line,
        int32_t streamHandle)
...`
- Defined: `core/moonshine-cpp.h:371`

### onLineStarted `virtual void onLineStarted(const LineStarted &)`
- Defined: `core/moonshine-cpp.h:390`
- Doc: Called when a new transcription line starts

### onLineUpdated `virtual void onLineUpdated(const LineUpdated &)`
- Defined: `core/moonshine-cpp.h:393`
- Doc: Called when an existing transcription line is updated

### onLineTextChanged `virtual void onLineTextChanged(const LineTextChanged &)`
- Defined: `core/moonshine-cpp.h:396`
- Doc: Called when the text of a transcription line changes

### onLineSpeakersChanged `virtual void onLineSpeakersChanged(const LineSpeakersChanged &)`
- Defined: `core/moonshine-cpp.h:400`
- Doc: Called when the speaker spans of a transcription line change. Can be called for lines that are already complete.

### onLineCompleted `virtual void onLineCompleted(const LineCompleted &)`
- Defined: `core/moonshine-cpp.h:403`
- Doc: Called when a transcription line is completed

### onError `virtual void onError(const Error &)`
- Defined: `core/moonshine-cpp.h:406`
- Doc: Called when an error occurs

### MoonshineException `public:
  MoonshineException(const std::string &message)
      : std::runtime_error(message)`
- Defined: `core/moonshine-cpp.h:413`

### getHandle `int32_t getHandle() const`
- Defined: `core/moonshine-cpp.h:489`
- Doc: Get the stream handle (for internal use)

### getHandle `int32_t getHandle() const`
- Defined: `core/moonshine-cpp.h:641`
- Doc: Get the transcriber handle (for internal use)

### Transcriber `Transcriber(int32_t handle, ModelArch modelArch, double updateInterval)
      : handle_(handle),
...`
- Defined: `core/moonshine-cpp.h:646`
- Doc: Internal constructor used by ``loadFromMemory`` to wrap an already-acquired C handle without re-running the from-files l

### TtsSynthesisResult `TtsSynthesisResult() : sampleRateHz(0)`
- Defined: `core/moonshine-cpp.h:672`

### TtsSynthesisResult `TtsSynthesisResult(std::vector<float> samples, int32_t sampleRateHz)
      : samples(std::move(sa...`
- Defined: `core/moonshine-cpp.h:674`

### getLanguage `const std::string &getLanguage() const`
- Defined: `core/moonshine-cpp.h:748`
- Doc: Get the language tag

### getHandle `int32_t getHandle() const`
- Defined: `core/moonshine-cpp.h:751`
- Doc: Get the synthesizer handle (for internal use)

### getLanguage `const std::string &getLanguage() const`
- Defined: `core/moonshine-cpp.h:834`
- Doc: Get the language tag

### getHandle `int32_t getHandle() const`
- Defined: `core/moonshine-cpp.h:837`
- Doc: Get the phonemizer handle (for internal use)

### IntentMatch `IntentMatch(std::string phrase, float sim)
      : canonicalPhrase(std::move(phrase)), similarity...`
- Defined: `core/moonshine-cpp.h:863`

### getHandle `int32_t getHandle() const`
- Defined: `core/moonshine-cpp.h:919`

### Stream `inline Stream::Stream(Transcriber *transcriber, double updateInterval,
                      uint...`
- Defined: `core/moonshine-cpp.h:932`
- Doc: Stream implementation

### Stream `inline Stream::Stream(Stream &&other)
    : transcriber_(other.transcriber_),
      handle_(other...`
- Defined: `core/moonshine-cpp.h:944`

### start `inline void Stream::start()`
- Defined: `core/moonshine-cpp.h:970`

### stop `inline void Stream::stop()`
- Defined: `core/moonshine-cpp.h:974`

### addAudio `inline void Stream::addAudio(const std::vector<float> &audioData,
                             in...`
- Defined: `core/moonshine-cpp.h:985`

### updateTranscription `inline Transcript Stream::updateTranscription(uint32_t flags)`
- Defined: `core/moonshine-cpp.h:1001`

### addListener `inline void Stream::addListener(TranscriptEventListener *listener)`
- Defined: `core/moonshine-cpp.h:1010`

### addListener `inline void Stream::addListener(
    std::function<void(const TranscriptEvent &)> listener)`
- Defined: `core/moonshine-cpp.h:1016`

### removeListener `inline void Stream::removeListener(TranscriptEventListener *listener)`
- Defined: `core/moonshine-cpp.h:1021`

### removeListener `inline void Stream::removeListener(
    std::function<void(const TranscriptEvent &)> listener)`
- Defined: `core/moonshine-cpp.h:1027`

### remove_if `std::remove_if(
          functionListeners_.begin(), functionListeners_.end(),
          [&liste...`
- Defined: `core/moonshine-cpp.h:1034`

### removeAllListeners `inline void Stream::removeAllListeners()`
- Defined: `core/moonshine-cpp.h:1050`

### close `inline void Stream::close()`
- Defined: `core/moonshine-cpp.h:1055`

### notifyFromTranscript `inline void Stream::notifyFromTranscript(const Transcript &transcript)`
- Defined: `core/moonshine-cpp.h:1063`

### emit `inline void Stream::emit(const TranscriptEvent &event)`
- Defined: `core/moonshine-cpp.h:1083`

### emitError `inline void Stream::emitError(const std::string &errorMessage)`
- Defined: `core/moonshine-cpp.h:1167`

### buildOptions `inline OptionsBuffer buildOptions(
    const std::string &spellingModelPath,
    const std::vecto...`
- Defined: `core/moonshine-cpp.h:1186`

### Transcriber `inline Transcriber::Transcriber(const std::string &modelPath,
                                Mod...`
- Defined: `core/moonshine-cpp.h:1213`

### Transcriber `inline Transcriber::Transcriber(
    const std::string &modelPath, ModelArch modelArch, double up...`
- Defined: `core/moonshine-cpp.h:1225`

### loadFromMemory `inline Transcriber Transcriber::loadFromMemory(
    const uint8_t *encoderData, size_t encoderDat...`
- Defined: `core/moonshine-cpp.h:1241`

### Transcriber `inline Transcriber::Transcriber(Transcriber &&other)
    : handle_(other.handle_),
      modelPat...`
- Defined: `core/moonshine-cpp.h:1266`

### close `inline void Transcriber::close()`
- Defined: `core/moonshine-cpp.h:1294`

### transcribeWithoutStreaming `inline Transcript Transcriber::transcribeWithoutStreaming(
    const std::vector<float> &audioDat...`
- Defined: `core/moonshine-cpp.h:1302`

### getVersion `inline int32_t Transcriber::getVersion() const`
- Defined: `core/moonshine-cpp.h:1317`

### createStream `inline Stream Transcriber::createStream(double updateInterval, uint32_t flags)`
- Defined: `core/moonshine-cpp.h:1321`

### getDefaultStream `inline Stream &Transcriber::getDefaultStream()`
- Defined: `core/moonshine-cpp.h:1325`

### start `inline void Transcriber::start()`
- Defined: `core/moonshine-cpp.h:1332`

### stop `inline void Transcriber::stop()`
- Defined: `core/moonshine-cpp.h:1334`

### addAudio `inline void Transcriber::addAudio(const std::vector<float> &audioData,
                          ...`
- Defined: `core/moonshine-cpp.h:1340`

### updateTranscription `inline Transcript Transcriber::updateTranscription(uint32_t flags)`
- Defined: `core/moonshine-cpp.h:1345`

### addListener `inline void Transcriber::addListener(TranscriptEventListener *listener)`
- Defined: `core/moonshine-cpp.h:1349`

### addListener `inline void Transcriber::addListener(
    std::function<void(const TranscriptEvent &)> listener)`
- Defined: `core/moonshine-cpp.h:1353`

### removeListener `inline void Transcriber::removeListener(TranscriptEventListener *listener)`
- Defined: `core/moonshine-cpp.h:1358`

### removeListener `inline void Transcriber::removeListener(
    std::function<void(const TranscriptEvent &)> listener)`
- Defined: `core/moonshine-cpp.h:1364`

### removeAllListeners `inline void Transcriber::removeAllListeners()`
- Defined: `core/moonshine-cpp.h:1371`

### parseTranscript `inline Transcript Transcriber::parseTranscript(
    const transcript_t *transcript_c)`
- Defined: `core/moonshine-cpp.h:1377`

### checkError `inline void Transcriber::checkError(int32_t error) const`
- Defined: `core/moonshine-cpp.h:1382`

### checkError `inline void Stream::checkError(int32_t error) const`
- Defined: `core/moonshine-cpp.h:1390`

### TextToSpeech `inline TextToSpeech::TextToSpeech(
    const std::string &language, const std::vector<moonshine_o...`
- Defined: `core/moonshine-cpp.h:1400`
- Doc: TextToSpeech implementation

### TextToSpeech `inline TextToSpeech::TextToSpeech(TextToSpeech &&other)
    : handle_(other.handle_), language_(s...`
- Defined: `core/moonshine-cpp.h:1410`

### synthesize `inline TtsSynthesisResult TextToSpeech::synthesize(
    const std::string &text, const std::vecto...`
- Defined: `core/moonshine-cpp.h:1425`

### synthesizeFromPhonemes `inline TtsSynthesisResult TextToSpeech::synthesizeFromPhonemes(
    const std::string &phonemes,
...`
- Defined: `core/moonshine-cpp.h:1445`

### close `inline void TextToSpeech::close()`
- Defined: `core/moonshine-cpp.h:1466`

### getVoices `inline std::string TextToSpeech::getVoices(
    const std::string &languages,
    const std::vect...`
- Defined: `core/moonshine-cpp.h:1473`

### getDependencies `inline std::string TextToSpeech::getDependencies(
    const std::string &languages,
    const std...`
- Defined: `core/moonshine-cpp.h:1493`

### checkError `inline void TextToSpeech::checkError(int32_t error) const`
- Defined: `core/moonshine-cpp.h:1513`

### GraphemeToPhonemizer `inline GraphemeToPhonemizer::GraphemeToPhonemizer(
    const std::string &language, const std::ve...`
- Defined: `core/moonshine-cpp.h:1523`
- Doc: GraphemeToPhonemizer implementation

### GraphemeToPhonemizer `inline GraphemeToPhonemizer::GraphemeToPhonemizer(GraphemeToPhonemizer &&other)
    : handle_(oth...`
- Defined: `core/moonshine-cpp.h:1533`

### toIpa `inline std::string GraphemeToPhonemizer::toIpa(
    const std::string &text, const std::vector<mo...`
- Defined: `core/moonshine-cpp.h:1549`

### close `inline void GraphemeToPhonemizer::close()`
- Defined: `core/moonshine-cpp.h:1565`

### getDependencies `inline std::string GraphemeToPhonemizer::getDependencies(
    const std::string &languages,
    c...`
- Defined: `core/moonshine-cpp.h:1572`

### checkError `inline void GraphemeToPhonemizer::checkError(int32_t error) const`
- Defined: `core/moonshine-cpp.h:1592`

### IntentRecognizer `inline IntentRecognizer::IntentRecognizer(const std::string &model_path,
                        ...`
- Defined: `core/moonshine-cpp.h:1600`

### IntentRecognizer `inline IntentRecognizer::IntentRecognizer(IntentRecognizer &&other) noexcept
    : handle_(other....`
- Defined: `core/moonshine-cpp.h:1611`

### registerIntent `inline void IntentRecognizer::registerIntent(
    const std::string &canonical_phrase, float *emb...`
- Defined: `core/moonshine-cpp.h:1626`

### unregisterIntent `inline bool IntentRecognizer::unregisterIntent(
    const std::string &canonical_phrase)`
- Defined: `core/moonshine-cpp.h:1633`

### getClosestIntents `inline std::vector<IntentMatch> IntentRecognizer::getClosestIntents(
    const std::string &utter...`
- Defined: `core/moonshine-cpp.h:1646`

### intentCount `inline int32_t IntentRecognizer::intentCount() const`
- Defined: `core/moonshine-cpp.h:1670`

### clearIntents `inline void IntentRecognizer::clearIntents()`
- Defined: `core/moonshine-cpp.h:1680`

### calculateEmbedding `inline std::vector<float> IntentRecognizer::calculateEmbedding(
    const std::string &sentence, ...`
- Defined: `core/moonshine-cpp.h:1684`

### close `inline void IntentRecognizer::close()`
- Defined: `core/moonshine-cpp.h:1698`

### checkError `inline void IntentRecognizer::checkError(int32_t error) const`
- Defined: `core/moonshine-cpp.h:1705`

## core/moonshine-download-smoke.cpp

### print_usage `void print_usage()`
- Defined: `core/moonshine-download-smoke.cpp:44`

### url_encode_path `std::string url_encode_path(const std::string& key)`
- Defined: `core/moonshine-download-smoke.cpp:52`

### fail `int fail(const std::string& message)`
- Defined: `core/moonshine-download-smoke.cpp:72`

### print_group_manifest `void print_group_manifest(const std::string& json_text)`
- Defined: `core/moonshine-download-smoke.cpp:82`
- Doc: Emits "<url>\t<relative_path>" for every file in a {"groups":[...]} manifest produced by moonshine_get_stt_dependencies 

### manifest_stt `int manifest_stt(const std::vector<std::string>& spec)`
- Defined: `core/moonshine-download-smoke.cpp:92`

### manifest_intent `int manifest_intent(const std::vector<std::string>& spec)`
- Defined: `core/moonshine-download-smoke.cpp:114`

### manifest_tts `int manifest_tts(const std::vector<std::string>& spec)`
- Defined: `core/moonshine-download-smoke.cpp:134`

### manifest_g2p `int manifest_g2p(const std::vector<std::string>& spec)`
- Defined: `core/moonshine-download-smoke.cpp:165`

### load_speech_or_tone `std::vector<float> load_speech_or_tone()`
- Defined: `core/moonshine-download-smoke.cpp:196`
- Doc: ------------------------------- run mode ---------------------------------

### is_streaming_arch `bool is_streaming_arch(uint32_t arch)`
- Defined: `core/moonshine-download-smoke.cpp:233`

### run_stt `int run_stt(const std::string& root, const std::vector<std::string>& spec)`
- Defined: `core/moonshine-download-smoke.cpp:240`

### run_intent `int run_intent(const std::string& root, const std::vector<std::string>& spec)`
- Defined: `core/moonshine-download-smoke.cpp:294`

### run_tts `int run_tts(const std::string& root, const std::vector<std::string>& spec)`
- Defined: `core/moonshine-download-smoke.cpp:322`

### run_g2p `int run_g2p(const std::string& root, const std::vector<std::string>& spec)`
- Defined: `core/moonshine-download-smoke.cpp:360`

### main `int main(int argc, char** argv)`
- Defined: `core/moonshine-download-smoke.cpp:387`

## core/moonshine-model-catalog.cpp

### to_lower `std::string to_lower(std::string s)`
- Defined: `core/moonshine-model-catalog.cpp:39`

### transform `std::transform(s.begin(), s.end(), s.begin(), [](unsigned char c)`
- Defined: `core/moonshine-model-catalog.cpp:41`

### is_streaming_arch `bool is_streaming_arch(int32_t model_arch)`
- Defined: `core/moonshine-model-catalog.cpp:46`

### stt_catalog `const std::vector<SttLanguageEntry>& stt_catalog()`
- Defined: `core/moonshine-model-catalog.cpp:56`
- Doc: Port of MODEL_INFO from python/src/moonshine_voice/download.py. The first model listed for a language is its default.

### embedding_catalog `const std::vector<EmbeddingModelEntry>& embedding_catalog()`
- Defined: `core/moonshine-model-catalog.cpp:123`
- Doc: Port of EMBEDDING_MODEL_INFO.

### find_stt_language `const SttLanguageEntry* find_stt_language(const std::string& language)`
- Defined: `core/moonshine-model-catalog.cpp:132`

### stt_component_files `std::vector<std::string> stt_component_files(const std::string& language_code,
                  ...`
- Defined: `core/moonshine-model-catalog.cpp:147`

### find_spelling_model `const SpellingModelEntry* find_spelling_model(const std::string& language_code)`
- Defined: `core/moonshine-model-catalog.cpp:169`

### find_embedding_model `const EmbeddingModelEntry* find_embedding_model(const std::string& model_name)`
- Defined: `core/moonshine-model-catalog.cpp:178`

### embedding_component_files `std::vector<std::string> embedding_component_files(const std::string& variant)`
- Defined: `core/moonshine-model-catalog.cpp:194`
- Doc: The C++ embedding loader (gemma-embedding-model.cpp) maps each variant to a specific ONNX filename. Note that "q8" resol

### stt_model_dependencies `std::optional<ModelDependencies> stt_model_dependencies(
    const std::string& language, std::op...`
- Defined: `core/moonshine-model-catalog.cpp:213`

### intent_model_dependencies `std::optional<ModelDependencies> intent_model_dependencies(
    const std::string& model_name, co...`
- Defined: `core/moonshine-model-catalog.cpp:250`

### stt_supported_languages `std::vector<std::string> stt_supported_languages()`
- Defined: `core/moonshine-model-catalog.cpp:272`

### intent_supported_models `std::vector<std::string> intent_supported_models()`
- Defined: `core/moonshine-model-catalog.cpp:280`

### intent_supported_variants `std::vector<std::string> intent_supported_variants(
    const std::string& model_name)`
- Defined: `core/moonshine-model-catalog.cpp:288`

## core/moonshine-model.cpp

### set_model_options_from_arch `int set_model_options_from_arch(MoonshineModel *model, int32_t model_arch)`
- Defined: `core/moonshine-model.cpp:60`

### MoonshineModel `MoonshineModel::MoonshineModel(
    bool log_ort_run, float max_tokens_per_second,
    const std:...`
- Defined: `core/moonshine-model.cpp:81`

### load `int MoonshineModel::load(const char *encoder_model_path,
                         const char *dec...`
- Defined: `core/moonshine-model.cpp:144`

### load_from_memory `int MoonshineModel::load_from_memory(const uint8_t *encoder_model_data,
                         ...`
- Defined: `core/moonshine-model.cpp:162`

### load_from_assets `int MoonshineModel::load_from_assets(const char *encoder_model_path,
                            ...`
- Defined: `core/moonshine-model.cpp:186`
- Doc: if defined(ANDROID)

### transcribe `int MoonshineModel::transcribe(const float *input_audio_data,
                               size...`
- Defined: `core/moonshine-model.cpp:215`
- Doc: endif

### transcribe_wav `int MoonshineModel::transcribe_wav(const char *wav_path, char **out_text)`
- Defined: `core/moonshine-model.cpp:564`

### load_alignment_model `int MoonshineModel::load_alignment_model(const char *alignment_model_path)`
- Defined: `core/moonshine-model.cpp:579`

### compute_word_timestamps `int MoonshineModel::compute_word_timestamps(
    float audio_duration, std::vector<TranscriberWor...`
- Defined: `core/moonshine-model.cpp:590`

## core/moonshine-streaming-model.cpp

### read_file_to_string `static std::string read_file_to_string(const std::string &path)`
- Defined: `core/moonshine-streaming-model.cpp:48`
- Doc: ============================================================================ Helper Functions ==========================

### parse_config_json `static bool parse_config_json(const std::string &json,
                              MoonshineStr...`
- Defined: `core/moonshine-streaming-model.cpp:58`
- Doc: TODO Use constants instead of loading config JSON

### reset `void MoonshineStreamingState::reset(const MoonshineStreamingConfig &cfg)`
- Defined: `core/moonshine-streaming-model.cpp:106`
- Doc: ============================================================================ MoonshineStreamingState Implementation ====

### MoonshineStreamingModel `MoonshineStreamingModel::MoonshineStreamingModel(
    bool log_ort_run, const std::vector<std::st...`
- Defined: `core/moonshine-streaming-model.cpp:145`
- Doc: ============================================================================ MoonshineStreamingModel Implementation ====

### load_config `int MoonshineStreamingModel::load_config(const char *config_path)`
- Defined: `core/moonshine-streaming-model.cpp:199`

### load_config_from_string `int MoonshineStreamingModel::load_config_from_string(const std::string &json)`
- Defined: `core/moonshine-streaming-model.cpp:208`

### load `int MoonshineStreamingModel::load(const char *model_dir,
                                  const ...`
- Defined: `core/moonshine-streaming-model.cpp:216`

### load_from_memory `int MoonshineStreamingModel::load_from_memory(
    const uint8_t *frontend_model_data, size_t fro...`
- Defined: `core/moonshine-streaming-model.cpp:289`

### load_from_assets `int MoonshineStreamingModel::load_from_assets(const char *model_dir,
                            ...`
- Defined: `core/moonshine-streaming-model.cpp:332`
- Doc: if defined(ANDROID)

### create_state `MoonshineStreamingState *MoonshineStreamingModel::create_state()`
- Defined: `core/moonshine-streaming-model.cpp:404`
- Doc: endif

### tokens_to_text `std::string MoonshineStreamingModel::tokens_to_text(
    const std::vector<int64_t> &tokens)`
- Defined: `core/moonshine-streaming-model.cpp:410`

### process_audio_chunk `int MoonshineStreamingModel::process_audio_chunk(MoonshineStreamingState *state,
                ...`
- Defined: `core/moonshine-streaming-model.cpp:420`
- Doc: ============================================================================ Streaming Inference Implementation ========

### encode `int MoonshineStreamingModel::encode(MoonshineStreamingState *state,
                             ...`
- Defined: `core/moonshine-streaming-model.cpp:583`

### compute_cross_kv `int MoonshineStreamingModel::compute_cross_kv(MoonshineStreamingState *state)`
- Defined: `core/moonshine-streaming-model.cpp:758`
- Doc: ============================================================================ Compute cross-attention K/V from memory (fo

### run_decoder_with_cross_kv `int MoonshineStreamingModel::run_decoder_with_cross_kv(
    MoonshineStreamingState *state, const...`
- Defined: `core/moonshine-streaming-model.cpp:846`
- Doc: ============================================================================ Run decoder with precomputed cross K/V (mor

### decode_step `int MoonshineStreamingModel::decode_step(MoonshineStreamingState *state,
                        ...`
- Defined: `core/moonshine-streaming-model.cpp:1068`
- Doc: ============================================================================ Single-token decode step ==================

### decode_tokens `int MoonshineStreamingModel::decode_tokens(MoonshineStreamingState *state,
                      ...`
- Defined: `core/moonshine-streaming-model.cpp:1115`
- Doc: ============================================================================ Multi-token decode step ===================

### decode_full `int MoonshineStreamingModel::decode_full(MoonshineStreamingState *state,
                        ...`
- Defined: `core/moonshine-streaming-model.cpp:1171`
- Doc: ============================================================================ Full decode with speculative decoding suppo

### decoder_reset `void MoonshineStreamingModel::decoder_reset(MoonshineStreamingState *state)`
- Defined: `core/moonshine-streaming-model.cpp:1343`

## core/moonshine-tts/src/file-information.cpp

### FileInformation `FileInformation::FileInformation(const FileInformation& o)
    : path(o.path), owned_storage_(o.o...`
- Defined: `core/moonshine-tts/src/file-information.cpp:7`

### load `void FileInformation::load(const uint8_t** out_memory, size_t* out_size)`
- Defined: `core/moonshine-tts/src/file-information.cpp:34`

### free `void FileInformation::free()`
- Defined: `core/moonshine-tts/src/file-information.cpp:80`

### set_memory `void FileInformationMap::set_memory(std::string_view key, const uint8_t* mem,
                   ...`
- Defined: `core/moonshine-tts/src/file-information.cpp:89`

### parse_file_list `void FileInformationMap::parse_file_list(
    const std::vector<std::pair<std::string, std::strin...`
- Defined: `core/moonshine-tts/src/file-information.cpp:98`

## core/moonshine-tts/src/file-information.h

### FileInformation `FileInformation(std::filesystem::path p, const uint8_t* mem, size_t sz)
      : path(std::move(p)...`
- Defined: `core/moonshine-tts/src/file-information.h:24`

### set_path `void set_path(std::string_view key, std::filesystem::path path)`
- Defined: `core/moonshine-tts/src/file-information.h:53`

### erase_key `void erase_key(std::string_view key)`
- Defined: `core/moonshine-tts/src/file-information.h:62`

### contains `bool contains(std::string_view key) const`
- Defined: `core/moonshine-tts/src/file-information.h:64`

## core/moonshine-tts/src/g2p-path.h

### resolve_path_under_root `inline std::filesystem::path resolve_path_under_root(
    const std::filesystem::path& root, cons...`
- Defined: `core/moonshine-tts/src/g2p-path.h:13`
- Doc: If ``path`` is absolute, returns it unchanged. If ``root`` is empty, returns ``path`` (relative to the process working d

### resolve_prefer_ort_model `inline std::filesystem::path resolve_prefer_ort_model(
    const std::filesystem::path& dir, std:...`
- Defined: `core/moonshine-tts/src/g2p-path.h:30`
- Doc: Prefer ``stem.ort`` when present, else ``stem.onnx`` (``basename`` may end with ``.ort`` or ``.onnx``). If neither exist

### resolve_disk_model_file_path `inline void resolve_disk_model_file_path(std::filesystem::path& path)`
- Defined: `core/moonshine-tts/src/g2p-path.h:56`
- Doc: For a path whose basename ends with ``.ort`` or ``.onnx``, set ``path`` to the existing sibling preferring ``stem.ort`` 

## core/moonshine-tts/src/g2p-word-log.cpp

### g2p_word_path_tag `const char* g2p_word_path_tag(G2pWordPath path)`
- Defined: `core/moonshine-tts/src/g2p-word-log.cpp:6`

### format_g2p_word_log_line `std::string format_g2p_word_log_line(const G2pWordLog& e)`
- Defined: `core/moonshine-tts/src/g2p-word-log.cpp:34`

## core/moonshine-tts/src/ipa-postprocess.cpp

### replace_utf8_all `void replace_utf8_all(std::string& s, std::string_view old_utf8,
                      std::strin...`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:20`

### trim_copy `std::string trim_copy(std::string t)`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:29`

### strip_length_markers_copy `std::string strip_length_markers_copy(std::string t)`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:36`

### apply_shared_g2p_to_piper_replacements `void apply_shared_g2p_to_piper_replacements(std::string& s)`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:45`

### apply_korean_post_normalize_ipa `void apply_korean_post_normalize_ipa(std::string& s)`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:53`

### apply_german_ipa_piper_style `void apply_german_ipa_piper_style(std::string& s)`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:76`
- Doc: U+0361 COMBINING DOUBLE INVERTED BREVE between consonants (narrow IPA tie bar) → espeak digraph.

### apply_lang_specific_replacements `void apply_lang_specific_replacements(std::string& s,
                                      std::...`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:105`

### py_isspace_one_utf8_char `bool py_isspace_one_utf8_char(std::string_view ch)`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:150`

### unicode_category_first_char_is_p_or_s `bool unicode_category_first_char_is_p_or_s(char32_t cp)`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:169`

### category_is_mn_or_me `bool category_is_mn_or_me(char32_t cp)`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:174`

### is_ipa_like_inventory_char `bool is_ipa_like_inventory_char(char32_t cp)`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:180`

### utf8_singleton_codepoint `char32_t utf8_singleton_codepoint(std::string_view token)`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:205`

### utf8_prev_codepoint_start `size_t utf8_prev_codepoint_start(const std::string& s, size_t char_start)`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:215`

### rewrite_russian_combining_acute_to_primary_stress `void rewrite_russian_combining_acute_to_primary_stress(std::string& s)`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:230`
- Doc: Map combining acute (U+0301) after a nucleus onto U+02C8 ˈ (Piper-style modifier stress). If the nucleus already has ˈ/ˌ

### apply_russian_ipa_piper_style `void apply_russian_ipa_piper_style(std::string& s)`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:276`
- Doc: Russian G2P uses narrow-IPA tie bars and retroflex letters; Piper / Kokoro / espeak-ng expect digraph affricates, /ʃ/ /ʒ

### repair_ascii_c_combining_cedilla_to_ccedilla_utf8 `void repair_ascii_c_combining_cedilla_to_ccedilla_utf8(std::string& s)`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:367`

### normalize_russian_ipa_piper_style `std::string normalize_russian_ipa_piper_style(std::string ipa)`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:378`

### normalize_german_ipa_piper_style `std::string normalize_german_ipa_piper_style(std::string ipa)`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:383`

### is_cmn_vowel_cp `bool is_cmn_vowel_cp(char32_t cp)`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:394`
- Doc: True for IPA vowel codepoints used in Mandarin (after mapping).

### is_cmn_tone_marker `bool is_cmn_tone_marker(char32_t cp)`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:416`
- Doc: True for espeak-ng Mandarin tone markers (single characters placed in syllables).

### normalize_chinese_ipa_piper_style `std::string normalize_chinese_ipa_piper_style(std::string ipa)`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:420`

### utf8_nfc_copy `std::string utf8_nfc_copy(std::string_view s)`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:659`

### normalize_g2p_ipa_for_piper `std::string normalize_g2p_ipa_for_piper(std::string_view ipa_utf8,
                              ...`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:671`

### coerce_unknown_ipa_chars_to_piper_inventory `std::string coerce_unknown_ipa_chars_to_piper_inventory(
    std::string_view ipa_utf8,
    const...`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:689`

### ipa_to_piper_ready `std::string ipa_to_piper_ready(
    std::string_view ipa_utf8, std::string_view piper_lang_key,
 ...`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:761`

### normalize_g2p_ipa_for_piper_engines `std::string normalize_g2p_ipa_for_piper_engines(std::string_view ipa_utf8)`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:773`

### ipa_string_to_phoneme_tokens `std::vector<std::string> ipa_string_to_phoneme_tokens(const std::string& s)`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:779`

### levenshtein_distance `int levenshtein_distance(const std::vector<std::string>& a,
                         const std::v...`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:805`

### pick_closest_alternative_index `int pick_closest_alternative_index(
    const std::vector<std::string>& predicted_phoneme_tokens,...`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:836`

### pick_closest_cmudict_ipa `std::string pick_closest_cmudict_ipa(
    const std::vector<std::string>& predicted_phoneme_token...`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:865`

### match_prediction_to_cmudict_ipa `std::optional<std::string> match_prediction_to_cmudict_ipa(
    const std::string& predicted, con...`
- Defined: `core/moonshine-tts/src/ipa-postprocess.cpp:881`

## core/moonshine-tts/src/json-config.cpp

### read_json_file `nlohmann::json read_json_file(const std::filesystem::path& p)`
- Defined: `core/moonshine-tts/src/json-config.cpp:13`

### validate_header `void validate_header(const nlohmann::json& cfg, const std::string& expect_kind,
                 ...`
- Defined: `core/moonshine-tts/src/json-config.cpp:23`

### stoi_to_itos `std::vector<std::string> stoi_to_itos(
    const std::unordered_map<std::string, int64_t>& stoi)`
- Defined: `core/moonshine-tts/src/json-config.cpp:46`

### load_oov_tables_from_json `OovOnnxTables load_oov_tables_from_json(const nlohmann::json& cfg,
                              ...`
- Defined: `core/moonshine-tts/src/json-config.cpp:63`

### load_oov_tables `OovOnnxTables load_oov_tables(const std::filesystem::path& model_onnx_path)`
- Defined: `core/moonshine-tts/src/json-config.cpp:87`

## core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp

### open_ar_session `std::unique_ptr<Ort::Session> open_ar_session(
    Ort::Env& env, const std::filesystem::path& mo...`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:33`

### open_ar_session_memory `std::unique_ptr<Ort::Session> open_ar_session_memory(
    Ort::Env& env, const void* data, size_t...`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:50`

### slurp_utf8_file_ar `std::string slurp_utf8_file_ar(const std::filesystem::path& p)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:64`

### bundle_load_utf8_ar `bool bundle_load_utf8_ar(const MoonshineG2POptions* opt,
                         std::string_vie...`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:74`

### bundle_load_binary_ar `bool bundle_load_binary_ar(const MoonshineG2POptions* opt,
                           std::string...`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:93`

### utf8_to_u32 `std::u32string utf8_to_u32(std::string_view utf8)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:126`

### u32_to_utf8 `std::string u32_to_utf8(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:139`

### is_space_u32 `bool is_space_u32(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:147`

### is_control_u32 `bool is_control_u32(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:156`

### is_punctuation_u32 `bool is_punctuation_u32(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:165`

### is_punct_char_word_group_u32 `bool is_punct_char_word_group_u32(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:179`
- Doc: ``token_word_group_indices`` uses :func:`_is_punct_char` (Unicode **P** categories only), not the broader BERT ``_is_pun

### is_chinese_char `bool is_chinese_char(std::uint32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:183`

### u32_nfc `std::u32string u32_nfc(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:192`

### strip_mn_nfd `std::u32string strip_mn_nfd(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:204`

### to_lower_u32 `std::u32string to_lower_u32(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:224`

### clean_text_u32 `std::u32string clean_text_u32(const std::u32string& text)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:233`

### tokenize_chinese_chars_u32 `std::u32string tokenize_chinese_chars_u32(const std::u32string& text)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:245`

### split_u32_whitespace `std::vector<std::u32string> split_u32_whitespace(std::u32string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:259`

### run_split_on_punc_u32 `std::vector<std::u32string> run_split_on_punc_u32(const std::u32string& text)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:284`

### normalization_ref_u32 `std::u32string normalization_ref_u32(const std::u32string& text_u32,
                            ...`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:320`

### basic_tokenize_u32 `std::vector<std::u32string> basic_tokenize_u32(
    const std::u32string& original_text_u32, cons...`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:329`

### align_basic_tokens_u32 `void align_basic_tokens_u32(const std::u32string& ref,
                            const std::vec...`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:361`

### wordpiece_tokenize_u32 `std::vector<std::u32string> wordpiece_tokenize_u32(
    const std::u32string& token,
    const st...`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:378`

### encode_bert_wordpiece `EncodedWp encode_bert_wordpiece(
    const std::u32string& text_u32,
    const std::unordered_map...`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:433`

### is_arabic_anchor_char `bool is_arabic_anchor_char(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:671`

### anchor_index_for_span `std::optional<int> anchor_index_for_span(const std::u32string& ref, int s,
                      ...`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:685`

### strip_arabic_diacritics_u32 `std::u32string strip_arabic_diacritics_u32(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:699`

### ArabicDiacOnnx `ArabicDiacOnnx::ArabicDiacOnnx(const MoonshineG2POptions* opt,
                               std...`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:725`

### diacritize `std::string ArabicDiacOnnx::diacritize(std::string_view text_utf8) const`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:786`

## core/moonshine-tts/src/lang-specific/arabic-diac-onnx.h

### model_dir `const std::filesystem::path& model_dir() const`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.h:38`

## core/moonshine-tts/src/lang-specific/arabic-ipa.cpp

### is_ar_combining `bool is_ar_combining(char32_t ch)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:22`

### is_ar_base_letter `bool is_ar_base_letter(char32_t ch)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:35`

### u32_nfc_u32 `std::u32string u32_nfc_u32(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:52`

### strip_ar_diac_u32 `std::u32string strip_ar_diac_u32(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:67`

### u32_to_utf8_str `std::string u32_to_utf8_str(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:78`

### has_vowel_mark_u32 `bool has_vowel_mark_u32(const std::u32string& marks)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:86`

### strip_spurious_tatweil_u32 `std::u32string strip_spurious_tatweil_u32(const std::u32string& w)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:135`

### apply_default_fatha_u32 `std::u32string apply_default_fatha_u32(const std::u32string& w)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:159`

### onset_ipa `std::string onset_ipa(char32_t base)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:202`

### vowel_from_marks `std::string vowel_from_marks(const std::u32string& marks)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:272`

### gem_ipa `std::string gem_ipa(const std::string& onset)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:308`

### diac_word_to_ipa_u32 `std::string diac_word_to_ipa_u32(const std::u32string& word)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:319`

### arabic_msa_strip_diacritics_utf8 `std::string arabic_msa_strip_diacritics_utf8(std::string_view utf8)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:401`

### arabic_msa_apply_onnx_partial_postprocess_utf8 `std::string arabic_msa_apply_onnx_partial_postprocess_utf8(
    std::string_view utf8)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:406`

### arabic_msa_word_to_ipa_with_assimilation_utf8 `std::string arabic_msa_word_to_ipa_with_assimilation_utf8(
    std::string_view filled_diac_utf8,...`
- Defined: `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp:414`

## core/moonshine-tts/src/lang-specific/arabic.cpp

### absolute_model_root_ar `std::filesystem::path absolute_model_root_ar(
    const std::filesystem::path& model_root)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic.cpp:18`

### has_arabic_script `bool has_arabic_script(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic.cpp:32`

### strip_lex_ipa_segment_dots `std::string strip_lex_ipa_segment_dots(std::string ipa)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic.cpp:92`

### ArabicRuleG2p `ArabicRuleG2p::ArabicRuleG2p(std::filesystem::path onnx_model_dir,
                             s...`
- Defined: `core/moonshine-tts/src/lang-specific/arabic.cpp:99`

### ArabicRuleG2p `ArabicRuleG2p::ArabicRuleG2p(std::filesystem::path onnx_model_dir,
                             s...`
- Defined: `core/moonshine-tts/src/lang-specific/arabic.cpp:105`

### ArabicRuleG2p `ArabicRuleG2p::ArabicRuleG2p(const MoonshineG2POptions& opt,
                             std::fi...`
- Defined: `core/moonshine-tts/src/lang-specific/arabic.cpp:114`

### ArabicRuleG2p `ArabicRuleG2p::ArabicRuleG2p(const MoonshineG2POptions& opt,
                             std::fi...`
- Defined: `core/moonshine-tts/src/lang-specific/arabic.cpp:121`

### dialect_ids `std::vector<std::string> ArabicRuleG2p::dialect_ids()`
- Defined: `core/moonshine-tts/src/lang-specific/arabic.cpp:131`

### dialect_resolves_to_arabic_rules `bool dialect_resolves_to_arabic_rules(std::string_view dialect_id)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic.cpp:136`

### resolve_arabic_dict_path `std::filesystem::path resolve_arabic_dict_path(
    const std::filesystem::path& model_root)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic.cpp:145`

### resolve_arabic_onnx_model_dir `std::filesystem::path resolve_arabic_onnx_model_dir(
    const std::filesystem::path& model_root)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic.cpp:151`

### g2p_word `std::string ArabicRuleG2p::g2p_word(std::string_view word_utf8)`
- Defined: `core/moonshine-tts/src/lang-specific/arabic.cpp:157`

### text_to_ipa `std::string ArabicRuleG2p::text_to_ipa(std::string text,
                                       s...`
- Defined: `core/moonshine-tts/src/lang-specific/arabic.cpp:173`

## core/moonshine-tts/src/lang-specific/arabic.h

### dialect_id `const std::string& dialect_id() const`
- Defined: `core/moonshine-tts/src/lang-specific/arabic.h:44`

## core/moonshine-tts/src/lang-specific/chinese-numbers.cpp

### digit_cp `char32_t digit_cp(unsigned d)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-numbers.cpp:16`

### cn_digit `std::string cn_digit(unsigned d)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-numbers.cpp:26`

### ends_with_ling_utf8 `bool ends_with_ling_utf8(const std::string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-numbers.cpp:32`

### section_under_10000 `std::string section_under_10000(unsigned n)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-numbers.cpp:40`

### int_to_han_u64 `std::string int_to_han_u64(std::uint64_t n)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-numbers.cpp:95`

### ascii_digit_string `bool ascii_digit_string(std::string_view t, std::uint64_t& out_val)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-numbers.cpp:145`

### int_to_mandarin_cardinal_han `std::string int_to_mandarin_cardinal_han(std::uint64_t n)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-numbers.cpp:165`

### arabic_numeral_token_to_han `std::optional<std::string> arabic_numeral_token_to_han(
    std::string_view token_sv)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-numbers.cpp:169`

## core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp

### utf8_nfc_utf8proc `std::string utf8_nfc_utf8proc(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp:15`

### ChineseOnnxG2p `ChineseOnnxG2p::ChineseOnnxG2p(std::filesystem::path model_dir,
                               st...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp:29`

### ChineseOnnxG2p `ChineseOnnxG2p::ChineseOnnxG2p(std::filesystem::path model_dir,
                               st...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp:33`

### ChineseOnnxG2p `ChineseOnnxG2p::ChineseOnnxG2p(const MoonshineG2POptions& opt,
                               std...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp:37`

### ChineseOnnxG2p `ChineseOnnxG2p::ChineseOnnxG2p(const MoonshineG2POptions& opt,
                               std...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp:43`

### text_to_ipa `std::string ChineseOnnxG2p::text_to_ipa(std::string text_utf8,
                                  ...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp:49`

### ChineseOnnxRuleG2p `ChineseOnnxRuleG2p::ChineseOnnxRuleG2p(std::filesystem::path onnx_model_dir,
                    ...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp:75`

### ChineseOnnxRuleG2p `ChineseOnnxRuleG2p::ChineseOnnxRuleG2p(std::filesystem::path onnx_model_dir,
                    ...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp:81`

### ChineseOnnxRuleG2p `ChineseOnnxRuleG2p::ChineseOnnxRuleG2p(const MoonshineG2POptions& opt,
                          ...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp:86`

### ChineseOnnxRuleG2p `ChineseOnnxRuleG2p::ChineseOnnxRuleG2p(const MoonshineG2POptions& opt,
                          ...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp:93`

### text_to_ipa `std::string ChineseOnnxRuleG2p::text_to_ipa(
    std::string text, std::vector<G2pWordLog>* per_w...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp:100`

## core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h

### tok `const ChineseTokPosOnnx& tok() const`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h:36`

## core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp

### open_session `std::unique_ptr<Ort::Session> open_session(
    Ort::Env& env, const std::filesystem::path& model...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:30`

### open_session_memory `std::unique_ptr<Ort::Session> open_session_memory(
    Ort::Env& env, const void* data, size_t le...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:47`

### slurp_utf8_file `std::string slurp_utf8_file(const std::filesystem::path& p)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:61`

### bundle_load_utf8 `bool bundle_load_utf8(const MoonshineG2POptions* opt,
                      std::string_view bund...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:71`

### bundle_load_binary `bool bundle_load_binary(const MoonshineG2POptions* opt,
                        std::string_view ...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:89`

### utf8_to_u32 `std::u32string utf8_to_u32(std::string_view utf8)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:122`

### u32_to_utf8 `std::string u32_to_utf8(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:135`

### is_space_u32 `bool is_space_u32(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:143`

### is_control_u32 `bool is_control_u32(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:152`

### is_punctuation_u32 `bool is_punctuation_u32(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:161`

### is_punct_char_word_group_u32 `bool is_punct_char_word_group_u32(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:175`
- Doc: ``token_word_group_indices`` uses :func:`_is_punct_char` (Unicode **P** categories only), not the broader BERT ``_is_pun

### is_chinese_char `bool is_chinese_char(std::uint32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:179`

### u32_nfc `std::u32string u32_nfc(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:188`

### strip_mn_nfd `std::u32string strip_mn_nfd(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:200`

### to_lower_u32 `std::u32string to_lower_u32(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:220`

### clean_text_u32 `std::u32string clean_text_u32(const std::u32string& text)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:229`

### tokenize_chinese_chars_u32 `std::u32string tokenize_chinese_chars_u32(const std::u32string& text)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:241`

### split_u32_whitespace `std::vector<std::u32string> split_u32_whitespace(std::u32string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:255`

### run_split_on_punc_u32 `std::vector<std::u32string> run_split_on_punc_u32(const std::u32string& text)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:280`

### normalization_ref_u32 `std::u32string normalization_ref_u32(const std::u32string& text_u32,
                            ...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:316`

### basic_tokenize_u32 `std::vector<std::u32string> basic_tokenize_u32(
    const std::u32string& original_text_u32, cons...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:337`

### align_basic_tokens_u32 `void align_basic_tokens_u32(const std::u32string& ref,
                            const std::vec...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:369`

### wordpiece_tokenize_u32 `std::vector<std::u32string> wordpiece_tokenize_u32(
    const std::u32string& token,
    const st...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:386`

### encode_bert_wordpiece `EncodedWp encode_bert_wordpiece(
    const std::u32string& text_u32,
    const std::unordered_map...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:441`

### cjk_tokpos_preferred_chunk_break_cp `bool cjk_tokpos_preferred_chunk_break_cp(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:631`

### cjk_tokpos_chunk_exclusive_end `template <typename EncodeFn>
std::size_t cjk_tokpos_chunk_exclusive_end(const std::u32string& ful...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:664`

### default_chinese_tok_pos_model_dir `std::filesystem::path default_chinese_tok_pos_model_dir(
    const std::filesystem::path& g2p_dat...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:703`

### ChineseTokPosOnnx `ChineseTokPosOnnx::ChineseTokPosOnnx(const MoonshineG2POptions* opt,
                            ...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:713`

### format_annotated_line `std::string ChineseTokPosOnnx::format_annotated_line(
    const std::vector<std::pair<std::string...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp:774`

## core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.h

### model_dir `const std::filesystem::path& model_dir() const`
- Defined: `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.h:41`

## core/moonshine-tts/src/lang-specific/chinese.cpp

### trim_copy_line `std::string trim_copy_line(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese.cpp:22`

### is_cjk_cp `bool is_cjk_cp(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese.cpp:36`

### is_ascii_digit_cp `bool is_ascii_digit_cp(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese.cpp:43`

### is_fullwidth_digit_cp `bool is_fullwidth_digit_cp(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese.cpp:45`

### token_has_g2p_content `bool token_has_g2p_content(const std::string& tok)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese.cpp:49`

### pos_in_set `bool pos_in_set(std::string_view p, const std::unordered_set<std::string>& s)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese.cpp:67`

### skip_phonetic_pos `const std::unordered_set<std::string>& skip_phonetic_pos()`
- Defined: `core/moonshine-tts/src/lang-specific/chinese.cpp:71`

### verb_like_pos `const std::unordered_set<std::string>& verb_like_pos()`
- Defined: `core/moonshine-tts/src/lang-specific/chinese.cpp:77`

### noun_like_pos `const std::unordered_set<std::string>& noun_like_pos()`
- Defined: `core/moonshine-tts/src/lang-specific/chinese.cpp:84`

### ipa_contains `bool ipa_contains(const std::string& ipa, std::string_view sub)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese.cpp:91`

### try_consume_g2p_token `bool try_consume_g2p_token(const std::string& text, size_t pos,
                           size_t...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese.cpp:95`

### load_chinese_lexicon_stream `void load_chinese_lexicon_stream(
    std::istream& in,
    std::unordered_map<std::string, std::...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese.cpp:190`

### ChineseRuleG2p `ChineseRuleG2p::ChineseRuleG2p(std::filesystem::path dict_tsv)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese.cpp:214`

### ChineseRuleG2p `ChineseRuleG2p::ChineseRuleG2p(std::string dict_tsv_utf8)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese.cpp:231`

### disambiguate_heteronym `std::string ChineseRuleG2p::disambiguate_heteronym(
    std::string_view word, std::string_view p...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese.cpp:239`

### han_reading_to_ipa `std::string ChineseRuleG2p::han_reading_to_ipa(std::string_view han) const`
- Defined: `core/moonshine-tts/src/lang-specific/chinese.cpp:400`

### char_fallback_ipa `std::string ChineseRuleG2p::char_fallback_ipa(std::string_view word) const`
- Defined: `core/moonshine-tts/src/lang-specific/chinese.cpp:425`

### g2p_word_impl `std::string ChineseRuleG2p::g2p_word_impl(std::string_view word,
                                ...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese.cpp:440`

### word_to_ipa `std::string ChineseRuleG2p::word_to_ipa(std::string_view word) const`
- Defined: `core/moonshine-tts/src/lang-specific/chinese.cpp:487`

### word_to_ipa_with_pos `std::string ChineseRuleG2p::word_to_ipa_with_pos(std::string_view word,
                         ...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese.cpp:491`

### text_to_ipa `std::string ChineseRuleG2p::text_to_ipa(std::string text,
                                       ...`
- Defined: `core/moonshine-tts/src/lang-specific/chinese.cpp:496`

### dialect_resolves_to_chinese_rules `bool dialect_resolves_to_chinese_rules(std::string_view dialect_id)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese.cpp:546`

### dialect_ids `std::vector<std::string> ChineseRuleG2p::dialect_ids()`
- Defined: `core/moonshine-tts/src/lang-specific/chinese.cpp:555`

### resolve_chinese_dict_path `std::filesystem::path resolve_chinese_dict_path(
    const std::filesystem::path& model_root)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese.cpp:560`

### resolve_chinese_onnx_model_dir `std::filesystem::path resolve_chinese_onnx_model_dir(
    const std::filesystem::path& model_root)`
- Defined: `core/moonshine-tts/src/lang-specific/chinese.cpp:565`

## core/moonshine-tts/src/lang-specific/chinese.h

### dialect_id `const std::string& dialect_id() const`
- Defined: `core/moonshine-tts/src/lang-specific/chinese.h:29`

## core/moonshine-tts/src/lang-specific/cmudict-tsv.cpp

### parse_cmudict_tsv_lines `void parse_cmudict_tsv_lines(
    std::istream& in,
    std::unordered_map<std::string, std::vect...`
- Defined: `core/moonshine-tts/src/lang-specific/cmudict-tsv.cpp:13`

### CmudictTsv `CmudictTsv::CmudictTsv(const std::filesystem::path& path)`
- Defined: `core/moonshine-tts/src/lang-specific/cmudict-tsv.cpp:57`

### CmudictTsv `CmudictTsv::CmudictTsv(std::string_view utf8_contents)`
- Defined: `core/moonshine-tts/src/lang-specific/cmudict-tsv.cpp:65`

### lookup `const std::vector<std::string>* CmudictTsv::lookup(std::string_view key) const`
- Defined: `core/moonshine-tts/src/lang-specific/cmudict-tsv.cpp:71`

## core/moonshine-tts/src/lang-specific/dutch.cpp

### dutch_unicode_tolower_cp `char32_t dutch_unicode_tolower_cp(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:30`

### append_lexicon_folded `void append_lexicon_folded(std::string& out, char32_t cl)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:102`
- Doc: Fold to ``a-z`` + hyphen for TSV keys (mirrors Python ``normalize_lexicon_key`` intent).

### normalize_lexicon_key_utf8 `std::string normalize_lexicon_key_utf8(const std::string& word)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:159`

### is_grapheme_char `bool is_grapheme_char(char32_t cl)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:177`

### normalize_grapheme_key_u32 `std::u32string normalize_grapheme_key_u32(const std::string& word)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:189`

### kTeenWord `static const char* kTeenWord(int n)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:211`

### join_unit_tens `std::string join_unit_tens(int u, std::string_view tens_word)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:220`

### below_100 `std::string below_100(int n)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:236`

### below_1000_spaced `std::string below_1000_spaced(int n)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:255`

### from_1000_to_9999 `std::string from_1000_to_9999(int n)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:277`

### fix_thousands_compound `std::string fix_thousands_compound(int q)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:309`

### below_1_000_000_v2 `std::string below_1_000_000_v2(int n)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:322`

### expand_cardinal_digits_to_dutch_words `std::string expand_cardinal_digits_to_dutch_words(std::string_view sv)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:338`

### is_ascii_digit `bool is_ascii_digit(char c)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:370`

### is_latin1_supplement_python_word_char `bool is_latin1_supplement_python_word_char(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:372`

### is_letterlike_math_word_char `bool is_letterlike_math_word_char(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:402`

### is_dutch_word_char `bool is_dutch_word_char(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:407`

### prev_utf8_index `size_t prev_utf8_index(const std::string& t, size_t byte_i)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:436`

### word_boundary_before `bool word_boundary_before(const std::string& t, size_t byte_i)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:447`

### word_boundary_after `bool word_boundary_after(const std::string& t, size_t byte_i)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:458`

### expand_digit_tokens_in_text `std::string expand_digit_tokens_in_text(std::string_view text_sv)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:468`

### digit_pass_through_pattern `bool digit_pass_through_pattern(std::string_view raw)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:519`

### all_ascii_digits_string `bool all_ascii_digits_string(const std::string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:543`

### apply_lexicon_ipa_postprocess `std::string apply_lexicon_ipa_postprocess(std::string ipa,
                                      ...`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:555`

### load_dutch_lexicon_stream `void load_dutch_lexicon_stream(
    std::istream& in, std::unordered_map<std::string, std::string...`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:623`

### load_dutch_lexicon_file `void load_dutch_lexicon_file(
    const std::filesystem::path& path,
    std::unordered_map<std::...`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:677`

### is_vowel_letter32 `bool is_vowel_letter32(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:688`

### strip_to_plain_vowel `char32_t strip_to_plain_vowel(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:698`

### word_has_written_stress_u32 `bool word_has_written_stress_u32(const std::u32string& w)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:722`

### stressed_syllable_from_acute `std::optional<size_t> stressed_syllable_from_acute(
    const std::vector<std::u32string>& syllab...`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:731`

### dutch_orthographic_syllables_u32 `std::vector<std::u32string> dutch_orthographic_syllables_u32(
    const std::u32string& word)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:792`

### remove_if `std::remove_if(syllables.begin(), syllables.end(),
                     [](const std::u32string& sy)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:851`

### unstressed_prefix_len_u32 `size_t unstressed_prefix_len_u32(const std::u32string& wl)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:856`

### default_stress_syllable_index `size_t default_stress_syllable_index(const std::vector<std::u32string>& syls,
                   ...`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:870`

### insert_primary_stress_before_vowel_dutch `std::string insert_primary_stress_before_vowel_dutch(std::string s)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:915`

### ipa_starts_with_nucleus_dutch `bool ipa_starts_with_nucleus_dutch(std::string_view rest)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:958`

### ipa_at_stress_mark_dutch `bool ipa_at_stress_mark_dutch(const std::string& ipa, size_t j)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:997`

### ipa_skip_pre_nucleus_dutch `size_t ipa_skip_pre_nucleus_dutch(std::string_view s, size_t j)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:1006`

### final_devoice_obstruents `std::string final_devoice_obstruents(std::string ipa)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:1044`

### letters_to_ipa_no_stress `std::string letters_to_ipa_no_stress(const std::u32string& syl_in,
                              ...`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:1082`

### strip_hyphens_u32 `std::u32string strip_hyphens_u32(const std::u32string& w)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:1415`

### rules_word_to_ipa_utf8 `std::string rules_word_to_ipa_utf8(const std::string& raw_word,
                                 ...`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:1425`

### resolve_dutch_dict_path `std::filesystem::path resolve_dutch_dict_path(
    const std::filesystem::path& model_root)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:1457`

### dialect_resolves_to_dutch_rules `bool dialect_resolves_to_dutch_rules(std::string_view dialect_id)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:1462`

### dialect_ids `std::vector<std::string> DutchRuleG2p::dialect_ids()`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:1470`

### normalize_ipa_stress_for_vocoder `std::string DutchRuleG2p::normalize_ipa_stress_for_vocoder(std::string ipa)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:1474`

### DutchRuleG2p `DutchRuleG2p::DutchRuleG2p(std::filesystem::path dict_tsv, Options options)
    : options_(options)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:1521`

### DutchRuleG2p `DutchRuleG2p::DutchRuleG2p(std::string dict_tsv_utf8, Options options)
    : options_(options)`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:1526`

### finalize_ipa `std::string DutchRuleG2p::finalize_ipa(std::string ipa,
                                       bo...`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:1532`

### lookup_or_rules `std::string DutchRuleG2p::lookup_or_rules(const std::string& raw_word) const`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:1545`

### word_to_ipa `std::string DutchRuleG2p::word_to_ipa(const std::string& word) const`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:1601`

### text_to_ipa_no_expand `std::string DutchRuleG2p::text_to_ipa_no_expand(
    const std::string& text, std::vector<G2pWord...`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:1622`

### text_to_ipa `std::string DutchRuleG2p::text_to_ipa(std::string text,
                                      std...`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.cpp:1698`

## core/moonshine-tts/src/lang-specific/dutch.h

### dialect_id `const std::string& dialect_id() const`
- Defined: `core/moonshine-tts/src/lang-specific/dutch.h:37`

## core/moonshine-tts/src/lang-specific/english-hand-oov.cpp

### utf8_starts_with `bool utf8_starts_with(const std::string& s, std::string_view p)`
- Defined: `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:18`

### last_utf8_char `std::string_view last_utf8_char(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:22`

### last_ipa_unit_is_vowel `bool last_ipa_unit_is_vowel(std::string_view prev)`
- Defined: `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:37`

### is_vowel `constexpr bool is_vowel(char c)`
- Defined: `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:49`

### is_consonant `constexpr bool is_consonant(char c)`
- Defined: `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:53`

### next_vowel_index `int next_vowel_index(std::string_view w, int start)`
- Defined: `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:57`

### magic_e_lengthens `bool magic_e_lengthens(std::string_view w, int vowel_i)`
- Defined: `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:66`

### th_voiced_word `bool th_voiced_word(std::string_view w)`
- Defined: `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:156`

### oov_single_consonant `std::string oov_single_consonant(char c, std::string_view w, int i)`
- Defined: `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:162`

### add_primary_stress_if_missing `std::string add_primary_stress_if_missing(std::string s)`
- Defined: `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:319`

### oov_grapheme_to_ipa `std::string oov_grapheme_to_ipa(std::string_view word)`
- Defined: `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:340`

### english_hand_oov_rules_ipa `std::string english_hand_oov_rules_ipa(std::string_view word)`
- Defined: `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp:437`

## core/moonshine-tts/src/lang-specific/english-numbers.cpp

### digit_sequence_ipa `std::string digit_sequence_ipa(std::string_view digits)`
- Defined: `core/moonshine-tts/src/lang-specific/english-numbers.cpp:21`

### under_100_ipa `std::string under_100_ipa(int n)`
- Defined: `core/moonshine-tts/src/lang-specific/english-numbers.cpp:34`

### under_1000_ipa `std::string under_1000_ipa(int n)`
- Defined: `core/moonshine-tts/src/lang-specific/english-numbers.cpp:50`

### cardinal_non_negative_ipa `std::optional<std::string> cardinal_non_negative_ipa(long long n)`
- Defined: `core/moonshine-tts/src/lang-specific/english-numbers.cpp:63`

### integer_decimal_string_ipa `std::optional<std::string> integer_decimal_string_ipa(std::string s)`
- Defined: `core/moonshine-tts/src/lang-specific/english-numbers.cpp:106`

### english_number_token_ipa `std::optional<std::string> english_number_token_ipa(std::string_view token)`
- Defined: `core/moonshine-tts/src/lang-specific/english-numbers.cpp:199`

## core/moonshine-tts/src/lang-specific/english.cpp

### append_log `void append_log(std::vector<G2pWordLog>* out, G2pWordLog entry)`
- Defined: `core/moonshine-tts/src/lang-specific/english.cpp:30`

### pick_english_heteronym_ipa `std::string pick_english_heteronym_ipa(std::vector<std::string> alts,
                           ...`
- Defined: `core/moonshine-tts/src/lang-specific/english.cpp:40`
- Doc: CMU-style heteronyms such as ``tomato`` include both US (stressed ``eɪ``) and UK (stressed ``ɑ``) readings. Lexicographi

### EnglishRuleG2p `EnglishRuleG2p::EnglishRuleG2p(
    std::filesystem::path dict_tsv,
    std::optional<std::filesy...`
- Defined: `core/moonshine-tts/src/lang-specific/english.cpp:81`

### EnglishRuleG2p `EnglishRuleG2p::EnglishRuleG2p(
    std::string dict_tsv_utf8, std::optional<std::filesystem::pat...`
- Defined: `core/moonshine-tts/src/lang-specific/english.cpp:109`

### dialect_ids `std::vector<std::string> EnglishRuleG2p::dialect_ids()`
- Defined: `core/moonshine-tts/src/lang-specific/english.cpp:139`

### text_to_ipa `std::string EnglishRuleG2p::text_to_ipa(std::string text,
                                       ...`
- Defined: `core/moonshine-tts/src/lang-specific/english.cpp:145`

### dialect_is_british_english_variant `bool dialect_is_british_english_variant(std::string_view dialect_id)`
- Defined: `core/moonshine-tts/src/lang-specific/english.cpp:238`

### dialect_resolves_to_english_rules `bool dialect_resolves_to_english_rules(std::string_view dialect_id)`
- Defined: `core/moonshine-tts/src/lang-specific/english.cpp:243`

## core/moonshine-tts/src/lang-specific/french-oov.cpp

### french_tolower_cp `char32_t french_tolower_cp(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/french-oov.cpp:16`

### is_allowed_ortho_cp `bool is_allowed_ortho_cp(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/french-oov.cpp:63`

### letters_only_u32 `std::u32string letters_only_u32(const std::string& raw)`
- Defined: `core/moonshine-tts/src/lang-specific/french-oov.cpp:74`

### v_u32 `bool v_u32(char32_t ch)`
- Defined: `core/moonshine-tts/src/lang-specific/french-oov.cpp:89`

### insert_stress_final_syllable `std::string insert_stress_final_syllable(std::string ipa)`
- Defined: `core/moonshine-tts/src/lang-specific/french-oov.cpp:119`

### prev_is_nucleus_idx `bool prev_is_nucleus_idx(const std::string& s, int idx)`
- Defined: `core/moonshine-tts/src/lang-specific/french-oov.cpp:167`

### utf8_last_cp_start `size_t utf8_last_cp_start(const std::string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/french-oov.cpp:213`

### utf8_prev_cp_start `size_t utf8_prev_cp_start(const std::string& s, size_t cp_start)`
- Defined: `core/moonshine-tts/src/lang-specific/french-oov.cpp:227`

### trim_final_by_orthography `std::string trim_final_by_orthography(std::string ipa,
                                      cons...`
- Defined: `core/moonshine-tts/src/lang-specific/french-oov.cpp:241`

### peek_eq `bool peek_eq(const std::u32string& w, size_t i, const char* ascii)`
- Defined: `core/moonshine-tts/src/lang-specific/french-oov.cpp:314`

### scan_graphemes `std::string scan_graphemes(const std::u32string& w)`
- Defined: `core/moonshine-tts/src/lang-specific/french-oov.cpp:327`

### oov_word_to_ipa `std::string oov_word_to_ipa(const std::string& word, bool with_stress)`
- Defined: `core/moonshine-tts/src/lang-specific/french-oov.cpp:689`

## core/moonshine-tts/src/lang-specific/french.cpp

### french_tolower_cp `char32_t french_tolower_cp(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:29`

### is_french_key_cp `bool is_french_key_cp(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:82`

### normalize_lookup_key_utf8 `std::string normalize_lookup_key_utf8(const std::string& word)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:93`

### is_latin1_supplement_python_word_char `bool is_latin1_supplement_python_word_char(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:112`
- Doc: Python ``re.UNICODE`` word chars in U+00AA..U+00FF (excludes × U+00D7 and ÷ U+00F7).

### is_letterlike_math_word_char `bool is_letterlike_math_word_char(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:143`

### is_french_word_char `bool is_french_word_char(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:148`

### to_lower_ascii `std::string to_lower_ascii(std::string_view w)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:176`

### to_lower_pos_inventory_utf8 `std::string to_lower_pos_inventory_utf8(const std::string& word)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:184`

### load_french_lexicon_stream `void load_french_lexicon_stream(
    std::istream& in, std::unordered_map<std::string, std::strin...`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:197`

### load_french_lexicon_file `void load_french_lexicon_file(
    const std::filesystem::path& path,
    std::unordered_map<std:...`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:229`

### parse_first_csv_field `std::string parse_first_csv_field(std::string_view line)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:240`

### load_french_pos_csv_stream `void load_french_pos_csv_stream(
    std::istream& in, const std::string& cat_upper,
    std::uno...`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:269`

### load_french_pos_dir `void load_french_pos_dir(
    const std::filesystem::path& dir,
    std::unordered_map<std::strin...`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:293`

### load_french_pos_from_csv_utf8_map `void load_french_pos_from_csv_utf8_map(
    const std::unordered_map<std::string, std::string>& c...`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:323`

### sort `std::sort(sorted.begin(), sorted.end(),
            [](const auto& a, const auto& b)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:333`

### below_100 `std::vector<std::string> below_100(int n)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:349`

### below_1000 `std::vector<std::string> below_1000(int n)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:412`

### below_1_000_000 `std::vector<std::string> below_1_000_000(int n)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:446`

### join_space `std::string join_space(const std::vector<std::string>& v)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:470`

### is_all_ascii_digits `bool is_all_ascii_digits(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:481`

### expand_cardinal_digits_to_french_words `std::string expand_cardinal_digits_to_french_words(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:493`

### expand_digit_tokens_in_text `std::string expand_digit_tokens_in_text(const std::string& text)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:517`

### h_aspire_set `const std::unordered_set<std::string>& h_aspire_set()`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:540`

### closed_liaison_determiners `const std::unordered_set<std::string>& closed_liaison_determiners()`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:551`

### pos_scan_order `const std::vector<std::string>& pos_scan_order()`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:558`

### categories_for_form `std::vector<std::string> categories_for_form(
    const std::string& word,
    const std::unorder...`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:564`

### classify_pos `std::optional<std::string> classify_pos(
    const std::string& word,
    const std::unordered_ma...`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:582`

### strip_stress `std::string strip_stress(std::string_view ipa)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:622`

### french_nucleus_prefixes `const std::vector<std::string>& french_nucleus_prefixes()`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:643`
- Doc: Longest-first nucleus prefixes (UTF-8 byte strings).

### replace_suffix_once `std::string replace_suffix_once(std::string ipa, std::string_view old_s,
                        ...`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:671`

### nasal_liaison_transform `std::optional<std::string> nasal_liaison_transform(const std::string& word,
                     ...`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:681`

### ortho_for_liaison `std::string ortho_for_liaison(std::string_view word)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:702`

### utf8_last_cp `bool utf8_last_cp(const std::string& s, char32_t& out_cp)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:722`

### orthographic_liaison_consonant `std::optional<std::string> orthographic_liaison_consonant(
    std::string_view word)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:738`

### ipa_starts_with_vowel_sound `bool ipa_starts_with_vowel_sound(std::string_view ipa_sv)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:766`

### ipa_ends_with_audible_consonant `bool ipa_ends_with_audible_consonant(std::string_view ipa_sv)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:849`

### liaison_strength_fn `LiaisonStrength liaison_strength_fn(const std::optional<std::string>& pos_left,
                 ...`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:922`

### lookup_lexicon `std::optional<std::string> lookup_lexicon(
    const std::unordered_map<std::string, std::string>...`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:1015`

### count_primary_stress_marks `size_t count_primary_stress_marks(const std::string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:1038`

### ensure_french_nuclear_stress `std::string FrenchRuleG2p::ensure_french_nuclear_stress(std::string ipa)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:1050`

### FrenchRuleG2p `FrenchRuleG2p::FrenchRuleG2p(std::filesystem::path dict_tsv,
                             std::fi...`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:1090`

### FrenchRuleG2p `FrenchRuleG2p::FrenchRuleG2p(std::string dict_tsv_utf8,
                             std::filesys...`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:1097`

### finalize_word_ipa `std::string FrenchRuleG2p::finalize_word_ipa(std::string ipa,
                                   ...`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:1115`

### word_to_ipa_impl `std::string FrenchRuleG2p::word_to_ipa_impl(const std::string& raw_word,
                        ...`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:1126`

### word_to_ipa `std::string FrenchRuleG2p::word_to_ipa(const std::string& word) const`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:1170`

### text_to_ipa `std::string FrenchRuleG2p::text_to_ipa(std::string text,
                                       s...`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:1174`

### text_to_ipa_impl `std::string FrenchRuleG2p::text_to_ipa_impl(
    const std::string& text, bool expand_digits,
   ...`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:1179`

### all_of `std::all_of(t.s.begin(), t.s.end(), [](unsigned char c)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:1328`

### dialect_resolves_to_french_rules `bool dialect_resolves_to_french_rules(std::string_view dialect_id)`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:1360`

### dialect_ids `std::vector<std::string> FrenchRuleG2p::dialect_ids()`
- Defined: `core/moonshine-tts/src/lang-specific/french.cpp:1368`

## core/moonshine-tts/src/lang-specific/french.h

### dialect_id `const std::string& dialect_id() const`
- Defined: `core/moonshine-tts/src/lang-specific/french.h:50`

## core/moonshine-tts/src/lang-specific/german.cpp

### german_tolower_cp `char32_t german_tolower_cp(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:29`

### is_key_char `bool is_key_char(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:46`

### normalize_lookup_key_utf8 `std::string normalize_lookup_key_utf8(const std::string& word)`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:56`
- Doc: NFC-style key: lowercase letters + umlauts + ß only (Python ``normalize_lookup_key``).

### is_german_word_char `bool is_german_word_char(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:71`

### is_vowel_l `bool is_vowel_l(char32_t ch)`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:103`

### char_before_for_ch `std::optional<char32_t> char_before_for_ch(const std::u32string& s, size_t i)`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:120`

### ch_ipa_utf8 `std::string ch_ipa_utf8(const std::u32string& full_word_nh, size_t i)`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:143`

### final_devoice `std::string final_devoice(std::string ipa)`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:161`

### st_sp_at_morpheme_start `bool st_sp_at_morpheme_start(const std::u32string& hyphen_word,
                             size...`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:186`

### unstressed_prefix_len_u32 `size_t unstressed_prefix_len_u32(const std::u32string& w)`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:210`

### strip_hyphens_u32 `std::u32string strip_hyphens_u32(const std::u32string& w)`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:224`

### german_orthographic_syllables_u32 `std::vector<std::u32string> german_orthographic_syllables_u32(
    const std::u32string& word_lower)`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:280`

### default_stress_syllable_index `size_t default_stress_syllable_index(const std::vector<std::u32string>& syls,
                   ...`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:338`

### insert_primary_stress_before_vowel_utf8 `std::string insert_primary_stress_before_vowel_utf8(std::string s)`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:369`

### ipa_starts_with_nucleus `bool ipa_starts_with_nucleus(std::string_view rest)`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:388`

### ipa_skip_pre_nucleus `size_t ipa_skip_pre_nucleus(std::string_view s, size_t j)`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:403`

### letters_to_ipa_no_stress `std::string letters_to_ipa_no_stress(const std::u32string& syl_lower,
                           ...`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:437`

### rules_word_to_ipa_utf8 `std::string rules_word_to_ipa_utf8(const std::string& raw_word,
                                 ...`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:718`

### load_german_lexicon_stream `void load_german_lexicon_stream(
    std::istream& in, std::unordered_map<std::string, std::strin...`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:753`

### load_german_lexicon_file `void load_german_lexicon_file(
    const std::filesystem::path& path,
    std::unordered_map<std:...`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:809`

### g2p_all_ascii_digits `bool g2p_all_ascii_digits(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:824`

### german_under_100_word `std::string german_under_100_word(int n)`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:836`

### german_hundred_head `std::string german_hundred_head(int h)`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:867`

### append_german_tokens_1_999 `void append_german_tokens_1_999(int n, std::vector<std::string>& out)`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:879`

### append_german_tokens_thousands `void append_german_tokens_thousands(int q, std::vector<std::string>& out)`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:895`

### append_german_below_1_000_000 `void append_german_below_1_000_000(int n, std::vector<std::string>& out)`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:907`

### expand_cardinal_digits_to_german_words `std::string expand_cardinal_digits_to_german_words(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:923`

### expand_german_digit_tokens_in_text `std::string expand_german_digit_tokens_in_text(std::string text)`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:961`

### ipa_at_stress_mark `bool ipa_at_stress_mark(const std::string& ipa, size_t j)`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:1011`

### normalize_ipa_stress_for_vocoder `std::string GermanRuleG2p::normalize_ipa_stress_for_vocoder(std::string ipa)`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:1020`

### GermanRuleG2p `GermanRuleG2p::GermanRuleG2p(std::filesystem::path dict_tsv, Options options)
    : options_(opti...`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:1067`

### GermanRuleG2p `GermanRuleG2p::GermanRuleG2p(std::string dict_tsv_utf8, Options options)
    : options_(options)`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:1072`

### finalize_ipa `std::string GermanRuleG2p::finalize_ipa(std::string ipa) const`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:1078`

### lookup_or_rules `std::string GermanRuleG2p::lookup_or_rules(const std::string& raw_word) const`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:1090`

### word_to_ipa `std::string GermanRuleG2p::word_to_ipa(const std::string& word) const`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:1156`

### text_to_ipa_no_expand `std::string GermanRuleG2p::text_to_ipa_no_expand(
    const std::string& text, std::vector<G2pWor...`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:1178`

### text_to_ipa `std::string GermanRuleG2p::text_to_ipa(std::string text,
                                       s...`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:1254`

### dialect_resolves_to_german_rules `bool dialect_resolves_to_german_rules(std::string_view dialect_id)`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:1262`

### dialect_ids `std::vector<std::string> GermanRuleG2p::dialect_ids()`
- Defined: `core/moonshine-tts/src/lang-specific/german.cpp:1270`

## core/moonshine-tts/src/lang-specific/german.h

### dialect_id `const std::string& dialect_id() const`
- Defined: `core/moonshine-tts/src/lang-specific/german.h:39`

## core/moonshine-tts/src/lang-specific/heteronym-context.cpp

### join_cells `std::string join_cells(const std::vector<std::string>& cells)`
- Defined: `core/moonshine-tts/src/lang-specific/heteronym-context.cpp:11`

## core/moonshine-tts/src/lang-specific/hindi-numbers.cpp

### append_join `void append_join(std::vector<std::string>& out,
                 const std::vector<std::string>& ...`
- Defined: `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp:42`

### under_100 `std::vector<std::string> under_100(int n)`
- Defined: `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp:49`

### tokens_0_999 `std::vector<std::string> tokens_0_999(int n)`
- Defined: `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp:67`

### below_1_000_000_tokens `std::vector<std::string> below_1_000_000_tokens(int n)`
- Defined: `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp:92`

### join_space `std::string join_space(const std::vector<std::string>& v)`
- Defined: `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp:119`

### all_ascii_digits `bool all_ascii_digits(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp:130`

### expand_cardinal_digits_to_hindi_words `std::string expand_cardinal_digits_to_hindi_words(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp:144`

### expand_hindi_digit_tokens_in_text `std::string expand_hindi_digit_tokens_in_text(std::string text)`
- Defined: `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp:168`

### expand_devanagari_digit_runs_in_text `std::string expand_devanagari_digit_runs_in_text(std::string text)`
- Defined: `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp:201`

## core/moonshine-tts/src/lang-specific/hindi.cpp

### utf8_nfc_utf8proc `std::string utf8_nfc_utf8proc(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.cpp:32`

### is_devanagari_digit `bool is_devanagari_digit(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.cpp:94`

### is_consonant `bool is_consonant(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.cpp:96`

### cons_ipa `std::string cons_ipa(char32_t base, bool nukta)`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.cpp:100`

### sv_starts_with `bool sv_starts_with(std::string_view s, std::string_view p)`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.cpp:111`

### nasal_for_place `std::string nasal_for_place(std::string_view first_onset)`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.cpp:115`

### syllable_weight `int syllable_weight(const Syllable& s)`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.cpp:154`

### assign_stress `std::string assign_stress(const std::vector<std::string>& ipa_syllables,
                        ...`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.cpp:166`

### apply_schwa_syncope `void apply_schwa_syncope(std::vector<Syllable>& syls)`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.cpp:200`

### parse_devanagari_to_syllables `std::optional<std::vector<Syllable>> parse_devanagari_to_syllables(
    const std::string& word)`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.cpp:226`

### render_syllables `std::string render_syllables(const std::vector<Syllable>& syls,
                             bool...`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.cpp:357`

### strip_edges_punct `void strip_edges_punct(std::string_view w, std::string& core)`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.cpp:423`

### has_devanagari `bool has_devanagari(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.cpp:447`

### all_ascii_digits_sv `bool all_ascii_digits_sv(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.cpp:457`

### builtin_hindi_dict_path `std::filesystem::path builtin_hindi_dict_path()`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.cpp:471`

### load_hindi_lexicon_stream `void load_hindi_lexicon_stream(
    std::istream& in, std::unordered_map<std::string, std::string...`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.cpp:478`

### HindiRuleG2p `HindiRuleG2p::HindiRuleG2p(std::filesystem::path dict_tsv, Options options)
    : options_(options)`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.cpp:506`

### HindiRuleG2p `HindiRuleG2p::HindiRuleG2p(std::string dict_tsv_utf8, Options options)
    : options_(options)`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.cpp:520`

### word_to_ipa `std::string HindiRuleG2p::word_to_ipa(const std::string& word) const`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.cpp:526`

### g2p_single_word `std::string HindiRuleG2p::g2p_single_word(std::string_view word) const`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.cpp:530`

### text_to_ipa_no_expand `std::string HindiRuleG2p::text_to_ipa_no_expand(
    std::string text, std::vector<G2pWordLog>* p...`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.cpp:550`

### text_to_ipa `std::string HindiRuleG2p::text_to_ipa(std::string text,
                                      std...`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.cpp:593`

### dialect_ids `std::vector<std::string> HindiRuleG2p::dialect_ids()`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.cpp:602`

### dialect_resolves_to_hindi_rules `bool dialect_resolves_to_hindi_rules(std::string_view dialect_id)`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.cpp:606`

### resolve_hindi_dict_path `std::filesystem::path resolve_hindi_dict_path(
    const std::filesystem::path& model_root)`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.cpp:614`

### hindi_text_to_ipa `std::string hindi_text_to_ipa(const std::string& text, bool with_stress,
                        ...`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.cpp:619`

## core/moonshine-tts/src/lang-specific/hindi.h

### dialect_id `const std::string& dialect_id() const`
- Defined: `core/moonshine-tts/src/lang-specific/hindi.h:33`

## core/moonshine-tts/src/lang-specific/italian.cpp

### italian_tolower_cp `char32_t italian_tolower_cp(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:34`

### is_italian_lexicon_key_cp `bool is_italian_lexicon_key_cp(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:69`

### normalize_lookup_key_utf8 `std::string normalize_lookup_key_utf8(const std::string& word)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:84`

### utf8_lowercase_italian `std::string utf8_lowercase_italian(const std::string& word)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:103`

### load_italian_lexicon_stream `void load_italian_lexicon_stream(
    std::istream& in, std::unordered_map<std::string, std::stri...`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:116`

### load_italian_lexicon_file `void load_italian_lexicon_file(
    const std::filesystem::path& path,
    std::unordered_map<std...`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:148`

### is_all_ascii_digits `bool is_all_ascii_digits(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:161`
- Doc: -- Italian numbers (italian_numbers.py) ---------------------------------

### under_100 `std::string under_100(int n)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:177`

### hundred_head `std::string hundred_head(int h)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:234`

### append_tokens_0_999 `void append_tokens_0_999(int n, std::vector<std::string>& out)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:246`

### spell_1_999_fused `std::string spell_1_999_fused(int n)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:273`

### append_thousands_multiplier `void append_thousands_multiplier(int q, std::vector<std::string>& out)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:295`

### below_1_000_000_tokens `void below_1_000_000_tokens(int n, std::vector<std::string>& out)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:313`

### expand_cardinal_digits_to_italian_words `std::string expand_cardinal_digits_to_italian_words(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:329`

### expand_digit_tokens_in_text `std::string expand_digit_tokens_in_text(std::string text)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:365`

### utf8_to_u32 `std::u32string utf8_to_u32(const std::string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:400`
- Doc: -- Rules (UTF-32 syllable pass) -----------------------------------------

### u32_to_utf8 `std::string u32_to_utf8(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:413`

### is_vowel_ch `bool is_vowel_ch(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:421`

### strip_accent_letter `char32_t strip_accent_letter(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:428`

### should_hiatus_it `bool should_hiatus_it(char32_t a, char32_t b)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:453`

### vowel_nucleus_spans `void vowel_nucleus_spans(const std::u32string& w,
                         std::vector<std::pair<...`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:483`

### valid_onset2 `bool valid_onset2(char a, char b)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:508`

### split_intervocalic_cluster `void split_intervocalic_cluster(const std::string& cluster, std::string& coda,
                  ...`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:522`

### italian_orthographic_syllables_u32 `std::vector<std::u32string> italian_orthographic_syllables_u32(
    std::u32string w)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:543`

### accented_vowel_in_u32 `bool accented_vowel_in_u32(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:617`

### default_stressed_syllable_index `size_t default_stressed_syllable_index(const std::vector<std::u32string>& syls,
                 ...`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:623`

### insert_primary_stress_before_vowel `std::string insert_primary_stress_before_vowel(std::string ipa)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:665`

### next_is_vowel_u32 `bool next_is_vowel_u32(const std::u32string& s, size_t j)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:692`

### ei_e_accent `bool ei_e_accent(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:704`

### italian_cg_palatal_letter `bool italian_cg_palatal_letter(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:712`
- Doc: After c/g (and related digraphs): letters that palatalize, matching Python ``in "eiéè"`` (the character set is e, i, é, 

### letters_to_ipa_no_stress `std::string letters_to_ipa_no_stress(const std::u32string& su)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:717`

### rules_word_to_ipa_utf8 `std::string rules_word_to_ipa_utf8(const std::string& raw, bool with_stress)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:979`

### is_italian_word_char `bool is_italian_word_char(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:1067`

### try_consume_italian_word `bool try_consume_italian_word(const std::string& text, size_t pos,
                              ...`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:1101`

### ItalianRuleG2p `ItalianRuleG2p::ItalianRuleG2p(std::filesystem::path dict_tsv, Options options)
    : options_(op...`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:1157`

### ItalianRuleG2p `ItalianRuleG2p::ItalianRuleG2p(std::string dict_tsv_utf8, Options options)
    : options_(options)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:1162`

### finalize_ipa `std::string ItalianRuleG2p::finalize_ipa(std::string ipa,
                                       ...`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:1168`

### lookup_or_rules `std::string ItalianRuleG2p::lookup_or_rules(const std::string& raw_word) const`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:1181`

### word_to_ipa `std::string ItalianRuleG2p::word_to_ipa(const std::string& word) const`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:1230`

### text_to_ipa_no_expand `std::string ItalianRuleG2p::text_to_ipa_no_expand(
    const std::string& text, std::vector<G2pWo...`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:1252`

### text_to_ipa `std::string ItalianRuleG2p::text_to_ipa(std::string text,
                                       ...`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:1322`

### dialect_resolves_to_italian_rules `bool dialect_resolves_to_italian_rules(std::string_view dialect_id)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:1330`

### dialect_ids `std::vector<std::string> ItalianRuleG2p::dialect_ids()`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:1338`

### resolve_italian_dict_path `std::filesystem::path resolve_italian_dict_path(
    const std::filesystem::path& model_root)`
- Defined: `core/moonshine-tts/src/lang-specific/italian.cpp:1342`

## core/moonshine-tts/src/lang-specific/italian.h

### dialect_id `const std::string& dialect_id() const`
- Defined: `core/moonshine-tts/src/lang-specific/italian.h:37`

## core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp

### utf8_nfkc_utf8proc `std::string utf8_nfkc_utf8proc(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp:18`

### katakana_to_hiragana_u32 `std::u32string katakana_to_hiragana_u32(const std::u32string& in)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp:30`

### u32_to_utf8 `std::string u32_to_utf8(const std::u32string& u)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp:50`

### utf8_starts_with_at `bool utf8_starts_with_at(const std::string& s, std::size_t off,
                         const st...`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp:58`

### long_mark_extend_last `void long_mark_extend_last(std::vector<std::string>& parts)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp:66`

### geminate_onset `std::string geminate_onset(const std::string& onset,
                           const std::string...`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp:151`

### katakana_hiragana_to_ipa `std::string katakana_hiragana_to_ipa(std::string_view sv)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp:162`

### japanese_is_kana_only `bool japanese_is_kana_only(std::string_view sv)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp:225`

### japanese_has_japanese_script `bool japanese_has_japanese_script(std::string_view sv)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp:254`

## core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp

### utf8_nfc_utf8proc `std::string utf8_nfc_utf8proc(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:21`

### is_han_cp `bool is_han_cp(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:33`

### is_single_han `bool is_single_han(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:39`

### only_hiragana `bool only_hiragana(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:44`

### only_katakana `bool only_katakana(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:57`

### only_han `bool only_han(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:73`

### trailing_particles_sorted `const std::vector<std::string>& trailing_particles_sorted()`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:175`

### sort `std::sort(v.begin(), v.end(),
              [](const std::string& a, const std::string& b)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:183`

### build_by_first `void build_by_first(
    const std::unordered_map<std::string, std::string>& lex,
    std::unorde...`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:227`

### sort `std::sort(vec.begin(), vec.end(),
              [](const std::string& a, const std::string& b)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:246`

### default_japanese_dict_path `std::filesystem::path default_japanese_dict_path(
    const std::filesystem::path& g2p_data_root)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:254`

### JapaneseOnnxG2p `JapaneseOnnxG2p::JapaneseOnnxG2p(std::filesystem::path model_dir,
                               ...`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:259`

### JapaneseOnnxG2p `JapaneseOnnxG2p::JapaneseOnnxG2p(std::filesystem::path model_dir,
                               ...`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:266`

### JapaneseOnnxG2p `JapaneseOnnxG2p::JapaneseOnnxG2p(const MoonshineG2POptions& opt,
                                ...`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:274`

### JapaneseOnnxG2p `JapaneseOnnxG2p::JapaneseOnnxG2p(const MoonshineG2POptions& opt,
                                ...`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:282`

### g2p_word `std::string JapaneseOnnxG2p::g2p_word(std::string word_utf8)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:291`

### text_to_ipa `std::string JapaneseOnnxG2p::text_to_ipa(std::string text_utf8)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp:356`

## core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.h

### tok `const JapaneseTokPosOnnx& tok() const`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.h:33`

## core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp

### open_session `std::unique_ptr<Ort::Session> open_session(
    Ort::Env& env, const std::filesystem::path& model...`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:30`

### open_session_memory `std::unique_ptr<Ort::Session> open_session_memory(
    Ort::Env& env, const void* data, size_t le...`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:47`

### slurp_utf8_file `std::string slurp_utf8_file(const std::filesystem::path& p)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:61`

### bundle_load_utf8 `bool bundle_load_utf8(const MoonshineG2POptions* opt,
                      std::string_view bund...`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:71`

### bundle_load_binary `bool bundle_load_binary(const MoonshineG2POptions* opt,
                        std::string_view ...`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:89`

### utf8_to_u32 `std::u32string utf8_to_u32(std::string_view utf8)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:122`

### u32_to_utf8 `std::string u32_to_utf8(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:135`

### is_space_u32 `bool is_space_u32(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:143`

### is_control_u32 `bool is_control_u32(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:152`

### is_punctuation_u32 `bool is_punctuation_u32(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:161`

### is_punct_char_word_group_u32 `bool is_punct_char_word_group_u32(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:175`
- Doc: ``token_word_group_indices`` uses :func:`_is_punct_char` (Unicode **P** categories only), not the broader BERT ``_is_pun

### is_chinese_char `bool is_chinese_char(std::uint32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:179`

### u32_nfc `std::u32string u32_nfc(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:188`

### strip_mn_nfd `std::u32string strip_mn_nfd(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:200`

### to_lower_u32 `std::u32string to_lower_u32(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:220`

### clean_text_u32 `std::u32string clean_text_u32(const std::u32string& text)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:229`

### tokenize_chinese_chars_u32 `std::u32string tokenize_chinese_chars_u32(const std::u32string& text)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:241`

### split_u32_whitespace `std::vector<std::u32string> split_u32_whitespace(std::u32string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:255`

### run_split_on_punc_u32 `std::vector<std::u32string> run_split_on_punc_u32(const std::u32string& text)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:280`

### normalization_ref_u32 `std::u32string normalization_ref_u32(const std::u32string& text_u32,
                            ...`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:316`

### basic_tokenize_u32 `std::vector<std::u32string> basic_tokenize_u32(
    const std::u32string& original_text_u32, cons...`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:325`

### align_basic_tokens_u32 `void align_basic_tokens_u32(const std::u32string& ref,
                            const std::vec...`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:357`

### wordpiece_tokenize_u32 `std::vector<std::u32string> wordpiece_tokenize_u32(
    const std::u32string& token,
    const st...`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:374`

### encode_bert_wordpiece `EncodedWp encode_bert_wordpiece(
    const std::u32string& text_u32,
    const std::unordered_map...`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:429`

### ud_upos_set `const std::unordered_set<std::string>& ud_upos_set()`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:597`

### morph_label_to_upos `std::string morph_label_to_upos(std::string label)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:605`

### cjk_tokpos_preferred_chunk_break_cp `bool cjk_tokpos_preferred_chunk_break_cp(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:649`

### cjk_tokpos_chunk_exclusive_end `template <typename EncodeFn>
std::size_t cjk_tokpos_chunk_exclusive_end(const std::u32string& ful...`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:682`

### default_japanese_tok_pos_model_dir `std::filesystem::path default_japanese_tok_pos_model_dir(
    const std::filesystem::path& g2p_da...`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:721`

### JapaneseTokPosOnnx `JapaneseTokPosOnnx::JapaneseTokPosOnnx(const MoonshineG2POptions* opt,
                          ...`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:731`

### format_annotated_line `std::string JapaneseTokPosOnnx::format_annotated_line(
    const std::vector<std::pair<std::strin...`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp:792`

## core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.h

### model_dir `const std::filesystem::path& model_dir() const`
- Defined: `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.h:41`

## core/moonshine-tts/src/lang-specific/japanese.cpp

### absolute_model_root `std::filesystem::path absolute_model_root(
    const std::filesystem::path& model_root)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese.cpp:15`

### JapaneseRuleG2p `JapaneseRuleG2p::JapaneseRuleG2p(std::filesystem::path onnx_model_dir,
                          ...`
- Defined: `core/moonshine-tts/src/lang-specific/japanese.cpp:31`

### JapaneseRuleG2p `JapaneseRuleG2p::JapaneseRuleG2p(std::filesystem::path onnx_model_dir,
                          ...`
- Defined: `core/moonshine-tts/src/lang-specific/japanese.cpp:36`

### JapaneseRuleG2p `JapaneseRuleG2p::JapaneseRuleG2p(const MoonshineG2POptions& opt,
                                ...`
- Defined: `core/moonshine-tts/src/lang-specific/japanese.cpp:41`

### JapaneseRuleG2p `JapaneseRuleG2p::JapaneseRuleG2p(const MoonshineG2POptions& opt,
                                ...`
- Defined: `core/moonshine-tts/src/lang-specific/japanese.cpp:47`

### text_to_ipa `std::string JapaneseRuleG2p::text_to_ipa(
    std::string text, std::vector<G2pWordLog>* per_word...`
- Defined: `core/moonshine-tts/src/lang-specific/japanese.cpp:60`

### dialect_ids `std::vector<std::string> JapaneseRuleG2p::dialect_ids()`
- Defined: `core/moonshine-tts/src/lang-specific/japanese.cpp:66`

### dialect_resolves_to_japanese_rules `bool dialect_resolves_to_japanese_rules(std::string_view dialect_id)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese.cpp:71`

### resolve_japanese_dict_path `std::filesystem::path resolve_japanese_dict_path(
    const std::filesystem::path& model_root)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese.cpp:79`

### resolve_japanese_onnx_model_dir `std::filesystem::path resolve_japanese_onnx_model_dir(
    const std::filesystem::path& model_root)`
- Defined: `core/moonshine-tts/src/lang-specific/japanese.cpp:85`

## core/moonshine-tts/src/lang-specific/japanese.h

### dialect_id `const std::string& dialect_id() const`
- Defined: `core/moonshine-tts/src/lang-specific/japanese.h:42`

## core/moonshine-tts/src/lang-specific/korean-numbers.cpp

### is_ascii_digit `bool is_ascii_digit(char c)`
- Defined: `core/moonshine-tts/src/lang-specific/korean-numbers.cpp:20`

### thousands_lookahead_ok `bool thousands_lookahead_ok(std::string_view suf)`
- Defined: `core/moonshine-tts/src/lang-specific/korean-numbers.cpp:22`

### strip_thousands_commas `std::string strip_thousands_commas(std::string_view raw)`
- Defined: `core/moonshine-tts/src/lang-specific/korean-numbers.cpp:38`

### normalize_numeral_token_string `std::string normalize_numeral_token_string(std::string_view raw)`
- Defined: `core/moonshine-tts/src/lang-specific/korean-numbers.cpp:51`

### hangul_digits_only `std::string hangul_digits_only(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/korean-numbers.cpp:65`

### section_under_10000 `std::string section_under_10000(unsigned n)`
- Defined: `core/moonshine-tts/src/lang-specific/korean-numbers.cpp:75`

### parse_uint_strict `bool parse_uint_strict(std::string_view sv, std::uint64_t& out)`
- Defined: `core/moonshine-tts/src/lang-specific/korean-numbers.cpp:123`

### int_to_sino_korean_hangul `std::string int_to_sino_korean_hangul(std::uint64_t n)`
- Defined: `core/moonshine-tts/src/lang-specific/korean-numbers.cpp:146`

### korean_reading_fragments_from_ascii_numeral_token `std::optional<std::vector<std::string>>
korean_reading_fragments_from_ascii_numeral_token(std::st...`
- Defined: `core/moonshine-tts/src/lang-specific/korean-numbers.cpp:187`

### is_ascii_numeral_token `bool is_ascii_numeral_token(std::string_view token)`
- Defined: `core/moonshine-tts/src/lang-specific/korean-numbers.cpp:286`

## core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp

### open_session `std::unique_ptr<Ort::Session> open_session(
    Ort::Env& env, const std::filesystem::path& model...`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:30`

### open_session_memory `std::unique_ptr<Ort::Session> open_session_memory(
    Ort::Env& env, const void* data, size_t le...`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:47`

### slurp_utf8_file `std::string slurp_utf8_file(const std::filesystem::path& p)`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:61`

### bundle_load_utf8 `bool bundle_load_utf8(const MoonshineG2POptions* opt,
                      std::string_view bund...`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:71`

### bundle_load_binary `bool bundle_load_binary(const MoonshineG2POptions* opt,
                        std::string_view ...`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:89`

### utf8_to_u32 `std::u32string utf8_to_u32(std::string_view utf8)`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:122`

### u32_to_utf8 `std::string u32_to_utf8(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:135`

### is_space_u32 `bool is_space_u32(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:143`

### is_control_u32 `bool is_control_u32(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:152`

### is_punctuation_u32 `bool is_punctuation_u32(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:161`

### is_punct_char_word_group_u32 `bool is_punct_char_word_group_u32(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:175`
- Doc: ``token_word_group_indices`` uses :func:`_is_punct_char` (Unicode **P** categories only), not the broader BERT ``_is_pun

### is_chinese_char `bool is_chinese_char(std::uint32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:179`

### u32_nfc `std::u32string u32_nfc(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:188`

### strip_mn_nfd `std::u32string strip_mn_nfd(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:200`

### to_lower_u32 `std::u32string to_lower_u32(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:220`

### clean_text_u32 `std::u32string clean_text_u32(const std::u32string& text)`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:229`

### tokenize_chinese_chars_u32 `std::u32string tokenize_chinese_chars_u32(const std::u32string& text)`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:241`

### split_u32_whitespace `std::vector<std::u32string> split_u32_whitespace(std::u32string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:255`

### run_split_on_punc_u32 `std::vector<std::u32string> run_split_on_punc_u32(const std::u32string& text)`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:280`

### normalization_ref_u32 `std::u32string normalization_ref_u32(const std::u32string& text_u32,
                            ...`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:316`

### basic_tokenize_u32 `std::vector<std::u32string> basic_tokenize_u32(
    const std::u32string& original_text_u32, cons...`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:325`

### align_basic_tokens_u32 `void align_basic_tokens_u32(const std::u32string& ref,
                            const std::vec...`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:357`

### wordpiece_tokenize_u32 `std::vector<std::u32string> wordpiece_tokenize_u32(
    const std::u32string& token,
    const st...`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:374`

### encode_bert_wordpiece `EncodedWp encode_bert_wordpiece(
    const std::u32string& text_u32,
    const std::unordered_map...`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:429`

### ud_upos_set `const std::unordered_set<std::string>& ud_upos_set()`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:597`

### morph_label_to_upos `std::string morph_label_to_upos(std::string label)`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:605`

### cjk_tokpos_preferred_chunk_break_cp `bool cjk_tokpos_preferred_chunk_break_cp(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:649`

### cjk_tokpos_chunk_exclusive_end `template <typename EncodeFn>
std::size_t cjk_tokpos_chunk_exclusive_end(const std::u32string& ful...`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:682`

### default_korean_tok_pos_model_dir `std::filesystem::path default_korean_tok_pos_model_dir(
    const std::filesystem::path& g2p_data...`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:721`

### KoreanTokPosOnnx `KoreanTokPosOnnx::KoreanTokPosOnnx(const MoonshineG2POptions* opt,
                              ...`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:731`

### format_annotated_line `std::string KoreanTokPosOnnx::format_annotated_line(
    const std::vector<std::pair<std::string,...`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp:791`

## core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.h

### model_dir `const std::filesystem::path& model_dir() const`
- Defined: `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.h:41`

## core/moonshine-tts/src/lang-specific/korean.cpp

### replace_all `void replace_all(std::string& s, const std::string& from,
                 const std::string& to)`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:60`

### utf8_nfc_utf8proc `std::string utf8_nfc_utf8proc(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:71`

### strip_mn_after_nfd `std::string strip_mn_after_nfd(const std::string& ipa)`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:83`

### is_sonorant_jong `bool is_sonorant_jong(int jong)`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:175`
- Doc: Sonorant codas: nasals (ㄴ,ㅁ,ŋ) and liquids (ㄹ and ㄹ-clusters). After these, lenis ㅈ voices to dʑ (same as after vowels).

### jong_triggers_tense `bool jong_triggers_tense(int jong)`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:182`

### tense_cho `int tense_cho(int plain_cho)`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:203`

### decompose_syllable_cp `std::optional<Syllable> decompose_syllable_cp(char32_t ch)`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:220`

### text_to_syllables `std::vector<Syllable> text_to_syllables(std::string_view text)`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:232`

### apply_linking `void apply_linking(std::vector<Syllable>& syls)`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:248`

### apply_lateralization `void apply_lateralization(std::vector<Syllable>& syls)`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:276`

### ipa_onset `std::string ipa_onset(int cho, bool tense, bool aspirate)`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:290`

### ipa_nucleus `std::string ipa_nucleus(int jung)`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:375`

### ipa_coda_simple `std::string ipa_coda_simple(int jong)`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:388`

### coda_nasal_assimilate `std::string coda_nasal_assimilate(int jong, std::optional<int> next_cho)`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:424`

### syllables_to_ipa `std::string syllables_to_ipa(const std::vector<Syllable>& syls,
                             std:...`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:446`

### sino_cardinal_speech_units `std::vector<std::string> sino_cardinal_speech_units(std::uint64_t n)`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:550`
- Doc: Split n into natural Korean speech units for TTS (千/百/나머지 boundaries). e.g. 1986 → ["천","구백","팔십육"],  2002 → ["이천","이"],

### g2p_hangul_rules_only_inner `std::string g2p_hangul_rules_only_inner(std::string_view hangul,
                                ...`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:577`

### normalize_korean_ipa `std::string KoreanRuleG2p::normalize_korean_ipa(std::string ipa,
                                ...`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:593`

### extract_hangul `std::string KoreanRuleG2p::extract_hangul(std::string_view s) const`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:722`

### g2p_hangul_rules_only `std::string KoreanRuleG2p::g2p_hangul_rules_only(
    std::string_view hangul) const`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:738`

### g2p_single_fragment `std::string KoreanRuleG2p::g2p_single_fragment(std::string_view frag) const`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:751`

### load_korean_lexicon_stream `void load_korean_lexicon_stream(
    std::istream& in, std::unordered_map<std::string, std::strin...`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:774`

### KoreanRuleG2p `KoreanRuleG2p::KoreanRuleG2p(std::filesystem::path dict_tsv, Options options)
    : options_(std:...`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:803`

### KoreanRuleG2p `KoreanRuleG2p::KoreanRuleG2p(std::string dict_tsv_utf8, Options options)
    : options_(std::move...`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:817`

### text_to_ipa `std::string KoreanRuleG2p::text_to_ipa(std::string text,
                                       s...`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:823`

### dialect_ids `std::vector<std::string> KoreanRuleG2p::dialect_ids()`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:1035`

### dialect_resolves_to_korean_rules `bool dialect_resolves_to_korean_rules(std::string_view dialect_id)`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:1040`

### resolve_korean_dict_path `std::filesystem::path resolve_korean_dict_path(
    const std::filesystem::path& model_root)`
- Defined: `core/moonshine-tts/src/lang-specific/korean.cpp:1048`

## core/moonshine-tts/src/lang-specific/korean.h

### dialect_id `const std::string& dialect_id() const`
- Defined: `core/moonshine-tts/src/lang-specific/korean.h:34`

## core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp

### open_session `Ort::Session open_session(Ort::Env& env,
                          const std::filesystem::path& m...`
- Defined: `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:20`

### open_session_memory `Ort::Session open_session_memory(Ort::Env& env, const void* data, size_t len,
                   ...`
- Defined: `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:37`

### encode_chars_for_model `std::vector<int64_t> encode_chars_for_model(
    const std::string& text,
    const std::unordere...`
- Defined: `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:45`

### decoder_io_padded `void decoder_io_padded(const std::vector<int64_t>& cur, int max_phoneme_len,
                    ...`
- Defined: `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:57`

### argmax_vocab_row `int argmax_vocab_row(const float* logits, int64_t vocab, int time_index)`
- Defined: `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:72`

### OnnxOovG2p `OnnxOovG2p::OnnxOovG2p(Ort::Env& env, const std::filesystem::path& model_onnx,
                  ...`
- Defined: `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:89`

### OnnxOovG2p `OnnxOovG2p::OnnxOovG2p(Ort::Env& env, const void* model_onnx_bytes,
                       size_t...`
- Defined: `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:96`

### predict_phonemes `std::vector<std::string> OnnxOovG2p::predict_phonemes(const std::string& word)`
- Defined: `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp:105`

## core/moonshine-tts/src/lang-specific/portuguese-rules.cpp

### pt_tolower `char32_t pt_tolower(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:23`

### is_pt_key_cp `bool is_pt_key_cp(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:68`

### normalize_lookup_key_utf8_impl `std::string normalize_lookup_key_utf8_impl(const std::string& word)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:84`

### normalize_lookup_key_utf8 `std::string normalize_lookup_key_utf8(const std::string& word)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:105`

### utf8_to_u32_pt `std::u32string utf8_to_u32_pt(const std::string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:109`

### u32_to_utf8_pt `std::string u32_to_utf8_pt(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:113`

### is_allowed_pt_grapheme `bool is_allowed_pt_grapheme(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:121`

### filter_pt_word_graphemes_utf8 `std::u32string filter_pt_word_graphemes_utf8(const std::string& word)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:134`

### is_vowel_pt_u32 `bool is_vowel_pt_u32(char32_t ch)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:150`

### strip_accent_base_pt `char32_t strip_accent_base_pt(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:158`

### should_hiatus_pt_u32 `bool should_hiatus_pt_u32(char32_t a, char32_t b)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:185`

### valid_onset2_end_u32 `bool valid_onset2_end_u32(char32_t a, char32_t b)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:260`

### port_orthographic_syllables_u32 `std::vector<std::u32string> port_orthographic_syllables_u32(
    const std::u32string& w0)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:296`

### accented_syllable_u32 `bool accented_syllable_u32(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:351`

### default_stressed_syllable_index_u32 `size_t default_stressed_syllable_index_u32(
    const std::vector<std::u32string>& syls, const st...`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:361`

### strip_stress_chars `std::string strip_stress_chars(std::string s)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:423`

### insert_primary_stress_before_vowel_utf8 `std::string insert_primary_stress_before_vowel_utf8(std::string ipa)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:429`

### roman_to_int_ascii `std::optional<int> roman_to_int_ascii(std::string_view u)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:452`

### roman_numeral_token_to_ipa `std::optional<std::string> roman_numeral_token_to_ipa(
    const std::string& letters_lower, bool...`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:490`

### prev_global_vowel_u32 `bool prev_global_vowel_u32(const std::u32string& full_word, size_t gidx)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:548`

### next_global_vowel_u32 `bool next_global_vowel_u32(const std::u32string& full_word, size_t gidx)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:568`

### syllable_has_u32 `bool syllable_has_u32(const std::u32string& s, char32_t ch)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:584`

### letters_to_ipa_no_stress_u32 `std::string letters_to_ipa_no_stress_u32(const std::u32string& s, bool is_pt_pt,
                ...`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:588`

### rules_word_to_ipa_single_u32 `std::string rules_word_to_ipa_single_u32(const std::u32string& wl,
                              ...`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:963`

### vowel_grapheme_tail_pt `bool vowel_grapheme_tail_pt(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:1017`

### pt_pt_apply_rules_final_s_to_esh `std::string pt_pt_apply_rules_final_s_to_esh(std::string ipa,
                                   ...`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:1025`

### rules_word_to_ipa_utf8 `std::string rules_word_to_ipa_utf8(const std::string& raw, bool is_pt_pt,
                       ...`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp:1160`

## core/moonshine-tts/src/lang-specific/portuguese.cpp

### utf8_lowercase_pt_surface `std::string utf8_lowercase_pt_surface(const std::string& word)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese.cpp:38`

### load_pt_lexicon_stream `void load_pt_lexicon_stream(std::istream& in,
                            std::unordered_map<std:...`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese.cpp:51`

### load_pt_lexicon_file `void load_pt_lexicon_file(const std::filesystem::path& path,
                          std::unord...`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese.cpp:83`

### is_all_ascii_digits `bool is_all_ascii_digits(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese.cpp:96`
- Doc: -- Numbers (portuguese_numbers.py) ------------------------------------------

### teens_word_pt `std::string teens_word_pt(int n, bool is_pt_pt)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese.cpp:120`

### under_100_tokens_pt `void under_100_tokens_pt(int n, bool is_pt_pt, std::vector<std::string>& out)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese.cpp:172`

### below_1000_tokens_pt `void below_1000_tokens_pt(int n, bool is_pt_pt, std::vector<std::string>& out)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese.cpp:199`

### below_1_000_000_tokens_pt `void below_1_000_000_tokens_pt(int n, bool is_pt_pt,
                               std::vector<s...`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese.cpp:227`

### expand_cardinal_digits_to_portuguese_words `std::string expand_cardinal_digits_to_portuguese_words(std::string_view s,
                      ...`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese.cpp:251`

### expand_digit_tokens_in_text `std::string expand_digit_tokens_in_text(std::string text, bool is_pt_pt)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese.cpp:288`

### is_pt_word_char `bool is_pt_word_char(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese.cpp:321`

### try_consume_pt_word `bool try_consume_pt_word(const std::string& text, size_t pos, size_t& out_end)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese.cpp:354`

### PortugueseRuleG2p `PortugueseRuleG2p::PortugueseRuleG2p(std::filesystem::path dict_tsv,
                            ...`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese.cpp:410`

### PortugueseRuleG2p `PortugueseRuleG2p::PortugueseRuleG2p(std::string dict_tsv_utf8,
                                 ...`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese.cpp:417`

### finalize_ipa `std::string PortugueseRuleG2p::finalize_ipa(std::string ipa,
                                    ...`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese.cpp:425`

### lookup_or_rules `std::string PortugueseRuleG2p::lookup_or_rules(
    const std::string& raw_word) const`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese.cpp:444`

### word_to_ipa `std::string PortugueseRuleG2p::word_to_ipa(const std::string& word) const`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese.cpp:507`

### text_to_ipa_no_expand `std::string PortugueseRuleG2p::text_to_ipa_no_expand(
    const std::string& text, std::vector<G2...`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese.cpp:530`

### text_to_ipa `std::string PortugueseRuleG2p::text_to_ipa(
    std::string text, std::vector<G2pWordLog>* per_wo...`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese.cpp:600`

### dialect_resolves_to_portugal_rules `bool dialect_resolves_to_portugal_rules(std::string_view dialect_id)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese.cpp:608`

### dialect_resolves_to_brazilian_portuguese_rules `bool dialect_resolves_to_brazilian_portuguese_rules(
    std::string_view dialect_id)`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese.cpp:617`

### dialect_ids `std::vector<std::string> PortugueseRuleG2p::dialect_ids()`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese.cpp:627`

### resolve_portuguese_dict_path `std::filesystem::path resolve_portuguese_dict_path(
    const std::filesystem::path& model_root, ...`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese.cpp:634`

## core/moonshine-tts/src/lang-specific/portuguese.h

### is_portugal `bool is_portugal() const`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese.h:37`

### dialect_id `const std::string& dialect_id() const`
- Defined: `core/moonshine-tts/src/lang-specific/portuguese.h:39`

## core/moonshine-tts/src/lang-specific/russian-numbers.cpp

### ru_ascii_all_digits `bool ru_ascii_all_digits(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/russian-numbers.cpp:13`

### ru_ones_digit `std::string ru_ones_digit(int n, bool feminine)`
- Defined: `core/moonshine-tts/src/lang-specific/russian-numbers.cpp:98`

### ru_append_under_100 `void ru_append_under_100(int n, bool feminine, std::vector<std::string>& out)`
- Defined: `core/moonshine-tts/src/lang-specific/russian-numbers.cpp:113`

### ru_append_cardinal_1_to_999 `void ru_append_cardinal_1_to_999(int n, bool feminine,
                                 std::vect...`
- Defined: `core/moonshine-tts/src/lang-specific/russian-numbers.cpp:133`

### ru_thousand_suffix `const char* ru_thousand_suffix(int q)`
- Defined: `core/moonshine-tts/src/lang-specific/russian-numbers.cpp:150`

### ru_append_below_1_000_000 `void ru_append_below_1_000_000(int n, std::vector<std::string>& out)`
- Defined: `core/moonshine-tts/src/lang-specific/russian-numbers.cpp:165`

### expand_cardinal_digits_to_russian_words `std::string expand_cardinal_digits_to_russian_words(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/russian-numbers.cpp:182`

### expand_russian_digit_tokens_in_text `std::string expand_russian_digit_tokens_in_text(std::string text)`
- Defined: `core/moonshine-tts/src/lang-specific/russian-numbers.cpp:219`

## core/moonshine-tts/src/lang-specific/russian.cpp

### is_unicode_mn `bool is_unicode_mn(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:36`

### is_combining_mark `bool is_combining_mark(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:55`

### russian_tolower_cp `char32_t russian_tolower_cp(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:57`

### is_russian_vowel_letter `bool is_russian_vowel_letter(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:67`

### is_russian_lex_key_cp `bool is_russian_lex_key_cp(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:75`

### append_nfd_expansion `void append_nfd_expansion(char32_t cp, std::u32string& out)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:125`

### u32_to_utf8 `std::string u32_to_utf8(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:135`

### unicode_tolower_like_python `char32_t unicode_tolower_like_python(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:143`

### normalize_lookup_key_utf8 `std::string normalize_lookup_key_utf8(const std::string& word)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:163`
- Doc: Mirrors Python ``normalize_lookup_key`` (lower + NFD + Mn strip + Cyrillic key filter).

### utf8_russian_lowercase `std::string utf8_russian_lowercase(const std::string& word)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:193`

### surface_is_all_lowercase_russian `bool surface_is_all_lowercase_russian(const std::string& surf)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:211`

### load_russian_lexicon_stream `void load_russian_lexicon_stream(
    std::istream& in, std::unordered_map<std::string, std::stri...`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:215`

### load_russian_lexicon_file `void load_russian_lexicon_file(
    const std::filesystem::path& path,
    std::unordered_map<std...`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:247`

### filter_russian_graphemes_keep_stress `std::string filter_russian_graphemes_keep_stress(std::string_view raw)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:258`

### strip_grapheme_diacritics_utf8 `std::string strip_grapheme_diacritics_utf8(std::string_view sv)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:280`

### acute_stressed_vowel_ordinal `std::optional<int> acute_stressed_vowel_ordinal(const std::string& w_nfc)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:304`

### vowel_ordinal_to_syllable `int vowel_ordinal_to_syllable(const std::vector<std::string>& syls,
                             ...`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:335`

### russian_orthographic_syllables_utf8 `std::vector<std::string> russian_orthographic_syllables_utf8(
    const std::string& word_lower)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:356`

### remove_if `std::remove_if(syllables.begin(), syllables.end(),
                     [](const std::string& x)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:423`

### stress_syllable_index `int stress_syllable_index(const std::vector<std::string>& syls,
                          const s...`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:428`

### syllable_index_per_codepoint `std::vector<int> syllable_index_per_codepoint(const std::string& w)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:452`

### palatalizable_cons `bool palatalizable_cons(char32_t ch)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:464`

### emit_consonant `std::string emit_consonant(char32_t ch, bool palatal)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:472`

### ipa_piece_ends_with_palatal `bool ipa_piece_ends_with_palatal(const std::string& piece)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:524`

### ipa_piece_last_is_vowel_letter `bool ipa_piece_last_is_vowel_letter(const std::string& piece)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:533`

### ipa_piece_after_hard_consonant `bool ipa_piece_after_hard_consonant(const std::string& piece)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:546`

### vowel_ipa `std::string vowel_ipa(char32_t ch, bool stressed, bool after_palatal,
                      bool ...`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:559`

### letters_to_ipa_rules `std::string letters_to_ipa_rules(const std::string& w_clean, int stress_syl)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:619`

### insert_primary_stress_before_vowel `std::string insert_primary_stress_before_vowel(std::string s)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:788`

### rules_word_to_ipa_single `std::string rules_word_to_ipa_single(const std::string& w_clean,
                                ...`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:808`

### rules_word_to_ipa `std::string rules_word_to_ipa(const std::string& raw, bool with_stress)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:820`

### is_latin1_supplement_python_word_char `bool is_latin1_supplement_python_word_char(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:885`

### is_unicode_word_char_w `bool is_unicode_word_char_w(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:906`

### utf8_contains_cyrillic `bool utf8_contains_cyrillic(const std::string& tok)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:931`

### try_consume_unicode_word `bool try_consume_unicode_word(const std::string& text, size_t pos,
                              ...`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:945`

### normalize_russian_fleeting_palatal_markers_utf8 `std::string normalize_russian_fleeting_palatal_markers_utf8(std::string ipa)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:976`
- Doc: Lexicon entries mark a fleeting soft sign as ⁽ʲ⁾ (U+207D U+02B2 U+207E). Piper / espeak-style phones and many vocoders o

### RussianRuleG2p `RussianRuleG2p::RussianRuleG2p(std::filesystem::path dict_tsv, Options options)
    : options_(op...`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:992`

### RussianRuleG2p `RussianRuleG2p::RussianRuleG2p(std::string dict_tsv_utf8, Options options)
    : options_(options)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:997`

### finalize_ipa `std::string RussianRuleG2p::finalize_ipa(std::string ipa) const`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:1003`

### lookup_or_rules `std::string RussianRuleG2p::lookup_or_rules(const std::string& raw_word) const`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:1017`

### word_to_ipa `std::string RussianRuleG2p::word_to_ipa(const std::string& word) const`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:1060`

### text_to_ipa_no_expand `std::string RussianRuleG2p::text_to_ipa_no_expand(
    const std::string& text, std::vector<G2pWo...`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:1082`

### text_to_ipa `std::string RussianRuleG2p::text_to_ipa(std::string text,
                                       ...`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:1156`

### dialect_resolves_to_russian_rules `bool dialect_resolves_to_russian_rules(std::string_view dialect_id)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:1164`

### dialect_ids `std::vector<std::string> RussianRuleG2p::dialect_ids()`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:1172`

### resolve_russian_dict_path `std::filesystem::path resolve_russian_dict_path(
    const std::filesystem::path& model_root)`
- Defined: `core/moonshine-tts/src/lang-specific/russian.cpp:1176`

## core/moonshine-tts/src/lang-specific/russian.h

### dialect_id `const std::string& dialect_id() const`
- Defined: `core/moonshine-tts/src/lang-specific/russian.h:36`

## core/moonshine-tts/src/lang-specific/spanish-numbers.cpp

### es_ascii_all_digits `bool es_ascii_all_digits(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish-numbers.cpp:13`

### es_append_under_100 `void es_append_under_100(int n, std::vector<std::string>& out)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish-numbers.cpp:76`

### es_append_below_1000 `void es_append_below_1000(int n, std::vector<std::string>& out)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish-numbers.cpp:97`

### es_append_below_1_000_000 `void es_append_below_1_000_000(int n, std::vector<std::string>& out)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish-numbers.cpp:122`

### expand_cardinal_digits_to_spanish_words `std::string expand_cardinal_digits_to_spanish_words(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish-numbers.cpp:143`

### expand_spanish_digit_tokens_in_text `std::string expand_spanish_digit_tokens_in_text(std::string text)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish-numbers.cpp:179`

## core/moonshine-tts/src/lang-specific/spanish-unicode.cpp

### lookup_sorted_pair `const char* lookup_sorted_pair(const std::pair<char32_t, const char*>* table,
                   ...`
- Defined: `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp:11`

### lower_bound `std::lower_bound(first, last, key,
                       [](const std::pair<char32_t, const char...`
- Defined: `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp:17`

### unicode_bitmap_get `bool unicode_bitmap_get(const std::uint32_t* bitmap, std::uint32_t nwords,
                      ...`
- Defined: `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp:25`

### utf32_to_utf8 `std::string utf32_to_utf8(const std::u32string& u)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp:39`

### utf8_to_utf32 `std::u32string utf8_to_utf32(const std::string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp:48`

### unicode_lower_utf8 `std::string unicode_lower_utf8(const std::string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp:52`

### strip_accents_utf8 `std::string strip_accents_utf8(const std::string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp:71`

### word_key `std::string word_key(const std::string& wraw)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp:90`

### is_word_char `bool is_word_char(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp:94`

### is_space_char `bool is_space_char(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp:99`

### strip_replacement_utf8 `const char* strip_replacement_utf8(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp:104`

## core/moonshine-tts/src/lang-specific/spanish.cpp

### is_vowel_ch `bool is_vowel_ch(char32_t ch)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:22`

### should_hiatus `bool should_hiatus(char32_t a, char32_t b)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:42`

### is_valid_onset2 `bool is_valid_onset2(char32_t a, char32_t b)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:144`

### clean_syllable_word `std::u32string clean_syllable_word(const std::u32string &word_lower)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:177`

### orthographic_syllables_utf8 `std::vector<std::string> orthographic_syllables_utf8(
    const std::string &word_lower_utf8)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:188`

### default_stressed_syllable_index_v2 `size_t default_stressed_syllable_index_v2(const std::u32string &w_clean_lower)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:225`

### lookup_x_exception `const char *lookup_x_exception(const std::string &wkey)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:294`

### apply_nasal_assimilation `std::string apply_nasal_assimilation(std::string s,
                                     const Sp...`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:303`

### insert_primary_stress_before_vowel `std::string insert_primary_stress_before_vowel(const std::string &ipa)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:332`

### count_primary_stress_utf8 `size_t count_primary_stress_utf8(const std::string &ipa)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:355`

### ipa_stress_at_start `bool ipa_stress_at_start(const std::string &ipa)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:370`

### apply_narrow_intervocalic_obstruents `std::string apply_narrow_intervocalic_obstruents(std::string ipa)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:379`

### apply_coda_s_weakening `std::string apply_coda_s_weakening(std::string ipa,
                                   SpanishDia...`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:416`

### postprocess_lexical_ipa `std::string postprocess_lexical_ipa(std::string ipa,
                                    const Sp...`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:431`

### prev_phoneme_was_vowel `bool prev_phoneme_was_vowel(const std::vector<std::string> &out)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:457`

### y_is_consonant `bool y_is_consonant(const std::u32string &letters_lower, size_t i)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:469`

### to_lower_cp `char32_t to_lower_cp(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:495`

### letters_to_ipa_no_stress `std::string letters_to_ipa_no_stress(const std::u32string &syl_lower,
                           ...`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:503`

### filter_word_letters_utf32 `std::u32string filter_word_letters_utf32(const std::string &wraw)`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:772`

### make_common `SpanishDialect make_common(const std::string &id, std::string ce_ci_z_ipa,
                      ...`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:790`

### spanish_dialect_cli_ids `std::vector<std::string> spanish_dialect_cli_ids()`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:815`
- Doc: include "spanish-numbers.cpp"

### dialect_ids `std::vector<std::string> SpanishRuleG2p::dialect_ids()`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:822`

### spanish_dialect_from_cli_id `SpanishDialect spanish_dialect_from_cli_id(
    const std::string &cli_id, bool narrow_intervocal...`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:826`

### SpanishRuleG2p `SpanishRuleG2p::SpanishRuleG2p(SpanishDialect dialect, bool with_stress,
                        ...`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:928`

### word_to_ipa `std::string SpanishRuleG2p::word_to_ipa(const std::string &word) const`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:934`

### text_to_ipa_no_expand `std::string SpanishRuleG2p::text_to_ipa_no_expand(
    const std::string &text, std::vector<G2pWo...`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:1002`

### text_to_ipa `std::string SpanishRuleG2p::text_to_ipa(std::string text,
                                       ...`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:1086`

### spanish_word_to_ipa `std::string spanish_word_to_ipa(const std::string &word,
                                const Sp...`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:1094`

### spanish_text_to_ipa `std::string spanish_text_to_ipa(const std::string &text,
                                const Sp...`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.cpp:1101`

## core/moonshine-tts/src/lang-specific/spanish.h

### dialect `const SpanishDialect& dialect() const`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.h:36`

### with_stress `bool with_stress() const`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.h:38`

### expand_cardinal_digits `bool expand_cardinal_digits() const`
- Defined: `core/moonshine-tts/src/lang-specific/spanish.h:39`

## core/moonshine-tts/src/lang-specific/turkish.cpp

### is_all_ascii_digits `bool is_all_ascii_digits(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:24`

### append_under_100 `void append_under_100(int n, std::vector<std::string>& out)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:45`

### append_tokens_0_999 `void append_tokens_0_999(int n, std::vector<std::string>& out)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:70`

### append_below_1_000_000 `void append_below_1_000_000(int n, std::vector<std::string>& out)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:94`

### join_space `std::string join_space(const std::vector<std::string>& p)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:115`

### expand_cardinal_digits_to_turkish_words `std::string expand_cardinal_digits_to_turkish_words(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:126`

### expand_turkish_digit_tokens_in_text `std::string expand_turkish_digit_tokens_in_text(std::string text)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:160`

### utf8_to_u32_nfc `std::u32string utf8_to_u32_nfc(const std::string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:195`
- Doc: -- NFC + lower + letters --------------------------------------------------

### turkish_tolower_cp `char32_t turkish_tolower_cp(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:206`

### turkish_lower_u32 `std::u32string turkish_lower_u32(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:217`

### is_tr_g2p_letter `bool is_tr_g2p_letter(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:226`

### letters_only_u32 `std::u32string letters_only_u32(const std::u32string& w)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:271`

### is_vowel_orth `bool is_vowel_orth(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:284`

### is_front_vowel `bool is_front_vowel(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:290`

### prev_letter_index `std::optional<size_t> prev_letter_index(const std::u32string& w, size_t i)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:295`

### next_letter_index `std::optional<size_t> next_letter_index(const std::u32string& w, size_t i)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:305`

### next_vowel_from `std::optional<char32_t> next_vowel_from(const std::u32string& w, size_t start)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:315`

### last_vowel_before `std::optional<char32_t> last_vowel_before(const std::u32string& w, size_t end)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:324`

### harmony_vowel_for_kg `std::optional<char32_t> harmony_vowel_for_kg(const std::u32string& w,
                           ...`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:333`

### map_k_or_g `std::string map_k_or_g(char32_t ch, const std::u32string& w, size_t i)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:342`

### map_simple_char `std::string map_simple_char(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:354`

### is_vowel_ipa_char `bool is_vowel_ipa_char(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:429`

### utf8_ipa_to_u32 `std::u32string utf8_ipa_to_u32(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:434`

### u32_to_utf8_ipa `std::string u32_to_utf8_ipa(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:439`

### insert_primary_stress_final `std::string insert_primary_stress_final(const std::string& ipa_utf8)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:447`

### is_turkish_word_char `bool is_turkish_word_char(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:496`

### is_space_cp `bool is_space_cp(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:516`

### TurkishRuleG2p `TurkishRuleG2p::TurkishRuleG2p(Options options) : options_(options)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:527`

### dialect_ids `std::vector<std::string> TurkishRuleG2p::dialect_ids()`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:529`

### word_to_ipa `std::string TurkishRuleG2p::word_to_ipa(const std::string& word) const`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:533`

### text_to_ipa_no_expand `std::string TurkishRuleG2p::text_to_ipa_no_expand(
    const std::string& text, std::vector<G2pWo...`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:617`

### text_to_ipa `std::string TurkishRuleG2p::text_to_ipa(std::string text,
                                       ...`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:695`

### dialect_resolves_to_turkish_rules `bool dialect_resolves_to_turkish_rules(std::string_view dialect_id)`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:703`

### turkish_word_to_ipa `std::string turkish_word_to_ipa(const std::string& word, bool with_stress,
                      ...`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:714`

### turkish_text_to_ipa `std::string turkish_text_to_ipa(const std::string& text, bool with_stress,
                      ...`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.cpp:722`

## core/moonshine-tts/src/lang-specific/turkish.h

### dialect_id `const std::string& dialect_id() const`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.h:28`

### with_stress `bool with_stress() const`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.h:30`

### expand_cardinal_digits `bool expand_cardinal_digits() const`
- Defined: `core/moonshine-tts/src/lang-specific/turkish.h:31`

## core/moonshine-tts/src/lang-specific/ukrainian.cpp

### is_all_ascii_digits `bool is_all_ascii_digits(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:26`

### utf8_nfc_utf8proc `std::string utf8_nfc_utf8proc(const std::string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:41`
- Doc: -- Stress stripping (NFD): remove common stress marks, keep U+0308 (ї vs і) --------------------

### ukrainian_strip_stress_marks_utf8 `std::string ukrainian_strip_stress_marks_utf8(std::string s)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:52`

### utf8_to_u32_nfc `std::u32string utf8_to_u32_nfc(const std::string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:78`

### ukrainian_lower_u32 `std::u32string ukrainian_lower_u32(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:89`

### thousand_noun_utf8 `std::string thousand_noun_utf8(int h)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:119`

### append_under_100_thousand_mult `void append_under_100_thousand_mult(int n, std::vector<std::string>& out)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:133`

### append_under_100_plain `void append_under_100_plain(int n, std::vector<std::string>& out)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:182`

### append_tokens_thousands_multiplier `void append_tokens_thousands_multiplier(int h, std::vector<std::string>& out)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:202`

### append_tokens_0_999 `void append_tokens_0_999(int n, std::vector<std::string>& out)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:223`

### append_below_1_000_000 `void append_below_1_000_000(int n, std::vector<std::string>& out)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:242`

### join_space `std::string join_space(const std::vector<std::string>& p)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:258`

### expand_cardinal_digits_to_ukrainian_words `std::string expand_cardinal_digits_to_ukrainian_words(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:269`

### expand_ukrainian_digit_tokens_in_text `std::string expand_ukrainian_digit_tokens_in_text(std::string text)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:303`

### is_vowel_letter `bool is_vowel_letter(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:339`
- Doc: -- G2P ---------------------------------------------------------------------------------------

### is_soft_vowel `bool is_soft_vowel(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:345`

### is_hard_no_pal `bool is_hard_no_pal(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:350`

### is_palatalizable `bool is_palatalizable(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:355`

### next_letter_index `std::optional<size_t> next_letter_index(const std::u32string& w, size_t start)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:362`

### v_allophone `std::string v_allophone(const std::u32string& w, size_t i)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:388`

### ends_with_palatal_suffix `bool ends_with_palatal_suffix(const std::string& p)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:403`

### is_vowel_ipa_piece `bool is_vowel_ipa_piece(const std::string& p)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:409`

### piece_ends_palatalized_consonant `bool piece_ends_palatalized_consonant(const std::vector<std::string>& pieces)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:433`

### palatalize_last `void palatalize_last(std::vector<std::string>& pieces)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:451`

### vowel_ipa `std::string vowel_ipa(char32_t ch, bool force_j, bool after_vowel_letter,
                      b...`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:470`

### ipa_vowel_char `bool ipa_vowel_char(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:519`

### u32_to_utf8 `std::string u32_to_utf8(const std::u32string& s)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:524`

### insert_primary_stress_penultimate `std::string insert_primary_stress_penultimate(const std::string& ipa_utf8)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:532`

### base_cons_ipa `std::string base_cons_ipa(char32_t c)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:573`

### word_to_ipa_inner `std::string word_to_ipa_inner(const std::u32string& w0, bool with_stress)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:620`

### filter_uk_word_chars `std::u32string filter_uk_word_chars(const std::u32string& w)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:726`

### is_ukrainian_word_char `bool is_ukrainian_word_char(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:743`

### is_space_cp `bool is_space_cp(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:760`

### word_to_ipa_from_utf32_word `std::string word_to_ipa_from_utf32_word(const std::u32string& letters,
                          ...`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:767`

### hyphen_join_word_ipas `std::string hyphen_join_word_ipas(const std::string& tok, bool with_stress)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:775`

### UkrainianRuleG2p `UkrainianRuleG2p::UkrainianRuleG2p(Options options) : options_(options)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:802`

### dialect_ids `std::vector<std::string> UkrainianRuleG2p::dialect_ids()`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:804`

### word_to_ipa `std::string UkrainianRuleG2p::word_to_ipa(const std::string& word) const`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:808`

### text_to_ipa_no_expand `std::string UkrainianRuleG2p::text_to_ipa_no_expand(
    const std::string& text, std::vector<G2p...`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:831`

### text_to_ipa `std::string UkrainianRuleG2p::text_to_ipa(
    std::string text, std::vector<G2pWordLog>* per_wor...`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:908`

### dialect_resolves_to_ukrainian_rules `bool dialect_resolves_to_ukrainian_rules(std::string_view dialect_id)`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:916`

### ukrainian_word_to_ipa `std::string ukrainian_word_to_ipa(const std::string& word, bool with_stress,
                    ...`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:927`

### ukrainian_text_to_ipa `std::string ukrainian_text_to_ipa(const std::string& text, bool with_stress,
                    ...`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.cpp:935`

## core/moonshine-tts/src/lang-specific/ukrainian.h

### dialect_id `const std::string& dialect_id() const`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.h:27`

### with_stress `bool with_stress() const`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.h:29`

### expand_cardinal_digits `bool expand_cardinal_digits() const`
- Defined: `core/moonshine-tts/src/lang-specific/ukrainian.h:30`

## core/moonshine-tts/src/lang-specific/vietnamese.cpp

### utf8_nfc_utf8proc `std::string utf8_nfc_utf8proc(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:22`

### utf8_lower_nfc `std::string utf8_lower_nfc(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:34`

### starts_with_sv `bool starts_with_sv(std::string_view s, std::string_view p)`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:53`

### ends_with_str `bool ends_with_str(const std::string& s, const std::string& suf)`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:57`

### split_tone `int split_tone(std::string_view in, std::string& body_nfc_out)`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:64`
- Doc: Tone combining marks (NFD) -> id 2..6; default 1 (ngang).

### is_vowel_letter_char `bool is_vowel_letter_char(char32_t cp)`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:100`

### is_vowel_first_utf8 `bool is_vowel_first_utf8(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:118`

### front_vowel_utf8 `bool front_vowel_utf8(std::string_view s)`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:130`

### rime_is_only_i `bool rime_is_only_i(std::string_view rest)`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:151`

### wants_labial_coda `bool wants_labial_coda(const std::string& nuc_ipa)`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:306`

### coda_simple `std::string coda_simple(const std::string& coda, const std::string& nuc_ipa)`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:322`

### nucleus_to_ipa `std::string nucleus_to_ipa(std::string_view nuc_sv)`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:355`
- Doc: UTF-8 NFC multigraphs (lowercase), same order as ``vietnamese_rule_g2p._NUCLEUS_PREFIX``.

### combine_nucleus_coda `std::string combine_nucleus_coda(const std::string& nuc_orth,
                                 co...`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:554`

### coda_obstruent_sac `bool coda_obstruent_sac(const std::string& coda)`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:596`

### tone_suffix_ipa `std::string tone_suffix_ipa(int tone, const std::string& coda_orth)`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:601`

### apply_tone `std::string apply_tone(const std::string& base, int tone, bool has_coda,
                       c...`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:631`

### is_unicode_edge_punct `bool is_unicode_edge_punct(char32_t cp, bool leading)`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:645`

### strip_edge_punct `std::string strip_edge_punct(std::string_view tok)`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:670`
- Doc: Strip leading/trailing punctuation by **code point** (never ``strchr`` on UTF-8 bytes — a byte like 0x99 can appear insi

### max_lex_key_words `int max_lex_key_words(const std::unordered_map<std::string, std::string>& lex)`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:714`

### load_vietnamese_lexicon_stream `void load_vietnamese_lexicon_stream(
    std::istream& in, std::unordered_map<std::string, std::s...`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:728`

### syllable_to_ipa `std::string VietnameseRuleG2p::syllable_to_ipa(std::string_view syllable_utf8)`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:757`

### VietnameseRuleG2p `VietnameseRuleG2p::VietnameseRuleG2p(std::filesystem::path dict_tsv)`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:784`

### VietnameseRuleG2p `VietnameseRuleG2p::VietnameseRuleG2p(std::string dict_tsv_utf8)`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:802`

### word_to_ipa `std::string VietnameseRuleG2p::word_to_ipa(std::string_view word) const`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:811`

### g2p_single_token `std::string VietnameseRuleG2p::g2p_single_token(std::string_view token) const`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:815`

### text_to_ipa `std::string VietnameseRuleG2p::text_to_ipa(
    std::string text, std::vector<G2pWordLog>* per_wo...`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:827`

### dialect_ids `std::vector<std::string> VietnameseRuleG2p::dialect_ids()`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:941`

### dialect_resolves_to_vietnamese_rules `bool dialect_resolves_to_vietnamese_rules(std::string_view dialect_id)`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:946`

### resolve_vietnamese_dict_path `std::filesystem::path resolve_vietnamese_dict_path(
    const std::filesystem::path& model_root)`
- Defined: `core/moonshine-tts/src/lang-specific/vietnamese.cpp:954`

## core/moonshine-tts/src/moonshine-asset-catalog.cpp

### normalize_lang_key_cli `std::string normalize_lang_key_cli(std::string_view raw)`
- Defined: `core/moonshine-tts/src/moonshine-asset-catalog.cpp:15`

### hyphen_to_underscore `std::string hyphen_to_underscore(std::string s)`
- Defined: `core/moonshine-tts/src/moonshine-asset-catalog.cpp:29`

### english_g2p_keys `std::vector<std::string> english_g2p_keys()`
- Defined: `core/moonshine-tts/src/moonshine-asset-catalog.cpp:38`

### chinese_g2p_keys `std::vector<std::string> chinese_g2p_keys()`
- Defined: `core/moonshine-tts/src/moonshine-asset-catalog.cpp:47`

### japanese_g2p_keys `std::vector<std::string> japanese_g2p_keys()`
- Defined: `core/moonshine-tts/src/moonshine-asset-catalog.cpp:57`

### korean_g2p_keys `std::vector<std::string> korean_g2p_keys()`
- Defined: `core/moonshine-tts/src/moonshine-asset-catalog.cpp:67`

### arabic_g2p_keys `std::vector<std::string> arabic_g2p_keys()`
- Defined: `core/moonshine-tts/src/moonshine-asset-catalog.cpp:73`

### french_g2p_keys `std::vector<std::string> french_g2p_keys()`
- Defined: `core/moonshine-tts/src/moonshine-asset-catalog.cpp:83`

### lookup_g2p_dependency_keys `std::optional<std::vector<std::string>> lookup_g2p_dependency_keys(
    std::string_view raw)`
- Defined: `core/moonshine-tts/src/moonshine-asset-catalog.cpp:222`

### moonshine_asset_catalog_populate_default_g2p_files `void moonshine_asset_catalog_populate_default_g2p_files(
    FileInformationMap& files)`
- Defined: `core/moonshine-tts/src/moonshine-asset-catalog.cpp:239`

### moonshine_asset_catalog_g2p_dependency_keys `std::optional<std::vector<std::string>>
moonshine_asset_catalog_g2p_dependency_keys(std::string_v...`
- Defined: `core/moonshine-tts/src/moonshine-asset-catalog.cpp:247`

### moonshine_asset_catalog_all_g2p_dependency_keys_union `std::vector<std::string>
moonshine_asset_catalog_all_g2p_dependency_keys_union()`
- Defined: `core/moonshine-tts/src/moonshine-asset-catalog.cpp:252`

### moonshine_asset_catalog_all_registered_language_tags `std::vector<std::string>
moonshine_asset_catalog_all_registered_language_tags()`
- Defined: `core/moonshine-tts/src/moonshine-asset-catalog.cpp:266`

## core/moonshine-tts/src/moonshine-g2p-options.cpp

### optional_path_from_string `std::optional<std::filesystem::path> optional_path_from_string(
    const std::string& value)`
- Defined: `core/moonshine-tts/src/moonshine-g2p-options.cpp:14`

### set_canonical_file `void set_canonical_file(FileInformationMap& files,
                        std::string_view canon...`
- Defined: `core/moonshine-tts/src/moonshine-g2p-options.cpp:23`

### set_override_file `void set_override_file(FileInformationMap& files, std::string_view map_key,
                     ...`
- Defined: `core/moonshine-tts/src/moonshine-g2p-options.cpp:34`

### is_known_g2p_option `bool is_known_g2p_option(std::string_view key)`
- Defined: `core/moonshine-tts/src/moonshine-g2p-options.cpp:44`

### prepare_g2p_file_information_path `void prepare_g2p_file_information_path(FileInformation& fi,
                                     ...`
- Defined: `core/moonshine-tts/src/moonshine-g2p-options.cpp:107`

### MoonshineG2POptions `MoonshineG2POptions::MoonshineG2POptions()`
- Defined: `core/moonshine-tts/src/moonshine-g2p-options.cpp:131`

### relative_asset_path `std::filesystem::path MoonshineG2POptions::relative_asset_path(
    std::string_view canonical_ke...`
- Defined: `core/moonshine-tts/src/moonshine-g2p-options.cpp:135`

### optional_override_path `std::optional<std::filesystem::path>
MoonshineG2POptions::optional_override_path(std::string_view...`
- Defined: `core/moonshine-tts/src/moonshine-g2p-options.cpp:145`

### asset_is_available `bool MoonshineG2POptions::asset_is_available(
    std::string_view canonical_key) const`
- Defined: `core/moonshine-tts/src/moonshine-g2p-options.cpp:158`

### read_binary_asset `std::vector<uint8_t> MoonshineG2POptions::read_binary_asset(
    std::string_view canonical_key) ...`
- Defined: `core/moonshine-tts/src/moonshine-g2p-options.cpp:174`

### read_utf8_asset `std::string MoonshineG2POptions::read_utf8_asset(
    std::string_view canonical_key) const`
- Defined: `core/moonshine-tts/src/moonshine-g2p-options.cpp:192`

### parse_options `void MoonshineG2POptions::parse_options(
    const std::vector<std::pair<std::string, std::string...`
- Defined: `core/moonshine-tts/src/moonshine-g2p-options.cpp:198`

## core/moonshine-tts/src/moonshine-g2p-options.h

### g2p_bundle_file_key `inline std::string g2p_bundle_file_key(std::string_view bundle_dir_key,
                         ...`
- Defined: `core/moonshine-tts/src/moonshine-g2p-options.h:18`
- Doc: ``<bundle_dir_key>/<filename>`` for ``FileInformationMap`` / ``read_*_asset``.

## core/moonshine-tts/src/moonshine-g2p.cpp

### trim_copy `std::string trim_copy(std::string_view s)`
- Defined: `core/moonshine-tts/src/moonshine-g2p.cpp:30`

### normalize_spanish_dialect_cli_key `std::string normalize_spanish_dialect_cli_key(std::string_view raw)`
- Defined: `core/moonshine-tts/src/moonshine-g2p.cpp:45`
- Doc: Normalize user input like ``es_ar`` / ``es-mx`` to keys accepted by ``spanish_dialect_from_cli_id`` (e.g. ``es-AR``, ``e

### rule_backend_name `const char* rule_backend_name(RuleBasedG2pKind k)`
- Defined: `core/moonshine-tts/src/moonshine-g2p.cpp:67`

### dialect_resolves_to_spanish_rules `bool dialect_resolves_to_spanish_rules(std::string_view dialect_id,
                             ...`
- Defined: `core/moonshine-tts/src/moonshine-g2p.cpp:107`

### dialect_uses_rule_based_g2p `bool dialect_uses_rule_based_g2p(std::string_view dialect_id,
                                 co...`
- Defined: `core/moonshine-tts/src/moonshine-g2p.cpp:121`

### MoonshineG2P `MoonshineG2P::MoonshineG2P(std::string dialect_id,
                           MoonshineG2POptions...`
- Defined: `core/moonshine-tts/src/moonshine-g2p.cpp:185`

### text_to_ipa `std::string MoonshineG2P::text_to_ipa(std::string_view text,
                                    ...`
- Defined: `core/moonshine-tts/src/moonshine-g2p.cpp:216`

## core/moonshine-tts/src/moonshine-g2p.h

### uses_spanish_rules `bool uses_spanish_rules() const`
- Defined: `core/moonshine-tts/src/moonshine-g2p.h:47`

### uses_german_rules `bool uses_german_rules() const`
- Defined: `core/moonshine-tts/src/moonshine-g2p.h:51`

### uses_french_rules `bool uses_french_rules() const`
- Defined: `core/moonshine-tts/src/moonshine-g2p.h:54`

### uses_dutch_rules `bool uses_dutch_rules() const`
- Defined: `core/moonshine-tts/src/moonshine-g2p.h:57`

### uses_italian_rules `bool uses_italian_rules() const`
- Defined: `core/moonshine-tts/src/moonshine-g2p.h:60`

### uses_russian_rules `bool uses_russian_rules() const`
- Defined: `core/moonshine-tts/src/moonshine-g2p.h:63`

### uses_chinese_rules `bool uses_chinese_rules() const`
- Defined: `core/moonshine-tts/src/moonshine-g2p.h:66`

### uses_korean_rules `bool uses_korean_rules() const`
- Defined: `core/moonshine-tts/src/moonshine-g2p.h:69`

### uses_vietnamese_rules `bool uses_vietnamese_rules() const`
- Defined: `core/moonshine-tts/src/moonshine-g2p.h:72`

### uses_japanese_rules `bool uses_japanese_rules() const`
- Defined: `core/moonshine-tts/src/moonshine-g2p.h:75`

### uses_arabic_rules `bool uses_arabic_rules() const`
- Defined: `core/moonshine-tts/src/moonshine-g2p.h:78`

### uses_portuguese_rules `bool uses_portuguese_rules() const`
- Defined: `core/moonshine-tts/src/moonshine-g2p.h:81`

### uses_turkish_rules `bool uses_turkish_rules() const`
- Defined: `core/moonshine-tts/src/moonshine-g2p.h:84`

### uses_ukrainian_rules `bool uses_ukrainian_rules() const`
- Defined: `core/moonshine-tts/src/moonshine-g2p.h:87`

### uses_hindi_rules `bool uses_hindi_rules() const`
- Defined: `core/moonshine-tts/src/moonshine-g2p.h:90`

### uses_english_rules `bool uses_english_rules() const`
- Defined: `core/moonshine-tts/src/moonshine-g2p.h:93`

### uses_onnx `static constexpr bool uses_onnx()`
- Defined: `core/moonshine-tts/src/moonshine-g2p.h:99`
- Doc: Always false: full-bundle ONNX G2P was removed; English may still load OOV ONNX inside ``EnglishRuleG2p``.

### dialect_id `const std::string& dialect_id() const`
- Defined: `core/moonshine-tts/src/moonshine-g2p.h:103`
- Doc: Canonical dialect id (e.g. ``es-AR`` for Spanish, ``en_us`` for US English).

## core/moonshine-tts/src/moonshine-tts-options.cpp

### apply_synthesis_output_effects `void apply_synthesis_output_effects(std::vector<float>& audio,
                                  ...`
- Defined: `core/moonshine-tts/src/moonshine-tts-options.cpp:12`

### MoonshineTTSOptions `MoonshineTTSOptions::MoonshineTTSOptions()`
- Defined: `core/moonshine-tts/src/moonshine-tts-options.cpp:38`

### apply_voice_engine_prefix `void MoonshineTTSOptions::apply_voice_engine_prefix()`
- Defined: `core/moonshine-tts/src/moonshine-tts-options.cpp:45`

### tts_relative_path `std::filesystem::path MoonshineTTSOptions::tts_relative_path(
    std::string_view canonical_key)...`
- Defined: `core/moonshine-tts/src/moonshine-tts-options.cpp:71`

### parse_options `void MoonshineTTSOptions::parse_options(
    const std::vector<std::pair<std::string, std::string...`
- Defined: `core/moonshine-tts/src/moonshine-tts-options.cpp:81`

## core/moonshine-tts/src/moonshine-tts.cpp

### utf8_nfc `std::string utf8_nfc(std::string_view s)`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:43`

### replace_utf8 `void replace_utf8(std::string& s, std::string_view old_s,
                  std::string_view new_s)`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:55`

### empty `bool empty() const`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:74`

### parse_synthesis_overrides_from_pairs `SynthesisOverrides parse_synthesis_overrides_from_pairs(
    const std::vector<std::pair<std::str...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:80`

### py_isspace_utf8_ch `bool py_isspace_utf8_ch(std::string_view ch)`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:97`

### collapse_whitespace_join_single_space `std::string collapse_whitespace_join_single_space(const std::string& s)`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:115`

### normalize_lang_key `std::string normalize_lang_key(std::string_view raw)`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:143`

### lookup_lang_profile `const LangProfile* lookup_lang_profile(std::string_view key)`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:165`

### resolve_lang_for_tts `void resolve_lang_for_tts(const std::string& lk, const MoonshineG2POptions& opt,
                ...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:202`
- Doc: Fills *profile* and *g2p_dialect* for ``MoonshineG2P`` (Kokoro locale + rule-based tag).

### kokoro_tts_lang_supported_inner `bool kokoro_tts_lang_supported_inner(std::string_view lang_cli,
                                 ...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:219`

### voice_prefix_ok `bool voice_prefix_ok(char kokoro_lang, std::string_view voice)`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:230`

### maybe_align_en_profile_for_kokoro_voice `void maybe_align_en_profile_for_kokoro_voice(std::string_view voice,
                            ...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:252`
- Doc: If ``--lang`` is US English but the user asked for a British Kokoro voice id (``bf_*`` / ``bm_*``), or the reverse, swit

### infer_lang_profile_from_kokoro_voice `bool infer_lang_profile_from_kokoro_voice(std::string_view voice_sv,
                            ...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:275`
- Doc: When the CLI language is not a Kokoro-backed locale (e.g. ``de`` for Piper-only), but the user selected a Kokoro voice i

### resolve_lang_for_kokoro `void resolve_lang_for_kokoro(const std::string& lk,
                             const MoonshineG...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:302`
- Doc: Like ``resolve_lang_for_tts`` for Kokoro paths, but if *lk* is not Kokoro-capable (Piper-only language), fall back to a 

### kokoro_voice_asset_exists `bool kokoro_voice_asset_exists(const std::string& voice_id,
                               const ...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:315`

### select_voice_id `std::string select_voice_id(char kokoro_lang, std::string_view requested,
                       ...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:357`

### apply_diphthong_map `void apply_diphthong_map(std::string& s, char kokoro_lang)`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:427`

### apply_chinese_kokoro_normalization `void apply_chinese_kokoro_normalization(std::string& ipa)`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:461`
- Doc: Mandarin Chinese IPA normalization for Kokoro: Chao tone letters → arrow contour symbols, consonant mappings to Kokoro's

### normalize_ipa_to_kokoro `std::string normalize_ipa_to_kokoro(
    std::string ipa, char kokoro_lang,
    const std::unorde...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:534`

### chunk_phonemes `std::vector<std::string> chunk_phonemes(const std::string& ps,
                                  ...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:556`

### phoneme_str_to_input_ids `std::vector<int64_t> phoneme_str_to_input_ids(
    const std::string& phonemes,
    const std::un...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:620`

### read_kokorovoice_bytes `void read_kokorovoice_bytes(const uint8_t* data, size_t size,
                            std::st...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:635`

### read_kokorovoice `void read_kokorovoice(const std::filesystem::path& path,
                      std::vector<float>...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:668`

### kokoro_tts_lang_supported `bool kokoro_tts_lang_supported(std::string_view lang_cli,
                               const Mo...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:684`

### ascii_lowercase_copy `std::string ascii_lowercase_copy(std::string_view s)`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:689`

### tts_map_path `std::filesystem::path tts_map_path(const FileInformationMap& m,
                                 ...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:699`

### make_piper_options `PiperTTSOptions make_piper_options(std::string_view language,
                                   ...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:709`

### kokoro_vocoder_dependency_keys_with_options `std::vector<std::string> kokoro_vocoder_dependency_keys_with_options(
    std::string_view langua...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:759`

### piper_vocoder_dependency_keys_with_options `std::vector<std::string> piper_vocoder_dependency_keys_with_options(
    std::string_view languag...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:865`

### make_zipvoice_options `ZipVoiceTTSOptions make_zipvoice_options(std::string_view language,
                             ...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:885`

### zipvoice_vocoder_dependency_keys `std::vector<std::string> zipvoice_vocoder_dependency_keys()`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:914`

### zipvoice_asset_present `bool zipvoice_asset_present(const MoonshineTTSOptions& opt,
                            std::stri...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:922`

### zipvoice_assets_available `bool zipvoice_assets_available(const MoonshineTTSOptions& opt)`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:939`

### detect_kokoro_style_input_name `void detect_kokoro_style_input_name()`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:999`

### detect_speed_input_element_type `void detect_speed_input_element_type()`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1010`

### speed `double speed() const`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1027`

### set_speed `void set_speed(double s)`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1029`

### normalize_audio `bool normalize_audio() const`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1037`

### set_normalize_audio `void set_normalize_audio(bool on)`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1039`

### output_volume `float output_volume() const`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1040`

### set_output_volume `void set_output_volume(float v)`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1041`

### KokoroTtsEngine `explicit KokoroTtsEngine(std::string_view language, MoonshineTTSOptions opt)`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1042`

### reload_voice_tensor `void reload_voice_tensor()`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1157`

### synthesize `std::vector<float> synthesize(std::string_view text)`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1198`

### synthesize_from_ipa `std::vector<float> synthesize_from_ipa(std::string_view ipa)`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1210`
- Doc: Synthesize from an existing IPA phoneme string (skips G2P). The input is normalized to Kokoro's phoneme inventory just l

### Impl `explicit Impl(std::string_view language, const MoonshineTTSOptions& opt_in)`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1329`

### synthesize_unlocked `std::vector<float> synthesize_unlocked(std::string_view text)`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1394`

### synthesize_from_phonemes_unlocked `std::vector<float> synthesize_from_phonemes_unlocked(
      std::string_view phonemes)`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1411`

### synthesize `std::vector<float> synthesize(std::string_view text)`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1422`

### synthesize_from_phonemes `std::vector<float> synthesize_from_phonemes(std::string_view phonemes)`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1427`

### synthesize_from_phonemes_with_overrides `std::vector<float> synthesize_from_phonemes_with_overrides(
      std::string_view phonemes, cons...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1432`

### synthesize_with_overrides `std::vector<float> synthesize_with_overrides(std::string_view text,
                             ...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1438`

### run_with_overrides `template <typename Produce>
  std::vector<float> run_with_overrides(const SynthesisOverrides& ov,...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1448`
- Doc: Applies ``ov`` to the active engine, invokes ``produce`` while holding the synthesis lock, then restores the previous ef

### MoonshineTTS `MoonshineTTS::MoonshineTTS(std::string_view language,
                           const MoonshineT...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1502`

### synthesize `std::vector<float> MoonshineTTS::synthesize(std::string_view text)`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1511`

### synthesize `std::vector<float> MoonshineTTS::synthesize(
    std::string_view text,
    const std::vector<std...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1515`

### synthesize_from_phonemes `std::vector<float> MoonshineTTS::synthesize_from_phonemes(
    std::string_view phonemes)`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1529`

### synthesize_from_phonemes `std::vector<float> MoonshineTTS::synthesize_from_phonemes(
    std::string_view phonemes,
    con...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1534`

### write_wav_mono_pcm16 `void write_wav_mono_pcm16(const std::filesystem::path& path,
                          const std:...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1548`

### moonshine_catalog_tts_vocoder_only_dependency_keys `std::vector<std::string> moonshine_catalog_tts_vocoder_only_dependency_keys(
    std::string_view...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1611`

### moonshine_catalog_tts_vocoder_only_dependency_keys `std::vector<std::string> moonshine_catalog_tts_vocoder_only_dependency_keys(
    std::string_view...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1638`

### moonshine_catalog_all_tts_vocoder_dependency_keys_union `std::vector<std::string>
moonshine_catalog_all_tts_vocoder_dependency_keys_union()`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1644`

### moonshine_list_tts_voices_with_availability `std::vector<MoonshineTtsVoiceAvailability>
moonshine_list_tts_voices_with_availability(std::strin...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1661`

### sort `std::sort(
        out.begin(), out.end(),
        [](const MoonshineTtsVoiceAvailability& a,
   ...`
- Defined: `core/moonshine-tts/src/moonshine-tts.cpp:1718`

## core/moonshine-tts/src/ort-onnx-external-data.cpp

### ort_add_external_initializer_files_for_onnx_model_buffer `void ort_add_external_initializer_files_for_onnx_model_buffer(
    Ort::SessionOptions& opts, con...`
- Defined: `core/moonshine-tts/src/ort-onnx-external-data.cpp:9`

## core/moonshine-tts/src/ort-session-options.cpp

### make_ort_session_options `Ort::SessionOptions make_ort_session_options(
    const std::vector<std::string>& provider_names,...`
- Defined: `core/moonshine-tts/src/ort-session-options.cpp:6`

## core/moonshine-tts/src/piper-tts.cpp

### normalize_lang_key `std::string normalize_lang_key(std::string_view raw)`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:34`

### py_isspace_utf8_ch `bool py_isspace_utf8_ch(std::string_view ch)`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:48`

### lookup_piper_lang_row `const PiperLangRow* lookup_piper_lang_row(std::string_view k)`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:72`

### piper_ipa_norm_lang_key `std::string piper_ipa_norm_lang_key(const std::string& lk,
                                    st...`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:129`

### resolve_piper_lang `void resolve_piper_lang(const std::string& lk, const MoonshineG2POptions& opt,
                  ...`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:143`

### pick_onnx_path `std::filesystem::path pick_onnx_path(const std::filesystem::path& voices_dir,
                   ...`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:177`

### piper_model_json_path_for_onnx `std::filesystem::path piper_model_json_path_for_onnx(
    const std::filesystem::path& onnx_path,...`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:233`
- Doc: Piper pairs ``foo.onnx`` with ``foo.onnx.json``. If ``json_dir`` is empty, that file sits beside ``onnx_path``.

### append_phoneme_ids `void append_phoneme_ids(
    const std::unordered_map<std::string, std::vector<int64_t>>& id_map,...`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:243`

### ipa_utf8_to_piper_ids `std::vector<int64_t> ipa_utf8_to_piper_ids(
    const std::string& ipa_nfc,
    const std::unorde...`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:255`

### resample_linear `std::vector<float> resample_linear(const std::vector<float>& x, int src_sr,
                     ...`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:277`

### load_piper_onnx_json `void load_piper_onnx_json(
    const std::filesystem::path& json_path,
    std::unordered_map<std...`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:300`

### load_piper_onnx_json_bytes `void load_piper_onnx_json_bytes(
    const char* data, size_t size, std::string_view ctx,
    std...`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:353`

### run_ort_from_phoneme_ids `std::vector<float> run_ort_from_phoneme_ids(const std::vector<int64_t>& ids)`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:445`

### reload_session_from_onnx `void reload_session_from_onnx()`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:510`

### Impl `explicit Impl(const PiperTTSOptions& opt)
      : speed_(opt.speed),
        ort_provider_names_(...`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:565`

### set_speed `void set_speed(double s)`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:612`

### set_lang `void set_lang(const std::string& lk)`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:620`

### set_onnx_model `void set_onnx_model(std::string_view stem_or_base)`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:634`

### synthesize `std::vector<float> synthesize(std::string_view text)`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:643`

### synthesize_from_ipa `std::vector<float> synthesize_from_ipa(std::string_view ipa_in)`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:648`

### synthesize_phoneme_ids `std::vector<float> synthesize_phoneme_ids(
      const std::vector<int64_t>& phoneme_ids)`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:668`

### PiperTTS `PiperTTS::PiperTTS(const PiperTTSOptions& opt)
    : impl_(std::make_unique<Impl>(opt))`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:674`

### set_lang `void PiperTTS::set_lang(std::string_view lang_cli)`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:682`

### set_speed `void PiperTTS::set_speed(double speed)`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:686`

### speed `double PiperTTS::speed() const`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:688`

### set_onnx_model `void PiperTTS::set_onnx_model(std::string_view basename_or_stem)`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:690`

### normalize_audio `bool PiperTTS::normalize_audio() const`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:694`

### set_normalize_audio `void PiperTTS::set_normalize_audio(bool on)`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:696`

### output_volume `float PiperTTS::output_volume() const`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:698`

### set_output_volume `void PiperTTS::set_output_volume(float volume)`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:700`

### synthesize `std::vector<float> PiperTTS::synthesize(std::string_view text)`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:704`

### synthesize_from_ipa `std::vector<float> PiperTTS::synthesize_from_ipa(std::string_view ipa)`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:708`

### synthesize_phoneme_ids `std::vector<float> PiperTTS::synthesize_phoneme_ids(
    const std::vector<int64_t>& phoneme_ids)`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:712`

### piper_default_model_bundle_relative_paths `bool piper_default_model_bundle_relative_paths(
    std::string_view lang_cli, const MoonshineG2P...`
- Defined: `core/moonshine-tts/src/piper-tts.cpp:795`

## core/moonshine-tts/src/rule-based-g2p-factory.cpp

### resolve_french_dict_path `std::filesystem::path resolve_french_dict_path(const MoonshineG2POptions& opt)`
- Defined: `core/moonshine-tts/src/rule-based-g2p-factory.cpp:40`

### resolve_french_csv_dir `std::filesystem::path resolve_french_csv_dir(const MoonshineG2POptions& opt)`
- Defined: `core/moonshine-tts/src/rule-based-g2p-factory.cpp:45`

### normalize_spanish_dialect_cli_key `std::string normalize_spanish_dialect_cli_key(std::string_view raw)`
- Defined: `core/moonshine-tts/src/rule-based-g2p-factory.cpp:50`

### file_looks_like_git_lfs_pointer `bool file_looks_like_git_lfs_pointer(const std::filesystem::path& p)`
- Defined: `core/moonshine-tts/src/rule-based-g2p-factory.cpp:73`

### utf8_content_git_lfs_pointer_stub `bool utf8_content_git_lfs_pointer_stub(std::string_view content)`
- Defined: `core/moonshine-tts/src/rule-based-g2p-factory.cpp:85`

### read_path_as_utf8 `std::string read_path_as_utf8(const std::filesystem::path& p)`
- Defined: `core/moonshine-tts/src/rule-based-g2p-factory.cpp:95`

### g2p_onnx_bundle_reachable `bool g2p_onnx_bundle_reachable(const MoonshineG2POptions& o,
                               std::...`
- Defined: `core/moonshine-tts/src/rule-based-g2p-factory.cpp:128`

### g2p_onnx_bundle_includes_model_file `bool g2p_onnx_bundle_includes_model_file(
    const MoonshineG2POptions& o, std::string_view bund...`
- Defined: `core/moonshine-tts/src/rule-based-g2p-factory.cpp:141`
- Doc: True when ``meta.json`` is available and the model file it names exists on disk or in memory.

### try_english `std::optional<RuleBasedG2pInstance> try_english(
    std::string_view trimmed, const MoonshineG2P...`
- Defined: `core/moonshine-tts/src/rule-based-g2p-factory.cpp:173`

### try_spanish `std::optional<RuleBasedG2pInstance> try_spanish(
    std::string_view trimmed, const MoonshineG2P...`
- Defined: `core/moonshine-tts/src/rule-based-g2p-factory.cpp:287`

### try_german `std::optional<RuleBasedG2pInstance> try_german(
    std::string_view trimmed, const MoonshineG2PO...`
- Defined: `core/moonshine-tts/src/rule-based-g2p-factory.cpp:304`

### try_french `std::optional<RuleBasedG2pInstance> try_french(
    std::string_view trimmed, const MoonshineG2PO...`
- Defined: `core/moonshine-tts/src/rule-based-g2p-factory.cpp:334`

### try_dutch `std::optional<RuleBasedG2pInstance> try_dutch(
    std::string_view trimmed, const MoonshineG2POp...`
- Defined: `core/moonshine-tts/src/rule-based-g2p-factory.cpp:384`

### try_italian `std::optional<RuleBasedG2pInstance> try_italian(
    std::string_view trimmed, const MoonshineG2P...`
- Defined: `core/moonshine-tts/src/rule-based-g2p-factory.cpp:416`

### try_russian `std::optional<RuleBasedG2pInstance> try_russian(
    std::string_view trimmed, const MoonshineG2P...`
- Defined: `core/moonshine-tts/src/rule-based-g2p-factory.cpp:448`

### try_chinese `std::optional<RuleBasedG2pInstance> try_chinese(
    std::string_view trimmed, const MoonshineG2P...`
- Defined: `core/moonshine-tts/src/rule-based-g2p-factory.cpp:479`

### try_korean `std::optional<RuleBasedG2pInstance> try_korean(
    std::string_view trimmed, const MoonshineG2PO...`
- Defined: `core/moonshine-tts/src/rule-based-g2p-factory.cpp:520`

### try_vietnamese `std::optional<RuleBasedG2pInstance> try_vietnamese(
    std::string_view trimmed, const Moonshine...`
- Defined: `core/moonshine-tts/src/rule-based-g2p-factory.cpp:546`

### try_japanese `std::optional<RuleBasedG2pInstance> try_japanese(
    std::string_view trimmed, const MoonshineG2...`
- Defined: `core/moonshine-tts/src/rule-based-g2p-factory.cpp:570`

### try_arabic `std::optional<RuleBasedG2pInstance> try_arabic(
    std::string_view trimmed, const MoonshineG2PO...`
- Defined: `core/moonshine-tts/src/rule-based-g2p-factory.cpp:610`

### try_turkish `std::optional<RuleBasedG2pInstance> try_turkish(
    std::string_view trimmed, const MoonshineG2P...`
- Defined: `core/moonshine-tts/src/rule-based-g2p-factory.cpp:649`

### try_ukrainian `std::optional<RuleBasedG2pInstance> try_ukrainian(
    std::string_view trimmed, const MoonshineG...`
- Defined: `core/moonshine-tts/src/rule-based-g2p-factory.cpp:664`

### try_hindi `std::optional<RuleBasedG2pInstance> try_hindi(
    std::string_view trimmed, const MoonshineG2POp...`
- Defined: `core/moonshine-tts/src/rule-based-g2p-factory.cpp:679`

### try_portuguese `std::optional<RuleBasedG2pInstance> try_portuguese(
    std::string_view trimmed, const Moonshine...`
- Defined: `core/moonshine-tts/src/rule-based-g2p-factory.cpp:706`

### create_rule_based_g2p `std::optional<RuleBasedG2pInstance> create_rule_based_g2p(
    std::string_view dialect_id, const...`
- Defined: `core/moonshine-tts/src/rule-based-g2p-factory.cpp:785`

## core/moonshine-tts/src/text-normalize.cpp

### is_word_char_utf8 `bool is_word_char_utf8(std::string_view unit)`
- Defined: `core/moonshine-tts/src/text-normalize.cpp:9`

### split_text_to_words `std::vector<std::string> split_text_to_words(std::string_view text)`
- Defined: `core/moonshine-tts/src/text-normalize.cpp:24`

### normalize_word_for_lookup `std::string normalize_word_for_lookup(std::string_view token)`
- Defined: `core/moonshine-tts/src/text-normalize.cpp:47`

### normalize_grapheme_key `std::string normalize_grapheme_key(std::string_view word_token)`
- Defined: `core/moonshine-tts/src/text-normalize.cpp:74`

## core/moonshine-tts/src/utf8-utils.cpp

### utf8_decode_at `bool utf8_decode_at(const std::string& s, size_t i, char32_t& out_cp,
                    size_t&...`
- Defined: `core/moonshine-tts/src/utf8-utils.cpp:6`

### utf8_str_to_u32 `std::u32string utf8_str_to_u32(const std::string& s)`
- Defined: `core/moonshine-tts/src/utf8-utils.cpp:61`

### utf8_append_codepoint `void utf8_append_codepoint(std::string& out, char32_t cp)`
- Defined: `core/moonshine-tts/src/utf8-utils.cpp:74`

### utf8_split_codepoints `std::vector<std::string> utf8_split_codepoints(const std::string& utf8)`
- Defined: `core/moonshine-tts/src/utf8-utils.cpp:92`

### codepoint_is_unicode_word_neighbor_for_digits `bool codepoint_is_unicode_word_neighbor_for_digits(char32_t c)`
- Defined: `core/moonshine-tts/src/utf8-utils.cpp:182`

### utf8_codepoint_before_index `std::optional<char32_t> utf8_codepoint_before_index(const std::string& s,
                       ...`
- Defined: `core/moonshine-tts/src/utf8-utils.cpp:219`

### utf8_codepoint_at_index `std::optional<char32_t> utf8_codepoint_at_index(const std::string& s,
                           ...`
- Defined: `core/moonshine-tts/src/utf8-utils.cpp:236`

### digit_ascii_span_expandable_python_w `bool digit_ascii_span_expandable_python_w(const std::string& text,
                              ...`
- Defined: `core/moonshine-tts/src/utf8-utils.cpp:249`

### normalize_rule_based_dialect_cli_key `std::string normalize_rule_based_dialect_cli_key(std::string_view raw)`
- Defined: `core/moonshine-tts/src/utf8-utils.cpp:265`

### dedupe_dialect_ids_preserve_first `std::vector<std::string> dedupe_dialect_ids_preserve_first(
    std::vector<std::string> ids)`
- Defined: `core/moonshine-tts/src/utf8-utils.cpp:277`

## core/moonshine-tts/src/utf8-utils.h

### erase_utf8_substr `inline void erase_utf8_substr(std::string& s, std::string_view sub)`
- Defined: `core/moonshine-tts/src/utf8-utils.h:27`
- Doc: Remove every occurrence of *sub* from *s*.

### is_ascii_whitespace `inline bool is_ascii_whitespace(unsigned char c)`
- Defined: `core/moonshine-tts/src/utf8-utils.h:45`
- Doc: Trim ASCII whitespace only (same policy as legacy ``trim_copy_sv`` helpers in language files). IMPORTANT: uses an explic

### trim_ascii_ws_copy `inline std::string trim_ascii_ws_copy(std::string_view s)`
- Defined: `core/moonshine-tts/src/utf8-utils.h:49`

## core/moonshine-tts/src/zipvoice-custom-ops.cpp

### SoftplusPoly `inline float SoftplusPoly(float z)`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:51`

### ComputeTile `void ComputeTile(void* user_data, size_t idx)`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:77`

### SwooshKernel `explicit SwooshKernel(bool is_left)
      : offset_(is_left ? kLeftOffset : kRightOffset),
      ...`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:96`

### Compute `void Compute(OrtKernelContext* context)`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:99`

### SigmoidScalar `inline float SigmoidScalar(float v)`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:123`

### ComputeGluRow `void ComputeGluRow(void* user_data, size_t r)`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:131`

### Compute `void Compute(OrtKernelContext* context)`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:147`

### ComputeConvRow `void ComputeConvRow(void* user_data, size_t row)`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:183`

### Compute `void Compute(OrtKernelContext* context)`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:205`

### ComputeBiasNormRow `void ComputeBiasNormRow(void* user_data, size_t r)`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:258`

### Compute `void Compute(OrtKernelContext* context)`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:277`

### ComputeBypassRow `void ComputeBypassRow(void* user_data, size_t r)`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:310`

### Compute `void Compute(OrtKernelContext* context)`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:323`

### CreateKernel `void* CreateKernel(const OrtApi& /*api*/,
                     const OrtKernelInfo* /*info*/) const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:350`

### GetName `const char* GetName() const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:354`

### GetInputTypeCount `size_t GetInputTypeCount() const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:355`

### GetInputType `ONNXTensorElementDataType GetInputType(size_t /*index*/) const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:356`

### GetOutputTypeCount `size_t GetOutputTypeCount() const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:359`

### GetOutputType `ONNXTensorElementDataType GetOutputType(size_t /*index*/) const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:360`

### CreateKernel `void* CreateKernel(const OrtApi& /*api*/,
                     const OrtKernelInfo* /*info*/) const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:366`

### GetName `const char* GetName() const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:370`

### GetInputTypeCount `size_t GetInputTypeCount() const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:371`

### GetInputType `ONNXTensorElementDataType GetInputType(size_t /*index*/) const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:372`

### GetOutputTypeCount `size_t GetOutputTypeCount() const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:375`

### GetOutputType `ONNXTensorElementDataType GetOutputType(size_t /*index*/) const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:376`

### CreateKernel `void* CreateKernel(const OrtApi& /*api*/,
                     const OrtKernelInfo* /*info*/) const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:382`

### GetName `const char* GetName() const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:386`

### GetInputTypeCount `size_t GetInputTypeCount() const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:387`

### GetInputType `ONNXTensorElementDataType GetInputType(size_t /*index*/) const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:388`

### GetOutputTypeCount `size_t GetOutputTypeCount() const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:391`

### GetOutputType `ONNXTensorElementDataType GetOutputType(size_t /*index*/) const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:392`

### CreateKernel `void* CreateKernel(const OrtApi& /*api*/,
                     const OrtKernelInfo* /*info*/) const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:399`

### GetName `const char* GetName() const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:403`

### GetInputTypeCount `size_t GetInputTypeCount() const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:404`

### GetInputType `ONNXTensorElementDataType GetInputType(size_t /*index*/) const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:405`

### GetOutputTypeCount `size_t GetOutputTypeCount() const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:408`

### GetOutputType `ONNXTensorElementDataType GetOutputType(size_t /*index*/) const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:409`

### CreateKernel `void* CreateKernel(const OrtApi& /*api*/,
                     const OrtKernelInfo* /*info*/) const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:415`

### GetName `const char* GetName() const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:419`

### GetInputTypeCount `size_t GetInputTypeCount() const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:420`

### GetInputType `ONNXTensorElementDataType GetInputType(size_t /*index*/) const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:421`

### GetOutputTypeCount `size_t GetOutputTypeCount() const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:424`

### GetOutputType `ONNXTensorElementDataType GetOutputType(size_t /*index*/) const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:425`

### CreateKernel `void* CreateKernel(const OrtApi& /*api*/,
                     const OrtKernelInfo* /*info*/) const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:431`

### GetName `const char* GetName() const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:435`

### GetInputTypeCount `size_t GetInputTypeCount() const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:436`

### GetInputType `ONNXTensorElementDataType GetInputType(size_t /*index*/) const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:437`

### GetOutputTypeCount `size_t GetOutputTypeCount() const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:440`

### GetOutputType `ONNXTensorElementDataType GetOutputType(size_t /*index*/) const`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:441`

### zipvoice_domain `Ort::CustomOpDomain& zipvoice_domain()`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:457`
- Doc: One process-lifetime domain holding all ops; safe to Add() to multiple SessionOptions.

### zipvoice_register_custom_ops `void zipvoice_register_custom_ops(Ort::SessionOptions& opts)`
- Defined: `core/moonshine-tts/src/zipvoice-custom-ops.cpp:472`

## core/moonshine-tts/src/zipvoice-mel.cpp

### hz_to_bin_count `int hz_to_bin_count(int n_fft)`
- Defined: `core/moonshine-tts/src/zipvoice-mel.cpp:11`

### hz_to_mel_htk `double hz_to_mel_htk(double f)`
- Defined: `core/moonshine-tts/src/zipvoice-mel.cpp:13`

### mel_to_hz_htk `double mel_to_hz_htk(double m)`
- Defined: `core/moonshine-tts/src/zipvoice-mel.cpp:15`

### fft_radix2 `void fft_radix2(std::vector<double>& re, std::vector<double>& im)`
- Defined: `core/moonshine-tts/src/zipvoice-mel.cpp:21`
- Doc: Iterative radix-2 Cooley-Tukey FFT for power-of-two ``n`` (in-place, natural -> natural order).

### reflect_index `size_t reflect_index(long idx, long len)`
- Defined: `core/moonshine-tts/src/zipvoice-mel.cpp:64`
- Doc: Reflect index into [0, len) the same way torch ``pad(mode="reflect")`` mirrors without repeating the edge sample.

### VocosFbank `VocosFbank::VocosFbank()`
- Defined: `core/moonshine-tts/src/zipvoice-mel.cpp:80`

### num_frames_for `int VocosFbank::num_frames_for(size_t num_samples)`
- Defined: `core/moonshine-tts/src/zipvoice-mel.cpp:131`

### extract `std::vector<float> VocosFbank::extract(const std::vector<float>& samples,
                       ...`
- Defined: `core/moonshine-tts/src/zipvoice-mel.cpp:135`

## core/moonshine-tts/src/zipvoice-tts.cpp

### normalize_lang_key `std::string normalize_lang_key(std::string_view raw)`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:33`

### resolve_zipvoice_lang `void resolve_zipvoice_lang(const std::string& lang, std::string& g2p_dialect,
                   ...`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:49`
- Doc: English-only for now; structured so more locales can be added. Returns the MoonshineG2P dialect id and the ``normalize_g

### resample_linear `std::vector<float> resample_linear(const std::vector<float>& x, int src_sr,
                     ...`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:59`

### trim_edge_silence `std::vector<float> trim_edge_silence(const std::vector<float>& wav,
                             ...`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:87`
- Doc: Approximate ``remove_silence`` edge trimming (pydub ``remove_silence_edges``): drop leading and trailing samples below `

### rms_of `float rms_of(const std::vector<float>& x)`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:116`

### get_time_steps `std::vector<float> get_time_steps(int num_step, float t_shift)`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:130`
- Doc: ``get_time_steps``: linspace(0, 1, num_step + 1) then ``t_shift * t / (1 + (t_shift - 1) * t)``.

### load_session `Ort::Session load_session(std::string_view key, bool register_custom_ops,
                       ...`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:217`

### load_asset_bytes `std::vector<uint8_t> load_asset_bytes(std::string_view key)`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:255`

### ipa_text_to_token_ids `std::vector<int64_t> ipa_text_to_token_ids(const std::string& text)`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:283`

### ipa_to_token_ids `std::vector<int64_t> ipa_to_token_ids(const std::string& ipa)`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:288`

### Impl `explicit Impl(const ZipVoiceTTSOptions& opt)`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:305`

### speed `double speed() const`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:425`

### set_speed `void set_speed(double s)`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:427`

### normalize_audio `bool normalize_audio() const`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:434`

### set_normalize_audio `void set_normalize_audio(bool on)`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:435`

### output_volume `float output_volume() const`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:436`

### set_output_volume `void set_output_volume(float v)`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:437`

### run_text_encoder `std::vector<float> run_text_encoder(const std::vector<int64_t>& tokens,
                         ...`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:441`
- Doc: Runs the text encoder for one target-token chunk and returns text_condition [frames*feat_dim] (row-major), setting *out_

### sample_chunk `std::vector<float> sample_chunk(const std::vector<int64_t>& tokens,
                             ...`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:489`
- Doc: One flow-matching Euler solve for a chunk; returns predicted features [T_gen*feat_dim] (row-major).

### run_vocoder `std::vector<float> run_vocoder(const std::vector<float>& pred,
                                 i...`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:566`
- Doc: pred [T_gen*feat] row-major -> vocoder -> waveform.

### chunk_target_ids `std::vector<std::vector<int64_t>> chunk_target_ids(
      const std::vector<int64_t>& ids)`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:601`
- Doc: Split target token ids into chunks near a target size, preferring space-token boundaries.

### cross_fade_concat `static std::vector<float> cross_fade_concat(
      const std::vector<std::vector<float>>& chunks,...`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:650`

### synthesize `std::vector<float> synthesize(std::string_view text)`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:690`

### synthesize_from_ipa `std::vector<float> synthesize_from_ipa(std::string_view ipa)`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:694`

### synthesize_from_token_ids `std::vector<float> synthesize_from_token_ids(std::vector<int64_t> ids)`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:698`

### ZipVoiceTTS `ZipVoiceTTS::ZipVoiceTTS(const ZipVoiceTTSOptions& opt)
    : impl_(std::make_unique<Impl>(opt))`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:728`

### set_speed `void ZipVoiceTTS::set_speed(double speed)`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:734`

### speed `double ZipVoiceTTS::speed() const`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:736`

### normalize_audio `bool ZipVoiceTTS::normalize_audio() const`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:737`

### set_normalize_audio `void ZipVoiceTTS::set_normalize_audio(bool on)`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:738`

### output_volume `float ZipVoiceTTS::output_volume() const`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:741`

### set_output_volume `void ZipVoiceTTS::set_output_volume(float volume)`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:742`

### synthesize `std::vector<float> ZipVoiceTTS::synthesize(std::string_view text)`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:745`

### synthesize_from_ipa `std::vector<float> ZipVoiceTTS::synthesize_from_ipa(std::string_view ipa)`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:749`

### zipvoice_compress_long_pauses `std::vector<float> zipvoice_compress_long_pauses(const std::vector<float>& wav,
                 ...`
- Defined: `core/moonshine-tts/src/zipvoice-tts.cpp:753`

## core/moonshine-tts/src/zipvoice-voices.cpp

### zipvoice_find_builtin_voice `const ZipVoiceBuiltinVoice* zipvoice_find_builtin_voice(std::string_view id)`
- Defined: `core/moonshine-tts/src/zipvoice-voices.cpp:6`

### zipvoice_builtin_voice_pcm_to_float `std::vector<float> zipvoice_builtin_voice_pcm_to_float(
    const ZipVoiceBuiltinVoice& voice)`
- Defined: `core/moonshine-tts/src/zipvoice-voices.cpp:17`

## core/moonshine-tts/tests/arabic-rule-g2p-test.cpp

### TEST_CASE `TEST_CASE(
    "arabic rule g2p: first 100 wiki lines match reference IPA when assets and "
    "...`
- Defined: `core/moonshine-tts/tests/arabic-rule-g2p-test.cpp:8`

## core/moonshine-tts/tests/chinese-rule-g2p-test.cpp

### make_temp_tsv `std::filesystem::path make_temp_tsv(const char* contents)`
- Defined: `core/moonshine-tts/tests/chinese-rule-g2p-test.cpp:20`

### TEST_CASE `TEST_CASE("chinese: dialect_resolves_to_chinese_rules")`
- Defined: `core/moonshine-tts/tests/chinese-rule-g2p-test.cpp:32`

### TEST_CASE `TEST_CASE(
    "chinese: lexicon lookup and Arabic numeral expansion via per-char Han "
    "IPA")`
- Defined: `core/moonshine-tts/tests/chinese-rule-g2p-test.cpp:43`

## core/moonshine-tts/tests/chinese-tok-pos-onnx-test.cpp

### TEST_CASE `TEST_CASE("chinese tok pos: single sentence matches reference file")`
- Defined: `core/moonshine-tts/tests/chinese-tok-pos-onnx-test.cpp:9`

### TEST_CASE `TEST_CASE(
    "chinese tok pos: first 100 wiki lines match reference when assets and "
    "gold...`
- Defined: `core/moonshine-tts/tests/chinese-tok-pos-onnx-test.cpp:26`

## core/moonshine-tts/tests/cmudict-tsv-test.cpp

### TEST_CASE `TEST_CASE("cmudict-tsv load and lookup")`
- Defined: `core/moonshine-tts/tests/cmudict-tsv-test.cpp:10`

## core/moonshine-tts/tests/dutch-rule-g2p-test.cpp

### make_temp_tsv `std::filesystem::path make_temp_tsv(const char* contents)`
- Defined: `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp:16`

### TEST_CASE `TEST_CASE("dutch: lowercase homograph overrides capitalized")`
- Defined: `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp:28`

### TEST_CASE `TEST_CASE(
    "dutch: lexicon stress not shifted by vocoder (unlike German policy)")`
- Defined: `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp:37`

### TEST_CASE `TEST_CASE("dutch: rule IPA gets vocoder stress when enabled")`
- Defined: `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp:49`

### TEST_CASE `TEST_CASE("dutch: normalize_ipa_stress_for_vocoder idempotent")`
- Defined: `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp:58`

### TEST_CASE `TEST_CASE("dutch: dialect_resolves_to_dutch_rules")`
- Defined: `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp:69`

### TEST_CASE `TEST_CASE("dutch: optional real dict fiets matches Python when data present")`
- Defined: `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp:78`

### TEST_CASE `TEST_CASE(
    "dutch: wiki-text first 100 lines match reference IPA when data and golden "
    "...`
- Defined: `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp:92`

## core/moonshine-tts/tests/english-hand-oov-test.cpp

### TEST_CASE `TEST_CASE("english_number_token_ipa")`
- Defined: `core/moonshine-tts/tests/english-hand-oov-test.cpp:12`

### TEST_CASE `TEST_CASE("english_hand_oov_rules_ipa nonempty")`
- Defined: `core/moonshine-tts/tests/english-hand-oov-test.cpp:19`

## core/moonshine-tts/tests/english-rule-g2p-test.cpp

### resolve_en_dict `std::filesystem::path resolve_en_dict()`
- Defined: `core/moonshine-tts/tests/english-rule-g2p-test.cpp:14`

### TEST_CASE `TEST_CASE("english: dialect_resolves_to_english_rules")`
- Defined: `core/moonshine-tts/tests/english-rule-g2p-test.cpp:21`

### TEST_CASE `TEST_CASE("english: tomato heteronym picks US vs British by dialect flag")`
- Defined: `core/moonshine-tts/tests/english-rule-g2p-test.cpp:37`

### TEST_CASE `TEST_CASE(
    "english: wiki-text first 100 lines match reference IPA when data and "
    "golde...`
- Defined: `core/moonshine-tts/tests/english-rule-g2p-test.cpp:50`

## core/moonshine-tts/tests/file-information-test.cpp

### TEST_CASE `TEST_CASE("FileInformation default memory fields")`
- Defined: `core/moonshine-tts/tests/file-information-test.cpp:10`

### TEST_CASE `TEST_CASE("FileInformationMap set_path and contains")`
- Defined: `core/moonshine-tts/tests/file-information-test.cpp:17`

### TEST_CASE `TEST_CASE("FileInformationMap erase_key")`
- Defined: `core/moonshine-tts/tests/file-information-test.cpp:27`

### TEST_CASE `TEST_CASE("FileInformationMap::parse_file_list")`
- Defined: `core/moonshine-tts/tests/file-information-test.cpp:34`

### TEST_CASE `TEST_CASE("FileInformationMap::parse_file_list null key_list throws")`
- Defined: `core/moonshine-tts/tests/file-information-test.cpp:59`

### TEST_CASE `TEST_CASE("FileInformationMap::parse_file_list memory size mismatch throws")`
- Defined: `core/moonshine-tts/tests/file-information-test.cpp:65`

## core/moonshine-tts/tests/french-rule-g2p-test.cpp

### strip_stress `std::string strip_stress(std::string s)`
- Defined: `core/moonshine-tts/tests/french-rule-g2p-test.cpp:15`

### french_dict_present `bool french_dict_present()`
- Defined: `core/moonshine-tts/tests/french-rule-g2p-test.cpp:35`

### TEST_CASE `TEST_CASE("french: dialect_resolves_to_french_rules")`
- Defined: `core/moonshine-tts/tests/french-rule-g2p-test.cpp:42`

### TEST_CASE `TEST_CASE("french: ensure_french_nuclear_stress")`
- Defined: `core/moonshine-tts/tests/french-rule-g2p-test.cpp:51`

### TEST_CASE `TEST_CASE("french: liaison les amis" * doctest::skip(!french_dict_present()))`
- Defined: `core/moonshine-tts/tests/french-rule-g2p-test.cpp:57`

### TEST_CASE `TEST_CASE("french: En 1891 cardinal expansion" *
          doctest::skip(!french_dict_present()))`
- Defined: `core/moonshine-tts/tests/french-rule-g2p-test.cpp:69`

### TEST_CASE `TEST_CASE("french: punctuation keeps space before next word" *
          doctest::skip(!french_di...`
- Defined: `core/moonshine-tts/tests/french-rule-g2p-test.cpp:82`

### TEST_CASE `TEST_CASE(
    "french: hyphenated OOV allez-vous matches Python (UTF-8 trim + stress)" *
    doc...`
- Defined: `core/moonshine-tts/tests/french-rule-g2p-test.cpp:93`

### TEST_CASE `TEST_CASE("french: uppercase accented letters in words (Saint-Étienne)" *
          doctest::skip...`
- Defined: `core/moonshine-tts/tests/french-rule-g2p-test.cpp:104`

### TEST_CASE `TEST_CASE(
    "french: wiki-text first 100 lines match reference IPA when data and "
    "golden...`
- Defined: `core/moonshine-tts/tests/french-rule-g2p-test.cpp:114`

## core/moonshine-tts/tests/german-rule-g2p-test.cpp

### make_temp_tsv `std::filesystem::path make_temp_tsv(const char* contents)`
- Defined: `core/moonshine-tts/tests/german-rule-g2p-test.cpp:16`

### TEST_CASE `TEST_CASE("german: lowercase homograph overrides capitalized")`
- Defined: `core/moonshine-tts/tests/german-rule-g2p-test.cpp:28`

### TEST_CASE `TEST_CASE(
    "german: lexicon entry with syllable-initial stress gets vocoder shift")`
- Defined: `core/moonshine-tts/tests/german-rule-g2p-test.cpp:37`

### TEST_CASE `TEST_CASE(
    "german: syllable-initial stress preserved when vocoder_stress false")`
- Defined: `core/moonshine-tts/tests/german-rule-g2p-test.cpp:45`

### TEST_CASE `TEST_CASE("german: OOV rules machen")`
- Defined: `core/moonshine-tts/tests/german-rule-g2p-test.cpp:55`

### TEST_CASE `TEST_CASE("german: normalize_ipa_stress_for_vocoder idempotent")`
- Defined: `core/moonshine-tts/tests/german-rule-g2p-test.cpp:67`

### TEST_CASE `TEST_CASE("german: dialect_resolves_to_german_rules")`
- Defined: `core/moonshine-tts/tests/german-rule-g2p-test.cpp:75`

### TEST_CASE `TEST_CASE("german: text token preserves comma")`
- Defined: `core/moonshine-tts/tests/german-rule-g2p-test.cpp:84`

### TEST_CASE `TEST_CASE(
    "german: Im Jahr 1891 matches reference IPA when data and golden exist")`
- Defined: `core/moonshine-tts/tests/german-rule-g2p-test.cpp:92`

### TEST_CASE `TEST_CASE(
    "german: wiki-text first 100 lines match reference IPA when data and "
    "golden...`
- Defined: `core/moonshine-tts/tests/german-rule-g2p-test.cpp:108`

## core/moonshine-tts/tests/heteronym-context-test.cpp

### TEST_CASE `TEST_CASE("heteronym_centered_context_window_cells short pad")`
- Defined: `core/moonshine-tts/tests/heteronym-context-test.cpp:9`

### TEST_CASE `TEST_CASE("heteronym_centered_context_window_cells crop")`
- Defined: `core/moonshine-tts/tests/heteronym-context-test.cpp:19`

## core/moonshine-tts/tests/hindi-rule-g2p-test.cpp

### check_wiki_parity `void check_wiki_parity(const std::filesystem::path& wiki,
                       const std::files...`
- Defined: `core/moonshine-tts/tests/hindi-rule-g2p-test.cpp:16`

### TEST_CASE `TEST_CASE("hindi: dialect_resolves_to_hindi_rules")`
- Defined: `core/moonshine-tts/tests/hindi-rule-g2p-test.cpp:36`

### TEST_CASE `TEST_CASE("hindi: कमल and मैं match reference IPA when golden exists")`
- Defined: `core/moonshine-tts/tests/hindi-rule-g2p-test.cpp:44`

### TEST_CASE `TEST_CASE("hindi: expand_cardinal_digits_to_hindi_words")`
- Defined: `core/moonshine-tts/tests/hindi-rule-g2p-test.cpp:59`

### TEST_CASE `TEST_CASE(
    "hindi: wiki-text first 100 lines match reference IPA when data and golden "
    "...`
- Defined: `core/moonshine-tts/tests/hindi-rule-g2p-test.cpp:65`

## core/moonshine-tts/tests/ipa-postprocess-test.cpp

### TEST_CASE `TEST_CASE("levenshtein_distance")`
- Defined: `core/moonshine-tts/tests/ipa-postprocess-test.cpp:9`

### TEST_CASE `TEST_CASE("pick_closest_cmudict_ipa single")`
- Defined: `core/moonshine-tts/tests/ipa-postprocess-test.cpp:16`

### TEST_CASE `TEST_CASE("match_prediction_to_cmudict_ipa")`
- Defined: `core/moonshine-tts/tests/ipa-postprocess-test.cpp:21`

### TEST_CASE `TEST_CASE("normalize_g2p_ipa_for_piper_engines")`
- Defined: `core/moonshine-tts/tests/ipa-postprocess-test.cpp:28`

### TEST_CASE `TEST_CASE("repair_ascii_c_combining_cedilla_to_ccedilla_utf8")`
- Defined: `core/moonshine-tts/tests/ipa-postprocess-test.cpp:44`

### TEST_CASE `TEST_CASE("normalize_g2p_ipa_for_piper NFC plus shared rules")`
- Defined: `core/moonshine-tts/tests/ipa-postprocess-test.cpp:56`

### TEST_CASE `TEST_CASE("coerce_unknown_ipa_chars_to_piper_inventory toy map")`
- Defined: `core/moonshine-tts/tests/ipa-postprocess-test.cpp:65`

### TEST_CASE `TEST_CASE("ipa_to_piper_ready without coercion")`
- Defined: `core/moonshine-tts/tests/ipa-postprocess-test.cpp:77`

### TEST_CASE `TEST_CASE("normalize_g2p_ipa_for_piper Korean rule IPA toward eSpeak-ng")`
- Defined: `core/moonshine-tts/tests/ipa-postprocess-test.cpp:88`

### TEST_CASE `TEST_CASE("normalize_russian_ipa_piper_style")`
- Defined: `core/moonshine-tts/tests/ipa-postprocess-test.cpp:110`

### TEST_CASE `TEST_CASE("normalize_german_ipa_piper_style")`
- Defined: `core/moonshine-tts/tests/ipa-postprocess-test.cpp:166`

### TEST_CASE `TEST_CASE("normalize_g2p_ipa_for_piper German applies piper-style pass")`
- Defined: `core/moonshine-tts/tests/ipa-postprocess-test.cpp:189`

### TEST_CASE `TEST_CASE("normalize_chinese_ipa_piper_style full pipeline single syllables")`
- Defined: `core/moonshine-tts/tests/ipa-postprocess-test.cpp:197`

### TEST_CASE `TEST_CASE("normalize_chinese_ipa_piper_style retroflexes")`
- Defined: `core/moonshine-tts/tests/ipa-postprocess-test.cpp:222`

### TEST_CASE `TEST_CASE("normalize_chinese_ipa_piper_style dental sibilants")`
- Defined: `core/moonshine-tts/tests/ipa-postprocess-test.cpp:239`

### TEST_CASE `TEST_CASE("normalize_chinese_ipa_piper_style velar fricative")`
- Defined: `core/moonshine-tts/tests/ipa-postprocess-test.cpp:246`

### TEST_CASE `TEST_CASE("normalize_chinese_ipa_piper_style er/erhua")`
- Defined: `core/moonshine-tts/tests/ipa-postprocess-test.cpp:253`

### TEST_CASE `TEST_CASE("normalize_chinese_ipa_piper_style mid vowel")`
- Defined: `core/moonshine-tts/tests/ipa-postprocess-test.cpp:260`

### TEST_CASE `TEST_CASE("normalize_chinese_ipa_piper_style -ong and -uo finals")`
- Defined: `core/moonshine-tts/tests/ipa-postprocess-test.cpp:273`

### TEST_CASE `TEST_CASE("normalize_chinese_ipa_piper_style ü-finals")`
- Defined: `core/moonshine-tts/tests/ipa-postprocess-test.cpp:286`

### TEST_CASE `TEST_CASE(
    "normalize_chinese_ipa_piper_style tone repositioning before nasals")`
- Defined: `core/moonshine-tts/tests/ipa-postprocess-test.cpp:300`

### TEST_CASE `TEST_CASE("normalize_chinese_ipa_piper_style aspiration")`
- Defined: `core/moonshine-tts/tests/ipa-postprocess-test.cpp:320`

### TEST_CASE `TEST_CASE("normalize_g2p_ipa_for_piper Chinese wired up for zh keys")`
- Defined: `core/moonshine-tts/tests/ipa-postprocess-test.cpp:333`

## core/moonshine-tts/tests/italian-rule-g2p-test.cpp

### make_temp_tsv `std::filesystem::path make_temp_tsv(const char* contents)`
- Defined: `core/moonshine-tts/tests/italian-rule-g2p-test.cpp:16`

### TEST_CASE `TEST_CASE("italian: dialect_resolves_to_italian_rules")`
- Defined: `core/moonshine-tts/tests/italian-rule-g2p-test.cpp:28`

### TEST_CASE `TEST_CASE("italian: lowercase homograph overrides capitalized")`
- Defined: `core/moonshine-tts/tests/italian-rule-g2p-test.cpp:37`

### TEST_CASE `TEST_CASE("italian: lexicon stress not shifted by vocoder")`
- Defined: `core/moonshine-tts/tests/italian-rule-g2p-test.cpp:46`

### TEST_CASE `TEST_CASE("italian: c'è matches reference IPA when data and golden exist")`
- Defined: `core/moonshine-tts/tests/italian-rule-g2p-test.cpp:55`

### TEST_CASE `TEST_CASE(
    "italian: wiki-text first 100 lines match reference IPA when data and "
    "golde...`
- Defined: `core/moonshine-tts/tests/italian-rule-g2p-test.cpp:73`

## core/moonshine-tts/tests/japanese-onnx-g2p-test.cpp

### TEST_CASE `TEST_CASE(
    "japanese onnx g2p: first 100 wiki IPA lines match reference when assets "
    "an...`
- Defined: `core/moonshine-tts/tests/japanese-onnx-g2p-test.cpp:9`

## core/moonshine-tts/tests/japanese-tok-pos-onnx-test.cpp

### TEST_CASE `TEST_CASE("japanese tok pos: single sentence matches reference file")`
- Defined: `core/moonshine-tts/tests/japanese-tok-pos-onnx-test.cpp:9`

### TEST_CASE `TEST_CASE(
    "japanese tok pos: long input is split and does not exceed model length")`
- Defined: `core/moonshine-tts/tests/japanese-tok-pos-onnx-test.cpp:27`

### TEST_CASE `TEST_CASE(
    "japanese tok pos: first 100 wiki lines match reference when assets and "
    "gol...`
- Defined: `core/moonshine-tts/tests/japanese-tok-pos-onnx-test.cpp:47`

## core/moonshine-tts/tests/json-config-test.cpp

### TEST_CASE `TEST_CASE("load_oov_tables from onnx-config.json")`
- Defined: `core/moonshine-tts/tests/json-config-test.cpp:10`

## core/moonshine-tts/tests/korean-rule-g2p-test.cpp

### ko_dict_path `std::filesystem::path ko_dict_path()`
- Defined: `core/moonshine-tts/tests/korean-rule-g2p-test.cpp:18`

### TEST_CASE `TEST_CASE("korean: dialect_resolves_to_korean_rules")`
- Defined: `core/moonshine-tts/tests/korean-rule-g2p-test.cpp:24`

### TEST_CASE `TEST_CASE(
    "korean: normalize strips all combining marks including tense and "
    "unreleased")`
- Defined: `core/moonshine-tts/tests/korean-rule-g2p-test.cpp:33`

### TEST_CASE `TEST_CASE("korean: int_to_sino_korean_hangul")`
- Defined: `core/moonshine-tts/tests/korean-rule-g2p-test.cpp:66`

### TEST_CASE `TEST_CASE("korean: korean_reading_fragments_from_ascii_numeral_token")`
- Defined: `core/moonshine-tts/tests/korean-rule-g2p-test.cpp:78`

### TEST_CASE `TEST_CASE("korean: G2P examples with data/ko/dict.tsv")`
- Defined: `core/moonshine-tts/tests/korean-rule-g2p-test.cpp:102`

## core/moonshine-tts/tests/korean-tok-pos-onnx-test.cpp

### TEST_CASE `TEST_CASE("korean tok pos: single sentence matches reference file")`
- Defined: `core/moonshine-tts/tests/korean-tok-pos-onnx-test.cpp:9`

### TEST_CASE `TEST_CASE(
    "korean tok pos: first 100 wiki lines match reference when assets and "
    "golde...`
- Defined: `core/moonshine-tts/tests/korean-tok-pos-onnx-test.cpp:26`

## core/moonshine-tts/tests/moonshine-g2p-options-test.cpp

### TEST_CASE `TEST_CASE("MoonshineG2POptions default constructor seeds canonical file keys")`
- Defined: `core/moonshine-tts/tests/moonshine-g2p-options-test.cpp:18`

### TEST_CASE `TEST_CASE(
    "MoonshineG2POptions relative_asset_path falls back when key absent")`
- Defined: `core/moonshine-tts/tests/moonshine-g2p-options-test.cpp:34`

### TEST_CASE `TEST_CASE("MoonshineG2POptions parse_options rejects unknown keys")`
- Defined: `core/moonshine-tts/tests/moonshine-g2p-options-test.cpp:42`

### TEST_CASE `TEST_CASE("MoonshineG2POptions parse_options accepts every known option")`
- Defined: `core/moonshine-tts/tests/moonshine-g2p-options-test.cpp:48`

### TEST_CASE `TEST_CASE(
    "MoonshineG2POptions parse_options empty path clears canonical entry")`
- Defined: `core/moonshine-tts/tests/moonshine-g2p-options-test.cpp:124`

### TEST_CASE `TEST_CASE("MoonshineG2POptions option names are case-insensitive")`
- Defined: `core/moonshine-tts/tests/moonshine-g2p-options-test.cpp:133`

## core/moonshine-tts/tests/moonshine-tts-options-test.cpp

### TEST_CASE `TEST_CASE("MoonshineTTSOptions parse_options ort_providers")`
- Defined: `core/moonshine-tts/tests/moonshine-tts-options-test.cpp:11`

## core/moonshine-tts/tests/moonshine-tts-speed-test.cpp

### bundled_tts_data_present `bool bundled_tts_data_present(const std::filesystem::path& root)`
- Defined: `core/moonshine-tts/tests/moonshine-tts-speed-test.cpp:13`

### TEST_CASE `TEST_CASE(
    "MoonshineTTS Kokoro: per-call speed changes duration and restores "
    "default")`
- Defined: `core/moonshine-tts/tests/moonshine-tts-speed-test.cpp:23`

### TEST_CASE `TEST_CASE("MoonshineTTS Piper: per-call speed reduces duration vs baseline")`
- Defined: `core/moonshine-tts/tests/moonshine-tts-speed-test.cpp:46`

## core/moonshine-tts/tests/onnx-g2p-smoke-test.cpp

### TEST_CASE `TEST_CASE(
    "MoonshineG2P en_us rule-based when MOONSHINE_TTS_MODELS_ROOT is set")`
- Defined: `core/moonshine-tts/tests/onnx-g2p-smoke-test.cpp:12`

### TEST_CASE `TEST_CASE("MoonshineG2P ja-JP when data/ja assets exist under repo")`
- Defined: `core/moonshine-tts/tests/onnx-g2p-smoke-test.cpp:32`

## core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp

### make_temp_tsv `std::filesystem::path make_temp_tsv(const char* contents)`
- Defined: `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp:16`

### TEST_CASE `TEST_CASE("portuguese: dialect flags")`
- Defined: `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp:28`

### TEST_CASE `TEST_CASE("portuguese: lowercase homograph overrides capitalized")`
- Defined: `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp:39`

### TEST_CASE `TEST_CASE("portuguese: lexicon stress not shifted by vocoder")`
- Defined: `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp:48`

### TEST_CASE `TEST_CASE("portuguese: casa matches reference IPA when data and golden exist")`
- Defined: `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp:57`

### TEST_CASE `TEST_CASE(
    "portuguese: wiki-text first 100 lines pt_br match reference IPA when data "
    "...`
- Defined: `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp:72`

### TEST_CASE `TEST_CASE(
    "portuguese: wiki-text first 100 lines pt_pt match reference IPA when data "
    "...`
- Defined: `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp:98`

## core/moonshine-tts/tests/rule-g2p-test-support.h

### repo_root_from_tests_cpp `inline std::filesystem::path repo_root_from_tests_cpp(
    const char* tests_cpp_file)`
- Defined: `core/moonshine-tts/tests/rule-g2p-test-support.h:21`
- Doc: Directory that contains ``data/`` (lexicons, ONNX assets) and usually ``models/``. Prefers the moonshine-tts tree when i

### tests_data_dir `inline std::filesystem::path tests_data_dir(
    const std::filesystem::path& repo_root)`
- Defined: `core/moonshine-tts/tests/rule-g2p-test-support.h:34`
- Doc: Pre-generated parity lines: ``<tts>/tests/data`` when built in-tree, or legacy monorepo paths.

### split_unix_lines `inline std::vector<std::string> split_unix_lines(std::string block)`
- Defined: `core/moonshine-tts/tests/rule-g2p-test-support.h:52`

### load_ref_text_trimmed `inline std::string load_ref_text_trimmed(const std::filesystem::path& p)`
- Defined: `core/moonshine-tts/tests/rule-g2p-test-support.h:65`

### load_ref_lines `inline std::vector<std::string> load_ref_lines(const std::filesystem::path& p)`
- Defined: `core/moonshine-tts/tests/rule-g2p-test-support.h:75`

### ref_lines_prefix `inline std::vector<std::string> ref_lines_prefix(
    const std::filesystem::path& golden, std::s...`
- Defined: `core/moonshine-tts/tests/rule-g2p-test-support.h:85`
- Doc: Use the first *n* lines from a golden file (generated for up to 100 wiki lines).

### read_text_first_lines `inline std::vector<std::string> read_text_first_lines(
    const std::filesystem::path& p, std::s...`
- Defined: `core/moonshine-tts/tests/rule-g2p-test-support.h:95`

### moonshine_tts_bundled_data_dir_relative `inline std::filesystem::path moonshine_tts_bundled_data_dir_relative()`
- Defined: `core/moonshine-tts/tests/rule-g2p-test-support.h:114`
- Doc: Path to the bundled ``moonshine-tts`` data tree, relative to the monorepo repository root. Tests that use this path must

## core/moonshine-tts/tests/russian-rule-g2p-test.cpp

### make_temp_tsv `std::filesystem::path make_temp_tsv(const char* contents)`
- Defined: `core/moonshine-tts/tests/russian-rule-g2p-test.cpp:20`

### TEST_CASE `TEST_CASE("russian: dialect_resolves_to_russian_rules")`
- Defined: `core/moonshine-tts/tests/russian-rule-g2p-test.cpp:32`

### TEST_CASE `TEST_CASE("russian: lowercase homograph overrides capitalized")`
- Defined: `core/moonshine-tts/tests/russian-rule-g2p-test.cpp:41`

### TEST_CASE `TEST_CASE("russian: litva matches reference IPA when data and golden exist")`
- Defined: `core/moonshine-tts/tests/russian-rule-g2p-test.cpp:68`
- Doc: endif

### TEST_CASE `TEST_CASE(
    "russian: Cyrillic preposition plus 1891 matches reference IPA when data "
    "an...`
- Defined: `core/moonshine-tts/tests/russian-rule-g2p-test.cpp:83`

### TEST_CASE `TEST_CASE(
    "russian: wiki-text first 100 lines match reference IPA when data and "
    "golde...`
- Defined: `core/moonshine-tts/tests/russian-rule-g2p-test.cpp:101`

## core/moonshine-tts/tests/spanish-rule-g2p-test.cpp

### check_wiki_parity `void check_wiki_parity(const std::filesystem::path& wiki,
                       const std::files...`
- Defined: `core/moonshine-tts/tests/spanish-rule-g2p-test.cpp:15`

### TEST_CASE `TEST_CASE("spanish: En 1891 matches reference IPA when golden exists")`
- Defined: `core/moonshine-tts/tests/spanish-rule-g2p-test.cpp:34`

### TEST_CASE `TEST_CASE("spanish: dialect ids include es-MX and es-ES")`
- Defined: `core/moonshine-tts/tests/spanish-rule-g2p-test.cpp:46`

### TEST_CASE `TEST_CASE(
    "spanish: wiki-text first 100 lines es_mx match reference IPA when data "
    "and...`
- Defined: `core/moonshine-tts/tests/spanish-rule-g2p-test.cpp:52`

### TEST_CASE `TEST_CASE(
    "spanish: wiki-text first 100 lines es_es match reference IPA when data "
    "and...`
- Defined: `core/moonshine-tts/tests/spanish-rule-g2p-test.cpp:64`

## core/moonshine-tts/tests/text-normalize-test.cpp

### TEST_CASE `TEST_CASE("split_text_to_words")`
- Defined: `core/moonshine-tts/tests/text-normalize-test.cpp:7`

### TEST_CASE `TEST_CASE("normalize_word_for_lookup")`
- Defined: `core/moonshine-tts/tests/text-normalize-test.cpp:15`

### TEST_CASE `TEST_CASE("normalize_grapheme_key strips alternate suffix")`
- Defined: `core/moonshine-tts/tests/text-normalize-test.cpp:20`

## core/moonshine-tts/tests/turkish-rule-g2p-test.cpp

### check_wiki_parity `void check_wiki_parity(const std::filesystem::path& wiki,
                       const std::files...`
- Defined: `core/moonshine-tts/tests/turkish-rule-g2p-test.cpp:15`

### TEST_CASE `TEST_CASE("turkish: dağ and değer match reference IPA when golden exists")`
- Defined: `core/moonshine-tts/tests/turkish-rule-g2p-test.cpp:33`

### TEST_CASE `TEST_CASE("turkish: dialect ids include tr and tr-TR")`
- Defined: `core/moonshine-tts/tests/turkish-rule-g2p-test.cpp:45`

### TEST_CASE `TEST_CASE(
    "turkish: wiki-text first 100 lines match reference IPA when data and "
    "golde...`
- Defined: `core/moonshine-tts/tests/turkish-rule-g2p-test.cpp:51`

## core/moonshine-tts/tests/ukrainian-rule-g2p-test.cpp

### check_wiki_parity `void check_wiki_parity(const std::filesystem::path& wiki,
                       const std::files...`
- Defined: `core/moonshine-tts/tests/ukrainian-rule-g2p-test.cpp:15`

### TEST_CASE `TEST_CASE("ukrainian: m'ясо and кінь match reference IPA when golden exists")`
- Defined: `core/moonshine-tts/tests/ukrainian-rule-g2p-test.cpp:33`

### TEST_CASE `TEST_CASE("ukrainian: dialect ids include uk and uk-UA")`
- Defined: `core/moonshine-tts/tests/ukrainian-rule-g2p-test.cpp:45`

### TEST_CASE `TEST_CASE(
    "ukrainian: wiki-text first 100 lines match reference IPA when data and "
    "gol...`
- Defined: `core/moonshine-tts/tests/ukrainian-rule-g2p-test.cpp:51`

## core/moonshine-tts/tests/utf8-utils-test.cpp

### TEST_CASE `TEST_CASE("utf8_split_codepoints ascii")`
- Defined: `core/moonshine-tts/tests/utf8-utils-test.cpp:7`

### TEST_CASE `TEST_CASE("utf8_split_codepoints two-byte")`
- Defined: `core/moonshine-tts/tests/utf8-utils-test.cpp:15`

### TEST_CASE `TEST_CASE("utf8_find_token_codepoints")`
- Defined: `core/moonshine-tts/tests/utf8-utils-test.cpp:22`

### TEST_CASE `TEST_CASE("digit_ascii_span_expandable_python_w")`
- Defined: `core/moonshine-tts/tests/utf8-utils-test.cpp:30`

## core/moonshine-tts/tests/vietnamese-rule-g2p-test.cpp

### vi_dict_path `std::filesystem::path vi_dict_path()`
- Defined: `core/moonshine-tts/tests/vietnamese-rule-g2p-test.cpp:17`

### TEST_CASE `TEST_CASE("vietnamese: dialect_resolves_to_vietnamese_rules")`
- Defined: `core/moonshine-tts/tests/vietnamese-rule-g2p-test.cpp:23`

### TEST_CASE `TEST_CASE("vietnamese: syllable OOV parity with Python samples")`
- Defined: `core/moonshine-tts/tests/vietnamese-rule-g2p-test.cpp:32`

### TEST_CASE `TEST_CASE("vietnamese: lexicon line with data/vi/dict.tsv")`
- Defined: `core/moonshine-tts/tests/vietnamese-rule-g2p-test.cpp:41`

## core/moonshine-tts/tests/zipvoice-tts-test.cpp

### TEST_CASE `TEST_CASE("zipvoice-builtin-voices")`
- Defined: `core/moonshine-tts/tests/zipvoice-tts-test.cpp:13`

### TEST_CASE `TEST_CASE("zipvoice-vocos-fbank")`
- Defined: `core/moonshine-tts/tests/zipvoice-tts-test.cpp:45`

### TEST_CASE `TEST_CASE("zipvoice-compress-long-pauses")`
- Defined: `core/moonshine-tts/tests/zipvoice-tts-test.cpp:66`

## core/moonshine-tts/tools/arabic-rule-g2p-cli.cpp

### usage `void usage(const char* argv0)`
- Defined: `core/moonshine-tts/tools/arabic-rule-g2p-cli.cpp:11`

### read_all_stdin `std::string read_all_stdin()`
- Defined: `core/moonshine-tts/tools/arabic-rule-g2p-cli.cpp:18`

### main `int main(int argc, char** argv)`
- Defined: `core/moonshine-tts/tools/arabic-rule-g2p-cli.cpp:26`

## core/moonshine-tts/tools/chinese-rule-g2p-cli.cpp

### usage `void usage(const char* argv0)`
- Defined: `core/moonshine-tts/tools/chinese-rule-g2p-cli.cpp:12`

### read_all_stdin `std::string read_all_stdin()`
- Defined: `core/moonshine-tts/tools/chinese-rule-g2p-cli.cpp:19`

### main `int main(int argc, char** argv)`
- Defined: `core/moonshine-tts/tools/chinese-rule-g2p-cli.cpp:27`

## core/moonshine-tts/tools/dutch-g2p-batch-cli.cpp

### usage `void usage(const char* argv0)`
- Defined: `core/moonshine-tts/tools/dutch-g2p-batch-cli.cpp:14`

### trim_sv `std::string trim_sv(std::string s)`
- Defined: `core/moonshine-tts/tools/dutch-g2p-batch-cli.cpp:29`

### read_all_stdin `std::string read_all_stdin()`
- Defined: `core/moonshine-tts/tools/dutch-g2p-batch-cli.cpp:41`

### main `int main(int argc, char** argv)`
- Defined: `core/moonshine-tts/tools/dutch-g2p-batch-cli.cpp:49`

## core/moonshine-tts/tools/dutch-rule-g2p-cli.cpp

### usage `void usage(const char* argv0)`
- Defined: `core/moonshine-tts/tools/dutch-rule-g2p-cli.cpp:12`

### read_all_stdin `std::string read_all_stdin()`
- Defined: `core/moonshine-tts/tools/dutch-rule-g2p-cli.cpp:21`

### main `int main(int argc, char** argv)`
- Defined: `core/moonshine-tts/tools/dutch-rule-g2p-cli.cpp:29`

## core/moonshine-tts/tools/french-g2p-batch-cli.cpp

### usage `void usage(const char* argv0)`
- Defined: `core/moonshine-tts/tools/french-g2p-batch-cli.cpp:14`

### trim_sv `std::string trim_sv(std::string s)`
- Defined: `core/moonshine-tts/tools/french-g2p-batch-cli.cpp:30`

### read_all_stdin `std::string read_all_stdin()`
- Defined: `core/moonshine-tts/tools/french-g2p-batch-cli.cpp:42`

### main `int main(int argc, char** argv)`
- Defined: `core/moonshine-tts/tools/french-g2p-batch-cli.cpp:50`

## core/moonshine-tts/tools/german-rule-g2p-cli.cpp

### usage `void usage(const char* argv0)`
- Defined: `core/moonshine-tts/tools/german-rule-g2p-cli.cpp:12`

### read_all_stdin `std::string read_all_stdin()`
- Defined: `core/moonshine-tts/tools/german-rule-g2p-cli.cpp:20`

### main `int main(int argc, char** argv)`
- Defined: `core/moonshine-tts/tools/german-rule-g2p-cli.cpp:28`

## core/moonshine-tts/tools/hindi-rule-g2p-cli.cpp

### usage `void usage(const char* argv0)`
- Defined: `core/moonshine-tts/tools/hindi-rule-g2p-cli.cpp:11`

### read_all_stdin `std::string read_all_stdin()`
- Defined: `core/moonshine-tts/tools/hindi-rule-g2p-cli.cpp:19`

### main `int main(int argc, char** argv)`
- Defined: `core/moonshine-tts/tools/hindi-rule-g2p-cli.cpp:27`

## core/moonshine-tts/tools/italian-rule-g2p-cli.cpp

### usage `void usage(const char* argv0)`
- Defined: `core/moonshine-tts/tools/italian-rule-g2p-cli.cpp:12`

### read_all_stdin `std::string read_all_stdin()`
- Defined: `core/moonshine-tts/tools/italian-rule-g2p-cli.cpp:21`

### main `int main(int argc, char** argv)`
- Defined: `core/moonshine-tts/tools/italian-rule-g2p-cli.cpp:29`

## core/moonshine-tts/tools/japanese-onnx-g2p-cli.cpp

### usage `void usage(const char* argv0)`
- Defined: `core/moonshine-tts/tools/japanese-onnx-g2p-cli.cpp:10`

### read_all_stdin `std::string read_all_stdin()`
- Defined: `core/moonshine-tts/tools/japanese-onnx-g2p-cli.cpp:15`

### main `int main(int argc, char** argv)`
- Defined: `core/moonshine-tts/tools/japanese-onnx-g2p-cli.cpp:23`

## core/moonshine-tts/tools/korean-rule-g2p-cli.cpp

### usage `void usage(const char* argv0)`
- Defined: `core/moonshine-tts/tools/korean-rule-g2p-cli.cpp:12`

### read_all_stdin `std::string read_all_stdin()`
- Defined: `core/moonshine-tts/tools/korean-rule-g2p-cli.cpp:19`

### main `int main(int argc, char** argv)`
- Defined: `core/moonshine-tts/tools/korean-rule-g2p-cli.cpp:27`

## core/moonshine-tts/tools/moonshine-g2p-cli.cpp

### usage `void usage(const char *argv0)`
- Defined: `core/moonshine-tts/tools/moonshine-g2p-cli.cpp:23`

### read_all_stdin `std::string read_all_stdin()`
- Defined: `core/moonshine-tts/tools/moonshine-g2p-cli.cpp:101`

### rule_based_kind_label `const char *rule_based_kind_label(RuleBasedG2pKind k)`
- Defined: `core/moonshine-tts/tools/moonshine-g2p-cli.cpp:107`

### print_rule_based_dialect_catalog `void print_rule_based_dialect_catalog(std::ostream &os)`
- Defined: `core/moonshine-tts/tools/moonshine-g2p-cli.cpp:146`

### main `int main(int argc, char **argv)`
- Defined: `core/moonshine-tts/tools/moonshine-g2p-cli.cpp:159`

## core/moonshine-tts/tools/moonshine-tts-cli.cpp

### usage `void usage(const char* argv0)`
- Defined: `core/moonshine-tts/tools/moonshine-tts-cli.cpp:14`

### infer_lang_from_text_utf8 `std::optional<std::string> infer_lang_from_text_utf8(const std::string& text)`
- Defined: `core/moonshine-tts/tools/moonshine-tts-cli.cpp:59`
- Doc: When the user does not pass ``--lang``, infer a tag so Japanese text does not run through English G2P / ``af_heart``.

### main `int main(int argc, char** argv)`
- Defined: `core/moonshine-tts/tools/moonshine-tts-cli.cpp:84`

## core/moonshine-tts/tools/piper-ipa-normalize-cli.cpp

### print_usage `void print_usage()`
- Defined: `core/moonshine-tts/tools/piper-ipa-normalize-cli.cpp:16`

### load_keys `bool load_keys(const std::string& path, std::unordered_set<std::string>& keys)`
- Defined: `core/moonshine-tts/tools/piper-ipa-normalize-cli.cpp:21`

### main `int main(int argc, char** argv)`
- Defined: `core/moonshine-tts/tools/piper-ipa-normalize-cli.cpp:41`

## core/moonshine-tts/tools/piper-phoneme-infer-cli.cpp

### usage `void usage(const char* argv0)`
- Defined: `core/moonshine-tts/tools/piper-phoneme-infer-cli.cpp:17`

### main `int main(int argc, char** argv)`
- Defined: `core/moonshine-tts/tools/piper-phoneme-infer-cli.cpp:33`

## core/moonshine-tts/tools/portuguese-rule-g2p-cli.cpp

### usage `void usage(const char* argv0)`
- Defined: `core/moonshine-tts/tools/portuguese-rule-g2p-cli.cpp:12`

### read_all_stdin `std::string read_all_stdin()`
- Defined: `core/moonshine-tts/tools/portuguese-rule-g2p-cli.cpp:21`

### main `int main(int argc, char** argv)`
- Defined: `core/moonshine-tts/tools/portuguese-rule-g2p-cli.cpp:29`

## core/moonshine-tts/tools/vietnamese-rule-g2p-cli.cpp

### usage `void usage(const char* argv0)`
- Defined: `core/moonshine-tts/tools/vietnamese-rule-g2p-cli.cpp:11`

### read_all_stdin `std::string read_all_stdin()`
- Defined: `core/moonshine-tts/tools/vietnamese-rule-g2p-cli.cpp:17`

### main `int main(int argc, char** argv)`
- Defined: `core/moonshine-tts/tools/vietnamese-rule-g2p-cli.cpp:25`

## core/moonshine-utils/debug-utils-test.cpp

### return_on_error_test `int return_on_error_test()`
- Defined: `core/moonshine-utils/debug-utils-test.cpp:10`

### return_on_false_test `int return_on_false_test()`
- Defined: `core/moonshine-utils/debug-utils-test.cpp:14`

### return_on_null_test `int return_on_null_test()`
- Defined: `core/moonshine-utils/debug-utils-test.cpp:19`

### return_on_not_equal_test `int return_on_not_equal_test()`
- Defined: `core/moonshine-utils/debug-utils-test.cpp:24`

### TEST_CASE `TEST_CASE("debug-utils")`
- Defined: `core/moonshine-utils/debug-utils-test.cpp:30`

### SUBCASE `SUBCASE("LOG")`
- Defined: `core/moonshine-utils/debug-utils-test.cpp:32`

### SUBCASE `SUBCASE("RETURN_ON_ERROR")`
- Defined: `core/moonshine-utils/debug-utils-test.cpp:36`

### SUBCASE `SUBCASE("RETURN_ON_FALSE")`
- Defined: `core/moonshine-utils/debug-utils-test.cpp:37`

### SUBCASE `SUBCASE("RETURN_ON_NULL")`
- Defined: `core/moonshine-utils/debug-utils-test.cpp:38`

### SUBCASE `SUBCASE("RETURN_ON_NOT_EQUAL")`
- Defined: `core/moonshine-utils/debug-utils-test.cpp:39`

### SUBCASE `SUBCASE("TIMER")`
- Defined: `core/moonshine-utils/debug-utils-test.cpp:40`

### SUBCASE `SUBCASE("DEBUG_CALLOC")`
- Defined: `core/moonshine-utils/debug-utils-test.cpp:45`

### SUBCASE `SUBCASE("TRACE")`
- Defined: `core/moonshine-utils/debug-utils-test.cpp:51`

### SUBCASE `SUBCASE("LOG_VARS")`
- Defined: `core/moonshine-utils/debug-utils-test.cpp:55`

### SUBCASE `SUBCASE("load_file_into_memory")`
- Defined: `core/moonshine-utils/debug-utils-test.cpp:76`

### SUBCASE `SUBCASE("save_memory_to_file")`
- Defined: `core/moonshine-utils/debug-utils-test.cpp:87`

### SUBCASE `SUBCASE("load_wav_data_beckett")`
- Defined: `core/moonshine-utils/debug-utils-test.cpp:100`

### SUBCASE `SUBCASE("load_wav_data_two_cities")`
- Defined: `core/moonshine-utils/debug-utils-test.cpp:114`

### SUBCASE `SUBCASE("save_wav_data")`
- Defined: `core/moonshine-utils/debug-utils-test.cpp:128`

## core/moonshine-utils/debug-utils.cpp

### log_backtrace `void log_backtrace()`
- Defined: `core/moonshine-utils/debug-utils.cpp:15`
- Doc: if defined(__APPLE__) include <cxxabi.h> include <execinfo.h> endif

### load_wav_data `bool load_wav_data(const char *path, float **out_float_data,
                   size_t *out_num_s...`
- Defined: `core/moonshine-utils/debug-utils.cpp:51`

### save_wav_data `bool save_wav_data(const char *path, const float *audio_data,
                   size_t num_sampl...`
- Defined: `core/moonshine-utils/debug-utils.cpp:196`

### float_vector_stats_to_string `std::string float_vector_stats_to_string(const std::vector<float> &vector)`
- Defined: `core/moonshine-utils/debug-utils.cpp:249`

### load_file_into_memory `std::vector<uint8_t> load_file_into_memory(const std::string &path)`
- Defined: `core/moonshine-utils/debug-utils.cpp:268`

### save_memory_to_file `void save_memory_to_file(const std::string &path,
                         const std::vector<uint...`
- Defined: `core/moonshine-utils/debug-utils.cpp:289`

## core/moonshine-utils/debug-utils.h

### _moonshine_filename_without_path `static inline const char *_moonshine_filename_without_path(const char *path)`
- Defined: `core/moonshine-utils/debug-utils.h:14`
- Doc: if defined(ANDROID) include <android/asset_manager.h> endif

### debug_calloc `debug_calloc(size, count, FILENAME_ONLY, __LINE__, __FUNCTION__)

static inline void *debug_callo...`
- Defined: `core/moonshine-utils/debug-utils.h:139`
- Doc: define DEBUG_CALLOC(size, count) \

### debug_free `static inline void debug_free(void *voidMemPtr, const char *file, int line,
                     ...`
- Defined: `core/moonshine-utils/debug-utils.h:155`
- Doc: define DEBUG_FREE(ptr) debug_free(ptr, FILENAME_ONLY, __LINE__, __FUNCTION__)

### debug_alloc_get_size `static inline size_t debug_alloc_get_size(void *voidMemPtr)`
- Defined: `core/moonshine-utils/debug-utils.h:175`

### gate `template <typename T>
T gate(T value, T min, T max)`
- Defined: `core/moonshine-utils/debug-utils.h:266`

## core/moonshine-utils/file-utils-test.cpp

### write_file `void write_file(const char *path, const std::vector<uint8_t> &bytes)`
- Defined: `core/moonshine-utils/file-utils-test.cpp:14`
- Doc: Writes `bytes` to `path` for the read-back tests below.

### TEST_CASE `TEST_CASE("fread_exact")`
- Defined: `core/moonshine-utils/file-utils-test.cpp:24`

### SUBCASE `SUBCASE("reads the full requested amount")`
- Defined: `core/moonshine-utils/file-utils-test.cpp:27`

### SUBCASE `SUBCASE("reads multi-byte elements and preserves values")`
- Defined: `core/moonshine-utils/file-utils-test.cpp:41`

### SUBCASE `SUBCASE("throws when fewer elements are available than requested")`
- Defined: `core/moonshine-utils/file-utils-test.cpp:58`

### SUBCASE `SUBCASE("throws on a partial trailing element")`
- Defined: `core/moonshine-utils/file-utils-test.cpp:71`

### SUBCASE `SUBCASE("throws when reading past end of file")`
- Defined: `core/moonshine-utils/file-utils-test.cpp:84`

### SUBCASE `SUBCASE("zero count is a no-op that returns count")`
- Defined: `core/moonshine-utils/file-utils-test.cpp:99`

### SUBCASE `SUBCASE("zero size is a no-op that returns count")`
- Defined: `core/moonshine-utils/file-utils-test.cpp:108`

## core/moonshine-utils/file-utils.cpp

### fread_exact `std::size_t fread_exact(void *ptr, std::size_t size, std::size_t count,
                        s...`
- Defined: `core/moonshine-utils/file-utils.cpp:9`
- Doc: include "debug-utils.h"

## core/moonshine-utils/string-utils-test.cpp

### TEST_CASE `TEST_CASE("string-utils")`
- Defined: `core/moonshine-utils/string-utils-test.cpp:7`
- Doc: define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN include <doctest.h>

### SUBCASE `SUBCASE("replace_all")`
- Defined: `core/moonshine-utils/string-utils-test.cpp:9`

### SUBCASE `SUBCASE("trim")`
- Defined: `core/moonshine-utils/string-utils-test.cpp:12`

### SUBCASE `SUBCASE("split")`
- Defined: `core/moonshine-utils/string-utils-test.cpp:13`

### SUBCASE `SUBCASE("starts_with")`
- Defined: `core/moonshine-utils/string-utils-test.cpp:17`

### SUBCASE `SUBCASE("starts_with_invalid")`
- Defined: `core/moonshine-utils/string-utils-test.cpp:18`

### SUBCASE `SUBCASE("ends_with")`
- Defined: `core/moonshine-utils/string-utils-test.cpp:21`

### SUBCASE `SUBCASE("ends_with_invalid")`
- Defined: `core/moonshine-utils/string-utils-test.cpp:22`

### SUBCASE `SUBCASE("name_to_index")`
- Defined: `core/moonshine-utils/string-utils-test.cpp:25`

### SUBCASE `SUBCASE("append_path_component")`
- Defined: `core/moonshine-utils/string-utils-test.cpp:29`

### SUBCASE `SUBCASE("to_lowercase")`
- Defined: `core/moonshine-utils/string-utils-test.cpp:35`

### SUBCASE `SUBCASE("bool_from_string")`
- Defined: `core/moonshine-utils/string-utils-test.cpp:40`

### SUBCASE `SUBCASE("bool_from_string_invalid")`
- Defined: `core/moonshine-utils/string-utils-test.cpp:46`

### SUBCASE `SUBCASE("float_from_string")`
- Defined: `core/moonshine-utils/string-utils-test.cpp:51`

### SUBCASE `SUBCASE("float_from_string_invalid")`
- Defined: `core/moonshine-utils/string-utils-test.cpp:56`

### SUBCASE `SUBCASE("int32_from_string")`
- Defined: `core/moonshine-utils/string-utils-test.cpp:61`

### SUBCASE `SUBCASE("int32_from_string_invalid")`
- Defined: `core/moonshine-utils/string-utils-test.cpp:66`

### SUBCASE `SUBCASE("size_t_from_string")`
- Defined: `core/moonshine-utils/string-utils-test.cpp:71`

### SUBCASE `SUBCASE("size_t_from_string_invalid")`
- Defined: `core/moonshine-utils/string-utils-test.cpp:76`

## core/moonshine-utils/string-utils.cpp

### replace_all `std::string replace_all(std::string str, const std::string &from,
                        const s...`
- Defined: `core/moonshine-utils/string-utils.cpp:9`
- Doc: See https://stackoverflow.com/questions/2896600/how-to-replace-all-occurrences-of-a-character-in-string

### trim `std::string trim(const std::string &str, const std::string &whitespace)`
- Defined: `core/moonshine-utils/string-utils.cpp:21`
- Doc: See https://stackoverflow.com/questions/1798112/removing-leading-and-trailing-spaces-from-a-string

### split `std::vector<std::string> split(const std::string &str,
                               const std::...`
- Defined: `core/moonshine-utils/string-utils.cpp:30`

### starts_with `bool starts_with(const std::string &str, const std::string &prefix)`
- Defined: `core/moonshine-utils/string-utils.cpp:43`

### ends_with `bool ends_with(const std::string &str, const std::string &suffix)`
- Defined: `core/moonshine-utils/string-utils.cpp:48`

### append_path_component `std::string append_path_component(const std::string &path,
                                  cons...`
- Defined: `core/moonshine-utils/string-utils.cpp:62`

### to_lowercase `std::string to_lowercase(const std::string &str)`
- Defined: `core/moonshine-utils/string-utils.cpp:85`

### bool_from_string `bool bool_from_string(const char *input)`
- Defined: `core/moonshine-utils/string-utils.cpp:91`

### bool_from_string `bool bool_from_string(const std::string &input)`
- Defined: `core/moonshine-utils/string-utils.cpp:98`

### float_from_string `float float_from_string(const char *input)`
- Defined: `core/moonshine-utils/string-utils.cpp:108`

### float_from_string `float float_from_string(const std::string &input)`
- Defined: `core/moonshine-utils/string-utils.cpp:115`

### int32_from_string `int32_t int32_from_string(const char *input)`
- Defined: `core/moonshine-utils/string-utils.cpp:126`

### int32_from_string `int32_t int32_from_string(const std::string &input)`
- Defined: `core/moonshine-utils/string-utils.cpp:133`

### size_t_from_string `size_t size_t_from_string(const char *input)`
- Defined: `core/moonshine-utils/string-utils.cpp:144`

### size_t_from_string `size_t size_t_from_string(const std::string &input)`
- Defined: `core/moonshine-utils/string-utils.cpp:151`

## core/ort-utils/moonshine-ort-allocator.cpp

### MoonshineAlloc `void *MoonshineAlloc(struct OrtAllocator *this_, size_t size)`
- Defined: `core/ort-utils/moonshine-ort-allocator.cpp:7`

### MoonshineFree `void MoonshineFree(struct OrtAllocator *this_, void *p)`
- Defined: `core/ort-utils/moonshine-ort-allocator.cpp:14`

### MoonshineInfo `const struct OrtMemoryInfo *MoonshineInfo(const struct OrtAllocator *this_)`
- Defined: `core/ort-utils/moonshine-ort-allocator.cpp:21`

### MoonshineReserve `void *MoonshineReserve(struct OrtAllocator *this_, size_t size)`
- Defined: `core/ort-utils/moonshine-ort-allocator.cpp:28`

### MoonshineAllocOnStream `void *MoonshineAllocOnStream(struct OrtAllocator *this_, size_t size,
                           ...`
- Defined: `core/ort-utils/moonshine-ort-allocator.cpp:34`

### friendlySizeString `void friendlySizeString(size_t byte_count, char *output, size_t output_size)`
- Defined: `core/ort-utils/moonshine-ort-allocator.cpp:49`

### printFriendlySize `void printFriendlySize(const char *prefix, size_t number)`
- Defined: `core/ort-utils/moonshine-ort-allocator.cpp:64`

### MoonshineOrtAllocator `MoonshineOrtAllocator::MoonshineOrtAllocator(const OrtMemoryInfo *memory_info)`
- Defined: `core/ort-utils/moonshine-ort-allocator.cpp:71`

### print_stats `void MoonshineOrtAllocator::print_stats()`
- Defined: `core/ort-utils/moonshine-ort-allocator.cpp:92`

## core/ort-utils/moonshine-tensor-view.cpp

### checked_mul `bool checked_mul(size_t a, size_t b, size_t *out)`
- Defined: `core/ort-utils/moonshine-tensor-view.cpp:18`
- Doc: Portable checked multiply for size_t: returns false on overflow (leaving *out untouched), otherwise stores a * b. We avo

### moonshine_tensor_from_shape_and_dtype `moonshine_tensor_t *moonshine_tensor_from_shape_and_dtype(
    const std::vector<int64_t> &shape,...`
- Defined: `core/ort-utils/moonshine-tensor-view.cpp:25`

### moonshine_tensor_from_ort_tensor `moonshine_tensor_t *moonshine_tensor_from_ort_tensor(const OrtApi *ort_api,
                     ...`
- Defined: `core/ort-utils/moonshine-tensor-view.cpp:99`

### MoonshineTensorView `MoonshineTensorView::MoonshineTensorView()
    : _tensor(nullptr), name("anonymous")`
- Defined: `core/ort-utils/moonshine-tensor-view.cpp:116`

### MoonshineTensorView `MoonshineTensorView::MoonshineTensorView(moonshine_tensor_t *tensor,
                            ...`
- Defined: `core/ort-utils/moonshine-tensor-view.cpp:119`

### MoonshineTensorView `MoonshineTensorView::MoonshineTensorView(const std::vector<int64_t> &shape,
                     ...`
- Defined: `core/ort-utils/moonshine-tensor-view.cpp:131`

### MoonshineTensorView `MoonshineTensorView::MoonshineTensorView(const MoonshineTensorView &other)
    : _shape(other._sh...`
- Defined: `core/ort-utils/moonshine-tensor-view.cpp:138`

### MoonshineTensorView `MoonshineTensorView::MoonshineTensorView(const OrtApi *ort_api,
                                 ...`
- Defined: `core/ort-utils/moonshine-tensor-view.cpp:145`

### shape `std::vector<int64_t> &MoonshineTensorView::shape()`
- Defined: `core/ort-utils/moonshine-tensor-view.cpp:177`

### element_count `size_t MoonshineTensorView::element_count()`
- Defined: `core/ort-utils/moonshine-tensor-view.cpp:179`

### bytes_count `size_t MoonshineTensorView::bytes_count()`
- Defined: `core/ort-utils/moonshine-tensor-view.cpp:184`

### dtype `uint32_t MoonshineTensorView::dtype()`
- Defined: `core/ort-utils/moonshine-tensor-view.cpp:190`

### reshape `void MoonshineTensorView::reshape(const std::vector<int64_t> &shape)`
- Defined: `core/ort-utils/moonshine-tensor-view.cpp:192`

### cast_f16_to_f32 `MoonshineTensorView MoonshineTensorView::cast_f16_to_f32()`
- Defined: `core/ort-utils/moonshine-tensor-view.cpp:201`

### argmax `int64_t MoonshineTensorView::argmax()`
- Defined: `core/ort-utils/moonshine-tensor-view.cpp:213`

### ort_dtype_to_moonshine_dtype `moonshine_dtype_t ort_dtype_to_moonshine_dtype(
    ONNXTensorElementDataType ort_dtype)`
- Defined: `core/ort-utils/moonshine-tensor-view.cpp:229`

### moonshine_dtype_to_ort_dtype `ONNXTensorElementDataType moonshine_dtype_to_ort_dtype(
    uint32_t moonshine_dtype)`
- Defined: `core/ort-utils/moonshine-tensor-view.cpp:257`

### ort_dtype_to_bytes_per_element `size_t ort_dtype_to_bytes_per_element(ONNXTensorElementDataType ort_dtype)`
- Defined: `core/ort-utils/moonshine-tensor-view.cpp:282`

### moonshine_dtype_to_bytes_per_element `size_t moonshine_dtype_to_bytes_per_element(uint32_t moonshine_dtype)`
- Defined: `core/ort-utils/moonshine-tensor-view.cpp:310`

### moonshine_tensor_from_token_vector `MoonshineTensorView *moonshine_tensor_from_token_vector(
    std::vector<int32_t> &vector)`
- Defined: `core/ort-utils/moonshine-tensor-view.cpp:316`

### token_vector_from_moonshine_tensor `std::vector<int32_t> token_vector_from_moonshine_tensor(
    MoonshineTensorView *moonshine_tensor)`
- Defined: `core/ort-utils/moonshine-tensor-view.cpp:324`

### create_ort_value `OrtValue *MoonshineTensorView::create_ort_value(const OrtApi *ort_api,
                          ...`
- Defined: `core/ort-utils/moonshine-tensor-view.cpp:331`

### float16_to_float32 `void float16_to_float32(const uint16_t *f16_array, float *f32_array,
                        size...`
- Defined: `core/ort-utils/moonshine-tensor-view.cpp:345`
- Doc: Thank you Claude.

### to_string `std::string MoonshineTensorView::to_string()`
- Defined: `core/ort-utils/moonshine-tensor-view.cpp:386`

## core/ort-utils/moonshine-tensor-view.h

### data `template <typename T>
  T *data()`
- Defined: `core/ort-utils/moonshine-tensor-view.h:77`
- Doc: Data pointer retrieval with type checking.

## core/ort-utils/ort-utils-ep-test.cpp

### TEST_CASE `TEST_CASE("ort_parse_provider_names")`
- Defined: `core/ort-utils/ort-utils-ep-test.cpp:9`
- Doc: include <filesystem> include <string>

### SUBCASE `SUBCASE("empty string")`
- Defined: `core/ort-utils/ort-utils-ep-test.cpp:11`

### SUBCASE `SUBCASE("comma-separated aliases")`
- Defined: `core/ort-utils/ort-utils-ep-test.cpp:15`

### SUBCASE `SUBCASE("execution provider suffix aliases")`
- Defined: `core/ort-utils/ort-utils-ep-test.cpp:22`

### SUBCASE `SUBCASE("empty token is rejected")`
- Defined: `core/ort-utils/ort-utils-ep-test.cpp:30`

### TEST_CASE `TEST_CASE("ort_append_execution_providers")`
- Defined: `core/ort-utils/ort-utils-ep-test.cpp:36`

### SUBCASE `SUBCASE("unknown provider returns error status")`
- Defined: `core/ort-utils/ort-utils-ep-test.cpp:47`

### SUBCASE `SUBCASE("cpu provider appends successfully")`
- Defined: `core/ort-utils/ort-utils-ep-test.cpp:56`

### SUBCASE `SUBCASE("coreml provider appends successfully")`
- Defined: `core/ort-utils/ort-utils-ep-test.cpp:64`
- Doc: if defined(__APPLE__)

### SUBCASE `SUBCASE("nnapi provider appends successfully")`
- Defined: `core/ort-utils/ort-utils-ep-test.cpp:72`
- Doc: if defined(__ANDROID__)

### TEST_CASE `TEST_CASE("ort session with execution providers")`
- Defined: `core/ort-utils/ort-utils-ep-test.cpp:82`

### SUBCASE `SUBCASE("cpu-only session creation")`
- Defined: `core/ort-utils/ort-utils-ep-test.cpp:98`

### SUBCASE `SUBCASE("coreml session creation")`
- Defined: `core/ort-utils/ort-utils-ep-test.cpp:118`
- Doc: if defined(__APPLE__)

### SUBCASE `SUBCASE("nnapi session creation")`
- Defined: `core/ort-utils/ort-utils-ep-test.cpp:138`
- Doc: if defined(__ANDROID__)

## core/ort-utils/ort-utils-ep.cpp

### trim_copy `std::string trim_copy(const std::string &s)`
- Defined: `core/ort-utils/ort-utils-ep.cpp:16`

### lowercase_copy `std::string lowercase_copy(std::string s)`
- Defined: `core/ort-utils/ort-utils-ep.cpp:28`

### normalize_provider_name `std::string normalize_provider_name(const std::string &name)`
- Defined: `core/ort-utils/ort-utils-ep.cpp:35`

### make_invalid_argument_status `OrtStatus *make_invalid_argument_status(const OrtApi *ort_api,
                                  ...`
- Defined: `core/ort-utils/ort-utils-ep.cpp:50`

### append_one_provider `OrtStatus *append_one_provider(
    const OrtApi *ort_api, OrtSessionOptions *session_options,
  ...`
- Defined: `core/ort-utils/ort-utils-ep.cpp:55`

### ort_parse_provider_names `std::vector<std::string> ort_parse_provider_names(const std::string &csv)`
- Defined: `core/ort-utils/ort-utils-ep.cpp:101`

### ort_append_execution_providers `OrtStatus *ort_append_execution_providers(
    const OrtApi *ort_api, OrtSessionOptions *session_...`
- Defined: `core/ort-utils/ort-utils-ep.cpp:125`

## core/ort-utils/ort-utils-test.cpp

### TEST_CASE `TEST_CASE("ort-utils")`
- Defined: `core/ort-utils/ort-utils-test.cpp:6`
- Doc: include <doctest.h>

### SUBCASE `SUBCASE("ort_session_from_path")`
- Defined: `core/ort-utils/ort-utils-test.cpp:8`

### SUBCASE `SUBCASE("ort_session_from_memory")`
- Defined: `core/ort-utils/ort-utils-test.cpp:12`

## core/ort-utils/ort-utils.cpp

### ort_session_from_path `int ort_session_from_path(const OrtApi *ort_api, OrtEnv *env,
                          OrtSessio...`
- Defined: `core/ort-utils/ort-utils.cpp:18`
- Doc: ifdef _WIN32 No memory mapping on Windows and wchar for the file path.

### ort_session_from_path `int ort_session_from_path(const OrtApi *ort_api, OrtEnv *env,
                          OrtSessio...`
- Defined: `core/ort-utils/ort-utils.cpp:37`
- Doc: else

### ort_session_from_memory `int ort_session_from_memory(const OrtApi *ort_api, OrtEnv *env,
                            OrtSe...`
- Defined: `core/ort-utils/ort-utils.cpp:81`
- Doc: endif

### ort_maybe_force_single_thread `void ort_maybe_force_single_thread(const OrtApi *ort_api,
                                   OrtS...`
- Defined: `core/ort-utils/ort-utils.cpp:93`

### ort_session_from_asset `int ort_session_from_asset(const OrtApi *ort_api, OrtEnv *env,
                           OrtSess...`
- Defined: `core/ort-utils/ort-utils.cpp:107`
- Doc: if defined(ANDROID)

### ort_get_shape `std::vector<int64_t> ort_get_shape(const OrtApi *ort_api,
                                   OrtT...`
- Defined: `core/ort-utils/ort-utils.cpp:151`
- Doc: endif

### ort_get_type `ONNXTensorElementDataType ort_get_type(const OrtApi *ort_api,
                                   ...`
- Defined: `core/ort-utils/ort-utils.cpp:168`

### ort_get_input_shape `std::vector<int64_t> ort_get_input_shape(const OrtApi *ort_api,
                                 ...`
- Defined: `core/ort-utils/ort-utils.cpp:178`

### ort_get_input_type `ONNXTensorElementDataType ort_get_input_type(const OrtApi *ort_api,
                             ...`
- Defined: `core/ort-utils/ort-utils.cpp:188`

### ort_get_output_shape `std::vector<int64_t> ort_get_output_shape(const OrtApi *ort_api,
                                ...`
- Defined: `core/ort-utils/ort-utils.cpp:198`

### ort_get_output_type `ONNXTensorElementDataType ort_get_output_type(const OrtApi *ort_api,
                            ...`
- Defined: `core/ort-utils/ort-utils.cpp:208`

### ort_get_value_shape `std::vector<int64_t> ort_get_value_shape(const OrtApi *ort_api,
                                 ...`
- Defined: `core/ort-utils/ort-utils.cpp:218`

### ort_get_value_type `ONNXTensorElementDataType ort_get_value_type(const OrtApi *ort_api,
                             ...`
- Defined: `core/ort-utils/ort-utils.cpp:227`

### ort_run `OrtStatus *ort_run(const OrtApi *ort_api, OrtSession *session,
                   const char *con...`
- Defined: `core/ort-utils/ort-utils.cpp:236`

## core/ort-utils/ort-utils.h

### ort_configure_execution_providers `inline void ort_configure_execution_providers(
    const OrtApi *ort_api, OrtSessionOptions *sess...`
- Defined: `core/ort-utils/ort-utils.h:113`

## core/reliability/fuzz-resampler.cpp

### sane_rate `float sane_rate(float rate)`
- Defined: `core/reliability/fuzz-resampler.cpp:17`

## core/reliability/fuzz-tensor-view.cpp

### next_u8 `uint8_t next_u8()`
- Defined: `core/reliability/fuzz-tensor-view.cpp:25`

### next_i64 `int64_t next_i64()`
- Defined: `core/reliability/fuzz-tensor-view.cpp:27`

## core/resampler-test.cpp

### test_resample_audio `void test_resample_audio(const std::vector<float> &input_audio,
                         int32_t ...`
- Defined: `core/resampler-test.cpp:13`

### TEST_CASE `TEST_CASE("resampler-test")`
- Defined: `core/resampler-test.cpp:43`

### SUBCASE `SUBCASE("resample-audio")`
- Defined: `core/resampler-test.cpp:45`

## core/resampler.cpp

### resample_audio `const std::vector<float> resample_audio(const std::vector<float> &audio,
                        ...`
- Defined: `core/resampler.cpp:4`
- Doc: include "debug-utils.h"

### downsample_audio `const std::vector<float> downsample_audio(const std::vector<float> &audio,
                      ...`
- Defined: `core/resampler.cpp:16`

### upsample_audio `const std::vector<float> upsample_audio(const std::vector<float> &audio,
                        ...`
- Defined: `core/resampler.cpp:55`

## core/silero-vad.cpp

### init_onnx_env `void SileroVad::init_onnx_env()`
- Defined: `core/silero-vad.cpp:5`
- Doc: include "ort-utils.h" include "silero-vad-model-data.h"

### init_engine_threads `void SileroVad::init_engine_threads(int inter_threads, int intra_threads)`
- Defined: `core/silero-vad.cpp:21`
- Doc: Initializes threading settings.

### SileroVad `SileroVad::SileroVad(int sample_rate, int windows_frame_size, float threshold,
                  ...`
- Defined: `core/silero-vad.cpp:29`

### load_from_memory `int SileroVad::load_from_memory(const uint8_t *model_data,
                                size_t...`
- Defined: `core/silero-vad.cpp:59`

### predict `void SileroVad::predict(const std::vector<float> &data_chunk,
                        float *out_...`
- Defined: `core/silero-vad.cpp:78`
- Doc: Inference: runs inference on one chunk of input data. data_chunk is expected to have window_size_samples samples (e.g., 

## core/silero-vad.h

### is_loaded `bool is_loaded() const`
- Defined: `core/silero-vad.h:84`

## core/speaker-diarizer.cpp

### turn_overlap_seconds `double turn_overlap_seconds(
    const std::vector<cppannote::StreamingDiarizationTurn> &a, int32...`
- Defined: `core/speaker-diarizer.cpp:17`
- Doc: Total seconds of overlap between the spans of two turn lists.

### Impl `explicit Impl(const SpeakerDiarizerOptions &options_in)
      : engine(), options(options_in)`
- Defined: `core/speaker-diarizer.cpp:66`

### session_config `cppannote::StreamingDiarizationConfig session_config() const`
- Defined: `core/speaker-diarizer.cpp:74`

### get_stream `StreamState &get_stream(int32_t stream_id)`
- Defined: `core/speaker-diarizer.cpp:82`

### allocate_stable_id `uint64_t allocate_stable_id()`
- Defined: `core/speaker-diarizer.cpp:91`

### map_snapshot_to_stable_ids `void map_snapshot_to_stable_ids(
      StreamState &state,
      const cppannote::StreamingDiariz...`
- Defined: `core/speaker-diarizer.cpp:102`
- Doc: Maps the clustering labels in `snapshot` onto stable speaker IDs by greedily matching each label against the labels of t

### sort `std::sort(candidates.begin(), candidates.end(),
              [](const auto &a, const auto &b)`
- Defined: `core/speaker-diarizer.cpp:135`

### SpeakerDiarizer `SpeakerDiarizer::SpeakerDiarizer(const SpeakerDiarizerOptions &options)
    : impl(std::make_uniq...`
- Defined: `core/speaker-diarizer.cpp:170`

### create_stream `int32_t SpeakerDiarizer::create_stream()`
- Defined: `core/speaker-diarizer.cpp:175`

### free_stream `void SpeakerDiarizer::free_stream(int32_t stream_id)`
- Defined: `core/speaker-diarizer.cpp:185`

### start_stream `void SpeakerDiarizer::start_stream(int32_t stream_id)`
- Defined: `core/speaker-diarizer.cpp:190`

### add_audio_to_stream `void SpeakerDiarizer::add_audio_to_stream(int32_t stream_id,
                                    ...`
- Defined: `core/speaker-diarizer.cpp:200`

### get_turns `std::vector<SpeakerTurn> SpeakerDiarizer::get_turns(int32_t stream_id)`
- Defined: `core/speaker-diarizer.cpp:217`

### finish_stream `std::vector<SpeakerTurn> SpeakerDiarizer::finish_stream(int32_t stream_id)`
- Defined: `core/speaker-diarizer.cpp:224`

### diarize `std::vector<SpeakerTurn> SpeakerDiarizer::diarize(const float *audio_data,
                      ...`
- Defined: `core/speaker-diarizer.cpp:235`

## core/spelling-fusion-data.cpp

### build_set `std::unordered_set<std::string> build_set(
    std::initializer_list<const char *> phrases)`
- Defined: `core/spelling-fusion-data.cpp:27`

### upper_modifiers `const std::unordered_set<std::string> &upper_modifiers()`
- Defined: `core/spelling-fusion-data.cpp:267`

### upper_modifiers_by_length `const std::vector<std::string> &upper_modifiers_by_length()`
- Defined: `core/spelling-fusion-data.cpp:280`

### sort `std::sort(v.begin(), v.end(),
              [](const std::string &a, const std::string &b)`
- Defined: `core/spelling-fusion-data.cpp:287`

### undo_words `const std::unordered_set<std::string> &undo_words()`
- Defined: `core/spelling-fusion-data.cpp:295`

### clear_words `const std::unordered_set<std::string> &clear_words()`
- Defined: `core/spelling-fusion-data.cpp:308`

### stop_words `const std::unordered_set<std::string> &stop_words()`
- Defined: `core/spelling-fusion-data.cpp:318`

### default_weak_homonyms `const std::unordered_set<std::string> &default_weak_homonyms()`
- Defined: `core/spelling-fusion-data.cpp:337`

### default_meta `const DefaultSpellingMeta &default_meta()`
- Defined: `core/spelling-fusion-data.cpp:355`

## core/spelling-fusion-test.cpp

### char_match `SpellingMatch char_match(const std::string &c)`
- Defined: `core/spelling-fusion-test.cpp:13`
- Doc: Helper: shorthand for "matcher said this character".

### no_match `SpellingMatch no_match()`
- Defined: `core/spelling-fusion-test.cpp:21`
- Doc: Helper: shorthand for "no match".

### TEST_CASE `TEST_CASE("spelling-fusion: normalize")`
- Defined: `core/spelling-fusion-test.cpp:24`

### TEST_CASE `TEST_CASE("spelling-fusion: matcher classifies plain letters")`
- Defined: `core/spelling-fusion-test.cpp:38`

### TEST_CASE `TEST_CASE("spelling-fusion: matcher classifies NATO codewords")`
- Defined: `core/spelling-fusion-test.cpp:49`

### TEST_CASE `TEST_CASE("spelling-fusion: matcher classifies digits")`
- Defined: `core/spelling-fusion-test.cpp:60`

### TEST_CASE `TEST_CASE("spelling-fusion: matcher parses 10..1000 number words")`
- Defined: `core/spelling-fusion-test.cpp:72`

### TEST_CASE `TEST_CASE("spelling-fusion: matcher applies upper-case modifier")`
- Defined: `core/spelling-fusion-test.cpp:84`

### TEST_CASE `TEST_CASE("spelling-fusion: matcher recognizes speller patterns")`
- Defined: `core/spelling-fusion-test.cpp:93`

### TEST_CASE `TEST_CASE("spelling-fusion: matcher classifies command words")`
- Defined: `core/spelling-fusion-test.cpp:102`

### TEST_CASE `TEST_CASE("spelling-fusion: matcher classifies special characters")`
- Defined: `core/spelling-fusion-test.cpp:113`

### TEST_CASE `TEST_CASE("spelling-fusion: weak-homonym detection")`
- Defined: `core/spelling-fusion-test.cpp:148`

### TEST_CASE `TEST_CASE("spelling-fusion: fuse without prediction")`
- Defined: `core/spelling-fusion-test.cpp:157`

### TEST_CASE `TEST_CASE("spelling-fusion: fuse drops unrecognized + no prediction")`
- Defined: `core/spelling-fusion-test.cpp:165`

### TEST_CASE `TEST_CASE("spelling-fusion: fuse passes through command words")`
- Defined: `core/spelling-fusion-test.cpp:172`

### TEST_CASE `TEST_CASE(
    "spelling-fusion: special-character match is preserved when the "
    "spelling mo...`
- Defined: `core/spelling-fusion-test.cpp:182`

### TEST_CASE `TEST_CASE("spelling-fusion: weak-homonym demotion")`
- Defined: `core/spelling-fusion-test.cpp:203`

### TEST_CASE `TEST_CASE("spelling-fusion: cross-class routing")`
- Defined: `core/spelling-fusion-test.cpp:224`

### TEST_CASE `TEST_CASE("spelling-fusion: same-class disagreement uses threshold")`
- Defined: `core/spelling-fusion-test.cpp:237`

### TEST_CASE `TEST_CASE("spelling-fusion: multi-digit ASR vs single-digit spelling")`
- Defined: `core/spelling-fusion-test.cpp:250`

### TEST_CASE `TEST_CASE("spelling-fusion: agreement preserves matcher casing")`
- Defined: `core/spelling-fusion-test.cpp:274`

### TEST_CASE `TEST_CASE("spelling-fusion: spelling-only when matcher misses")`
- Defined: `core/spelling-fusion-test.cpp:283`

### TEST_CASE `TEST_CASE("spelling-fusion: data tables are non-empty")`
- Defined: `core/spelling-fusion-test.cpp:292`

## core/spelling-fusion.cpp

### is_ascii_drop `bool is_ascii_drop(char c)`
- Defined: `core/spelling-fusion.cpp:24`

### is_ascii_letter `bool is_ascii_letter(char c)`
- Defined: `core/spelling-fusion.cpp:34`

### ascii_to_lower `char ascii_to_lower(char c)`
- Defined: `core/spelling-fusion.cpp:38`

### consume_curly_quote `size_t consume_curly_quote(const std::string &input, size_t i)`
- Defined: `core/spelling-fusion.cpp:46`
- Doc: Try to consume a 3-byte UTF-8 curly quote starting at ``input[i]``. Returns the number of bytes consumed (3) on success,

### split_on_whitespace `std::vector<std::string> split_on_whitespace(const std::string &s)`
- Defined: `core/spelling-fusion.cpp:62`
- Doc: Split ``s`` on ASCII whitespace, dropping empty tokens.

### parse_number_words `std::optional<int> parse_number_words(const std::string &text)`
- Defined: `core/spelling-fusion.cpp:107`

### is_ascii_digit_string `bool is_ascii_digit_string(const std::string &s)`
- Defined: `core/spelling-fusion.cpp:180`

### is_printable_ascii `bool is_printable_ascii(char c)`
- Defined: `core/spelling-fusion.cpp:188`

### spelling_normalize `std::string spelling_normalize(const std::string &text)`
- Defined: `core/spelling-fusion.cpp:194`

### SpellingMatcher `SpellingMatcher::SpellingMatcher()
    : lookup_(&spelling_fusion_data::lookup_table()),
      up...`
- Defined: `core/spelling-fusion.cpp:233`

### classify `SpellingMatch SpellingMatcher::classify(const std::string &raw_text) const`
- Defined: `core/spelling-fusion.cpp:243`

### is_weak_homonym `bool SpellingMatcher::is_weak_homonym(const std::string &raw_text) const`
- Defined: `core/spelling-fusion.cpp:299`

### resolve `std::optional<std::string> SpellingMatcher::resolve(
    const std::string &text) const`
- Defined: `core/spelling-fusion.cpp:304`

### resolve_spelled_letter `std::optional<std::string> SpellingMatcher::resolve_spelled_letter(
    const std::string &text) ...`
- Defined: `core/spelling-fusion.cpp:325`

### string_is_letter `bool string_is_letter(const std::string &c)`
- Defined: `core/spelling-fusion.cpp:373`
- Doc: Mirror Python's ``str.isalpha()`` / ``str.isdigit()`` semantics on the ASCII strings that the matcher emits. The ASR sid

### string_is_digit `bool string_is_digit(const std::string &c)`
- Defined: `core/spelling-fusion.cpp:380`

### single_char_is_letter `bool single_char_is_letter(const std::string &c)`
- Defined: `core/spelling-fusion.cpp:388`

### apply_case `std::string apply_case(const std::string &ch, const std::string &hint)`
- Defined: `core/spelling-fusion.cpp:392`

### fuse_default `FusedResult fuse_default(const std::string &raw_text,
                         const SpellingMatc...`
- Defined: `core/spelling-fusion.cpp:406`

## core/spelling-fusion.h

### is_character `bool is_character() const`
- Defined: `core/spelling-fusion.h:40`

### is_recognized `bool is_recognized() const`
- Defined: `core/spelling-fusion.h:42`

### is_character `bool is_character() const`
- Defined: `core/spelling-fusion.h:91`

## core/spelling-model-test.cpp

### find_model_path `std::string find_model_path()`
- Defined: `core/spelling-model-test.cpp:21`
- Doc: Locate the bundled spelling model. CMake copies the test runner into the build dir alongside ``test-assets/spelling_cnn.

### find_wav `std::string find_wav(const std::string &label, const std::string &filename)`
- Defined: `core/spelling-model-test.cpp:32`

### read_file `std::vector<uint8_t> read_file(const std::string &path)`
- Defined: `core/spelling-model-test.cpp:47`
- Doc: Read entire file into a byte buffer.

### TEST_CASE `TEST_CASE("spelling-model: load from path")`
- Defined: `core/spelling-model-test.cpp:59`

### TEST_CASE `TEST_CASE("spelling-model: load from memory")`
- Defined: `core/spelling-model-test.cpp:72`

### TEST_CASE `TEST_CASE("spelling-model: predict on bundled clips")`
- Defined: `core/spelling-model-test.cpp:85`

### TEST_CASE `TEST_CASE("spelling-model: invalid arguments are rejected")`
- Defined: `core/spelling-model-test.cpp:132`

## core/spelling-model.cpp

### lookup_metadata `std::optional<std::string> lookup_metadata(const OrtApi *ort_api,
                               ...`
- Defined: `core/spelling-model.cpp:26`
- Doc: Read a single key from the model's custom_metadata_map, returning nullopt when the key isn't present or any ORT call fai

### trim `std::string trim(const std::string &s)`
- Defined: `core/spelling-model.cpp:45`
- Doc: Trim ASCII whitespace.

### parse_class_list_json `std::vector<std::string> parse_class_list_json(const std::string &raw)`
- Defined: `core/spelling-model.cpp:59`
- Doc: Parse a JSON string array of class labels (e.g. ``["a","b",...]``). We deliberately don't pull in nlohmann/json for this

### SpellingModel `SpellingModel::SpellingModel(bool log_ort_run,
                             const std::vector<std...`
- Defined: `core/spelling-model.cpp:94`

### initialize_session_options `void SpellingModel::initialize_session_options()`
- Defined: `core/spelling-model.cpp:136`

### apply_default_metadata `void SpellingModel::apply_default_metadata()`
- Defined: `core/spelling-model.cpp:156`

### load `int SpellingModel::load(const char *model_path)`
- Defined: `core/spelling-model.cpp:168`

### load_from_memory `int SpellingModel::load_from_memory(const uint8_t *model_data,
                                  ...`
- Defined: `core/spelling-model.cpp:176`

### populate_metadata_from_session `int SpellingModel::populate_metadata_from_session()`
- Defined: `core/spelling-model.cpp:185`

### predict `int SpellingModel::predict(const float *audio, size_t audio_size,
                           int3...`
- Defined: `core/spelling-model.cpp:242`

## core/spelling-model.h

### sample_rate `int32_t sample_rate() const`
- Defined: `core/spelling-model.h:56`
- Doc: Accessors.

### clip_seconds `float clip_seconds() const`
- Defined: `core/spelling-model.h:57`

### classes `const std::vector<std::string> &classes() const`
- Defined: `core/spelling-model.h:58`

## core/tts-repeated-memory-test.cpp

### read_rss_kb `size_t read_rss_kb()`
- Defined: `core/tts-repeated-memory-test.cpp:53`

### median `size_t median(std::vector<size_t> values)`
- Defined: `core/tts-repeated-memory-test.cpp:89`

### env_size `size_t env_size(const char *name, size_t default_value)`
- Defined: `core/tts-repeated-memory-test.cpp:98`

### detect_continual_growth `bool detect_continual_growth(const std::vector<size_t> &samples,
                             siz...`
- Defined: `core/tts-repeated-memory-test.cpp:117`
- Doc: Mirrors transcriber-streaming-memory-test's detector: fits a line to the post-warmup samples and reports sustained growt

### create_synth `int32_t create_synth(const EngineSpec &spec)`
- Defined: `core/tts-repeated-memory-test.cpp:222`

### synth_once `bool synth_once(int32_t handle, size_t text_index)`
- Defined: `core/tts-repeated-memory-test.cpp:235`

### reload_strict `bool reload_strict()`
- Defined: `core/tts-repeated-memory-test.cpp:247`

### run_growth_phase `void run_growth_phase(const std::string &label, size_t iterations,
                      const st...`
- Defined: `core/tts-repeated-memory-test.cpp:259`
- Doc: Runs `iterations` of `body`, sampling RSS after each, and checks for sustained post-warmup growth. Reports the regressio

### exercise_engine `void exercise_engine(const EngineSpec &spec)`
- Defined: `core/tts-repeated-memory-test.cpp:293`

### run_growth_phase `run_growth_phase(
        std::string(spec.name) + " synth", synth_iterations,
        [handle](s...`
- Defined: `core/tts-repeated-memory-test.cpp:306`

### run_growth_phase `run_growth_phase(
      std::string(spec.name) + " reload", reload_iterations,
      [&spec](size...`
- Defined: `core/tts-repeated-memory-test.cpp:322`
- Doc: Repeated create/synthesize/free: probes model load + teardown. Reloading is heavier (especially ZipVoice), so it runs fe

### file_present `bool file_present(const fs::path &p)`
- Defined: `core/tts-repeated-memory-test.cpp:338`

### kokoro_spec `std::optional<EngineSpec> kokoro_spec()`
- Defined: `core/tts-repeated-memory-test.cpp:343`

### piper_spec `std::optional<EngineSpec> piper_spec()`
- Defined: `core/tts-repeated-memory-test.cpp:354`

### zipvoice_spec `std::optional<EngineSpec> zipvoice_spec()`
- Defined: `core/tts-repeated-memory-test.cpp:388`

### TEST_CASE `TEST_CASE("tts-repeated-memory-kokoro")`
- Defined: `core/tts-repeated-memory-test.cpp:406`

### TEST_CASE `TEST_CASE("tts-repeated-memory-piper")`
- Defined: `core/tts-repeated-memory-test.cpp:415`

### TEST_CASE `TEST_CASE("tts-repeated-memory-zipvoice")`
- Defined: `core/tts-repeated-memory-test.cpp:425`

### discover_data_root `std::optional<fs::path> discover_data_root()`
- Defined: `core/tts-repeated-memory-test.cpp:439`
- Doc: Discovers core/moonshine-tts/data relative to common working directories used by the test scripts (repo root, test-asset

### main `int main(int argc, char **argv)`
- Defined: `core/tts-repeated-memory-test.cpp:463`

## core/voice-activity-detector-test.cpp

### TEST_CASE `TEST_CASE("voice-activity-detector-test")`
- Defined: `core/voice-activity-detector-test.cpp:10`
- Doc: define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN include <doctest.h>

### SUBCASE `SUBCASE("vad-block")`
- Defined: `core/voice-activity-detector-test.cpp:15`

### SUBCASE `SUBCASE("vad-stream")`
- Defined: `core/voice-activity-detector-test.cpp:54`

### SUBCASE `SUBCASE("vad-threshold-0")`
- Defined: `core/voice-activity-detector-test.cpp:122`

## core/voice-activity-detector.cpp

### seconds_from_sample_count `float seconds_from_sample_count(size_t sample_count)`
- Defined: `core/voice-activity-detector.cpp:14`

### VoiceActivityDetector `VoiceActivityDetector::VoiceActivityDetector(float threshold,
                                   ...`
- Defined: `core/voice-activity-detector.cpp:23`

### start `void VoiceActivityDetector::start()`
- Defined: `core/voice-activity-detector.cpp:49`

### stop `void VoiceActivityDetector::stop()`
- Defined: `core/voice-activity-detector.cpp:61`

### process_audio `void VoiceActivityDetector::process_audio(const float *audio_data,
                              ...`
- Defined: `core/voice-activity-detector.cpp:68`

### clear_completed_segment_audio_data `void VoiceActivityDetector::clear_completed_segment_audio_data()`
- Defined: `core/voice-activity-detector.cpp:98`

### retained_segment_audio_byte_count `size_t VoiceActivityDetector::retained_segment_audio_byte_count() const`
- Defined: `core/voice-activity-detector.cpp:106`

### completed_segment_audio_byte_count `size_t VoiceActivityDetector::completed_segment_audio_byte_count() const`
- Defined: `core/voice-activity-detector.cpp:114`

### process_audio_chunk `void VoiceActivityDetector::process_audio_chunk(const float *audio_data,
                        ...`
- Defined: `core/voice-activity-detector.cpp:124`

### on_voice_start `void VoiceActivityDetector::on_voice_start()`
- Defined: `core/voice-activity-detector.cpp:195`

### on_voice_continuing `void VoiceActivityDetector::on_voice_continuing()`
- Defined: `core/voice-activity-detector.cpp:209`

### on_voice_end `void VoiceActivityDetector::on_voice_end()`
- Defined: `core/voice-activity-detector.cpp:218`

### to_string `std::string VoiceActivitySegment::to_string() const`
- Defined: `core/voice-activity-detector.cpp:227`

### to_string `std::string VoiceActivityDetector::to_string() const`
- Defined: `core/voice-activity-detector.cpp:237`

## core/voice-activity-detector.h

### is_active `bool is_active() const`
- Defined: `core/voice-activity-detector.h:53`

### get_segments `const std::vector<VoiceActivitySegment> *get_segments() const`
- Defined: `core/voice-activity-detector.h:56`

## core/word-alignment-benchmark.cpp

### load_wav `static float* load_wav(const char* path, long* num_samples_out)`
- Defined: `core/word-alignment-benchmark.cpp:9`
- Doc: include "file-utils.h" include "moonshine-c-api.h"

### run_benchmark `static BenchResult run_benchmark(const char* model_path, const char* wav_path,
                  ...`
- Defined: `core/word-alignment-benchmark.cpp:37`

### main `int main(int argc, char** argv)`
- Defined: `core/word-alignment-benchmark.cpp:96`

## core/word-alignment-test.cpp

### TEST_CASE `TEST_CASE("word-timestamps")`
- Defined: `core/word-alignment-test.cpp:11`
- Doc: define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN include <doctest.h>

### SUBCASE `SUBCASE("non-streaming-transcribe-with-word-timestamps")`
- Defined: `core/word-alignment-test.cpp:13`

## core/word-alignment.cpp

### dtw `void dtw(const std::vector<float>& cost_matrix, int N, int M,
         std::vector<int>& text_ind...`
- Defined: `core/word-alignment.cpp:11`
- Doc: DTW (Dynamic Time Warping)

### compute_median `static float compute_median(std::vector<float>& window)`
- Defined: `core/word-alignment.cpp:92`
- Doc: Median filter (along last axis of 3D array)

### median_filter `void median_filter(std::vector<float>& data, int channels, int height,
                   int wid...`
- Defined: `core/word-alignment.cpp:98`

### token_starts_new_word `static bool token_starts_new_word(BinTokenizer* tokenizer, int token_id)`
- Defined: `core/word-alignment.cpp:158`
- Doc: Helper: check if a token's raw bytes start with the SentencePiece word boundary marker (UTF-8 encoding of U+2581 LOWER O

### decode_tokens `static std::string decode_tokens(BinTokenizer* tokenizer,
                                 const ...`
- Defined: `core/word-alignment.cpp:173`
- Doc: Helper: decode a list of token IDs to text.

### align_words `std::vector<TranscriberWord> align_words(const float* cross_attention_data,
                     ...`
- Defined: `core/word-alignment.cpp:180`
- Doc: align_words: main entry point

## examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/AssetDirectoryCopy.kt

### copyDirIfNeeded
- Defined: `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/AssetDirectoryCopy.kt:10`
- Doc: package ai.moonshine.examples.intentrecognizer import android.content.Context import java.io.File import java.io.FileOut

## examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/PhraseAdapter.kt

### resetToDefaults
- Defined: `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/PhraseAdapter.kt:27`

### addEmptyRow
- Defined: `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/PhraseAdapter.kt:40`

### removeRow
- Defined: `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/PhraseAdapter.kt:46`

### flashHighlight
- Defined: `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/PhraseAdapter.kt:54`

### currentPhrases
- Defined: `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/PhraseAdapter.kt:71`
- Doc: val idx = items.indexOfFirst { it.id == id } if (idx >= 0) { notifyItemChanged(idx) } Handler(Looper.getMainLooper()).po

### rowIdMatchingCanonical
- Defined: `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/PhraseAdapter.kt:72`

### bind
- Defined: `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/PhraseAdapter.kt:89`

## examples/android/TextToSpeech/app/src/main/java/ai/moonshine/examples/texttospeech/AssetDirectoryCopy.kt

### copyDirIfNeeded
- Defined: `examples/android/TextToSpeech/app/src/main/java/ai/moonshine/examples/texttospeech/AssetDirectoryCopy.kt:10`
- Doc: package ai.moonshine.examples.texttospeech import android.content.Context import java.io.File import java.io.FileOutputS

## examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java

### onCreate
- Defined: `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java:50`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`

### TranscriptEventListener
- Defined: `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java:62`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`

### onLineTextChanged
- Defined: `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java:64`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`

### onLineCompleted
- Defined: `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java:75`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`

### onDestroy
- Defined: `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java:133`
- Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`

## examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift

### bootstrapIfNeeded
- Defined: `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:52`

### scheduleDebouncedIntentSync
- Defined: `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:110`

### phraseTextCommitted
- Defined: `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:119`

### addPhrase
- Defined: `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:132`

### removePhrase
- Defined: `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:137`

### toggleListening
- Defined: `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:143`

### handleCompletedTranscriptLine
- Defined: `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:168`

### pauseMicIfNeededForBackground
- Defined: `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:207`

### handleTranscriptLineStarted
- Defined: `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:218`

### handleTranscriptLineTextChanged
- Defined: `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:226`

### handleTranscriptLineCompleted
- Defined: `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift:231`

## examples/ios/IntentRecognizer/IntentRecognizer/IntentTranscriptBridge.swift

### onLineStarted
- Defined: `examples/ios/IntentRecognizer/IntentRecognizer/IntentTranscriptBridge.swift:7`

### onLineTextChanged
- Defined: `examples/ios/IntentRecognizer/IntentRecognizer/IntentTranscriptBridge.swift:13`

### onLineCompleted
- Defined: `examples/ios/IntentRecognizer/IntentRecognizer/IntentTranscriptBridge.swift:20`

## examples/ios/TextToSpeech/TextToSpeech/TextToSpeechApp.swift

### hash
- Defined: `examples/ios/TextToSpeech/TextToSpeech/TextToSpeechApp.swift:10`

### hash
- Defined: `examples/ios/TextToSpeech/TextToSpeech/TextToSpeechApp.swift:65`

### initialize
- Defined: `examples/ios/TextToSpeech/TextToSpeech/TextToSpeechApp.swift:95`

### changeLanguage
- Defined: `examples/ios/TextToSpeech/TextToSpeech/TextToSpeechApp.swift:173`
- Doc: MARK: - Public language / voice switching

### changeVoice
- Defined: `examples/ios/TextToSpeech/TextToSpeech/TextToSpeechApp.swift:189`

### speak
- Defined: `examples/ios/TextToSpeech/TextToSpeech/TextToSpeechApp.swift:194`

## examples/ios/Transcriber/Transcriber/TranscriberApp.swift

### addNewMessage
- Defined: `examples/ios/Transcriber/Transcriber/TranscriberApp.swift:65`

### updateLatestMessage
- Defined: `examples/ios/Transcriber/Transcriber/TranscriberApp.swift:69`

### handleRecordingChanged
- Defined: `examples/ios/Transcriber/Transcriber/TranscriberApp.swift:73`

## examples/ios/Transcriber/TranscriberUITests/TranscriberUITests.swift

### setUpWithError
- Defined: `examples/ios/Transcriber/TranscriberUITests/TranscriberUITests.swift:11`

### tearDownWithError
- Defined: `examples/ios/Transcriber/TranscriberUITests/TranscriberUITests.swift:20`

### testExample
- Defined: `examples/ios/Transcriber/TranscriberUITests/TranscriberUITests.swift:26`

### testLaunchPerformance
- Defined: `examples/ios/Transcriber/TranscriberUITests/TranscriberUITests.swift:35`

## examples/ios/Transcriber/TranscriberUITests/TranscriberUITestsLaunchTests.swift

### setUpWithError
- Defined: `examples/ios/Transcriber/TranscriberUITests/TranscriberUITestsLaunchTests.swift:15`

### testLaunch
- Defined: `examples/ios/Transcriber/TranscriberUITests/TranscriberUITestsLaunchTests.swift:21`

## examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift

### transcribeWithoutStreaming
- Defined: `examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift:5`
- Doc: Transcribe audio data offline without streaming

### transcribeWithStreaming
- Defined: `examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift:26`
- Doc: Example of streaming transcription

### onLineStarted
- Defined: `examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift:33`

### onLineTextChanged
- Defined: `examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift:39`

### onLineCompleted
- Defined: `examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift:46`

### parseArguments
- Defined: `examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift:82`

### main
- Defined: `examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift:146`
- Doc: MARK: - Main

## examples/macos/MicTranscription/Sources/MicTranscription/main.swift

### main
- Defined: `examples/macos/MicTranscription/Sources/MicTranscription/main.swift:5`
- Doc: MARK: - Main

### onLineStarted
- Defined: `examples/macos/MicTranscription/Sources/MicTranscription/main.swift:42`

### onLineTextChanged
- Defined: `examples/macos/MicTranscription/Sources/MicTranscription/main.swift:48`

### onLineCompleted
- Defined: `examples/macos/MicTranscription/Sources/MicTranscription/main.swift:55`

## examples/macos/TextToSpeech/Sources/TextToSpeech/main.swift

### writeWav
- Defined: `examples/macos/TextToSpeech/Sources/TextToSpeech/main.swift:6`
- Doc: MARK: - WAV Writing

### printUsage
- Defined: `examples/macos/TextToSpeech/Sources/TextToSpeech/main.swift:66`

### parseArguments
- Defined: `examples/macos/TextToSpeech/Sources/TextToSpeech/main.swift:86`

### resolveAssetRoot
- Defined: `examples/macos/TextToSpeech/Sources/TextToSpeech/main.swift:163`
- Doc: MARK: - Asset Root Resolution

### resolveDevice
- Defined: `examples/macos/TextToSpeech/Sources/TextToSpeech/main.swift:205`
- Doc: MARK: - Device Resolution

### main
- Defined: `examples/macos/TextToSpeech/Sources/TextToSpeech/main.swift:246`
- Doc: MARK: - Main

## examples/python/basic_transcription.py

### transcribe_without_streaming `def transcribe_without_streaming(transcriber, audio_data, sample_rate)`
- Defined: `examples/python/basic_transcription.py:16`
- Doc: Transcribe audio data offline without streaming.

### transcribe_with_streaming `def transcribe_with_streaming(transcriber, audio_data, sample_rate)`
- Defined: `examples/python/basic_transcription.py:30`
- Doc: Example of streaming transcription.

### on_line_started `def on_line_started(self, event)`
- Defined: `examples/python/basic_transcription.py:38`

### on_line_text_changed `def on_line_text_changed(self, event)`
- Defined: `examples/python/basic_transcription.py:41`

### on_line_completed `def on_line_completed(self, event)`
- Defined: `examples/python/basic_transcription.py:44`

## examples/python/dialog_flow.py

### setup_wifi `def setup_wifi(d)`
- Defined: `examples/python/dialog_flow.py:46`
- Doc: Classic slot-filling flow: network name, password, confirm, apply.

### set_timezone `def set_timezone(d)`
- Defined: `examples/python/dialog_flow.py:70`
- Doc: Sub-flow that can be composed with ``yield from``.

### full_onboarding `def full_onboarding(d)`
- Defined: `examples/python/dialog_flow.py:80`
- Doc: Compose sub-flows with ``yield from``.

### _apply_wifi_config `def _apply_wifi_config(ssid, password)`
- Defined: `examples/python/dialog_flow.py:89`

### run_live `def run_live(args)`
- Defined: `examples/python/dialog_flow.py:142`

### run_interactive `def run_interactive(flow_name)`
- Defined: `examples/python/dialog_flow.py:279`
- Doc: Keyboard-driven demo – prompts go to stdout, replies come from stdin.

### run_scripted `def run_scripted(flow_name, answers)`
- Defined: `examples/python/dialog_flow.py:347`
- Doc: Drive a flow from a pre-canned list of utterances.

### main `def main()`
- Defined: `examples/python/dialog_flow.py:411`

### __init__ `def __init__(self)`
- Defined: `examples/python/dialog_flow.py:112`

### _overwrite `def _overwrite(self, text)`
- Defined: `examples/python/dialog_flow.py:116`

### on_line_started `def on_line_started(self, event)`
- Defined: `examples/python/dialog_flow.py:122`

### on_line_text_changed `def on_line_text_changed(self, event)`
- Defined: `examples/python/dialog_flow.py:125`

### on_line_completed `def on_line_completed(self, event)`
- Defined: `examples/python/dialog_flow.py:128`

### mute `def mute(should_mute)`
- Defined: `examples/python/dialog_flow.py:202`

### set_spelling_mode `def set_spelling_mode(active)`
- Defined: `examples/python/dialog_flow.py:206`
- Doc: Toggle the C++ spelling-CNN fusion path on the live mic stream.

### speak `def speak(text)`
- Defined: `examples/python/dialog_flow.py:212`
- Doc: Log every spoken prompt and (optionally) pass it through TTS.

### speak `def speak(text)`
- Defined: `examples/python/dialog_flow.py:293`

### speak `def speak(text)`
- Defined: `examples/python/dialog_flow.py:363`

## examples/python/intent_recognition.py

### on_lights_on `def on_lights_on(trigger, utterance, similarity)`
- Defined: `examples/python/intent_recognition.py:26`
- Doc: Handler for turning lights on.

### on_lights_off `def on_lights_off(trigger, utterance, similarity)`
- Defined: `examples/python/intent_recognition.py:31`
- Doc: Handler for turning lights off.

### on_weather `def on_weather(trigger, utterance, similarity)`
- Defined: `examples/python/intent_recognition.py:36`
- Doc: Handler for weather queries.

### on_timer `def on_timer(trigger, utterance, similarity)`
- Defined: `examples/python/intent_recognition.py:41`
- Doc: Handler for timer requests.

### on_music_play `def on_music_play(trigger, utterance, similarity)`
- Defined: `examples/python/intent_recognition.py:46`
- Doc: Handler for playing music.

### on_music_stop `def on_music_stop(trigger, utterance, similarity)`
- Defined: `examples/python/intent_recognition.py:51`
- Doc: Handler for stopping music.

### main `def main()`
- Defined: `examples/python/intent_recognition.py:80`

### __init__ `def __init__(self)`
- Defined: `examples/python/intent_recognition.py:59`

### update_last_terminal_line `def update_last_terminal_line(self, new_text)`
- Defined: `examples/python/intent_recognition.py:62`

### on_line_started `def on_line_started(self, event)`
- Defined: `examples/python/intent_recognition.py:69`

### on_line_text_changed `def on_line_text_changed(self, event)`
- Defined: `examples/python/intent_recognition.py:72`

### on_line_completed `def on_line_completed(self, event)`
- Defined: `examples/python/intent_recognition.py:75`

## examples/python/mic_transcription.py

### __init__ `def __init__(self)`
- Defined: `examples/python/mic_transcription.py:15`

### update_last_terminal_line `def update_last_terminal_line(self, new_text)`
- Defined: `examples/python/mic_transcription.py:20`

### on_line_started `def on_line_started(self, event)`
- Defined: `examples/python/mic_transcription.py:30`

### on_line_text_changed `def on_line_text_changed(self, event)`
- Defined: `examples/python/mic_transcription.py:33`

### on_line_completed `def on_line_completed(self, event)`
- Defined: `examples/python/mic_transcription.py:36`

### on_line_completed `def on_line_completed(self, event)`
- Defined: `examples/python/mic_transcription.py:45`

## examples/python/ollama-voice/ollama_voice.py

### __init__ `def __init__(self)`
- Defined: `examples/python/ollama-voice/ollama_voice.py:17`

### spin `def spin(self)`
- Defined: `examples/python/ollama-voice/ollama_voice.py:20`

### __init__ `def __init__(self, ollama_model, system_prompt)`
- Defined: `examples/python/ollama-voice/ollama_voice.py:34`
- Doc: Initialize the OllamaVoice listener.

### on_line_text_changed `def on_line_text_changed(self, event)`
- Defined: `examples/python/ollama-voice/ollama_voice.py:59`
- Doc: Called whenever the transcription of the current line changes (live updates).

### on_line_completed `def on_line_completed(self, event)`
- Defined: `examples/python/ollama-voice/ollama_voice.py:69`
- Doc: Called when a line (segment) of speech has been fully transcribed.

## examples/raspberry-pi/my-dalek/my-dalek.py

### on_intent_triggered_on `def on_intent_triggered_on(trigger, utterance, similarity)`
- Defined: `examples/raspberry-pi/my-dalek/my-dalek.py:38`
- Doc: Handler for when an intent is triggered.

### on_move_forward `def on_move_forward(trigger, utterance, similarity)`
- Defined: `examples/raspberry-pi/my-dalek/my-dalek.py:92`

### on_move_backward `def on_move_backward(trigger, utterance, similarity)`
- Defined: `examples/raspberry-pi/my-dalek/my-dalek.py:94`

### on_turn_left `def on_turn_left(trigger, utterance, similarity)`
- Defined: `examples/raspberry-pi/my-dalek/my-dalek.py:96`

### on_turn_right `def on_turn_right(trigger, utterance, similarity)`
- Defined: `examples/raspberry-pi/my-dalek/my-dalek.py:98`

### on_exterminate `def on_exterminate(trigger, utterance, similarity)`
- Defined: `examples/raspberry-pi/my-dalek/my-dalek.py:100`

### __init__ `def __init__(self)`
- Defined: `examples/raspberry-pi/my-dalek/my-dalek.py:47`

### update_last_terminal_line `def update_last_terminal_line(self, new_text)`
- Defined: `examples/raspberry-pi/my-dalek/my-dalek.py:50`

### on_line_started `def on_line_started(self, event)`
- Defined: `examples/raspberry-pi/my-dalek/my-dalek.py:57`

### on_line_text_changed `def on_line_text_changed(self, event)`
- Defined: `examples/raspberry-pi/my-dalek/my-dalek.py:60`

### on_line_completed `def on_line_completed(self, event)`
- Defined: `examples/raspberry-pi/my-dalek/my-dalek.py:63`

## examples/windows/cli-transcriber/cli-transcriber.cpp

### COMInitializer `public:
  COMInitializer()`
- Defined: `examples/windows/cli-transcriber/cli-transcriber.cpp:25`

### onLineStarted `public:
  void onLineStarted(const moonshine::LineStarted &event) override`
- Defined: `examples/windows/cli-transcriber/cli-transcriber.cpp:37`

### onLineTextChanged `void onLineTextChanged(const moonshine::LineTextChanged &event) override`
- Defined: `examples/windows/cli-transcriber/cli-transcriber.cpp:43`

### onLineCompleted `void onLineCompleted(const moonshine::LineCompleted &event) override`
- Defined: `examples/windows/cli-transcriber/cli-transcriber.cpp:51`

### onError `void onError(const moonshine::Error &event) override`
- Defined: `examples/windows/cli-transcriber/cli-transcriber.cpp:59`

### MicrophoneCapture `public:
  MicrophoneCapture() : is_capturing_(false), sample_rate_(16000)`
- Defined: `examples/windows/cli-transcriber/cli-transcriber.cpp:72`

### Initialize `bool Initialize()`
- Defined: `examples/windows/cli-transcriber/cli-transcriber.cpp:94`

### Start `void Start()`
- Defined: `examples/windows/cli-transcriber/cli-transcriber.cpp:191`

### Stop `void Stop()`
- Defined: `examples/windows/cli-transcriber/cli-transcriber.cpp:207`

### SetAudioCallback `void SetAudioCallback(
      std::function<void(const std::vector<float> &, int32_t)> callback)`
- Defined: `examples/windows/cli-transcriber/cli-transcriber.cpp:222`

### CaptureLoop `private:
  void CaptureLoop()`
- Defined: `examples/windows/cli-transcriber/cli-transcriber.cpp:227`

### WavFileProducer `public:
  explicit WavFileProducer(std::string wav_path,
                           float chunk_d...`
- Defined: `examples/windows/cli-transcriber/cli-transcriber.cpp:325`

### getNextAudio `bool getNextAudio(std::vector<float> &out_audio_data)`
- Defined: `examples/windows/cli-transcriber/cli-transcriber.cpp:335`

### sampleRate `int32_t sampleRate() const`
- Defined: `examples/windows/cli-transcriber/cli-transcriber.cpp:347`

### loadWavData `private:
  void loadWavData(const std::string &wav_path)`
- Defined: `examples/windows/cli-transcriber/cli-transcriber.cpp:349`

### runWavTranscription `int runWavTranscription(const std::string &model_path,
                        moonshine::ModelAr...`
- Defined: `examples/windows/cli-transcriber/cli-transcriber.cpp:455`

### main `int main(int argc, char *argv[])`
- Defined: `examples/windows/cli-transcriber/cli-transcriber.cpp:488`

## micro/examples/rp2350/generated/neural_tts_pack.S

### g_neural_tts_pack
- Defined: `micro/examples/rp2350/generated/neural_tts_pack.S:5`

### g_neural_tts_pack_end
- Defined: `micro/examples/rp2350/generated/neural_tts_pack.S:8`

## micro/examples/rp2350/scripts/capture_neural_tts.py

### find_port `def find_port()`
- Defined: `micro/examples/rp2350/scripts/capture_neural_tts.py:22`

### main `def main()`
- Defined: `micro/examples/rp2350/scripts/capture_neural_tts.py:29`

## micro/examples/rp2350/scripts/capture_stt.py

### _resolve_serial `def _resolve_serial(explicit, timeout)`
- Defined: `micro/examples/rp2350/scripts/capture_stt.py:36`
- Doc: Return the device serial node, waiting for it to (re)appear after flash.

### _open_raw `def _open_raw(dev)`
- Defined: `micro/examples/rp2350/scripts/capture_stt.py:61`
- Doc: Open the CDC device in raw, NON-BLOCKING mode (mirrors usb_audio_bridge).

### _save_wav `def _save_wav(path, raw, rate)`
- Defined: `micro/examples/rp2350/scripts/capture_stt.py:109`

### main `def main()`
- Defined: `micro/examples/rp2350/scripts/capture_stt.py:117`

### __init__ `def __init__(self, fd)`
- Defined: `micro/examples/rp2350/scripts/capture_stt.py:74`

### _fill `def _fill(self)`
- Defined: `micro/examples/rp2350/scripts/capture_stt.py:78`

### readline `def readline(self)`
- Defined: `micro/examples/rp2350/scripts/capture_stt.py:92`

### read_exact `def read_exact(self, n)`
- Defined: `micro/examples/rp2350/scripts/capture_stt.py:100`

## micro/examples/rp2350/scripts/flash.sh

### find_mounted_volume
- Defined: `micro/examples/rp2350/scripts/flash.sh:66`
- Doc: Echo the first currently-mounted candidate (empty if none are mounted yet).

### usage
- Defined: `micro/examples/rp2350/scripts/flash.sh:78`
- Doc: Require a variant argument and map it to the firmware artifact name.

### wait_volume_writable
- Defined: `micro/examples/rp2350/scripts/flash.sh:227`
- Doc: macOS sometimes reports the BOOTSEL volume before it's actually writable (Permission denied on the first cp). Poll until

### draw_bar
- Defined: `micro/examples/rp2350/scripts/flash.sh:259`
- Doc: 2. Copy with a progress bar. cp may return non-zero because the Pico reboots mid-write (sometimes before cp's final fsyn

## micro/examples/rp2350/scripts/generate_speaker_test_clips.py

### _read_pcm `def _read_pcm(path)`
- Defined: `micro/examples/rp2350/scripts/generate_speaker_test_clips.py:27`

### _write_header `def _write_header()`
- Defined: `micro/examples/rp2350/scripts/generate_speaker_test_clips.py:46`

### main `def main()`
- Defined: `micro/examples/rp2350/scripts/generate_speaker_test_clips.py:74`

## micro/examples/rp2350/scripts/monitor.sh

### _wait_for_any_usbmodem
- Defined: `micro/examples/rp2350/scripts/monitor.sh:89`

### _wait_for_specific_tty
- Defined: `micro/examples/rp2350/scripts/monitor.sh:113`

## micro/examples/rp2350/scripts/tts_speak.py

### find_port `def find_port()`
- Defined: `micro/examples/rp2350/scripts/tts_speak.py:36`

### main `def main()`
- Defined: `micro/examples/rp2350/scripts/tts_speak.py:44`

### send_line `def send_line(s)`
- Defined: `micro/examples/rp2350/scripts/tts_speak.py:71`

## micro/examples/rp2350/scripts/usb_audio_bridge.py

### _resolve_serial `def _resolve_serial(explicit, timeout)`
- Defined: `micro/examples/rp2350/scripts/usb_audio_bridge.py:49`
- Doc: Return the device serial node, waiting for it to (re)appear.

### _open_raw `def _open_raw(dev)`
- Defined: `micro/examples/rp2350/scripts/usb_audio_bridge.py:80`
- Doc: Open the CDC device in raw, NON-BLOCKING mode.

### main `def main()`
- Defined: `micro/examples/rp2350/scripts/usb_audio_bridge.py:140`

### __init__ `def __init__(self, fd)`
- Defined: `micro/examples/rp2350/scripts/usb_audio_bridge.py:104`

### _fill `def _fill(self)`
- Defined: `micro/examples/rp2350/scripts/usb_audio_bridge.py:108`

### readline `def readline(self)`
- Defined: `micro/examples/rp2350/scripts/usb_audio_bridge.py:123`

### read_exact `def read_exact(self, n)`
- Defined: `micro/examples/rp2350/scripts/usb_audio_bridge.py:131`

### _dev `def _dev(arg)`
- Defined: `micro/examples/rp2350/scripts/usb_audio_bridge.py:163`

### save_stream `def save_stream(tag, samples, rate)`
- Defined: `micro/examples/rp2350/scripts/usb_audio_bridge.py:184`

### on_audio `def on_audio(indata, frames, time_info, status)`
- Defined: `micro/examples/rp2350/scripts/usb_audio_bridge.py:206`

### sender `def sender()`
- Defined: `micro/examples/rp2350/scripts/usb_audio_bridge.py:224`

### flush_mic `def flush_mic()`
- Defined: `micro/examples/rp2350/scripts/usb_audio_bridge.py:260`

### receiver `def receiver()`
- Defined: `micro/examples/rp2350/scripts/usb_audio_bridge.py:268`

### _on_signal `def _on_signal(signum, frame)`
- Defined: `micro/examples/rp2350/scripts/usb_audio_bridge.py:404`

## micro/examples/rp2350/src/app_common.cc

### LedPulse `void LedPulse(unsigned pin, int count, int on_ms, int off_ms)`
- Defined: `micro/examples/rp2350/src/app_common.cc:32`

### BoardInit `unsigned BoardInit()`
- Defined: `micro/examples/rp2350/src/app_common.cc:41`

### PrintBootBanner `void PrintBootBanner()`
- Defined: `micro/examples/rp2350/src/app_common.cc:83`

## micro/examples/rp2350/src/audio_service.cc

### SetTtsVolume `void SetTtsVolume(float volume)`
- Defined: `micro/examples/rp2350/src/audio_service.cc:65`

### TtsVolume `float TtsVolume()`
- Defined: `micro/examples/rp2350/src/audio_service.cc:71`

### RecognizerInit `void RecognizerInit(kiss_fftr_state* fft)`
- Defined: `micro/examples/rp2350/src/audio_service.cc:73`

### RecognizeOne `int RecognizeOne(AudioInput& input, uint8_t* arena, std::size_t arena_size,
                 int1...`
- Defined: `micro/examples/rp2350/src/audio_service.cc:102`

### PlayCapturedClip `void PlayCapturedClip(const int16_t* window, int num_samples,
                      AudioOutput& ...`
- Defined: `micro/examples/rp2350/src/audio_service.cc:386`
- Doc: Play back the front-aligned capture window (what the classifier saw) before the TTS reply so mic wiring/gain issues are 

### SpeakEmit `void SpeakEmit(void* user, const int16_t* samples, int n)`
- Defined: `micro/examples/rp2350/src/audio_service.cc:439`

### SkipSpaces `const char* SkipSpaces(const char* p)`
- Defined: `micro/examples/rp2350/src/audio_service.cc:463`

### PopClause `const char* PopClause(const char* text, char* out, size_t cap)`
- Defined: `micro/examples/rp2350/src/audio_service.cc:472`
- Doc: Copy one clause from `text` into `out` (cap bytes). Return pointer to the remainder, or nullptr when done. Splits at pun

### Speak `void Speak(const char* text, AudioOutput& output, AudioInput& input,
           uint8_t* arena, s...`
- Defined: `micro/examples/rp2350/src/audio_service.cc:498`

### RunAudioService `void RunAudioService(AudioInput& input, AudioOutput& output, uint8_t* arena,
                    ...`
- Defined: `micro/examples/rp2350/src/audio_service.cc:546`

## micro/examples/rp2350/src/echo_app.cc

### RunEchoApp `void RunEchoApp()`
- Defined: `micro/examples/rp2350/src/echo_app.cc:27`

## micro/examples/rp2350/src/echo_hardware_app.cc

### RunEchoHardwareApp `void RunEchoHardwareApp()`
- Defined: `micro/examples/rp2350/src/echo_hardware_app.cc:23`

## micro/examples/rp2350/src/i2s_audio_io.cc

### CaptureWriteIdx `inline unsigned CaptureWriteIdx()`
- Defined: `micro/examples/rp2350/src/i2s_audio_io.cc:49`
- Doc: Current DMA write position as a ring word index (0..kRingWords-1).

### StartCaptureDma `void StartCaptureDma()`
- Defined: `micro/examples/rp2350/src/i2s_audio_io.cc:54`

### I2sAudioInput `I2sAudioInput::I2sAudioInput(int sample_rate)
    : sm_(0), dc_blocker_(sample_rate)`
- Defined: `micro/examples/rp2350/src/i2s_audio_io.cc:75`

### ReadHop `bool I2sAudioInput::ReadHop(int16_t* out, int n)`
- Defined: `micro/examples/rp2350/src/i2s_audio_io.cc:95`

### Drain `void I2sAudioInput::Drain()`
- Defined: `micro/examples/rp2350/src/i2s_audio_io.cc:113`

## micro/examples/rp2350/src/i2s_audio_out.cc

### StereoFrame `inline uint32_t StereoFrame(int16_t s)`
- Defined: `micro/examples/rp2350/src/i2s_audio_out.cc:20`
- Doc: Pack one mono int16 sample into a 32-bit stereo I2S frame: MSB-first shift means [31:16] is the ws=0 slot and [15:0] the

### PeakNormalizeGain `float PeakNormalizeGain(const int16_t* samples, int n, float target,
                        floa...`
- Defined: `micro/examples/rp2350/src/i2s_audio_out.cc:42`

### PeakNormalizeGain `float PeakNormalizeGain(const float* samples, int n, float target,
                        float ...`
- Defined: `micro/examples/rp2350/src/i2s_audio_out.cc:57`

### I2sAudioOutput `I2sAudioOutput::I2sAudioOutput(unsigned data_pin, unsigned clock_base,
                          ...`
- Defined: `micro/examples/rp2350/src/i2s_audio_out.cc:71`

### ReadIdx `unsigned I2sAudioOutput::ReadIdx() const`
- Defined: `micro/examples/rp2350/src/i2s_audio_out.cc:100`

### Used `unsigned I2sAudioOutput::Used() const`
- Defined: `micro/examples/rp2350/src/i2s_audio_out.cc:106`

### StartDma `void I2sAudioOutput::StartDma()`
- Defined: `micro/examples/rp2350/src/i2s_audio_out.cc:110`

### PushFrame `void I2sAudioOutput::PushFrame(uint32_t frame)`
- Defined: `micro/examples/rp2350/src/i2s_audio_out.cc:117`

### ApplyClockDiv `void I2sAudioOutput::ApplyClockDiv()`
- Defined: `micro/examples/rp2350/src/i2s_audio_out.cc:130`

### Begin `void I2sAudioOutput::Begin(int sample_rate, int num_samples, const char* kind)`
- Defined: `micro/examples/rp2350/src/i2s_audio_out.cc:139`

### Write `void I2sAudioOutput::Write(const int16_t* samples, int n)`
- Defined: `micro/examples/rp2350/src/i2s_audio_out.cc:157`

### End `void I2sAudioOutput::End()`
- Defined: `micro/examples/rp2350/src/i2s_audio_out.cc:166`

## micro/examples/rp2350/src/i2s_audio_out.h

### SetGain `void SetGain(float gain)`
- Defined: `micro/examples/rp2350/src/i2s_audio_out.h:56`
- Doc: Linear playback gain applied before I2S conversion. Use with PeakNormalizeGain() to bring quiet clips up to a usable lev

## micro/examples/rp2350/src/i2s_mic_process.cc

### I2sRawToInt32 `int32_t I2sRawToInt32(uint32_t raw)`
- Defined: `micro/examples/rp2350/src/i2s_mic_process.cc:7`

### I2sRawToInt16 `int16_t I2sRawToInt16(uint32_t raw)`
- Defined: `micro/examples/rp2350/src/i2s_mic_process.cc:11`

### I2sDcBlocker `I2sDcBlocker::I2sDcBlocker(int sample_rate_hz, float cutoff_hz)
    : r_(std::exp(-2.f * 3.141592...`
- Defined: `micro/examples/rp2350/src/i2s_mic_process.cc:17`

### Process `int16_t I2sDcBlocker::Process(int16_t x)`
- Defined: `micro/examples/rp2350/src/i2s_mic_process.cc:21`

### Reset `void I2sDcBlocker::Reset()`
- Defined: `micro/examples/rp2350/src/i2s_mic_process.cc:31`

### I2sRemoveBufferDc `void I2sRemoveBufferDc(int16_t* samples, int n)`
- Defined: `micro/examples/rp2350/src/i2s_mic_process.cc:36`

## micro/examples/rp2350/src/main_audio_loopback_test.cc

### Record `void Record(spelling::I2sAudioInput& input)`
- Defined: `micro/examples/rp2350/src/main_audio_loopback_test.cc:26`

### Play `void Play(spelling::I2sAudioOutput& output)`
- Defined: `micro/examples/rp2350/src/main_audio_loopback_test.cc:39`

### main `int main()`
- Defined: `micro/examples/rp2350/src/main_audio_loopback_test.cc:60`

## micro/examples/rp2350/src/main_echo_hardware.cc

### main `int main()`
- Defined: `micro/examples/rp2350/src/main_echo_hardware.cc:9`
- Doc: include "app_common.h" include "echo_hardware_app.h"

## micro/examples/rp2350/src/main_i2s_audio_test.cc

### BuildSineTable `void BuildSineTable()`
- Defined: `micro/examples/rp2350/src/main_i2s_audio_test.cc:96`

### PlayTone `void PlayTone(spelling::I2sAudioOutput& out, double freq, int ms)`
- Defined: `micro/examples/rp2350/src/main_i2s_audio_test.cc:107`
- Doc: Play `freq` Hz for `ms` ms with a short attack/release to avoid clicks. Uses the same I2sAudioOutput sink as the live ap

### PlaySweep `void PlaySweep(spelling::I2sAudioOutput& out, double f0, double f1, int ms)`
- Defined: `micro/examples/rp2350/src/main_i2s_audio_test.cc:135`
- Doc: Linear frequency sweep from `f0` to `f1` over `ms`, click-free at the ends.

### TtsEmit `void TtsEmit(void* user, const int16_t* samples, int n)`
- Defined: `micro/examples/rp2350/src/main_i2s_audio_test.cc:171`

### SpeakText `void SpeakText(spelling::I2sAudioOutput& out, neural_tts::NeuralTts& tts,
               const ch...`
- Defined: `micro/examples/rp2350/src/main_i2s_audio_test.cc:190`
- Doc: Synthesize `text` and play it. `label` is just the human-readable name for the log line (for letters it differs from the

### main `int main()`
- Defined: `micro/examples/rp2350/src/main_i2s_audio_test.cc:223`

## micro/examples/rp2350/src/main_i2s_mic_test.cc

### Add `void Add(int32_t s, uint32_t raw)`
- Defined: `micro/examples/rp2350/src/main_i2s_mic_test.cc:59`

### DrainUsbInput `void DrainUsbInput()`
- Defined: `micro/examples/rp2350/src/main_i2s_mic_test.cc:70`

### DrawBar `void DrawBar(double level, double full_scale)`
- Defined: `micro/examples/rp2350/src/main_i2s_mic_test.cc:75`

### ChannelRms `double ChannelRms(const ChannelStats& st)`
- Defined: `micro/examples/rp2350/src/main_i2s_mic_test.cc:85`

### ReportChannel `void ReportChannel(const char* name, const ChannelStats& st, bool active)`
- Defined: `micro/examples/rp2350/src/main_i2s_mic_test.cc:92`

### RecordWindow `void RecordWindow(PIO pio, uint sm, ChannelStats* a, ChannelStats* b,
                  spelling:...`
- Defined: `micro/examples/rp2350/src/main_i2s_mic_test.cc:112`

### StreamToHost `void StreamToHost(const int16_t* samples, int n)`
- Defined: `micro/examples/rp2350/src/main_i2s_mic_test.cc:131`

### WaitForClipAck `bool WaitForClipAck(int timeout_ms)`
- Defined: `micro/examples/rp2350/src/main_i2s_mic_test.cc:144`
- Doc: Wait for usb_audio_bridge.py to finish playing the clip and send CLIP_ACK.

### main `int main()`
- Defined: `micro/examples/rp2350/src/main_i2s_mic_test.cc:167`

## micro/examples/rp2350/src/main_i2s_relay.cc

### ReadLine `int ReadLine(char* buf, int maxlen)`
- Defined: `micro/examples/rp2350/src/main_i2s_relay.cc:71`
- Doc: Read one newline-terminated line into `buf` (NUL-terminated), blocking until a non-empty line arrives. Feeds the watchdo

### ReadByteTimed `int ReadByteTimed(int timeout_ms)`
- Defined: `micro/examples/rp2350/src/main_i2s_relay.cc:88`
- Doc: Read one byte, waiting up to ~timeout_ms. Returns -1 on timeout.

### ReadHop `int ReadHop(int16_t* out, int n)`
- Defined: `micro/examples/rp2350/src/main_i2s_relay.cc:98`
- Doc: Scan for the 0xA5 0x5A sync, then read up to `n` int16 LE samples into `out`. Returns the number of samples read; a shor

### PlayStream `int PlayStream(spelling::I2sAudioOutput& out, int rate, int total)`
- Defined: `micro/examples/rp2350/src/main_i2s_relay.cc:140`
- Doc: Receive `total` samples from the host into RAM, then play them to the I2S amp at `rate` Hz. Returns the number of sample

### main `int main()`
- Defined: `micro/examples/rp2350/src/main_i2s_relay.cc:181`

## micro/examples/rp2350/src/main_live.cc

### main `int main()`
- Defined: `micro/examples/rp2350/src/main_live.cc:10`
- Doc: include "app_common.h" include "echo_app.h"

## micro/examples/rp2350/src/main_step1_blinky.cc

### main `int main()`
- Defined: `micro/examples/rp2350/src/main_step1_blinky.cc:10`
- Doc: include "pico/stdlib.h"

## micro/examples/rp2350/src/main_step1_blinky_w.cc

### main `int main()`
- Defined: `micro/examples/rp2350/src/main_step1_blinky_w.cc:9`
- Doc: include "pico/cyw43_arch.h" include "pico/stdlib.h"

## micro/examples/rp2350/src/main_step2_printf.cc

### LedInit `bool LedInit()`
- Defined: `micro/examples/rp2350/src/main_step2_printf.cc:16`

### LedPut `void LedPut(bool on)`
- Defined: `micro/examples/rp2350/src/main_step2_printf.cc:26`

### main `int main()`
- Defined: `micro/examples/rp2350/src/main_step2_printf.cc:36`

## micro/examples/rp2350/src/main_step3_fft.cc

### LedInit `bool LedInit()`
- Defined: `micro/examples/rp2350/src/main_step3_fft.cc:18`

### LedPut `void LedPut(bool on)`
- Defined: `micro/examples/rp2350/src/main_step3_fft.cc:28`

### main `int main()`
- Defined: `micro/examples/rp2350/src/main_step3_fft.cc:42`

## micro/examples/rp2350/src/main_step5_synth.cc

### LedInit `bool LedInit()`
- Defined: `micro/examples/rp2350/src/main_step5_synth.cc:22`

### LedPut `void LedPut(bool on)`
- Defined: `micro/examples/rp2350/src/main_step5_synth.cc:32`

### main `int main()`
- Defined: `micro/examples/rp2350/src/main_step5_synth.cc:42`

## micro/examples/rp2350/src/main_step6_decoder.cc

### LedInit `bool LedInit()`
- Defined: `micro/examples/rp2350/src/main_step6_decoder.cc:27`

### LedPut `void LedPut(bool on)`
- Defined: `micro/examples/rp2350/src/main_step6_decoder.cc:37`

### main `int main()`
- Defined: `micro/examples/rp2350/src/main_step6_decoder.cc:50`

## micro/examples/rp2350/src/main_step7_synthesize.cc

### LedInit `bool LedInit()`
- Defined: `micro/examples/rp2350/src/main_step7_synthesize.cc:34`

### LedPut `void LedPut(bool on)`
- Defined: `micro/examples/rp2350/src/main_step7_synthesize.cc:44`

### DiscardPcm `void DiscardPcm(void* user, const int16_t* samples, int n)`
- Defined: `micro/examples/rp2350/src/main_step7_synthesize.cc:55`

### PaintStack `void PaintStack()`
- Defined: `micro/examples/rp2350/src/main_step7_synthesize.cc:65`

### StackFreeBytes `uint32_t StackFreeBytes()`
- Defined: `micro/examples/rp2350/src/main_step7_synthesize.cc:73`

### main `int main()`
- Defined: `micro/examples/rp2350/src/main_step7_synthesize.cc:82`

## micro/examples/rp2350/src/main_step7b_framesweep.cc

### LedInit `bool LedInit()`
- Defined: `micro/examples/rp2350/src/main_step7b_framesweep.cc:24`

### LedPut `void LedPut(bool on)`
- Defined: `micro/examples/rp2350/src/main_step7b_framesweep.cc:34`

### PaintStack `void PaintStack()`
- Defined: `micro/examples/rp2350/src/main_step7b_framesweep.cc:50`

### StackFreeBytes `uint32_t StackFreeBytes()`
- Defined: `micro/examples/rp2350/src/main_step7b_framesweep.cc:58`

### main `int main()`
- Defined: `micro/examples/rp2350/src/main_step7b_framesweep.cc:67`

## micro/examples/rp2350/src/main_step7c_synthonly.cc

### LedInit `bool LedInit()`
- Defined: `micro/examples/rp2350/src/main_step7c_synthonly.cc:28`

### LedPut `void LedPut(bool on)`
- Defined: `micro/examples/rp2350/src/main_step7c_synthonly.cc:38`

### SynthFrame `void SynthFrame(void* /*user*/, int t, neural_tts::WorldFrame* f)`
- Defined: `micro/examples/rp2350/src/main_step7c_synthonly.cc:48`
- Doc: 100-frame voiced spans alternating with 30-frame unvoiced spans.

### DiscardPcm `void DiscardPcm(void* user, const int16_t* samples, int n)`
- Defined: `micro/examples/rp2350/src/main_step7c_synthonly.cc:63`

### PaintStack `void PaintStack()`
- Defined: `micro/examples/rp2350/src/main_step7c_synthonly.cc:73`

### StackFreeBytes `uint32_t StackFreeBytes()`
- Defined: `micro/examples/rp2350/src/main_step7c_synthonly.cc:81`

### main `int main()`
- Defined: `micro/examples/rp2350/src/main_step7c_synthonly.cc:90`

## micro/examples/rp2350/src/main_test.cc

### main `int main()`
- Defined: `micro/examples/rp2350/src/main_test.cc:11`
- Doc: include "app_common.h" include "test_app.h"

## micro/examples/rp2350/src/main_tflm_invoke_test.cc

### BeginEvent `uint32_t BeginEvent(const char* tag) override`
- Defined: `micro/examples/rp2350/src/main_tflm_invoke_test.cc:68`

### EndEvent `void EndEvent(uint32_t handle) override`
- Defined: `micro/examples/rp2350/src/main_tflm_invoke_test.cc:73`

### Reset `void Reset()`
- Defined: `micro/examples/rp2350/src/main_tflm_invoke_test.cc:76`

### Report `void Report()`
- Defined: `micro/examples/rp2350/src/main_tflm_invoke_test.cc:77`

### FeedWatchdog `bool FeedWatchdog(repeating_timer_t*)`
- Defined: `micro/examples/rp2350/src/main_tflm_invoke_test.cc:100`
- Doc: Feed the watchdog from a timer IRQ for the first ~2 minutes: single ops may legitimately run tens of seconds (reference 

### main `int main()`
- Defined: `micro/examples/rp2350/src/main_tflm_invoke_test.cc:107`

## micro/examples/rp2350/src/main_tts.cc

### main `int main()`
- Defined: `micro/examples/rp2350/src/main_tts.cc:63`

## micro/examples/rp2350/src/main_tts_ladder_test.cc

### EmitPcm `void EmitPcm(void* user, const int16_t* samples, int n)`
- Defined: `micro/examples/rp2350/src/main_tts_ladder_test.cc:90`
- Doc: if TTS_LADDER_STAGE >= 4

### main `int main()`
- Defined: `micro/examples/rp2350/src/main_tts_ladder_test.cc:103`

## micro/examples/rp2350/src/main_usb_banner_test.cc

### main `int main()`
- Defined: `micro/examples/rp2350/src/main_usb_banner_test.cc:28`

## micro/examples/rp2350/src/main_wifi.cc

### main `int main()`
- Defined: `micro/examples/rp2350/src/main_wifi.cc:16`
- Doc: include "app_common.h" include "usb_audio_io.h"  // UsbAudioInput / UsbAudioOutput include "wifi_app.h"      // RunWifiA

## micro/examples/rp2350/src/main_wifi_hardware.cc

### main `int main()`
- Defined: `micro/examples/rp2350/src/main_wifi_hardware.cc:11`
- Doc: include "app_common.h" include "wifi_hardware_app.h"

## micro/examples/rp2350/src/op_profiler.cc

### BeginEvent `uint32_t OpProfiler::BeginEvent(const char* tag)`
- Defined: `micro/examples/rp2350/src/op_profiler.cc:10`

### EndEvent `void OpProfiler::EndEvent(uint32_t event_handle)`
- Defined: `micro/examples/rp2350/src/op_profiler.cc:23`

### Report `void OpProfiler::Report(const char* label) const`
- Defined: `micro/examples/rp2350/src/op_profiler.cc:28`

## micro/examples/rp2350/src/op_profiler.h

### Reset `void Reset()`
- Defined: `micro/examples/rp2350/src/op_profiler.h:46`
- Doc: Drop all recorded events (call before each Invoke you want to measure in isolation).

### num_events `int num_events() const`
- Defined: `micro/examples/rp2350/src/op_profiler.h:50`

## micro/examples/rp2350/src/spelling_labels.h

### SpokenForLabel `inline const char* SpokenForLabel(const char* label)`
- Defined: `micro/examples/rp2350/src/spelling_labels.h:25`
- Doc: Map a class label to the text the TTS should speak. Letters are single characters 'a'..'z'; everything else (the digit w

## micro/examples/rp2350/src/test_app.cc

### RunVadDemo `void RunVadDemo(uint8_t* arena, std::size_t arena_size, kiss_fftr_state* fft)`
- Defined: `micro/examples/rp2350/src/test_app.cc:66`
- Doc: Streaming VAD demo over the embedded clips (each treated as a 1 s stream): one FFT per 32 ms hop through the MelStreamer

### RunTestApp `void RunTestApp(unsigned led_pin)`
- Defined: `micro/examples/rp2350/src/test_app.cc:146`

## micro/examples/rp2350/src/tts_service.cc

### SetBootReport `void SetBootReport(const BootReport& report)`
- Defined: `micro/examples/rp2350/src/tts_service.cc:21`

### ReadLine `int ReadLine(char* buf, int maxlen)`
- Defined: `micro/examples/rp2350/src/tts_service.cc:34`
- Doc: Read one newline-terminated line from USB CDC into `buf` (NUL-terminated), blocking until a non-empty line arrives. CR a

### EmitToUsb `void EmitToUsb(void* user, const int16_t* samples, int n)`
- Defined: `micro/examples/rp2350/src/tts_service.cc:55`
- Doc: PCM chunks stream straight to the CDC byte pipe as they render. Flush every chunk: newlib's stdout buffer otherwise hold

### RunTtsService `void RunTtsService(uint8_t* arena, std::size_t arena_size)`
- Defined: `micro/examples/rp2350/src/tts_service.cc:62`

## micro/examples/rp2350/src/usb_audio_io.cc

### ReadByteTimed `int ReadByteTimed(int timeout_ms)`
- Defined: `micro/examples/rp2350/src/usb_audio_io.cc:18`
- Doc: Read one byte, waiting up to ~timeout_ms. Returns -1 on timeout.

### ReadHop `bool UsbAudioInput::ReadHop(int16_t* out, int n)`
- Defined: `micro/examples/rp2350/src/usb_audio_io.cc:24`

### Drain `void UsbAudioInput::Drain()`
- Defined: `micro/examples/rp2350/src/usb_audio_io.cc:59`

### Begin `void UsbAudioOutput::Begin(int sample_rate, int num_samples, const char* kind)`
- Defined: `micro/examples/rp2350/src/usb_audio_io.cc:66`

### Write `void UsbAudioOutput::Write(const int16_t* samples, int n)`
- Defined: `micro/examples/rp2350/src/usb_audio_io.cc:71`

### End `void UsbAudioOutput::End()`
- Defined: `micro/examples/rp2350/src/usb_audio_io.cc:75`

## micro/examples/rp2350/src/wifi_app.cc

### DigitWord `const char* DigitWord(char c)`
- Defined: `micro/examples/rp2350/src/wifi_app.cc:50`

### SymbolChar `bool SymbolChar(const char* label, char* out)`
- Defined: `micro/examples/rp2350/src/wifi_app.cc:58`
- Doc: Symbol class label -> the character it inserts.

### SymbolWord `const char* SymbolWord(char c)`
- Defined: `micro/examples/rp2350/src/wifi_app.cc:68`
- Doc: Symbol character -> the word the TTS should say for it.

### Classify `Tok Classify(const char* label, char* out_char)`
- Defined: `micro/examples/rp2350/src/wifi_app.cc:78`

### AppendSpokenForChar `void AppendSpokenForChar(char* dst, std::size_t cap, char c)`
- Defined: `micro/examples/rp2350/src/wifi_app.cc:110`
- Doc: Append the spoken word(s) for one credential character to `dst` (a phrase builder), separated by a leading space when `d

### SpeakSpelled `void SpeakSpelled(const char* prefix, const char* text, AudioOutput& out,
                  Audio...`
- Defined: `micro/examples/rp2350/src/wifi_app.cc:133`
- Doc: Speak a credential back, spelled out ("see ay tee one"), with an optional prefix ("the name is ...").

### SpeakName `void SpeakName(const char* name, AudioOutput& out, AudioInput& in,
               uint8_t* arena,...`
- Defined: `micro/examples/rp2350/src/wifi_app.cc:147`
- Doc: Announce a network name: first say it as whole words (letting the TTS g2p pronounce the raw text), then spell it out let

### SpeakIp `void SpeakIp(AudioOutput& out, AudioInput& in, uint8_t* arena,
             std::size_t arena_size)`
- Defined: `micro/examples/rp2350/src/wifi_app.cc:156`
- Doc: Speak the current STA IPv4 address digit-by-digit ("one nine two dot ...").

### DoConnect `void DoConnect(const char* ssid, const char* pw, AudioOutput& out,
               AudioInput& in,...`
- Defined: `micro/examples/rp2350/src/wifi_app.cc:190`
- Doc: Join `ssid`/`pw` (WPA2-PSK), waiting for the link and a DHCP lease, pumping the CYW43 poll context throughout. Speaks su

### AppendChar `std::size_t AppendChar(char* buf, std::size_t len, char c, bool* caps,
                       Aud...`
- Defined: `micro/examples/rp2350/src/wifi_app.cc:222`
- Doc: Append one recognized credential character to `buf`, applying a pending caps flag, and echo it back. Returns the new len

### ScanResultCb `int ScanResultCb(void* /*env*/, const cyw43_ev_scan_result_t* r)`
- Defined: `micro/examples/rp2350/src/wifi_app.cc:254`

### ScanNetworks `void ScanNetworks(AudioInput& in)`
- Defined: `micro/examples/rp2350/src/wifi_app.cc:275`
- Doc: Scan for nearby networks into g_scan_ssids. Blocking: pumps the poll-mode CYW43 context (and drains the mic so its FIFO 

### LowerAscii `char LowerAscii(char c)`
- Defined: `micro/examples/rp2350/src/wifi_app.cc:299`

### HasPrefixCi `bool HasPrefixCi(const char* name, const char* prefix, std::size_t plen)`
- Defined: `micro/examples/rp2350/src/wifi_app.cc:305`
- Doc: Case-insensitive: does `name` begin with the `plen`-char `prefix`?

### EqualsCi `bool EqualsCi(const char* a, const char* b)`
- Defined: `micro/examples/rp2350/src/wifi_app.cc:313`

### CountPrefixMatches `int CountPrefixMatches(const char* prefix, int* only_idx)`
- Defined: `micro/examples/rp2350/src/wifi_app.cc:323`
- Doc: Count scanned SSIDs starting (case-insensitively) with `prefix`; on a single match, write its index to *only_idx.

### FindExactMatch `int FindExactMatch(const char* name)`
- Defined: `micro/examples/rp2350/src/wifi_app.cc:335`

### AnnounceMatch `void AnnounceMatch(const char* name, char* ssid, std::size_t* ssid_len,
                   AudioO...`
- Defined: `micro/examples/rp2350/src/wifi_app.cc:345`
- Doc: Adopt `name` as the chosen SSID (copied into `ssid`), say it back spelled out, and ask for confirmation. The caller then

### RunWifiAppWithIo `void RunWifiAppWithIo(AudioInput& in, AudioOutput& out)`
- Defined: `micro/examples/rp2350/src/wifi_app.cc:358`

## micro/examples/rp2350/src/wifi_hardware_app.cc

### RunWifiHardwareApp `void RunWifiHardwareApp()`
- Defined: `micro/examples/rp2350/src/wifi_hardware_app.cc:12`

## micro/feature-generation/include/feature_generation/feature_generation.h

### n_mels `int n_mels() const`
- Defined: `micro/feature-generation/include/feature_generation/feature_generation.h:119`

### target_frames `int target_frames() const`
- Defined: `micro/feature-generation/include/feature_generation/feature_generation.h:121`

### n_freq `int n_freq() const`
- Defined: `micro/feature-generation/include/feature_generation/feature_generation.h:122`

### params `const LogMelParams& params() const`
- Defined: `micro/feature-generation/include/feature_generation/feature_generation.h:123`

### filled `int filled() const`
- Defined: `micro/feature-generation/include/feature_generation/feature_generation.h:185`

### n_mels `int n_mels() const`
- Defined: `micro/feature-generation/include/feature_generation/feature_generation.h:187`

### window_frames `int window_frames() const`
- Defined: `micro/feature-generation/include/feature_generation/feature_generation.h:188`

## micro/feature-generation/scripts/generate_mel_tables.py

### _include_guard `def _include_guard(stem)`
- Defined: `micro/feature-generation/scripts/generate_mel_tables.py:28`

### hann_window_periodic `def hann_window_periodic(length)`
- Defined: `micro/feature-generation/scripts/generate_mel_tables.py:32`

### hz_to_mel_slaney `def hz_to_mel_slaney(hz)`
- Defined: `micro/feature-generation/scripts/generate_mel_tables.py:40`

### mel_to_hz_slaney `def mel_to_hz_slaney(mel)`
- Defined: `micro/feature-generation/scripts/generate_mel_tables.py:50`

### make_csr_filterbank `def make_csr_filterbank(n_freq, n_mels, sample_rate, f_min, f_max)`
- Defined: `micro/feature-generation/scripts/generate_mel_tables.py:60`

### fmt_floats `def fmt_floats(values, per_line)`
- Defined: `micro/feature-generation/scripts/generate_mel_tables.py:89`

### fmt_ints `def fmt_ints(values, per_line)`
- Defined: `micro/feature-generation/scripts/generate_mel_tables.py:97`

### main `def main()`
- Defined: `micro/feature-generation/scripts/generate_mel_tables.py:105`

## micro/feature-generation/src/log_mel.cc

### ReflectIndex `inline int ReflectIndex(int i, int n)`
- Defined: `micro/feature-generation/src/log_mel.cc:69`
- Doc: Reflect index without duplicating the boundary. Matches torch.nn.functional.pad(x, (pad, pad), mode="reflect"): index -1

### ToFloatSample `inline float ToFloatSample(float s)`
- Defined: `micro/feature-generation/src/log_mel.cc:87`
- Doc: Per-sample input conversion for ComputeImpl. Lets the STT clip be stored as raw int16 mic samples (half the SRAM of fp32

### ToFloatSample `inline float ToFloatSample(int16_t s)`
- Defined: `micro/feature-generation/src/log_mel.cc:88`

### HzToMelSlaney `float HzToMelSlaney(float hz)`
- Defined: `micro/feature-generation/src/log_mel.cc:92`

### MelToHzSlaney `float MelToHzSlaney(float mel)`
- Defined: `micro/feature-generation/src/log_mel.cc:99`

### HannWindowPeriodic `std::vector<float> HannWindowPeriodic(int length)`
- Defined: `micro/feature-generation/src/log_mel.cc:106`

### MakeMelFilterbank `std::vector<float> MakeMelFilterbank(int n_freq, int n_mels, int sample_rate,
                   ...`
- Defined: `micro/feature-generation/src/log_mel.cc:120`

### LogMelSpectrogram `LogMelSpectrogram::LogMelSpectrogram(const LogMelParams& params)
    : params_(params), n_freq_(p...`
- Defined: `micro/feature-generation/src/log_mel.cc:162`

### ComputeImpl `template <typename SampleT>
void LogMelSpectrogram::ComputeImpl(const SampleT* waveform,
        ...`
- Defined: `micro/feature-generation/src/log_mel.cc:311`

### Compute `void LogMelSpectrogram::Compute(const float* waveform, std::size_t n_samples,
                   ...`
- Defined: `micro/feature-generation/src/log_mel.cc:439`
- Doc: Public entry points: fp32 (unchanged API) and int16 (the on-device STT clip buffer). Both share the templated body above

### Compute `void LogMelSpectrogram::Compute(const int16_t* waveform, std::size_t n_samples,
                 ...`
- Defined: `micro/feature-generation/src/log_mel.cc:443`

## micro/feature-generation/src/mel_streamer.cc

### MelStreamer `MelStreamer::MelStreamer(int n_mels, int window_frames, int n_fft,
                         const...`
- Defined: `micro/feature-generation/src/mel_streamer.cc:9`

### Reset `void MelStreamer::Reset()`
- Defined: `micro/feature-generation/src/mel_streamer.cc:38`

### PushHop `void MelStreamer::PushHop(const float* hop_samples)`
- Defined: `micro/feature-generation/src/mel_streamer.cc:52`

### BuildModelInput `void MelStreamer::BuildModelInput(float* out) const`
- Defined: `micro/feature-generation/src/mel_streamer.cc:92`

## micro/feature-generation/tests/feature_generation_test.cc

### DenseToCsr `void DenseToCsr(const std::vector<float>& dense, int n_mels, int n_freq,
                std::vec...`
- Defined: `micro/feature-generation/tests/feature_generation_test.cc:24`
- Doc: Build the CSR form of the Slaney filterbank from the dense matrix, matching what a flash-table generator emits.

### TF_LITE_MICRO_TEST `TF_LITE_MICRO_TESTS_BEGIN

TF_LITE_MICRO_TEST(HannWindowPeriodicEndpoints)`
- Defined: `micro/feature-generation/tests/feature_generation_test.cc:43`

### TF_LITE_MICRO_TEST `TF_LITE_MICRO_TEST(MelScaleRoundTrip)`
- Defined: `micro/feature-generation/tests/feature_generation_test.cc:53`

### TF_LITE_MICRO_TEST `TF_LITE_MICRO_TEST(StreamerMatchesBatch)`
- Defined: `micro/feature-generation/tests/feature_generation_test.cc:60`

## micro/g2p/include/g2p/g2p_dict.h

### size `size_t size() const`
- Defined: `micro/g2p/include/g2p/g2p_dict.h:42`

### empty `bool empty() const`
- Defined: `micro/g2p/include/g2p/g2p_dict.h:44`

## micro/g2p/src/g2p.cc

### HasDigit `bool HasDigit(const std::string& s)`
- Defined: `micro/g2p/src/g2p.cc:13`

### ResolveToken `std::string ResolveToken(const std::string& tok, const Lexicon* overrides)`
- Defined: `micro/g2p/src/g2p.cc:22`
- Doc: Resolve a single token to an IPA string via the lookup pipeline.

### TextToPhones `std::vector<std::string> TextToPhones(const std::string& text,
                                  ...`
- Defined: `micro/g2p/src/g2p.cc:32`

## micro/g2p/src/g2p_dict.cc

### DecodeIpa `std::string DecodeIpa(uint32_t start, unsigned count)`
- Defined: `micro/g2p/src/g2p_dict.cc:16`
- Doc: Decode `count` packed phone ids starting at body offset `start` into IPA.

### RestartKey `std::string RestartKey(int block)`
- Defined: `micro/g2p/src/g2p_dict.cc:27`
- Doc: The restart (first) key of a block: its entry always has sharedPrefixLen == 0.

### NormalizeWordKey `std::string NormalizeWordKey(std::string_view word)`
- Defined: `micro/g2p/src/g2p_dict.cc:34`

### DictLookup `bool DictLookup(std::string_view word, std::string* ipa)`
- Defined: `micro/g2p/src/g2p_dict.cc:50`

### Add `void Lexicon::Add(std::string_view word, std::string_view ipa)`
- Defined: `micro/g2p/src/g2p_dict.cc:105`
- Doc: -------------------------------------------------------------------------- // Lexicon (runtime overrides) --------------

### EnsureSorted `void Lexicon::EnsureSorted() const`
- Defined: `micro/g2p/src/g2p_dict.cc:112`

### stable_sort `std::stable_sort(
      entries_.begin(), entries_.end(),
      [](const auto& a, const auto& b)`
- Defined: `micro/g2p/src/g2p_dict.cc:115`

### Lookup `bool Lexicon::Lookup(std::string_view word, std::string* ipa) const`
- Defined: `micro/g2p/src/g2p_dict.cc:131`

### LoadFromFile `bool Lexicon::LoadFromFile(const std::string& path)`
- Defined: `micro/g2p/src/g2p_dict.cc:144`

## micro/g2p/src/g2p_numbers.cc

### DigitSequenceIpa `std::string DigitSequenceIpa(std::string_view digits)`
- Defined: `micro/g2p/src/g2p_numbers.cc:39`

### Under100Ipa `std::string Under100Ipa(int n)`
- Defined: `micro/g2p/src/g2p_numbers.cc:50`

### Under1000Ipa `std::string Under1000Ipa(int n)`
- Defined: `micro/g2p/src/g2p_numbers.cc:60`

### CardinalNonNegativeIpa `bool CardinalNonNegativeIpa(long long n, std::string* out)`
- Defined: `micro/g2p/src/g2p_numbers.cc:69`

### IntegerDecimalStringIpa `bool IntegerDecimalStringIpa(std::string s, std::string* out)`
- Defined: `micro/g2p/src/g2p_numbers.cc:107`

### NumberWordToIpa `bool NumberWordToIpa(std::string_view token, std::string* ipa)`
- Defined: `micro/g2p/src/g2p_numbers.cc:183`

## micro/g2p/src/g2p_phones.cc

### HasDigit `bool HasDigit(const char* s)`
- Defined: `micro/g2p/src/g2p_phones.cc:15`

### ResolveTokenBuf `bool ResolveTokenBuf(const char* tok, char* out, std::size_t cap,
                     const Lexi...`
- Defined: `micro/g2p/src/g2p_phones.cc:27`
- Doc: Resolve one word token to IPA in `out` (capacity includes NUL). Peak heap use is one short std::string inside the dictio

### push `bool PhoneTokenList::push(const char* tok)`
- Defined: `micro/g2p/src/g2p_phones.cc:44`

### TokenizeIpaToList `bool TokenizeIpaToList(const char* ipa, PhoneTokenList* out)`
- Defined: `micro/g2p/src/g2p_phones.cc:52`

### TextToPhoneList `bool TextToPhoneList(const char* text, PhoneTokenList* out,
                     const Lexicon* o...`
- Defined: `micro/g2p/src/g2p_phones.cc:60`

## micro/g2p/src/g2p_rules.cc

### Utf8StartsWith `bool Utf8StartsWith(const std::string& s, std::string_view p)`
- Defined: `micro/g2p/src/g2p_rules.cc:18`

### LastUtf8Char `std::string_view LastUtf8Char(std::string_view s)`
- Defined: `micro/g2p/src/g2p_rules.cc:22`

### LastIpaUnitIsVowel `bool LastIpaUnitIsVowel(std::string_view prev)`
- Defined: `micro/g2p/src/g2p_rules.cc:33`

### IsVowel `constexpr bool IsVowel(char c)`
- Defined: `micro/g2p/src/g2p_rules.cc:46`

### IsConsonant `constexpr bool IsConsonant(char c)`
- Defined: `micro/g2p/src/g2p_rules.cc:50`

### NextVowelIndex `int NextVowelIndex(std::string_view w, int start)`
- Defined: `micro/g2p/src/g2p_rules.cc:54`

### MagicELengthens `bool MagicELengthens(std::string_view w, int vowel_i)`
- Defined: `micro/g2p/src/g2p_rules.cc:61`

### ThVoicedWord `bool ThVoicedWord(std::string_view w)`
- Defined: `micro/g2p/src/g2p_rules.cc:200`

### SingleConsonant `std::string SingleConsonant(char c, std::string_view w, int i)`
- Defined: `micro/g2p/src/g2p_rules.cc:206`

### AddPrimaryStressIfMissing `std::string AddPrimaryStressIfMissing(std::string s)`
- Defined: `micro/g2p/src/g2p_rules.cc:351`

### GraphemeToIpa `std::string GraphemeToIpa(std::string_view word)`
- Defined: `micro/g2p/src/g2p_rules.cc:370`

### RulesWordToIpa `std::string RulesWordToIpa(std::string_view word)`
- Defined: `micro/g2p/src/g2p_rules.cc:450`

### LetterHomophoneToIpa `bool LetterHomophoneToIpa(std::string_view word, std::string* ipa)`
- Defined: `micro/g2p/src/g2p_rules.cc:466`

## micro/g2p/src/ipa_tokens.cc

### IsDirectAscii `bool IsDirectAscii(char c)`
- Defined: `micro/g2p/src/ipa_tokens.cc:81`
- Doc: Single ASCII phones that map straight to a table key (and aren't covered by the rule table above).

### Utf8Len `size_t Utf8Len(unsigned char lead)`
- Defined: `micro/g2p/src/ipa_tokens.cc:107`

### TokenizeIpa `std::vector<std::string> TokenizeIpa(const std::string& ipa)`
- Defined: `micro/g2p/src/ipa_tokens.cc:117`

## micro/klatt-tts/include/tts/klatt.h

### Step `inline float Step(float x)`
- Defined: `micro/klatt-tts/include/tts/klatt.h:51`

### Reset `void Reset()`
- Defined: `micro/klatt-tts/include/tts/klatt.h:57`

### Step `inline float Step(float x)`
- Defined: `micro/klatt-tts/include/tts/klatt.h:108`

### Reset `void Reset()`
- Defined: `micro/klatt-tts/include/tts/klatt.h:116`

### Step `inline float Step(float x)`
- Defined: `micro/klatt-tts/include/tts/klatt.h:125`

### Reset `void Reset()`
- Defined: `micro/klatt-tts/include/tts/klatt.h:131`

## micro/klatt-tts/include/tts/synth_stream.h

### done `bool done() const`
- Defined: `micro/klatt-tts/include/tts/synth_stream.h:72`

### sample_rate `int sample_rate() const`
- Defined: `micro/klatt-tts/include/tts/synth_stream.h:76`

### total_samples `int total_samples() const`
- Defined: `micro/klatt-tts/include/tts/synth_stream.h:77`

### ArenaReset `void ArenaReset()`
- Defined: `micro/klatt-tts/include/tts/synth_stream.h:84`

## micro/klatt-tts/src/config.cc

### ClassName `const char* ClassName(PhoneClass c)`
- Defined: `micro/klatt-tts/src/config.cc:13`

### SourceName `const char* SourceName(Source s)`
- Defined: `micro/klatt-tts/src/config.cc:33`

### SetPhoneField `bool SetPhoneField(Phone& p, const std::string& field, float v)`
- Defined: `micro/klatt-tts/src/config.cc:105`
- Doc: Apply one "<field> <value>" override to a phone. Returns false if `field` is not a recognized numeric field.

### Lookup `const Phone* VoiceParams::Lookup(const std::string& ipa) const`
- Defined: `micro/klatt-tts/src/config.cc:138`

### DefaultVoiceParams `VoiceParams DefaultVoiceParams()`
- Defined: `micro/klatt-tts/src/config.cc:145`

### LoadVoiceConfig `bool LoadVoiceConfig(const std::string& path, VoiceParams& vp)`
- Defined: `micro/klatt-tts/src/config.cc:151`

### DumpVoiceConfig `bool DumpVoiceConfig(const std::string& path, const VoiceParams& vp)`
- Defined: `micro/klatt-tts/src/config.cc:215`

## micro/klatt-tts/src/klatt.cc

### GlottalPulse `inline float GlottalPulse(float phase, float open, float close)`
- Defined: `micro/klatt-tts/src/klatt.cc:16`
- Doc: Rosenberg-style glottal flow pulse as a function of phase in [0, 1). Open phase rises (cos), then a shorter closing phas

### TiltCoef `float TiltCoef(float tilt_db, float sample_rate)`
- Defined: `micro/klatt-tts/src/klatt.cc:29`
- Doc: One-pole low-pass coefficient `c` (y = (1-c)x + c*y1) such that the response is `tilt_db` down at 3 kHz. Returns 0 (bypa

### SetParams `void Resonator::SetParams(float freq_hz, float bw_hz, float sample_rate)`
- Defined: `micro/klatt-tts/src/klatt.cc:47`

### SetBandpass `void Biquad::SetBandpass(float freq_hz, float q, float sample_rate)`
- Defined: `micro/klatt-tts/src/klatt.cc:54`

### SetParams `void Antiresonator::SetParams(float freq_hz, float bw_hz, float sample_rate)`
- Defined: `micro/klatt-tts/src/klatt.cc:69`

### KlattSynth `KlattSynth::KlattSynth(float sample_rate, const KlattParams& params)
    : sample_rate_(sample_ra...`
- Defined: `micro/klatt-tts/src/klatt.cc:81`

### EnsureLfShape `void KlattSynth::EnsureLfShape(float rd)`
- Defined: `micro/klatt-tts/src/klatt.cc:94`
- Doc: Map Fant's single Rd parameter to the LF glottal-flow-derivative shape, in time normalized to one pitch period (T0 = 1).

### LfDeriv `inline float KlattSynth::LfDeriv(float phase) const`
- Defined: `micro/klatt-tts/src/klatt.cc:165`
- Doc: Normalized LF flow derivative; the negative excitation peak (at te) == -1.

### NextNoise `float KlattSynth::NextNoise()`
- Defined: `micro/klatt-tts/src/klatt.cc:172`

### RenderFrame `void KlattSynth::RenderFrame(const SynthFrame& cur, const SynthFrame& nxt,
                      ...`
- Defined: `micro/klatt-tts/src/klatt.cc:180`

### Render `std::vector<float> KlattSynth::Render(const std::vector<SynthFrame>& frames,
                    ...`
- Defined: `micro/klatt-tts/src/klatt.cc:295`

## micro/klatt-tts/src/phonemes.cc

### LookupPhone `const Phone* LookupPhone(const std::string& ipa)`
- Defined: `micro/klatt-tts/src/phonemes.cc:89`

### DefaultPhoneTable `std::vector<Phone> DefaultPhoneTable()`
- Defined: `micro/klatt-tts/src/phonemes.cc:95`

## micro/klatt-tts/src/synth_internal.cc

### SegFromPhone `Segment SegFromPhone(const Phone& p)`
- Defined: `micro/klatt-tts/src/synth_internal.cc:14`

### AppendStop `void AppendStop(const Phone& p, const VoiceParams& vp, int src_token,
                Segment* ou...`
- Defined: `micro/klatt-tts/src/synth_internal.cc:38`
- Doc: Expand a stop into closure -> burst -> (aspiration) sub-segments so that voice-onset-time distinguishes /p t k/ from /b 

### BuildSegments `int BuildSegments(const char* const* phones, int n_phones, const VoiceParams& vp,
               ...`
- Defined: `micro/klatt-tts/src/synth_internal.cc:74`

### BuildSegments `std::vector<Segment> BuildSegments(const std::vector<std::string>& phones,
                      ...`
- Defined: `micro/klatt-tts/src/synth_internal.cc:175`

### SmoothBidir `void SmoothBidir(float* v, size_t n, float tau_ms)`
- Defined: `micro/klatt-tts/src/synth_internal.cc:189`

### SmoothFwd `void SmoothFwd(float* v, size_t n, float tau_ms)`
- Defined: `micro/klatt-tts/src/synth_internal.cc:200`

### SmoothAsym `void SmoothAsym(float* v, size_t n, float attack_ms, float release_ms)`
- Defined: `micro/klatt-tts/src/synth_internal.cc:208`

### CountFrames `size_t CountFrames(const std::vector<Segment>& segs, float dur_scale)`
- Defined: `micro/klatt-tts/src/synth_internal.cc:221`

### FillParamTracks `void FillParamTracks(const std::vector<Segment>& segs, const VoiceParams& vp,
                   ...`
- Defined: `micro/klatt-tts/src/synth_internal.cc:231`

### FrameAt `SynthFrame FrameAt(const ParamTracks& t, size_t i)`
- Defined: `micro/klatt-tts/src/synth_internal.cc:338`

### MakeKlattParams `KlattParams MakeKlattParams(const VoiceParams& vp)`
- Defined: `micro/klatt-tts/src/synth_internal.cc:357`

## micro/klatt-tts/src/synth_stream.cc

### SoftClip `inline float SoftClip(float x)`
- Defined: `micro/klatt-tts/src/synth_stream.cc:18`
- Doc: Soft limiter: perfectly linear up to a knee (so the RMS body of the signal is untouched), then a saturating soft knee th

### StreamSynth `StreamSynth::StreamSynth(const VoiceParams& vp, uint8_t* arena,
                         size_t a...`
- Defined: `micro/klatt-tts/src/synth_stream.cc:29`

### ArenaBytes `uint8_t* StreamSynth::ArenaBytes(size_t count, size_t align)`
- Defined: `micro/klatt-tts/src/synth_stream.cc:33`

### ArenaFloats `float* StreamSynth::ArenaFloats(size_t count)`
- Defined: `micro/klatt-tts/src/synth_stream.cc:40`

### BeginText `int StreamSynth::BeginText(const char* text, const StreamOptions& opts,
                         ...`
- Defined: `micro/klatt-tts/src/synth_stream.cc:45`

### BeginIpa `int StreamSynth::BeginIpa(const char* ipa, const StreamOptions& opts)`
- Defined: `micro/klatt-tts/src/synth_stream.cc:53`

### BeginPhones `int StreamSynth::BeginPhones(const std::vector<std::string>& phones,
                            ...`
- Defined: `micro/klatt-tts/src/synth_stream.cc:59`

### RenderNextFrame `void StreamSynth::RenderNextFrame()`
- Defined: `micro/klatt-tts/src/synth_stream.cc:124`

### Read `int StreamSynth::Read(float* out, int max_samples)`
- Defined: `micro/klatt-tts/src/synth_stream.cc:139`

## micro/klatt-tts/tests/tts_test.cc

### Contains `bool Contains(const std::vector<std::string>& toks, const char* needle)`
- Defined: `micro/klatt-tts/tests/tts_test.cc:16`

### TF_LITE_MICRO_TEST `TF_LITE_MICRO_TESTS_BEGIN

TF_LITE_MICRO_TEST(G2PProducesPhones)`
- Defined: `micro/klatt-tts/tests/tts_test.cc:25`

### TF_LITE_MICRO_TEST `TF_LITE_MICRO_TEST(G2PNumberNormalization)`
- Defined: `micro/klatt-tts/tests/tts_test.cc:34`

### TF_LITE_MICRO_TEST `TF_LITE_MICRO_TEST(StreamSynthProducesAudioInRange)`
- Defined: `micro/klatt-tts/tests/tts_test.cc:40`

## micro/neural-tts/host/tflm_ref/add.cpp

### EvalAdd `TfLiteStatus EvalAdd(TfLiteContext* context, TfLiteNode* node,
                     TfLiteAddPara...`
- Defined: `micro/neural-tts/host/tflm_ref/add.cpp:34`

### EvalAddQuantized `TfLiteStatus EvalAddQuantized(TfLiteContext* context, TfLiteNode* node,
                         ...`
- Defined: `micro/neural-tts/host/tflm_ref/add.cpp:90`

### AddInit `void* AddInit(TfLiteContext* context, const char* buffer, size_t length)`
- Defined: `micro/neural-tts/host/tflm_ref/add.cpp:162`

### AddEval `TfLiteStatus AddEval(TfLiteContext* context, TfLiteNode* node)`
- Defined: `micro/neural-tts/host/tflm_ref/add.cpp:167`

### Register_ADD `TFLMRegistration Register_ADD()`
- Defined: `micro/neural-tts/host/tflm_ref/add.cpp:195`

## micro/neural-tts/host/tflm_ref/conv.cpp

### ConvEval `TfLiteStatus ConvEval(TfLiteContext* context, TfLiteNode* node)`
- Defined: `micro/neural-tts/host/tflm_ref/conv.cpp:37`

### Register_CONV_2D `TFLMRegistration Register_CONV_2D()`
- Defined: `micro/neural-tts/host/tflm_ref/conv.cpp:128`

## micro/neural-tts/host/tflm_ref/host_platform.cpp

### InitializeTarget `void InitializeTarget()`
- Defined: `micro/neural-tts/host/tflm_ref/host_platform.cpp:25`

### ticks_per_second `uint32_t ticks_per_second()`
- Defined: `micro/neural-tts/host/tflm_ref/host_platform.cpp:27`

### GetCurrentTimeTicks `uint32_t GetCurrentTimeTicks()`
- Defined: `micro/neural-tts/host/tflm_ref/host_platform.cpp:29`

## micro/neural-tts/host/tflm_ref/transpose_conv.cpp

### RuntimePaddingType `inline PaddingType RuntimePaddingType(TfLitePadding padding)`
- Defined: `micro/neural-tts/host/tflm_ref/transpose_conv.cpp:59`

### CalculateOpData `TfLiteStatus CalculateOpData(TfLiteContext* context, TfLiteNode* node,
                          ...`
- Defined: `micro/neural-tts/host/tflm_ref/transpose_conv.cpp:71`

### TransposeConvInit `void* TransposeConvInit(TfLiteContext* context, const char* buffer,
                        size_...`
- Defined: `micro/neural-tts/host/tflm_ref/transpose_conv.cpp:145`

### TransposeConvPrepare `TfLiteStatus TransposeConvPrepare(TfLiteContext* context, TfLiteNode* node)`
- Defined: `micro/neural-tts/host/tflm_ref/transpose_conv.cpp:151`

### TransposeConvEval `TfLiteStatus TransposeConvEval(TfLiteContext* context, TfLiteNode* node)`
- Defined: `micro/neural-tts/host/tflm_ref/transpose_conv.cpp:260`

### Register_TRANSPOSE_CONV `TFLMRegistration Register_TRANSPOSE_CONV()`
- Defined: `micro/neural-tts/host/tflm_ref/transpose_conv.cpp:409`

## micro/neural-tts/host/tts_cli.cc

### ReadFile `std::vector<uint8_t> ReadFile(const char* path)`
- Defined: `micro/neural-tts/host/tts_cli.cc:31`

### WriteWavHeader `void WriteWavHeader(FILE* f, int rate, int nsamples)`
- Defined: `micro/neural-tts/host/tts_cli.cc:46`

### Emit `void Emit(void* user, const int16_t* samples, int n)`
- Defined: `micro/neural-tts/host/tts_cli.cc:70`

### main `int main(int argc, char** argv)`
- Defined: `micro/neural-tts/host/tts_cli.cc:77`

## micro/neural-tts/host/worldlite_synth_cli.cc

### main `int main(int argc, char** argv)`
- Defined: `micro/neural-tts/host/worldlite_synth_cli.cc:14`
- Doc: include "neural_tts/worldlite_synth.h"

## micro/neural-tts/include/neural_tts/neural_tts.h

### ok `bool ok() const`
- Defined: `micro/neural-tts/include/neural_tts/neural_tts.h:48`

### stats `const Stats& stats() const`
- Defined: `micro/neural-tts/include/neural_tts/neural_tts.h:84`

## micro/neural-tts/include/neural_tts/pack_format.h

### Pack `public:
  explicit Pack(const uint8_t* base)
      : base_(base),
        h_(reinterpret_cast<con...`
- Defined: `micro/neural-tts/include/neural_tts/pack_format.h:142`

### ok `bool ok() const`
- Defined: `micro/neural-tts/include/neural_tts/pack_format.h:146`

### h `const PackHeader& h() const`
- Defined: `micro/neural-tts/include/neural_tts/pack_format.h:151`

### raw `const uint8_t* raw(uint32_t off) const`
- Defined: `micro/neural-tts/include/neural_tts/pack_format.h:152`

### model `const unsigned char* model() const`
- Defined: `micro/neural-tts/include/neural_tts/pack_format.h:153`

### codebook `const int8_t* codebook(int s) const`
- Defined: `micro/neural-tts/include/neural_tts/pack_format.h:155`

### codebook_scale `const float* codebook_scale(int s) const`
- Defined: `micro/neural-tts/include/neural_tts/pack_format.h:158`

### dtypes `const DiphoneTypeRec* dtypes() const`
- Defined: `micro/neural-tts/include/neural_tts/pack_format.h:161`

### dunits `const DiphoneUnitRec* dunits() const`
- Defined: `micro/neural-tts/include/neural_tts/pack_format.h:164`

### wunits `const WordUnitRec* wunits() const`
- Defined: `micro/neural-tts/include/neural_tts/pack_format.h:167`

### wkeys `const uint8_t* wkeys() const`
- Defined: `micro/neural-tts/include/neural_tts/pack_format.h:170`

### centroid `const int8_t* centroid(int type_idx) const`
- Defined: `micro/neural-tts/include/neural_tts/pack_format.h:171`

### codes `const uint8_t* codes(uint32_t off) const`
- Defined: `micro/neural-tts/include/neural_tts/pack_format.h:175`

### f0_stream `const uint8_t* f0_stream(uint32_t off) const`
- Defined: `micro/neural-tts/include/neural_tts/pack_format.h:178`

### phone_token `const char* phone_token(int id) const`
- Defined: `micro/neural-tts/include/neural_tts/pack_format.h:181`

### dur_ratio `const float* dur_ratio() const`
- Defined: `micro/neural-tts/include/neural_tts/pack_format.h:184`

### phone_class `const uint8_t* phone_class() const`
- Defined: `micro/neural-tts/include/neural_tts/pack_format.h:187`

### func_idx `const uint16_t* func_idx() const`
- Defined: `micro/neural-tts/include/neural_tts/pack_format.h:188`

### func_blob `const uint8_t* func_blob() const`
- Defined: `micro/neural-tts/include/neural_tts/pack_format.h:191`

## micro/neural-tts/include/neural_tts/pb_decoder.h

### ok `bool ok() const`
- Defined: `micro/neural-tts/include/neural_tts/pb_decoder.h:54`

### decode_us `uint64_t decode_us() const`
- Defined: `micro/neural-tts/include/neural_tts/pb_decoder.h:75`
- Doc: cumulative microseconds spent inside TFLM Invoke() + latent prep

### tiles_decoded `int tiles_decoded() const`
- Defined: `micro/neural-tts/include/neural_tts/pb_decoder.h:76`

## micro/neural-tts/include/neural_tts/worldlite_synth.h

### KissFftrPlanBytes `inline size_t KissFftrPlanBytes(int nfft, int inverse_fft)`
- Defined: `micro/neural-tts/include/neural_tts/worldlite_synth.h:39`
- Doc: Bytes kiss_fftr_alloc needs for one real-FFT plan (query with mem=nullptr).

### KissFftrPairBytes `inline size_t KissFftrPairBytes(int nfft)`
- Defined: `micro/neural-tts/include/neural_tts/worldlite_synth.h:46`
- Doc: Forward + inverse plan storage for Synthesize() (typically ~21 KiB at nfft=1024).

### ok `bool ok() const`
- Defined: `micro/neural-tts/include/neural_tts/worldlite_synth.h:82`
- Doc: False if kissfft plan setup failed; using the synth in that state chases garbage plan state forever.

### fwd_plan `const void* fwd_plan() const`
- Defined: `micro/neural-tts/include/neural_tts/worldlite_synth.h:87`
- Doc: Bring-up: plan pointers + a self-test that runs one forward+inverse FFT pair through the plans (the on-device pipeline l

### inv_plan `const void* inv_plan() const`
- Defined: `micro/neural-tts/include/neural_tts/worldlite_synth.h:88`

## micro/neural-tts/src/neural_tts.cc

### NowUs `inline uint64_t NowUs()`
- Defined: `micro/neural-tts/src/neural_tts.cc:54`

### Exp10 `inline float Exp10(float x)`
- Defined: `micro/neural-tts/src/neural_tts.cc:90`

### BitReader `public:
  explicit BitReader(const uint8_t* p) : p_(p)`
- Defined: `micro/neural-tts/src/neural_tts.cc:121`

### get `uint32_t get(int bits)`
- Defined: `micro/neural-tts/src/neural_tts.cc:123`

### ReadVarU8 `int ReadVarU8(const uint8_t*& p)`
- Defined: `micro/neural-tts/src/neural_tts.cc:139`

### DecodeF0Stream `void DecodeF0Stream(const uint8_t* p, int n_frames, float* out,
                    F0RunSpan* runs)`
- Defined: `micro/neural-tts/src/neural_tts.cc:163`
- Doc: Decode a unit's f0 side stream into per-frame Hz (0 = unvoiced).

### F0FromCode `inline float F0FromCode(uint8_t q)`
- Defined: `micro/neural-tts/src/neural_tts.cc:212`

### Bump `public:
  Bump(uint8_t* base, size_t size) : base_(base), size_(size)`
- Defined: `micro/neural-tts/src/neural_tts.cc:235`

### Alloc `void* Alloc(size_t bytes, size_t align = 4)`
- Defined: `micro/neural-tts/src/neural_tts.cc:237`

### AllocArray `template <typename T>
  T* AllocArray(size_t n, size_t align = 4)`
- Defined: `micro/neural-tts/src/neural_tts.cc:243`

### Mark `size_t Mark() const`
- Defined: `micro/neural-tts/src/neural_tts.cc:247`

### Reset `void Reset(size_t mark)`
- Defined: `micro/neural-tts/src/neural_tts.cc:248`

### remaining `size_t remaining() const`
- Defined: `micro/neural-tts/src/neural_tts.cc:249`

### Engine `public:
  Engine(const Pack& pk, uint8_t* arena, size_t arena_size,
         NeuralTts::Stats* st...`
- Defined: `micro/neural-tts/src/neural_tts.cc:261`

### IsSil `bool IsSil(int pid) const`
- Defined: `micro/neural-tts/src/neural_tts.cc:291`

### IsGap `bool IsGap(int pid) const`
- Defined: `micro/neural-tts/src/neural_tts.cc:296`

### Canon `int Canon(int pid) const`
- Defined: `micro/neural-tts/src/neural_tts.cc:299`

### TimedEmit `static void TimedEmit(void* user, const int16_t* samples, int n)`
- Defined: `micro/neural-tts/src/neural_tts.cc:342`

### BlendLenUnit `static int BlendLenUnit(int rule_n, int nat_n)`
- Defined: `micro/neural-tts/src/neural_tts.cc:351`

### PhoneId `int Engine::PhoneId(const char* token) const`
- Defined: `micro/neural-tts/src/neural_tts.cc:437`

### BuildRunsFromPtrs `int Engine::BuildRunsFromPtrs(const char* const* tokens, int n_tokens)`
- Defined: `micro/neural-tts/src/neural_tts.cc:446`

### BuildRuns `int Engine::BuildRuns(const std::vector<std::string>& tokens)`
- Defined: `micro/neural-tts/src/neural_tts.cc:491`

### FindDiphoneType `int Engine::FindDiphoneType(int a, int b) const`
- Defined: `micro/neural-tts/src/neural_tts.cc:498`

### KeyCompare `static int KeyCompare(const uint8_t* a, int la, const uint8_t* b, int lb)`
- Defined: `micro/neural-tts/src/neural_tts.cc:516`
- Doc: Lexicographic compare of two phone-id keys.

### FindWord `int Engine::FindWord(const uint8_t* key, int len) const`
- Defined: `micro/neural-tts/src/neural_tts.cc:523`

### RunAfterBuild `int Engine::RunAfterBuild(NeuralTts::EmitFn emit, void* user, bool plan_only)`
- Defined: `micro/neural-tts/src/neural_tts.cc:546`
- Doc: --------------------------------------------------------------------------

### Run `int Engine::Run(std::vector<std::string>* tokens, NeuralTts::EmitFn emit,
                void* u...`
- Defined: `micro/neural-tts/src/neural_tts.cc:596`

### Run `int Engine::Run(const g2p::PhoneTokenList* phones, NeuralTts::EmitFn emit,
                void* ...`
- Defined: `micro/neural-tts/src/neural_tts.cc:609`
- Doc: if defined(PICO_BUILD)

### ComputeProsodyBuckets `void Engine::ComputeProsodyBuckets(int n)`
- Defined: `micro/neural-tts/src/neural_tts.cc:621`
- Doc: endif

### ProsOff `float Engine::ProsOff(const float* table, int chunk_start) const`
- Defined: `micro/neural-tts/src/neural_tts.cc:697`

### SegOff `float Engine::SegOff(const float* table, int seg) const`
- Defined: `micro/neural-tts/src/neural_tts.cc:702`

### MatchWords `void Engine::MatchWords(int n)`
- Defined: `micro/neural-tts/src/neural_tts.cc:706`

### SelectDiphones `void Engine::SelectDiphones(int n)`
- Defined: `micro/neural-tts/src/neural_tts.cc:806`

### BuildParts `void Engine::BuildParts(int n)`
- Defined: `micro/neural-tts/src/neural_tts.cc:927`

### UnpackCodes `void Engine::UnpackCodes(uint32_t codes_off, int n_latents, uint16_t* out)`
- Defined: `micro/neural-tts/src/neural_tts.cc:1080`

### DecodedRows `const int16_t* Engine::DecodedRows(bool word, int idx, int frame_base,
                          ...`
- Defined: `micro/neural-tts/src/neural_tts.cc:1096`

### WarpPositions `static void WarpPositions(int m, int n, float* pos)`
- Defined: `micro/neural-tts/src/neural_tts.cc:1129`
- Doc: warp positions (synth_diphone_world.py warp / warp_anchored)

### WarpAnchoredPositions `static void WarpAnchoredPositions(int m, int n, bool anchor_end,
                                ...`
- Defined: `micro/neural-tts/src/neural_tts.cc:1138`

### BuildRanges `int Engine::BuildRanges(const Part& p, int T, Range ranges[2]) const`
- Defined: `micro/neural-tts/src/neural_tts.cc:1166`

### MaterializeF0 `void Engine::MaterializeF0()`
- Defined: `micro/neural-tts/src/neural_tts.cc:1187`
- Doc: f0 prepass: the pitch track comes entirely from the flash-side f0 streams (never from the TFLM decoder), so the full-utt

### MaterializePartTrack `void Engine::MaterializePartTrack(int pi)`
- Defined: `micro/neural-tts/src/neural_tts.cc:1243`
- Doc: Write the track rows (benv/bap, NOT f0_: that's already final) of one part. Parts are materialized strictly in order, ma

### GainEqAt `void Engine::GainEqAt(int pi)`
- Defined: `micro/neural-tts/src/neural_tts.cc:1343`

### SmoothJoinAt `void Engine::SmoothJoinAt(int j)`
- Defined: `micro/neural-tts/src/neural_tts.cc:1391`

### FrameLnEnergy `float Engine::FrameLnEnergy(int t) const`
- Defined: `micro/neural-tts/src/neural_tts.cc:1422`

### LoudKnotAt `static float LoudKnotAt(const int8_t* k, float scale, float u)`
- Defined: `micro/neural-tts/src/neural_tts.cc:1433`
- Doc: Interpolate a unit's baked loudness knots at unit fraction u in [0, 1], returning LSA (natural-log summed-band amplitude

### PlanLoudness `void Engine::PlanLoudness()`
- Defined: `micro/neural-tts/src/neural_tts.cc:1443`

### AdvanceJoins `void Engine::AdvanceJoins()`
- Defined: `micro/neural-tts/src/neural_tts.cc:1546`

### EnsureFinal `void Engine::EnsureFinal(int t)`
- Defined: `micro/neural-tts/src/neural_tts.cc:1579`

### F0Pass `void Engine::F0Pass()`
- Defined: `micro/neural-tts/src/neural_tts.cc:1599`

### RenderGetFrame `static void RenderGetFrame(void* user, int t, WorldFrame* frame)`
- Defined: `micro/neural-tts/src/neural_tts.cc:1694`

### SynthesizeChunk `int Engine::SynthesizeChunk(int lo, int hi, bool first, bool last,
                            Ne...`
- Defined: `micro/neural-tts/src/neural_tts.cc:1719`

### NeuralTts `NeuralTts::NeuralTts(const uint8_t* pack, uint8_t* arena, size_t arena_size)
    : pack_(pack), a...`
- Defined: `micro/neural-tts/src/neural_tts.cc:1969`
- Doc: --------------------------------------------------------------------------

### SynthesizeTokens `int NeuralTts::SynthesizeTokens(void* tokens_vec, EmitFn emit, void* user,
                      ...`
- Defined: `micro/neural-tts/src/neural_tts.cc:1974`

### Synthesize `int NeuralTts::Synthesize(const char* text, EmitFn emit, void* user)`
- Defined: `micro/neural-tts/src/neural_tts.cc:1983`

### SynthesizeIpa `int NeuralTts::SynthesizeIpa(const char* ipa, EmitFn emit, void* user)`
- Defined: `micro/neural-tts/src/neural_tts.cc:2000`

### EstimateSamples `int NeuralTts::EstimateSamples(const char* text)`
- Defined: `micro/neural-tts/src/neural_tts.cc:2017`

### EstimateSamplesIpa `int NeuralTts::EstimateSamplesIpa(const char* ipa)`
- Defined: `micro/neural-tts/src/neural_tts.cc:2034`

## micro/neural-tts/src/pb_decoder.cc

### NowUs `uint64_t NowUs()`
- Defined: `micro/neural-tts/src/pb_decoder.cc:36`

### Exp10 `inline float Exp10(float x)`
- Defined: `micro/neural-tts/src/pb_decoder.cc:47`
- Doc: exp10f(x) = 10^x for the benv dB/20 -> amplitude conversion

### BeginEvent `public:
  uint32_t BeginEvent(const char*) override`
- Defined: `micro/neural-tts/src/pb_decoder.cc:56`

### EndEvent `void EndEvent(uint32_t) override`
- Defined: `micro/neural-tts/src/pb_decoder.cc:62`

### Reset `void Reset()`
- Defined: `micro/neural-tts/src/pb_decoder.cc:63`

### PbDecoder `PbDecoder::PbDecoder(const Config& config, uint8_t* arena,
                     size_t arena_byte...`
- Defined: `micro/neural-tts/src/pb_decoder.cc:72`

### arena_used_bytes `size_t PbDecoder::arena_used_bytes() const`
- Defined: `micro/neural-tts/src/pb_decoder.cc:130`

### BeginUtterance `void PbDecoder::BeginUtterance(const PbCodedUtterance* utt)`
- Defined: `micro/neural-tts/src/pb_decoder.cc:134`

### DecodeTileAt `bool PbDecoder::DecodeTileAt(int latent_start)`
- Defined: `micro/neural-tts/src/pb_decoder.cc:143`

### GetFrame `void PbDecoder::GetFrame(int t, WorldFrame* frame)`
- Defined: `micro/neural-tts/src/pb_decoder.cc:200`

### GetFrameThunk `void PbDecoder::GetFrameThunk(void* user, int t, WorldFrame* frame)`
- Defined: `micro/neural-tts/src/pb_decoder.cc:234`

### ReadRows `void PbDecoder::ReadRows(int t0, int n, int16_t* out)`
- Defined: `micro/neural-tts/src/pb_decoder.cc:238`

## micro/neural-tts/src/worldlite_synth.cc

### HzToMel `float HzToMel(float hz)`
- Defined: `micro/neural-tts/src/worldlite_synth.cc:47`

### InitTables `void WorldLiteSynth::InitTables()`
- Defined: `micro/neural-tts/src/worldlite_synth.cc:51`

### WorldLiteSynth `WorldLiteSynth::WorldLiteSynth() : rng_state_(0x8f1bbcdcu), owns_fft_plans_(true)`
- Defined: `micro/neural-tts/src/worldlite_synth.cc:88`

### WorldLiteSynth `WorldLiteSynth::WorldLiteSynth(void* plan_mem, size_t plan_mem_bytes)
    : rng_state_(0x8f1bbcdc...`
- Defined: `micro/neural-tts/src/worldlite_synth.cc:94`

### FftSelfTest `float WorldLiteSynth::FftSelfTest()`
- Defined: `micro/neural-tts/src/worldlite_synth.cc:126`

### Randn `float WorldLiteSynth::Randn()`
- Defined: `micro/neural-tts/src/worldlite_synth.cc:142`

### ExpandFrame `void WorldLiteSynth::ExpandFrame(const WorldFrame& f, float* spec_pow,
                          ...`
- Defined: `micro/neural-tts/src/worldlite_synth.cc:154`

### MinimumPhase `void WorldLiteSynth::MinimumPhase(const float* log_amp_half,
                                  ki...`
- Defined: `micro/neural-tts/src/worldlite_synth.cc:170`

### RenderPulse `void WorldLiteSynth::RenderPulse(const float* spec_pow, const float* ap,
                        ...`
- Defined: `micro/neural-tts/src/worldlite_synth.cc:199`

### FlushTo `void WorldLiteSynth::FlushTo(int abs_pos, float gain, EmitFn emit,
                             v...`
- Defined: `micro/neural-tts/src/worldlite_synth.cc:295`

### Synthesize `void WorldLiteSynth::Synthesize(GetFrameFn get_frame, void* frame_user,
                         ...`
- Defined: `micro/neural-tts/src/worldlite_synth.cc:314`

## micro/stt-training/stt_training/augment.py

### __init__ `def __init__(self, sample_rate, musan_noise_dir, rir_dir, gain_db, noise_snr_min, noise_snr_max, bandpass_p, max_rirs, max_noise_seconds, seed)`
- Defined: `micro/stt-training/stt_training/augment.py:36`
- Imported by: `micro/stt-training/stt_training/train.py`

### _load_concat_noise `def _load_concat_noise(self, noise_dir, max_seconds)`
- Defined: `micro/stt-training/stt_training/augment.py:82`
- Imported by: `micro/stt-training/stt_training/train.py`

### _load_rirs `def _load_rirs(self, rir_dir, max_rirs)`
- Defined: `micro/stt-training/stt_training/augment.py:106`
- Imported by: `micro/stt-training/stt_training/train.py`

### n_transforms `def n_transforms(self)`
- Defined: `micro/stt-training/stt_training/augment.py:139`
- Imported by: `micro/stt-training/stt_training/train.py`

### has_external_data `def has_external_data(self)`
- Defined: `micro/stt-training/stt_training/augment.py:143`
- Imported by: `micro/stt-training/stt_training/train.py`

### _mask `def _mask(p, b, dev)`
- Defined: `micro/stt-training/stt_training/augment.py:148`
- Imported by: `micro/stt-training/stt_training/train.py`

### _rms `def _rms(x)`
- Defined: `micro/stt-training/stt_training/augment.py:152`
- Imported by: `micro/stt-training/stt_training/train.py`

### _gain `def _gain(self, x, b, dev)`
- Defined: `micro/stt-training/stt_training/augment.py:155`
- Imported by: `micro/stt-training/stt_training/train.py`

### _polarity `def _polarity(self, x, b, dev)`
- Defined: `micro/stt-training/stt_training/augment.py:161`
- Imported by: `micro/stt-training/stt_training/train.py`

### _shift `def _shift(self, x, b, t, dev)`
- Defined: `micro/stt-training/stt_training/augment.py:165`
- Imported by: `micro/stt-training/stt_training/train.py`

### _snr_scale `def _snr_scale(self, sig, noise, b, dev)`
- Defined: `micro/stt-training/stt_training/augment.py:174`
- Imported by: `micro/stt-training/stt_training/train.py`

### _colored_noise `def _colored_noise(self, x, b, t, dev)`
- Defined: `micro/stt-training/stt_training/augment.py:181`
- Imported by: `micro/stt-training/stt_training/train.py`

### _bandpass `def _bandpass(self, x, b, t, dev)`
- Defined: `micro/stt-training/stt_training/augment.py:194`
- Imported by: `micro/stt-training/stt_training/train.py`

### _bg_noise `def _bg_noise(self, x, b, t, dev)`
- Defined: `micro/stt-training/stt_training/augment.py:210`
- Imported by: `micro/stt-training/stt_training/train.py`

### _rir `def _rir(self, x, b, t, dev)`
- Defined: `micro/stt-training/stt_training/augment.py:219`
- Imported by: `micro/stt-training/stt_training/train.py`

### forward `def forward(self, waveform)`
- Defined: `micro/stt-training/stt_training/augment.py:238`
- Imported by: `micro/stt-training/stt_training/train.py`

## micro/stt-training/stt_training/checkpoint.py

### resolve_checkpoint `def resolve_checkpoint(path)`
- Defined: `micro/stt-training/stt_training/checkpoint.py:17`
- Doc: Accept a ``.pt`` file, a run directory, or the checkpoints parent.
- Depends on: `micro/stt-training/stt_training/model.py`
- Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/export.py`

### load_model `def load_model(path, device)`
- Defined: `micro/stt-training/stt_training/checkpoint.py:35`
- Doc: Load a checkpoint. Returns ``(model, classes, cfg)``.
- Depends on: `micro/stt-training/stt_training/model.py`
- Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/export.py`

### load_representative_waveforms `def load_representative_waveforms(data_roots, n, target_samples, sample_rate, seed)`
- Defined: `micro/stt-training/stt_training/checkpoint.py:61`
- Doc: Sample up to ``n`` fixed-length mono waveforms from ``<root>/<class>/*.wav``.
- Depends on: `micro/stt-training/stt_training/model.py`
- Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/export.py`

## micro/stt-training/stt_training/dataset.py

### _warn_decode_failure `def _warn_decode_failure(src, exc)`
- Defined: `micro/stt-training/stt_training/dataset.py:27`
- Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/train.py`

### voice_id_from_path `def voice_id_from_path(path)`
- Defined: `micro/stt-training/stt_training/dataset.py:39`
- Doc: Stable per-voice id for speaker-independent splits.
- Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/train.py`

### speaker_independent_split `def speaker_independent_split(dataset, val_fraction, seed)`
- Defined: `micro/stt-training/stt_training/dataset.py:120`
- Doc: Split indices so no voice appears in both train and val.
- Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/train.py`

### build_class_balanced_sampler `def build_class_balanced_sampler(labels, power)`
- Defined: `micro/stt-training/stt_training/dataset.py:142`
- Doc: Weighted sampler that softens class imbalance.
- Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/train.py`

### report_class_coverage `def report_class_coverage(dataset, classes)`
- Defined: `micro/stt-training/stt_training/dataset.py:163`
- Doc: Print per-class clip counts and warn about empty classes.
- Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/train.py`

### mixup `def mixup(x, y, num_classes, alpha)`
- Defined: `micro/stt-training/stt_training/dataset.py:190`
- Doc: Standard mixup. Returns (mixed_x, soft_targets).
- Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/train.py`

### soft_cross_entropy `def soft_cross_entropy(logits, soft_targets, smoothing)`
- Defined: `micro/stt-training/stt_training/dataset.py:205`
- Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/train.py`

### __init__ `def __init__(self, roots, classes, sample_rate, clip_seconds)`
- Defined: `micro/stt-training/stt_training/dataset.py:54`
- Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/train.py`

### __len__ `def __len__(self)`
- Defined: `micro/stt-training/stt_training/dataset.py:89`
- Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/train.py`

### _load_wav `def _load_wav(self, path)`
- Defined: `micro/stt-training/stt_training/dataset.py:92`
- Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/train.py`

### __getitem__ `def __getitem__(self, idx)`
- Defined: `micro/stt-training/stt_training/dataset.py:109`
- Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/train.py`

### voice_ids `def voice_ids(self)`
- Defined: `micro/stt-training/stt_training/dataset.py:113`
- Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/train.py`

### load_waveform `def load_waveform(self, idx)`
- Defined: `micro/stt-training/stt_training/dataset.py:116`
- Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/train.py`

## micro/stt-training/stt_training/evaluate.py

### _confusions `def _confusions(y_true, y_pred, classes, top)`
- Defined: `micro/stt-training/stt_training/evaluate.py:30`
- Depends on: `micro/stt-training/stt_training/checkpoint.py`, `micro/stt-training/stt_training/dataset.py`, `micro/stt-training/stt_training/export.py`, `micro/stt-training/stt_training/features.py`, `micro/stt-training/stt_training/train.py`

### main `def main()`
- Defined: `micro/stt-training/stt_training/evaluate.py:38`
- Depends on: `micro/stt-training/stt_training/checkpoint.py`, `micro/stt-training/stt_training/dataset.py`, `micro/stt-training/stt_training/export.py`, `micro/stt-training/stt_training/features.py`, `micro/stt-training/stt_training/train.py`

### _report `def _report(name, y_true, y_pred, classes)`
- Defined: `micro/stt-training/stt_training/evaluate.py:102`
- Depends on: `micro/stt-training/stt_training/checkpoint.py`, `micro/stt-training/stt_training/dataset.py`, `micro/stt-training/stt_training/export.py`, `micro/stt-training/stt_training/features.py`, `micro/stt-training/stt_training/train.py`

## micro/stt-training/stt_training/export.py

### _inline_buffers `def _inline_buffers(buf)`
- Defined: `micro/stt-training/stt_training/export.py:37`
- Doc: Re-serialize a .tflite with every external weight buffer inlined (TFLM-safe).
- Depends on: `micro/stt-training/stt_training/checkpoint.py`, `micro/stt-training/stt_training/features.py`
- Imported by: `micro/stt-training/stt_training/evaluate.py`

### _interpreter `def _interpreter(path)`
- Defined: `micro/stt-training/stt_training/export.py:62`
- Depends on: `micro/stt-training/stt_training/checkpoint.py`, `micro/stt-training/stt_training/features.py`
- Imported by: `micro/stt-training/stt_training/evaluate.py`

### _run_tflite `def _run_tflite(interp, feats)`
- Defined: `micro/stt-training/stt_training/export.py:70`
- Depends on: `micro/stt-training/stt_training/checkpoint.py`, `micro/stt-training/stt_training/features.py`
- Imported by: `micro/stt-training/stt_training/evaluate.py`

### export `def export(args)`
- Defined: `micro/stt-training/stt_training/export.py:86`
- Depends on: `micro/stt-training/stt_training/checkpoint.py`, `micro/stt-training/stt_training/features.py`
- Imported by: `micro/stt-training/stt_training/evaluate.py`

### _default_calibration_roots `def _default_calibration_roots(args)`
- Defined: `micro/stt-training/stt_training/export.py:197`
- Depends on: `micro/stt-training/stt_training/checkpoint.py`, `micro/stt-training/stt_training/features.py`
- Imported by: `micro/stt-training/stt_training/evaluate.py`

### build_argparser `def build_argparser()`
- Defined: `micro/stt-training/stt_training/export.py:207`
- Depends on: `micro/stt-training/stt_training/checkpoint.py`, `micro/stt-training/stt_training/features.py`
- Imported by: `micro/stt-training/stt_training/evaluate.py`

### main `def main()`
- Defined: `micro/stt-training/stt_training/export.py:220`
- Depends on: `micro/stt-training/stt_training/checkpoint.py`, `micro/stt-training/stt_training/features.py`
- Imported by: `micro/stt-training/stt_training/evaluate.py`

## micro/stt-training/stt_training/features.py

### __init__ `def __init__(self, sample_rate, n_fft, hop_length, n_mels, f_min, f_max, target_frames, eps)`
- Defined: `micro/stt-training/stt_training/features.py:23`
- Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/export.py`, `micro/stt-training/stt_training/train.py`

### _fix_length `def _fix_length(self, x)`
- Defined: `micro/stt-training/stt_training/features.py:50`
- Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/export.py`, `micro/stt-training/stt_training/train.py`

### forward `def forward(self, waveform)`
- Defined: `micro/stt-training/stt_training/features.py:58`
- Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/export.py`, `micro/stt-training/stt_training/train.py`

### __init__ `def __init__(self, freq_mask_param, time_mask_param, n_freq_masks, n_time_masks)`
- Defined: `micro/stt-training/stt_training/features.py:73`
- Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/export.py`, `micro/stt-training/stt_training/train.py`

### forward `def forward(self, x)`
- Defined: `micro/stt-training/stt_training/features.py:86`
- Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/export.py`, `micro/stt-training/stt_training/train.py`

## micro/stt-training/stt_training/model.py

### _make_divisible `def _make_divisible(v, divisor)`
- Defined: `micro/stt-training/stt_training/model.py:19`
- Doc: Round channel counts to a multiple of ``divisor`` (mobile-friendly).
- Imported by: `micro/stt-training/stt_training/checkpoint.py`, `micro/stt-training/stt_training/train.py`

### normalize_stride `def normalize_stride(v)`
- Defined: `micro/stt-training/stt_training/model.py:27`
- Doc: Coerce an int / ``"2,2"`` string / tuple into ``(freq_stride, time_stride)``.
- Imported by: `micro/stt-training/stt_training/checkpoint.py`, `micro/stt-training/stt_training/train.py`

### build_model `def build_model(num_classes)`
- Defined: `micro/stt-training/stt_training/model.py:167`
- Imported by: `micro/stt-training/stt_training/checkpoint.py`, `micro/stt-training/stt_training/train.py`

### __init__ `def __init__(self, in_c, out_c, kernel, stride, groups, act)`
- Defined: `micro/stt-training/stt_training/model.py:47`
- Imported by: `micro/stt-training/stt_training/checkpoint.py`, `micro/stt-training/stt_training/train.py`

### __init__ `def __init__(self, in_c, out_c, stride, expand_ratio)`
- Defined: `micro/stt-training/stt_training/model.py:61`
- Imported by: `micro/stt-training/stt_training/checkpoint.py`, `micro/stt-training/stt_training/train.py`

### forward `def forward(self, x)`
- Defined: `micro/stt-training/stt_training/model.py:77`
- Imported by: `micro/stt-training/stt_training/checkpoint.py`, `micro/stt-training/stt_training/train.py`

### __init__ `def __init__(self, num_classes, width_mult, dropout, stem_stride, pad_to_odd)`
- Defined: `micro/stt-training/stt_training/model.py:100`
- Imported by: `micro/stt-training/stt_training/checkpoint.py`, `micro/stt-training/stt_training/train.py`

### _init_weights `def _init_weights(self)`
- Defined: `micro/stt-training/stt_training/model.py:146`
- Imported by: `micro/stt-training/stt_training/checkpoint.py`, `micro/stt-training/stt_training/train.py`

### forward `def forward(self, x)`
- Defined: `micro/stt-training/stt_training/model.py:157`
- Imported by: `micro/stt-training/stt_training/checkpoint.py`, `micro/stt-training/stt_training/train.py`

## micro/stt-training/stt_training/train.py

### default_data_roots `def default_data_roots(tts_dir, ps_dir)`
- Defined: `micro/stt-training/stt_training/train.py:49`
- Doc: Discover training roots: one per ZipVoice speaker, plus People's Speech.
- Depends on: `micro/stt-training/stt_training/augment.py`, `micro/stt-training/stt_training/dataset.py`, `micro/stt-training/stt_training/features.py`, `micro/stt-training/stt_training/model.py`, `micro/stt-training/stt_training/words.py`
- Imported by: `micro/stt-training/stt_training/evaluate.py`

### evaluate `def evaluate(model, feature_fn, loader, device)`
- Defined: `micro/stt-training/stt_training/train.py:60`
- Depends on: `micro/stt-training/stt_training/augment.py`, `micro/stt-training/stt_training/dataset.py`, `micro/stt-training/stt_training/features.py`, `micro/stt-training/stt_training/model.py`, `micro/stt-training/stt_training/words.py`
- Imported by: `micro/stt-training/stt_training/evaluate.py`

### train `def train(args)`
- Defined: `micro/stt-training/stt_training/train.py:88`
- Depends on: `micro/stt-training/stt_training/augment.py`, `micro/stt-training/stt_training/dataset.py`, `micro/stt-training/stt_training/features.py`, `micro/stt-training/stt_training/model.py`, `micro/stt-training/stt_training/words.py`
- Imported by: `micro/stt-training/stt_training/evaluate.py`

### build_argparser `def build_argparser()`
- Defined: `micro/stt-training/stt_training/train.py:275`
- Depends on: `micro/stt-training/stt_training/augment.py`, `micro/stt-training/stt_training/dataset.py`, `micro/stt-training/stt_training/features.py`, `micro/stt-training/stt_training/model.py`, `micro/stt-training/stt_training/words.py`
- Imported by: `micro/stt-training/stt_training/evaluate.py`

### main `def main()`
- Defined: `micro/stt-training/stt_training/train.py:317`
- Depends on: `micro/stt-training/stt_training/augment.py`, `micro/stt-training/stt_training/dataset.py`, `micro/stt-training/stt_training/features.py`, `micro/stt-training/stt_training/model.py`, `micro/stt-training/stt_training/words.py`
- Imported by: `micro/stt-training/stt_training/evaluate.py`

### lr_at `def lr_at(step)`
- Defined: `micro/stt-training/stt_training/train.py:193`
- Depends on: `micro/stt-training/stt_training/augment.py`, `micro/stt-training/stt_training/dataset.py`, `micro/stt-training/stt_training/features.py`, `micro/stt-training/stt_training/model.py`, `micro/stt-training/stt_training/words.py`
- Imported by: `micro/stt-training/stt_training/evaluate.py`

## micro/stt-training/stt_training/words.py

### folder_for_word `def folder_for_word(word)`
- Defined: `micro/stt-training/stt_training/words.py:18`
- Doc: Filesystem-safe label folder for a word.
- Imported by: `micro/stt-training/stt_training/__init__.py`, `micro/stt-training/stt_training/train.py`, `micro/stt-training/tools/extract_clips.py`, `micro/stt-training/tools/mine_peoples_speech.py`, `micro/stt-training/tools/synthesize.py`

### load_words `def load_words(path)`
- Defined: `micro/stt-training/stt_training/words.py:31`
- Doc: Load command words from ``words.txt`` (one per line, ``#`` comments).
- Imported by: `micro/stt-training/stt_training/__init__.py`, `micro/stt-training/stt_training/train.py`, `micro/stt-training/tools/extract_clips.py`, `micro/stt-training/tools/mine_peoples_speech.py`, `micro/stt-training/tools/synthesize.py`

### resolve_classes `def resolve_classes(path, include_unknown)`
- Defined: `micro/stt-training/stt_training/words.py:53`
- Doc: Return the ordered class list: command words plus the reject class.
- Imported by: `micro/stt-training/stt_training/__init__.py`, `micro/stt-training/stt_training/train.py`, `micro/stt-training/tools/extract_clips.py`, `micro/stt-training/tools/mine_peoples_speech.py`, `micro/stt-training/tools/synthesize.py`

## micro/stt-training/tools/download_musan_rirs.py

### download_musan_noise `def download_musan_noise(out_dir, small, seed)`
- Defined: `micro/stt-training/tools/download_musan_rirs.py:37`

### download_rirs `def download_rirs(out_dir, max_files, seed)`
- Defined: `micro/stt-training/tools/download_musan_rirs.py:67`

### main `def main()`
- Defined: `micro/stt-training/tools/download_musan_rirs.py:94`

## micro/stt-training/tools/extract_clips.py

### _cut_natural_clip `def _cut_natural_clip(audio, start_s, end_s)`
- Defined: `micro/stt-training/tools/extract_clips.py:116`
- Doc: Neighbour-clamped clip covering ``[start_s, end_s]`` padded and grown.
- Depends on: `micro/stt-training/stt_training/words.py`

### _resolve_device `def _resolve_device(choice)`
- Defined: `micro/stt-training/tools/extract_clips.py:144`
- Depends on: `micro/stt-training/stt_training/words.py`

### _load_rows `def _load_rows(path)`
- Defined: `micro/stt-training/tools/extract_clips.py:156`
- Depends on: `micro/stt-training/stt_training/words.py`

### _safe `def _safe(s)`
- Defined: `micro/stt-training/tools/extract_clips.py:167`
- Depends on: `micro/stt-training/stt_training/words.py`

### main `def main()`
- Defined: `micro/stt-training/tools/extract_clips.py:171`
- Depends on: `micro/stt-training/stt_training/words.py`

### __init__ `def __init__(self, device, with_star)`
- Defined: `micro/stt-training/tools/extract_clips.py:56`
- Depends on: `micro/stt-training/stt_training/words.py`

### _ids `def _ids(self, word)`
- Defined: `micro/stt-training/tools/extract_clips.py:71`
- Depends on: `micro/stt-training/stt_training/words.py`

### align `def align(self, audio_1d, words)`
- Defined: `micro/stt-training/tools/extract_clips.py:74`
- Doc: Return one ``AlignedWord`` per input word (``None`` if unpronounceable).
- Depends on: `micro/stt-training/stt_training/words.py`

### emit `def emit(label, clip_id, char_start, speaker, clip, sample_rate)`
- Defined: `micro/stt-training/tools/extract_clips.py:212`
- Depends on: `micro/stt-training/stt_training/words.py`

## micro/stt-training/tools/mine_peoples_speech.py

### _new_fs `def _new_fs()`
- Defined: `micro/stt-training/tools/mine_peoples_speech.py:69`
- Depends on: `micro/stt-training/stt_training/words.py`

### _shard_paths `def _shard_paths(config, split)`
- Defined: `micro/stt-training/tools/mine_peoples_speech.py:75`
- Depends on: `micro/stt-training/stt_training/words.py`

### iter_peoples_speech `def iter_peoples_speech(config, split, offset, limit)`
- Defined: `micro/stt-training/tools/mine_peoples_speech.py:131`
- Doc: Yield ``(clip_id, transcript, speaker, fetch_audio)`` rows.
- Depends on: `micro/stt-training/stt_training/words.py`

### _tokens_with_pos `def _tokens_with_pos(text)`
- Defined: `micro/stt-training/tools/mine_peoples_speech.py:187`
- Depends on: `micro/stt-training/stt_training/words.py`

### find_matches `def find_matches(text, targets)`
- Defined: `micro/stt-training/tools/mine_peoples_speech.py:191`
- Doc: Return ``[(label, char_start, char_end), ...]`` for command words in text.
- Depends on: `micro/stt-training/stt_training/words.py`

### _safe_name `def _safe_name(clip_id)`
- Defined: `micro/stt-training/tools/mine_peoples_speech.py:207`
- Depends on: `micro/stt-training/stt_training/words.py`

### save_audio_16k `def save_audio_16k(fetch, out_path)`
- Defined: `micro/stt-training/tools/mine_peoples_speech.py:211`
- Depends on: `micro/stt-training/stt_training/words.py`

### _load_seen_keys `def _load_seen_keys(path)`
- Defined: `micro/stt-training/tools/mine_peoples_speech.py:231`
- Depends on: `micro/stt-training/stt_training/words.py`

### main `def main()`
- Defined: `micro/stt-training/tools/mine_peoples_speech.py:247`
- Depends on: `micro/stt-training/stt_training/words.py`

### __init__ `def __init__(self, shard, max_attempts)`
- Defined: `micro/stt-training/tools/mine_peoples_speech.py:90`
- Depends on: `micro/stt-training/stt_training/words.py`

### _open `def _open(self)`
- Defined: `micro/stt-training/tools/mine_peoples_speech.py:98`
- Depends on: `micro/stt-training/stt_training/words.py`

### num_row_groups `def num_row_groups(self)`
- Defined: `micro/stt-training/tools/mine_peoples_speech.py:103`
- Depends on: `micro/stt-training/stt_training/words.py`

### row_group_num_rows `def row_group_num_rows(self, rg)`
- Defined: `micro/stt-training/tools/mine_peoples_speech.py:106`
- Depends on: `micro/stt-training/stt_training/words.py`

### read_columns `def read_columns(self, rg, columns)`
- Defined: `micro/stt-training/tools/mine_peoples_speech.py:109`
- Depends on: `micro/stt-training/stt_training/words.py`

### _fetch `def _fetch(_rg, _i)`
- Defined: `micro/stt-training/tools/mine_peoples_speech.py:157`
- Depends on: `micro/stt-training/stt_training/words.py`

## micro/stt-training/tools/synthesize.py

### discover_voices `def discover_voices(language)`
- Defined: `micro/stt-training/tools/synthesize.py:58`
- Doc: Return the installed ZipVoice speakers, falling back to the known list.
- Depends on: `micro/stt-training/stt_training/words.py`

### _resample_to_16k `def _resample_to_16k(samples, sr)`
- Defined: `micro/stt-training/tools/synthesize.py:76`
- Depends on: `micro/stt-training/stt_training/words.py`

### main `def main()`
- Defined: `micro/stt-training/tools/synthesize.py:85`
- Depends on: `micro/stt-training/stt_training/words.py`

## micro/stt/include/stt/stt.h

### feature_scratch `float* feature_scratch() const`
- Defined: `micro/stt/include/stt/stt.h:65`
- Doc: Scratch for the fp32 log-mel features, carved from the arena's activation overlay (dead until Invoke()). Contract: produ

### input_quant `TensorQuant input_quant() const`
- Defined: `micro/stt/include/stt/stt.h:66`

### output_quant `TensorQuant output_quant() const`
- Defined: `micro/stt/include/stt/stt.h:68`

### n_classes `int n_classes() const`
- Defined: `micro/stt/include/stt/stt.h:69`

### input_count `std::size_t input_count() const`
- Defined: `micro/stt/include/stt/stt.h:70`

### arena_used_bytes `std::size_t arena_used_bytes() const`
- Defined: `micro/stt/include/stt/stt.h:71`

## micro/stt/scripts/desktop_parity.py

### _resolve_meta `def _resolve_meta(tflite)`
- Defined: `micro/stt/scripts/desktop_parity.py:60`
- Doc: Load whichever metadata sidecar sits next to the model.
- Depends on: `micro/stt/scripts/generate_embedded_data.py`

### _int16_roundtrip `def _int16_roundtrip(samples)`
- Defined: `micro/stt/scripts/desktop_parity.py:76`
- Doc: Replicate the embedded int16 blob and the firmware's inverse.
- Depends on: `micro/stt/scripts/generate_embedded_data.py`

### _softmax_prob `def _softmax_prob(logits, idx)`
- Defined: `micro/stt/scripts/desktop_parity.py:92`
- Depends on: `micro/stt/scripts/generate_embedded_data.py`

### _parse_device_log `def _parse_device_log(path)`
- Defined: `micro/stt/scripts/desktop_parity.py:98`
- Doc: Pull ``(exp, got)`` pairs from a pico_monitor.log per-clip table.
- Depends on: `micro/stt/scripts/generate_embedded_data.py`

### main `def main(argv)`
- Defined: `micro/stt/scripts/desktop_parity.py:111`
- Depends on: `micro/stt/scripts/generate_embedded_data.py`

## micro/stt/scripts/generate_embedded_data.py

### _include_guard `def _include_guard(stem)`
- Defined: `micro/stt/scripts/generate_embedded_data.py:63`
- Doc: Traditional include-guard macro for a generated header stem (no ext).
- Imported by: `micro/stt/scripts/desktop_parity.py`, `micro/vad/scripts/generate_vad_embedded_data.py`

### _resolve_int8_mel_tflite `def _resolve_int8_mel_tflite(explicit)`
- Defined: `micro/stt/scripts/generate_embedded_data.py:68`
- Doc: Return the checked-in SpellingCNN int8 model under moonshine-micro/models/.
- Imported by: `micro/stt/scripts/desktop_parity.py`, `micro/vad/scripts/generate_vad_embedded_data.py`

### _meta_sidecar `def _meta_sidecar(tflite)`
- Defined: `micro/stt/scripts/generate_embedded_data.py:90`
- Imported by: `micro/stt/scripts/desktop_parity.py`, `micro/vad/scripts/generate_vad_embedded_data.py`

### _load_meta `def _load_meta(tflite)`
- Defined: `micro/stt/scripts/generate_embedded_data.py:103`
- Doc: Load the model's audio metadata, or die loudly if it's missing.
- Imported by: `micro/stt/scripts/desktop_parity.py`, `micro/vad/scripts/generate_vad_embedded_data.py`

### _format_byte_array `def _format_byte_array(data, width)`
- Defined: `micro/stt/scripts/generate_embedded_data.py:142`
- Doc: Render `data` as comma-separated 0x.. literals, wrapping every `width`.
- Imported by: `micro/stt/scripts/desktop_parity.py`, `micro/vad/scripts/generate_vad_embedded_data.py`

### _format_int16_array `def _format_int16_array(samples, width)`
- Defined: `micro/stt/scripts/generate_embedded_data.py:151`
- Doc: Render signed int16 samples as comma-separated literals.
- Imported by: `micro/stt/scripts/desktop_parity.py`, `micro/vad/scripts/generate_vad_embedded_data.py`

### _f32 `def _f32(x)`
- Defined: `micro/stt/scripts/generate_embedded_data.py:160`
- Doc: Round a Python float (f64) to the nearest IEEE-754 float32 value.
- Imported by: `micro/stt/scripts/desktop_parity.py`, `micro/vad/scripts/generate_vad_embedded_data.py`

### _format_float32_array `def _format_float32_array(vals, width)`
- Defined: `micro/stt/scripts/generate_embedded_data.py:171`
- Doc: Render floats as comma-separated C ``float`` literals (``...f``).
- Imported by: `micro/stt/scripts/desktop_parity.py`, `micro/vad/scripts/generate_vad_embedded_data.py`

### _format_plain_int_array `def _format_plain_int_array(vals, width)`
- Defined: `micro/stt/scripts/generate_embedded_data.py:180`
- Doc: Render ints as comma-separated literals (no width padding).
- Imported by: `micro/stt/scripts/desktop_parity.py`, `micro/vad/scripts/generate_vad_embedded_data.py`

### _fp32_to_int16_pcm `def _fp32_to_int16_pcm(samples)`
- Defined: `micro/stt/scripts/generate_embedded_data.py:189`
- Doc: Symmetric 16-bit quantization with saturation.
- Imported by: `micro/stt/scripts/desktop_parity.py`, `micro/vad/scripts/generate_vad_embedded_data.py`

### _is_riff_wav `def _is_riff_wav(path)`
- Defined: `micro/stt/scripts/generate_embedded_data.py:207`
- Doc: True when ``path`` looks like a real PCM wav (not a Git LFS pointer).
- Imported by: `micro/stt/scripts/desktop_parity.py`, `micro/vad/scripts/generate_vad_embedded_data.py`

### _load_clip `def _load_clip(path, sample_rate, n_samples)`
- Defined: `micro/stt/scripts/generate_embedded_data.py:216`
- Doc: Read a wav, conform to (sample_rate, n_samples), return int16 PCM.
- Imported by: `micro/stt/scripts/desktop_parity.py`, `micro/vad/scripts/generate_vad_embedded_data.py`

### _write_model_files `def _write_model_files(out_dir, tflite)`
- Defined: `micro/stt/scripts/generate_embedded_data.py:228`
- Imported by: `micro/stt/scripts/desktop_parity.py`, `micro/vad/scripts/generate_vad_embedded_data.py`

### _write_audio_config_file `def _write_audio_config_file(out_dir)`
- Defined: `micro/stt/scripts/generate_embedded_data.py:268`
- Doc: Emit ``audio_config.h`` with the model's mel-front-end constants.
- Imported by: `micro/stt/scripts/desktop_parity.py`, `micro/vad/scripts/generate_vad_embedded_data.py`

### _write_mel_tables_file `def _write_mel_tables_file(out_dir)`
- Defined: `micro/stt/scripts/generate_embedded_data.py:327`
- Doc: Emit ``mel_tables.{h,cc}``: the precomputed Hann window + CSR mel
- Imported by: `micro/stt/scripts/desktop_parity.py`, `micro/vad/scripts/generate_vad_embedded_data.py`

### _write_classes_files `def _write_classes_files(out_dir, classes)`
- Defined: `micro/stt/scripts/generate_embedded_data.py:465`
- Imported by: `micro/stt/scripts/desktop_parity.py`, `micro/vad/scripts/generate_vad_embedded_data.py`

### _write_clips_files `def _write_clips_files(out_dir, decoded, sample_rate, n_samples)`
- Defined: `micro/stt/scripts/generate_embedded_data.py:501`
- Doc: Write one ``int16`` array per clip plus a small descriptor table.
- Imported by: `micro/stt/scripts/desktop_parity.py`, `micro/vad/scripts/generate_vad_embedded_data.py`

### _pick_clips `def _pick_clips(wavs_roots, classes, clips_per_class, max_classes)`
- Defined: `micro/stt/scripts/generate_embedded_data.py:586`
- Doc: Pick a deterministic per-class subset (alphabetical by filename).
- Imported by: `micro/stt/scripts/desktop_parity.py`, `micro/vad/scripts/generate_vad_embedded_data.py`

### _pick_clips_hub `def _pick_clips_hub(repo_id, configs, classes, clips_per_class, max_classes, sample_rate, n_samples, cache_dir)`
- Defined: `micro/stt/scripts/generate_embedded_data.py:617`
- Doc: Pick a deterministic per-class subset from packed HF speech shards.
- Imported by: `micro/stt/scripts/desktop_parity.py`, `micro/vad/scripts/generate_vad_embedded_data.py`

### main `def main(argv)`
- Defined: `micro/stt/scripts/generate_embedded_data.py:680`
- Imported by: `micro/stt/scripts/desktop_parity.py`, `micro/vad/scripts/generate_vad_embedded_data.py`

## micro/stt/src/classifier.cc

### Saturate8 `inline int8_t Saturate8(float v)`
- Defined: `micro/stt/src/classifier.cc:26`
- Doc: Saturating round-and-cast for the input-quantization step. Same formula as the host reference classifier so both agree a

### Classifier `Classifier::Classifier(const unsigned char* model_data,
                       unsigned int /*mod...`
- Defined: `micro/stt/src/classifier.cc:52`

### Run `void Classifier::Run(const float* features, float* logits_out) const`
- Defined: `micro/stt/src/classifier.cc:225`

## micro/stt/src/predictor.cc

### Argmax `int Argmax(const float* logits, int n_logits)`
- Defined: `micro/stt/src/predictor.cc:6`

### SoftmaxProb `float SoftmaxProb(const float* logits, int n_logits, int index)`
- Defined: `micro/stt/src/predictor.cc:19`

## micro/stt/tests/predictor_test.cc

### TF_LITE_MICRO_TEST `TF_LITE_MICRO_TESTS_BEGIN

TF_LITE_MICRO_TEST(ArgmaxPicksLargest)`
- Defined: `micro/stt/tests/predictor_test.cc:11`
- Doc: include "stt/stt.h" include "tensorflow/lite/micro/testing/micro_test.h"

### TF_LITE_MICRO_TEST `TF_LITE_MICRO_TEST(ArgmaxTiesGoToLowestIndex)`
- Defined: `micro/stt/tests/predictor_test.cc:18`

### TF_LITE_MICRO_TEST `TF_LITE_MICRO_TEST(SoftmaxProbsSumToOne)`
- Defined: `micro/stt/tests/predictor_test.cc:23`

### TF_LITE_MICRO_TEST `TF_LITE_MICRO_TEST(SoftmaxProbMatchesHandComputed)`
- Defined: `micro/stt/tests/predictor_test.cc:30`

### TF_LITE_MICRO_TEST `TF_LITE_MICRO_TEST(SoftmaxStableOnLargeLogits)`
- Defined: `micro/stt/tests/predictor_test.cc:36`

## micro/test-support/host/tflm_host_stub.cc

### MicroPrintf `void MicroPrintf(const char* format, ...)`
- Defined: `micro/test-support/host/tflm_host_stub.cc:18`
- Doc: include <cstdarg> include <cstddef> include <cstdio>

### VMicroPrintf `void VMicroPrintf(const char* format, va_list args)`
- Defined: `micro/test-support/host/tflm_host_stub.cc:26`

### MicroSnprintf `int MicroSnprintf(char* buffer, size_t buf_size, const char* format, ...)`
- Defined: `micro/test-support/host/tflm_host_stub.cc:31`

### MicroVsnprintf `int MicroVsnprintf(char* buffer, size_t buf_size, const char* format,
                   va_list ...`
- Defined: `micro/test-support/host/tflm_host_stub.cc:39`

### InitializeTarget `void InitializeTarget()`
- Defined: `micro/test-support/host/tflm_host_stub.cc:46`

## micro/vad/include/vad/vad.h

### feature_scratch `float* feature_scratch() const`
- Defined: `micro/vad/include/vad/vad.h:64`
- Doc: Scratch for the fp32 log-mel window, borrowed from the arena overlay (dead until Invoke()). Contract: produce features h

### input_quant `VadTensorQuant input_quant() const`
- Defined: `micro/vad/include/vad/vad.h:65`

### output_quant `VadTensorQuant output_quant() const`
- Defined: `micro/vad/include/vad/vad.h:67`

### input_count `std::size_t input_count() const`
- Defined: `micro/vad/include/vad/vad.h:68`

### arena_used_bytes `std::size_t arena_used_bytes() const`
- Defined: `micro/vad/include/vad/vad.h:69`

### segment_start_sample `std::size_t segment_start_sample() const`
- Defined: `micro/vad/include/vad/vad.h:113`
- Doc: Boundaries (absolute sample indices) of the most-recent segment.

### segment_end_sample `std::size_t segment_end_sample() const`
- Defined: `micro/vad/include/vad/vad.h:114`

### samples_processed `std::size_t samples_processed() const`
- Defined: `micro/vad/include/vad/vad.h:115`

## micro/vad/scripts/generate_vad_embedded_data.py

### _smooth_window_frames `def _smooth_window_frames()`
- Defined: `micro/vad/scripts/generate_vad_embedded_data.py:66`
- Depends on: `micro/stt/scripts/generate_embedded_data.py`

### _write_vad_config `def _write_vad_config(out_dir)`
- Defined: `micro/vad/scripts/generate_vad_embedded_data.py:72`
- Depends on: `micro/stt/scripts/generate_embedded_data.py`

### _write_vad_mel_tables `def _write_vad_mel_tables(out_dir)`
- Defined: `micro/vad/scripts/generate_vad_embedded_data.py:117`
- Depends on: `micro/stt/scripts/generate_embedded_data.py`

### _write_vad_model `def _write_vad_model(out_dir, tflite)`
- Defined: `micro/vad/scripts/generate_vad_embedded_data.py:190`
- Depends on: `micro/stt/scripts/generate_embedded_data.py`

### _auto_tflite `def _auto_tflite()`
- Defined: `micro/vad/scripts/generate_vad_embedded_data.py:224`
- Depends on: `micro/stt/scripts/generate_embedded_data.py`

### main `def main(argv)`
- Defined: `micro/vad/scripts/generate_vad_embedded_data.py:229`
- Depends on: `micro/stt/scripts/generate_embedded_data.py`

## micro/vad/src/vad.cc

### Saturate8 `inline int8_t Saturate8(float v)`
- Defined: `micro/vad/src/vad.cc:21`

### Vad `Vad::Vad(const unsigned char* model_data, unsigned int /*model_size*/,
         uint8_t* tensor_a...`
- Defined: `micro/vad/src/vad.cc:37`

### Predict `float Vad::Predict(const float* features) const`
- Defined: `micro/vad/src/vad.cc:170`

## micro/vad/src/vad_segmenter.cc

### VadSegmenter `VadSegmenter::VadSegmenter(float threshold, int window_frames, int hop,
                         ...`
- Defined: `micro/vad/src/vad_segmenter.cc:5`

### Start `void VadSegmenter::Start()`
- Defined: `micro/vad/src/vad_segmenter.cc:21`

### ProcessFrame `VadEvent VadSegmenter::ProcessFrame(float raw_probability)`
- Defined: `micro/vad/src/vad_segmenter.cc:31`

### Finish `VadEvent VadSegmenter::Finish()`
- Defined: `micro/vad/src/vad_segmenter.cc:83`

### ExtractClipFrontAligned `void ExtractClipFrontAligned(const float* src, std::size_t src_len,
                             ...`
- Defined: `micro/vad/src/vad_segmenter.cc:92`

### EnergyCentroidIndex `std::size_t EnergyCentroidIndex(const int16_t* buf, std::size_t start,
                          ...`
- Defined: `micro/vad/src/vad_segmenter.cc:105`

## micro/vad/tests/vad_segmenter_test.cc

### Repeat `std::vector<float> Repeat(float v, int n)`
- Defined: `micro/vad/tests/vad_segmenter_test.cc:19`

### Concat `std::vector<float> Concat(std::initializer_list<std::vector<float>> parts)`
- Defined: `micro/vad/tests/vad_segmenter_test.cc:21`

### TF_LITE_MICRO_TEST `TF_LITE_MICRO_TESTS_BEGIN

TF_LITE_MICRO_TEST(SingleSegmentDetected)`
- Defined: `micro/vad/tests/vad_segmenter_test.cc:47`

### TF_LITE_MICRO_TEST `TF_LITE_MICRO_TEST(TwoSegmentsDetected)`
- Defined: `micro/vad/tests/vad_segmenter_test.cc:59`

### TF_LITE_MICRO_TEST `TF_LITE_MICRO_TEST(TrailingSegmentFlushed)`
- Defined: `micro/vad/tests/vad_segmenter_test.cc:67`

### TF_LITE_MICRO_TEST `TF_LITE_MICRO_TEST(NoLookBehindStartsLater)`
- Defined: `micro/vad/tests/vad_segmenter_test.cc:74`

### TF_LITE_MICRO_TEST `TF_LITE_MICRO_TEST(ExtractClipFrontAlignedZeroPads)`
- Defined: `micro/vad/tests/vad_segmenter_test.cc:85`

### TF_LITE_MICRO_TEST `TF_LITE_MICRO_TEST(EnergyCentroidIndexWeightsByPower)`
- Defined: `micro/vad/tests/vad_segmenter_test.cc:95`

## python/setup.py

### read_readme `def read_readme()`
- Defined: `python/setup.py:26`

### read_license `def read_license()`
- Defined: `python/setup.py:32`

### read_requirements `def read_requirements()`
- Defined: `python/setup.py:39`

### has_ext_modules `def has_ext_modules(self)`
- Defined: `python/setup.py:10`

### finalize_options `def finalize_options(self)`
- Defined: `python/setup.py:15`

### get_tag `def get_tag(self)`
- Defined: `python/setup.py:20`

## python/src/moonshine_voice/__init__.py

### __getattr__ `def __getattr__(name)`
- Defined: `python/src/moonshine_voice/__init__.py:81`
- Doc: Lazy import for transcriber, mic_transcriber, and intent_recognizer modules.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

## python/src/moonshine_voice/alphanumeric_listener.py

### spoken_form `def spoken_form(char)`
- Defined: `python/src/moonshine_voice/alphanumeric_listener.py:306`
- Doc: Return a TTS-friendly phrase for a single character.
- Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`

### _normalize `def _normalize(text)`
- Defined: `python/src/moonshine_voice/alphanumeric_listener.py:355`
- Doc: Return *text* lower-cased with quotes/punctuation removed.
- Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`

### _build_lookup `def _build_lookup()`
- Defined: `python/src/moonshine_voice/alphanumeric_listener.py:370`
- Doc: Merge all character vocabularies into a single lookup table.
- Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`

### _parse_number_words `def _parse_number_words(text)`
- Defined: `python/src/moonshine_voice/alphanumeric_listener.py:424`
- Doc: Parse English number words in the range 10 – 1 000.
- Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`

### letters_only_matcher `def letters_only_matcher()`
- Defined: `python/src/moonshine_voice/alphanumeric_listener.py:716`
- Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`

### digits_only_matcher `def digits_only_matcher()`
- Defined: `python/src/moonshine_voice/alphanumeric_listener.py:720`
- Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`

### is_character `def is_character(self)`
- Defined: `python/src/moonshine_voice/alphanumeric_listener.py:80`
- Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`

### is_terminator `def is_terminator(self)`
- Defined: `python/src/moonshine_voice/alphanumeric_listener.py:84`
- Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`

### is_recognized `def is_recognized(self)`
- Defined: `python/src/moonshine_voice/alphanumeric_listener.py:88`
- Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`

### __init__ `def __init__(self)`
- Defined: `python/src/moonshine_voice/alphanumeric_listener.py:542`
- Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`

### classify `def classify(self, raw_text)`
- Defined: `python/src/moonshine_voice/alphanumeric_listener.py:570`
- Doc: Classify a single utterance into an :class:`AlphanumericMatch`.
- Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`

### classify_sequence `def classify_sequence(self, raw_text)`
- Defined: `python/src/moonshine_voice/alphanumeric_listener.py:606`
- Doc: Classify a potentially multi-token utterance.
- Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`

### _resolve `def _resolve(self, text)`
- Defined: `python/src/moonshine_voice/alphanumeric_listener.py:637`
- Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`

### _resolve_spelled_letter `def _resolve_spelled_letter(self, text)`
- Defined: `python/src/moonshine_voice/alphanumeric_listener.py:652`
- Doc: Recognise speller patterns like ``"A for Alpha"`` / ``"B as in Boy"``.
- Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`

### _char_accepted `def _char_accepted(self, char)`
- Defined: `python/src/moonshine_voice/alphanumeric_listener.py:705`
- Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`

### __init__ `def __init__(self, callback)`
- Defined: `python/src/moonshine_voice/alphanumeric_listener.py:808`
- Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`

### __call__ `def __call__(self, event)`
- Defined: `python/src/moonshine_voice/alphanumeric_listener.py:829`
- Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`

### text `def text(self)`
- Defined: `python/src/moonshine_voice/alphanumeric_listener.py:840`
- Doc: The currently assembled text.
- Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`

### stopped `def stopped(self)`
- Defined: `python/src/moonshine_voice/alphanumeric_listener.py:845`
- Doc: Whether a stop command has been received.
- Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`

### matcher `def matcher(self)`
- Defined: `python/src/moonshine_voice/alphanumeric_listener.py:850`
- Doc: The underlying :class:`AlphanumericMatcher`.
- Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`

### clear `def clear(self)`
- Defined: `python/src/moonshine_voice/alphanumeric_listener.py:854`
- Doc: Programmatically clear the buffer.
- Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`

### undo `def undo(self)`
- Defined: `python/src/moonshine_voice/alphanumeric_listener.py:865`
- Doc: Remove and return the last character, or ``None`` if empty.
- Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`

### _process_utterance `def _process_utterance(self, line)`
- Defined: `python/src/moonshine_voice/alphanumeric_listener.py:879`
- Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`

### _speak_character `def _speak_character(self, char)`
- Defined: `python/src/moonshine_voice/alphanumeric_listener.py:941`
- Doc: Speak the TTS phrase for ``char`` if a TTS backend is wired.
- Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`

### _play_error_feedback `def _play_error_feedback(self)`
- Defined: `python/src/moonshine_voice/alphanumeric_listener.py:957`
- Doc: Ask the TTS backend to play its error beep, if it supports one.
- Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`

### on_event `def on_event(event)`
- Defined: `python/src/moonshine_voice/alphanumeric_listener.py:1063`
- Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`

## python/src/moonshine_voice/cached_embeddings.py

### default_cached_embeddings_path `def default_cached_embeddings_path()`
- Defined: `python/src/moonshine_voice/cached_embeddings.py:62`
- Doc: Return the absolute path of the packaged cached embeddings TSV.
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### write_cached_embeddings_tsv `def write_cached_embeddings_tsv(path, entries)`
- Defined: `python/src/moonshine_voice/cached_embeddings.py:260`
- Doc: Write a TSV compatible with :class:`CachedEmbeddings`.
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### calculate_embedding `def calculate_embedding(self, sentence)`
- Defined: `python/src/moonshine_voice/cached_embeddings.py:52`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### distance `def distance(self, embedding_a, embedding_b)`
- Defined: `python/src/moonshine_voice/cached_embeddings.py:54`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### __init__ `def __init__(self)`
- Defined: `python/src/moonshine_voice/cached_embeddings.py:95`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### active `def active(self)`
- Defined: `python/src/moonshine_voice/cached_embeddings.py:150`
- Doc: ``True`` when the cache has at least one usable entry.
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### path `def path(self)`
- Defined: `python/src/moonshine_voice/cached_embeddings.py:155`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### metadata `def metadata(self)`
- Defined: `python/src/moonshine_voice/cached_embeddings.py:159`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### phrases `def phrases(self)`
- Defined: `python/src/moonshine_voice/cached_embeddings.py:163`
- Doc: Return the list of cached phrases (normalized keys).
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### __len__ `def __len__(self)`
- Defined: `python/src/moonshine_voice/cached_embeddings.py:167`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### __contains__ `def __contains__(self, sentence)`
- Defined: `python/src/moonshine_voice/cached_embeddings.py:170`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### get `def get(self, sentence)`
- Defined: `python/src/moonshine_voice/cached_embeddings.py:175`
- Doc: Return the cached embedding or ``None`` if not present.
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### calculate_embedding `def calculate_embedding(self, sentence)`
- Defined: `python/src/moonshine_voice/cached_embeddings.py:179`
- Doc: Return the embedding for ``sentence``.
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### distance `def distance(self, embedding_a, embedding_b)`
- Defined: `python/src/moonshine_voice/cached_embeddings.py:195`
- Doc: Return the cosine similarity between two embedding vectors.
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### _load `def _load(self, path)`
- Defined: `python/src/moonshine_voice/cached_embeddings.py:218`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### _parse_meta `def _parse_meta(self, s)`
- Defined: `python/src/moonshine_voice/cached_embeddings.py:238`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### _normalize `def _normalize(s)`
- Defined: `python/src/moonshine_voice/cached_embeddings.py:245`
- Doc: Normalize a phrase for lookup.
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

## python/src/moonshine_voice/cli.py

### _package_version `def _package_version()`
- Defined: `python/src/moonshine_voice/cli.py:50`
- Imported by: `python/tests/test_cli.py`

### _usage `def _usage()`
- Defined: `python/src/moonshine_voice/cli.py:68`
- Imported by: `python/tests/test_cli.py`

### main `def main(argv)`
- Defined: `python/src/moonshine_voice/cli.py:91`
- Doc: Dispatch to a subcommand. Returns a process exit code.
- Imported by: `python/tests/test_cli.py`

## python/src/moonshine_voice/dialog_flow.py

### spell_out `def spell_out(s)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1656`
- Doc: Return ``s`` as a TTS-friendly spoken-form phrase.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _summarise `def _summarise(text, max_len)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1684`
- Doc: Truncate ``text`` for debug logs so we don't spam the terminal.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _run_beep_diagnostic `def _run_beep_diagnostic()`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1704`
- Doc: Play the success / error beeps and a reference tone, then return.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### calculate_embedding `def calculate_embedding(self, sentence)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:222`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### distance `def distance(self, embedding_a, embedding_b)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:224`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### __init__ `def __init__(self, backend, phrases_by_key)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:255`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### threshold `def threshold(self)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:282`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### match `def match(self, utterance)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:285`
- Doc: Return the best-matching key, or *None* if below threshold.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### match_with_score `def match_with_score(self, utterance)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:290`
- Doc: Return ``(key, similarity)`` of the best match above threshold.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### __init__ `def __init__(self, trigger_phrase)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:345`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### say `def say(self, text)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:350`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### ask `def ask(self, prompt)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:354`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### confirm `def confirm(self, prompt)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:374`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### choose `def choose(self, prompt, options)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:384`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### cancel `def cancel(self)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:402`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### restart `def restart(self)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:405`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### replay_last_prompt `def replay_last_prompt(self)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:408`
- Doc: Return a :class:`Say` that re-speaks the most recent prompt.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### __init__ `def __init__(self, matcher)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:435`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### __init__ `def __init__(self, flow_fn, trigger_phrase)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:443`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### __init__ `def __init__(self)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:558`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### register_flow `def register_flow(self, trigger_phrase, flow)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:662`
- Doc: Register a flow function to be started when ``trigger_phrase`` fires.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### unregister_flow `def unregister_flow(self, trigger_phrase)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:674`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### register_global `def register_global(self, trigger_phrase, handler)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:680`
- Doc: Register a phrase that is always live, even while a flow runs.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _invalidate_trigger_matcher `def _invalidate_trigger_matcher(self)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:691`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### is_active `def is_active(self)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:697`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### active_trigger `def active_trigger(self)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:702`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### registered_flows `def registered_flows(self)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:707`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### on_line_started `def on_line_started(self, event)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:712`
- Doc: Tag any transcript line that opens while we're talking.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### on_line_completed `def on_line_completed(self, event)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:746`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### on_error `def on_error(self, event)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:772`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### process_utterance `def process_utterance(self, utterance)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:777`
- Doc: Route an utterance.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _should_short_circuit_to_alpha `def _should_short_circuit_to_alpha(self, active, utterance)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:870`
- Doc: Return True if an alphanumeric prompt should consume ``utterance``
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _match_trigger `def _match_trigger(self, utterance)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:888`
- Doc: Return ``(kind, phrase)`` where ``kind`` is ``"global"`` / ``"flow"`` / ``None``.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _get_trigger_matcher `def _get_trigger_matcher(self)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:910`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _start_flow `def _start_flow(self, trigger_phrase)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:934`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _deliver_to_active `def _deliver_to_active(self, active, utterance)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:944`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _advance `def _advance(self, active, value)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:991`
- Doc: Drive the generator until it blocks on user input or finishes.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _throw `def _throw(self, active, exc)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1055`
- Doc: Raise ``exc`` into the generator and process whatever it yields next.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _set_spelling_mode `def _set_spelling_mode(self, active)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1091`
- Doc: Toggle ``MOONSHINE_FLAG_SPELLING_MODE`` on the underlying transcriber.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _spelling_mode_for_prompt `def _spelling_mode_for_prompt(self, prompt)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1114`
- Doc: Whether ``prompt`` expects alphanumeric (spelled) input.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _alpha_session_for `def _alpha_session_for(self, prompt)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1118`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _get_spelled_matcher `def _get_spelled_matcher(self)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1127`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _get_digits_matcher `def _get_digits_matcher(self)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1132`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _restart_flow `def _restart_flow(self, active)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1137`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _finish_flow `def _finish_flow(self, active)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1146`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### cancel_active `def cancel_active(self)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1156`
- Doc: Abandon any currently running flow.  Returns ``True`` if there was one.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### say `def say(self, text)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1169`
- Doc: Speak ``text`` through the configured TTS, outside any flow.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _invoke_global `def _invoke_global(self, trigger_phrase)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1199`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _interpret_answer `def _interpret_answer(self, prompt, utterance, active)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1236`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _interpret_ask `def _interpret_ask(self, prompt, utterance, active)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1247`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _interpret_alphanumeric `def _interpret_alphanumeric(self, prompt, utterance, active)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1259`
- Doc: Drive the AlphanumericMatcher session for SPELLED / DIGITS.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _interpret_confirm `def _interpret_confirm(self, prompt, utterance, active)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1338`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _interpret_choose `def _interpret_choose(self, prompt, utterance, active)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1355`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _get_confirm_matcher `def _get_confirm_matcher(self, prompt)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1372`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _get_choose_matcher `def _get_choose_matcher(self, prompt)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1388`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _build_matcher `def _build_matcher(self, phrases_by_key, threshold)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1407`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _reprompt_or_abandon `def _reprompt_or_abandon(self, prompt, active, exc)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1424`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _speak `def _speak(self, text)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1440`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _speak_character_feedback `def _speak_character_feedback(self, character)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1485`
- Doc: Speak ``spoken_form(character)`` as mid-prompt spell-back.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _play_beep `def _play_beep(self, kind)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1504`
- Doc: Play the recognition cue identified by ``kind``.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _play_success_beep `def _play_success_beep(self)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1551`
- Doc: Play the "recognized" cue, if a beep callback is wired.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _play_error_beep `def _play_error_beep(self)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1560`
- Doc: Play the "not recognized" cue, if a beep callback is wired.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _speak_undo_feedback `def _speak_undo_feedback(self, character)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1569`
- Doc: Speak ``"deleting <spoken_form(character)>"`` after an UNDO.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _log `def _log(self, msg)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1589`
- Doc: Emit a timestamped trace line to stderr when ``debug=True``.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### __init__ `def __init__(self, text)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1620`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### __init__ `def __init__(self, exc)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1625`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### __iter__ `def __iter__(self)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1650`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### wifi_setup `def wifi_setup(d)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:1980`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### mute `def mute(should_mute)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:2069`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### set_spelling_mode `def set_spelling_mode(active)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:2073`
- Doc: Toggle the C++ spelling-CNN fusion path on the live mic stream.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### speak `def speak(text)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:2081`
- Doc: Log every spoken prompt and (optionally) pass it through TTS.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### on_line_completed `def on_line_completed(self, event)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:2105`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

### _default_factory `def _default_factory(phrases_by_key, threshold)`
- Defined: `python/src/moonshine_voice/dialog_flow.py:633`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`

## python/src/moonshine_voice/download.py

### find_model_info `def find_model_info(language, model_arch)`
- Defined: `python/src/moonshine_voice/download.py:168`
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### supported_languages_friendly `def supported_languages_friendly()`
- Defined: `python/src/moonshine_voice/download.py:197`
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### supported_languages `def supported_languages()`
- Defined: `python/src/moonshine_voice/download.py:203`
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### get_components_for_model_info `def get_components_for_model_info(model_info)`
- Defined: `python/src/moonshine_voice/download.py:207`
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### download_model_from_info `def download_model_from_info(model_info)`
- Defined: `python/src/moonshine_voice/download.py:234`
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### supported_embedding_models `def supported_embedding_models()`
- Defined: `python/src/moonshine_voice/download.py:254`
- Doc: Return list of supported embedding model names.
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### supported_embedding_models_friendly `def supported_embedding_models_friendly()`
- Defined: `python/src/moonshine_voice/download.py:259`
- Doc: Return a friendly string listing supported embedding models.
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### get_embedding_model_variants `def get_embedding_model_variants(model_name)`
- Defined: `python/src/moonshine_voice/download.py:266`
- Doc: Return list of available variants for an embedding model.
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### get_embedding_model `def get_embedding_model(model_name, variant)`
- Defined: `python/src/moonshine_voice/download.py:276`
- Doc: Download an embedding model and return (path, arch).
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### _spelling_language_key `def _spelling_language_key(language)`
- Defined: `python/src/moonshine_voice/download.py:339`
- Doc: Map a user language tag to the key used in :data:`SPELLING_MODEL_INFO`, or ``None``.
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### _spelling_model_root_path `def _spelling_model_root_path(language_key, cache_root)`
- Defined: `python/src/moonshine_voice/download.py:358`
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### download_spelling_model_for_language `def download_spelling_model_for_language(language)`
- Defined: `python/src/moonshine_voice/download.py:365`
- Doc: Download the alphanumeric spelling model for ``language`` if one is
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### get_spelling_model_path `def get_spelling_model_path(language)`
- Defined: `python/src/moonshine_voice/download.py:395`
- Doc: Return the on-disk path to the spelling model for ``language``.
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### get_model_for_language `def get_model_for_language(wanted_language, wanted_model_arch)`
- Defined: `python/src/moonshine_voice/download.py:410`
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### log_model_info `def log_model_info(wanted_language, wanted_model_arch)`
- Defined: `python/src/moonshine_voice/download.py:438`
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### normalize_moonshine_language_tag `def normalize_moonshine_language_tag(language)`
- Defined: `python/src/moonshine_voice/download.py:461`
- Doc: Normalize a user language tag to the form expected by the Moonshine C API (e.g. en_us).
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### _normalize_tts_language_tag_display `def _normalize_tts_language_tag_display(tag)`
- Defined: `python/src/moonshine_voice/download.py:467`
- Doc: Lowercase language tag with hyphens only (underscores and spaces → ``-``, collapse repeats).
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### dedupe_tts_language_tags_for_display `def dedupe_tts_language_tags_for_display(tags)`
- Defined: `python/src/moonshine_voice/download.py:474`
- Doc: Drop aliases that differ only by ``_`` vs ``-`` / spaces; return sorted hyphenated tags.
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### _tts_asset_cache_root `def _tts_asset_cache_root(override)`
- Defined: `python/src/moonshine_voice/download.py:485`
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### tts_asset_cache_path `def tts_asset_cache_path(cache_root)`
- Defined: `python/src/moonshine_voice/download.py:491`
- Doc: Resolved directory for the TTS/G2P on-disk layout (same root `download_tts_assets` uses).
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### _merge_tts_query_options `def _merge_tts_query_options(options)`
- Defined: `python/src/moonshine_voice/download.py:496`
- Doc: Options passed to ``moonshine_get_tts_dependencies`` (``voice`` with optional ``kokoro_`` / ``piper_`` prefix, path over
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### _options_specify_asset_root `def _options_specify_asset_root(opts)`
- Defined: `python/src/moonshine_voice/download.py:511`
- Doc: True when the caller already set a C API root key (see ``MoonshineTTSOptions::parse_options``).
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### _voice_query_options `def _voice_query_options(options)`
- Defined: `python/src/moonshine_voice/download.py:522`
- Doc: Options for ``moonshine_get_tts_voices`` (and related voice-list queries).
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### _entries_to_present_and_downloadable `def _entries_to_present_and_downloadable(entries)`
- Defined: `python/src/moonshine_voice/download.py:563`
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### _tts_voices_json_to_catalog `def _tts_voices_json_to_catalog(raw)`
- Defined: `python/src/moonshine_voice/download.py:569`
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### list_tts_languages `def list_tts_languages()`
- Defined: `python/src/moonshine_voice/download.py:588`
- Doc: TTS language tags supported by the native catalog for the given path/voice options
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### get_tts_voice_catalog `def get_tts_voice_catalog()`
- Defined: `python/src/moonshine_voice/download.py:611`
- Doc: Full map of language tag → voice entries (``id`` + ``state``: ``found`` or ``missing``).
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### list_tts_voices `def list_tts_voices(language)`
- Defined: `python/src/moonshine_voice/download.py:634`
- Doc: Voice ids for one language, split by on-disk availability (raises `MoonshineTtsLanguageError`
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### validate_tts_language `def validate_tts_language(language)`
- Defined: `python/src/moonshine_voice/download.py:673`
- Doc: Normalize and validate a TTS language tag against the native catalog.
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### _normalize_tts_voice_stem `def _normalize_tts_voice_stem(stem)`
- Defined: `python/src/moonshine_voice/download.py:701`
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### _tts_voice_want_aliases `def _tts_voice_want_aliases(voice)`
- Defined: `python/src/moonshine_voice/download.py:711`
- Doc: Normalized ids the user may mean (prefixed catalog id vs bare stem).
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### validate_tts_voice_downloaded `def validate_tts_voice_downloaded(language, voice, asset_root)`
- Defined: `python/src/moonshine_voice/download.py:728`
- Doc: Ensure ``voice`` is present (native ``state`` ``found``) for ``language`` under ``asset_root``.
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### validate_tts_voice_known `def validate_tts_voice_known(language, voice)`
- Defined: `python/src/moonshine_voice/download.py:760`
- Doc: Ensure ``voice`` appears in the native TTS catalog for ``language``.
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### ensure_tts_voice_downloaded `def ensure_tts_voice_downloaded(language, voice, asset_root)`
- Defined: `python/src/moonshine_voice/download.py:799`
- Doc: Ensure ``voice`` is on disk under ``asset_root``, like `validate_tts_voice_downloaded`.
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### is_downloadable_tts_asset_key `def is_downloadable_tts_asset_key(key)`
- Defined: `python/src/moonshine_voice/download.py:842`
- Doc: Return False for G2P override labels (no path) returned when custom options are set.
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### cdn_url_for_tts_asset_key `def cdn_url_for_tts_asset_key(key)`
- Defined: `python/src/moonshine_voice/download.py:850`
- Doc: HTTPS URL for a canonical asset key under ``TTS_CDN_BASE_URL``.
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### list_tts_dependency_keys `def list_tts_dependency_keys(languages)`
- Defined: `python/src/moonshine_voice/download.py:857`
- Doc: Resolve required TTS asset paths via the native ``moonshine_get_tts_dependencies`` API.
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### list_g2p_dependency_keys `def list_g2p_dependency_keys(languages, options)`
- Defined: `python/src/moonshine_voice/download.py:882`
- Doc: Resolve G2P-only asset paths via ``moonshine_get_g2p_dependencies`` (comma-separated from C).
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### download_tts_assets `def download_tts_assets(language)`
- Defined: `python/src/moonshine_voice/download.py:897`
- Doc: Download every file required for TTS for the given language (and optional prefixed ``voice``) into the cache.
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

### download_g2p_assets `def download_g2p_assets(language)`
- Defined: `python/src/moonshine_voice/download.py:953`
- Doc: Download G2P lexicon/model files into the TTS asset cache layout (same CDN tree as TTS).
- Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`

## python/src/moonshine_voice/download_file.py

### get_cache_dir `def get_cache_dir(app_name)`
- Defined: `python/src/moonshine_voice/download_file.py:13`
- Doc: Get the cache directory, respecting environment override.
- Imported by: `python/src/moonshine_voice/download.py`

### hash_file `def hash_file(path, algorithm)`
- Defined: `python/src/moonshine_voice/download_file.py:19`
- Doc: Compute hash of a file.
- Imported by: `python/src/moonshine_voice/download.py`

### download_file `def download_file(url, dest, expected_sha256, resume, show_progress, timeout)`
- Defined: `python/src/moonshine_voice/download_file.py:28`
- Doc: Download a file with progress bar, resume support, and integrity checking.
- Imported by: `python/src/moonshine_voice/download.py`

### download_model `def download_model(url, filename, expected_sha256, app_name)`
- Defined: `python/src/moonshine_voice/download_file.py:149`
- Doc: Download a model file to the cache directory.
- Imported by: `python/src/moonshine_voice/download.py`

## python/src/moonshine_voice/errors.py

### check_error `def check_error(error_code)`
- Defined: `python/src/moonshine_voice/errors.py:107`
- Doc: Check error code and raise appropriate exception if non-zero.
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/tts.py`, `scripts/tts_g2p_intelligibility.py`

### __init__ `def __init__(self, message, error_code)`
- Defined: `python/src/moonshine_voice/errors.py:9`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/tts.py`, `scripts/tts_g2p_intelligibility.py`

### __init__ `def __init__(self, message)`
- Defined: `python/src/moonshine_voice/errors.py:17`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/tts.py`, `scripts/tts_g2p_intelligibility.py`

### __init__ `def __init__(self, message)`
- Defined: `python/src/moonshine_voice/errors.py:24`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/tts.py`, `scripts/tts_g2p_intelligibility.py`

### __init__ `def __init__(self, message)`
- Defined: `python/src/moonshine_voice/errors.py:31`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/tts.py`, `scripts/tts_g2p_intelligibility.py`

### __init__ `def __init__(self, language, alternatives, message)`
- Defined: `python/src/moonshine_voice/errors.py:38`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/tts.py`, `scripts/tts_g2p_intelligibility.py`

### __init__ `def __init__(self, message)`
- Defined: `python/src/moonshine_voice/errors.py:57`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/tts.py`, `scripts/tts_g2p_intelligibility.py`

### __init__ `def __init__(self, voice, language, alternatives)`
- Defined: `python/src/moonshine_voice/errors.py:81`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/tts.py`, `scripts/tts_g2p_intelligibility.py`

## python/src/moonshine_voice/g2p.py

### main `def main()`
- Defined: `python/src/moonshine_voice/g2p.py:118`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`

### __init__ `def __init__(self, language)`
- Defined: `python/src/moonshine_voice/g2p.py:30`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`

### language `def language(self)`
- Defined: `python/src/moonshine_voice/g2p.py:85`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`

### asset_root `def asset_root(self)`
- Defined: `python/src/moonshine_voice/g2p.py:89`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`

### to_ipa `def to_ipa(self, text, options)`
- Defined: `python/src/moonshine_voice/g2p.py:92`
- Doc: Return IPA for ``text`` (single string from the native layer).
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`

### close `def close(self)`
- Defined: `python/src/moonshine_voice/g2p.py:100`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`

### __enter__ `def __enter__(self)`
- Defined: `python/src/moonshine_voice/g2p.py:105`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`

### __exit__ `def __exit__(self, exc_type, exc, tb)`
- Defined: `python/src/moonshine_voice/g2p.py:108`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`

### __del__ `def __del__(self)`
- Defined: `python/src/moonshine_voice/g2p.py:111`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`

## python/src/moonshine_voice/intent_recognizer.py

### trigger_phrase `def trigger_phrase(self)`
- Defined: `python/src/moonshine_voice/intent_recognizer.py:37`
- Doc: Alias for ``canonical_phrase`` (backward compatibility).
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### __init__ `def __init__(self, model_path, model_arch, model_variant, threshold)`
- Defined: `python/src/moonshine_voice/intent_recognizer.py:61`
- Doc: Initialize an intent recognizer.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### _setup_function_signatures `def _setup_function_signatures(self)`
- Defined: `python/src/moonshine_voice/intent_recognizer.py:109`
- Doc: Setup ctypes function signatures for the intent recognizer C API.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### __enter__ `def __enter__(self)`
- Defined: `python/src/moonshine_voice/intent_recognizer.py:191`
- Doc: Context manager entry.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### __exit__ `def __exit__(self, exc_type, exc_val, exc_tb)`
- Defined: `python/src/moonshine_voice/intent_recognizer.py:195`
- Doc: Context manager exit.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### close `def close(self)`
- Defined: `python/src/moonshine_voice/intent_recognizer.py:199`
- Doc: Free the intent recognizer resources.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### __del__ `def __del__(self)`
- Defined: `python/src/moonshine_voice/intent_recognizer.py:206`
- Doc: Cleanup on deletion.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### register_intent `def register_intent(self, trigger_phrase, handler)`
- Defined: `python/src/moonshine_voice/intent_recognizer.py:211`
- Doc: Register an intent with a canonical phrase.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### unregister_intent `def unregister_intent(self, trigger_phrase)`
- Defined: `python/src/moonshine_voice/intent_recognizer.py:253`
- Doc: Remove a registered intent.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### get_closest_intents `def get_closest_intents(self, utterance, tolerance_threshold)`
- Defined: `python/src/moonshine_voice/intent_recognizer.py:274`
- Doc: Rank registered intents against ``utterance`` synchronously.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### process_utterance `def process_utterance(self, utterance)`
- Defined: `python/src/moonshine_voice/intent_recognizer.py:331`
- Doc: Process an utterance and invoke the handler of the most similar intent.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### threshold `def threshold(self)`
- Defined: `python/src/moonshine_voice/intent_recognizer.py:358`
- Doc: Minimum similarity used by ``process_utterance`` / default for ``get_closest_intents``.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### threshold `def threshold(self, value)`
- Defined: `python/src/moonshine_voice/intent_recognizer.py:363`
- Doc: Set the default similarity threshold (Python-side; passed per call to native code).
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### intent_count `def intent_count(self)`
- Defined: `python/src/moonshine_voice/intent_recognizer.py:368`
- Doc: Get the number of registered intents.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### clear_intents `def clear_intents(self)`
- Defined: `python/src/moonshine_voice/intent_recognizer.py:377`
- Doc: Clear all registered intents.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### calculate_embedding `def calculate_embedding(self, sentence)`
- Defined: `python/src/moonshine_voice/intent_recognizer.py:385`
- Doc: Calculate the embedding vector for a sentence.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### distance `def distance(self, embedding_a, embedding_b)`
- Defined: `python/src/moonshine_voice/intent_recognizer.py:421`
- Doc: Compute the cosine similarity between two embedding vectors.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### set_on_intent `def set_on_intent(self, callback)`
- Defined: `python/src/moonshine_voice/intent_recognizer.py:454`
- Doc: Set a callback that is invoked for any recognized intent.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### on_line_completed `def on_line_completed(self, event)`
- Defined: `python/src/moonshine_voice/intent_recognizer.py:469`
- Doc: Called when a transcription line is completed.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### on_error `def on_error(self, event)`
- Defined: `python/src/moonshine_voice/intent_recognizer.py:485`
- Doc: Called when an error occurs.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### on_intent_triggered_on `def on_intent_triggered_on(trigger, utterance, similarity)`
- Defined: `python/src/moonshine_voice/intent_recognizer.py:555`
- Doc: Handler for when an intent is triggered.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### __init__ `def __init__(self)`
- Defined: `python/src/moonshine_voice/intent_recognizer.py:564`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### update_last_terminal_line `def update_last_terminal_line(self, new_text)`
- Defined: `python/src/moonshine_voice/intent_recognizer.py:567`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### on_line_started `def on_line_started(self, event)`
- Defined: `python/src/moonshine_voice/intent_recognizer.py:574`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### on_line_text_changed `def on_line_text_changed(self, event)`
- Defined: `python/src/moonshine_voice/intent_recognizer.py:577`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

### on_line_completed `def on_line_completed(self, event)`
- Defined: `python/src/moonshine_voice/intent_recognizer.py:580`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`

## python/src/moonshine_voice/mic_transcriber.py

### __init__ `def __init__(self, model_path, model_arch, update_interval, device, samplerate, channels, blocksize, options, spelling_model_path, transcribe_flags)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:22`
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

### _query_device_default_samplerate `def _query_device_default_samplerate(self)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:60`
- Doc: Return the input device's native default sample rate, or None on failure.
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

### _open_input_stream `def _open_input_stream(self, samplerate, callback)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:78`
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

### _start_listening `def _start_listening(self)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:89`
- Doc: Start listening to the microphone (or specified audio device).
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

### _process_audio_queue `def _process_audio_queue(self)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:128`
- Doc: Drain queued audio into the stream from a dedicated worker thread.
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

### _add_batch `def _add_batch(self, batch)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:163`
- Doc: Concatenate consecutive same-sample-rate chunks and add each run once.
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

### _add_run `def _add_run(self, chunks, sample_rate)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:176`
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

### _start_worker `def _start_worker(self)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:186`
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

### _stop_worker `def _stop_worker(self)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:195`
- Doc: Signal the worker to drain the queue and exit, then join it.
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

### start `def start(self)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:202`
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

### stop `def stop(self)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:209`
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

### close `def close(self)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:216`
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

### transcribe_flags `def transcribe_flags(self)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:223`
- Doc: Flags currently applied to streamed ``update_transcription`` calls.
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

### set_transcribe_flags `def set_transcribe_flags(self, flags)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:227`
- Doc: Update the per-update flags on the underlying mic stream.
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

### add_listener `def add_listener(self, listener)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:236`
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

### remove_listener `def remove_listener(self, listener)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:239`
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

### remove_all_listeners `def remove_all_listeners(self)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:242`
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

### push_listener `def push_listener(self, listener)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:245`
- Doc: Push a temporary listener, saving the current listeners on a stack.
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

### pop_listener `def pop_listener(self)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:249`
- Doc: Restore the listeners that were active before the last push.
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

### pop_all_listeners `def pop_all_listeners(self)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:253`
- Doc: Unwind the entire listener stack, restoring the original listeners.
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

### audio_callback `def audio_callback(in_data, frames, time, status)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:95`
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

### __init__ `def __init__(self)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:281`
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

### update_last_terminal_line `def update_last_terminal_line(self, line)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:286`
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

### on_line_started `def on_line_started(self, event)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:308`
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

### on_line_text_changed `def on_line_text_changed(self, event)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:311`
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

### on_line_completed `def on_line_completed(self, event)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:314`
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

### on_line_completed `def on_line_completed(self, event)`
- Defined: `python/src/moonshine_voice/mic_transcriber.py:320`
- Depends on: `python/src/moonshine_voice/utils.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`

## python/src/moonshine_voice/moonshine_api.py

### _decode_utf8_from_c `def _decode_utf8_from_c(buf)`
- Defined: `python/src/moonshine_voice/moonshine_api.py:34`
- Doc: Decode C malloc NUL-terminated bytes; tolerate rare invalid UTF-8 from native G2P output.
- Depends on: `python/src/moonshine_voice/errors.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`, `scripts/eval-alphanumeric.py`

### _load_libc `def _load_libc()`
- Defined: `python/src/moonshine_voice/moonshine_api.py:42`
- Depends on: `python/src/moonshine_voice/errors.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`, `scripts/eval-alphanumeric.py`

### _get_libc `def _get_libc()`
- Defined: `python/src/moonshine_voice/moonshine_api.py:56`
- Depends on: `python/src/moonshine_voice/errors.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`, `scripts/eval-alphanumeric.py`

### moonshine_free `def moonshine_free(address)`
- Defined: `python/src/moonshine_voice/moonshine_api.py:65`
- Doc: Release memory allocated by the Moonshine C API (``malloc``). Pass the raw pointer value (integer).
- Depends on: `python/src/moonshine_voice/errors.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`, `scripts/eval-alphanumeric.py`

### _require_struct_size `def _require_struct_size(name, struct, expected, note)`
- Defined: `python/src/moonshine_voice/moonshine_api.py:130`
- Doc: Fail fast if a ctypes struct drifts from the compiled C ABI.
- Depends on: `python/src/moonshine_voice/errors.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`, `scripts/eval-alphanumeric.py`

### model_arch_to_string `def model_arch_to_string(model_arch)`
- Defined: `python/src/moonshine_voice/moonshine_api.py:199`
- Doc: Convert a model architecture to a string.
- Depends on: `python/src/moonshine_voice/errors.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`, `scripts/eval-alphanumeric.py`

### string_to_model_arch `def string_to_model_arch(model_arch_string)`
- Defined: `python/src/moonshine_voice/moonshine_api.py:217`
- Doc: Convert a string to a model architecture.
- Depends on: `python/src/moonshine_voice/errors.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`, `scripts/eval-alphanumeric.py`

### moonshine_options_array `def moonshine_options_array(options)`
- Defined: `python/src/moonshine_voice/moonshine_api.py:322`
- Doc: Build a ``moonshine_option_t`` array. Keep the returned list alive until the C call completes.
- Depends on: `python/src/moonshine_voice/errors.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`, `scripts/eval-alphanumeric.py`

### moonshine_c_string_array `def moonshine_c_string_array(strings)`
- Defined: `python/src/moonshine_voice/moonshine_api.py:339`
- Doc: Build ``const char *filenames[]`` for TTS/G2P create-from-files helpers.
- Depends on: `python/src/moonshine_voice/errors.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`, `scripts/eval-alphanumeric.py`

### moonshine_memory_arrays `def moonshine_memory_arrays(buffers)`
- Defined: `python/src/moonshine_voice/moonshine_api.py:348`
- Doc: Build parallel ``uint8_t*`` and ``uint64_t`` size arrays for in-memory TTS/G2P creation.
- Depends on: `python/src/moonshine_voice/errors.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`, `scripts/eval-alphanumeric.py`

### moonshine_get_g2p_dependencies_string `def moonshine_get_g2p_dependencies_string(languages, options)`
- Defined: `python/src/moonshine_voice/moonshine_api.py:373`
- Doc: Call ``moonshine_get_g2p_dependencies`` and return the comma-separated key list (UTF-8).
- Depends on: `python/src/moonshine_voice/errors.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`, `scripts/eval-alphanumeric.py`

### moonshine_get_tts_dependencies_string `def moonshine_get_tts_dependencies_string(languages, options)`
- Defined: `python/src/moonshine_voice/moonshine_api.py:398`
- Doc: Call ``moonshine_get_tts_dependencies`` and return the JSON array string (UTF-8).
- Depends on: `python/src/moonshine_voice/errors.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`, `scripts/eval-alphanumeric.py`

### moonshine_try_get_tts_voices `def moonshine_try_get_tts_voices(languages, options)`
- Defined: `python/src/moonshine_voice/moonshine_api.py:423`
- Doc: Call ``moonshine_get_tts_voices`` without raising.
- Depends on: `python/src/moonshine_voice/errors.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`, `scripts/eval-alphanumeric.py`

### moonshine_get_tts_voices_string `def moonshine_get_tts_voices_string(languages, options)`
- Defined: `python/src/moonshine_voice/moonshine_api.py:452`
- Doc: Call ``moonshine_get_tts_voices`` and return the JSON object string (UTF-8).
- Depends on: `python/src/moonshine_voice/errors.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`, `scripts/eval-alphanumeric.py`

### moonshine_text_to_speech_samples `def moonshine_text_to_speech_samples(tts_synthesizer_handle, text, options)`
- Defined: `python/src/moonshine_voice/moonshine_api.py:468`
- Doc: Call ``moonshine_text_to_speech``; returns ``(samples, sample_rate_hz)``. Frees the native audio buffer.
- Depends on: `python/src/moonshine_voice/errors.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`, `scripts/eval-alphanumeric.py`

### moonshine_phonemes_to_speech_samples `def moonshine_phonemes_to_speech_samples(tts_synthesizer_handle, phonemes, options)`
- Defined: `python/src/moonshine_voice/moonshine_api.py:505`
- Doc: Call ``moonshine_phonemes_to_speech``; returns ``(samples, sample_rate_hz)``.
- Depends on: `python/src/moonshine_voice/errors.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`, `scripts/eval-alphanumeric.py`

### moonshine_text_to_phonemes_string `def moonshine_text_to_phonemes_string(grapheme_to_phonemizer_handle, text, options)`
- Defined: `python/src/moonshine_voice/moonshine_api.py:546`
- Doc: Call ``moonshine_text_to_phonemes``; returns the IPA string (single segment).
- Depends on: `python/src/moonshine_voice/errors.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`, `scripts/eval-alphanumeric.py`

### __str__ `def __str__(self)`
- Defined: `python/src/moonshine_voice/moonshine_api.py:244`
- Depends on: `python/src/moonshine_voice/errors.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`, `scripts/eval-alphanumeric.py`

### __str__ `def __str__(self)`
- Defined: `python/src/moonshine_voice/moonshine_api.py:272`
- Depends on: `python/src/moonshine_voice/errors.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`, `scripts/eval-alphanumeric.py`

### __str__ `def __str__(self)`
- Defined: `python/src/moonshine_voice/moonshine_api.py:302`
- Depends on: `python/src/moonshine_voice/errors.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`, `scripts/eval-alphanumeric.py`

### __str__ `def __str__(self)`
- Defined: `python/src/moonshine_voice/moonshine_api.py:317`
- Doc: Return a string representation of the transcript.
- Depends on: `python/src/moonshine_voice/errors.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`, `scripts/eval-alphanumeric.py`

### __new__ `def __new__(cls)`
- Defined: `python/src/moonshine_voice/moonshine_api.py:589`
- Depends on: `python/src/moonshine_voice/errors.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`, `scripts/eval-alphanumeric.py`

### _load_library `def _load_library(self)`
- Defined: `python/src/moonshine_voice/moonshine_api.py:595`
- Doc: Load the Moonshine shared library.
- Depends on: `python/src/moonshine_voice/errors.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`, `scripts/eval-alphanumeric.py`

### _setup_function_signatures `def _setup_function_signatures(self)`
- Defined: `python/src/moonshine_voice/moonshine_api.py:642`
- Doc: Setup ctypes function signatures for the C API.
- Depends on: `python/src/moonshine_voice/errors.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`, `scripts/eval-alphanumeric.py`

### lib `def lib(self)`
- Defined: `python/src/moonshine_voice/moonshine_api.py:888`
- Doc: Get the loaded library.
- Depends on: `python/src/moonshine_voice/errors.py`
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`, `scripts/eval-alphanumeric.py`

## python/src/moonshine_voice/tts.py

### _load_beep_samples `def _load_beep_samples(np, kind)`
- Defined: `python/src/moonshine_voice/tts.py:88`
- Doc: Return ``(samples_float32, sample_rate)`` for the named beep.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### _import_say_audio_deps `def _import_say_audio_deps()`
- Defined: `python/src/moonshine_voice/tts.py:116`
- Doc: Import numpy and sounddevice for `TextToSpeech.say`; raise MoonshineError if missing.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### _resolve_default_output_index `def _resolve_default_output_index(sd)`
- Defined: `python/src/moonshine_voice/tts.py:129`
- Doc: Return PortAudio's current default output device index, if any.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### list_output_devices `def list_output_devices()`
- Defined: `python/src/moonshine_voice/tts.py:163`
- Doc: Return human-readable output device descriptions for diagnostics.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### _say_enumerate_output_devices `def _say_enumerate_output_devices(sd)`
- Defined: `python/src/moonshine_voice/tts.py:219`
- Doc: PortAudio device indices with at least one output channel, and host API name.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### _say_device_lines `def _say_device_lines(outs)`
- Defined: `python/src/moonshine_voice/tts.py:241`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### _say_device_spec_key `def _say_device_spec_key(device)`
- Defined: `python/src/moonshine_voice/tts.py:245`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### _select_output_sample_rate `def _select_output_sample_rate(sd)`
- Defined: `python/src/moonshine_voice/tts.py:270`
- Doc: Pick the best output sample rate the device will actually open.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### _resample_linear `def _resample_linear(np, samples, source_sr, target_sr)`
- Defined: `python/src/moonshine_voice/tts.py:339`
- Doc: Numpy-only linear-interpolation resample of mono float32 audio.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### _normalize_clone_argument `def _normalize_clone_argument(clone)`
- Defined: `python/src/moonshine_voice/tts.py:360`
- Doc: Return ``(pcm, sample_rate)`` from a ``clone`` spec.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### _autotranscribe_clone_pcm `def _autotranscribe_clone_pcm(pcm, sample_rate)`
- Defined: `python/src/moonshine_voice/tts.py:389`
- Doc: Transcribe a clone reference clip so ZipVoice gets text aligned with the audio.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### _say_resolve_output_index `def _say_resolve_output_index(spec_key, outs)`
- Defined: `python/src/moonshine_voice/tts.py:423`
- Doc: Return PortAudio output device index, or None for the host default stream device.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### _parse_options_cli `def _parse_options_cli(pairs)`
- Defined: `python/src/moonshine_voice/tts.py:1333`
- Doc: Parse ``KEY=value`` pairs from repeated ``--options`` (values stay strings except booleans).
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### _write_wav_mono_pcm16 `def _write_wav_mono_pcm16(path, samples, sample_rate_hz)`
- Defined: `python/src/moonshine_voice/tts.py:1356`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### _try `def _try(sr)`
- Defined: `python/src/moonshine_voice/tts.py:295`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### __init__ `def __init__(self, language)`
- Defined: `python/src/moonshine_voice/tts.py:477`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### _init_playback_state `def _init_playback_state(self, output_device, volume, debug)`
- Defined: `python/src/moonshine_voice/tts.py:604`
- Doc: Shared playback/queue state used by both the from-files and ZipVoice-from-memory paths.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### _init_zipvoice_from_clone `def _init_zipvoice_from_clone(self, language)`
- Defined: `python/src/moonshine_voice/tts.py:636`
- Doc: Create a ZipVoice synthesizer from an in-memory reference clip (mono float PCM).
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### _announce_resolved_device `def _announce_resolved_device(self, sd, resolved)`
- Defined: `python/src/moonshine_voice/tts.py:734`
- Doc: Print a one-liner identifying the PortAudio device we opened.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### _log `def _log(self, msg)`
- Defined: `python/src/moonshine_voice/tts.py:793`
- Doc: Emit a timestamped trace line to stderr when ``debug=True``.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### _c_options_for_create `def _c_options_for_create(self)`
- Defined: `python/src/moonshine_voice/tts.py:819`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### language `def language(self)`
- Defined: `python/src/moonshine_voice/tts.py:828`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### asset_root `def asset_root(self)`
- Defined: `python/src/moonshine_voice/tts.py:832`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### synthesize `def synthesize(self, text)`
- Defined: `python/src/moonshine_voice/tts.py:835`
- Doc: Synthesize ``text`` to PCM float samples ``(-1..1)`` and sample rate in Hz.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### synthesize_from_phonemes `def synthesize_from_phonemes(self, phonemes)`
- Defined: `python/src/moonshine_voice/tts.py:856`
- Doc: Synthesize speech directly from IPA ``phonemes``, skipping grapheme-to-phoneme conversion.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### say `def say(self, text)`
- Defined: `python/src/moonshine_voice/tts.py:883`
- Doc: Queue ``text`` for synthesis and playback, returning immediately.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### play_error `def play_error(self)`
- Defined: `python/src/moonshine_voice/tts.py:928`
- Doc: Play the bundled "error" beep and return immediately.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### play_success `def play_success(self)`
- Defined: `python/src/moonshine_voice/tts.py:962`
- Doc: Play the bundled "success" beep and return immediately.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### _ensure_say_workers `def _ensure_say_workers(self)`
- Defined: `python/src/moonshine_voice/tts.py:987`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### _synth_worker `def _synth_worker(self)`
- Defined: `python/src/moonshine_voice/tts.py:1005`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### _synthesize_one `def _synthesize_one(self, req, np)`
- Defined: `python/src/moonshine_voice/tts.py:1060`
- Doc: Synthesize a single utterance into a _PlayItem (runs on synthesis thread).
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### _play_worker `def _play_worker(self)`
- Defined: `python/src/moonshine_voice/tts.py:1069`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### _play_one `def _play_one(self, item, sd, np)`
- Defined: `python/src/moonshine_voice/tts.py:1097`
- Doc: Resolve the device and play a single synthesized utterance (runs on playback thread).
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### is_talking `def is_talking(self)`
- Defined: `python/src/moonshine_voice/tts.py:1242`
- Doc: Return ``True`` if utterances are queued, being synthesized, or currently playing.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### wait `def wait(self)`
- Defined: `python/src/moonshine_voice/tts.py:1255`
- Doc: Block until all queued utterances have been synthesized and played.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### stop `def stop(self)`
- Defined: `python/src/moonshine_voice/tts.py:1260`
- Doc: Clear the utterance queue and stop any audio currently playing.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### close `def close(self)`
- Defined: `python/src/moonshine_voice/tts.py:1288`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### __enter__ `def __enter__(self)`
- Defined: `python/src/moonshine_voice/tts.py:1320`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### __exit__ `def __exit__(self, exc_type, exc, tb)`
- Defined: `python/src/moonshine_voice/tts.py:1323`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### __del__ `def __del__(self)`
- Defined: `python/src/moonshine_voice/tts.py:1326`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

## python/src/moonshine_voice/utils.py

### get_assets_path `def get_assets_path()`
- Defined: `python/src/moonshine_voice/utils.py:9`
- Doc: Get the path to the assets directory included in the package.
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`

### get_model_path `def get_model_path(model_name)`
- Defined: `python/src/moonshine_voice/utils.py:27`
- Doc: Get the path to a specific model directory in the assets folder.
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`

### load_wav_file `def load_wav_file(file_path)`
- Defined: `python/src/moonshine_voice/utils.py:47`
- Doc: Load a WAV file and return audio data as float array and sample rate.
- Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/tts.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`

## python/tests/test_cli.py

### console_script `def console_script(name)`
- Defined: `python/tests/test_cli.py:24`
- Doc: Locate the installed console script, falling back to ``python -m``.
- Depends on: `python/src/moonshine_voice/cli.py`

### run `def run()`
- Defined: `python/tests/test_cli.py:40`
- Depends on: `python/src/moonshine_voice/cli.py`

### describe `def describe(result)`
- Defined: `python/tests/test_cli.py:49`
- Depends on: `python/src/moonshine_voice/cli.py`

### test_console_scripts_are_installed `def test_console_scripts_are_installed(name)`
- Defined: `python/tests/test_cli.py:58`
- Doc: Both the primary command and the short alias must be on PATH.
- Depends on: `python/src/moonshine_voice/cli.py`

### test_help_lists_every_command `def test_help_lists_every_command()`
- Defined: `python/tests/test_cli.py:65`
- Depends on: `python/src/moonshine_voice/cli.py`

### test_version_reports_package_name `def test_version_reports_package_name()`
- Defined: `python/tests/test_cli.py:72`
- Depends on: `python/src/moonshine_voice/cli.py`

### test_unknown_command_is_a_usage_error `def test_unknown_command_is_a_usage_error()`
- Defined: `python/tests/test_cli.py:78`
- Depends on: `python/src/moonshine_voice/cli.py`

### test_subcommand_help_parses `def test_subcommand_help_parses(command)`
- Defined: `python/tests/test_cli.py:84`
- Doc: ``<command> --help`` must succeed and show the friendly command prefix.
- Depends on: `python/src/moonshine_voice/cli.py`

## python/tests/test_docs.py

### parse_annotation `def parse_annotation(line)`
- Defined: `python/tests/test_docs.py:73`
- Doc: Returns the doc-test mode from an annotation comment, or None.

### extract_blocks `def extract_blocks(path)`
- Defined: `python/tests/test_docs.py:84`
- Doc: Yields a DocBlock for every fenced code block in a markdown file.

### resolve_mode `def resolve_mode(language, annotation)`
- Defined: `python/tests/test_docs.py:120`

### collect_all_blocks `def collect_all_blocks()`
- Defined: `python/tests/test_docs.py:130`

### run_bash_block `def run_bash_block(block, cwd, timeout)`
- Defined: `python/tests/test_docs.py:137`
- Doc: Runs a bash block as a script, returning the CompletedProcess.

### check_python_syntax `def check_python_syntax(block)`
- Defined: `python/tests/test_docs.py:158`

### describe `def describe(result)`
- Defined: `python/tests/test_docs.py:171`

### test_doc_block `def test_doc_block(block, tmp_path)`
- Defined: `python/tests/test_docs.py:185`

### test_id `def test_id(self)`
- Defined: `python/tests/test_docs.py:68`

## python/tests/test_mic_transcriber_threading.py

### test_capture_callback_is_not_blocked_by_transcription `def test_capture_callback_is_not_blocked_by_transcription(monkeypatch)`
- Defined: `python/tests/test_mic_transcriber_threading.py:165`

### __init__ `def __init__(self, update_interval)`
- Defined: `python/tests/test_mic_transcriber_threading.py:55`

### start `def start(self)`
- Defined: `python/tests/test_mic_transcriber_threading.py:66`

### stop `def stop(self)`
- Defined: `python/tests/test_mic_transcriber_threading.py:69`

### close `def close(self)`
- Defined: `python/tests/test_mic_transcriber_threading.py:73`

### set_transcribe_flags `def set_transcribe_flags(self, flags)`
- Defined: `python/tests/test_mic_transcriber_threading.py:76`

### add_listener `def add_listener(self, listener)`
- Defined: `python/tests/test_mic_transcriber_threading.py:79`

### remove_listener `def remove_listener(self, listener)`
- Defined: `python/tests/test_mic_transcriber_threading.py:82`

### remove_all_listeners `def remove_all_listeners(self)`
- Defined: `python/tests/test_mic_transcriber_threading.py:85`

### add_audio `def add_audio(self, audio_data, sample_rate)`
- Defined: `python/tests/test_mic_transcriber_threading.py:88`

### _run_update `def _run_update(self)`
- Defined: `python/tests/test_mic_transcriber_threading.py:97`

### __init__ `def __init__(self)`
- Defined: `python/tests/test_mic_transcriber_threading.py:105`

### create_stream `def create_stream(self, update_interval, flags, transcribe_flags)`
- Defined: `python/tests/test_mic_transcriber_threading.py:108`

### close `def close(self)`
- Defined: `python/tests/test_mic_transcriber_threading.py:112`

### __init__ `def __init__(self, samplerate, blocksize, device, channels, dtype, callback)`
- Defined: `python/tests/test_mic_transcriber_threading.py:125`

### start `def start(self)`
- Defined: `python/tests/test_mic_transcriber_threading.py:135`

### stop `def stop(self)`
- Defined: `python/tests/test_mic_transcriber_threading.py:139`

### close `def close(self)`
- Defined: `python/tests/test_mic_transcriber_threading.py:142`

### _feed `def _feed(self)`
- Defined: `python/tests/test_mic_transcriber_threading.py:145`

## python/tests/test_modules.py

### run_module `def run_module(module)`
- Defined: `python/tests/test_modules.py:29`
- Depends on: `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### describe `def describe(result)`
- Defined: `python/tests/test_modules.py:39`
- Depends on: `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### assets_path `def assets_path()`
- Defined: `python/tests/test_modules.py:47`
- Depends on: `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### test_transcriber_transcribes_bundled_audio `def test_transcriber_transcribes_bundled_audio()`
- Defined: `python/tests/test_modules.py:52`
- Depends on: `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### test_diarization_finds_two_speakers_on_endgame_clip `def test_diarization_finds_two_speakers_on_endgame_clip()`
- Defined: `python/tests/test_modules.py:62`
- Doc: Synthetic Nagg/Nell ZipVoice dialogue should yield two speaker IDs.
- Depends on: `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### test_tts_synthesizes_wav `def test_tts_synthesizes_wav(tmp_path)`
- Defined: `python/tests/test_modules.py:109`
- Depends on: `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### test_g2p_prints_ipa `def test_g2p_prints_ipa()`
- Defined: `python/tests/test_modules.py:124`
- Depends on: `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### test_intent_recognizer_triggers_intents `def test_intent_recognizer_triggers_intents()`
- Defined: `python/tests/test_modules.py:130`
- Depends on: `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### test_download_g2p_assets `def test_download_g2p_assets()`
- Defined: `python/tests/test_modules.py:143`
- Depends on: `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### test_dialog_flow_lists_output_devices `def test_dialog_flow_lists_output_devices()`
- Defined: `python/tests/test_modules.py:150`
- Depends on: `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

### test_mic_module_arguments_parse `def test_mic_module_arguments_parse(module, args)`
- Defined: `python/tests/test_modules.py:162`
- Doc: Microphone modules can't run headlessly, so just start them and make
- Depends on: `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`

## scripts/analyze_ko_phoneme_patterns.py

### levenshtein_alignment `def levenshtein_alignment(s, t)`
- Defined: `scripts/analyze_ko_phoneme_patterns.py:29`
- Doc: Return (distance, list of (op, s_char, t_char)) edit operations.

### extract_substitution_patterns `def extract_substitution_patterns(ops, context_size)`
- Defined: `scripts/analyze_ko_phoneme_patterns.py:63`
- Doc: Extract substitution/insertion/deletion patterns with surrounding context.

### classify_phoneme `def classify_phoneme(ch)`
- Defined: `scripts/analyze_ko_phoneme_patterns.py:82`
- Doc: Classify a single IPA character into a broad category.

### main `def main()`
- Defined: `scripts/analyze_ko_phoneme_patterns.py:98`

## scripts/analyze_ko_stress.py

### count_hangul_syllables `def count_hangul_syllables(word)`
- Defined: `scripts/analyze_ko_stress.py:77`
- Doc: Count Hangul syllable characters in a word.
- Depends on: `python/src/moonshine_voice/download.py`

### extract_stress_positions `def extract_stress_positions(ipa)`
- Defined: `scripts/analyze_ko_stress.py:82`
- Doc: Extract the character positions of stress markers relative to the IPA string.
- Depends on: `python/src/moonshine_voice/download.py`

### extract_stress_pattern `def extract_stress_pattern(ipa, num_syllables)`
- Defined: `scripts/analyze_ko_stress.py:104`
- Doc: Create a simplified stress pattern string.
- Depends on: `python/src/moonshine_voice/download.py`

### analyze_stress_position_type `def analyze_stress_position_type(ipa)`
- Defined: `scripts/analyze_ko_stress.py:140`
- Doc: Classify where primary stress ˈ appears relative to the word start.
- Depends on: `python/src/moonshine_voice/download.py`

### setup_piper_phonemizer `def setup_piper_phonemizer()`
- Defined: `scripts/analyze_ko_stress.py:158`
- Doc: Set up Piper's eSpeak phonemizer with NFC patch.
- Depends on: `python/src/moonshine_voice/download.py`

### get_piper_ipa `def get_piper_ipa(phonemizer, word)`
- Defined: `scripts/analyze_ko_stress.py:188`
- Depends on: `python/src/moonshine_voice/download.py`

### main `def main()`
- Defined: `scripts/analyze_ko_stress.py:198`
- Depends on: `python/src/moonshine_voice/download.py`

### phonemize_nfc `def phonemize_nfc(self, voice, text)`
- Defined: `scripts/analyze_ko_stress.py:163`
- Depends on: `python/src/moonshine_voice/download.py`

## scripts/check-banned-constructs.sh

### scan
- Defined: `scripts/check-banned-constructs.sh:76`
- Doc: Print repo-relative paths of first-party files matching a regex, sorted.

## scripts/check-clang-tidy.sh

### extract_keys
- Defined: `scripts/check-clang-tidy.sh:60`
- Doc: Extract a sorted, de-duplicated list of "<check>\t<relpath>" pairs from a clang-tidy log. run-clang-tidy prints one "pat

## scripts/compare_ko_phonemes.py

### get_piper_phonemes `def get_piper_phonemes(text, piper_voice)`
- Defined: `scripts/compare_ko_phonemes.py:28`
- Doc: Get phonemes from Piper's eSpeak phonemizer.
- Depends on: `python/src/moonshine_voice/download.py`

### levenshtein_alignment `def levenshtein_alignment(s, t)`
- Defined: `scripts/compare_ko_phonemes.py:42`
- Doc: Return (distance, list of (op, s_char, t_char)) edit operations.
- Depends on: `python/src/moonshine_voice/download.py`

### classify_char `def classify_char(ch)`
- Defined: `scripts/compare_ko_phonemes.py:75`
- Depends on: `python/src/moonshine_voice/download.py`

### main `def main()`
- Defined: `scripts/compare_ko_phonemes.py:87`
- Depends on: `python/src/moonshine_voice/download.py`

### phonemize_nfc `def phonemize_nfc(self, voice, text)`
- Defined: `scripts/compare_ko_phonemes.py:136`
- Depends on: `python/src/moonshine_voice/download.py`

## scripts/convert_tokenizer.py

### write_bin_tokenizer `def write_bin_tokenizer(tokens, output_path)`
- Defined: `scripts/convert_tokenizer.py:29`
- Doc: Write tokens to BinTokenizer format.

### convert_sentencepiece `def convert_sentencepiece(input_path, output_path)`
- Defined: `scripts/convert_tokenizer.py:51`
- Doc: Convert SentencePiece .model file to BinTokenizer format.

### convert_huggingface_json `def convert_huggingface_json(input_path, output_path)`
- Defined: `scripts/convert_tokenizer.py:84`
- Doc: Convert HuggingFace tokenizer.json to BinTokenizer format.

### main `def main()`
- Defined: `scripts/convert_tokenizer.py:127`

## scripts/eval-alphanumeric.py

### folder_name_to_expected_char `def folder_name_to_expected_char(name, matcher)`
- Defined: `scripts/eval-alphanumeric.py:46`
- Doc: Resolve a folder name (e.g. ``"a"``, ``"eight"``) to its character.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/moonshine_api.py`

### predict_character `def predict_character(transcriber, audio, sample_rate, transcribe_flags)`
- Defined: `scripts/eval-alphanumeric.py:54`
- Doc: Run transcription and return predictions for a single clip.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/moonshine_api.py`

### print_confusion_matrix `def print_confusion_matrix(matrix, labels, title)`
- Defined: `scripts/eval-alphanumeric.py:106`
- Doc: Pretty-print a confusion matrix with ``labels`` along both axes.
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/moonshine_api.py`

### main `def main()`
- Defined: `scripts/eval-alphanumeric.py:138`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/moonshine_api.py`

### on_event `def on_event(event)`
- Defined: `scripts/eval-alphanumeric.py:79`
- Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/moonshine_api.py`

## scripts/eval-librispeech.py

### parse_args `def parse_args()`
- Defined: `scripts/eval-librispeech.py:87`

### detect_text_column `def detect_text_column(sample)`
- Defined: `scripts/eval-librispeech.py:149`

### load_eval_dataset `def load_eval_dataset(args)`
- Defined: `scripts/eval-librispeech.py:158`

### decode_audio `def decode_audio(audio_field)`
- Defined: `scripts/eval-librispeech.py:172`
- Doc: Return (float32 mono @16kHz, sample_rate) from a non-decoded audio field.

### make_moonshine_c_backend `def make_moonshine_c_backend(args, streaming)`
- Defined: `scripts/eval-librispeech.py:192`

### make_hf_backend `def make_hf_backend(args)`
- Defined: `scripts/eval-librispeech.py:233`

### main `def main()`
- Defined: `scripts/eval-librispeech.py:282`

### transcribe_batch `def transcribe_batch(audio, sample_rate)`
- Defined: `scripts/eval-librispeech.py:211`

### transcribe_streaming `def transcribe_streaming(audio, sample_rate)`
- Defined: `scripts/eval-librispeech.py:217`

### transcribe `def transcribe(audio, sample_rate)`
- Defined: `scripts/eval-librispeech.py:268`

## scripts/export-decoder-with-attention.py

### main `def main()`
- Defined: `scripts/export-decoder-with-attention.py:33`

## scripts/export_zipvoice_model.py

### run `def run(cmd, cwd)`
- Defined: `scripts/export_zipvoice_model.py:53`

### convert_to_ort `def convert_to_ort(python, onnx_path, custom_op_lib)`
- Defined: `scripts/export_zipvoice_model.py:58`

### main `def main()`
- Defined: `scripts/export_zipvoice_model.py:72`

### deploy `def deploy(src_onnx, canonical_stem)`
- Defined: `scripts/export_zipvoice_model.py:134`

## scripts/export_zipvoice_voices_for_cpp.py

### slug_from_voice_id `def slug_from_voice_id(voice_id)`
- Defined: `scripts/export_zipvoice_voices_for_cpp.py:55`
- Doc: ``voice_000_american_female`` -> ``american_female``.

### select_voices `def select_voices(voices)`
- Defined: `scripts/export_zipvoice_voices_for_cpp.py:60`
- Doc: One masculine + one feminine speaker per accent (first of each in file order).

### _clean_cut_index `def _clean_cut_index(wav, sr, max_samples)`
- Defined: `scripts/export_zipvoice_voices_for_cpp.py:81`
- Doc: End index (<= max_samples) that ends at a *strong* natural pause when possible.

### load_clip_pcm16 `def load_clip_pcm16(path)`
- Defined: `scripts/export_zipvoice_voices_for_cpp.py:127`

### c_escape `def c_escape(s)`
- Defined: `scripts/export_zipvoice_voices_for_cpp.py:177`

### main `def main()`
- Defined: `scripts/export_zipvoice_voices_for_cpp.py:181`

### __init__ `def __init__(self)`
- Defined: `scripts/export_zipvoice_voices_for_cpp.py:154`

### transcribe_pcm16 `def transcribe_pcm16(self, pcm)`
- Defined: `scripts/export_zipvoice_voices_for_cpp.py:165`

### close `def close(self)`
- Defined: `scripts/export_zipvoice_voices_for_cpp.py:170`

## scripts/generate-diarization-test-audio.py

### _synthesize_utterance `def _synthesize_utterance(voice, text, asset_root)`
- Defined: `scripts/generate-diarization-test-audio.py:60`

### _append_silence `def _append_silence(samples, sample_rate, seconds)`
- Defined: `scripts/generate-diarization-test-audio.py:78`

### generate_dialogue_wav `def generate_dialogue_wav(asset_root)`
- Defined: `scripts/generate-diarization-test-audio.py:84`

### main `def main()`
- Defined: `scripts/generate-diarization-test-audio.py:97`

## scripts/generate-silero-vad-data.py

### fetch_source_onnx `def fetch_source_onnx(dest_dir)`
- Defined: `scripts/generate-silero-vad-data.py:88`
- Doc: Download the pinned upstream Silero VAD .onnx and verify its SHA-256.

### convert_onnx_to_ort `def convert_onnx_to_ort(onnx_path, out_dir, optimization)`
- Defined: `scripts/generate-silero-vad-data.py:105`
- Doc: Serialize an .onnx model to a .ort flatbuffer at the given opt level.

### render_header `def render_header(data, source_name, optimization)`
- Defined: `scripts/generate-silero-vad-data.py:130`

### main `def main()`
- Defined: `scripts/generate-silero-vad-data.py:159`

## scripts/patch-release.sh

### main
- Defined: `scripts/patch-release.sh:32`

## scripts/prepare-release.sh

### main
- Defined: `scripts/prepare-release.sh:67`
- Doc: All imperative work lives inside main() so bash parses the whole script before executing anything (mirrors build-all-pla

## scripts/reliability-remote.sh

### record_failure
- Defined: `scripts/reliability-remote.sh:69`

### require_tool
- Defined: `scripts/reliability-remote.sh:89`

### run_test
- Defined: `scripts/reliability-remote.sh:183`

### run_fuzzer
- Defined: `scripts/reliability-remote.sh:439`

## scripts/run-benchmarks.py

### __init__ `def __init__(self)`
- Defined: `scripts/run-benchmarks.py:133`

### on_line_completed `def on_line_completed(self, event)`
- Defined: `scripts/run-benchmarks.py:137`

## scripts/setup-android-ci.sh

### log
- Defined: `scripts/setup-android-ci.sh:27`

## scripts/test-android.sh

### log
- Defined: `scripts/test-android.sh:37`

### die
- Defined: `scripts/test-android.sh:38`

### cleanup
- Defined: `scripts/test-android.sh:82`

## scripts/test-docs.sh

### cleanup
- Defined: `scripts/test-docs.sh:31`

## scripts/test-examples.sh

### usage
- Defined: `scripts/test-examples.sh:56`

### log
- Defined: `scripts/test-examples.sh:94`

### die
- Defined: `scripts/test-examples.sh:98`

### cleanup
- Defined: `scripts/test-examples.sh:157`

### download_url_for
- Defined: `scripts/test-examples.sh:169`

### download_one
- Defined: `scripts/test-examples.sh:178`

### extract_tgz
- Defined: `scripts/test-examples.sh:194`

### list_example_project_names
- Defined: `scripts/test-examples.sh:204`
- Doc: List immediate child directories of examples/<platform>/ (used to know which release assets to download: <platform>-<dir

### download_platform_example_archives
- Defined: `scripts/test-examples.sh:213`
- Doc: Download every <platform>-<project>.tar.gz for that platform and extract into dest_root (same layout as the old monolith

### copy_local_example_trees
- Defined: `scripts/test-examples.sh:230`
- Doc: Copy examples/android and examples/ios from the repository (parent of scripts/) into the same layout used after extracti

### portable_sed_inplace
- Defined: `scripts/test-examples.sh:247`
- Doc: Portable in-place edit (BSD/macOS sed and GNU sed differ on -i), applied to each given file with the supplied sed expres

### read_library_version
- Defined: `scripts/test-examples.sh:260`
- Doc: Read the moonshine-voice version this checkout would publish, parsed from the root build.gradle.kts coordinates("ai.moon

### publish_local_library
- Defined: `scripts/test-examples.sh:270`
- Doc: Build the AAR from this checkout and install it into the local Maven cache so the example builds can resolve it. Delegat

### write_local_library_init_script
- Defined: `scripts/test-examples.sh:279`
- Doc: Write a Gradle init script that adds mavenLocal() as the first dependency resolution repository for every build. Using b

### apply_local_library_overrides
- Defined: `scripts/test-examples.sh:299`
- Doc: Point the copied Android examples at the locally-built library: sync each example's requested moonshine-voice version to

### ensure_local_swift_package
- Defined: `scripts/test-examples.sh:320`
- Doc: Ensure a locally-built XCFramework exists for the swift package to wrap. The example apps consume the MoonshineVoice pro

### copy_local_swift_package
- Defined: `scripts/test-examples.sh:333`
- Doc: Copy this checkout's swift/ package into the iOS tree so the examples can reference it locally. Excludes the SwiftPM .bu

### rewrite_pbxproj_to_local_package
- Defined: `scripts/test-examples.sh:346`
- Doc: Rewrite one project.pbxproj so its remote moonshine-swift package reference becomes a local reference at ${relpath}. The

### apply_local_library_overrides_ios
- Defined: `scripts/test-examples.sh:414`
- Doc: Point every copied iOS example at the local swift package.

### pick_xcode_scheme
- Defined: `scripts/test-examples.sh:430`

### run_android_builds
- Defined: `scripts/test-examples.sh:474`

### run_ios_builds
- Defined: `scripts/test-examples.sh:512`

### main
- Defined: `scripts/test-examples.sh:552`

## scripts/test-model-downloads.sh

### download_and_run
- Defined: `scripts/test-model-downloads.sh:103`
- Doc: download_and_run <label> <modality> <spec...> The spec is passed both to the manifest and run subcommands. The model roo

### run_swift_framework_tests
- Defined: `scripts/test-model-downloads.sh:195`
- Doc: Swift: run the opt-in network tests when a Swift toolchain and the local XCFramework the package links against are both 

### run_android_framework_tests
- Defined: `scripts/test-model-downloads.sh:223`
- Doc: Android: run the opt-in instrumentation test, but only if a device/emulator is already connected (this script does not m

## scripts/test-python.sh

### cleanup
- Defined: `scripts/test-python.sh:28`

## scripts/tts_g2p_intelligibility.py

### levenshtein_distance `def levenshtein_distance(s, t)`
- Defined: `scripts/tts_g2p_intelligibility.py:102`
- Doc: Character-level Levenshtein (edit) distance between two strings.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### uses_wikitext2_corpus `def uses_wikitext2_corpus(tag)`
- Defined: `scripts/tts_g2p_intelligibility.py:218`
- Doc: WikiText-2 on Hugging Face is English-only; use it for US/UK (and generic ``en``) tags.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### moonshine_tag_to_wikipedia_lang `def moonshine_tag_to_wikipedia_lang(tag)`
- Defined: `scripts/tts_g2p_intelligibility.py:226`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### moonshine_tag_to_whisper_language `def moonshine_tag_to_whisper_language(tag)`
- Defined: `scripts/tts_g2p_intelligibility.py:238`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### moonshine_tag_to_upstream_kokoro_lang_code `def moonshine_tag_to_upstream_kokoro_lang_code(tag)`
- Defined: `scripts/tts_g2p_intelligibility.py:250`
- Doc: Locale supported by ``pip install kokoro`` / ``KPipeline`` (not all Moonshine TTS languages).
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### load_wiki_text_directory `def load_wiki_text_directory(dir_path)`
- Defined: `scripts/tts_g2p_intelligibility.py:268`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### _read_nonempty_lines `def _read_nonempty_lines(text)`
- Defined: `scripts/tts_g2p_intelligibility.py:278`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### load_wiki_text_file `def load_wiki_text_file(path)`
- Defined: `scripts/tts_g2p_intelligibility.py:288`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### load_wiki_texts `def load_wiki_texts(path)`
- Defined: `scripts/tts_g2p_intelligibility.py:319`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### _wiki_max_graphemes_for_moonshine_tag `def _wiki_max_graphemes_for_moonshine_tag(tag, base_max)`
- Defined: `scripts/tts_g2p_intelligibility.py:325`
- Doc: Cap line length for locales whose native G2P tokenizer expands text (e.g. Chinese WordPiece
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### clean_wiki_text_line `def clean_wiki_text_line(raw)`
- Defined: `scripts/tts_g2p_intelligibility.py:339`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### _split_oversized_wiki_piece `def _split_oversized_wiki_piece(s)`
- Defined: `scripts/tts_g2p_intelligibility.py:360`
- Doc: Wikipedia dumps often use a few very long lines per article. ``clean_wiki_text_line`` caps length,
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### normalize_eval_lines `def normalize_eval_lines(raw_lines)`
- Defined: `scripts/tts_g2p_intelligibility.py:415`
- Doc: Chunk or filter lines so each fits Moonshine G2P / TTS (same bounds as wiki download).
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### wikipedia_paragraph_to_candidates `def wikipedia_paragraph_to_candidates(para)`
- Defined: `scripts/tts_g2p_intelligibility.py:446`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### try_import_datasets `def try_import_datasets()`
- Defined: `scripts/tts_g2p_intelligibility.py:477`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### _parse_datasets_version_tuple `def _parse_datasets_version_tuple(version)`
- Defined: `scripts/tts_g2p_intelligibility.py:486`
- Doc: Best-effort parse for ``datasets.__version__`` (handles ``4.4.0rc1``).
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### require_datasets_compatible_with_python `def require_datasets_compatible_with_python()`
- Defined: `scripts/tts_g2p_intelligibility.py:506`
- Doc: ``datasets`` before 4.4.0 breaks on Python 3.14 inside dill/pickle (Hasher.hash / load_dataset).
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### fetch_lines_wikitext2 `def fetch_lines_wikitext2()`
- Defined: `scripts/tts_g2p_intelligibility.py:528`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### _prefers_natural_wikipedia_prose_for_tag `def _prefers_natural_wikipedia_prose_for_tag(tag)`
- Defined: `scripts/tts_g2p_intelligibility.py:569`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### _german_wikipedia_lead_penalty `def _german_wikipedia_lead_penalty(line)`
- Defined: `scripts/tts_g2p_intelligibility.py:576`
- Doc: Higher → more like a corporate / legal / definition lead (sample these later).
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### fetch_lines_wikipedia `def fetch_lines_wikipedia(wiki_lang)`
- Defined: `scripts/tts_g2p_intelligibility.py:593`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### fetch_lines_for_moonshine_language `def fetch_lines_for_moonshine_language(lang_tag)`
- Defined: `scripts/tts_g2p_intelligibility.py:655`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### all_moonshine_tts_language_tags `def all_moonshine_tts_language_tags()`
- Defined: `scripts/tts_g2p_intelligibility.py:672`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### ensure_wiki_text_files `def ensure_wiki_text_files(output_dir, languages)`
- Defined: `scripts/tts_g2p_intelligibility.py:682`
- Doc: Ensure ``output_dir/<lang>.txt`` exists for each language.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### resample_linear `def resample_linear(samples, orig_sr, target_sr)`
- Defined: `scripts/tts_g2p_intelligibility.py:735`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### _tts_cache_key `def _tts_cache_key(payload)`
- Defined: `scripts/tts_g2p_intelligibility.py:749`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### _tts_track_to_engine_slug `def _tts_track_to_engine_slug(track)`
- Defined: `scripts/tts_g2p_intelligibility.py:754`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### _tts_sentence_prefix_for_cache `def _tts_sentence_prefix_for_cache(text, max_chars)`
- Defined: `scripts/tts_g2p_intelligibility.py:766`
- Doc: First ``max_chars`` Unicode scalars of the line, scrubbed for use in filenames.
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### _tts_cache_stem `def _tts_cache_stem(text, track, payload)`
- Defined: `scripts/tts_g2p_intelligibility.py:778`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### _tts_cache_wav_and_meta_paths `def _tts_cache_wav_and_meta_paths(root, lang, stem)`
- Defined: `scripts/tts_g2p_intelligibility.py:785`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### _write_wav_int16_mono `def _write_wav_int16_mono(path, samples, sample_rate)`
- Defined: `scripts/tts_g2p_intelligibility.py:792`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### _read_wav_int16_mono `def _read_wav_int16_mono(path)`
- Defined: `scripts/tts_g2p_intelligibility.py:803`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### _load_tts_wav_meta `def _load_tts_wav_meta(meta_path)`
- Defined: `scripts/tts_g2p_intelligibility.py:819`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### _save_tts_wav_meta `def _save_tts_wav_meta(meta_path, phonemes)`
- Defined: `scripts/tts_g2p_intelligibility.py:832`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### _try_read_tts_wav_cache `def _try_read_tts_wav_cache(cache_root, lang, payload)`
- Defined: `scripts/tts_g2p_intelligibility.py:845`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### _write_tts_wav_cache `def _write_tts_wav_cache(cache_root, lang, payload, samples, sample_rate, phonemes)`
- Defined: `scripts/tts_g2p_intelligibility.py:872`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### try_import_cer `def try_import_cer()`
- Defined: `scripts/tts_g2p_intelligibility.py:894`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### try_import_whisper_model `def try_import_whisper_model()`
- Defined: `scripts/tts_g2p_intelligibility.py:903`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### discover_voices `def discover_voices(language, asset_root)`
- Defined: `scripts/tts_g2p_intelligibility.py:918`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### prepare_asset_root `def prepare_asset_root(language, voices, cache_root)`
- Defined: `scripts/tts_g2p_intelligibility.py:931`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### overlay_repo_tts_data_into_asset_root `def overlay_repo_tts_data_into_asset_root(asset_root, tts_data_root, lang)`
- Defined: `scripts/tts_g2p_intelligibility.py:955`
- Doc: Copy files from ``tts_data_root/<lang>/`` onto the downloaded asset tree so repo
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### _kokoro_ja_text_for_misaki_cutlet `def _kokoro_ja_text_for_misaki_cutlet(text)`
- Defined: `scripts/tts_g2p_intelligibility.py:989`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### moonshine_kokoro_catalog_voice_to_package_voice `def moonshine_kokoro_catalog_voice_to_package_voice(catalog_id)`
- Defined: `scripts/tts_g2p_intelligibility.py:995`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### try_import_k_pipeline `def try_import_k_pipeline()`
- Defined: `scripts/tts_g2p_intelligibility.py:1002`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### try_import_piper_voice `def try_import_piper_voice()`
- Defined: `scripts/tts_g2p_intelligibility.py:1011`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### ensure_piper_espeak_phonemizer_uses_nfc_for_eval `def ensure_piper_espeak_phonemizer_uses_nfc_for_eval()`
- Defined: `scripts/tts_g2p_intelligibility.py:1023`
- Doc: ``piper-tts`` decomposes espeak IPA with Unicode NFD, so combining marks (e.g. U+0327 cedilla)
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### resolve_piper_onnx_path `def resolve_piper_onnx_path(asset_root, piper_voice_catalog_id)`
- Defined: `scripts/tts_g2p_intelligibility.py:1074`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### build_upstream_kokoro_pipeline `def build_upstream_kokoro_pipeline(lang_code)`
- Defined: `scripts/tts_g2p_intelligibility.py:1086`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### synthesize_upstream_kokoro_package `def synthesize_upstream_kokoro_package(pipeline, text, voice)`
- Defined: `scripts/tts_g2p_intelligibility.py:1104`
- Doc: hexgrad/kokoro ``KPipeline`` (misaki + espeak-ng G2P inside the package).
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### synthesize_upstream_piper_package `def synthesize_upstream_piper_package(piper_voice, text)`
- Defined: `scripts/tts_g2p_intelligibility.py:1136`
- Doc: ``piper-tts`` ``PiperVoice`` (phonemize + espeak-ng data bundled with the package).
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### transcribe_whisper `def transcribe_whisper(model, samples, sample_rate, whisper_lang)`
- Defined: `scripts/tts_g2p_intelligibility.py:1180`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### run_language `def run_language(language, lines)`
- Defined: `scripts/tts_g2p_intelligibility.py:1197`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### line_result_to_dict `def line_result_to_dict(r)`
- Defined: `scripts/tts_g2p_intelligibility.py:1474`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### _fmt_metric `def _fmt_metric(x)`
- Defined: `scripts/tts_g2p_intelligibility.py:1494`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### _fmt_cer_percent `def _fmt_cer_percent(x)`
- Defined: `scripts/tts_g2p_intelligibility.py:1498`
- Doc: Format CER as a percentage for markdown tables (jiwer CER is a 0–1 ratio).
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### _reference_cer_from_upstream_averages `def _reference_cer_from_upstream_averages(kokoro, piper)`
- Defined: `scripts/tts_g2p_intelligibility.py:1505`
- Doc: Reference CER: lowest of Kokoro and Piper when both are present; otherwise whichever upstream
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### format_cer_summary_markdown_table `def format_cer_summary_markdown_table(languages_report)`
- Defined: `scripts/tts_g2p_intelligibility.py:1519`
- Doc: GitHub-flavored markdown table: Language, Moonshine CER, Reference CER (min Kokoro/Piper).
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### main `def main()`
- Defined: `scripts/tts_g2p_intelligibility.py:1556`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### flush `def flush()`
- Defined: `scripts/tts_g2p_intelligibility.py:295`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

### phonemize_nfc `def phonemize_nfc(self, voice, text)`
- Defined: `scripts/tts_g2p_intelligibility.py:1041`
- Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`

## swift/Sources/MoonshineVoice/Errors.swift

### checkError
- Defined: `swift/Sources/MoonshineVoice/Errors.swift:40`
- Doc: Helper function to check error codes and throw appropriate Swift errors

## swift/Sources/MoonshineVoice/MicTranscriber.swift

### feedCapturedAudio
- Defined: `swift/Sources/MoonshineVoice/MicTranscriber.swift:262`
- Doc: Sink for a single captured audio buffer.  Called from the ``AVAudioEngine`` capture tap (a high-priority audio thread), 

## swift/Sources/MoonshineVoice/MoonshineAPI.swift

### getVersion
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:21`
- Doc: Get the version of the loaded Moonshine library.

### errorToString
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:26`
- Doc: Convert an error code to a human-readable string.

### loadTranscriberFromFiles
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:34`
- Doc: Load a transcriber from files on disk.

### freeTranscriber
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:93`
- Doc: Free a transcriber handle.

### transcribeWithoutStreaming
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:98`
- Doc: Transcribe audio without streaming.

### createStream
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:134`
- Doc: Create a stream for real-time transcription.

### freeStream
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:141`
- Doc: Free a stream handle.

### startStream
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:147`
- Doc: Start a stream.

### stopStream
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:153`
- Doc: Stop a stream.

### addAudioToStream
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:159`
- Doc: Add audio data to a stream.

### transcribeStream
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:184`
- Doc: Transcribe a stream and get updated results.

### createTtsSynthesizerFromFiles
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:305`
- Doc: Create a TTS synthesizer from files on disk.

### createTtsSynthesizerFromMemory
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:361`
- Doc: Create a TTS synthesizer from in-memory asset buffers keyed by canonical filename.  The buffers pointed to by ``memoryPt

### textToSpeech
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:421`
- Doc: Synthesize text to speech, returning PCM float samples and sample rate.

### phonemesToSpeech
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:485`
- Doc: Synthesize speech from IPA phonemes, returning PCM float samples and sample rate.  `phonemes` is an IPA string in the sa

### freeTtsSynthesizer
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:545`
- Doc: Free a TTS synthesizer handle.

### getTtsVoices
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:550`
- Doc: Get TTS voices JSON for the given languages.

### getTtsDependencies
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:600`
- Doc: Get TTS dependencies JSON for the given languages.

### getG2pDependencies
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:650`
- Doc: Get G2P-only asset dependency keys as a comma-separated string.

### getSttDependencies
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:668`
- Doc: Get the speech-to-text model download manifest as a JSON object string.  - Parameters: - language: Language code (e.g. `

### getIntentDependencies
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:685`
- Doc: Get the intent-recognition embedding model download manifest as a JSON object string.  - Parameters: - modelName: Embedd

### createIntentRecognizer
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:744`
- Doc: MARK: - Intent recognition

### freeIntentRecognizer
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:761`

### registerIntentRecognizerIntent
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:765`

### unregisterIntentRecognizerIntent
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:775`
- Doc: Returns: `true` if an intent was removed, `false` if the phrase was not registered.

### getClosestIntents
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:787`

### getIntentRecognizerIntentCount
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:826`

### clearIntentRecognizerIntents
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:834`

### calculateIntentEmbedding
- Defined: `swift/Sources/MoonshineVoice/MoonshineAPI.swift:838`

## swift/Sources/MoonshineVoice/TranscriptEventListener.swift

### onLineStarted
- Defined: `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:10`
- Doc: Called when a new transcription line starts.

### onLineUpdated
- Defined: `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:13`
- Doc: Called when an existing transcription line is updated.

### onLineTextChanged
- Defined: `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:16`
- Doc: Called when the text of a transcription line changes.

### onLineSpeakersChanged
- Defined: `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:20`
- Doc: Called when the speaker spans of a transcription line change. Can be called for lines that are already complete.

### onLineCompleted
- Defined: `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:23`
- Doc: Called when a transcription line is completed.

### onError
- Defined: `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:26`
- Doc: Called when an error occurs.

### onLineStarted
- Defined: `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:31`

### onLineUpdated
- Defined: `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:32`

### onLineTextChanged
- Defined: `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:33`

### onLineSpeakersChanged
- Defined: `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:34`

### onLineCompleted
- Defined: `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:35`

### onError
- Defined: `swift/Sources/MoonshineVoice/TranscriptEventListener.swift:36`

## swift/Sources/MoonshineVoice/TranscriptionStream.swift

### start
- Defined: `swift/Sources/MoonshineVoice/TranscriptionStream.swift:10`
- Imported by: `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift::FakeStream`

### stop
- Defined: `swift/Sources/MoonshineVoice/TranscriptionStream.swift:11`
- Imported by: `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift::FakeStream`

### close
- Defined: `swift/Sources/MoonshineVoice/TranscriptionStream.swift:12`
- Imported by: `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift::FakeStream`

### addAudio
- Defined: `swift/Sources/MoonshineVoice/TranscriptionStream.swift:13`
- Imported by: `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift::FakeStream`

### addListener
- Defined: `swift/Sources/MoonshineVoice/TranscriptionStream.swift:14`
- Imported by: `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift::FakeStream`

### addListener
- Defined: `swift/Sources/MoonshineVoice/TranscriptionStream.swift:15`
- Imported by: `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift::FakeStream`

### removeListener
- Defined: `swift/Sources/MoonshineVoice/TranscriptionStream.swift:16`
- Imported by: `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift::FakeStream`

### removeListener
- Defined: `swift/Sources/MoonshineVoice/TranscriptionStream.swift:17`
- Imported by: `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift::FakeStream`

### removeAllListeners
- Defined: `swift/Sources/MoonshineVoice/TranscriptionStream.swift:18`
- Imported by: `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift::FakeStream`

## swift/Tests/MoonshineVoiceTests/AssetDownloaderNetworkTests.swift

### setUpWithError
- Defined: `swift/Tests/MoonshineVoiceTests/AssetDownloaderNetworkTests.swift:19`

### tearDown
- Defined: `swift/Tests/MoonshineVoiceTests/AssetDownloaderNetworkTests.swift:27`

### testDownloadsAndRunsSttModel
- Defined: `swift/Tests/MoonshineVoiceTests/AssetDownloaderNetworkTests.swift:49`
- Doc: Downloads the tiny English STT model, loads it with ``Transcriber``, and transcribes a bundled WAV, asserting on known w

### testDownloadsAndRunsTtsVoice
- Defined: `swift/Tests/MoonshineVoiceTests/AssetDownloaderNetworkTests.swift:76`
- Doc: Downloads a Kokoro English voice plus its G2P assets, then synthesizes speech from the downloaded directory.

### testDownloadsAndRunsIntentModel
- Defined: `swift/Tests/MoonshineVoiceTests/AssetDownloaderNetworkTests.swift:96`
- Doc: Downloads the (large) intent-recognition embedding model and runs a trivial match. Gated by the same env var as the othe

## swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift

### setUp
- Defined: `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:13`

### tearDown
- Defined: `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:22`

### testDownloadsSttModelIntoEmptyDirectory
- Defined: `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:93`
- Doc: MARK: - STT

### testSkipsAlreadyPresentFiles
- Defined: `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:107`

### testIncludeSpellingAddsFilesForEnglish
- Defined: `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:122`

### testDownloadsIntentModel
- Defined: `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:144`
- Doc: MARK: - Intent / TTS

### testDownloadsTtsAssetsIntoNestedPaths
- Defined: `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:153`

### testReportsProgress
- Defined: `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:163`
- Doc: MARK: - Progress, errors, resume

### testHttpErrorSurfacesAsAssetDownloadError
- Defined: `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:177`

### testResumesFromPartialDownload
- Defined: `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:196`

### record
- Defined: `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:237`

### canInit
- Defined: `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:285`

### canonicalRequest
- Defined: `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:287`

### startLoading
- Defined: `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:288`

### stopLoading
- Defined: `swift/Tests/MoonshineVoiceTests/AssetDownloaderTests.swift:306`

## swift/Tests/MoonshineVoiceTests/IntentRecognizerTests.swift

### testCreateIntentRecognizer_invalidPath_throws
- Defined: `swift/Tests/MoonshineVoiceTests/IntentRecognizerTests.swift:7`

### testIntentRecognizer_closestIntents_whenEmbeddingModelPresent
- Defined: `swift/Tests/MoonshineVoiceTests/IntentRecognizerTests.swift:21`

## swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift

### start
- Defined: `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift:51`

### close
- Defined: `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift:53`

### stop
- Defined: `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift:56`
- Doc: The real stream flushes any trailing audio on stop.

### addAudio
- Defined: `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift:57`

### addListener
- Defined: `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift:78`

### addListener
- Defined: `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift:80`

### removeListener
- Defined: `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift:81`

### removeListener
- Defined: `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift:82`

### removeAllListeners
- Defined: `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift:83`

### testCaptureCallbackIsNotBlockedByTranscription
- Defined: `swift/Tests/MoonshineVoiceTests/MicTranscriberThreadingTests.swift:95`

## swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift

### testCreateSynthesizer
- Defined: `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:36`
- Doc: MARK: - Creation Tests

### testCreateSynthesizerWithVoice
- Defined: `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:44`

### testCreateSynthesizerInvalidLanguage
- Defined: `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:56`

### testSynthesizeBasic
- Defined: `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:68`
- Doc: MARK: - Synthesis Tests

### testSynthesizeLongerText
- Defined: `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:80`

### testSynthesizeWithVoiceOption
- Defined: `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:100`

### testSynthesizeWithSpeedOption
- Defined: `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:115`

### testSynthesizeSampleRange
- Defined: `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:135`

### testSynthesizeMultipleCalls
- Defined: `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:151`

### testSayDefaultDevice
- Defined: `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:169`
- Doc: MARK: - Say Tests

### testSayMultipleCalls
- Defined: `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:180`

### testGetVoices
- Defined: `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:194`
- Doc: MARK: - Static Query Tests

### testGetDependencies
- Defined: `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:207`

### any
- Defined: `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:225`

### testGetVoicesListsZipVoice
- Defined: `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:233`

### testZipVoiceBuiltinVoiceSynthesizes
- Defined: `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:246`

### testZipVoiceClonePCMSynthesizes
- Defined: `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:258`

### testGetAudioOutputDevices
- Defined: `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:282`
- Doc: if os(macOS)

### testCloseIdempotent
- Defined: `swift/Tests/MoonshineVoiceTests/TextToSpeechTests.swift:296`
- Doc: MARK: - Resource Management

## swift/Tests/MoonshineVoiceTests/TranscriberTests.swift

### testTranscribeWithoutStreaming_beckett
- Defined: `swift/Tests/MoonshineVoiceTests/TranscriberTests.swift:52`
- Doc: MARK: - Non-Streaming Tests

### testTranscribeWithoutStreaming_twoCities
- Defined: `swift/Tests/MoonshineVoiceTests/TranscriberTests.swift:80`

### testTranscribeWithoutStreaming_emptyAudio
- Defined: `swift/Tests/MoonshineVoiceTests/TranscriberTests.swift:108`

### testTranscribeWithStreaming
- Defined: `swift/Tests/MoonshineVoiceTests/TranscriberTests.swift:126`
- Doc: MARK: - Streaming Tests

### testTranscribeWithStreamingAll
- Defined: `swift/Tests/MoonshineVoiceTests/TranscriberTests.swift:200`

### testTranscribeWithStreaming_manualUpdates
- Defined: `swift/Tests/MoonshineVoiceTests/TranscriberTests.swift:205`

### testTranscribeWithStreaming_emptyAudio
- Defined: `swift/Tests/MoonshineVoiceTests/TranscriberTests.swift:233`

### testGetVersion
- Defined: `swift/Tests/MoonshineVoiceTests/TranscriberTests.swift:256`
- Doc: MARK: - Helper Tests

### testFrameworkBundle
- Defined: `swift/Tests/MoonshineVoiceTests/TranscriberTests.swift:267`

### testSpellingModeApiSurface
- Defined: `swift/Tests/MoonshineVoiceTests/TranscriberTests.swift:276`

### testTranscribeWithDebugWAV_twoCities
- Defined: `swift/Tests/MoonshineVoiceTests/TranscriberTests.swift:311`
