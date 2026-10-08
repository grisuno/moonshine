# Index (page 1 of 2)
Pages: [INDEX.md](INDEX.md), [INDEX_p2.md](INDEX_p2.md)

| File | Purpose | Subsystem | Symbols | Used by |
|------|---------|-----------|---------|---------|
| `android/java/androidTest/java/ai/moonshine/voice/AssetDownloaderTest.java` | AssetDownloaderTest: End-to-end tests that exercise {@link AssetDownloader} against the... | android_java_androidTest_java_ai_moonshine_voice | 6 | 0 |
| `android/java/androidTest/java/ai/moonshine/voice/IntentRecognizerTest.java` | - | android_java_androidTest_java_ai_moonshine_voice | 3 | 0 |
| `android/java/androidTest/java/ai/moonshine/voice/JNITest.java` | - | android_java_androidTest_java_ai_moonshine_voice | 9 | 0 |
| `android/java/androidTest/java/ai/moonshine/voice/NoTranscriptionTest.java` | - | android_java_androidTest_java_ai_moonshine_voice | 13 | 0 |
| `android/java/androidTest/java/ai/moonshine/voice/TextToSpeechTest.java` | TextToSpeechTest: ZipVoice TTS coverage for the Android JNI binding.  <p>The catalog /... | android_java_androidTest_java_ai_moonshine_voice | 7 | 0 |
| `android/java/androidTest/java/ai/moonshine/voice/TranscriberTest.java` | - | android_java_androidTest_java_ai_moonshine_voice | 14 | 0 |
| `android/java/androidTest/java/ai/moonshine/voice/Utils.java` | - | android_java_androidTest_java_ai_moonshine_voice | 9 | 0 |
| `android/java/main/java/ai/moonshine/voice/AssetDownloader.java` | AssetDownloader: Downloads the model/data files a Moonshine engine needs into an app-chosen... | voice | 14 | 0 |
| `android/java/main/java/ai/moonshine/voice/GraphemeToPhonemizer.java` | GraphemeToPhonemizer: Grapheme-to-phoneme (IPA) via the Moonshine native API.  <p>Aligns with... | voice | 12 | 0 |
| `android/java/main/java/ai/moonshine/voice/IntentMatch.java` | IntentMatch: package ai.moonshine.voice; /** One ranked intent from {@link... | voice | 2 | 0 |
| `android/java/main/java/ai/moonshine/voice/IntentRecognizer.java` | IntentRecognizer: Semantic intent recognizer: registers canonical phrases and ranks them against... | voice | 14 | 0 |
| `android/java/main/java/ai/moonshine/voice/JNI.java` | - | voice | 2 | 6 |
| `android/java/main/java/ai/moonshine/voice/MicCaptureProcessor.java` | MicCaptureProcessor: Reads a stream of audio data from the microphone on a separate thread... | voice | 3 | 0 |
| `android/java/main/java/ai/moonshine/voice/MicTranscriber.java` | loadFromAssets: These load* methods are overridden to complete the CompletableFuture when the... | voice | 16 | 0 |
| `android/java/main/java/ai/moonshine/voice/ModelSpec.java` | ModelSpec: Describes which model's files {@link AssetDownloader} (or {@link... | voice | 8 | 1 |
| `android/java/main/java/ai/moonshine/voice/MoonshineDownloadWorker.java` | MoonshineDownloadWorker: Runs {@link AssetDownloader#ensureModelPresent} under WorkManager so... | voice | 6 | 0 |
| `android/java/main/java/ai/moonshine/voice/SpeakerSpan.java` | SpeakerSpan: One contiguous span of speech within a line attributed to a single speaker. | voice | 2 | 0 |
| `android/java/main/java/ai/moonshine/voice/TextToSpeech.java` | TextToSpeech: On-device text-to-speech via the Moonshine native API (Kokoro / Piper / ZipVoice... | voice | 40 | 0 |
| `android/java/main/java/ai/moonshine/voice/Transcriber.java` | getTranscribeFlags: Sets the flags applied to subsequent transcription calls. | voice | 29 | 0 |
| `android/java/main/java/ai/moonshine/voice/TranscriberOption.java` | - | voice | 4 | 3 |
| `android/java/main/java/ai/moonshine/voice/Transcript.java` | - | voice | 2 | 0 |
| `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java` | - | voice | 20 | 4 |
| `android/java/main/java/ai/moonshine/voice/TranscriptEventListener.java` | - | voice | 7 | 0 |
| `android/java/main/java/ai/moonshine/voice/TranscriptLine.java` | - | voice | 2 | 3 |
| `android/java/main/java/ai/moonshine/voice/TtsSynthesisResult.java` | TtsSynthesisResult: package ai.moonshine.voice; /** PCM float samples (~-1..1) and sample rate... | voice | 3 | 0 |
| `android/java/main/java/ai/moonshine/voice/WordTiming.java` | - | voice | 2 | 0 |
| `android/java/test/java/ai/moonshine/voice/ExampleUnitTest.java` | ExampleUnitTest: Example local unit test, which will execute on the development machine (host).... | misc | 2 | 0 |
| `android/moonshine-jni/moonshine-jni.cpp` | - | misc | 29 | 0 |
| `clang-format.sh` | - | root | 0 | 0 |
| `core/benchmark.cpp` | - | core | 7 | 0 |
| `core/bin-tokenizer/bin-tokenizer-test.cpp` | - | bin-tokenizer | 4 | 0 |
| `core/bin-tokenizer/bin-tokenizer.cpp` | BinTokenizer: if defined(ANDROID) | bin-tokenizer | 8 | 0 |
| `core/bin-tokenizer/bin-tokenizer.h` | - | bin-tokenizer | 2 | 11 |
| `core/cosine-distance-test.cpp` | - | core | 8 | 0 |
| `core/cosine-distance.cpp` | - | core | 1 | 0 |
| `core/cosine-distance.h` | Computes cosine distance between two vectors: 1 - (a·b)/(\|\|a\|\|*\|\|b\|\|). | core | 2 | 2 |
| `core/cpp-annote/src/annotation_support.h` | segment_union: Union (\|): covers both segments including any gap between them. | core_cpp-annote_src | 8 | 1 |
| `core/cpp-annote/src/clustering_vbx.cpp` | - | core_cpp-annote_src | 14 | 0 |
| `core/cpp-annote/src/clustering_vbx.h` | vbx_clustering_hard: ``embeddings`` row-major ``(num_chunks * num_speakers * dim)``... | core_cpp-annote_src | 3 | 3 |
| `core/cpp-annote/src/community1_cpp_annote_embedded.cpp` | - | core_cpp-annote_src | 0 | 0 |
| `core/cpp-annote/src/community1_cpp_annote_embedded.h` | - | core_cpp-annote_src | 13 | 1 |
| `core/cpp-annote/src/community1_ort_embedded.cpp` | - | core_cpp-annote_src | 0 | 0 |
| `core/cpp-annote/src/community1_ort_embedded.h` | - | core_cpp-annote_src | 9 | 1 |
| `core/cpp-annote/src/compute_fbank.cpp` | - | core_cpp-annote_src | 2 | 0 |
| `core/cpp-annote/src/compute_fbank.h` | wespeaker_like_fbank: Mono waveform ``[-1,1]`` → log-fbank, shape ``(T * num_mel_bins)`` row-major. | core_cpp-annote_src | 2 | 3 |
| `core/cpp-annote/src/cpp-annote-engine.h` | - | core_cpp-annote_src | 18 | 3 |
| `core/cpp-annote/src/cpp-annote-streaming.cpp` | - | core_cpp-annote_src | 26 | 0 |
| `core/cpp-annote/src/cpp-annote-streaming.h` | StreamingDiarizationSession: Session bound to a ``CppAnnoteEngine``; the engine must outlive the... | core_cpp-annote_src | 20 | 3 |
| `core/cpp-annote/src/cpp-annote.cpp` | - | core_cpp-annote_src | 65 | 0 |
| `core/cpp-annote/src/cpp-annote.h` | CppAnnote: Loads segmentation and embedding ORT models from compiled-in data and manages... | core_cpp-annote_src | 10 | 2 |
| `core/cpp-annote/src/embedding_ort_infer.cpp` | - | core_cpp-annote_src | 9 | 0 |
| `core/cpp-annote/src/embedding_ort_infer.h` | - | core_cpp-annote_src | 6 | 2 |
| `core/cpp-annote/src/filter_train.cpp` | - | core_cpp-annote_src | 1 | 0 |
| `core/cpp-annote/src/filter_train.h` | filter_embeddings_train: Row-major ``embeddings`` length ``num_chunks * num_speakers * dim``... | core_cpp-annote_src | 2 | 2 |
| `core/cpp-annote/src/hungarian.h` | - | core_cpp-annote_src | 8 | 1 |
| `core/cpp-annote/src/parity_log.cpp` | - | core_cpp-annote_src | 7 | 0 |
| `core/cpp-annote/src/parity_log.h` | env_parity_level: ``PYANNOTE_CPP_PARITY``: unset or ``0`` = off; ``1`` = stderr light log; ``2``... | core_cpp-annote_src | 6 | 3 |
| `core/cpp-annote/src/plda_vbx.cpp` | load: The upstream file-based PldaModel::load() (cnpy NPZ loading) is removed in this vendored... | core_cpp-annote_src | 10 | 0 |
| `core/cpp-annote/src/plda_vbx.h` | load_from_arrays: Load from raw NumPy-export tensors (same layout as HF ``xvec_transform.npz`` /... | core_cpp-annote_src | 5 | 4 |
| `core/cpp-annote/src/scipy_linkage.cpp` | - | core_cpp-annote_src | 14 | 0 |
| `core/cpp-annote/src/scipy_linkage.h` | pdist_euclidean: Row-major `X`: `n` rows, `d` cols → condensed pairwise Euclidean distances... | core_cpp-annote_src | 6 | 2 |
| `core/cpp-annote/src/wav_pcm_float32.h` | load_wav_pcm16_mono_float32: PCM 16 LE mono or stereo (mean to mono) → float32 mono... | core_cpp-annote_src | 9 | 3 |
| `core/embedding-model.h` | EmbeddingModel: Abstract interface for embedding models that convert text to vector representations. | core | 6 | 2 |
| `core/gemma-embedding-model-test.cpp` | - | core | 14 | 0 |
| `core/gemma-embedding-model.cpp` | attention_mask: Create attention mask (all 1s for actual tokens) | core | 20 | 0 |
| `core/gemma-embedding-model.h` | GemmaEmbeddingModel: Gemma Embedding Model implementation using ONNX Runtime C API. | core | 15 | 4 |
| `core/intent-recognizer-test.cpp` | Path to the Gemma embedding model | core | 59 | 0 |
| `core/intent-recognizer.cpp` | - | core | 12 | 0 |
| `core/intent-recognizer.h` | EmbeddingModelArch: Supported embedding model architectures. | core | 13 | 3 |
| `core/moonshine-c-api-memory-test.cpp` | Integration test: TTS from memory while CWD is an empty sandbox (no repo data). | core | 7 | 0 |
| `core/moonshine-c-api-test.cpp` | find_moonshine_tts_data_dir: Resolve ``moonshine-tts/data`` for tests run from ``test-assets/``... | core | 81 | 0 |
| `core/moonshine-c-api.cpp` | parse_common_options: Handles common options that are not specific to any particular API. | core | 72 | 0 |
| `core/moonshine-c-api.h` | Moonshine is a library for building interactive voice applications. | core | 57 | 12 |
| `core/moonshine-cpp-test.cpp` | load_wav_data: Duplicate of load_wav_data in debug-utils.cpp to avoid depending on internal... | core | 15 | 0 |
| `core/moonshine-cpp.h` | Moonshine C++ API - Header-only library | core | 127 | 3 |
| `core/moonshine-download-smoke.cpp` | moonshine-download-smoke: a tiny CLI used by scripts/test-model-downloads.sh to verify that the... | core | 17 | 0 |
| `core/moonshine-model-catalog.cpp` | stt_catalog: Port of MODEL_INFO from python/src/moonshine_voice/download.py. | core | 19 | 0 |
| `core/moonshine-model-catalog.h` | Native catalog of downloadable model assets (speech-to-text transcription, the optional... | core | 3 | 2 |
| `core/moonshine-model.cpp` | load_from_assets: if defined(ANDROID) | core | 34 | 0 |
| `core/moonshine-model.h` | load_from_assets: if defined(ANDROID) | core | 9 | 2 |
| `core/moonshine-streaming-model.cpp` | Streaming model constants | core | 42 | 0 |
| `core/moonshine-streaming-model.h` | Streaming model configuration (matches streaming_config.json) | core | 19 | 1 |
| `core/moonshine-tts/src/constants.h` | - | core_moonshine-tts_src | 1 | 2 |
| `core/moonshine-tts/src/file-information.cpp` | - | core_moonshine-tts_src | 5 | 0 |
| `core/moonshine-tts/src/file-information.h` | FileInformation: Describes a bundled asset: optional on-disk ``path`` (relative to a caller root... | core_moonshine-tts_src | 10 | 8 |
| `core/moonshine-tts/src/g2p-path.h` | resolve_path_under_root: If ``path`` is absolute, returns it unchanged. | core_moonshine-tts_src | 5 | 12 |
| `core/moonshine-tts/src/g2p-word-log.cpp` | - | core_moonshine-tts_src | 2 | 0 |
| `core/moonshine-tts/src/g2p-word-log.h` | G2pWordPath: How a surface word was converted to IPA in ``MoonshineG2P`` / ``EnglishRuleG2p``... | core_moonshine-tts_src | 5 | 19 |
| `core/moonshine-tts/src/ipa-postprocess.cpp` | apply_german_ipa_piper_style: U+0361 COMBINING DOUBLE INVERTED BREVE between consonants (narrow... | core_moonshine-tts_src | 49 | 0 |
| `core/moonshine-tts/src/ipa-postprocess.h` | repair_ascii_c_combining_cedilla_to_ccedilla_utf8: Replace ASCII ``c`` + U+0327 COMBINING... | core_moonshine-tts_src | 4 | 7 |
| `core/moonshine-tts/src/json-config.cpp` | - | core_moonshine-tts_src | 5 | 0 |
| `core/moonshine-tts/src/json-config.h` | - | core_moonshine-tts_src | 2 | 3 |
| `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp` | is_punct_char_word_group_u32: ``token_word_group_indices`` uses :func:`_is_punct_char` (Unicode... | lang-specific | 36 | 0 |
| `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.h` | ArabicDiacOnnx: BERT token-classification tashkīl (Arabert-style), mirroring... | lang-specific | 4 | 2 |
| `core/moonshine-tts/src/lang-specific/arabic-ipa.cpp` | - | lang-specific | 15 | 0 |
| `core/moonshine-tts/src/lang-specific/arabic-ipa.h` | - | lang-specific | 1 | 2 |
| `core/moonshine-tts/src/lang-specific/arabic.cpp` | - | lang-specific | 13 | 0 |
| `core/moonshine-tts/src/lang-specific/arabic.h` | ArabicRuleG2p: MSA Arabic G2P: ONNX partial tashkīl + lexicon + IPA rules (mirrors... | lang-specific | 7 | 5 |
| `core/moonshine-tts/src/lang-specific/chinese-numbers.cpp` | - | lang-specific | 9 | 0 |
| `core/moonshine-tts/src/lang-specific/chinese-numbers.h` | - | lang-specific | 1 | 2 |
| `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.cpp` | - | lang-specific | 12 | 0 |
| `core/moonshine-tts/src/lang-specific/chinese-onnx-g2p.h` | ChineseOnnxG2p: ONNX BIO segmentation + UPOS + ``data/zh_hans/dict.tsv`` (mirrors... | lang-specific | 6 | 4 |
| `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp` | is_punct_char_word_group_u32: ``token_word_group_indices`` uses :func:`_is_punct_char` (Unicode... | lang-specific | 35 | 0 |
| `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.h` | ChineseTokPosOnnx: Simplified-Chinese surfaces + UD UPOS via ONNX... | lang-specific | 5 | 3 |
| `core/moonshine-tts/src/lang-specific/chinese.cpp` | - | lang-specific | 28 | 0 |
| `core/moonshine-tts/src/lang-specific/chinese.h` | ChineseRuleG2p: Simplified Chinese lexicon G2P (``data/zh_hans/dict.tsv`` ipa-dict IPA)... | lang-specific | 6 | 5 |
| `core/moonshine-tts/src/lang-specific/cmudict-tsv.cpp` | - | lang-specific | 6 | 0 |
| `core/moonshine-tts/src/lang-specific/cmudict-tsv.h` | CmudictTsv: word key (normalized grapheme) -> sorted unique IPA strings (TSV: word<TAB>ipa). | lang-specific | 3 | 3 |
| `core/moonshine-tts/src/lang-specific/dutch.cpp` | append_lexicon_folded: Fold to ``a-z`` + hyphen for TSV keys (mirrors Python... | lang-specific | 54 | 0 |
| `core/moonshine-tts/src/lang-specific/dutch.h` | DutchRuleG2p: Rule- and lexicon-based Dutch G2P, mirroring ``dutch_rule_g2p.py`` /... | lang-specific | 8 | 6 |
| `core/moonshine-tts/src/lang-specific/english-hand-oov.cpp` | - | lang-specific | 14 | 0 |
| `core/moonshine-tts/src/lang-specific/english-hand-oov.h` | - | lang-specific | 1 | 3 |
| `core/moonshine-tts/src/lang-specific/english-numbers.cpp` | - | lang-specific | 7 | 0 |
| `core/moonshine-tts/src/lang-specific/english-numbers.h` | - | lang-specific | 1 | 3 |
| `core/moonshine-tts/src/lang-specific/english.cpp` | pick_english_heteronym_ipa: CMU-style heteronyms such as ``tomato`` include both US (stressed... | lang-specific | 8 | 0 |
| `core/moonshine-tts/src/lang-specific/english.h` | EnglishRuleG2p: US English lexicon + OOV ONNX + hand OOV fallback (no heteronym ONNX). | lang-specific | 8 | 4 |
| `core/moonshine-tts/src/lang-specific/french-compound-map.cpp` | - | lang-specific | 0 | 0 |
| `core/moonshine-tts/src/lang-specific/french-compound-map.h` | - | lang-specific | 1 | 2 |
| `core/moonshine-tts/src/lang-specific/french-internal.h` | - | lang-specific | 1 | 2 |
| `core/moonshine-tts/src/lang-specific/french-oov.cpp` | - | lang-specific | 13 | 0 |
| `core/moonshine-tts/src/lang-specific/french.cpp` | is_latin1_supplement_python_word_char: Python ``re.UNICODE`` word chars in U+00AA..U+00FF... | lang-specific | 55 | 0 |
| `core/moonshine-tts/src/lang-specific/french.h` | FrenchRuleG2p: Lexicon + liaison + OOV rules + cardinal digit expansion (mirrors ``french_g2p.py``). | lang-specific | 8 | 5 |
| `core/moonshine-tts/src/lang-specific/german.cpp` | normalize_lookup_key_utf8: NFC-style key: lowercase letters + umlauts + ß only (Python... | lang-specific | 43 | 0 |
| `core/moonshine-tts/src/lang-specific/german.h` | GermanRuleG2p: Rule- and lexicon-based German G2P (High German), mirroring ``german_rule_g2p.py``. | lang-specific | 8 | 8 |
| `core/moonshine-tts/src/lang-specific/heteronym-context.cpp` | - | lang-specific | 1 | 0 |
| `core/moonshine-tts/src/lang-specific/heteronym-context.h` | - | lang-specific | 1 | 2 |
| `core/moonshine-tts/src/lang-specific/hindi-numbers.cpp` | - | lang-specific | 11 | 0 |
| `core/moonshine-tts/src/lang-specific/hindi-numbers.h` | - | lang-specific | 1 | 3 |
| `core/moonshine-tts/src/lang-specific/hindi.cpp` | - | lang-specific | 29 | 0 |
| `core/moonshine-tts/src/lang-specific/hindi.h` | HindiRuleG2p: Hindi Devanagari G2P: ``dict.tsv`` lookup + rule-based parsing (mirrors... | lang-specific | 7 | 5 |
| `core/moonshine-tts/src/lang-specific/ipa-symbols.h` | - | lang-specific | 1 | 8 |
| `core/moonshine-tts/src/lang-specific/italian.cpp` | italian_cg_palatal_letter: After c/g (and related digraphs): letters that palatalize, matching... | lang-specific | 47 | 0 |
| `core/moonshine-tts/src/lang-specific/italian.h` | ItalianRuleG2p: Rule- and lexicon-based Italian G2P, mirroring ``italian_rule_g2p.py`` /... | lang-specific | 7 | 5 |
| `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.cpp` | - | lang-specific | 10 | 0 |
| `core/moonshine-tts/src/lang-specific/japanese-kana-to-ipa.h` | - | lang-specific | 3 | 2 |
| `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.cpp` | - | lang-specific | 18 | 0 |
| `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.h` | JapaneseOnnxG2p: ONNX LUW segmentation + ``data/ja/dict.tsv`` + kana IPA (mirrors... | lang-specific | 4 | 4 |
| `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp` | is_punct_char_word_group_u32: ``token_word_group_indices`` uses :func:`_is_punct_char` (Unicode... | lang-specific | 38 | 0 |
| `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.h` | JapaneseTokPosOnnx: Japanese LUW surfaces + UD UPOS via ONNX... | lang-specific | 5 | 3 |
| `core/moonshine-tts/src/lang-specific/japanese.cpp` | - | lang-specific | 10 | 0 |
| `core/moonshine-tts/src/lang-specific/japanese.h` | JapaneseRuleG2p: Japanese G2P via ONNX LUW segmentation + ``data/ja/dict.tsv`` (mirrors... | lang-specific | 7 | 3 |
| `core/moonshine-tts/src/lang-specific/korean-numbers.cpp` | - | lang-specific | 11 | 0 |
| `core/moonshine-tts/src/lang-specific/korean-numbers.h` | - | lang-specific | 2 | 3 |
| `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp` | is_punct_char_word_group_u32: ``token_word_group_indices`` uses :func:`_is_punct_char` (Unicode... | lang-specific | 38 | 0 |
| `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.h` | KoreanTokPosOnnx: Korean whitespace-level words + UD UPOS via ONNX... | lang-specific | 5 | 2 |
| `core/moonshine-tts/src/lang-specific/korean.cpp` | is_sonorant_jong: Sonorant codas: nasals (ㄴ,ㅁ,ŋ) and liquids (ㄹ and ㄹ-clusters). | lang-specific | 33 | 0 |
| `core/moonshine-tts/src/lang-specific/korean.h` | KoreanRuleG2p: Lexicon + Hangul rule G2P (연음, 유음화, 비음화, ㅎ aspiration, 경음화), mirroring... | lang-specific | 8 | 5 |
| `core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp` | - | lang-specific | 10 | 0 |
| `core/moonshine-tts/src/lang-specific/onnx-g2p-models.h` | - | lang-specific | 2 | 2 |
| `core/moonshine-tts/src/lang-specific/portuguese-rules.cpp` | - | lang-specific | 27 | 0 |
| `core/moonshine-tts/src/lang-specific/portuguese-rules.h` | - | lang-specific | 2 | 2 |
| `core/moonshine-tts/src/lang-specific/portuguese.cpp` | - | lang-specific | 26 | 0 |
| `core/moonshine-tts/src/lang-specific/portuguese.h` | PortugueseRuleG2p: Rule- and lexicon-based Portuguese G2P (Brazil / Portugal), mirroring... | lang-specific | 9 | 5 |
| `core/moonshine-tts/src/lang-specific/russian-numbers.cpp` | Russian cardinal expansion (russian_numbers.py). #include from russian.cpp (same TU). | lang-specific | 10 | 1 |
| `core/moonshine-tts/src/lang-specific/russian.cpp` | normalize_lookup_key_utf8: Mirrors Python ``normalize_lookup_key`` (lower + NFD + Mn strip +... | lang-specific | 47 | 0 |
| `core/moonshine-tts/src/lang-specific/russian.h` | RussianRuleG2p: Rule- and lexicon-based Russian G2P, mirroring ``russian_rule_g2p.py``. | lang-specific | 7 | 4 |
| `core/moonshine-tts/src/lang-specific/spanish-numbers.cpp` | Spanish cardinal expansion (spanish_numbers.py). #include from spanish.cpp (same TU). | lang-specific | 8 | 1 |
| `core/moonshine-tts/src/lang-specific/spanish-unicode-tables.cpp` | - | lang-specific | 0 | 0 |
| `core/moonshine-tts/src/lang-specific/spanish-unicode-tables.h` | k_unicode_strip_table: Definitions in spanish_unicode_tables.cpp (generated Unicode data). | lang-specific | 9 | 2 |
| `core/moonshine-tts/src/lang-specific/spanish-unicode.cpp` | - | lang-specific | 11 | 0 |
| `core/moonshine-tts/src/lang-specific/spanish-unicode.h` | strip_replacement_utf8: UTF-8 replacement from the strip table, or nullptr when absent. | lang-specific | 4 | 2 |
| `core/moonshine-tts/src/lang-specific/spanish.cpp` | - | lang-specific | 31 | 0 |
| `core/moonshine-tts/src/lang-specific/spanish.h` | SpanishRuleG2p: Rule-based Spanish G2P (mirrors ``spanish_rule_g2p.py``). | lang-specific | 9 | 5 |
| `core/moonshine-tts/src/lang-specific/turkish.cpp` | - | lang-specific | 39 | 0 |
| `core/moonshine-tts/src/lang-specific/turkish.h` | TurkishRuleG2p: Rule-based Turkish G2P (mirrors ``turkish_rule_g2p.py``): nearly phonemic... | lang-specific | 9 | 4 |
| `core/moonshine-tts/src/lang-specific/ukrainian.cpp` | - | lang-specific | 47 | 0 |
| `core/moonshine-tts/src/lang-specific/ukrainian.h` | UkrainianRuleG2p: Rule-based Ukrainian G2P (mirrors ``ukrainian_rule_g2p.py``): Cyrillic +... | lang-specific | 9 | 4 |
| `core/moonshine-tts/src/lang-specific/vietnamese.cpp` | split_tone: Tone combining marks (NFD) -> id 2..6; default 1 (ngang). | lang-specific | 32 | 0 |
| `core/moonshine-tts/src/lang-specific/vietnamese.h` | VietnameseRuleG2p: Vietnamese lexicon + greedy longest-match + OOV syllable rules (Northern IPA... | lang-specific | 6 | 5 |
| `core/moonshine-tts/src/moonshine-asset-catalog.cpp` | - | core_moonshine-tts_src | 13 | 0 |
| `core/moonshine-tts/src/moonshine-asset-catalog.h` | moonshine_asset_catalog_populate_default_g2p_files: Fills ``files`` with default canonical G2P... | core_moonshine-tts_src | 2 | 4 |
| `core/moonshine-tts/src/moonshine-g2p-options.cpp` | - | core_moonshine-tts_src | 14 | 0 |
| `core/moonshine-tts/src/moonshine-g2p-options.h` | MoonshineG2POptions: Options for constructing ``MoonshineG2P`` (rule-engine paths and toggles... | core_moonshine-tts_src | 6 | 18 |
| `core/moonshine-tts/src/moonshine-g2p.cpp` | normalize_spanish_dialect_cli_key: Normalize user input like ``es_ar`` / ``es-mx`` to keys... | core_moonshine-tts_src | 7 | 0 |
| `core/moonshine-tts/src/moonshine-g2p.h` | MoonshineG2P: Single entry point: *dialect_id* is a tag such as ``en_us``, ``es-AR``, ``de``... | core_moonshine-tts_src | 21 | 11 |
| `core/moonshine-tts/src/moonshine-tts-options.cpp` | - | core_moonshine-tts_src | 7 | 0 |
| `core/moonshine-tts/src/moonshine-tts-options.h` | MoonshineTTSOptions: Shared configuration for ``MoonshineTTS`` (Kokoro and Piper file paths... | core_moonshine-tts_src | 5 | 5 |
| `core/moonshine-tts/src/moonshine-tts.cpp` | SynthesisOverrides: Per-call overrides parsed from ``MoonshineTTS::synthesize`` option pairs. | core_moonshine-tts_src | 82 | 0 |
| `core/moonshine-tts/src/moonshine-tts.h` | MoonshineTTS: Unified TTS: **Kokoro** and **Piper** ONNX backends; shared ``MoonshineG2P`` where... | core_moonshine-tts_src | 7 | 5 |
| `core/moonshine-tts/src/ort-onnx-external-data.cpp` | - | core_moonshine-tts_src | 1 | 0 |
| `core/moonshine-tts/src/ort-onnx-external-data.h` | ort_add_external_initializer_files_for_onnx_model_buffer: If ``files`` contains an in-memory... | core_moonshine-tts_src | 2 | 8 |
| `core/moonshine-tts/src/ort-session-options.cpp` | - | core_moonshine-tts_src | 1 | 0 |
| `core/moonshine-tts/src/ort-session-options.h` | - | core_moonshine-tts_src | 1 | 9 |
| `core/moonshine-tts/src/piper-tts.cpp` | piper_model_json_path_for_onnx: Piper pairs ``foo.onnx`` with ``foo.onnx.json``. | core_moonshine-tts_src | 40 | 0 |
| `core/moonshine-tts/src/piper-tts.h` | PiperTTSOptions: Piper ONNX TTS + ``MoonshineG2P`` IPA (filtered to each model's... | core_moonshine-tts_src | 15 | 3 |
| `core/moonshine-tts/src/piper-voice-catalog.cpp` | Bundled Piper ONNX stems, kept in sync with ``moonshine-tts/data/*/piper-voices/*.onnx``. | core_moonshine-tts_src | 0 | 0 |
| `core/moonshine-tts/src/piper-voice-catalog.h` | piper_bundled_voice_stems_for_data_subdir: ONNX stems (no ``.onnx``) shipped under... | core_moonshine-tts_src | 2 | 2 |
| `core/moonshine-tts/src/rule-based-g2p-factory.cpp` | g2p_onnx_bundle_includes_model_file: True when ``meta.json`` is available and the model file it... | core_moonshine-tts_src | 26 | 0 |
| `core/moonshine-tts/src/rule-based-g2p-factory.h` | - | core_moonshine-tts_src | 4 | 3 |
| `core/moonshine-tts/src/rule-based-g2p.h` | RuleBasedG2p: Shared interface for lexicon + rules G2P backends used by ``MoonshineG2P``. | core_moonshine-tts_src | 3 | 19 |
| `core/moonshine-tts/src/text-normalize.cpp` | - | core_moonshine-tts_src | 4 | 0 |
| `core/moonshine-tts/src/text-normalize.h` | - | core_moonshine-tts_src | 1 | 5 |
| `core/moonshine-tts/src/utf8-utils.cpp` | - | core_moonshine-tts_src | 10 | 0 |
| `core/moonshine-tts/src/utf8-utils.h` | erase_utf8_substr: Remove every occurrence of *sub* from *s*. | core_moonshine-tts_src | 10 | 45 |
| `core/moonshine-tts/src/zipvoice-custom-ops.cpp` | Custom ONNX Runtime operators for the ZipVoice Zipformer (domain ai.zipvoice). | core_moonshine-tts_src | 62 | 0 |
| `core/moonshine-tts/src/zipvoice-custom-ops.h` | zipvoice_register_custom_ops: Registers the ``ai.zipvoice`` custom ONNX Runtime operators... | core_moonshine-tts_src | 2 | 2 |
| `core/moonshine-tts/src/zipvoice-mel.cpp` | fft_radix2: Iterative radix-2 Cooley-Tukey FFT for power-of-two ``n`` (in-place, natural ->... | core_moonshine-tts_src | 15 | 0 |
| `core/moonshine-tts/src/zipvoice-mel.h` | VocosFbank: Log-mel feature frontend matching ZipVoice's ``VocosFbank``... | core_moonshine-tts_src | 4 | 3 |
| `core/moonshine-tts/src/zipvoice-tts.cpp` | resolve_zipvoice_lang: English-only for now; structured so more locales can be added. | core_moonshine-tts_src | 49 | 0 |
| `core/moonshine-tts/src/zipvoice-tts.h` | ZipVoiceTTSOptions: Options for the ZipVoice zero-shot voice-cloning ONNX TTS engine. | core_moonshine-tts_src | 13 | 3 |
| `core/moonshine-tts/src/zipvoice-voices-data.cpp` | - | core_moonshine-tts_src | 0 | 0 |
| `core/moonshine-tts/src/zipvoice-voices.cpp` | - | core_moonshine-tts_src | 3 | 0 |
| `core/moonshine-tts/src/zipvoice-voices.h` | ZipVoiceBuiltinVoice: One built-in ZipVoice reference voice to clone, sourced from the VCTK... | core_moonshine-tts_src | 5 | 4 |
| `core/moonshine-tts/tests/arabic-rule-g2p-test.cpp` | - | tests | 2 | 0 |
| `core/moonshine-tts/tests/chinese-rule-g2p-test.cpp` | - | tests | 4 | 0 |
| `core/moonshine-tts/tests/chinese-tok-pos-onnx-test.cpp` | - | tests | 3 | 0 |
| `core/moonshine-tts/tests/cmudict-tsv-test.cpp` | - | tests | 2 | 0 |
| `core/moonshine-tts/tests/dutch-rule-g2p-test.cpp` | - | tests | 9 | 0 |
| `core/moonshine-tts/tests/english-hand-oov-test.cpp` | - | tests | 3 | 0 |
| `core/moonshine-tts/tests/english-rule-g2p-test.cpp` | - | tests | 5 | 0 |
| `core/moonshine-tts/tests/file-information-test.cpp` | - | tests | 7 | 0 |
| `core/moonshine-tts/tests/french-rule-g2p-test.cpp` | - | tests | 11 | 0 |
| `core/moonshine-tts/tests/german-rule-g2p-test.cpp` | - | tests | 11 | 0 |
| `core/moonshine-tts/tests/heteronym-context-test.cpp` | - | tests | 3 | 0 |
| `core/moonshine-tts/tests/hindi-rule-g2p-test.cpp` | - | tests | 6 | 0 |
| `core/moonshine-tts/tests/ipa-postprocess-test.cpp` | ma_in: 妈 ma˥˥ → mˈa5 via the zh path | tests | 27 | 0 |
| `core/moonshine-tts/tests/italian-rule-g2p-test.cpp` | - | tests | 7 | 0 |
| `core/moonshine-tts/tests/japanese-onnx-g2p-test.cpp` | - | tests | 2 | 0 |
| `core/moonshine-tts/tests/japanese-tok-pos-onnx-test.cpp` | - | tests | 4 | 0 |
| `core/moonshine-tts/tests/json-config-test.cpp` | - | tests | 2 | 0 |
| `core/moonshine-tts/tests/korean-rule-g2p-test.cpp` | - | tests | 7 | 0 |
| `core/moonshine-tts/tests/korean-tok-pos-onnx-test.cpp` | - | tests | 3 | 0 |
| `core/moonshine-tts/tests/moonshine-g2p-options-test.cpp` | - | tests | 7 | 0 |
| `core/moonshine-tts/tests/moonshine-tts-options-test.cpp` | - | tests | 2 | 0 |
| `core/moonshine-tts/tests/moonshine-tts-speed-test.cpp` | - | tests | 4 | 0 |
| `core/moonshine-tts/tests/onnx-g2p-smoke-test.cpp` | - | tests | 3 | 0 |
| `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp` | - | tests | 8 | 0 |
| `core/moonshine-tts/tests/rule-g2p-test-support.h` | Shared helpers for rule-G2P / ONNX parity tests (pre-generated reference lines under... | tests | 9 | 21 |
| `core/moonshine-tts/tests/russian-rule-g2p-test.cpp` | - | tests | 7 | 0 |
| `core/moonshine-tts/tests/spanish-rule-g2p-test.cpp` | - | tests | 6 | 0 |
| `core/moonshine-tts/tests/text-normalize-test.cpp` | - | tests | 4 | 0 |
| `core/moonshine-tts/tests/turkish-rule-g2p-test.cpp` | - | tests | 5 | 0 |
| `core/moonshine-tts/tests/ukrainian-rule-g2p-test.cpp` | - | tests | 5 | 0 |
| `core/moonshine-tts/tests/utf8-utils-test.cpp` | - | tests | 5 | 0 |
| `core/moonshine-tts/tests/vietnamese-rule-g2p-test.cpp` | - | tests | 5 | 0 |
| `core/moonshine-tts/tests/zipvoice-tts-test.cpp` | - | tests | 6 | 0 |
| `core/moonshine-tts/tools/arabic-rule-g2p-cli.cpp` | MSA Arabic ONNX + rule G2P (mirrors ``arabic_rule_g2p.py`` CLI subset). | tools | 3 | 0 |
| `core/moonshine-tts/tools/chinese-rule-g2p-cli.cpp` | Simplified Chinese ONNX segmentation + UPOS + lexicon G2P (mirrors ``chinese_rule_g2p.py`` CLI). | tools | 3 | 0 |
| `core/moonshine-tts/tools/dutch-g2p-batch-cli.cpp` | Dutch rule + lexicon G2P (no ONNX). | tools | 4 | 0 |
| `core/moonshine-tts/tools/dutch-rule-g2p-cli.cpp` | Stand-alone Dutch rule + lexicon G2P (no ONNX). | tools | 3 | 0 |
| `core/moonshine-tts/tools/french-g2p-batch-cli.cpp` | French rule + lexicon G2P (no ONNX). | tools | 4 | 0 |
| `core/moonshine-tts/tools/german-rule-g2p-cli.cpp` | Stand-alone German rule + lexicon G2P (no ONNX). | tools | 3 | 0 |
| `core/moonshine-tts/tools/hindi-rule-g2p-cli.cpp` | Hindi rule + lexicon G2P (no ONNX). | tools | 3 | 0 |
| `core/moonshine-tts/tools/italian-rule-g2p-cli.cpp` | Stand-alone Italian rule + lexicon G2P (no ONNX). | tools | 3 | 0 |
| `core/moonshine-tts/tools/japanese-onnx-g2p-cli.cpp` | - | tools | 3 | 0 |
| `core/moonshine-tts/tools/korean-rule-g2p-cli.cpp` | Korean rule + lexicon G2P (no ONNX). | tools | 3 | 0 |
| `core/moonshine-tts/tools/moonshine-g2p-cli.cpp` | Unified G2P CLI: rule-based dialects (English, Spanish, German, …). | tools | 5 | 0 |
| `core/moonshine-tts/tools/moonshine-tts-cli.cpp` | CLI: Moonshine G2P + Kokoro or Piper ONNX → WAV (via MoonshineTTS). | tools | 3 | 0 |
| `core/moonshine-tts/tools/piper-ipa-normalize-cli.cpp` | Prints Piper-ready IPA (NFC + replacements + optional inventory coercion) for parity tests. | tools | 3 | 0 |
| `core/moonshine-tts/tools/piper-phoneme-infer-cli.cpp` | Dev / CI: Piper ONNX from a JSON list of int64 phoneme ids (parity with ``speak.py`` ORT path). | tools | 2 | 0 |
| `core/moonshine-tts/tools/portuguese-rule-g2p-cli.cpp` | Stand-alone Portuguese rule + lexicon G2P (no ONNX). | tools | 3 | 0 |
| `core/moonshine-tts/tools/vietnamese-rule-g2p-cli.cpp` | Vietnamese rule + lexicon G2P. | tools | 3 | 0 |
| `core/moonshine-utils/debug-utils-test.cpp` | - | moonshine-utils | 21 | 0 |
| `core/moonshine-utils/debug-utils.cpp` | - | moonshine-utils | 8 | 0 |
| `core/moonshine-utils/debug-utils.h` | debug_calloc: define DEBUG_CALLOC(size, count) \ | moonshine-utils | 52 | 30 |
| `core/moonshine-utils/file-utils-test.cpp` | write_file: Writes `bytes` to `path` for the read-back tests below. | moonshine-utils | 12 | 0 |
| `core/moonshine-utils/file-utils.cpp` | - | moonshine-utils | 1 | 0 |
| `core/moonshine-utils/file-utils.h` | Wrapper around std::fread that throws std::runtime_error unless the full requested number of... | moonshine-utils | 2 | 5 |
| `core/moonshine-utils/string-utils-test.cpp` | - | moonshine-utils | 20 | 0 |
| `core/moonshine-utils/string-utils.cpp` | See https://stackoverflow.com/questions/2896600/how-to-replace-all-occurrences-of-a-character-in... | moonshine-utils | 15 | 0 |
| `core/moonshine-utils/string-utils.h` | - | moonshine-utils | 7 | 12 |
| `core/moonshine-utils/test-utils.h` | - | moonshine-utils | 2 | 0 |
| `core/ort-utils/moonshine-ort-allocator.cpp` | - | ort-utils | 10 | 0 |
| `core/ort-utils/moonshine-ort-allocator.h` | - | ort-utils | 3 | 7 |
| `core/ort-utils/moonshine-tensor-view.cpp` | checked_mul: Portable checked multiply for size_t: returns false on overflow (leaving *out... | ort-utils | 24 | 0 |
| `core/ort-utils/moonshine-tensor-view.h` | create_ort_value: You need to call ort_api->ReleaseValue(output_ort_tensor) to release this... | ort-utils | 21 | 5 |
| `core/ort-utils/moonshine-tensor.cpp` | - | ort-utils | 2 | 0 |
| `core/ort-utils/moonshine-tensor.h` | moonshine_dtype_t: ifdef __cplusplus | ort-utils | 7 | 2 |
| `core/ort-utils/ort-utils-cxx.h` | - | ort-utils | 1 | 1 |
| `core/ort-utils/ort-utils-ep-test.cpp` | SUBCASE: if defined(__APPLE__) | ort-utils | 15 | 0 |
| `core/ort-utils/ort-utils-ep.cpp` | - | ort-utils | 7 | 0 |
| `core/ort-utils/ort-utils-test.cpp` | - | ort-utils | 4 | 0 |
| `core/ort-utils/ort-utils.cpp` | No memory mapping on Windows and wchar for the file path. | ort-utils | 15 | 0 |
| `core/ort-utils/ort-utils.h` | ort_session_from_asset: if defined(ANDROID) | ort-utils | 15 | 16 |
| `core/reliability/fuzz-bin-tokenizer.cpp` | libFuzzer harness for the binary tokenizer. | reliability | 1 | 0 |
| `core/reliability/fuzz-resampler.cpp` | libFuzzer harness for the audio resampler. | reliability | 3 | 0 |
| `core/reliability/fuzz-string-utils.cpp` | libFuzzer harness for the string utilities. | reliability | 1 | 0 |
| `core/reliability/fuzz-tensor-view.cpp` | libFuzzer harness for MoonshineTensorView construction. | reliability | 4 | 0 |
| `core/reliability/fuzz-wav-pcm.cpp` | libFuzzer harness for the WAV/RIFF parsers. | reliability | 0 | 0 |
| `core/resampler-test.cpp` | - | core | 7 | 0 |
| `core/resampler.cpp` | - | core | 4 | 0 |
| `core/resampler.h` | - | core | 4 | 4 |
| `core/silero-vad.cpp` | init_engine_threads: Initializes threading settings. | core | 5 | 0 |
| `core/silero-vad.h` | init_onnx_env: Initializes the common ONNX runtime environment (env, session_options... | core | 6 | 2 |
| `core/speaker-diarizer.cpp` | turn_overlap_seconds: Total seconds of overlap between the spans of two turn lists. | core | 16 | 0 |
| `core/speaker-diarizer.h` | One contiguous span of speech attributed to a single speaker on the stream timeline. | core | 9 | 1 |
| `core/spelling-fusion-data.cpp` | - | core | 9 | 0 |
| `core/spelling-fusion-data.h` | Compiled-in tables for the spelling matcher. | core | 9 | 4 |
| `core/spelling-fusion-test.cpp` | char_match: Helper: shorthand for "matcher said this character". | core | 24 | 0 |
| `core/spelling-fusion.cpp` | consume_curly_quote: Try to consume a 3-byte UTF-8 curly quote starting at ``input[i]``. | core | 19 | 0 |
| `core/spelling-fusion.h` | C++ port of the matcher / fusion logic from | core | 11 | 5 |
| `core/spelling-model-test.cpp` | Clip: (label_dir, expected canonical char). | core | 11 | 0 |
| `core/spelling-model.cpp` | lookup_metadata: Read a single key from the model's custom_metadata_map, returning nullopt when... | core | 12 | 0 |
| `core/spelling-model.h` | Wraps the SpellingCNN ``.ort`` model. | core | 11 | 2 |
| `core/tts-repeated-memory-test.cpp` | Repeated-use memory regression test for the text-to-speech synthesizers. | core | 22 | 0 |
| `core/voice-activity-detector-test.cpp` | - | core | 5 | 0 |
| `core/voice-activity-detector.cpp` | - | core | 16 | 0 |
| `core/voice-activity-detector.h` | - | core | 16 | 2 |
| `core/word-alignment-benchmark.cpp` | - | core | 4 | 0 |
| `core/word-alignment-test.cpp` | - | core | 3 | 0 |
| `core/word-alignment.cpp` | DTW (Dynamic Time Warping) | core | 15 | 0 |
| `core/word-alignment.h` | dtw: Dynamic Time Warping on a cost matrix [N x M] Returns aligned (text_indices, time_indices)... | core | 4 | 3 |
| `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/AssetDirectoryCopy.kt` | copyDirIfNeeded: package ai.moonshine.examples.intentrecognizer import android.content.Context... | intentrecognizer | 1 | 0 |
| `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/MainActivity.kt` | - | intentrecognizer | 1 | 0 |
| `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/PhraseAdapter.kt` | currentPhrases: val idx = items.indexOfFirst { it.id == id } if (idx >= 0) {... | intentrecognizer | 8 | 0 |
| `examples/android/IntentRecognizer/settings.gradle.kts` | - | misc | 0 | 0 |
| `examples/android/TextToSpeech/app/src/main/java/ai/moonshine/examples/texttospeech/AssetDirectoryCopy.kt` | copyDirIfNeeded: package ai.moonshine.examples.texttospeech import android.content.Context... | texttospeech | 1 | 0 |
| `examples/android/TextToSpeech/app/src/main/java/ai/moonshine/examples/texttospeech/MainActivity.kt` | - | texttospeech | 1 | 0 |
| `examples/android/TextToSpeech/settings.gradle.kts` | - | misc | 0 | 0 |
| `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java` | MainActivity: Minimal microphone transcription sample. | misc | 6 | 0 |
| `examples/android/Transcriber/settings.gradle.kts` | - | misc | 0 | 0 |
| `examples/c++/download-library.sh` | - | misc | 0 | 0 |
| `examples/ios/IntentRecognizer/IntentRecognizer/ContentView.swift` | - | IntentRecognizer | 1 | 0 |
| `examples/ios/IntentRecognizer/IntentRecognizer/IntentRecognizerApp.swift` | - | IntentRecognizer | 1 | 0 |
| `examples/ios/IntentRecognizer/IntentRecognizer/IntentSessionModel.swift` | - | IntentRecognizer | 13 | 0 |
| `examples/ios/IntentRecognizer/IntentRecognizer/IntentTranscriptBridge.swift` | IntentTranscriptBridge: Forwards streaming and completed transcript lines to... | IntentRecognizer | 4 | 0 |
| `examples/ios/IntentRecognizer/scripts/copy-moonshine-models.sh` | - | misc | 0 | 0 |
| `examples/ios/TextToSpeech/TextToSpeech/ContentView.swift` | - | TextToSpeech | 1 | 0 |
| `examples/ios/TextToSpeech/TextToSpeech/TextToSpeechApp.swift` | KokoroLanguage: Kokoro/Piper-supported languages with display names. | TextToSpeech | 11 | 0 |
| `examples/ios/Transcriber/Transcriber/ContentView.swift` | ContentView.swift Transcriber  Created by Pete Warden on 1/1/26. | Transcriber | 1 | 0 |
| `examples/ios/Transcriber/Transcriber/TranscriberApp.swift` | TranscriberApp.swift Transcriber  Created by Pete Warden on 1/1/26. | Transcriber | 4 | 0 |
| `examples/ios/Transcriber/TranscriberTests/TranscriberTests.swift` | TranscriberTests.swift TranscriberTests  Created by Pete Warden on 1/1/26. | misc | 1 | 0 |
| `examples/ios/Transcriber/TranscriberUITests/TranscriberUITests.swift` | TranscriberUITests.swift TranscriberUITests  Created by Pete Warden on 1/1/26. | TranscriberUITests | 5 | 0 |
| `examples/ios/Transcriber/TranscriberUITests/TranscriberUITestsLaunchTests.swift` | TranscriberUITestsLaunchTests.swift TranscriberUITests  Created by Pete Warden on 1/1/26. | TranscriberUITests | 3 | 0 |
| `examples/macos/BasicTranscription/Package.swift` | swift-tools-version: 6.1 | misc | 0 | 0 |
| `examples/macos/BasicTranscription/Sources/BasicTranscription/main.swift` | Arguments: MARK: - Command Line Argument Parsing | misc | 9 | 0 |
| `examples/macos/MicTranscription/Package.swift` | swift-tools-version: 6.1 | misc | 0 | 0 |
| `examples/macos/MicTranscription/Sources/MicTranscription/main.swift` | main: MARK: - Main | misc | 5 | 0 |
| `examples/macos/TextToSpeech/Package.swift` | swift-tools-version: 6.1 | misc | 0 | 0 |
| `examples/macos/TextToSpeech/Sources/TextToSpeech/main.swift` | Arguments: MARK: - Command Line Argument Parsing | misc | 7 | 0 |
| `examples/python/basic_transcription.py` | Basic usage example for Moonshine Voice. | python | 6 | 0 |
| `examples/python/dialog_flow.py` | Multi-step dialog flow example using Moonshine Voice. | python | 19 | 0 |
| `examples/python/intent_recognition.py` | Intent recognition example using Moonshine Voice. | python | 13 | 0 |
| `examples/python/mic_transcription.py` | Uses the MicTranscriber class to transcribe audio from a microphone. | python | 8 | 0 |
| `examples/python/ollama-voice/ollama_voice.py` | Example of using the Moonshine Voice library to transcribe speech and send it to an Ollama LLM... | misc | 7 | 0 |
| `examples/raspberry-pi/my-dalek/my-dalek.py` | TranscriptPrinter: Listener that prints transcript updates to the terminal. | misc | 12 | 0 |
| `examples/windows/cli-transcriber/cli-transcriber.cpp` | Helper class to manage COM initialization | misc | 23 | 0 |
| `micro/examples/rp2350/generated/audio_config.h` | AUTO-GENERATED by moonshine-micro/scripts/generate_embedded_data.py DO NOT EDIT. | generated | 1 | 7 |
| `micro/examples/rp2350/generated/classes.cc` | AUTO-GENERATED by moonshine-micro/scripts/generate_embedded_data.py DO NOT EDIT. | generated | 0 | 0 |
| `micro/examples/rp2350/generated/classes.h` | AUTO-GENERATED by moonshine-micro/scripts/generate_embedded_data.py DO NOT EDIT. | generated | 2 | 5 |
| `micro/examples/rp2350/generated/mel_tables.cc` | AUTO-GENERATED by moonshine-micro/scripts/generate_embedded_data.py DO NOT EDIT. | generated | 0 | 0 |
| `micro/examples/rp2350/generated/mel_tables.h` | AUTO-GENERATED by moonshine-micro/scripts/generate_embedded_data.py DO NOT EDIT. | generated | 5 | 6 |
| `micro/examples/rp2350/generated/model_data.cc` | AUTO-GENERATED by moonshine-micro/scripts/generate_embedded_data.py DO NOT EDIT. | generated | 0 | 0 |
| `micro/examples/rp2350/generated/model_data.h` | AUTO-GENERATED by moonshine-micro/scripts/generate_embedded_data.py DO NOT EDIT. | generated | 3 | 4 |
| `micro/examples/rp2350/generated/neural_tts_demo_data.cc` | Auto-generated by scripts/export_pb_demo_data.py; do not edit. | generated | 0 | 0 |
| `micro/examples/rp2350/generated/neural_tts_demo_data.h` | Auto-generated by scripts/export_pb_demo_data.py; do not edit. | generated | 11 | 6 |
| `micro/examples/rp2350/generated/neural_tts_pack.S` | Auto-generated by scripts/export_neural_tts_pack.py; do not edit. | generated | 2 | 0 |
| `micro/examples/rp2350/generated/speaker_test_clips.cc` | AUTO-GENERATED by examples/rp2350/scripts/generate_speaker_test_clips.py DO NOT EDIT. | generated | 0 | 0 |
| `micro/examples/rp2350/generated/speaker_test_clips.h` | AUTO-GENERATED by examples/rp2350/scripts/generate_speaker_test_clips.py DO NOT EDIT. | generated | 3 | 2 |
| `micro/examples/rp2350/generated/test_clips.cc` | AUTO-GENERATED by moonshine-micro/scripts/generate_embedded_data.py DO NOT EDIT. | generated | 0 | 0 |
| `micro/examples/rp2350/generated/test_clips.h` | AUTO-GENERATED by moonshine-micro/scripts/generate_embedded_data.py DO NOT EDIT. | generated | 3 | 2 |
| `micro/examples/rp2350/generated/vad_config.h` | AUTO-GENERATED by moonshine-micro/vad/scripts/generate_vad_embedded_data.py DO NOT EDIT. | generated | 1 | 5 |
| `micro/examples/rp2350/generated/vad_mel_tables.cc` | AUTO-GENERATED by moonshine-micro/scripts/generate_vad_embedded_data.py DO NOT EDIT. | generated | 0 | 0 |
| `micro/examples/rp2350/generated/vad_mel_tables.h` | AUTO-GENERATED by moonshine-micro/scripts/generate_vad_embedded_data.py DO NOT EDIT. | generated | 5 | 5 |
| `micro/examples/rp2350/generated/vad_model_data.cc` | AUTO-GENERATED by moonshine-micro/scripts/generate_vad_embedded_data.py DO NOT EDIT. | generated | 0 | 0 |
| `micro/examples/rp2350/generated/vad_model_data.h` | AUTO-GENERATED by moonshine-micro/scripts/generate_vad_embedded_data.py DO NOT EDIT. | generated | 3 | 3 |
| `micro/examples/rp2350/lwipopts.h` | Minimal lwIP configuration for the voice WiFi-setup app (moonshine_micro_echo_wifi). | misc | 42 | 0 |
| `micro/examples/rp2350/scripts/capture_neural_tts.py` | Capture the neural_tts_test app's USB output: logs + AUDIO frames -> wavs. | micro_examples_rp2350_scripts | 2 | 0 |
| `micro/examples/rp2350/scripts/capture_stt.py` | Capture the exact audio the on-device STT receives, over USB CDC. | micro_examples_rp2350_scripts | 9 | 0 |
| `micro/examples/rp2350/scripts/flash.sh` | Flash a moonshine-micro moonshine_micro_echo*.uf2 to a Raspberry Pi Pico 2 (RP2350) that's been... | micro_examples_rp2350_scripts | 4 | 0 |
| `micro/examples/rp2350/scripts/generate_speaker_test_clips.py` | Embed 1 s int16 PCM clips for the I2S speaker bring-up test. | micro_examples_rp2350_scripts | 3 | 0 |
| `micro/examples/rp2350/scripts/monitor.sh` | Robust USB CDC monitor for the Pico 2 boot log. | micro_examples_rp2350_scripts | 2 | 0 |
| `micro/examples/rp2350/scripts/tts_speak.py` | Speak text on the RP2350 firmware and save the streamed PCM as a WAV. | micro_examples_rp2350_scripts | 3 | 0 |
| `micro/examples/rp2350/scripts/usb_audio_bridge.py` | Bridge the laptop mic + speaker to the RP2350 over USB (audio peripheral sim). | micro_examples_rp2350_scripts | 15 | 0 |
| `micro/examples/rp2350/src/app_common.cc` | - | src | 3 | 0 |
| `micro/examples/rp2350/src/app_common.h` | Shared boot + state for the RP2350 example, used by both app paths: * echo_app -- the live... | src | 7 | 10 |
| `micro/examples/rp2350/src/audio_io.h` | Audio input/output abstraction for the live recognition service. | src | 3 | 5 |
| `micro/examples/rp2350/src/audio_service.cc` | SPELLING_AUDIO_DIAG gates the verbose recognizer diagnostics: per-hop "listening" heartbeats... | src | 12 | 0 |
| `micro/examples/rp2350/src/audio_service.h` | Live USB audio service: turns the laptop into the RP2350's mic + speaker. | src | 8 | 4 |
| `micro/examples/rp2350/src/echo_app.cc` | - | src | 1 | 0 |
| `micro/examples/rp2350/src/echo_app.h` | The default app path: the live mic/speaker recognition service. | src | 1 | 2 |
| `micro/examples/rp2350/src/echo_hardware_app.cc` | - | src | 1 | 0 |
| `micro/examples/rp2350/src/echo_hardware_app.h` | On-board hardware echo service (I2S mic + I2S amp). | src | 1 | 2 |
| `micro/examples/rp2350/src/i2s_audio_io.cc` | CaptureWriteIdx: Current DMA write position as a ring word index (0..kRingWords-1). | src | 5 | 0 |
| `micro/examples/rp2350/src/i2s_audio_io.h` | I2S microphone input for the on-board echo service (SPH0645 / Adafruit 3421). | src | 2 | 4 |
| `micro/examples/rp2350/src/i2s_audio_out.cc` | StereoFrame: Pack one mono int16 sample into a 32-bit stereo I2S frame: MSB-first shift means... | src | 12 | 0 |
| `micro/examples/rp2350/src/i2s_audio_out.h` | I2S speaker output for the on-board echo service (MAX98357A / Adafruit 3006). | src | 9 | 6 |
| `micro/examples/rp2350/src/i2s_mic_process.cc` | - | src | 6 | 0 |
| `micro/examples/rp2350/src/i2s_mic_process.h` | SPH0645 / Adafruit 3421 I2S sample conversion and DC removal. | src | 7 | 4 |
| `micro/examples/rp2350/src/main_audio_loopback_test.cc` | Standalone mic -> speaker loopback test (the `moonshine_micro_audio_loopback_test` target). | src | 3 | 0 |
| `micro/examples/rp2350/src/main_echo_hardware.cc` | Entry point for the on-board hardware echo service (the `moonshine_micro_echo_hardware` target). | src | 1 | 0 |
| `micro/examples/rp2350/src/main_i2s_audio_test.cc` | Standalone speaker / audio-output bring-up test (the `moonshine_micro_i2s_audio_test` target). | src | 11 | 0 |
| `micro/examples/rp2350/src/main_i2s_mic_test.cc` | Standalone I2S microphone bring-up test (the `moonshine_micro_i2s_mic_test` target). | src | 10 | 0 |
| `micro/examples/rp2350/src/main_i2s_relay.cc` | Dumb PCM -> I2S relay (the `moonshine_micro_i2s_relay` target). | src | 6 | 0 |
| `micro/examples/rp2350/src/main_live.cc` | Entry point for the live mic/speaker echo service (the `moonshine_micro_echo` target). | src | 1 | 0 |
| `micro/examples/rp2350/src/main_step1_blinky.cc` | Step 1 of the minimal bring-up ladder: blink the LED, nothing else. | src | 1 | 0 |
| `micro/examples/rp2350/src/main_step1_blinky_w.cc` | Step 1b of the minimal bring-up ladder: blink the LED on a Pico 2 W. | src | 1 | 0 |
| `micro/examples/rp2350/src/main_step2_printf.cc` | Step 2 of the minimal bring-up ladder: blink the LED AND print one line per second over USB CDC. | src | 3 | 0 |
| `micro/examples/rp2350/src/main_step3_fft.cc` | Step 3 of the minimal bring-up ladder: step 2 + heap probe + one kissfft plan + one 1024-point... | src | 3 | 0 |
| `micro/examples/rp2350/src/main_step5_synth.cc` | Step 5 of the minimal bring-up ladder: step 4 + the real WorldLiteSynth (constructor allocates... | src | 4 | 0 |
| `micro/examples/rp2350/src/main_step6_decoder.cc` | Step 6 of the minimal bring-up ladder: step 5 + the TFLM decoder. | src | 7 | 0 |
| `micro/examples/rp2350/src/main_step7_synthesize.cc` | Step 7 of the minimal bring-up ladder: step 6 + full WORLD-lite synthesis of each demo utterance... | src | 10 | 0 |
| `micro/examples/rp2350/src/main_step7b_framesweep.cc` | Step 7b of the minimal bring-up ladder: step 6 + sweep GetFrame through EVERY frame of each... | src | 8 | 0 |
| `micro/examples/rp2350/src/main_step7c_synthonly.cc` | Step 7c of the minimal bring-up ladder: the mirror image of step 7b. | src | 9 | 0 |
| `micro/examples/rp2350/src/main_test.cc` | Entry point for the embedded-clip accuracy sweep (the `moonshine_micro_echo_test` target). | src | 1 | 0 |
| `micro/examples/rp2350/src/main_tflm_invoke_test.cc` | Rung-2 bring-up firmware: banner + TFLM interpreter init + ONE Invoke() of the s16x8 neural-TTS... | src | 11 | 0 |
| `micro/examples/rp2350/src/main_tts.cc` | Entry point for the standalone TTS service (`moonshine_micro_tts`). | src | 4 | 0 |
| `micro/examples/rp2350/src/main_tts_ladder_test.cc` | Incremental bring-up ladder for the neural-TTS stack. | src | 8 | 0 |
| `micro/examples/rp2350/src/main_usb_banner_test.cc` | Minimal USB CDC stdio soak test (the `moonshine_micro_usb_banner_test` target). | src | 2 | 0 |
| `micro/examples/rp2350/src/main_wifi.cc` | Entry point for the voice-driven WiFi setup app (the `moonshine_micro_echo_wifi` target; needs a... | src | 1 | 0 |
| `micro/examples/rp2350/src/main_wifi_hardware.cc` | Entry point for the voice-driven WiFi setup app on the on-board hardware audio I/O (the... | src | 1 | 0 |
| `micro/examples/rp2350/src/op_profiler.cc` | See op_profiler.h for the rationale (why not tflite::MicroProfiler). | src | 4 | 0 |
| `micro/examples/rp2350/src/op_profiler.h` | Lightweight per-op profiler for the moonshine-micro SpellingCNN build. | src | 4 | 2 |
| `micro/examples/rp2350/src/spelling_labels.h` | Spoken "sound-alike" word for each recognized class label, so the readback TTS says "bee" for... | src | 2 | 3 |
| `micro/examples/rp2350/src/test_app.cc` | RunVadDemo: Streaming VAD demo over the embedded clips (each treated as a 1 s stream): one FFT... | src | 2 | 0 |
| `micro/examples/rp2350/src/test_app.h` | The embedded-clip accuracy sweep (the moonshine_micro_echo_test target): run the embedded clip... | src | 1 | 2 |
| `micro/examples/rp2350/src/tts_service.cc` | Flash-resident neural TTS pack (generated/neural_tts_pack.S). | src | 5 | 0 |
| `micro/examples/rp2350/src/tts_service.h` | USB streaming text-to-speech service for the RP2350 firmware. | src | 3 | 3 |
| `micro/examples/rp2350/src/usb_audio_io.cc` | ReadByteTimed: Read one byte, waiting up to ~timeout_ms. | src | 6 | 0 |
| `micro/examples/rp2350/src/usb_audio_io.h` | USB CDC implementation of the AudioInput / AudioOutput interfaces: the laptop acts as the... | src | 3 | 4 |
| `micro/examples/rp2350/src/wifi_app.cc` | Tok: What a recognized class label means during credential entry. | src | 23 | 0 |
| `micro/examples/rp2350/src/wifi_app.h` | Shared voice-driven WiFi setup state machine. | src | 1 | 3 |
| `micro/examples/rp2350/src/wifi_hardware_app.cc` | - | src | 1 | 0 |
| `micro/examples/rp2350/src/wifi_hardware_app.h` | Voice-driven WiFi setup on the on-board hardware audio I/O (I2S mic + I2S amp) instead of the... | src | 1 | 2 |
| `micro/feature-generation/include/feature_generation/feature_generation.h` | feature-generation -- portable, heap-free log-mel spectrogram front-end. | misc | 21 | 5 |
| `micro/feature-generation/scripts/generate_mel_tables.py` | Emit C++ flash tables (periodic Hann window + CSR Slaney mel filterbank) for the... | misc | 8 | 0 |
| `micro/feature-generation/src/fft_scratch.cc` | - | micro_feature-generation_src | 0 | 0 |
| `micro/feature-generation/src/fft_scratch.h` | Shared FFT scratch pool for the on-device log-mel front-ends. | micro_feature-generation_src | 4 | 3 |
| `micro/feature-generation/src/log_mel.cc` | Heap-free log-mel spectrogram for the on-device build. | micro_feature-generation_src | 17 | 0 |
| `micro/feature-generation/src/mel_streamer.cc` | - | micro_feature-generation_src | 4 | 0 |
| `micro/feature-generation/tests/feature_generation_test.cc` | Unit tests for the feature-generation module, using TFLM's micro_test.h. | misc | 7 | 0 |
| `micro/g2p/include/g2p/g2p.h` | English grapheme-to-phoneme front end. | g2p | 1 | 6 |
| `micro/g2p/include/g2p/g2p_dict.h` | Baked common-word pronunciation dictionary + runtime override table. | g2p | 9 | 6 |
| `micro/g2p/include/g2p/g2p_phones.h` | Heap-free phone-token list for on-device TTS (CYW43 leaves little malloc headroom). | g2p | 5 | 2 |
| `micro/g2p/src/g2p.cc` | ResolveToken: Resolve a single token to an IPA string via the lookup pipeline. | micro_g2p_src | 3 | 0 |
| `micro/g2p/src/g2p_dict.cc` | DecodeIpa: Decode `count` packed phone ids starting at body offset `start` into IPA. | micro_g2p_src | 9 | 0 |
| `micro/g2p/src/g2p_dict_data.h` | AUTO-GENERATED by tools/build_g2p_dict.py -- do not edit by hand. | micro_g2p_src | 1 | 1 |
| `micro/g2p/src/g2p_numbers.cc` | - | micro_g2p_src | 7 | 0 |
| `micro/g2p/src/g2p_numbers.h` | English number-token normalization (numeral -> IPA). | micro_g2p_src | 2 | 3 |
| `micro/g2p/src/g2p_phones.cc` | ResolveTokenBuf: Resolve one word token to IPA in `out` (capacity includes NUL). | micro_g2p_src | 5 | 0 |
| `micro/g2p/src/g2p_rules.cc` | - | micro_g2p_src | 15 | 0 |
| `micro/g2p/src/g2p_rules.h` | Rule-based English letter-to-sound (grapheme -> IPA). | micro_g2p_src | 2 | 3 |
| `micro/g2p/src/ipa_tokens.cc` | IPA string -> base-phone token stream (TokenizeIpa). | micro_g2p_src | 4 | 0 |
| `micro/klatt-tts/include/tts/config.h` | Externalized, tunable voice parameters. | tts | 5 | 5 |
| `micro/klatt-tts/include/tts/klatt.h` | Klatt-style cascade formant synthesizer (simplified). | tts | 20 | 3 |
| `micro/klatt-tts/include/tts/phonemes.h` | English phoneme inventory for the formant synthesizer. | tts | 5 | 4 |
| `micro/klatt-tts/include/tts/synth_internal.h` | Shared internals for the batch (synth.cc) and streaming (synth_stream.cc) drivers. | tts | 9 | 3 |
| `micro/klatt-tts/include/tts/synth_stream.h` | Streaming, caller-arena formant synthesizer for the RP2350 (and desktop). | tts | 15 | 2 |
| `micro/klatt-tts/include/tts/tts.h` | tts -- portable, dependency-free formant (Klatt-style) text-to-speech. | tts | 1 | 1 |
| `micro/klatt-tts/src/config.cc` | SetPhoneField: Apply one "<field> <value>" override to a phone. | micro_klatt-tts_src | 7 | 0 |
| `micro/klatt-tts/src/klatt.cc` | GlottalPulse: Rosenberg-style glottal flow pulse as a function of phase in [0, 1). | micro_klatt-tts_src | 11 | 0 |
| `micro/klatt-tts/src/phonemes.cc` | - | micro_klatt-tts_src | 2 | 0 |
| `micro/klatt-tts/src/synth_internal.cc` | AppendStop: Expand a stop into closure -> burst -> (aspiration) sub-segments so that... | micro_klatt-tts_src | 11 | 0 |
| `micro/klatt-tts/src/synth_stream.cc` | SoftClip: Soft limiter: perfectly linear up to a knee (so the RMS body of the signal is... | micro_klatt-tts_src | 9 | 0 |
| `micro/klatt-tts/tests/tts_test.cc` | Unit tests for the TTS synth core, using TFLM's micro_test.h. | misc | 4 | 0 |
| `micro/neural-tts/host/tflm_ref/add.cpp` | Copyright 2021 The TensorFlow Authors. | tflm_ref | 5 | 0 |
| `micro/neural-tts/host/tflm_ref/conv.cpp` | Copyright 2024 The TensorFlow Authors. | tflm_ref | 2 | 0 |
| `micro/neural-tts/host/tflm_ref/host_platform.cpp` | Host (desktop) implementations of the TFLM platform hooks the RP2350 build gets from... | tflm_ref | 3 | 0 |
| `micro/neural-tts/host/tflm_ref/transpose_conv.cpp` | Copyright 2024 The TensorFlow Authors. | tflm_ref | 7 | 0 |
| `micro/neural-tts/host/tts_cli.cc` | Native (desktop) driver for the on-device neural TTS engine. | host | 6 | 0 |
| `micro/neural-tts/host/worldlite_synth_cli.cc` | Host harness for WorldLiteSynth: reads raw [T,61] float32 WORLD-lite controls (f0, benv[48]... | host | 2 | 0 |
| `micro/neural-tts/include/neural_tts/neural_tts.h` | neural_tts -- black-box text-to-speech for the RP2350. | neural_tts | 10 | 5 |
| `micro/neural-tts/include/neural_tts/pack_format.h` | Binary layout of the neural-TTS flash pack, mirroring scripts/export_neural_tts_pack.py (the... | neural_tts | 25 | 1 |
| `micro/neural-tts/include/neural_tts/pb_decoder.h` | TFLM wrapper for the Phase B RVQ decoder (s16x8: int16 activations, int8 weights). | neural_tts | 14 | 6 |
| `micro/neural-tts/include/neural_tts/worldlite_synth.h` | WORLD-lite vocoder synthesis (float32, kissfft) for the RP2350. | neural_tts | 17 | 9 |
| `micro/neural-tts/src/hooks.cc` | Default (no-op) progress hooks. pb_decoder.cc calls tts_checkpoint / tts_trace before every TFLM... | micro_neural-tts_src | 0 | 0 |
| `micro/neural-tts/src/neural_tts.cc` | Black-box neural TTS pipeline (see neural_tts.h). | micro_neural-tts_src | 71 | 0 |
| `micro/neural-tts/src/pb_decoder.cc` | Progress hook (defined by the app): records where the pipeline is for post-reboot hang reports... | micro_neural-tts_src | 16 | 0 |
| `micro/neural-tts/src/worldlite_synth.cc` | Float32 kissfft port of WORLD Synthesis() specialized to the WORLD-lite band parameterization. | micro_neural-tts_src | 17 | 0 |
| `micro/stt-training/config.sh` | Shared configuration for the STT training pipeline. | stt-training | 0 | 0 |
| `micro/stt-training/run_all.sh` | End-to-end pipeline: synthesize -> mine -> extract -> train -> evaluate -> export. | stt-training | 0 | 0 |
| `micro/stt-training/stt_training/__init__.py` | Standalone training recipe for the moonshine-micro on-device word classifier. | stt_training | 0 | 0 |
| `micro/stt-training/stt_training/augment.py` | GPU-resident waveform augmentation, applied before the log-mel front-end. | stt_training | 17 | 1 |
| `micro/stt-training/stt_training/checkpoint.py` | Shared checkpoint loading for export and evaluation. | stt_training | 3 | 2 |
| `micro/stt-training/stt_training/dataset.py` | Speech-Commands-style dataset over local ``<root>/<class>/*.wav`` trees. | stt_training | 14 | 2 |
| `micro/stt-training/stt_training/evaluate.py` | Evaluate a trained checkpoint (and, optionally, the exported int8 .tflite). | stt_training | 3 | 0 |
| `micro/stt-training/stt_training/export.py` | Export a trained WordCNN to the int8 LiteRT format the RP2350 firmware uses. | stt_training | 7 | 1 |
| `micro/stt-training/stt_training/features.py` | Log-mel feature front-end and SpecAugment. | stt_training | 7 | 3 |
| `micro/stt-training/stt_training/model.py` | WordCNN: the compact MobileNetV2-style classifier deployed on the RP2350. | stt_training | 12 | 2 |
| `micro/stt-training/stt_training/train.py` | Train the WordCNN command classifier. | stt_training | 6 | 1 |
| `micro/stt-training/stt_training/words.py` | Vocabulary handling: load ``words.txt`` and turn it into model classes. | stt_training | 3 | 5 |
| `micro/stt-training/tools/download_musan_rirs.py` | Download optional augmentation assets: MUSAN noise + OpenSLR-26 RIRs. | micro_stt-training_tools | 3 | 0 |
| `micro/stt-training/tools/extract_clips.py` | Cut per-word training clips from mined People's Speech utterances. | micro_stt-training_tools | 11 | 0 |
| `micro/stt-training/tools/mine_peoples_speech.py` | Mine People's Speech for command words (and generic "unknown" speech). | micro_stt-training_tools | 16 | 0 |
| `micro/stt-training/tools/synthesize.py` | Synthesize the command vocabulary with Moonshine Voice ZipVoice TTS. | micro_stt-training_tools | 3 | 0 |
| `micro/stt/include/stt/stt.h` | stt -- on-device speech-to-text (isolated-letter/digit) classifier. | misc | 13 | 5 |
| `micro/stt/scripts/desktop_parity.py` | Desktop regression check for the moonshine-micro on-device embedded-clip test loop. | micro_stt_scripts | 5 | 0 |
| `micro/stt/scripts/generate_embedded_data.py` | Generate the compiled-in data blobs for the moonshine-micro Pico build. | micro_stt_scripts | 20 | 2 |
| `micro/stt/src/classifier.cc` | TFLM-based on-device classifier. | micro_stt_src | 3 | 0 |
| `micro/stt/src/predictor.cc` | - | micro_stt_src | 2 | 0 |
| `micro/stt/tests/predictor_test.cc` | Unit tests for the STT prediction helpers, using TFLM's micro_test.h. | misc | 5 | 0 |
| `micro/test-support/host/tflm_host_stub.cc` | Host (desktop) implementations of the handful of TFLM platform hooks that the modules and the... | misc | 5 | 0 |
| `micro/test-support/run_micro_test.sh` | Run a TFLM micro_test.h binary and translate its output into an exit code.  micro_test.h wraps... | misc | 0 | 0 |
| `micro/vad/include/vad/vad.h` | vad -- on-device voice activity detection. | misc | 19 | 5 |
| `micro/vad/scripts/generate_vad_embedded_data.py` | Generate the compiled-in VAD data blobs for the moonshine-micro Pico build. | misc | 6 | 0 |
| `micro/vad/src/vad.cc` | TFLM-based on-device VAD inference. | micro_vad_src | 3 | 0 |
| `micro/vad/src/vad_segmenter.cc` | - | micro_vad_src | 6 | 0 |
| `micro/vad/tests/vad_segmenter_test.cc` | Unit tests for the VAD segmenter, using TFLM's micro_test.h. | misc | 8 | 0 |
| `python/setup.py` | Setup script for moonshine-voice package. | misc | 8 | 0 |
| `python/src/moonshine_voice/__init__.py` | Moonshine Voice - Fast, accurate, on-device AI library for building interactive voice applications. | moonshine_voice | 1 | 0 |
| `python/src/moonshine_voice/alphanumeric_listener.py` | Alphanumeric listener for character-by-character speech-to-text input. | moonshine_voice | 31 | 3 |
| `python/src/moonshine_voice/cached_embeddings.py` | Load pre-computed sentence embeddings from a packaged TSV file. | moonshine_voice | 19 | 2 |
| `python/src/moonshine_voice/cli.py` | Console-script entry point for the ``moonshine-voice`` package. | moonshine_voice | 3 | 1 |

Next: [INDEX_p2.md](INDEX_p2.md)
