# android/java/main/java/ai/moonshine/voice

*Community 11 | 12 files | cohesion 1.00*

## Definition

This community groups 12 file(s) rooted at `android/java/main/java/ai/moonshine/voice` with dominant language java (cohesion 1.00). Central symbols: `Error`, `JNI`, `JNITest`, `LineCompleted`, `LineSpeakersChanged`, `LineStarted`, `LineTextChanged`, `LineUpdated`. Core file: `android/java/main/java/ai/moonshine/voice/Transcriber.java` (29 symbols).

## Files

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `android/java/androidTest/java/ai/moonshine/voice/JNITest.java` | java | testing | 9 | no |
| `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java` | java | testing | 13 | no |
| `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java` | java | testing | 14 | no |
| `android/java/main/java/ai/moonshine/voice/JNI.java` | java | utility | 2 | no |
| `android/java/main/java/ai/moonshine/voice/ModelSpec.java` | java | business_logic | 8 | no |
| `android/java/main/java/ai/moonshine/voice/Transcriber.java` | java | utility | 29 | no |
| `android/java/main/java/ai/moonshine/voice/TranscriberOption.java` | java | utility | 4 | no |
| `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java` | java | infrastructure | 20 | no |
| `android/java/main/java/ai/moonshine/voice/TranscriptLine.java` | java | utility | 2 | no |
| `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/MainActivity.kt` | kt | utility | 1 | no |
| `examples/android/TextToSpeech/app/src/main/java/ai/moonshine/examples/texttospeech/MainActivity.kt` | kt | utility | 1 | no |
| `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java` | java | utility | 6 | no |

## Key Symbols

- `JNITest` (class, `android/java/androidTest/java/ai/moonshine/voice/JNITest.java:28`)
- `setUp` (method, `android/java/androidTest/java/ai/moonshine/voice/JNITest.java:32`)
- `testMoonshineGetVersion` (method, `android/java/androidTest/java/ai/moonshine/voice/JNITest.java:43`)
- `testMoonshineGetG2pDependencies` (method, `android/java/androidTest/java/ai/moonshine/voice/JNITest.java:48`)
- `testMoonshineErrorToString` (method, `android/java/androidTest/java/ai/moonshine/voice/JNITest.java:55`)
- `testMoonshineTranscriptToString` (method, `android/java/androidTest/java/ai/moonshine/voice/JNITest.java:60`)
- `testMoonshineLoadTranscriber` (method, `android/java/androidTest/java/ai/moonshine/voice/JNITest.java:81`)
- `testMoonshineTranscribe` (method, `android/java/androidTest/java/ai/moonshine/voice/JNITest.java:112`)
- `testMoonshineStreaming` (method, `android/java/androidTest/java/ai/moonshine/voice/JNITest.java:148`)
- `NoTranscriptionTest` (class, `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java:29`)
- `setUp` (method, `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java:37`)
- `testMoonshineNoTranscription` (method, `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java:47`)
- `TranscriptEventListener` (method, `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java:70`)
- `onLineStarted` (method, `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java:71`)
- `onLineUpdated` (method, `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java:76`)
- `onLineTextChanged` (method, `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java:81`)
- `onLineCompleted` (method, `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java:86`)
- `onError` (method, `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java:91`)
- `onLineStartedEvent` (method, `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java:111`)
- `onLineUpdatedEvent` (method, `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java:120`)
- `onLineTextChangedEvent` (method, `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java:128`)
- `onLineCompletedEvent` (method, `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java:134`)
- `TranscriberTest` (class, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java:33`)
- `setUp` (method, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java:43`)
- `testMoonshineTranscriberStreaming` (method, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java:53`)
- `TranscriptEventListener` (method, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java:82`)
- `onLineStarted` (method, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java:83`)
- `onLineUpdated` (method, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java:88`)
- `onLineTextChanged` (method, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java:93`)
- `onLineCompleted` (method, `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java:98`)

## Internal vs External Edges

- Internal resolved imports (EXTRACTED): 17
- Cross-boundary resolved imports (EXTRACTED): 0

## Connections

- [INFERRED] shares_context community 0 <-> 11 (strength 0.5): Inferred shared context (layer utility) with no import path between community 0 (core: moonshine-cpp) and community 11 (android/java/main/java/ai/moonshine/voice).

## Risks

- [taint medium] `android/java/androidTest/java/ai/moonshine/voice/JNITest.java` -> `android/java/androidTest/java/ai/moonshine/voice/JNITest.java` via `input` (0 hops)
- [taint medium] `android/java/androidTest/java/ai/moonshine/voice/JNITest.java` -> `android/java/main/java/ai/moonshine/voice/TranscriptLine.java` via `input` (1 hops)
- [taint medium] `android/java/androidTest/java/ai/moonshine/voice/JNITest.java` -> `android/java/main/java/ai/moonshine/voice/JNI.java` via `input` (1 hops)
- [taint medium] `android/java/main/java/ai/moonshine/voice/Transcriber.java` -> `android/java/main/java/ai/moonshine/voice/Transcriber.java` via `input` (0 hops)
- [taint medium] `android/java/main/java/ai/moonshine/voice/Transcriber.java` -> `android/java/main/java/ai/moonshine/voice/TranscriberOption.java` via `input` (1 hops)
- [taint medium] `android/java/main/java/ai/moonshine/voice/Transcriber.java` -> `android/java/main/java/ai/moonshine/voice/JNI.java` via `input` (1 hops)
- [taint critical] `android/java/main/java/ai/moonshine/voice/Transcriber.java` -> `android/java/main/java/ai/moonshine/voice/Transcriber.java` via `exec` (0 hops)
- [taint critical] `android/java/main/java/ai/moonshine/voice/Transcriber.java` -> `android/java/main/java/ai/moonshine/voice/TranscriberOption.java` via `exec` (1 hops)
- [taint critical] `android/java/main/java/ai/moonshine/voice/Transcriber.java` -> `android/java/main/java/ai/moonshine/voice/JNI.java` via `exec` (1 hops)
- [taint critical] `android/java/main/java/ai/moonshine/voice/Transcriber.java` -> `android/java/main/java/ai/moonshine/voice/Transcriber.java` via `exec` (0 hops)
- [taint critical] `android/java/main/java/ai/moonshine/voice/Transcriber.java` -> `android/java/main/java/ai/moonshine/voice/TranscriberOption.java` via `exec` (1 hops)
- [taint critical] `android/java/main/java/ai/moonshine/voice/Transcriber.java` -> `android/java/main/java/ai/moonshine/voice/JNI.java` via `exec` (1 hops)
- [taint critical] `android/java/main/java/ai/moonshine/voice/Transcriber.java` -> `android/java/main/java/ai/moonshine/voice/Transcriber.java` via `exec` (0 hops)
- [taint critical] `android/java/main/java/ai/moonshine/voice/Transcriber.java` -> `android/java/main/java/ai/moonshine/voice/TranscriberOption.java` via `exec` (1 hops)
- [taint critical] `android/java/main/java/ai/moonshine/voice/Transcriber.java` -> `android/java/main/java/ai/moonshine/voice/JNI.java` via `exec` (1 hops)

## Open Questions

- Why do 12 file(s) lack file-level docs (e.g. `android/java/androidTest/java/ai/moonshine/voice/JNITest.java`)? What purpose do they serve?
- Is the dangerous import `input` in `android/java/androidTest/java/ai/moonshine/voice/JNITest.java` still required, or can it be isolated?
- What would break if the most connected file in android/java/main/java/ai/moonshine/voice changed?
- Should android/java/main/java/ai/moonshine/voice be split, given cohesion 1.00?

## Sources

- `android/java/androidTest/java/ai/moonshine/voice/JNITest.java`
- `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java`
- `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java`
- `android/java/main/java/ai/moonshine/voice/JNI.java`
- `android/java/main/java/ai/moonshine/voice/ModelSpec.java`
- `android/java/main/java/ai/moonshine/voice/Transcriber.java`
- `android/java/main/java/ai/moonshine/voice/TranscriberOption.java`
- `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`
- `android/java/main/java/ai/moonshine/voice/TranscriptLine.java`
- `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/MainActivity.kt`
- `examples/android/TextToSpeech/app/src/main/java/ai/moonshine/examples/texttospeech/MainActivity.kt`
- `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java`
