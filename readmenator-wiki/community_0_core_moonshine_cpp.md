# core: moonshine-cpp

*Community 0 | 72 files | cohesion 0.88*

## Definition

This community groups 72 file(s) rooted at `core` with dominant language cpp (cohesion 0.88). Central symbols: `0`, `AudioProducer`, `BIN_TOKENIZER_H`, `BenchResult`, `BinTokenizer`, `CHECK_DTYPE`, `CHECK_GRAPHEME_PHONEMIZER_HANDLE`, `CHECK_INTENT_RECOGNIZER_HANDLE`. Core file: `core/moonshine-cpp.h` (127 symbols). Documented purpose: Path to the Gemma embedding model.

## Files

### `core` (42 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `core/benchmark.cpp` | cpp | utility | 7 | no |
| `core/embedding-model.h` | h | business_logic | 6 | no |
| `core/gemma-embedding-model-test.cpp` | cpp | business_logic | 14 | no |
| `core/gemma-embedding-model.cpp` | cpp | business_logic | 20 | no |

### `core/ort-utils` (11 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `core/ort-utils/moonshine-ort-allocator.cpp` | cpp | utility | 10 | no |
| `core/ort-utils/moonshine-ort-allocator.h` | h | utility | 3 | no |
| `core/ort-utils/moonshine-tensor-view.cpp` | cpp | presentation | 24 | no |
| `core/ort-utils/moonshine-tensor-view.h` | h | presentation | 21 | no |

### `core/moonshine-utils` (10 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `core/moonshine-utils/debug-utils-test.cpp` | cpp | testing | 21 | no |
| `core/moonshine-utils/debug-utils.cpp` | cpp | utility | 8 | no |
| `core/moonshine-utils/debug-utils.h` | h | utility | 52 | no |
| `core/moonshine-utils/file-utils-test.cpp` | cpp | testing | 12 | no |

### `core/reliability` (4 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `core/reliability/fuzz-bin-tokenizer.cpp` | cpp | utility | 1 | yes |
| `core/reliability/fuzz-resampler.cpp` | cpp | utility | 3 | yes |
| `core/reliability/fuzz-string-utils.cpp` | cpp | utility | 1 | yes |

### `core/bin-tokenizer` (3 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `core/bin-tokenizer/bin-tokenizer-test.cpp` | cpp | testing | 4 | no |
| `core/bin-tokenizer/bin-tokenizer.cpp` | cpp | utility | 8 | no |
| `core/bin-tokenizer/bin-tokenizer.h` | h | utility | 2 | no |

### `android/moonshine-jni` (1 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `android/moonshine-jni/moonshine-jni.cpp` | cpp | utility | 29 | no |

### `examples/windows/cli-transcriber` (1 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `examples/windows/cli-transcriber/cli-transcriber.cpp` | cpp | utility | 23 | yes |

*... and 52 more files in this community.*


## Key Symbols

- `LOG_TAG` (macro, `android/moonshine-jni/moonshine-jni.cpp:13`) `#define LOG_TAG`
- `get_class` (function, `android/moonshine-jni/moonshine-jni.cpp:19`) `static jclass get_class(JNIEnv *env, const char *className)`
- `get_field` (function, `android/moonshine-jni/moonshine-jni.cpp:27`) `static jfieldID get_field(JNIEnv *env, jclass clazz, const char *fieldName,`
- `get_method` (function, `android/moonshine-jni/moonshine-jni.cpp:36`) `static jmethodID get_method(JNIEnv *env, jclass clazz, const char *methodName,`
- `c_transcript_from_jobject` (function, `android/moonshine-jni/moonshine-jni.cpp:46`) `static std::unique_ptr<transcript_t> c_transcript_from_jobject(     JNIEnv *env,`
- `transcript` (function, `android/moonshine-jni/moonshine-jni.cpp:77`) `std::unique_ptr<transcript_t> transcript(new transcript_t());`
- `c_transcript_to_jobject` (function, `android/moonshine-jni/moonshine-jni.cpp:112`) `static jobject c_transcript_to_jobject(JNIEnv *env, struct transcript_t *transcr`
- `fill_moonshine_options` (function, `android/moonshine-jni/moonshine-jni.cpp:265`) `static bool fill_moonshine_options(     JNIEnv *env, jobjectArray joptions, std:`
- `release_moonshine_options` (function, `android/moonshine-jni/moonshine-jni.cpp:300`) `static void release_moonshine_options(     JNIEnv *env, const std::vector<moonsh`
- `MOONSHINE_ERROR_INVALID_ARGUMENT` (variable, `android/moonshine-jni/moonshine-jni.cpp:514`) `extern "C" JNIEXPORT int JNICALL Java_ai_moonshine_voice_JNI_moonshineAddAudioTo`
- `nullptr` (variable, `android/moonshine-jni/moonshine-jni.cpp:533`) `extern "C" JNIEXPORT jobject JNICALL Java_ai_moonshine_voice_JNI_moonshineTransc`
- `copts` (variable, `android/moonshine-jni/moonshine-jni.cpp:557`) `extern "C" JNIEXPORT jint JNICALL Java_ai_moonshine_voice_JNI_moonshineCreateTts`
- `copts` (variable, `android/moonshine-jni/moonshine-jni.cpp:610`) `extern "C" JNIEXPORT jint JNICALL Java_ai_moonshine_voice_JNI_moonshineCreateTts`
- `copy` (function, `android/moonshine-jni/moonshine-jni.cpp:673`) `std::vector<uint8_t> copy(static_cast<size_t>(len));`
- `copts` (variable, `android/moonshine-jni/moonshine-jni.cpp:712`) `extern "C" JNIEXPORT jstring JNICALL Java_ai_moonshine_voice_JNI_moonshineGetG2p`
- `copts` (variable, `android/moonshine-jni/moonshine-jni.cpp:752`) `extern "C" JNIEXPORT jstring JNICALL Java_ai_moonshine_voice_JNI_moonshineGetTts`
- `copts` (variable, `android/moonshine-jni/moonshine-jni.cpp:792`) `extern "C" JNIEXPORT jstring JNICALL Java_ai_moonshine_voice_JNI_moonshineGetStt`
- `copts` (variable, `android/moonshine-jni/moonshine-jni.cpp:832`) `extern "C" JNIEXPORT jstring JNICALL Java_ai_moonshine_voice_JNI_moonshineGetInt`
- `copts` (variable, `android/moonshine-jni/moonshine-jni.cpp:872`) `extern "C" JNIEXPORT jstring JNICALL Java_ai_moonshine_voice_JNI_moonshineGetTts`
- `copts` (variable, `android/moonshine-jni/moonshine-jni.cpp:911`) `extern "C" JNIEXPORT jobject JNICALL Java_ai_moonshine_voice_JNI_moonshineTextTo`
- `copts` (variable, `android/moonshine-jni/moonshine-jni.cpp:961`) `extern "C" JNIEXPORT jobject JNICALL Java_ai_moonshine_voice_JNI_moonshinePhonem`
- `copts` (variable, `android/moonshine-jni/moonshine-jni.cpp:1011`) `extern "C" JNIEXPORT jint JNICALL Java_ai_moonshine_voice_JNI_moonshineCreateGra`
- `copts` (variable, `android/moonshine-jni/moonshine-jni.cpp:1064`) `extern "C" JNIEXPORT jint JNICALL Java_ai_moonshine_voice_JNI_moonshineCreateGra`
- `copts` (variable, `android/moonshine-jni/moonshine-jni.cpp:1165`) `extern "C" JNIEXPORT jstring JNICALL Java_ai_moonshine_voice_JNI_moonshineTextTo`
- `MOONSHINE_ERROR_INVALID_ARGUMENT` (variable, `android/moonshine-jni/moonshine-jni.cpp:1205`) `extern "C" JNIEXPORT jint JNICALL Java_ai_moonshine_voice_JNI_moonshineCreateInt`
- `MOONSHINE_ERROR_INVALID_ARGUMENT` (variable, `android/moonshine-jni/moonshine-jni.cpp:1238`) `extern "C" JNIEXPORT jint JNICALL Java_ai_moonshine_voice_JNI_moonshineRegisterI`
- `MOONSHINE_ERROR_INVALID_ARGUMENT` (variable, `android/moonshine-jni/moonshine-jni.cpp:1268`) `extern "C" JNIEXPORT jint JNICALL Java_ai_moonshine_voice_JNI_moonshineUnregiste`
- `nullptr` (variable, `android/moonshine-jni/moonshine-jni.cpp:1286`) `extern "C" JNIEXPORT jobjectArray JNICALL Java_ai_moonshine_voice_JNI_moonshineG`
- `nullptr` (variable, `android/moonshine-jni/moonshine-jni.cpp:1355`) `extern "C" JNIEXPORT jfloatArray JNICALL Java_ai_moonshine_voice_JNI_moonshineCa`
- `AudioProducer` (class, `core/benchmark.cpp:11`)

## Internal vs External Edges

- Internal resolved imports (EXTRACTED): 125
- Cross-boundary resolved imports (EXTRACTED): 17

## Connections

- [EXTRACTED] depends_on community 0 <-> 4 (strength 0.9): Extracted import edge crosses communities: core/moonshine-c-api.cpp imports core/moonshine-tts/src/moonshine-asset-catalog.h.
- [EXTRACTED] depends_on community 0 <-> 3 (strength 0.9): Extracted import edge crosses communities: core/moonshine-c-api.cpp imports core/moonshine-tts/src/moonshine-g2p.h.
- [EXTRACTED] depends_on community 2 <-> 0 (strength 0.9): Extracted import edge crosses communities: core/moonshine-tts/src/lang-specific/korean.cpp imports core/moonshine-utils/debug-utils.h.
- [EXTRACTED] depends_on community 5 <-> 0 (strength 0.9): Extracted import edge crosses communities: core/reliability/fuzz-wav-pcm.cpp imports core/moonshine-utils/debug-utils.h.
- [INFERRED] shares_context community 0 <-> 1 (strength 0.5): Inferred shared context (layer utility) with no import path between community 0 (core: moonshine-cpp) and community 1 (micro/examples/rp2350/src: pack_format).
- [INFERRED] shares_context community 0 <-> 6 (strength 0.5): Inferred shared context (layer utility) with no import path between community 0 (core: moonshine-cpp) and community 6 (micro/g2p/src).
- [INFERRED] shares_context community 0 <-> 7 (strength 0.5): Inferred shared context (language cpp) with no import path between community 0 (core: moonshine-cpp) and community 7 (core/moonshine-tts/src/lang-specific: english-hand-oov).
- [INFERRED] shares_context community 0 <-> 8 (strength 0.5): Inferred shared context (layer utility) with no import path between community 0 (core: moonshine-cpp) and community 8 (python/src/moonshine_voice: dialog_flow).
- [INFERRED] shares_context community 0 <-> 9 (strength 0.5): Inferred shared context (layer utility) with no import path between community 0 (core: moonshine-cpp) and community 9 (micro/examples/rp2350/src: worldlite_synth).
- [INFERRED] shares_context community 0 <-> 10 (strength 0.5): Inferred shared context (layer utility) with no import path between community 0 (core: moonshine-cpp) and community 10 (micro/stt-training/stt_training).

## Risks

- [taint critical] `core/moonshine-utils/debug-utils.cpp` -> `core/moonshine-utils/debug-utils.cpp` via `exec` (0 hops)
- [taint critical] `core/moonshine-utils/debug-utils.cpp` -> `core/moonshine-utils/debug-utils.h` via `exec` (1 hops)
- [layer strict] `core/intent-recognizer-test.cpp` (testing) -> `core/moonshine-c-api.h` (presentation)
- [layer strict] `core/tts-repeated-memory-test.cpp` (testing) -> `core/moonshine-c-api.h` (presentation)
- [layer strict] `core/word-alignment-test.cpp` (testing) -> `core/moonshine-c-api.h` (presentation)
- [dataflow DEAD_STORE] `core/intent-recognizer-test.cpp:154` `TEST_CASE` `threshold`: `threshold` assigned at line 154 but never read afterwards.
- [dataflow UNCHECKED_ALLOC] `core/intent-recognizer-test.cpp:593` `SUBCASE` `buf`: Result of allocator stored in `buf` is never checked against NULL.
- [dataflow DEAD_STORE] `core/moonshine-c-api.cpp:446` `moonshine_transcribe_stream` `next_intent_recognizer_handle`: `next_intent_recognizer_handle` assigned at line 446 but never read afterwards.
- [dataflow UNCHECKED_ALLOC] `core/moonshine-c-api.cpp:476` `duplicate_c_string` `out`: Result of allocator stored in `out` is never checked against NULL.
- [dataflow UNCHECKED_ALLOC] `core/moonshine-c-api.cpp:700` `moonshine_calculate_intent_embedding` `buf`: Result of allocator stored in `buf` is never checked against NULL.
- [dataflow DEAD_STORE] `core/moonshine-c-api.cpp:753` `b` `next_text_to_speech_synthesizer_handle`: `next_text_to_speech_synthesizer_handle` assigned at line 753 but never read afterwards.
- [dataflow DEAD_STORE] `core/moonshine-c-api.cpp:814` `maybe_autotranscribe_zipvoice_clone` `n`: `n` assigned at line 814 but never read afterwards.
- [dataflow UNCHECKED_ALLOC] `core/moonshine-c-api.cpp:1145` `malloc_string_copy` `p`: Result of allocator stored in `p` is never checked against NULL.
- [dataflow DEAD_STORE] `core/moonshine-c-api.cpp:1800` `moonshine_get_intent_dependencies` `next_grapheme_phonemizer_handle`: `next_grapheme_phonemizer_handle` assigned at line 1800 but never read afterwards.
- [dataflow UNCHECKED_ALLOC] `core/moonshine-c-api.cpp:2047` `moonshine_text_to_phonemes` `buf`: Result of allocator stored in `buf` is never checked against NULL.

## Open Questions

- Why do 51 file(s) lack file-level docs (e.g. `android/moonshine-jni/moonshine-jni.cpp`)? What purpose do they serve?
- Is the dangerous import `exec` in `core/moonshine-utils/debug-utils.cpp` still required, or can it be isolated?
- What would break if the most connected file in core: moonshine-cpp changed?
- Should core: moonshine-cpp be split, given cohesion 0.88?

## Sources

- `android/moonshine-jni/moonshine-jni.cpp`
- `core/benchmark.cpp`
- `core/bin-tokenizer/bin-tokenizer-test.cpp`
- `core/bin-tokenizer/bin-tokenizer.cpp`
- `core/bin-tokenizer/bin-tokenizer.h`
- `core/embedding-model.h`
- `core/gemma-embedding-model-test.cpp`
- `core/gemma-embedding-model.cpp`
- `core/gemma-embedding-model.h`
- `core/intent-recognizer-test.cpp`
- `core/intent-recognizer.cpp`
- `core/intent-recognizer.h`
- `core/moonshine-c-api-memory-test.cpp`
- `core/moonshine-c-api-test.cpp`
- `core/moonshine-c-api.cpp`
- `core/moonshine-c-api.h`
- `core/moonshine-cpp-test.cpp`
- `core/moonshine-cpp.h`
- `core/moonshine-download-smoke.cpp`
- `core/moonshine-model-catalog.cpp`
- *... and 52 more*
