# Subsystem: core (page 1 of 3)
Pages: [KB_core.md](KB_core.md), [KB_core_p2.md](KB_core_p2.md), [KB_core_p3.md](KB_core_p3.md)

## core/benchmark.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `AudioProducer` (class, line 11)
  - `AudioProducer` (function, line 13) `public:
  AudioProducer(std::string wav_path, float chunk_duration_seconds = 0.0214f)
      : cur...`
  - `getNextAudio` (function, line 18) `bool getNextAudio(std::vector<float> &out_audio_data)`
  - `sample_rate` (function, line 30) `int32_t sample_rate() const`
  - `audio_data_size` (function, line 31) `size_t audio_data_size() const`
  - `main` (function, line 43) `int main(int argc, char *argv[])`
  - `loadWavData` (function, line 109) `void AudioProducer::loadWavData(std::string wav_path)`
- Depends on: `core/moonshine-cpp.h`, `core/moonshine-utils/file-utils.h`

## core/cosine-distance-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 8) `TEST_CASE("cosine-distance")`
  - `SUBCASE` (function, line 9) `SUBCASE("identical vectors give zero distance")`
  - `SUBCASE` (function, line 15) `SUBCASE("orthogonal vectors give distance one")`
  - `SUBCASE` (function, line 21) `SUBCASE("opposite vectors give distance two")`
  - `SUBCASE` (function, line 27) `SUBCASE("mismatched length throws")`
  - `SUBCASE` (function, line 33) `SUBCASE("zero vector gives zero distance")`
  - `SUBCASE` (function, line 39) `SUBCASE("matches scipy implementation")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 5) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/cosine-distance.h`

## core/cosine-distance.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `cosine_distance` (function, line 6) `float cosine_distance(const std::vector<float>& a,
                      const std::vector<float>...`
- Depends on: `core/cosine-distance.h`

## core/cosine-distance.h
- Doc: Computes cosine distance between two vectors: 1 - (a·b)/(||a||*||b||).
- Layer: utility
- Language: h
- Symbols:
  - `cosine_distance` (function, line 9) `float cosine_distance(const std::vector<float>& a, const std::vector<float>& b);`
  - `COSINE_DISTANCE_H_` (macro, line 2) `#define COSINE_DISTANCE_H_`
- Imported by: `core/cosine-distance-test.cpp`, `core/cosine-distance.cpp`

## core/embedding-model.h
- Doc: EmbeddingModel: Abstract interface for embedding models that convert text to vector representations.
- Layer: business_logic
- Language: h
- Symbols:
  - `EmbeddingModel` (class, line 12)
  - `get_similarity` (function, line 29) `float get_similarity(const std::string &a, const std::string &b)`
  - `get_similarity` (function, line 41) `float get_similarity(const std::string &text,
                       const std::vector<float> &em...`
  - `get_similarity` (function, line 53) `float get_similarity(const std::vector<float> &embedding_a,
                       const std::vec...`
  - `cosine_similarity` (function, line 65) `float cosine_similarity(const std::vector<float> &a,
                          const std::vector<...`
  - `EMBEDDING_MODEL_H` (macro, line 2) `#define EMBEDDING_MODEL_H`
- Imported by: `core/gemma-embedding-model.h`, `core/intent-recognizer.h`

## core/gemma-embedding-model-test.cpp
- Layer: business_logic
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 10) `TEST_CASE("gemma-embedding-model")`
  - `SUBCASE` (function, line 18) `SUBCASE("load model")`
  - `SUBCASE` (function, line 26) `SUBCASE("get embeddings")`
  - `SUBCASE` (function, line 46) `SUBCASE("identical strings have similarity 1.0")`
  - `SUBCASE` (function, line 55) `SUBCASE("similar strings have high similarity")`
  - `SUBCASE` (function, line 67) `SUBCASE("different strings have lower similarity")`
  - `SUBCASE` (function, line 79) `SUBCASE("query and document embeddings")`
  - `SUBCASE` (function, line 99) `SUBCASE("truncate embedding with MRL")`
  - `SUBCASE` (function, line 126) `SUBCASE("config values")`
  - `TEST_CASE` (function, line 138) `TEST_CASE("gemma-embedding-model error handling")`
  - `SUBCASE` (function, line 139) `SUBCASE("load nonexistent model")`
  - `SUBCASE` (function, line 146) `SUBCASE("get embeddings without loading")`
  - `SUBCASE` (function, line 152) `SUBCASE("load invalid variant")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 7) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/gemma-embedding-model.h`

## core/gemma-embedding-model.cpp
- Doc: attention_mask: Create attention mask (all 1s for actual tokens)
- Layer: business_logic
- Language: cpp
- Symbols:
  - `GemmaEmbeddingModel` (function, line 21) `GemmaEmbeddingModel::GemmaEmbeddingModel()
    : ort_api_(nullptr),
      ort_env_(nullptr),
    ...`
  - `load` (function, line 67) `int GemmaEmbeddingModel::load(const char *model_dir,
                              const char *mo...`
  - `load_from_memory` (function, line 111) `int GemmaEmbeddingModel::load_from_memory(const uint8_t *model_data,
                            ...`
  - `load_tokenizer` (function, line 131) `int GemmaEmbeddingModel::load_tokenizer(const char *tokenizer_path)`
  - `load_tokenizer_from_memory` (function, line 142) `int GemmaEmbeddingModel::load_tokenizer_from_memory(const uint8_t *data,
                        ...`
  - `tokenize` (function, line 161) `std::vector<int64_t> GemmaEmbeddingModel::tokenize(const std::string &text)`
  - `run_inference` (function, line 186) `std::vector<float> GemmaEmbeddingModel::run_inference(
    const std::vector<int64_t> &input_ids,...`
  - `get_embeddings` (function, line 298) `std::vector<float> GemmaEmbeddingModel::get_embeddings(
    const std::string &text)`
  - `get_embeddings_with_prefix` (function, line 315) `std::vector<float> GemmaEmbeddingModel::get_embeddings_with_prefix(
    const std::string &text, ...`
  - `get_query_embeddings` (function, line 320) `std::vector<float> GemmaEmbeddingModel::get_query_embeddings(
    const std::string &query)`
  - `get_document_embeddings` (function, line 325) `std::vector<float> GemmaEmbeddingModel::get_document_embeddings(
    const std::string &document)`
  - `truncate_embedding` (function, line 330) `std::vector<float> GemmaEmbeddingModel::truncate_embedding(
    const std::vector<float> &embeddi...`
  - `normalize_embedding` (function, line 346) `void GemmaEmbeddingModel::normalize_embedding(std::vector<float> &embedding)`
  - `is_loaded` (function, line 362) `bool GemmaEmbeddingModel::is_loaded() const`
  - `get_config` (function, line 364) `const GemmaEmbeddingConfig &GemmaEmbeddingModel::get_config() const`
  - `output_shape` (function, line 263) `std::vector<int64_t> output_shape(num_dims);`
  - `embedding` (function, line 288) `std::vector<float> embedding(output_data, output_data + output_size);`
  - `attention_mask` (function, line 309) `std::vector<int64_t> attention_mask(input_ids.size(), 1);`
  - `truncated` (function, line 337) `std::vector<float> truncated(embedding.begin(), embedding.begin() + target_dim);`
  - `DEBUG_ALLOC_ENABLED` (macro, line 17) `#define DEBUG_ALLOC_ENABLED`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/gemma-embedding-model.h`, `core/moonshine-utils/debug-utils.h`, `core/moonshine-utils/string-utils.h`, `core/ort-utils/ort-utils.h`

## core/gemma-embedding-model.h
- Doc: GemmaEmbeddingModel: Gemma Embedding Model implementation using ONNX Runtime C API.
- Layer: business_logic
- Language: h
- Symbols:
  - `GemmaEmbeddingConfig` (struct, line 17)
  - `GemmaEmbeddingModel` (class, line 31)
  - `load` (function, line 51) `int load(const char *model_dir, const char *model_variant = "q4");`
  - `load_from_memory` (function, line 61) `int load_from_memory(const uint8_t *model_data, size_t model_data_size, const uint8_t *tokenizer_data, size_t...`
  - `prefix` (function, line 73) `* Get embeddings with a specific prefix (for query vs document embeddings). * @param text The input text to embed. *...`
  - `embeddings` (function, line 83) `* Get query embeddings (uses query prefix). * @param query The query text. * @return A vector of floats representing...`
  - `truncate_embedding` (function, line 102) `static std::vector<float> truncate_embedding( const std::vector<float> &embedding, int target_dim);`
  - `is_loaded` (function, line 109) `bool is_loaded() const;`
  - `get_config` (function, line 115) `const GemmaEmbeddingConfig &get_config() const;`
  - `load_tokenizer` (function, line 148) `int load_tokenizer(const char *tokenizer_path);`
  - `load_tokenizer_from_memory` (function, line 156) `int load_tokenizer_from_memory(const uint8_t *data, size_t data_size);`
  - `tokenize` (function, line 163) `std::vector<int64_t> tokenize(const std::string &text);`
  - `run_inference` (function, line 171) `std::vector<float> run_inference(const std::vector<int64_t> &input_ids, const std::vector<int64_t> &attention_mask);`
  - `normalize_embedding` (function, line 178) `static void normalize_embedding(std::vector<float> &embedding);`
  - `GEMMA_EMBEDDING_MODEL_H` (macro, line 2) `#define GEMMA_EMBEDDING_MODEL_H`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/embedding-model.h`, `core/ort-utils/moonshine-ort-allocator.h`
- Imported by: `core/gemma-embedding-model-test.cpp`, `core/gemma-embedding-model.cpp`, `core/intent-recognizer-test.cpp`, `core/intent-recognizer.cpp`

## core/intent-recognizer-test.cpp
- Doc: Path to the Gemma embedding model
- Layer: testing
- Language: cpp
- Symbols:
  - `IntentTestCase` (struct, line 111)
  - `PrecisionRecallResult` (struct, line 116)
  - `DiscriminationTest` (struct, line 284)
  - `make_options` (function, line 19) `IntentRecognizerOptions make_options()`
  - `embedding_model_available` (function, line 27) `bool embedding_model_available()`
  - `TEST_CASE` (function, line 31) `TEST_CASE("intent-recognizer unit tests")`
  - `SUBCASE` (function, line 40) `SUBCASE("register and count intents")`
  - `SUBCASE` (function, line 50) `SUBCASE("unregister intent")`
  - `SUBCASE` (function, line 59) `SUBCASE("unregister nonexistent intent")`
  - `SUBCASE` (function, line 64) `SUBCASE("clear intents")`
  - `SUBCASE` (function, line 73) `SUBCASE("rank_intents returns empty for empty utterance")`
  - `SUBCASE` (function, line 78) `SUBCASE("rank_intents sorts by similarity descending and respects max")`
  - `SUBCASE` (function, line 96) `SUBCASE("rank_intents with max_results limit")`
  - `precision` (function, line 122) `float precision() const`
  - `recall` (function, line 127) `float recall() const`
  - `f1_score` (function, line 132) `float f1_score() const`
  - `accuracy` (function, line 138) `float accuracy() const`
  - `TEST_CASE` (function, line 147) `TEST_CASE("intent-recognizer precision/recall with GemmaEmbeddingModel")`
  - `SUBCASE` (function, line 174) `SUBCASE("basic intent matching")`
  - `SUBCASE` (function, line 188) `SUBCASE("precision/recall evaluation")`
  - `SUBCASE` (function, line 283) `SUBCASE("intent discrimination")`
  - `SUBCASE` (function, line 326) `SUBCASE("similarity scores for exact matches")`
  - `TEST_CASE` (function, line 347) `TEST_CASE("intent-recognizer register with pre-computed embedding")`
  - `SUBCASE` (function, line 356) `SUBCASE("register with NULL embedding auto-computes")`
  - `SUBCASE` (function, line 366) `SUBCASE("register with pre-computed embedding")`
  - `SUBCASE` (function, line 380) `SUBCASE("update existing intent preserves count")`
  - `TEST_CASE` (function, line 389) `TEST_CASE("intent-recognizer priority ranking")`
  - `SUBCASE` (function, line 398) `SUBCASE("higher priority intent ranks first regardless of similarity")`
  - `SUBCASE` (function, line 408) `SUBCASE("equal priority falls back to similarity ordering")`
  - `TEST_CASE` (function, line 419) `TEST_CASE("intent-recognizer calculate_embedding")`
  - `SUBCASE` (function, line 428) `SUBCASE("returns non-empty embedding")`
  - `SUBCASE` (function, line 434) `SUBCASE("get_embedding_size returns correct dimension")`
  - `SUBCASE` (function, line 441) `SUBCASE("same text produces same embedding")`
  - `TEST_CASE` (function, line 451) `TEST_CASE("C API intent registration with embedding and priority")`
  - `SUBCASE` (function, line 463) `SUBCASE("register with NULL embedding succeeds")`
  - `SUBCASE` (function, line 469) `SUBCASE("register with nullptr canonical_phrase fails")`
  - `SUBCASE` (function, line 474) `SUBCASE("register multiple intents with different priorities")`
  - `SUBCASE` (function, line 482) `SUBCASE("unregister and clear work")`
  - `TEST_CASE` (function, line 497) `TEST_CASE("C API moonshine_calculate_intent_embedding")`
  - `SUBCASE` (function, line 509) `SUBCASE("basic embedding calculation")`
  - `SUBCASE` (function, line 529) `SUBCASE("null sentence returns error")`
  - `SUBCASE` (function, line 537) `SUBCASE("null out_embedding returns error")`
  - `SUBCASE` (function, line 544) `SUBCASE("null out_embedding_size returns error")`
  - `SUBCASE` (function, line 551) `SUBCASE("invalid handle returns error")`
  - `SUBCASE` (function, line 559) `SUBCASE("round-trip: compute embedding then register with it")`
  - `TEST_CASE` (function, line 589) `TEST_CASE("C API moonshine_free_intent_embedding")`
  - `SUBCASE` (function, line 590) `SUBCASE("safe on nullptr")`
  - `SUBCASE` (function, line 592) `SUBCASE("frees malloc-allocated buffer")`
  - `TEST_CASE` (function, line 599) `TEST_CASE("C API moonshine_calculate_embedding_distance")`
  - `SUBCASE` (function, line 611) `SUBCASE("identical embeddings have similarity ~1.0")`
  - `SUBCASE` (function, line 627) `SUBCASE("similar sentences have high similarity")`
  - `SUBCASE` (function, line 648) `SUBCASE("dissimilar sentences have low similarity")`
  - `SUBCASE` (function, line 669) `SUBCASE("null embedding_a returns error")`
  - `SUBCASE` (function, line 677) `SUBCASE("null embedding_b returns error")`
  - `SUBCASE` (function, line 685) `SUBCASE("null out_similarity returns error")`
  - `SUBCASE` (function, line 692) `SUBCASE("zero embedding_size returns error")`
  - `SUBCASE` (function, line 700) `SUBCASE("invalid handle returns error")`
  - `TEST_CASE` (function, line 711) `TEST_CASE("C API moonshine_get_closest_intents with priority")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 13) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/gemma-embedding-model.h`, `core/intent-recognizer.h`, `core/moonshine-c-api.h`

## core/intent-recognizer.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `RankedEntry` (struct, line 86)
  - `create_embedding_model` (function, line 11) `std::unique_ptr<EmbeddingModel> create_embedding_model(
    const IntentRecognizerOptions &options)`
  - `IntentRecognizer` (function, line 31) `IntentRecognizer::IntentRecognizer(const IntentRecognizerOptions &options)
    : embedding_model_...`
  - `register_intent` (function, line 36) `void IntentRecognizer::register_intent(const std::string &trigger_phrase)`
  - `register_intent` (function, line 40) `void IntentRecognizer::register_intent(const std::string &trigger_phrase,
                       ...`
  - `unregister_intent` (function, line 68) `bool IntentRecognizer::unregister_intent(const std::string &trigger_phrase)`
  - `sort` (function, line 115) `std::sort(entries.begin(), entries.end(), [](const auto &a, const auto &b)`
  - `get_intent_count` (function, line 130) `size_t IntentRecognizer::get_intent_count() const`
  - `clear_intents` (function, line 135) `void IntentRecognizer::clear_intents()`
  - `calculate_embedding` (function, line 140) `std::vector<float> IntentRecognizer::calculate_embedding(
    const std::string &sentence) const`
  - `calculate_similarity` (function, line 146) `float IntentRecognizer::calculate_similarity(
    const std::vector<float> &a, const std::vector<...`
  - `get_embedding_size` (function, line 152) `size_t IntentRecognizer::get_embedding_size() const`
- Depends on: `core/gemma-embedding-model.h`, `core/intent-recognizer.h`

## core/intent-recognizer.h
- Doc: EmbeddingModelArch: Supported embedding model architectures.
- Layer: utility
- Language: h
- Symbols:
  - `IntentRecognizerOptions` (struct, line 23)
  - `Intent` (struct, line 37)
  - `EmbeddingModelArch` (enum, line 16)
  - `EmbeddingModelArch` (class, line 16)
  - `IntentRecognizer` (class, line 48)
  - `register_intent` (function, line 66) `void register_intent(const std::string &trigger_phrase);`
  - `unregister_intent` (function, line 86) `bool unregister_intent(const std::string &trigger_phrase);`
  - `get_intent_count` (function, line 103) `size_t get_intent_count() const;`
  - `clear_intents` (function, line 108) `void clear_intents();`
  - `calculate_embedding` (function, line 115) `std::vector<float> calculate_embedding(const std::string &sentence) const;`
  - `calculate_similarity` (function, line 123) `float calculate_similarity(const std::vector<float> &a, const std::vector<float> &b) const;`
  - `get_embedding_size` (function, line 130) `size_t get_embedding_size() const;`
  - `INTENT_RECOGNIZER_H` (macro, line 2) `#define INTENT_RECOGNIZER_H`
- Depends on: `core/embedding-model.h`
- Imported by: `core/intent-recognizer-test.cpp`, `core/intent-recognizer.cpp`, `core/moonshine-c-api.cpp`

## core/moonshine-c-api-memory-test.cpp
- Doc: Integration test: TTS from memory while CWD is an empty sandbox (no repo data).
- Layer: presentation
- Language: cpp
- Symbols:
  - `read_binary_file` (function, line 34) `std::vector<uint8_t> read_binary_file(const std::filesystem::path& p)`
  - `kokoro_lang_for_voice_stem` (function, line 44) `const char* kokoro_lang_for_voice_stem(std::string_view stem)`
  - `sample_text_for_kokoro_lang` (function, line 79) `const char* sample_text_for_kokoro_lang(const char* lang)`
  - `append_files_under` (function, line 110) `void append_files_under(
    const std::filesystem::path& root, const std::filesystem::path& sub,...`
  - `build_kokoro_g2p_memory_bundle` (function, line 140) `void build_kokoro_g2p_memory_bundle(
    const std::filesystem::path& data_root,
    std::vector<...`
  - `main` (function, line 266) `int main(int argc, char** argv)`
  - `DOCTEST_CONFIG_IMPLEMENT` (macro, line 6) `#define DOCTEST_CONFIG_IMPLEMENT`
- Depends on: `core/moonshine-c-api.h`

## core/moonshine-c-api-test.cpp
- Doc: find_moonshine_tts_data_dir: Resolve ``moonshine-tts/data`` for tests run from ``test-assets/``...
- Layer: presentation
- Language: cpp
- Symbols:
  - `GraphemePhonemizerLangCase` (struct, line 100)
  - `find_de_piper_voices_dir` (function, line 22) `std::filesystem::path find_de_piper_voices_dir()`
  - `read_binary_file` (function, line 37) `std::vector<uint8_t> read_binary_file(const std::filesystem::path& p)`
  - `find_moonshine_tts_data_dir` (function, line 48) `std::optional<std::filesystem::path> find_moonshine_tts_data_dir()`
  - `free_phonemes_output` (function, line 72) `void free_phonemes_output(const char* ipa)`
  - `grapheme_phonemizer_smoke` (function, line 78) `void grapheme_phonemizer_smoke(const std::filesystem::path& data_root,
                          ...`
  - `TEST_CASE` (function, line 110) `TEST_CASE("moonshine-test-v2")`
  - `SUBCASE` (function, line 111) `SUBCASE("transcribe-complete")`
  - `SUBCASE` (function, line 154) `SUBCASE("transcribe-stream")`
  - `SUBCASE` (function, line 247) `SUBCASE("transcribe-complete-from-memory")`
  - `SUBCASE` (function, line 313) `SUBCASE("transcribe-without-streaming-skip-transcription")`
  - `SUBCASE` (function, line 357) `SUBCASE("transcribe-without-streaming-vad-threshold-0")`
  - `SUBCASE` (function, line 407) `SUBCASE("transcribe-valid-options")`
  - `SUBCASE` (function, line 438) `SUBCASE("transcribe-invalid-option")`
  - `SUBCASE` (function, line 451) `SUBCASE("spelling-mode-flag-noop-without-model")`
  - `SUBCASE` (function, line 478) `SUBCASE("spelling-mode-replaces-line-text")`
  - `SUBCASE` (function, line 524) `SUBCASE("tts-synthesizer-valid-options")`
  - `SUBCASE` (function, line 548) `SUBCASE("tts-synthesizer-per-call-speed-kokoro")`
  - `SUBCASE` (function, line 597) `SUBCASE("tts-piper-german-from-memory")`
  - `TEST_CASE` (function, line 657) `TEST_CASE("moonshine-phonemes-to-speech-c-api")`
  - `SUBCASE` (function, line 658) `SUBCASE("invalid-handle")`
  - `SUBCASE` (function, line 667) `SUBCASE("invalid-arguments")`
  - `SUBCASE` (function, line 696) `SUBCASE("kokoro-matches-text-to-speech")`
  - `TEST_CASE` (function, line 784) `TEST_CASE("grapheme-to-phonemizer-c-api")`
  - `SUBCASE` (function, line 785) `SUBCASE("create-invalid-filenames-pointer")`
  - `SUBCASE` (function, line 795) `SUBCASE("text-to-phonemes-invalid-handle")`
  - `SUBCASE` (function, line 802) `SUBCASE("text-to-phonemes-invalid-arguments")`
  - `SUBCASE` (function, line 829) `SUBCASE("rule-based-languages-smoke")`
  - `SUBCASE` (function, line 868) `SUBCASE("chinese-when-onnx-bundle-present")`
  - `SUBCASE` (function, line 885) `SUBCASE("japanese-when-onnx-bundle-present")`
  - `SUBCASE` (function, line 904) `SUBCASE("arabic-when-onnx-bundle-present")`
  - `TEST_CASE` (function, line 923) `TEST_CASE("moonshine-tts-g2p-dependency-api")`
  - `SUBCASE` (function, line 924) `SUBCASE("null-output-pointer")`
  - `SUBCASE` (function, line 933) `SUBCASE("options-count-without-options-pointer")`
  - `SUBCASE` (function, line 943) `SUBCASE("g2p-empty-means-all-languages")`
  - `SUBCASE` (function, line 961) `SUBCASE("g2p-arabic-onnx-model-key-matches-meta-onnx-filename")`
  - `SUBCASE` (function, line 974) `SUBCASE("g2p-french-lists-pos-csv-files-not-directory-prefix")`
  - `SUBCASE` (function, line 988) `SUBCASE("g2p-single-language")`
  - `SUBCASE` (function, line 997) `SUBCASE("g2p-unsupported-language")`
  - `SUBCASE` (function, line 1005) `SUBCASE("g2p-multiple-languages")`
  - `SUBCASE` (function, line 1017) `SUBCASE("g2p-appends-override-key-when-option-set")`
  - `SUBCASE` (function, line 1029) `SUBCASE("tts-json-single-language")`
  - `SUBCASE` (function, line 1044) `SUBCASE("tts-empty-all-languages-json")`
  - `SUBCASE` (function, line 1055) `SUBCASE("tts-unsupported-language")`
  - `SUBCASE` (function, line 1063) `SUBCASE("tts-multiple-languages")`
  - `SUBCASE` (function, line 1076) `SUBCASE("tts-piper-engine-on-en_us")`
  - `SUBCASE` (function, line 1090) `SUBCASE("tts-kokoro-engine-on-fr")`
  - `SUBCASE` (function, line 1104) `SUBCASE("tts-explicit-piper-onnx-map-keys")`
  - `SUBCASE` (function, line 1119) `SUBCASE("tts-piper-voice-selects-onnx-basename")`
  - `SUBCASE` (function, line 1132) `SUBCASE("tts-voices-json-object-en_us")`
  - `SUBCASE` (function, line 1155) `SUBCASE("tts-voices-kokoro-reports-missing-without-assets")`
  - `SUBCASE` (function, line 1169) `SUBCASE("tts-voices-unsupported-language")`
  - `SUBCASE` (function, line 1176) `SUBCASE("tts-voices-piper-de-includes-thorsten-stem")`
  - `SUBCASE` (function, line 1196) `SUBCASE("tts-voices-piper-en_us-includes-saikat-stem")`
  - `SUBCASE` (function, line 1216) `SUBCASE("tts-zipvoice-dependencies")`
  - `SUBCASE` (function, line 1234) `SUBCASE("tts-zipvoice-voices-listing")`
  - `TEST_CASE` (function, line 1253) `TEST_CASE("moonshine-stt-intent-dependency-api")`
  - `SUBCASE` (function, line 1254) `SUBCASE("null-output-pointer")`
  - `SUBCASE` (function, line 1262) `SUBCASE("options-count-without-options-pointer")`
  - `SUBCASE` (function, line 1271) `SUBCASE("stt-empty-language-is-invalid")`
  - `SUBCASE` (function, line 1278) `SUBCASE("stt-english-default-is-medium-streaming")`
  - `SUBCASE` (function, line 1296) `SUBCASE("stt-english-tiny-non-streaming")`
  - `SUBCASE` (function, line 1317) `SUBCASE("stt-non-english-omits-attention-extra")`
  - `SUBCASE` (function, line 1334) `SUBCASE("stt-english-name-lookup")`
  - `SUBCASE` (function, line 1342) `SUBCASE("stt-include-spelling-adds-group-for-english")`
  - `SUBCASE` (function, line 1359) `SUBCASE("stt-include-spelling-noop-for-non-english")`
  - `SUBCASE` (function, line 1373) `SUBCASE("stt-unknown-language")`
  - `SUBCASE` (function, line 1381) `SUBCASE("stt-unknown-arch-for-language")`
  - `SUBCASE` (function, line 1391) `SUBCASE("stt-invalid-arch-value")`
  - `SUBCASE` (function, line 1401) `SUBCASE("intent-default-variant-is-q4")`
  - `SUBCASE` (function, line 1415) `SUBCASE("intent-null-model-name-uses-default")`
  - `SUBCASE` (function, line 1424) `SUBCASE("intent-q8-maps-to-model-quantized")`
  - `SUBCASE` (function, line 1441) `SUBCASE("intent-fp32-uses-bare-model-onnx")`
  - `SUBCASE` (function, line 1455) `SUBCASE("intent-unknown-model")`
  - `SUBCASE` (function, line 1462) `SUBCASE("intent-unknown-variant")`
  - `SUBCASE` (function, line 1498) `SUBCASE("builtin-voice-synthesizes-audio")`
  - `SUBCASE` (function, line 1522) `SUBCASE("user-pcm-with-explicit-transcript")`
  - `csv` (function, line 948) `const std::string csv(out);`
  - `json` (function, line 1034) `const std::string json(out);`
  - `pcm` (function, line 1525) `std::vector<float> pcm(24000, 0.f);`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 17) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-c-api.h`, `core/moonshine-utils/debug-utils.h`, `core/moonshine-utils/string-utils.h`

## core/moonshine-c-api.cpp
- Doc: parse_common_options: Handles common options that are not specific to any particular API.
- Layer: presentation
- Language: cpp
- Symbols:
  - `OptionPair` (type_alias, line 79) `typedef std::pair<std::string, std::string> OptionPair;`
  - `OptionVector` (type_alias, line 81) `typedef std::vector<OptionPair> OptionVector;`
  - `parse_option_vector` (function, line 83) `OptionVector parse_option_vector(const moonshine_option_t *options,
                             ...`
  - `parse_common_options` (function, line 98) `OptionVector parse_common_options(const OptionVector &options)`
  - `parse_transcriber_options` (function, line 110) `void parse_transcriber_options(const OptionVector &options,
                               Transc...`
  - `allocate_transcriber_handle` (function, line 171) `int32_t allocate_transcriber_handle(Transcriber *transcriber)`
  - `free_transcriber_handle` (function, line 178) `void free_transcriber_handle(int32_t handle)`
  - `moonshine_load_transcriber_from_memory` (function, line 240) `int32_t moonshine_load_transcriber_from_memory(
    const uint8_t *encoder_model_data, size_t enc...`
  - `moonshine_free_transcriber` (function, line 291) `void moonshine_free_transcriber(int32_t transcriber_handle)`
  - `moonshine_transcribe_without_streaming` (function, line 299) `int32_t moonshine_transcribe_without_streaming(
    int32_t transcriber_handle, float *audio_data...`
  - `moonshine_create_stream` (function, line 322) `int32_t moonshine_create_stream(int32_t transcriber_handle, uint32_t flags)`
  - `moonshine_free_stream` (function, line 336) `int32_t moonshine_free_stream(int32_t transcriber_handle,
                              int32_t s...`
  - `moonshine_start_stream` (function, line 352) `int32_t moonshine_start_stream(int32_t transcriber_handle,
                               int32_t...`
  - `moonshine_stop_stream` (function, line 368) `int32_t moonshine_stop_stream(int32_t transcriber_handle,
                              int32_t s...`
  - `moonshine_transcript_to_string` (function, line 384) `const char *moonshine_transcript_to_string(
    const struct transcript_t *transcript)`
  - `moonshine_transcribe_add_audio_to_stream` (function, line 394) `int32_t moonshine_transcribe_add_audio_to_stream(int32_t transcriber_handle,
                    ...`
  - `moonshine_transcribe_stream` (function, line 420) `int32_t moonshine_transcribe_stream(int32_t transcriber_handle,
                                 ...`
  - `allocate_intent_recognizer_handle` (function, line 448) `int32_t allocate_intent_recognizer_handle(IntentRecognizer *recognizer)`
  - `free_intent_recognizer_handle` (function, line 455) `void free_intent_recognizer_handle(int32_t handle)`
  - `duplicate_c_string` (function, line 471) `char *duplicate_c_string(const char *s)`
  - `moonshine_create_intent_recognizer` (function, line 485) `int32_t moonshine_create_intent_recognizer(const char *model_path,
                              ...`
  - `moonshine_free_intent_recognizer` (function, line 516) `void moonshine_free_intent_recognizer(int32_t intent_recognizer_handle)`
  - `moonshine_register_intent` (function, line 527) `int32_t moonshine_register_intent(int32_t intent_recognizer_handle,
                             ...`
  - `moonshine_unregister_intent` (function, line 553) `int32_t moonshine_unregister_intent(int32_t intent_recognizer_handle,
                           ...`
  - `moonshine_get_closest_intents` (function, line 578) `int32_t moonshine_get_closest_intents(int32_t intent_recognizer_handle,
                         ...`
  - `moonshine_free_intent_matches` (function, line 636) `void moonshine_free_intent_matches(moonshine_intent_match_t *matches,
                           ...`
  - `moonshine_get_intent_count` (function, line 647) `int32_t moonshine_get_intent_count(int32_t intent_recognizer_handle)`
  - `moonshine_clear_intents` (function, line 659) `int32_t moonshine_clear_intents(int32_t intent_recognizer_handle)`
  - `moonshine_calculate_intent_embedding` (function, line 673) `int32_t moonshine_calculate_intent_embedding(int32_t intent_recognizer_handle,
                  ...`
  - `moonshine_free_intent_embedding` (function, line 714) `void moonshine_free_intent_embedding(float *embedding)`
  - `moonshine_calculate_embedding_distance` (function, line 716) `int32_t moonshine_calculate_embedding_distance(int32_t intent_recognizer_handle,
                ...`
  - `allocate_text_to_speech_synthesizer_handle` (function, line 755) `int32_t allocate_text_to_speech_synthesizer_handle(
    moonshine_tts::MoonshineTTS *synthesizer)`
  - `parse_tts_options` (function, line 763) `void parse_tts_options(const OptionVector &options,
                       moonshine_tts::Moonshi...`
  - `maybe_autotranscribe_zipvoice_clone` (function, line 778) `void maybe_autotranscribe_zipvoice_clone(
    const OptionVector &options,
    moonshine_tts::Moo...`
  - `moonshine_create_tts_synthesizer_from_files` (function, line 870) `int32_t moonshine_create_tts_synthesizer_from_files(
    const char *language, const char **filen...`
  - `moonshine_create_tts_synthesizer_from_memory` (function, line 911) `int32_t moonshine_create_tts_synthesizer_from_memory(
    const char *language, const char **file...`
  - `moonshine_free_tts_synthesizer` (function, line 1000) `void moonshine_free_tts_synthesizer(int32_t tts_synthesizer_handle)`
  - `moonshine_text_to_speech` (function, line 1041) `int32_t moonshine_text_to_speech(int32_t tts_synthesizer_handle,
                                ...`
  - `moonshine_phonemes_to_speech` (function, line 1089) `int32_t moonshine_phonemes_to_speech(int32_t tts_synthesizer_handle,
                            ...`
  - `malloc_string_copy` (function, line 1144) `char *malloc_string_copy(const std::string &s)`
  - `split_comma_nonempty_language_tokens` (function, line 1153) `std::vector<std::string> split_comma_nonempty_language_tokens(const char *s)`
  - `append_unique_in_order` (function, line 1178) `void append_unique_in_order(std::vector<std::string> &acc,
                            const std:...`
  - `json_utf8_string_literal` (function, line 1188) `std::string json_utf8_string_literal(const std::string &s)`
  - `json_flat_string_array` (function, line 1230) `std::string json_flat_string_array(const std::vector<std::string> &items)`
  - `json_model_dependencies` (function, line 1247) `std::string json_model_dependencies(const moonshine::ModelDependencies &deps)`
  - `json_tts_voice_entry` (function, line 1264) `std::string json_tts_voice_entry(
    const moonshine_tts::MoonshineTtsVoiceAvailability &v)`
  - `json_tts_voices_lang_array` (function, line 1274) `std::string json_tts_voices_lang_array(
    const std::vector<moonshine_tts::MoonshineTtsVoiceAva...`
  - `json_tts_voices_root_object` (function, line 1288) `std::string json_tts_voices_root_object(
    const std::vector<std::pair<
        std::string, st...`
  - `apply_g2p_dependency_query_c_options` (function, line 1306) `void apply_g2p_dependency_query_c_options(
    const moonshine_option_t *options, uint64_t option...`
  - `append_g2p_explicit_override_keys_from_c_options` (function, line 1356) `void append_g2p_explicit_override_keys_from_c_options(
    const moonshine_option_t *options, uin...`
  - `moonshine_get_g2p_dependencies` (function, line 1387) `int32_t moonshine_get_g2p_dependencies(const char *languages,
                                   ...`
  - `moonshine_get_tts_dependencies` (function, line 1451) `int32_t moonshine_get_tts_dependencies(const char *languages,
                                   ...`
  - `moonshine_get_tts_voices` (function, line 1548) `int32_t moonshine_get_tts_voices(const char *languages,
                                 const mo...`
  - `normalize_option_key` (function, line 1654) `std::string normalize_option_key(const char *name)`
  - `parse_int_option` (function, line 1662) `std::optional<int32_t> parse_int_option(const std::string &value)`
  - `moonshine_get_stt_dependencies` (function, line 1681) `int32_t moonshine_get_stt_dependencies(const char *language,
                                    ...`
  - `moonshine_get_intent_dependencies` (function, line 1743) `int32_t moonshine_get_intent_dependencies(const char *model_name,
                               ...`
  - `allocate_grapheme_phonemizer_handle` (function, line 1802) `int32_t allocate_grapheme_phonemizer_handle(moonshine_tts::MoonshineG2P *g2p)`
  - `parse_grapheme_phonemizer_options` (function, line 1809) `void parse_grapheme_phonemizer_options(
    const moonshine_option_t *in_options, uint64_t in_opt...`
  - `finalize_g2p_options_for_phonemizer_create` (function, line 1846) `void finalize_g2p_options_for_phonemizer_create(
    moonshine_tts::MoonshineG2POptions &g2p_opt)`
  - `moonshine_create_grapheme_to_phonemizer_from_files` (function, line 1869) `int32_t moonshine_create_grapheme_to_phonemizer_from_files(
    const char *language, const char ...`
  - `moonshine_create_grapheme_to_phonemizer_from_memory` (function, line 1928) `int32_t moonshine_create_grapheme_to_phonemizer_from_memory(
    const char *language, const char...`
  - `moonshine_free_grapheme_to_phonemizer` (function, line 1995) `void moonshine_free_grapheme_to_phonemizer(
    int32_t grapheme_to_phonemizer_handle)`
  - `moonshine_text_to_phonemes` (function, line 2012) `int32_t moonshine_text_to_phonemes(int32_t grapheme_to_phonemizer_handle,
                       ...`
  - `a` (function, line 735) `std::vector<float> a(embedding_a, embedding_a + embedding_size);`
  - `b` (function, line 736) `std::vector<float> b(embedding_b, embedding_b + embedding_size);`
  - `pcm` (function, line 815) `std::vector<float> pcm(n);`
  - `key` (function, line 946) `const std::string key(filenames[i]);`
  - `CHECK_TRANSCRIBER_HANDLE` (macro, line 70) `#define CHECK_TRANSCRIBER_HANDLE(handle)`
  - `CHECK_INTENT_RECOGNIZER_HANDLE` (macro, line 462) `#define CHECK_INTENT_RECOGNIZER_HANDLE(handle)`
  - `CHECK_TTS_SYNTHESIZER_HANDLE` (macro, line 857) `#define CHECK_TTS_SYNTHESIZER_HANDLE(synth_handle)`
  - `CHECK_GRAPHEME_PHONEMIZER_HANDLE` (macro, line 1853) `#define CHECK_GRAPHEME_PHONEMIZER_HANDLE(g2p_handle)`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/intent-recognizer.h`, `core/moonshine-c-api.h`, `core/moonshine-model-catalog.h`, `core/moonshine-model.h`, `core/moonshine-tts/src/moonshine-asset-catalog.h`, `core/moonshine-tts/src/moonshine-g2p.h`, `core/moonshine-tts/src/moonshine-tts.h`, `core/moonshine-utils/debug-utils.h`, `core/moonshine-utils/string-utils.h`, `core/ort-utils/moonshine-ort-allocator.h`, `core/ort-utils/moonshine-tensor-view.h`, `core/ort-utils/ort-utils.h`


Next: [KB_core_p2.md](KB_core_p2.md)
