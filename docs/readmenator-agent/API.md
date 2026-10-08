# API (page 1 of 10)
Pages: [API.md](API.md), [API_p2.md](API_p2.md), [API_p3.md](API_p3.md), [API_p4.md](API_p4.md), [API_p5.md](API_p5.md), [API_p6.md](API_p6.md), [API_p7.md](API_p7.md), [API_p8.md](API_p8.md), [API_p9.md](API_p9.md), [API_p10.md](API_p10.md)

## android/java/main/java/ai/moonshine/voice/AssetDownloader.java
- `ProgressListener.AssetDownloader` (method) `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:59`
- `ProgressListener.AssetDownloader` (method) `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:69`
- `ProgressListener.isModelPresent` (method) `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:74`
- `ProgressListener.ensureModelPresent` (method) `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:97`
- `ResolvedFile.resolveFiles` (method) `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:126`
- `ResolvedFile.filesFromGroupManifest` (method) `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:158`
- `ResolvedFile.filesFromKeyArray` (method) `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:179`
- `ResolvedFile.filesFromKeyList` (method) `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:191`
- `ResolvedFile.encodeKey` (method) `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:205`
- `ResolvedFile.downloadOne` (method) `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:222`
- `ResolvedFile.ensureSpaceAvailable` (method) `android/java/main/java/ai/moonshine/voice/AssetDownloader.java:305`

## android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java
- `GraphemeToPhonemizer.GraphemeToPhonemizer` (method) `android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java:22`
- `GraphemeToPhonemizer.GraphemeToPhonemizer` (method) `android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java:38`
- `GraphemeToPhonemizer.fromMemory` (method) `android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java:42`
- `GraphemeToPhonemizer.GraphemeToPhonemizer` (method) `android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java:58`
- `GraphemeToPhonemizer.getG2pDependencies` (method) `android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java:65`
- `GraphemeToPhonemizer.toArray` (method) `android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java:68`
- `GraphemeToPhonemizer.getLanguage` (method) `android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java:75`
- `GraphemeToPhonemizer.toIpa` (method) `android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java:81`
- `GraphemeToPhonemizer.toIpa` (method) `android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java:88`
- `GraphemeToPhonemizer.close` (method) `android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java:92`
- `GraphemeToPhonemizer.finalize` (method) `android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java:101`

## android/java/main/java/ai/moonshine/voice/IntentMatch.java
- `IntentMatch.IntentMatch` (method) `android/java/main/java/ai/moonshine/voice/IntentMatch.java:6`

## android/java/main/java/ai/moonshine/voice/IntentRecognizer.java
- `IntentRecognizer.IntentRecognizer` (method) `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java:18`
- `IntentRecognizer.IntentRecognizer` (method) `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java:26`
- `IntentRecognizer.getIntentDependencies` (method) `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java:42`
- `IntentRecognizer.finalize` (method) `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java:57`
- `IntentRecognizer.close` (method) `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java:64`
- `IntentRecognizer.registerIntent` (method) `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java:71`
- `IntentRecognizer.registerIntent` (method) `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java:83`
- `IntentRecognizer.calculateEmbedding` (method) `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java:97`
- `IntentRecognizer.unregisterIntent` (method) `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java:107`
- `IntentRecognizer.getClosestIntents` (method) `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java:118`
- `IntentRecognizer.getIntentCount` (method) `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java:128`
- `IntentRecognizer.clearIntents` (method) `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java:137`
- `IntentRecognizer.checkHandle` (method) `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java:145`

## android/java/main/java/ai/moonshine/voice/JNI.java
Imported by: `android/java/androidTest/java/ai/moonshine/voice/JNITest.java`, `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java`, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java`, `android/java/main/java/ai/moonshine/voice/Transcriber.java`, `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/MainActivity.kt`, `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java`
- `JNI.ensureLibraryLoaded` (method) `android/java/main/java/ai/moonshine/voice/JNI.java:160`

## android/java/main/java/ai/moonshine/voice/MicCaptureProcessor.java
- `MicCaptureProcessor.consumeAudio` (method) `android/java/main/java/ai/moonshine/voice/MicCaptureProcessor.java:20`
- `MicCaptureProcessor.run` (method) `android/java/main/java/ai/moonshine/voice/MicCaptureProcessor.java:40`

## android/java/main/java/ai/moonshine/voice/MicTranscriber.java
- `MicTranscriber.MicTranscriber` (method) `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:20`
- `MicTranscriber.loadFromAssets` (method) `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:32` -- These load* methods are overridden to complete the CompletableFuture when the transcriber is loaded, so we can...
- `MicTranscriber.loadFromAssets` (method) `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:37`
- `MicTranscriber.loadFromFiles` (method) `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:45`
- `MicTranscriber.loadFromMemory` (method) `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:50`
- `MicTranscriber.loadFromMemory` (method) `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:57`
- `MicTranscriber.onMicPermissionGranted` (method) `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:65`
- `MicTranscriber.startProcessing` (method) `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:69`
- `MicTranscriber.startAudioProcessingLoop` (method) `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:74`
- `MicTranscriber.Thread` (method) `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:77`
- `MicTranscriber.run` (method) `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:78`
- `MicTranscriber.startMicCaptureLoop` (method) `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:85`
- `MicTranscriber.stop` (method) `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:95`
- `MicTranscriber.start` (method) `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:100`
- `MicTranscriber.audioProcessingLoop` (method) `android/java/main/java/ai/moonshine/voice/MicTranscriber.java:105`

## android/java/main/java/ai/moonshine/voice/ModelSpec.java
Imported by: `examples/android/TextToSpeech/app/src/main/java/ai/moonshine/examples/texttospeech/MainActivity.kt`
- `ModelSpec.ModelSpec` (method) `android/java/main/java/ai/moonshine/voice/ModelSpec.java:30` -- public final class ModelSpec { public enum Type { STT, TTS, INTENT, G2P } public final Type type; /** Language code...
- `ModelSpec.stt` (method) `android/java/main/java/ai/moonshine/voice/ModelSpec.java:42`
- `ModelSpec.stt` (method) `android/java/main/java/ai/moonshine/voice/ModelSpec.java:47`
- `ModelSpec.tts` (method) `android/java/main/java/ai/moonshine/voice/ModelSpec.java:53`
- `ModelSpec.intent` (method) `android/java/main/java/ai/moonshine/voice/ModelSpec.java:58`
- `ModelSpec.g2p` (method) `android/java/main/java/ai/moonshine/voice/ModelSpec.java:63`
- `ModelSpec.toOptions` (method) `android/java/main/java/ai/moonshine/voice/ModelSpec.java:73`

## android/java/main/java/ai/moonshine/voice/MoonshineDownloadWorker.java
- `MoonshineDownloadWorker.MoonshineDownloadWorker` (method) `android/java/main/java/ai/moonshine/voice/MoonshineDownloadWorker.java:55`
- `MoonshineDownloadWorker.buildRequest` (method) `android/java/main/java/ai/moonshine/voice/MoonshineDownloadWorker.java:65`
- `MoonshineDownloadWorker.toInputData` (method) `android/java/main/java/ai/moonshine/voice/MoonshineDownloadWorker.java:80`
- `MoonshineDownloadWorker.specFromData` (method) `android/java/main/java/ai/moonshine/voice/MoonshineDownloadWorker.java:97`
- `MoonshineDownloadWorker.doWork` (method) `android/java/main/java/ai/moonshine/voice/MoonshineDownloadWorker.java:119`

## android/java/main/java/ai/moonshine/voice/SpeakerSpan.java
- `SpeakerSpan.toString` (method) `android/java/main/java/ai/moonshine/voice/SpeakerSpan.java:24` -- TranscriptLine.haveSpeakersChanged to detect revisions.  public class SpeakerSpan { /** Time offset from the start...

## android/java/main/java/ai/moonshine/voice/TextToSpeech.java
- `PlayItem.TextToSpeech` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:98`
- `PlayItem.TextToSpeech` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:118`
- `PlayItem.fromMemory` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:126`
- `PlayItem.fromZipVoiceClone` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:153`
- `PlayItem.floatPcmToLeBytes` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:167`
- `PlayItem.TextToSpeech` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:176`
- `PlayItem.getLanguage` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:181`
- `PlayItem.getG2pDependencies` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:187`
- `PlayItem.getTtsDependencies` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:197`
- `PlayItem.getTtsVoices` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:207`
- `PlayItem.toArray` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:215`
- `PlayItem.synthesize` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:227`
- `PlayItem.synthesize` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:234`
- `PlayItem.synthesizeFromPhonemes` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:249`
- `PlayItem.synthesizeFromPhonemes` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:256`
- `PlayItem.say` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:270`
- `PlayItem.say` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:278`
- `PlayItem.say` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:286` -- Queue {@code text} for synthesis and playback with options, returning immediately.
- `PlayItem.say` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:302`
- `PlayItem.say` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:309`
- `PlayItem.waitUntilDone` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:327`
- `PlayItem.stop` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:346`
- `PlayItem.isTalking` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:368`
- `PlayItem.ensureWorkers` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:373`
- `PlayItem.synthWorker` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:391`
- `PlayItem.playWorker` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:434`
- `PlayItem.playOneItem` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:459`
- `PlayItem.playPcmFloat` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:469`
- `PlayItem.decrementPending` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:508`
- `PlayItem.drainQueue` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:519`
- `PlayItem.joinWorkers` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:522`
- `PlayItem.getAudioOutputDevices` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:549`
- `PlayItem.obtainSayTrackLocked` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:560`
- `PlayItem.buildAudioTrack` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:604`
- `PlayItem.releaseSayTrackLocked` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:646`
- `PlayItem.close` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:659`
- `PlayItem.finalize` (method) `android/java/main/java/ai/moonshine/voice/TextToSpeech.java:676`

## android/java/main/java/ai/moonshine/voice/Transcriber.java
Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`
- `Transcriber.Transcriber` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:46`
- `Transcriber.Transcriber` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:48`
- `Transcriber.setTranscribeFlags` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:60`
- `Transcriber.getTranscribeFlags` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:61` -- Sets the flags applied to subsequent transcription calls.
- `Transcriber.getSttDependencies` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:75`
- `Transcriber.loadFromFiles` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:88`
- `Transcriber.loadFromMemory` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:99`
- `Transcriber.loadFromMemory` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:113`
- `Transcriber.loadFromAssets` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:125`
- `Transcriber.loadFromAssets` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:140`
- `Transcriber.finalize` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:162`
- `Transcriber.transcribeWithoutStreaming` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:174`
- `Transcriber.transcribeWithoutStreaming` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:180`
- `Transcriber.createStream` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:186`
- `Transcriber.freeStream` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:190`
- `Transcriber.startStream` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:194`
- `Transcriber.stopStream` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:198`
- `Transcriber.start` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:210`
- `Transcriber.stop` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:212`
- `Transcriber.addListener` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:214`
- `Transcriber.removeListener` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:218`
- `Transcriber.removeAllListeners` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:222`
- `Transcriber.addAudio` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:224`
- `Transcriber.addAudioToStream` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:229`
- `Transcriber.notifyFromTranscript` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:242`
- `Transcriber.emit` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:276`
- `Transcriber.getDefaultStreamHandle` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:282`
- `Transcriber.readAllBytes` (method) `android/java/main/java/ai/moonshine/voice/Transcriber.java:290`

## android/java/main/java/ai/moonshine/voice/TranscriberOption.java
Imported by: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java`, `android/java/main/java/ai/moonshine/voice/Transcriber.java`, `examples/android/TextToSpeech/app/src/main/java/ai/moonshine/examples/texttospeech/MainActivity.kt`
- `TranscriberOption.TranscriberOption` (method) `android/java/main/java/ai/moonshine/voice/TranscriberOption.java:5`
- `TranscriberOption.name` (method) `android/java/main/java/ai/moonshine/voice/TranscriberOption.java:10`
- `TranscriberOption.value` (method) `android/java/main/java/ai/moonshine/voice/TranscriberOption.java:14`

## android/java/main/java/ai/moonshine/voice/Transcript.java
- `Transcript.text` (method) `android/java/main/java/ai/moonshine/voice/Transcript.java:6`

## android/java/main/java/ai/moonshine/voice/TranscriptEvent.java
Imported by: `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java`, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java`, `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/MainActivity.kt`, `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java`
- `LineStarted.LineStarted` (method) `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java:17`
- `LineStarted.accept` (method) `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java:24`
- `LineUpdated.LineUpdated` (method) `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java:32`
- `LineUpdated.accept` (method) `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java:39`
- `LineTextChanged.LineTextChanged` (method) `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java:47`
- `LineTextChanged.accept` (method) `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java:54`
- `LineSpeakersChanged.LineSpeakersChanged` (method) `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java:68`
- `LineSpeakersChanged.accept` (method) `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java:75`
- `LineCompleted.LineCompleted` (method) `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java:83`
- `LineCompleted.accept` (method) `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java:90`
- `Error.Error` (method) `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java:98`
- `Error.accept` (method) `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java:105`

## android/java/main/java/ai/moonshine/voice/TranscriptEventListener.java
- `TranscriptEventListener.onLineStarted` (method) `android/java/main/java/ai/moonshine/voice/TranscriptEventListener.java:4`
- `TranscriptEventListener.onLineUpdated` (method) `android/java/main/java/ai/moonshine/voice/TranscriptEventListener.java:5`
- `TranscriptEventListener.onLineTextChanged` (method) `android/java/main/java/ai/moonshine/voice/TranscriptEventListener.java:6`
- `TranscriptEventListener.onLineSpeakersChanged` (method) `android/java/main/java/ai/moonshine/voice/TranscriptEventListener.java:7`
- `TranscriptEventListener.onLineCompleted` (method) `android/java/main/java/ai/moonshine/voice/TranscriptEventListener.java:8`
- `TranscriptEventListener.onError` (method) `android/java/main/java/ai/moonshine/voice/TranscriptEventListener.java:9`

## android/java/main/java/ai/moonshine/voice/TranscriptLine.java
Imported by: `android/java/androidTest/java/ai/moonshine/voice/JNITest.java`, `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java`, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java`
- `TranscriptLine.toString` (method) `android/java/main/java/ai/moonshine/voice/TranscriptLine.java:29`

## android/java/main/java/ai/moonshine/voice/TtsSynthesisResult.java
- `TtsSynthesisResult.TtsSynthesisResult` (method) `android/java/main/java/ai/moonshine/voice/TtsSynthesisResult.java:6`
- `TtsSynthesisResult.TtsSynthesisResult` (method) `android/java/main/java/ai/moonshine/voice/TtsSynthesisResult.java:8`

## android/java/main/java/ai/moonshine/voice/WordTiming.java
- `WordTiming.toString` (method) `android/java/main/java/ai/moonshine/voice/WordTiming.java:7`

## android/moonshine-jni/moonshine-jni.cpp
Depends on: `core/moonshine-c-api.h`
- `get_class` (function) `android/moonshine-jni/moonshine-jni.cpp:19` `static jclass get_class(JNIEnv *env, const char *className)`
- `get_field` (function) `android/moonshine-jni/moonshine-jni.cpp:27` `static jfieldID get_field(JNIEnv *env, jclass clazz, const char *fieldName,
                     ...`
- `get_method` (function) `android/moonshine-jni/moonshine-jni.cpp:36` `static jmethodID get_method(JNIEnv *env, jclass clazz, const char *methodName,
                  ...`
- `c_transcript_from_jobject` (function) `android/moonshine-jni/moonshine-jni.cpp:46` `static std::unique_ptr<transcript_t> c_transcript_from_jobject(
    JNIEnv *env, jobject javaTran...`
- `transcript` (function) `android/moonshine-jni/moonshine-jni.cpp:77` `std::unique_ptr<transcript_t> transcript(new transcript_t());`
- `c_transcript_to_jobject` (function) `android/moonshine-jni/moonshine-jni.cpp:112` `static jobject c_transcript_to_jobject(JNIEnv *env, struct transcript_t *transcript)`
- `fill_moonshine_options` (function) `android/moonshine-jni/moonshine-jni.cpp:265` `static bool fill_moonshine_options(
    JNIEnv *env, jobjectArray joptions, std::vector<moonshine...`
- `release_moonshine_options` (function) `android/moonshine-jni/moonshine-jni.cpp:300` `static void release_moonshine_options(
    JNIEnv *env, const std::vector<moonshine_option_t> &co...`
- `copy` (function) `android/moonshine-jni/moonshine-jni.cpp:673` `std::vector<uint8_t> copy(static_cast<size_t>(len));`

## core/benchmark.cpp
Depends on: `core/moonshine-cpp.h`, `core/moonshine-utils/file-utils.h`
- `AudioProducer` (function) `core/benchmark.cpp:13` `public:
  AudioProducer(std::string wav_path, float chunk_duration_seconds = 0.0214f)
      : cur...`
- `getNextAudio` (function) `core/benchmark.cpp:18` `bool getNextAudio(std::vector<float> &out_audio_data)`
- `sample_rate` (function) `core/benchmark.cpp:30` `int32_t sample_rate() const`
- `audio_data_size` (function) `core/benchmark.cpp:31` `size_t audio_data_size() const`
- `main` (function) `core/benchmark.cpp:43` `int main(int argc, char *argv[])`
- `loadWavData` (function) `core/benchmark.cpp:109` `void AudioProducer::loadWavData(std::string wav_path)`

## core/bin-tokenizer/bin-tokenizer.cpp
Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/moonshine-utils/debug-utils.h`, `core/moonshine-utils/file-utils.h`, `core/moonshine-utils/string-utils.h`
- `BinTokenizer` (function) `core/bin-tokenizer/bin-tokenizer.cpp:12` `BinTokenizer::BinTokenizer(const char *tokenizer_path,
                           const char *spa...`
- `bytes` (function) `core/bin-tokenizer/bin-tokenizer.cpp:39` `std::vector<uint8_t> bytes(byte_count);`
- `BinTokenizer` (function) `core/bin-tokenizer/bin-tokenizer.cpp:50` `BinTokenizer::BinTokenizer(const uint8_t *tokenizer_data,
                           size_t token...`
- `BinTokenizer` (function) `core/bin-tokenizer/bin-tokenizer.cpp:106` `BinTokenizer::BinTokenizer(const char *tokenizer_path,
                           AAssetManager *...` -- if defined(ANDROID)
- `text_to_special_token` (function) `core/bin-tokenizer/bin-tokenizer.cpp:148` `template <typename T>
T BinTokenizer::text_to_special_token(const std::string &text)`
- `text_to_tokens` (function) `core/bin-tokenizer/bin-tokenizer.cpp:173` `template <typename T>
std::vector<T> BinTokenizer::text_to_tokens(const std::string &text)`
- `remaining_bytes` (function) `core/bin-tokenizer/bin-tokenizer.cpp:176` `std::vector<uint8_t> remaining_bytes(replaced_spaces_text.begin(), replaced_spaces_text.end());`
- `tokens_to_text` (function) `core/bin-tokenizer/bin-tokenizer.cpp:222` `template <typename T>
std::string BinTokenizer::tokens_to_text(const std::vector<T> &tokens,
    ...`

## core/cosine-distance.cpp
Depends on: `core/cosine-distance.h`
- `cosine_distance` (function) `core/cosine-distance.cpp:6` `float cosine_distance(const std::vector<float>& a,
                      const std::vector<float>...`

## core/cosine-distance.h
Imported by: `core/cosine-distance-test.cpp`, `core/cosine-distance.cpp`
- `cosine_distance` (function) `core/cosine-distance.h:9` `float cosine_distance(const std::vector<float>& a, const std::vector<float>& b);` -- Computes cosine distance between two vectors: 1 - (a·b)/(||a||*||b||).

## core/cpp-annote/src/annotation_support.h
Imported by: `core/cpp-annote/src/cpp-annote.cpp`
- `empty` (function) `core/cpp-annote/src/annotation_support.h:28` `bool empty() const`
- `duration` (function) `core/cpp-annote/src/annotation_support.h:30` `double duration() const`
- `segment_union` (function) `core/cpp-annote/src/annotation_support.h:37` `inline Segment segment_union(const Segment& a, const Segment& b)` -- Union (|): covers both segments including any gap between them.
- `segment_gap` (function) `core/cpp-annote/src/annotation_support.h:49` `inline Segment segment_gap(const Segment& self_, const Segment& other)` -- Gap (^): self is first operand, other is second (matches Python `self ^ other`).
- `timeline_support_sorted` (function) `core/cpp-annote/src/annotation_support.h:60` `inline std::vector<Segment> timeline_support_sorted(
    const std::vector<Segment>& segments, do...` -- Timeline.support_iter / Timeline.support(collar) `segments` must be sorted by increasing start (Timeline order).
- `sort` (function) `core/cpp-annote/src/annotation_support.h:66` `std::sort(segs.begin(), segs.end(), [](const Segment& x, const Segment& y)`

## core/cpp-annote/src/clustering_vbx.cpp
Depends on: `core/cpp-annote/src/clustering_vbx.h`, `core/cpp-annote/src/filter_train.h`, `core/cpp-annote/src/hungarian.h`, `core/cpp-annote/src/parity_log.h`, `core/cpp-annote/src/scipy_linkage.h`
- `row_normalize` (function) `core/cpp-annote/src/clustering_vbx.cpp:22` `void row_normalize(Eigen::MatrixXd& M)`
- `cdist_cosine` (function) `core/cpp-annote/src/clustering_vbx.cpp:31` `void cdist_cosine(const Eigen::MatrixXd& X, const Eigen::MatrixXd& C,
                  Eigen::Ma...`
- `kmeans_fit_predict` (function) `core/cpp-annote/src/clustering_vbx.cpp:50` `std::vector<int> kmeans_fit_predict(const Eigen::MatrixXd& Xnorm, int k,
                        ...`
- `r` (function) `core/cpp-annote/src/clustering_vbx.cpp:55` `std::vector<int> r(static_cast<std::size_t>(n));`
- `uni` (function) `core/cpp-annote/src/clustering_vbx.cpp:60` `std::uniform_int_distribution<int> uni(0, n - 1);`
- `best_labs` (function) `core/cpp-annote/src/clustering_vbx.cpp:62` `std::vector<int> best_labs(static_cast<std::size_t>(n), 0);`
- `labels` (function) `core/cpp-annote/src/clustering_vbx.cpp:68` `std::vector<int> labels(static_cast<std::size_t>(n), 0);`
- `cnt` (function) `core/cpp-annote/src/clustering_vbx.cpp:87` `std::vector<int> cnt(static_cast<std::size_t>(k), 0);`
- `centroids_from_labels` (function) `core/cpp-annote/src/clustering_vbx.cpp:115` `Eigen::MatrixXd centroids_from_labels(const Eigen::MatrixXd& train,
                             ...`
- `hungarian_maximize` (function) `core/cpp-annote/src/clustering_vbx.cpp:133` `void hungarian_maximize(const Eigen::MatrixXd& score,
                        std::vector<int>& a...`
- `cost` (function) `core/cpp-annote/src/clustering_vbx.cpp:145` `std::vector<std::vector<double>> cost( static_cast<std::size_t>(m), std::vector<double>(static_cast<std::size_t>(m)...`
- `vbx_clustering_hard` (function) `core/cpp-annote/src/clustering_vbx.cpp:166` `void vbx_clustering_hard(const plda_vbx::PldaModel& plda,
                         const VbxClust...`
- `xflat` (function) `core/cpp-annote/src/clustering_vbx.cpp:192` `std::vector<double> xflat( static_cast<std::size_t>(train_n.rows() * train_n.cols()));`
- `fea_f` (function) `core/cpp-annote/src/clustering_vbx.cpp:357` `std::vector<float> fea_f(static_cast<size_t>(fea.rows() * fea.cols()));`

## core/cpp-annote/src/clustering_vbx.h
Depends on: `core/cpp-annote/src/plda_vbx.h`
Imported by: `core/cpp-annote/src/clustering_vbx.cpp`, `core/cpp-annote/src/cpp-annote-engine.h`, `core/cpp-annote/src/cpp-annote.cpp`
- `vbx_clustering_hard` (function) `core/cpp-annote/src/clustering_vbx.h:34` `void vbx_clustering_hard(const plda_vbx::PldaModel& plda, const VbxClusteringParams& pr, int num_chunks, int...` -- ``embeddings`` row-major ``(num_chunks * num_speakers * dim)``; ``binarized`` ``(num_chunks * num_frames *...

## core/cpp-annote/src/compute_fbank.cpp
Depends on: `core/cpp-annote/src/compute_fbank.h`
- `wespeaker_like_fbank` (function) `core/cpp-annote/src/compute_fbank.cpp:13` `void wespeaker_like_fbank(float sample_hz, int num_mel_bins,
                          float fram...`
- `scaled` (function) `core/cpp-annote/src/compute_fbank.cpp:31` `std::vector<float> scaled(static_cast<std::size_t>(std::max(0, num_samples)));`

## core/cpp-annote/src/compute_fbank.h
Imported by: `core/cpp-annote/src/compute_fbank.cpp`, `core/cpp-annote/src/cpp-annote.cpp`, `core/cpp-annote/src/embedding_ort_infer.cpp`
- `wespeaker_like_fbank` (function) `core/cpp-annote/src/compute_fbank.h:16` `void wespeaker_like_fbank(float sample_hz, int num_mel_bins, float frame_length_ms, float frame_shift_ms, const...` -- Mono waveform ``[-1,1]`` → log-fbank, shape ``(T * num_mel_bins)`` row-major.

## core/cpp-annote/src/cpp-annote-engine.h
Depends on: `core/cpp-annote/src/clustering_vbx.h`, `core/cpp-annote/src/cpp-annote.h`, `core/cpp-annote/src/plda_vbx.h`
Imported by: `core/cpp-annote/src/cpp-annote-streaming.h`, `core/cpp-annote/src/cpp-annote.cpp`, `core/speaker-diarizer.cpp`
- `print` (function) `core/cpp-annote/src/cpp-annote-engine.h:33` `void print(std::ostream& os, const char* prefix = "  ") const`
- `accumulate` (function) `core/cpp-annote/src/cpp-annote-engine.h:49` `void accumulate(const DiarizationProfile& o)`
- `extract_chunk_audio` (function) `core/cpp-annote/src/cpp-annote-engine.h:73` `static std::vector<float> extract_chunk_audio(const float* audio, int64_t num_samples, int64_t offset, int...`
- `run_segmentation_ort_single` (function) `core/cpp-annote/src/cpp-annote-engine.h:79` `std::vector<float> run_segmentation_ort_single(const float* chunk_buf);`
- `run_embedding_ort_single` (function) `core/cpp-annote/src/cpp-annote-engine.h:81` `std::vector<float> run_embedding_ort_single(const float* chunk_mono, const float* seg_binarized);`
- `segmentation_model_sample_rate` (function) `core/cpp-annote/src/cpp-annote-engine.h:89` `int segmentation_model_sample_rate() const`
- `segmentation_num_channels` (function) `core/cpp-annote/src/cpp-annote-engine.h:90` `int segmentation_num_channels() const`
- `segmentation_chunk_num_samples` (function) `core/cpp-annote/src/cpp-annote-engine.h:91` `int segmentation_chunk_num_samples() const`
- `segmentation_chunk_step_sec` (function) `core/cpp-annote/src/cpp-annote-engine.h:92` `double segmentation_chunk_step_sec() const`
- `segmentation_chunk_duration_sec` (function) `core/cpp-annote/src/cpp-annote-engine.h:93` `double segmentation_chunk_duration_sec() const`
- `seg_frames_per_chunk` (function) `core/cpp-annote/src/cpp-annote-engine.h:94` `int seg_frames_per_chunk() const`
- `seg_classes` (function) `core/cpp-annote/src/cpp-annote-engine.h:95` `int seg_classes() const`
- `embedding_dimension` (function) `core/cpp-annote/src/cpp-annote-engine.h:96` `int embedding_dimension() const`
- `init_config_and_models` (function) `core/cpp-annote/src/cpp-annote-engine.h:140` `void init_config_and_models(const std::string& embedding_onnx_path);`

## core/cpp-annote/src/cpp-annote-streaming.cpp
Depends on: `core/cpp-annote/src/cpp-annote-streaming.h`, `core/cpp-annote/src/wav_pcm_float32.h`
- `segment_iou` (function) `core/cpp-annote/src/cpp-annote-streaming.cpp:22` `double segment_iou(double a0, double a1, double b0, double b1)`
- `turns_match` (function) `core/cpp-annote/src/cpp-annote-streaming.cpp:31` `bool turns_match(const StreamingDiarizationTurn& a,
                 const StreamingDiarizationTu...`
- `StreamingDiarizationSession` (function) `core/cpp-annote/src/cpp-annote-streaming.cpp:40` `StreamingDiarizationSession::StreamingDiarizationSession(
    CppAnnoteEngine& engine, StreamingD...`
- `start_session` (function) `core/cpp-annote/src/cpp-annote-streaming.cpp:63` `void StreamingDiarizationSession::start_session()`
- `cluster_overlap_margin_sec` (function) `core/cpp-annote/src/cpp-annote-streaming.cpp:79` `double StreamingDiarizationSession::cluster_overlap_margin_sec() const`
- `cluster_decode_margin_sec` (function) `core/cpp-annote/src/cpp-annote-streaming.cpp:83` `double StreamingDiarizationSession::cluster_decode_margin_sec() const`
- `active_cluster_window_start_sec` (function) `core/cpp-annote/src/cpp-annote-streaming.cpp:93` `double StreamingDiarizationSession::active_cluster_window_start_sec() const`
- `cluster_decode_window_start_sec` (function) `core/cpp-annote/src/cpp-annote-streaming.cpp:100` `double StreamingDiarizationSession::cluster_decode_window_start_sec() const`
- `abs_sample_offset_for_sec` (function) `core/cpp-annote/src/cpp-annote-streaming.cpp:113` `int64_t StreamingDiarizationSession::abs_sample_offset_for_sec(double sec) const`
- `evict_chunk_cache_if_needed` (function) `core/cpp-annote/src/cpp-annote-streaming.cpp:121` `void StreamingDiarizationSession::evict_chunk_cache_if_needed()`
- `trim_buffer_if_needed` (function) `core/cpp-annote/src/cpp-annote-streaming.cpp:137` `void StreamingDiarizationSession::trim_buffer_if_needed()`
- `cache_new_chunks` (function) `core/cpp-annote/src/cpp-annote-streaming.cpp:168` `void StreamingDiarizationSession::cache_new_chunks()`
- `add_audio_chunk` (function) `core/cpp-annote/src/cpp-annote-streaming.cpp:200` `void StreamingDiarizationSession::add_audio_chunk(const float* pcm,
                             ...`
- `chunk` (function) `core/cpp-annote/src/cpp-annote-streaming.cpp:212` `std::vector<float> chunk(pcm, pcm + num_samples);`
- `carry_last_updated_times` (function) `core/cpp-annote/src/cpp-annote-streaming.cpp:226` `void StreamingDiarizationSession::carry_last_updated_times(
    std::vector<StreamingDiarizationT...`
- `append_frozen_turn_if_new` (function) `core/cpp-annote/src/cpp-annote-streaming.cpp:250` `void StreamingDiarizationSession::append_frozen_turn_if_new(
    std::vector<StreamingDiarization...`
- `relabel_active_turns` (function) `core/cpp-annote/src/cpp-annote-streaming.cpp:261` `void StreamingDiarizationSession::relabel_active_turns(
    std::vector<StreamingDiarizationTurn>...`
- `sort` (function) `core/cpp-annote/src/cpp-annote-streaming.cpp:314` `std::sort(candidates.begin(), candidates.end(),
              [](const auto& a, const auto& b)`
- `merge_frozen_and_active_turns` (function) `core/cpp-annote/src/cpp-annote-streaming.cpp:343` `void StreamingDiarizationSession::merge_frozen_and_active_turns(
    std::vector<StreamingDiariza...`
- `sort` (function) `core/cpp-annote/src/cpp-annote-streaming.cpp:381` `std::sort(merged.begin(), merged.end(),
            [](const StreamingDiarizationTurn& a,
       ...`
- `maybe_refresh` (function) `core/cpp-annote/src/cpp-annote-streaming.cpp:395` `void StreamingDiarizationSession::maybe_refresh(bool force)`
- `seg_out` (function) `core/cpp-annote/src/cpp-annote-streaming.cpp:486` `std::vector<float> seg_out(static_cast<size_t>(C_full) * static_cast<size_t>(FK));`
- `emb_all` (function) `core/cpp-annote/src/cpp-annote-streaming.cpp:488` `std::vector<float> emb_all(static_cast<size_t>(C_full) * static_cast<size_t>(K) * static_cast<size_t>(dim)...`
- `snapshot` (function) `core/cpp-annote/src/cpp-annote-streaming.cpp:549` `StreamingDiarizationSnapshot StreamingDiarizationSession::snapshot() const`
- `refresh_and_snapshot` (function) `core/cpp-annote/src/cpp-annote-streaming.cpp:554` `StreamingDiarizationSnapshot
StreamingDiarizationSession::refresh_and_snapshot()`
- `end_session` (function) `core/cpp-annote/src/cpp-annote-streaming.cpp:561` `StreamingDiarizationSnapshot StreamingDiarizationSession::end_session()`

## core/cpp-annote/src/cpp-annote-streaming.h
Depends on: `core/cpp-annote/src/cpp-annote-engine.h`
Imported by: `core/cpp-annote/src/cpp-annote-streaming.cpp`, `core/cpp-annote/src/cpp-annote.cpp`, `core/speaker-diarizer.cpp`
- `start_session` (function) `core/cpp-annote/src/cpp-annote-streaming.h:60` `void start_session();`
- `add_audio_chunk` (function) `core/cpp-annote/src/cpp-annote-streaming.h:63` `void add_audio_chunk(const float* pcm, std::size_t num_samples, int sample_rate);` -- Append ``num_samples`` mono ``pcm`` at ``sample_rate`` Hz; resamples each chunk to the engine model rate and...
- `cache_new_chunks` (function) `core/cpp-annote/src/cpp-annote-streaming.h:80` `private: void cache_new_chunks();`
- `trim_buffer_if_needed` (function) `core/cpp-annote/src/cpp-annote-streaming.h:81` `void trim_buffer_if_needed();`
- `evict_chunk_cache_if_needed` (function) `core/cpp-annote/src/cpp-annote-streaming.h:82` `void evict_chunk_cache_if_needed();`
- `maybe_refresh` (function) `core/cpp-annote/src/cpp-annote-streaming.h:83` `void maybe_refresh(bool force);`
- `carry_last_updated_times` (function) `core/cpp-annote/src/cpp-annote-streaming.h:84` `static void carry_last_updated_times( std::vector<StreamingDiarizationTurn>& next, const...`
- `append_frozen_turn_if_new` (function) `core/cpp-annote/src/cpp-annote-streaming.h:87` `static void append_frozen_turn_if_new( std::vector<StreamingDiarizationTurn>& frozen, const...`
- `merge_frozen_and_active_turns` (function) `core/cpp-annote/src/cpp-annote-streaming.h:90` `void merge_frozen_and_active_turns( std::vector<StreamingDiarizationTurn> active_turns);`
- `relabel_active_turns` (function) `core/cpp-annote/src/cpp-annote-streaming.h:95` `void relabel_active_turns(std::vector<StreamingDiarizationTurn>& active_turns);` -- Relabels the raw per-window clustering labels of `active_turns` into a persistent namespace that is stable across...
- `cluster_overlap_margin_sec` (function) `core/cpp-annote/src/cpp-annote-streaming.h:96` `double cluster_overlap_margin_sec() const;`
- `cluster_decode_margin_sec` (function) `core/cpp-annote/src/cpp-annote-streaming.h:97` `double cluster_decode_margin_sec() const;`
- `active_cluster_window_start_sec` (function) `core/cpp-annote/src/cpp-annote-streaming.h:98` `double active_cluster_window_start_sec() const;`
- `cluster_decode_window_start_sec` (function) `core/cpp-annote/src/cpp-annote-streaming.h:99` `double cluster_decode_window_start_sec() const;`
- `abs_sample_offset_for_sec` (function) `core/cpp-annote/src/cpp-annote-streaming.h:100` `int64_t abs_sample_offset_for_sec(double sec) const;`

## core/cpp-annote/src/cpp-annote.cpp
Depends on: `core/cpp-annote/src/annotation_support.h`, `core/cpp-annote/src/clustering_vbx.h`, `core/cpp-annote/src/community1_cpp_annote_embedded.h`, `core/cpp-annote/src/community1_ort_embedded.h`, `core/cpp-annote/src/compute_fbank.h`, `core/cpp-annote/src/cpp-annote-engine.h`, `core/cpp-annote/src/cpp-annote-streaming.h`, `core/cpp-annote/src/cpp-annote.h`, `core/cpp-annote/src/embedding_ort_infer.h`, `core/cpp-annote/src/parity_log.h`, `core/cpp-annote/src/plda_vbx.h`, `core/cpp-annote/src/wav_pcm_float32.h`
- `json_double` (function) `core/cpp-annote/src/cpp-annote.cpp:40` `double json_double(const std::string &json, const char *key)`
- `json_bool` (function) `core/cpp-annote/src/cpp-annote.cpp:50` `bool json_bool(const std::string &json, const char *key)`
- `closest_frame` (function) `core/cpp-annote/src/cpp-annote.cpp:60` `int closest_frame(double t, double sw_start, double sw_duration,
                  double sw_step)`
- `trim_warmup_inplace` (function) `core/cpp-annote/src/cpp-annote.cpp:66` `void trim_warmup_inplace(std::vector<float> &data, size_t num_chunks,
                         si...`
- `out` (function) `core/cpp-annote/src/cpp-annote.cpp:78` `std::vector<float> out(num_chunks * new_frames * num_classes);`
- `inference_aggregate` (function) `core/cpp-annote/src/cpp-annote.cpp:93` `void inference_aggregate(const std::vector<float> &scores, size_t num_chunks,
                   ...`
- `agg` (function) `core/cpp-annote/src/cpp-annote.cpp:113` `std::vector<float> agg(static_cast<size_t>(num_out_frames) * num_classes, 0.f);`
- `occ` (function) `core/cpp-annote/src/cpp-annote.cpp:115` `std::vector<float> occ(static_cast<size_t>(num_out_frames) * num_classes, 0.f);`
- `mask_max` (function) `core/cpp-annote/src/cpp-annote.cpp:117` `std::vector<float> mask_max(static_cast<size_t>(num_out_frames) * num_classes, 0.f);`
- `speaker_count_initial_uint8` (function) `core/cpp-annote/src/cpp-annote.cpp:166` `std::vector<std::uint8_t> speaker_count_initial_uint8(
    std::vector<float> binarized, size_t n...`
- `summed` (function) `core/cpp-annote/src/cpp-annote.cpp:174` `std::vector<float> summed(num_chunks * nf * 1);`
- `cap_count` (function) `core/cpp-annote/src/cpp-annote.cpp:198` `std::vector<std::int8_t> cap_count(const std::vector<std::uint8_t> &u8,
                         ...`
- `crop_loose_frame_range` (function) `core/cpp-annote/src/cpp-annote.cpp:208` `void crop_loose_frame_range(double focus_start, double focus_end,
                            dou...`
- `extent_of_frames` (function) `core/cpp-annote/src/cpp-annote.cpp:219` `void extent_of_frames(double sw_start, double sw_step, size_t n_rows,
                      doubl...`
- `crop_feature_loose` (function) `core/cpp-annote/src/cpp-annote.cpp:225` `void crop_feature_loose(const std::vector<float> &data, int n_samples,
                        in...`
- `argsort_desc_stable` (function) `core/cpp-annote/src/cpp-annote.cpp:256` `std::vector<int> argsort_desc_stable(const float *row, int k)`
- `idx` (function) `core/cpp-annote/src/cpp-annote.cpp:257` `std::vector<int> idx(static_cast<size_t>(k));`
- `stable_sort` (function) `core/cpp-annote/src/cpp-annote.cpp:259` `std::stable_sort(idx.begin(), idx.end(), [row](int a, int b)`
- `reconstruct_to_diarization` (function) `core/cpp-annote/src/cpp-annote.cpp:268` `std::vector<float> reconstruct_to_diarization(
    const std::vector<float> &segmentations, int C...`
- `clustered` (function) `core/cpp-annote/src/cpp-annote.cpp:283` `std::vector<float> clustered(static_cast<size_t>(C) * static_cast<size_t>(F) * static_cast<size_t>(num_clusters)...`
- `seen_k` (function) `core/cpp-annote/src/cpp-annote.cpp:291` `std::vector<char> seen_k(static_cast<size_t>(num_clusters), 0);`
- `padded` (function) `core/cpp-annote/src/cpp-annote.cpp:345` `std::vector<float> padded( static_cast<size_t>(T) * static_cast<size_t>(max_spf), 0.f);`
- `cnt_2d` (function) `core/cpp-annote/src/cpp-annote.cpp:370` `std::vector<float> cnt_2d(static_cast<size_t>(Tcnt));`
- `binary` (function) `core/cpp-annote/src/cpp-annote.cpp:383` `std::vector<float> binary( static_cast<size_t>(act_rows) * static_cast<size_t>(K), 0.f);`
- `binarize_column` (function) `core/cpp-annote/src/cpp-annote.cpp:401` `void binarize_column(const float *k_scores, int num_frames, double sw_start,
                    ...`
- `ts` (function) `core/cpp-annote/src/cpp-annote.cpp:408` `std::vector<double> ts(static_cast<size_t>(num_frames));`
- `try_regex_double` (function) `core/cpp-annote/src/cpp-annote.cpp:437` `bool try_regex_double(const std::string &json, const std::string &key_esc,
                      ...`
- `filter_min_duration_on` (function) `core/cpp-annote/src/cpp-annote.cpp:449` `void filter_min_duration_on(std::vector<std::pair<double, double>> &regs,
                       ...`
- `try_json_bool_field` (function) `core/cpp-annote/src/cpp-annote.cpp:463` `bool try_json_bool_field(const std::string &json, const char *key_esc,
                         b...`
- `try_regex_int` (function) `core/cpp-annote/src/cpp-annote.cpp:476` `bool try_regex_int(const std::string &json, const std::string &key_esc,
                   int &out)`
- `make_segmentation_session` (function) `core/cpp-annote/src/cpp-annote.cpp:490` `Ort::Session make_segmentation_session(Ort::Env &env,
                                       Ort:...`
- `make_embedding_session` (function) `core/cpp-annote/src/cpp-annote.cpp:504` `std::unique_ptr<Ort::Session> make_embedding_session(
    Ort::Env &env, Ort::SessionOptions &opt...`
- `init_config_and_models` (function) `core/cpp-annote/src/cpp-annote.cpp:515` `void CppAnnoteEngine::init_config_and_models(
    const std::string &embedding_onnx_path)`
- `seg_json` (function) `core/cpp-annote/src/cpp-annote.cpp:517` `const std::string seg_json( cppannote::embedded_community1::segmentation_json...`
- `rf_txt` (function) `core/cpp-annote/src/cpp-annote.cpp:536` `const std::string rf_txt( cppannote::embedded_community1::receptive_field_json...`
- `sj` (function) `core/cpp-annote/src/cpp-annote.cpp:543` `const std::string sj( cppannote::embedded_community1::pipeline_snapshot_json...`
- `emb_json` (function) `core/cpp-annote/src/cpp-annote.cpp:566` `const std::string emb_json( cppannote::embedded_community1::embedding_json...`
- `in_name_` (function) `core/cpp-annote/src/cpp-annote.cpp:611` `in_name_(session_.GetInputNameAllocated(0, alloc_)),
      out_name_(session_.GetOutputNameAlloca...`
- `in_name_` (function) `core/cpp-annote/src/cpp-annote.cpp:624` `in_name_(session_.GetInputNameAllocated(0, alloc_)),
      out_name_(session_.GetOutputNameAlloca...`
- `extract_chunk_audio` (function) `core/cpp-annote/src/cpp-annote.cpp:633` `std::vector<float> CppAnnoteEngine::extract_chunk_audio(const float *audio,
                     ...`
- `buf` (function) `core/cpp-annote/src/cpp-annote.cpp:638` `std::vector<float> buf(static_cast<size_t>(num_channels) * static_cast<size_t>(chunk_num_samples), 0.f);`
- `run_segmentation_ort_single` (function) `core/cpp-annote/src/cpp-annote.cpp:653` `std::vector<float> CppAnnoteEngine::run_segmentation_ort_single(
    const float *chunk_buf)`
- `run_embedding_ort_single` (function) `core/cpp-annote/src/cpp-annote.cpp:682` `std::vector<float> CppAnnoteEngine::run_embedding_ort_single(
    const float *chunk_mono, const ...`
- `chunk_for_fbank` (function) `core/cpp-annote/src/cpp-annote.cpp:694` `std::vector<float> chunk_for_fbank(chunk_mono, chunk_mono + chunk_num_samples);`
- `result` (function) `core/cpp-annote/src/cpp-annote.cpp:722` `std::vector<float> result(static_cast<size_t>(K) * static_cast<size_t>(dim));`
- `clean_col` (function) `core/cpp-annote/src/cpp-annote.cpp:724` `std::vector<float> clean_col(static_cast<size_t>(F), 0.f);`
- `full_col` (function) `core/cpp-annote/src/cpp-annote.cpp:725` `std::vector<float> full_col(static_cast<size_t>(F), 0.f);`
- `cluster_and_decode` (function) `core/cpp-annote/src/cpp-annote.cpp:753` `std::vector<DiarizationTurn> CppAnnoteEngine::cluster_and_decode(
    const std::vector<float> &s...`
- `col` (function) `core/cpp-annote/src/cpp-annote.cpp:859` `std::vector<float> col(static_cast<size_t>(rows));`
- `sort` (function) `core/cpp-annote/src/cpp-annote.cpp:893` `std::sort(turns.begin(), turns.end(),
            [](const DiarizationTurn &a, const DiarizationT...`
- `write_json` (function) `core/cpp-annote/src/cpp-annote.cpp:915` `void DiarizationResults::write_json(std::ostream &os) const`
- `write_json` (function) `core/cpp-annote/src/cpp-annote.cpp:931` `void DiarizationResults::write_json(const std::string &path) const`
- `Impl` (function) `core/cpp-annote/src/cpp-annote.cpp:950` `Impl() : engine()`
- `Impl` (function) `core/cpp-annote/src/cpp-annote.cpp:951` `Impl(const std::string& seg_path, const std::string& emb_path)
      : engine(seg_path, emb_path)`
- `get_stream` (function) `core/cpp-annote/src/cpp-annote.cpp:954` `StreamingDiarizationSession &get_stream(int32_t id)`
- `to_results` (function) `core/cpp-annote/src/cpp-annote.cpp:963` `static DiarizationResults to_results(
      const StreamingDiarizationSnapshot &snap)`
- `CppAnnote` (function) `core/cpp-annote/src/cpp-annote.cpp:974` `CppAnnote::CppAnnote() : impl_(std::make_unique<Impl>())`
- `CppAnnote` (function) `core/cpp-annote/src/cpp-annote.cpp:976` `CppAnnote::CppAnnote(const std::string& segmentation_onnx_path,
                      const std::...`
- `create_stream` (function) `core/cpp-annote/src/cpp-annote.cpp:985` `int32_t CppAnnote::create_stream(double cluster_cadence,
                                 double ...`
- `free_stream` (function) `core/cpp-annote/src/cpp-annote.cpp:997` `void CppAnnote::free_stream(int32_t stream_id)`
- `start_stream` (function) `core/cpp-annote/src/cpp-annote.cpp:1002` `void CppAnnote::start_stream(int32_t stream_id)`
- `stop_stream` (function) `core/cpp-annote/src/cpp-annote.cpp:1006` `DiarizationResults CppAnnote::stop_stream(int32_t stream_id)`
- `add_audio_to_stream` (function) `core/cpp-annote/src/cpp-annote.cpp:1011` `void CppAnnote::add_audio_to_stream(int32_t stream_id, const float *audio_data,
                 ...`
- `diarize` (function) `core/cpp-annote/src/cpp-annote.cpp:1019` `DiarizationResults CppAnnote::diarize(const float *audio_data,
                                  ...`
- `diarize_stream` (function) `core/cpp-annote/src/cpp-annote.cpp:1033` `DiarizationResults CppAnnote::diarize_stream(int32_t stream_id)`

## core/cpp-annote/src/cpp-annote.h
Imported by: `core/cpp-annote/src/cpp-annote-engine.h`, `core/cpp-annote/src/cpp-annote.cpp`
- `write_json` (function) `core/cpp-annote/src/cpp-annote.h:25` `void write_json(const std::string &path) const;`
- `create_stream` (function) `core/cpp-annote/src/cpp-annote.h:58` `int32_t create_stream(double cluster_cadence = 2.0, double analyze_cadence = 0.0);` -- Allocate a new streaming diarization session and return its handle.
- `free_stream` (function) `core/cpp-annote/src/cpp-annote.h:62` `void free_stream(int32_t stream_id);` -- Release a stream and all associated resources.
- `start_stream` (function) `core/cpp-annote/src/cpp-annote.h:65` `void start_stream(int32_t stream_id);` -- Initialize a stream, clearing any buffered audio and cached results.
- `add_audio_to_stream` (function) `core/cpp-annote/src/cpp-annote.h:73` `void add_audio_to_stream(int32_t stream_id, const float *audio_data, uint64_t audio_length, int32_t sample_rate);` -- Append PCM audio to a stream.


Next: [API_p2.md](API_p2.md)
