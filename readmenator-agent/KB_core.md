# Subsystem: core

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
- Layer: infrastructure
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
- Layer: infrastructure
- Language: cpp
- Symbols:
  - `cosine_distance` (function, line 6) `float cosine_distance(const std::vector<float>& a,
                      const std::vector<float>...`
- Depends on: `core/cosine-distance.h`

## core/cosine-distance.h
- Layer: infrastructure
- Doc: Computes cosine distance between two vectors: 1 - (a·b)/(||a||*||b||). Matches scipy.spatial.distance.cdist(..., metric=
- Language: h
- Symbols:
  - `cosine_distance` (function, line 9) `float cosine_distance(const std::vector<float>& a, const std::vector<float>& b);`
  - `COSINE_DISTANCE_H_` (macro, line 2) `#define COSINE_DISTANCE_H_`
- Imported by: `core/cosine-distance-test.cpp`, `core/cosine-distance.cpp`

## core/embedding-model.h
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
- Layer: business_logic
- Language: h
- Symbols:
  - `GemmaEmbeddingConfig` (struct, line 17)
  - `GemmaEmbeddingModel` (class, line 31)
  - `load` (function, line 51) `int load(const char *model_dir, const char *model_variant = "q4");`
  - `load_from_memory` (function, line 61) `int load_from_memory(const uint8_t *model_data, size_t model_data_size, const uint8_t *tokenizer_data, size_t tokenizer_data_size);`
  - `prefix` (function, line 73) `* Get embeddings with a specific prefix (for query vs document embeddings). * @param text The input text to embed. * @param prefix The prefix to prepend (e.g., "task: search result | query: * "). * @r`
  - `embeddings` (function, line 83) `* Get query embeddings (uses query prefix). * @param query The query text. * @return A vector of floats representing the query embedding. */ std::vector<float> get_query_embeddings(const std::string &`
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
- Layer: testing
- Doc: Path to the Gemma embedding model
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
- Layer: presentation
- Doc: Integration test: TTS from memory while CWD is an empty sandbox (no repo data). Usage: moonshine-c-api-memory-test <ABSO
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

## core/moonshine-c-api.h
- Layer: presentation
- Doc: Moonshine is a library for building interactive voice applications. It
- Language: h
- Symbols:
  - `moonshine_option_t` (struct, line 137)
  - `transcript_word_t` (struct, line 194)
  - `speaker_span_t` (struct, line 212)
  - `transcript_line_t` (struct, line 231)
  - `transcript_t` (struct, line 276)
  - `moonshine_intent_match_t` (struct, line 611)
  - `main` (function, line 38) `int main(int argc, char *argv[])`
  - `moonshine_get_version` (function, line 286) `MOONSHINE_EXPORT int32_t moonshine_get_version(void);`
  - `moonshine_error_to_string` (function, line 290) `MOONSHINE_EXPORT const char *moonshine_error_to_string(int32_t error);`
  - `moonshine_transcript_to_string` (function, line 295) `MOONSHINE_EXPORT const char *moonshine_transcript_to_string( const struct transcript_t *transcript);`
  - `moonshine_load_transcriber_from_files` (function, line 357) `MOONSHINE_EXPORT int32_t moonshine_load_transcriber_from_files( const char *path, uint32_t model_arch, const struct moonshine_option_t *options, uint64_t options_count, int32_t moonshine_version);`
  - `moonshine_free_transcriber` (function, line 388) `MOONSHINE_EXPORT void moonshine_free_transcriber(int32_t transcriber_handle);`
  - `moonshine_transcribe_without_streaming` (function, line 425) `MOONSHINE_EXPORT int32_t moonshine_transcribe_without_streaming( int32_t transcriber_handle, float *audio_data, uint64_t audio_length, int32_t sample_rate, uint32_t flags, struct transcript_t **out_tr`
  - `moonshine_create_stream` (function, line 507) `MOONSHINE_EXPORT int32_t moonshine_create_stream(int32_t transcriber_handle, uint32_t flags);`
  - `moonshine_free_stream` (function, line 513) `MOONSHINE_EXPORT int32_t moonshine_free_stream(int32_t transcriber_handle, int32_t stream_handle);`
  - `moonshine_start_stream` (function, line 524) `MOONSHINE_EXPORT int32_t moonshine_start_stream(int32_t transcriber_handle, int32_t stream_handle);`
  - `moonshine_stop_stream` (function, line 531) `MOONSHINE_EXPORT int32_t moonshine_stop_stream(int32_t transcriber_handle, int32_t stream_handle);`
  - `moonshine_transcribe_add_audio_to_stream` (function, line 564) `MOONSHINE_EXPORT int32_t moonshine_transcribe_add_audio_to_stream( int32_t transcriber_handle, int32_t stream_handle, const float *new_audio_data, uint64_t audio_length, int32_t sample_rate, uint32_t `
  - `moonshine_transcribe_stream` (function, line 597) `MOONSHINE_EXPORT int32_t moonshine_transcribe_stream( int32_t transcriber_handle, int32_t stream_handle, uint32_t flags, struct transcript_t **out_transcript);`
  - `moonshine_free_intent_recognizer` (function, line 638) `MOONSHINE_EXPORT void moonshine_free_intent_recognizer( int32_t intent_recognizer_handle);`
  - `moonshine_register_intent` (function, line 652) `MOONSHINE_EXPORT int32_t moonshine_register_intent( int32_t intent_recognizer_handle, const char *canonical_phrase, float *embedding, uint64_t embedding_size, int32_t priority);`
  - `moonshine_unregister_intent` (function, line 659) `MOONSHINE_EXPORT int32_t moonshine_unregister_intent( int32_t intent_recognizer_handle, const char *canonical_phrase);`
  - `moonshine_free_intent_matches` (function, line 685) `MOONSHINE_EXPORT void moonshine_free_intent_matches( struct moonshine_intent_match_t *matches, uint64_t count);`
  - `moonshine_clear_intents` (function, line 698) `MOONSHINE_EXPORT int32_t moonshine_clear_intents(int32_t intent_recognizer_handle);`
  - `moonshine_calculate_intent_embedding` (function, line 708) `MOONSHINE_EXPORT int32_t moonshine_calculate_intent_embedding( int32_t intent_recognizer_handle, const char *sentence, float **out_embedding, uint64_t *out_embedding_size, const char *model_name);`
  - `moonshine_free_intent_embedding` (function, line 715) `MOONSHINE_EXPORT void moonshine_free_intent_embedding(float *embedding);`
  - `moonshine_calculate_embedding_distance` (function, line 725) `MOONSHINE_EXPORT int32_t moonshine_calculate_embedding_distance( int32_t intent_recognizer_handle, const float *embedding_a, const float *embedding_b, uint64_t embedding_size, float *out_similarity);`
  - `moonshine_create_tts_synthesizer_from_memory` (function, line 784) `MOONSHINE_EXPORT int32_t moonshine_create_tts_synthesizer_from_memory( const char *language, const char **filenames, const uint64_t filenames_count, const uint8_t **memory, const uint64_t *memory_size`
  - `moonshine_free_tts_synthesizer` (function, line 793) `MOONSHINE_EXPORT void moonshine_free_tts_synthesizer( int32_t tts_synthesizer_handle);`
  - `moonshine_get_g2p_dependencies` (function, line 813) `MOONSHINE_EXPORT int32_t moonshine_get_g2p_dependencies( const char *languages, const struct moonshine_option_t *options, uint64_t options_count, char **out_dependencies_json);`
  - `moonshine_get_tts_dependencies` (function, line 830) `MOONSHINE_EXPORT int32_t moonshine_get_tts_dependencies( const char *languages, const struct moonshine_option_t *options, uint64_t options_count, char **out_dependencies_json);`
  - `moonshine_get_tts_voices` (function, line 858) `MOONSHINE_EXPORT int32_t moonshine_get_tts_voices( const char *languages, const struct moonshine_option_t *options, uint64_t options_count, char **out_voices_json);`
  - `moonshine_get_stt_dependencies` (function, line 892) `MOONSHINE_EXPORT int32_t moonshine_get_stt_dependencies( const char *language, const struct moonshine_option_t *options, uint64_t options_count, char **out_dependencies_json);`
  - `moonshine_get_intent_dependencies` (function, line 915) `MOONSHINE_EXPORT int32_t moonshine_get_intent_dependencies( const char *model_name, const struct moonshine_option_t *options, uint64_t options_count, char **out_dependencies_json);`
  - `moonshine_text_to_speech` (function, line 929) `MOONSHINE_EXPORT int32_t moonshine_text_to_speech( int32_t tts_synthesizer_handle, const char *text, const struct moonshine_option_t *options, uint64_t options_count, float **out_audio_data, uint64_t `
  - `moonshine_phonemes_to_speech` (function, line 953) `MOONSHINE_EXPORT int32_t moonshine_phonemes_to_speech( int32_t tts_synthesizer_handle, const char *phonemes, const struct moonshine_option_t *options, uint64_t options_count, float **out_audio_data, u`
  - `moonshine_free_grapheme_to_phonemizer` (function, line 1013) `MOONSHINE_EXPORT void moonshine_free_grapheme_to_phonemizer( int32_t grapheme_to_phonemizer_handle);`
  - `moonshine_text_to_phonemes` (function, line 1019) `MOONSHINE_EXPORT int32_t moonshine_text_to_phonemes( int32_t grapheme_to_phonemizer_handle, const char *text, const struct moonshine_option_t *options, uint64_t options_count, const char **out_phoneme`
  - `effect` (variable, line 84) `extern "C" { #endif /* ------------------------------ CONSTANTS -------------------------------- */ /* What version of the Moonshine library the header file is associated with. You should pass this ve`
  - `MOONSHINE_C_API_H` (macro, line 2) `#define MOONSHINE_C_API_H`
  - `MOONSHINE_EXPORT` (macro, line 78) `#define MOONSHINE_EXPORT`
  - `MOONSHINE_EXPORT` (macro, line 80) `#define MOONSHINE_EXPORT`
  - `MOONSHINE_HEADER_VERSION` (macro, line 95) `#define MOONSHINE_HEADER_VERSION`
  - `MOONSHINE_MODEL_ARCH_TINY` (macro, line 98) `#define MOONSHINE_MODEL_ARCH_TINY`
  - `MOONSHINE_MODEL_ARCH_BASE` (macro, line 99) `#define MOONSHINE_MODEL_ARCH_BASE`
  - `MOONSHINE_MODEL_ARCH_TINY_STREAMING` (macro, line 100) `#define MOONSHINE_MODEL_ARCH_TINY_STREAMING`
  - `MOONSHINE_MODEL_ARCH_BASE_STREAMING` (macro, line 101) `#define MOONSHINE_MODEL_ARCH_BASE_STREAMING`
  - `MOONSHINE_MODEL_ARCH_SMALL_STREAMING` (macro, line 102) `#define MOONSHINE_MODEL_ARCH_SMALL_STREAMING`
  - `MOONSHINE_MODEL_ARCH_MEDIUM_STREAMING` (macro, line 103) `#define MOONSHINE_MODEL_ARCH_MEDIUM_STREAMING`
  - `MOONSHINE_ERROR_NONE` (macro, line 106) `#define MOONSHINE_ERROR_NONE`
  - `MOONSHINE_ERROR_UNKNOWN` (macro, line 107) `#define MOONSHINE_ERROR_UNKNOWN`
  - `MOONSHINE_ERROR_INVALID_HANDLE` (macro, line 108) `#define MOONSHINE_ERROR_INVALID_HANDLE`
  - `MOONSHINE_ERROR_INVALID_ARGUMENT` (macro, line 109) `#define MOONSHINE_ERROR_INVALID_ARGUMENT`
  - `MOONSHINE_FLAG_FORCE_UPDATE` (macro, line 112) `#define MOONSHINE_FLAG_FORCE_UPDATE`
  - `MOONSHINE_FLAG_SPELLING_MODE` (macro, line 126) `#define MOONSHINE_FLAG_SPELLING_MODE`
  - `MOONSHINE_EMBEDDING_MODEL_ARCH_GEMMA_300M` (macro, line 604) `#define MOONSHINE_EMBEDDING_MODEL_ARCH_GEMMA_300M`
  - `MOONSHINE_INTENT_MAX_MATCHES` (macro, line 608) `#define MOONSHINE_INTENT_MAX_MATCHES`
- Imported by: `android/moonshine-jni/moonshine-jni.cpp`, `core/intent-recognizer-test.cpp`, `core/moonshine-c-api-memory-test.cpp`, `core/moonshine-c-api-test.cpp`, `core/moonshine-c-api.cpp`, `core/moonshine-cpp.h`, `core/moonshine-download-smoke.cpp`, `core/moonshine-model-catalog.cpp`, `core/moonshine-model.h`, `core/tts-repeated-memory-test.cpp`, `core/word-alignment-benchmark.cpp`, `core/word-alignment-test.cpp`

## core/moonshine-cpp-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `load_wav_data` (function, line 13) `bool load_wav_data(const char *path, float **out_float_data,
                   size_t *out_num_s...`
  - `file_exists` (function, line 132) `bool file_exists(const std::string &path)`
  - `onLineStarted` (function, line 147) `void onLineStarted(const moonshine::LineStarted &) override`
  - `onLineUpdated` (function, line 150) `void onLineUpdated(const moonshine::LineUpdated &) override`
  - `onLineTextChanged` (function, line 153) `void onLineTextChanged(const moonshine::LineTextChanged &) override`
  - `onLineCompleted` (function, line 156) `void onLineCompleted(const moonshine::LineCompleted &) override`
  - `TEST_CASE` (function, line 163) `TEST_CASE("moonshine-cpp-test")`
  - `SUBCASE` (function, line 164) `SUBCASE("transcribe-without-streaming")`
  - `SUBCASE` (function, line 193) `SUBCASE("transcribe-with-streaming")`
  - `SUBCASE` (function, line 288) `SUBCASE("g2p")`
  - `SUBCASE` (function, line 306) `SUBCASE("intent recognizer invalid model path throws")`
  - `SUBCASE` (function, line 312) `SUBCASE("spelling-mode-replaces-line-text-via-cpp-ctor")`
  - `SUBCASE` (function, line 347) `SUBCASE("loadFromMemory-with-spelling-buffer")`
  - `SUBCASE` (function, line 395) `SUBCASE("intent recognizer closest intents when embedding model present")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 7) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-cpp.h`

## core/moonshine-cpp.h
- Layer: utility
- Doc: Moonshine C++ API - Header-only library
- Language: h
- Symbols:
  - `WordTiming` (struct, line 83)
  - `SpeakerSpan` (struct, line 104)
  - `TranscriptLine` (struct, line 139)
  - `Transcript` (struct, line 264)
  - `TtsSynthesisResult` (struct, line 667)
  - `IntentMatch` (struct, line 858)
  - `OptionsBuffer` (struct, line 1181)
  - `ModelArch` (enum, line 66)
  - `EmbeddingModelArch` (enum, line 76)
  - `Type` (enum, line 299)
  - `ModelArch` (class, line 66)
  - `TranscriptEvent` (class, line 296)
  - `LineStarted` (class, line 325)
  - `LineUpdated` (class, line 332)
  - `LineTextChanged` (class, line 339)
  - `LineSpeakersChanged` (class, line 349)
  - `LineCompleted` (class, line 356)
  - `Error` (class, line 363)
  - `TranscriptEventListener` (class, line 385)
  - `Stream` (class, line 421)
  - `Transcriber` (class, line 514)
  - `TextToSpeech` (class, line 702)
  - `GraphemeToPhonemizer` (class, line 800)
  - `IntentRecognizer` (class, line 868)
  - `onLineStarted` (function, line 16) `* public:
 *     void onLineStarted(const moonshine::LineStarted& event) override`
  - `onLineCompleted` (function, line 19) `*     void onLineCompleted(const moonshine::LineCompleted& event) override`
  - `main` (function, line 24) `*
 * int main()`
  - `WordTiming` (function, line 93) `WordTiming() : start(0.0f), end(0.0f), confidence(0.0f)`
  - `WordTiming` (function, line 94) `WordTiming(const std::string &word, float start, float end, float confidence)
      : word(word),...`
  - `SpeakerSpan` (function, line 120) `SpeakerSpan()
      : startTime(0.0f),
        duration(0.0f),
        speakerId(0),
        spea...`
  - `SpeakerSpan` (function, line 127) `SpeakerSpan(float startTime, float duration, uint64_t speakerId,
              uint32_t speakerIn...`
  - `TranscriptLine` (function, line 186) `TranscriptLine()
      : startTime(0.0f),
        duration(0.0f),
        lineId(0),
        isCo...`
  - `TranscriptLine` (function, line 198) `TranscriptLine(const transcript_line_t &line_c)
      : startTime(line_c.start_time),
        dur...`
  - `toString` (function, line 233) `std::string toString() const`
  - `Transcript` (function, line 269) `Transcript()`
  - `Transcript` (function, line 272) `Transcript(const transcript_t *transcript_c)`
  - `toString` (function, line 283) `std::string toString() const`
  - `TranscriptEvent` (function, line 320) `protected:
  TranscriptEvent(const TranscriptLine &line, int32_t streamHandle, Type type)
      :...`
  - `LineStarted` (function, line 327) `public:
  LineStarted(const TranscriptLine &line, int32_t streamHandle)
      : TranscriptEvent(l...`
  - `LineUpdated` (function, line 334) `public:
  LineUpdated(const TranscriptLine &line, int32_t streamHandle)
      : TranscriptEvent(l...`
  - `LineTextChanged` (function, line 341) `public:
  LineTextChanged(const TranscriptLine &line, int32_t streamHandle)
      : TranscriptEve...`
  - `LineSpeakersChanged` (function, line 351) `public:
  LineSpeakersChanged(const TranscriptLine &line, int32_t streamHandle)
      : Transcrip...`
  - `LineCompleted` (function, line 358) `public:
  LineCompleted(const TranscriptLine &line, int32_t streamHandle)
      : TranscriptEvent...`
  - `Error` (function, line 368) `Error(const std::string &errorMessage, int32_t streamHandle)
      : TranscriptEvent(TranscriptLi...`
  - `Error` (function, line 372) `Error(const std::string &errorMessage, const TranscriptLine &line,
        int32_t streamHandle)
...`
  - `onLineStarted` (function, line 390) `virtual void onLineStarted(const LineStarted &)`
  - `onLineUpdated` (function, line 393) `virtual void onLineUpdated(const LineUpdated &)`
  - `onLineTextChanged` (function, line 396) `virtual void onLineTextChanged(const LineTextChanged &)`
  - `onLineSpeakersChanged` (function, line 400) `virtual void onLineSpeakersChanged(const LineSpeakersChanged &)`
  - `onLineCompleted` (function, line 403) `virtual void onLineCompleted(const LineCompleted &)`
  - `onError` (function, line 406) `virtual void onError(const Error &)`
  - `MoonshineException` (function, line 414) `public:
  MoonshineException(const std::string &message)
      : std::runtime_error(message)`
  - `getHandle` (function, line 489) `int32_t getHandle() const`
  - `getHandle` (function, line 641) `int32_t getHandle() const`
  - `Transcriber` (function, line 646) `Transcriber(int32_t handle, ModelArch modelArch, double updateInterval)
      : handle_(handle),
...`
  - `TtsSynthesisResult` (function, line 673) `TtsSynthesisResult() : sampleRateHz(0)`
  - `TtsSynthesisResult` (function, line 674) `TtsSynthesisResult(std::vector<float> samples, int32_t sampleRateHz)
      : samples(std::move(sa...`
  - `getLanguage` (function, line 748) `const std::string &getLanguage() const`
  - `getHandle` (function, line 751) `int32_t getHandle() const`
  - `getLanguage` (function, line 834) `const std::string &getLanguage() const`
  - `getHandle` (function, line 837) `int32_t getHandle() const`
  - `IntentMatch` (function, line 863) `IntentMatch(std::string phrase, float sim)
      : canonicalPhrase(std::move(phrase)), similarity...`
  - `getHandle` (function, line 920) `int32_t getHandle() const`
  - `Stream` (function, line 932) `inline Stream::Stream(Transcriber *transcriber, double updateInterval,
                      uint...`
  - `Stream` (function, line 945) `inline Stream::Stream(Stream &&other)
    : transcriber_(other.transcriber_),
      handle_(other...`
  - `start` (function, line 971) `inline void Stream::start()`
  - `stop` (function, line 975) `inline void Stream::stop()`
  - `addAudio` (function, line 986) `inline void Stream::addAudio(const std::vector<float> &audioData,
                             in...`
  - `updateTranscription` (function, line 1002) `inline Transcript Stream::updateTranscription(uint32_t flags)`
  - `addListener` (function, line 1011) `inline void Stream::addListener(TranscriptEventListener *listener)`
  - `addListener` (function, line 1017) `inline void Stream::addListener(
    std::function<void(const TranscriptEvent &)> listener)`
  - `removeListener` (function, line 1022) `inline void Stream::removeListener(TranscriptEventListener *listener)`
  - `removeListener` (function, line 1028) `inline void Stream::removeListener(
    std::function<void(const TranscriptEvent &)> listener)`
  - `remove_if` (function, line 1034) `std::remove_if(
          functionListeners_.begin(), functionListeners_.end(),
          [&liste...`
  - `removeAllListeners` (function, line 1051) `inline void Stream::removeAllListeners()`
  - `close` (function, line 1056) `inline void Stream::close()`
  - `notifyFromTranscript` (function, line 1064) `inline void Stream::notifyFromTranscript(const Transcript &transcript)`
  - `emit` (function, line 1084) `inline void Stream::emit(const TranscriptEvent &event)`
  - `emitError` (function, line 1168) `inline void Stream::emitError(const std::string &errorMessage)`
  - `buildOptions` (function, line 1187) `inline OptionsBuffer buildOptions(
    const std::string &spellingModelPath,
    const std::vecto...`
  - `Transcriber` (function, line 1214) `inline Transcriber::Transcriber(const std::string &modelPath,
                                Mod...`
  - `Transcriber` (function, line 1226) `inline Transcriber::Transcriber(
    const std::string &modelPath, ModelArch modelArch, double up...`
  - `loadFromMemory` (function, line 1242) `inline Transcriber Transcriber::loadFromMemory(
    const uint8_t *encoderData, size_t encoderDat...`
  - `Transcriber` (function, line 1267) `inline Transcriber::Transcriber(Transcriber &&other)
    : handle_(other.handle_),
      modelPat...`
  - `close` (function, line 1295) `inline void Transcriber::close()`
  - `transcribeWithoutStreaming` (function, line 1303) `inline Transcript Transcriber::transcribeWithoutStreaming(
    const std::vector<float> &audioDat...`
  - `getVersion` (function, line 1318) `inline int32_t Transcriber::getVersion() const`
  - `createStream` (function, line 1322) `inline Stream Transcriber::createStream(double updateInterval, uint32_t flags)`
  - `getDefaultStream` (function, line 1326) `inline Stream &Transcriber::getDefaultStream()`
  - `start` (function, line 1333) `inline void Transcriber::start()`
  - `stop` (function, line 1335) `inline void Transcriber::stop()`
  - `addAudio` (function, line 1341) `inline void Transcriber::addAudio(const std::vector<float> &audioData,
                          ...`
  - `updateTranscription` (function, line 1346) `inline Transcript Transcriber::updateTranscription(uint32_t flags)`
  - `addListener` (function, line 1350) `inline void Transcriber::addListener(TranscriptEventListener *listener)`
  - `addListener` (function, line 1354) `inline void Transcriber::addListener(
    std::function<void(const TranscriptEvent &)> listener)`
  - `removeListener` (function, line 1359) `inline void Transcriber::removeListener(TranscriptEventListener *listener)`
  - `removeListener` (function, line 1365) `inline void Transcriber::removeListener(
    std::function<void(const TranscriptEvent &)> listener)`
  - `removeAllListeners` (function, line 1372) `inline void Transcriber::removeAllListeners()`
  - `parseTranscript` (function, line 1378) `inline Transcript Transcriber::parseTranscript(
    const transcript_t *transcript_c)`
  - `checkError` (function, line 1383) `inline void Transcriber::checkError(int32_t error) const`
  - `checkError` (function, line 1391) `inline void Stream::checkError(int32_t error) const`
  - `TextToSpeech` (function, line 1400) `inline TextToSpeech::TextToSpeech(
    const std::string &language, const std::vector<moonshine_o...`
  - `TextToSpeech` (function, line 1411) `inline TextToSpeech::TextToSpeech(TextToSpeech &&other)
    : handle_(other.handle_), language_(s...`
  - `synthesize` (function, line 1426) `inline TtsSynthesisResult TextToSpeech::synthesize(
    const std::string &text, const std::vecto...`
  - `synthesizeFromPhonemes` (function, line 1446) `inline TtsSynthesisResult TextToSpeech::synthesizeFromPhonemes(
    const std::string &phonemes,
...`
  - `close` (function, line 1467) `inline void TextToSpeech::close()`
  - `getVoices` (function, line 1474) `inline std::string TextToSpeech::getVoices(
    const std::string &languages,
    const std::vect...`
  - `getDependencies` (function, line 1494) `inline std::string TextToSpeech::getDependencies(
    const std::string &languages,
    const std...`
  - `checkError` (function, line 1514) `inline void TextToSpeech::checkError(int32_t error) const`
  - `GraphemeToPhonemizer` (function, line 1523) `inline GraphemeToPhonemizer::GraphemeToPhonemizer(
    const std::string &language, const std::ve...`
  - `GraphemeToPhonemizer` (function, line 1534) `inline GraphemeToPhonemizer::GraphemeToPhonemizer(GraphemeToPhonemizer &&other)
    : handle_(oth...`
  - `toIpa` (function, line 1550) `inline std::string GraphemeToPhonemizer::toIpa(
    const std::string &text, const std::vector<mo...`
  - `close` (function, line 1566) `inline void GraphemeToPhonemizer::close()`
  - `getDependencies` (function, line 1573) `inline std::string GraphemeToPhonemizer::getDependencies(
    const std::string &languages,
    c...`
  - `checkError` (function, line 1593) `inline void GraphemeToPhonemizer::checkError(int32_t error) const`
  - `IntentRecognizer` (function, line 1601) `inline IntentRecognizer::IntentRecognizer(const std::string &model_path,
                        ...`
  - `IntentRecognizer` (function, line 1612) `inline IntentRecognizer::IntentRecognizer(IntentRecognizer &&other) noexcept
    : handle_(other....`
  - `registerIntent` (function, line 1627) `inline void IntentRecognizer::registerIntent(
    const std::string &canonical_phrase, float *emb...`
  - `unregisterIntent` (function, line 1634) `inline bool IntentRecognizer::unregisterIntent(
    const std::string &canonical_phrase)`
  - `getClosestIntents` (function, line 1647) `inline std::vector<IntentMatch> IntentRecognizer::getClosestIntents(
    const std::string &utter...`
  - `intentCount` (function, line 1671) `inline int32_t IntentRecognizer::intentCount() const`
  - `clearIntents` (function, line 1681) `inline void IntentRecognizer::clearIntents()`
  - `calculateEmbedding` (function, line 1685) `inline std::vector<float> IntentRecognizer::calculateEmbedding(
    const std::string &sentence, ...`
  - `close` (function, line 1699) `inline void IntentRecognizer::close()`
  - `checkError` (function, line 1706) `inline void IntentRecognizer::checkError(int32_t error) const`
  - `transcriber` (function, line 25) `* moonshine::Transcriber transcriber("path/to/models", * moonshine::ModelArch::BASE);`
  - `MOONSHINE_CPP_H` (macro, line 2) `#define MOONSHINE_CPP_H`
- Depends on: `core/moonshine-c-api.h`
- Imported by: `core/benchmark.cpp`, `core/moonshine-cpp-test.cpp`, `examples/windows/cli-transcriber/cli-transcriber.cpp`

## core/moonshine-download-smoke.cpp
- Layer: utility
- Doc: moonshine-download-smoke: a tiny CLI used by scripts/test-model-downloads.sh to verify that the native download manifest
- Language: cpp
- Symbols:
  - `print_usage` (function, line 45) `void print_usage()`
  - `url_encode_path` (function, line 53) `std::string url_encode_path(const std::string& key)`
  - `fail` (function, line 73) `int fail(const std::string& message)`
  - `print_group_manifest` (function, line 82) `void print_group_manifest(const std::string& json_text)`
  - `manifest_stt` (function, line 93) `int manifest_stt(const std::vector<std::string>& spec)`
  - `manifest_intent` (function, line 115) `int manifest_intent(const std::vector<std::string>& spec)`
  - `manifest_tts` (function, line 135) `int manifest_tts(const std::vector<std::string>& spec)`
  - `manifest_g2p` (function, line 166) `int manifest_g2p(const std::vector<std::string>& spec)`
  - `load_speech_or_tone` (function, line 197) `std::vector<float> load_speech_or_tone()`
  - `is_streaming_arch` (function, line 234) `bool is_streaming_arch(uint32_t arch)`
  - `run_stt` (function, line 241) `int run_stt(const std::string& root, const std::vector<std::string>& spec)`
  - `run_intent` (function, line 295) `int run_intent(const std::string& root, const std::vector<std::string>& spec)`
  - `run_tts` (function, line 323) `int run_tts(const std::string& root, const std::vector<std::string>& spec)`
  - `run_g2p` (function, line 361) `int run_g2p(const std::string& root, const std::vector<std::string>& spec)`
  - `main` (function, line 388) `int main(int argc, char** argv)`
  - `csv` (function, line 176) `const std::string csv(out);`
  - `audio` (function, line 218) `std::vector<float> audio(data, data + used);`
- Depends on: `core/moonshine-c-api.h`, `core/moonshine-utils/debug-utils.h`

## core/moonshine-model-catalog.cpp
- Layer: business_logic
- Language: cpp
- Symbols:
  - `SttModelEntry` (struct, line 17)
  - `SttLanguageEntry` (struct, line 22)
  - `SpellingModelEntry` (struct, line 28)
  - `EmbeddingModelEntry` (struct, line 33)
  - `to_lower` (function, line 40) `std::string to_lower(std::string s)`
  - `transform` (function, line 41) `std::transform(s.begin(), s.end(), s.begin(), [](unsigned char c)`
  - `is_streaming_arch` (function, line 47) `bool is_streaming_arch(int32_t model_arch)`
  - `stt_catalog` (function, line 56) `const std::vector<SttLanguageEntry>& stt_catalog()`
  - `embedding_catalog` (function, line 123) `const std::vector<EmbeddingModelEntry>& embedding_catalog()`
  - `find_stt_language` (function, line 133) `const SttLanguageEntry* find_stt_language(const std::string& language)`
  - `stt_component_files` (function, line 148) `std::vector<std::string> stt_component_files(const std::string& language_code,
                  ...`
  - `find_spelling_model` (function, line 170) `const SpellingModelEntry* find_spelling_model(const std::string& language_code)`
  - `find_embedding_model` (function, line 179) `const EmbeddingModelEntry* find_embedding_model(const std::string& model_name)`
  - `embedding_component_files` (function, line 194) `std::vector<std::string> embedding_component_files(const std::string& variant)`
  - `stt_model_dependencies` (function, line 214) `std::optional<ModelDependencies> stt_model_dependencies(
    const std::string& language, std::op...`
  - `intent_model_dependencies` (function, line 251) `std::optional<ModelDependencies> intent_model_dependencies(
    const std::string& model_name, co...`
  - `stt_supported_languages` (function, line 273) `std::vector<std::string> stt_supported_languages()`
  - `intent_supported_models` (function, line 281) `std::vector<std::string> intent_supported_models()`
  - `intent_supported_variants` (function, line 289) `std::vector<std::string> intent_supported_variants(
    const std::string& model_name)`
- Depends on: `core/moonshine-c-api.h`, `core/moonshine-model-catalog.h`

## core/moonshine-model-catalog.h
- Layer: business_logic
- Doc: Native catalog of downloadable model assets (speech-to-text transcription, the optional alphanumeric spelling model, and
- Language: h
- Symbols:
  - `ModelDependencyGroup` (struct, line 24)
  - `ModelDependencies` (struct, line 29)
  - `MOONSHINE_MODEL_CATALOG_H` (macro, line 2) `#define MOONSHINE_MODEL_CATALOG_H`
- Imported by: `core/moonshine-c-api.cpp`, `core/moonshine-model-catalog.cpp`

## core/moonshine-model.cpp
- Layer: business_logic
- Language: cpp
- Symbols:
  - `set_model_options_from_arch` (function, line 60) `int set_model_options_from_arch(MoonshineModel *model, int32_t model_arch)`
  - `MoonshineModel` (function, line 82) `MoonshineModel::MoonshineModel(
    bool log_ort_run, float max_tokens_per_second,
    const std:...`
  - `load` (function, line 145) `int MoonshineModel::load(const char *encoder_model_path,
                         const char *dec...`
  - `load_from_memory` (function, line 163) `int MoonshineModel::load_from_memory(const uint8_t *encoder_model_data,
                         ...`
  - `load_from_assets` (function, line 186) `int MoonshineModel::load_from_assets(const char *encoder_model_path,
                            ...`
  - `transcribe` (function, line 216) `int MoonshineModel::transcribe(const float *input_audio_data,
                               size...`
  - `transcribe_wav` (function, line 565) `int MoonshineModel::transcribe_wav(const char *wav_path, char **out_text)`
  - `load_alignment_model` (function, line 580) `int MoonshineModel::load_alignment_model(const char *alignment_model_path)`
  - `compute_word_timestamps` (function, line 591) `int MoonshineModel::compute_word_timestamps(
    float audio_duration, std::vector<TranscriberWor...`
  - `encoder_input_names` (function, line 231) `std::vector<char *> encoder_input_names(encoder_input_count);`
  - `encoder_output_names` (function, line 232) `std::vector<char *> encoder_output_names(encoder_output_count);`
  - `encoder_outputs` (function, line 268) `std::vector<OrtValue *> encoder_outputs(encoder_output_count);`
  - `decoder_input_names` (function, line 326) `std::vector<const char *> decoder_input_names(decoder_input_count);`
  - `decoder_output_names` (function, line 338) `std::vector<const char *> decoder_output_names(decoder_output_count);`
  - `decoder_inputs_data` (function, line 382) `std::vector<MoonshineTensorView *> decoder_inputs_data(decoder_input_count);`
  - `decoder_outputs` (function, line 442) `std::vector<OrtValue *> decoder_outputs(decoder_output_count);`
  - `tokens_int` (function, line 601) `std::vector<int> tokens_int(last_tokens.begin(), last_tokens.end());`
  - `rearranged` (function, line 613) `std::vector<float> rearranged(L * H * total_steps * E);`
  - `output_names_alloc` (function, line 679) `std::vector<char *> output_names_alloc(align_output_count);`
  - `output_names` (function, line 686) `std::vector<const char *> output_names(align_output_count);`
  - `outputs` (function, line 692) `std::vector<OrtValue *> outputs(align_output_count, nullptr);`
  - `attn_shape` (function, line 732) `std::vector<int64_t> attn_shape(attn_ndims);`
  - `cross_attention_data` (function, line 744) `std::vector<float> cross_attention_data(attn_layers * per_layer);`
  - `DEBUG_ALLOC_ENABLED` (macro, line 36) `#define DEBUG_ALLOC_ENABLED`
  - `MOONSHINE_TINY_NUM_LAYERS` (macro, line 41) `#define MOONSHINE_TINY_NUM_LAYERS`
  - `MOONSHINE_TINY_NUM_KV_HEADS` (macro, line 42) `#define MOONSHINE_TINY_NUM_KV_HEADS`
  - `MOONSHINE_TINY_HEAD_DIM` (macro, line 43) `#define MOONSHINE_TINY_HEAD_DIM`
  - `MOONSHINE_TINY_PAST_ELEMENT_COUNT` (macro, line 45) `#define MOONSHINE_TINY_PAST_ELEMENT_COUNT`
  - `MOONSHINE_BASE_NUM_LAYERS` (macro, line 49) `#define MOONSHINE_BASE_NUM_LAYERS`
  - `MOONSHINE_BASE_NUM_KV_HEADS` (macro, line 50) `#define MOONSHINE_BASE_NUM_KV_HEADS`
  - `MOONSHINE_BASE_HEAD_DIM` (macro, line 51) `#define MOONSHINE_BASE_HEAD_DIM`
  - `MOONSHINE_BASE_PAST_ELEMENT_COUNT` (macro, line 53) `#define MOONSHINE_BASE_PAST_ELEMENT_COUNT`
  - `MOONSHINE_DECODER_START_TOKEN_ID` (macro, line 56) `#define MOONSHINE_DECODER_START_TOKEN_ID`
  - `MOONSHINE_EOS_TOKEN_ID` (macro, line 57) `#define MOONSHINE_EOS_TOKEN_ID`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/moonshine-model.h`, `core/moonshine-utils/debug-utils.h`, `core/moonshine-utils/string-utils.h`, `core/ort-utils/moonshine-ort-allocator.h`, `core/ort-utils/moonshine-tensor-view.h`, `core/ort-utils/ort-utils.h`

## core/moonshine-model.h
- Layer: business_logic
- Language: h
- Symbols:
  - `MoonshineModel` (struct, line 17)
  - `load` (function, line 72) `int load(const char *encoder_model_path, const char *decoder_model_path, const char *tokenizer_path, int32_t model_type);`
  - `load_alignment_model` (function, line 75) `int load_alignment_model(const char *alignment_model_path);`
  - `load_from_memory` (function, line 77) `int load_from_memory(const uint8_t *encoder_model_data, size_t encoder_model_data_size, const uint8_t *decoder_model_data, size_t decoder_model_data_size, const uint8_t *tokenizer_data, size_t tokeniz`
  - `load_from_assets` (function, line 85) `int load_from_assets(const char *encoder_model_path, const char *decoder_model_path, const char *tokenizer_path, int32_t model_type, AAssetManager *assetManager);`
  - `transcribe` (function, line 91) `int transcribe(const float *input_audio_data, size_t input_audio_data_size, char **out_text);`
  - `transcribe_wav` (function, line 94) `int transcribe_wav(const char *wav_path, char **out_text);`
  - `compute_word_timestamps` (function, line 101) `int compute_word_timestamps(float audio_duration, std::vector<TranscriberWord> &words_out);`
  - `MOONSHINE_MODEL_H` (macro, line 2) `#define MOONSHINE_MODEL_H`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/moonshine-c-api.h`, `core/ort-utils/moonshine-ort-allocator.h`, `core/word-alignment.h`
- Imported by: `core/moonshine-c-api.cpp`, `core/moonshine-model.cpp`

## core/moonshine-streaming-model.cpp
- Layer: business_logic
- Doc: Streaming model constants
- Language: cpp
- Symbols:
  - `read_file_to_string` (function, line 49) `static std::string read_file_to_string(const std::string &path)`
  - `parse_config_json` (function, line 58) `static bool parse_config_json(const std::string &json,
                              MoonshineStr...`
  - `reset` (function, line 107) `void MoonshineStreamingState::reset(const MoonshineStreamingConfig &cfg)`
  - `MoonshineStreamingModel` (function, line 146) `MoonshineStreamingModel::MoonshineStreamingModel(
    bool log_ort_run, const std::vector<std::st...`
  - `load_config` (function, line 200) `int MoonshineStreamingModel::load_config(const char *config_path)`
  - `load_config_from_string` (function, line 209) `int MoonshineStreamingModel::load_config_from_string(const std::string &json)`
  - `load` (function, line 217) `int MoonshineStreamingModel::load(const char *model_dir,
                                  const ...`
  - `load_from_memory` (function, line 290) `int MoonshineStreamingModel::load_from_memory(
    const uint8_t *frontend_model_data, size_t fro...`
  - `load_from_assets` (function, line 332) `int MoonshineStreamingModel::load_from_assets(const char *model_dir,
                            ...`
  - `create_state` (function, line 405) `MoonshineStreamingState *MoonshineStreamingModel::create_state()`
  - `tokens_to_text` (function, line 411) `std::string MoonshineStreamingModel::tokens_to_text(
    const std::vector<int64_t> &tokens)`
  - `process_audio_chunk` (function, line 421) `int MoonshineStreamingModel::process_audio_chunk(MoonshineStreamingState *state,
                ...`
  - `encode` (function, line 584) `int MoonshineStreamingModel::encode(MoonshineStreamingState *state,
                             ...`
  - `compute_cross_kv` (function, line 759) `int MoonshineStreamingModel::compute_cross_kv(MoonshineStreamingState *state)`
  - `run_decoder_with_cross_kv` (function, line 847) `int MoonshineStreamingModel::run_decoder_with_cross_kv(
    MoonshineStreamingState *state, const...`
  - `decode_step` (function, line 1069) `int MoonshineStreamingModel::decode_step(MoonshineStreamingState *state,
                        ...`
  - `decode_tokens` (function, line 1116) `int MoonshineStreamingModel::decode_tokens(MoonshineStreamingState *state,
                      ...`
  - `decode_full` (function, line 1172) `int MoonshineStreamingModel::decode_full(MoonshineStreamingState *state,
                        ...`
  - `decoder_reset` (function, line 1344) `void MoonshineStreamingModel::decoder_reset(MoonshineStreamingState *state)`
  - `audio_vec` (function, line 442) `std::vector<float> audio_vec(audio_chunk, audio_chunk + chunk_len);`
  - `feat_shape` (function, line 529) `std::vector<int64_t> feat_shape(num_dims);`
  - `enc_shape` (function, line 667) `std::vector<int64_t> enc_shape(num_dims);`
  - `new_encoded` (function, line 686) `std::vector<float> new_encoded(new_frames * config.encoder_dim);`
  - `k_shape` (function, line 803) `std::vector<int64_t> k_shape(num_dims);`
  - `token_data` (function, line 865) `std::vector<int64_t> token_data(tokens.begin(), tokens.end());`
  - `output_names_alloc` (function, line 932) `std::vector<char *> output_names_alloc(decoder_output_count);`
  - `outputs` (function, line 945) `std::vector<OrtValue *> outputs(decoder_output_count, nullptr);`
  - `attn_shape` (function, line 1022) `std::vector<int64_t> attn_shape(attn_ndims);`
  - `token_vec` (function, line 1138) `std::vector<int64_t> token_vec(tokens_len);`
  - `DEBUG_ALLOC_ENABLED` (macro, line 24) `#define DEBUG_ALLOC_ENABLED`
  - `MOONSHINE_STREAMING_TINY_ENCODER_DIM` (macro, line 29) `#define MOONSHINE_STREAMING_TINY_ENCODER_DIM`
  - `MOONSHINE_STREAMING_TINY_DECODER_DIM` (macro, line 30) `#define MOONSHINE_STREAMING_TINY_DECODER_DIM`
  - `MOONSHINE_STREAMING_TINY_DEPTH` (macro, line 31) `#define MOONSHINE_STREAMING_TINY_DEPTH`
  - `MOONSHINE_STREAMING_TINY_NHEADS` (macro, line 32) `#define MOONSHINE_STREAMING_TINY_NHEADS`
  - `MOONSHINE_STREAMING_TINY_HEAD_DIM` (macro, line 33) `#define MOONSHINE_STREAMING_TINY_HEAD_DIM`
  - `MOONSHINE_STREAMING_BASE_ENCODER_DIM` (macro, line 35) `#define MOONSHINE_STREAMING_BASE_ENCODER_DIM`
  - `MOONSHINE_STREAMING_BASE_DECODER_DIM` (macro, line 36) `#define MOONSHINE_STREAMING_BASE_DECODER_DIM`
  - `MOONSHINE_STREAMING_BASE_DEPTH` (macro, line 37) `#define MOONSHINE_STREAMING_BASE_DEPTH`
  - `MOONSHINE_STREAMING_BASE_NHEADS` (macro, line 38) `#define MOONSHINE_STREAMING_BASE_NHEADS`
  - `MOONSHINE_STREAMING_BASE_HEAD_DIM` (macro, line 39) `#define MOONSHINE_STREAMING_BASE_HEAD_DIM`
  - `MOONSHINE_DECODER_START_TOKEN_ID` (macro, line 41) `#define MOONSHINE_DECODER_START_TOKEN_ID`
  - `MOONSHINE_EOS_TOKEN_ID` (macro, line 42) `#define MOONSHINE_EOS_TOKEN_ID`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/moonshine-streaming-model.h`, `core/moonshine-utils/debug-utils.h`, `core/moonshine-utils/string-utils.h`, `core/ort-utils/moonshine-ort-allocator.h`, `core/ort-utils/ort-utils.h`

## core/moonshine-streaming-model.h
- Layer: business_logic
- Doc: Streaming model configuration (matches streaming_config.json)
- Language: h
- Symbols:
  - `MoonshineStreamingConfig` (struct, line 17)
  - `MoonshineStreamingState` (struct, line 35)
  - `MoonshineStreamingModel` (struct, line 72)
  - `reset` (function, line 69) `void reset(const MoonshineStreamingConfig &cfg);`
  - `load` (function, line 117) `int load(const char *model_dir, const char *tokenizer_path, int32_t model_type);`
  - `load_from_memory` (function, line 120) `int load_from_memory( const uint8_t *frontend_model_data, size_t frontend_model_data_size, const uint8_t *encoder_model_data, size_t encoder_model_data_size, const uint8_t *adapter_model_data, size_t `
  - `load_from_assets` (function, line 130) `int load_from_assets(const char *model_dir, const char *tokenizer_path, int32_t model_type, AAssetManager *assetManager);`
  - `transcribe` (function, line 135) `int transcribe(const float *input_audio_data, size_t input_audio_data_size, char **out_text);`
  - `process_audio_chunk` (function, line 139) `int process_audio_chunk(MoonshineStreamingState *state, const float *audio_chunk, size_t chunk_len, int *features_out);`
  - `encode` (function, line 143) `int encode(MoonshineStreamingState *state, bool is_final, int *new_frames_out);`
  - `decode_step` (function, line 147) `int decode_step(MoonshineStreamingState *state, int token, float *logits_out);`
  - `decode_full` (function, line 161) `int decode_full(MoonshineStreamingState *state, const int *speculative_tokens, int speculative_len, int **tokens_out, int *tokens_len_out);`
  - `decoder_reset` (function, line 164) `void decoder_reset(MoonshineStreamingState *state);`
  - `create_state` (function, line 167) `MoonshineStreamingState *create_state();`
  - `load_config` (function, line 173) `private: int load_config(const char *config_path);`
  - `load_config_from_string` (function, line 174) `int load_config_from_string(const std::string &json);`
  - `run_decoder_with_cross_kv` (function, line 177) `int run_decoder_with_cross_kv(MoonshineStreamingState *state, const std::vector<int64_t> &tokens, std::vector<float> &logits_out);`
  - `compute_cross_kv` (function, line 182) `int compute_cross_kv(MoonshineStreamingState *state);`
  - `MOONSHINE_STREAMING_MODEL_H` (macro, line 2) `#define MOONSHINE_STREAMING_MODEL_H`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/ort-utils/moonshine-ort-allocator.h`, `core/word-alignment.h`
- Imported by: `core/moonshine-streaming-model.cpp`

## core/resampler-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `test_resample_audio` (function, line 13) `void test_resample_audio(const std::vector<float> &input_audio,
                         int32_t ...`
  - `TEST_CASE` (function, line 44) `TEST_CASE("resampler-test")`
  - `SUBCASE` (function, line 45) `SUBCASE("resample-audio")`
  - `max_element` (function, line 20) `*std::max_element(input_audio.begin(), input_audio.end());`
  - `min_element` (function, line 27) `*std::min_element(input_audio.begin(), input_audio.end());`
  - `wav_data_vector` (function, line 55) `const std::vector<float> wav_data_vector(wav_data, wav_data + wav_data_size);`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 9) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-utils/debug-utils.h`, `core/resampler.h`

## core/resampler.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `resample_audio` (function, line 5) `const std::vector<float> resample_audio(const std::vector<float> &audio,
                        ...`
  - `downsample_audio` (function, line 17) `const std::vector<float> downsample_audio(const std::vector<float> &audio,
                      ...`
  - `upsample_audio` (function, line 56) `const std::vector<float> upsample_audio(const std::vector<float> &audio,
                        ...`
  - `output_audio` (function, line 23) `std::vector<float> output_audio(output_audio_size);`
- Depends on: `core/moonshine-utils/debug-utils.h`, `core/resampler.h`

## core/resampler.h
- Layer: utility
- Language: h
- Symbols:
  - `resample_audio` (function, line 6) `const std::vector<float> resample_audio(const std::vector<float> &audio, float input_sample_rate, float output_sample_rate);`
  - `downsample_audio` (function, line 10) `const std::vector<float> downsample_audio(const std::vector<float> &audio, float input_sample_rate, float output_sample_rate);`
  - `upsample_audio` (function, line 14) `const std::vector<float> upsample_audio(const std::vector<float> &audio, float input_sample_rate, float output_sample_rate);`
  - `RESAMPLER_H` (macro, line 2) `#define RESAMPLER_H`
- Imported by: `core/reliability/fuzz-resampler.cpp`, `core/resampler-test.cpp`, `core/resampler.cpp`, `core/voice-activity-detector.cpp`

## core/silero-vad.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `init_onnx_env` (function, line 6) `void SileroVad::init_onnx_env()`
  - `init_engine_threads` (function, line 21) `void SileroVad::init_engine_threads(int inter_threads, int intra_threads)`
  - `SileroVad` (function, line 30) `SileroVad::SileroVad(int sample_rate, int windows_frame_size, float threshold,
                  ...`
  - `load_from_memory` (function, line 60) `int SileroVad::load_from_memory(const uint8_t *model_data,
                                size_t...`
  - `predict` (function, line 78) `void SileroVad::predict(const std::vector<float> &data_chunk,
                        float *out_...`
- Depends on: `core/ort-utils/ort-utils.h`, `core/silero-vad.h`

## core/silero-vad.h
- Layer: utility
- Language: h
- Symbols:
  - `SileroVad` (class, line 22)
  - `is_loaded` (function, line 85) `bool is_loaded() const`
  - `init_onnx_env` (function, line 68) `void init_onnx_env();`
  - `init_engine_threads` (function, line 71) `void init_engine_threads(int inter_threads, int intra_threads);`
  - `load_from_memory` (function, line 83) `int load_from_memory(const uint8_t *model_data, size_t model_data_size);`
  - `predict` (function, line 87) `void predict(const std::vector<float> &data_chunk, float *out_probability, int *out_flag);`
- Imported by: `core/silero-vad.cpp`, `core/voice-activity-detector.h`

## core/speaker-diarizer.cpp
- Layer: infrastructure
- Language: cpp
- Symbols:
  - `StreamState` (struct, line 43)
  - `turn_overlap_seconds` (function, line 17) `double turn_overlap_seconds(
    const std::vector<cppannote::StreamingDiarizationTurn> &a, int32...`
  - `Impl` (function, line 67) `explicit Impl(const SpeakerDiarizerOptions &options_in)
      : engine(), options(options_in)`
  - `session_config` (function, line 75) `cppannote::StreamingDiarizationConfig session_config() const`
  - `get_stream` (function, line 83) `StreamState &get_stream(int32_t stream_id)`
  - `allocate_stable_id` (function, line 92) `uint64_t allocate_stable_id()`
  - `map_snapshot_to_stable_ids` (function, line 102) `void map_snapshot_to_stable_ids(
      StreamState &state,
      const cppannote::StreamingDiariz...`
  - `sort` (function, line 135) `std::sort(candidates.begin(), candidates.end(),
              [](const auto &a, const auto &b)`
  - `SpeakerDiarizer` (function, line 171) `SpeakerDiarizer::SpeakerDiarizer(const SpeakerDiarizerOptions &options)
    : impl(std::make_uniq...`
  - `create_stream` (function, line 176) `int32_t SpeakerDiarizer::create_stream()`
  - `free_stream` (function, line 186) `void SpeakerDiarizer::free_stream(int32_t stream_id)`
  - `start_stream` (function, line 191) `void SpeakerDiarizer::start_stream(int32_t stream_id)`
  - `add_audio_to_stream` (function, line 201) `void SpeakerDiarizer::add_audio_to_stream(int32_t stream_id,
                                    ...`
  - `get_turns` (function, line 218) `std::vector<SpeakerTurn> SpeakerDiarizer::get_turns(int32_t stream_id)`
  - `finish_stream` (function, line 225) `std::vector<SpeakerTurn> SpeakerDiarizer::finish_stream(int32_t stream_id)`
  - `diarize` (function, line 236) `std::vector<SpeakerTurn> SpeakerDiarizer::diarize(const float *audio_data,
                      ...`
- Depends on: `core/cpp-annote/src/cpp-annote-engine.h`, `core/cpp-annote/src/cpp-annote-streaming.h`, `core/moonshine-utils/debug-utils.h`, `core/speaker-diarizer.h`

## core/speaker-diarizer.h
- Layer: infrastructure
- Doc: One contiguous span of speech attributed to a single speaker on the stream timeline.
- Language: h
- Symbols:
  - `SpeakerTurn` (struct, line 10)
  - `SpeakerDiarizerOptions` (struct, line 24)
  - `Impl` (struct, line 74)
  - `SpeakerDiarizer` (class, line 42)
  - `create_stream` (function, line 51) `int32_t create_stream();`
  - `free_stream` (function, line 52) `void free_stream(int32_t stream_id);`
  - `start_stream` (function, line 53) `void start_stream(int32_t stream_id);`
  - `add_audio_to_stream` (function, line 58) `void add_audio_to_stream(int32_t stream_id, const float *audio_data, uint64_t audio_length, int32_t sample_rate);`
  - `SPEAKER_DIARIZER_H` (macro, line 2) `#define SPEAKER_DIARIZER_H`
- Imported by: `core/speaker-diarizer.cpp`

## core/spelling-fusion-data.cpp
- Layer: data_access
- Language: cpp
- Symbols:
  - `build_set` (function, line 28) `std::unordered_set<std::string> build_set(
    std::initializer_list<const char *> phrases)`
  - `upper_modifiers` (function, line 268) `const std::unordered_set<std::string> &upper_modifiers()`
  - `upper_modifiers_by_length` (function, line 281) `const std::vector<std::string> &upper_modifiers_by_length()`
  - `sort` (function, line 287) `std::sort(v.begin(), v.end(),
              [](const std::string &a, const std::string &b)`
  - `undo_words` (function, line 296) `const std::unordered_set<std::string> &undo_words()`
  - `clear_words` (function, line 309) `const std::unordered_set<std::string> &clear_words()`
  - `stop_words` (function, line 319) `const std::unordered_set<std::string> &stop_words()`
  - `default_weak_homonyms` (function, line 338) `const std::unordered_set<std::string> &default_weak_homonyms()`
  - `default_meta` (function, line 356) `const DefaultSpellingMeta &default_meta()`
- Depends on: `core/spelling-fusion-data.h`, `core/spelling-fusion.h`

## core/spelling-fusion-data.h
- Layer: data_access
- Doc: Compiled-in tables for the spelling matcher. Values are hand-ported
- Language: h
- Symbols:
  - `DefaultSpellingMeta` (struct, line 53)
  - `upper_modifiers` (function, line 27) `const std::unordered_set<std::string> &upper_modifiers();`
  - `upper_modifiers_by_length` (function, line 28) `const std::vector<std::string> &upper_modifiers_by_length();`
  - `undo_words` (function, line 32) `const std::unordered_set<std::string> &undo_words();`
  - `clear_words` (function, line 33) `const std::unordered_set<std::string> &clear_words();`
  - `stop_words` (function, line 34) `const std::unordered_set<std::string> &stop_words();`
  - `default_weak_homonyms` (function, line 40) `const std::unordered_set<std::string> &default_weak_homonyms();`
  - `default_meta` (function, line 60) `const DefaultSpellingMeta &default_meta();`
  - `SPELLING_FUSION_DATA_H` (macro, line 2) `#define SPELLING_FUSION_DATA_H`
- Imported by: `core/spelling-fusion-data.cpp`, `core/spelling-fusion-test.cpp`, `core/spelling-fusion.cpp`, `core/spelling-model.cpp`

## core/spelling-fusion-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `char_match` (function, line 13) `SpellingMatch char_match(const std::string &c)`
  - `no_match` (function, line 21) `SpellingMatch no_match()`
  - `TEST_CASE` (function, line 25) `TEST_CASE("spelling-fusion: normalize")`
  - `TEST_CASE` (function, line 39) `TEST_CASE("spelling-fusion: matcher classifies plain letters")`
  - `TEST_CASE` (function, line 50) `TEST_CASE("spelling-fusion: matcher classifies NATO codewords")`
  - `TEST_CASE` (function, line 61) `TEST_CASE("spelling-fusion: matcher classifies digits")`
  - `TEST_CASE` (function, line 73) `TEST_CASE("spelling-fusion: matcher parses 10..1000 number words")`
  - `TEST_CASE` (function, line 85) `TEST_CASE("spelling-fusion: matcher applies upper-case modifier")`
  - `TEST_CASE` (function, line 94) `TEST_CASE("spelling-fusion: matcher recognizes speller patterns")`
  - `TEST_CASE` (function, line 103) `TEST_CASE("spelling-fusion: matcher classifies command words")`
  - `TEST_CASE` (function, line 114) `TEST_CASE("spelling-fusion: matcher classifies special characters")`
  - `TEST_CASE` (function, line 149) `TEST_CASE("spelling-fusion: weak-homonym detection")`
  - `TEST_CASE` (function, line 158) `TEST_CASE("spelling-fusion: fuse without prediction")`
  - `TEST_CASE` (function, line 166) `TEST_CASE("spelling-fusion: fuse drops unrecognized + no prediction")`
  - `TEST_CASE` (function, line 173) `TEST_CASE("spelling-fusion: fuse passes through command words")`
  - `TEST_CASE` (function, line 183) `TEST_CASE(
    "spelling-fusion: special-character match is preserved when the "
    "spelling mo...`
  - `TEST_CASE` (function, line 204) `TEST_CASE("spelling-fusion: weak-homonym demotion")`
  - `TEST_CASE` (function, line 225) `TEST_CASE("spelling-fusion: cross-class routing")`
  - `TEST_CASE` (function, line 238) `TEST_CASE("spelling-fusion: same-class disagreement uses threshold")`
  - `TEST_CASE` (function, line 251) `TEST_CASE("spelling-fusion: multi-digit ASR vs single-digit spelling")`
  - `TEST_CASE` (function, line 275) `TEST_CASE("spelling-fusion: agreement preserves matcher casing")`
  - `TEST_CASE` (function, line 284) `TEST_CASE("spelling-fusion: spelling-only when matcher misses")`
  - `TEST_CASE` (function, line 293) `TEST_CASE("spelling-fusion: data tables are non-empty")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 7) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/spelling-fusion-data.h`, `core/spelling-fusion.h`

## core/spelling-fusion.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `is_ascii_drop` (function, line 25) `bool is_ascii_drop(char c)`
  - `is_ascii_letter` (function, line 35) `bool is_ascii_letter(char c)`
  - `ascii_to_lower` (function, line 39) `char ascii_to_lower(char c)`
  - `consume_curly_quote` (function, line 46) `size_t consume_curly_quote(const std::string &input, size_t i)`
  - `split_on_whitespace` (function, line 62) `std::vector<std::string> split_on_whitespace(const std::string &s)`
  - `parse_number_words` (function, line 108) `std::optional<int> parse_number_words(const std::string &text)`
  - `is_ascii_digit_string` (function, line 181) `bool is_ascii_digit_string(const std::string &s)`
  - `is_printable_ascii` (function, line 189) `bool is_printable_ascii(char c)`
  - `spelling_normalize` (function, line 195) `std::string spelling_normalize(const std::string &text)`
  - `SpellingMatcher` (function, line 234) `SpellingMatcher::SpellingMatcher()
    : lookup_(&spelling_fusion_data::lookup_table()),
      up...`
  - `classify` (function, line 244) `SpellingMatch SpellingMatcher::classify(const std::string &raw_text) const`
  - `is_weak_homonym` (function, line 300) `bool SpellingMatcher::is_weak_homonym(const std::string &raw_text) const`
  - `resolve` (function, line 305) `std::optional<std::string> SpellingMatcher::resolve(
    const std::string &text) const`
  - `resolve_spelled_letter` (function, line 326) `std::optional<std::string> SpellingMatcher::resolve_spelled_letter(
    const std::string &text) ...`
  - `string_is_letter` (function, line 373) `bool string_is_letter(const std::string &c)`
  - `string_is_digit` (function, line 381) `bool string_is_digit(const std::string &c)`
  - `single_char_is_letter` (function, line 389) `bool single_char_is_letter(const std::string &c)`
  - `apply_case` (function, line 393) `std::string apply_case(const std::string &ch, const std::string &hint)`
  - `fuse_default` (function, line 407) `FusedResult fuse_default(const std::string &raw_text,
                         const SpellingMatc...`
- Depends on: `core/spelling-fusion-data.h`, `core/spelling-fusion.h`

## core/spelling-fusion.h
- Layer: utility
- Doc: C++ port of the matcher / fusion logic from
- Language: h
- Symbols:
  - `SpellingMatch` (struct, line 34)
  - `SpellingPrediction` (struct, line 47)
  - `FusedResult` (struct, line 88)
  - `SpellingMatchType` (enum, line 26)
  - `SpellingMatchType` (class, line 26)
  - `SpellingMatcher` (class, line 53)
  - `is_character` (function, line 41) `bool is_character() const`
  - `is_recognized` (function, line 42) `bool is_recognized() const`
  - `is_character` (function, line 91) `bool is_character() const`
  - `is_weak_homonym` (function, line 66) `bool is_weak_homonym(const std::string &raw_text) const;`
  - `SPELLING_FUSION_H` (macro, line 2) `#define SPELLING_FUSION_H`
- Imported by: `core/spelling-fusion-data.cpp`, `core/spelling-fusion-test.cpp`, `core/spelling-fusion.cpp`, `core/spelling-model-test.cpp`, `core/spelling-model.h`

## core/spelling-model-test.cpp
- Layer: business_logic
- Language: cpp
- Symbols:
  - `Clip` (struct, line 99)
  - `find_model_path` (function, line 21) `std::string find_model_path()`
  - `find_wav` (function, line 33) `std::string find_wav(const std::string &label, const std::string &filename)`
  - `read_file` (function, line 47) `std::vector<uint8_t> read_file(const std::string &path)`
  - `TEST_CASE` (function, line 60) `TEST_CASE("spelling-model: load from path")`
  - `TEST_CASE` (function, line 73) `TEST_CASE("spelling-model: load from memory")`
  - `TEST_CASE` (function, line 86) `TEST_CASE("spelling-model: predict on bundled clips")`
  - `TEST_CASE` (function, line 133) `TEST_CASE("spelling-model: invalid arguments are rejected")`
  - `buffer` (function, line 53) `std::vector<uint8_t> buffer(static_cast<size_t>(size));`
  - `dummy` (function, line 143) `std::vector<float> dummy(16000, 0.0f);`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 12) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-utils/debug-utils.h`, `core/spelling-fusion.h`, `core/spelling-model.h`

## core/spelling-model.cpp
- Layer: business_logic
- Language: cpp
- Symbols:
  - `lookup_metadata` (function, line 26) `std::optional<std::string> lookup_metadata(const OrtApi *ort_api,
                               ...`
  - `trim` (function, line 45) `std::string trim(const std::string &s)`
  - `parse_class_list_json` (function, line 59) `std::vector<std::string> parse_class_list_json(const std::string &raw)`
  - `SpellingModel` (function, line 95) `SpellingModel::SpellingModel(bool log_ort_run,
                             const std::vector<std...`
  - `initialize_session_options` (function, line 137) `void SpellingModel::initialize_session_options()`
  - `apply_default_metadata` (function, line 157) `void SpellingModel::apply_default_metadata()`
  - `load` (function, line 169) `int SpellingModel::load(const char *model_path)`
  - `load_from_memory` (function, line 177) `int SpellingModel::load_from_memory(const uint8_t *model_data,
                                  ...`
  - `populate_metadata_from_session` (function, line 186) `int SpellingModel::populate_metadata_from_session()`
  - `predict` (function, line 243) `int SpellingModel::predict(const float *audio, size_t audio_size,
                           int3...`
  - `clip` (function, line 260) `std::vector<float> clip(target_samples_, 0.0f);`
  - `probs` (function, line 307) `std::vector<float> probs(row_size);`
- Depends on: `core/moonshine-utils/debug-utils.h`, `core/ort-utils/moonshine-tensor-view.h`, `core/ort-utils/ort-utils.h`, `core/spelling-fusion-data.h`, `core/spelling-model.h`

## core/spelling-model.h
- Layer: business_logic
- Doc: Wraps the SpellingCNN ``.ort`` model. An instance is created
- Language: h
- Symbols:
  - `SpellingModel` (class, line 24)
  - `sample_rate` (function, line 56) `int32_t sample_rate() const`
  - `clip_seconds` (function, line 57) `float clip_seconds() const`
  - `classes` (function, line 58) `const std::vector<std::string> &classes() const`
  - `load` (function, line 39) `int load(const char *model_path);`
  - `load_from_memory` (function, line 43) `int load_from_memory(const uint8_t *model_data, size_t model_data_size);`
  - `predict` (function, line 52) `int predict(const float *audio, size_t audio_size, int32_t sample_rate, SpellingPrediction *out_prediction);`
  - `initialize_session_options` (function, line 61) `private: void initialize_session_options();`
  - `populate_metadata_from_session` (function, line 62) `int populate_metadata_from_session();`
  - `apply_default_metadata` (function, line 63) `void apply_default_metadata();`
  - `SPELLING_MODEL_H` (macro, line 2) `#define SPELLING_MODEL_H`
- Depends on: `core/spelling-fusion.h`
- Imported by: `core/spelling-model-test.cpp`, `core/spelling-model.cpp`

## core/tts-repeated-memory-test.cpp
- Layer: testing
- Doc: Repeated-use memory regression test for the text-to-speech synthesizers.  The transcriber has a long-stream memory test 
- Language: cpp
- Symbols:
  - `EngineSpec` (struct, line 216)
  - `read_rss_kb` (function, line 54) `size_t read_rss_kb()`
  - `median` (function, line 90) `size_t median(std::vector<size_t> values)`
  - `env_size` (function, line 99) `size_t env_size(const char *name, size_t default_value)`
  - `detect_continual_growth` (function, line 117) `bool detect_continual_growth(const std::vector<size_t> &samples,
                             siz...`
  - `create_synth` (function, line 223) `int32_t create_synth(const EngineSpec &spec)`
  - `synth_once` (function, line 236) `bool synth_once(int32_t handle, size_t text_index)`
  - `reload_strict` (function, line 248) `bool reload_strict()`
  - `run_growth_phase` (function, line 259) `void run_growth_phase(const std::string &label, size_t iterations,
                      const st...`
  - `exercise_engine` (function, line 294) `void exercise_engine(const EngineSpec &spec)`
  - `run_growth_phase` (function, line 306) `run_growth_phase(
        std::string(spec.name) + " synth", synth_iterations,
        [handle](s...`
  - `run_growth_phase` (function, line 322) `run_growth_phase(
      std::string(spec.name) + " reload", reload_iterations,
      [&spec](size...`
  - `file_present` (function, line 339) `bool file_present(const fs::path &p)`
  - `kokoro_spec` (function, line 344) `std::optional<EngineSpec> kokoro_spec()`
  - `piper_spec` (function, line 355) `std::optional<EngineSpec> piper_spec()`
  - `zipvoice_spec` (function, line 389) `std::optional<EngineSpec> zipvoice_spec()`
  - `TEST_CASE` (function, line 407) `TEST_CASE("tts-repeated-memory-kokoro")`
  - `TEST_CASE` (function, line 416) `TEST_CASE("tts-repeated-memory-piper")`
  - `TEST_CASE` (function, line 426) `TEST_CASE("tts-repeated-memory-zipvoice")`
  - `discover_data_root` (function, line 439) `std::optional<fs::path> discover_data_root()`
  - `main` (function, line 464) `int main(int argc, char **argv)`
  - `DOCTEST_CONFIG_IMPLEMENT` (macro, line 27) `#define DOCTEST_CONFIG_IMPLEMENT`
- Depends on: `core/moonshine-c-api.h`

## core/voice-activity-detector-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 11) `TEST_CASE("voice-activity-detector-test")`
  - `SUBCASE` (function, line 15) `SUBCASE("vad-block")`
  - `SUBCASE` (function, line 54) `SUBCASE("vad-stream")`
  - `SUBCASE` (function, line 122) `SUBCASE("vad-threshold-0")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 8) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-utils/debug-utils.h`, `core/voice-activity-detector.h`

## core/voice-activity-detector.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `seconds_from_sample_count` (function, line 15) `float seconds_from_sample_count(size_t sample_count)`
  - `VoiceActivityDetector` (function, line 24) `VoiceActivityDetector::VoiceActivityDetector(float threshold,
                                   ...`
  - `start` (function, line 50) `void VoiceActivityDetector::start()`
  - `stop` (function, line 62) `void VoiceActivityDetector::stop()`
  - `process_audio` (function, line 69) `void VoiceActivityDetector::process_audio(const float *audio_data,
                              ...`
  - `clear_completed_segment_audio_data` (function, line 99) `void VoiceActivityDetector::clear_completed_segment_audio_data()`
  - `retained_segment_audio_byte_count` (function, line 107) `size_t VoiceActivityDetector::retained_segment_audio_byte_count() const`
  - `completed_segment_audio_byte_count` (function, line 115) `size_t VoiceActivityDetector::completed_segment_audio_byte_count() const`
  - `process_audio_chunk` (function, line 125) `void VoiceActivityDetector::process_audio_chunk(const float *audio_data,
                        ...`
  - `on_voice_start` (function, line 196) `void VoiceActivityDetector::on_voice_start()`
  - `on_voice_continuing` (function, line 210) `void VoiceActivityDetector::on_voice_continuing()`
  - `on_voice_end` (function, line 219) `void VoiceActivityDetector::on_voice_end()`
  - `to_string` (function, line 228) `std::string VoiceActivitySegment::to_string() const`
  - `to_string` (function, line 238) `std::string VoiceActivityDetector::to_string() const`
  - `input_audio_vector` (function, line 79) `std::vector<float> input_audio_vector(audio_data, audio_data + audio_data_size);`
  - `audio_vec` (function, line 136) `std::vector<float> audio_vec(audio_data, audio_data + audio_data_size);`
- Depends on: `core/moonshine-utils/debug-utils.h`, `core/resampler.h`, `core/voice-activity-detector.h`

## core/voice-activity-detector.h
- Layer: utility
- Language: h
- Symbols:
  - `VoiceActivitySegment` (struct, line 9)
  - `VoiceActivityDetector` (class, line 22)
  - `is_active` (function, line 53) `bool is_active() const`
  - `get_segments` (function, line 56) `const std::vector<VoiceActivitySegment> *get_segments() const`
  - `start` (function, line 51) `void start();`
  - `stop` (function, line 52) `void stop();`
  - `process_audio` (function, line 54) `void process_audio(const float *audio_data, size_t audio_data_size, int32_t sample_rate);`
  - `retained_segment_audio_byte_count` (function, line 59) `size_t retained_segment_audio_byte_count() const;`
  - `completed_segment_audio_byte_count` (function, line 60) `size_t completed_segment_audio_byte_count() const;`
  - `clear_completed_segment_audio_data` (function, line 61) `void clear_completed_segment_audio_data();`
  - `clear` (function, line 65) `private: void clear();`
  - `on_voice_start` (function, line 66) `void on_voice_start();`
  - `on_voice_end` (function, line 67) `void on_voice_end();`
  - `on_voice_continuing` (function, line 68) `void on_voice_continuing();`
  - `process_audio_chunk` (function, line 69) `void process_audio_chunk(const float *audio_data, size_t audio_data_size);`
  - `VOICE_ACTIVITY_DETECTOR_H` (macro, line 2) `#define VOICE_ACTIVITY_DETECTOR_H`
- Depends on: `core/silero-vad.h`
- Imported by: `core/voice-activity-detector-test.cpp`, `core/voice-activity-detector.cpp`

## core/word-alignment-benchmark.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `BenchResult` (struct, line 31)
  - `load_wav` (function, line 10) `static float* load_wav(const char* path, long* num_samples_out)`
  - `run_benchmark` (function, line 38) `static BenchResult run_benchmark(const char* model_path, const char* wav_path,
                  ...`
  - `main` (function, line 97) `int main(int argc, char** argv)`
- Depends on: `core/moonshine-c-api.h`, `core/moonshine-utils/file-utils.h`

## core/word-alignment-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 12) `TEST_CASE("word-timestamps")`
  - `SUBCASE` (function, line 13) `SUBCASE("non-streaming-transcribe-with-word-timestamps")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 9) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-c-api.h`, `core/moonshine-utils/debug-utils.h`

## core/word-alignment.cpp
- Layer: utility
- Doc: DTW (Dynamic Time Warping)
- Language: cpp
- Symbols:
  - `WordGroup` (struct, line 304)
  - `dtw` (function, line 12) `void dtw(const std::vector<float>& cost_matrix, int N, int M,
         std::vector<int>& text_ind...`
  - `compute_median` (function, line 93) `static float compute_median(std::vector<float>& window)`
  - `median_filter` (function, line 99) `void median_filter(std::vector<float>& data, int channels, int height,
                   int wid...`
  - `token_starts_new_word` (function, line 159) `static bool token_starts_new_word(BinTokenizer* tokenizer, int token_id)`
  - `decode_tokens` (function, line 174) `static std::string decode_tokens(BinTokenizer* tokenizer,
                                 const ...`
  - `align_words` (function, line 181) `std::vector<TranscriberWord> align_words(const float* cross_attention_data,
                     ...`
  - `D` (function, line 16) `std::vector<float> D((N + 1) * (M + 1), std::numeric_limits<float>::infinity());`
  - `trace` (function, line 22) `std::vector<int> trace(N * M, 0);`
  - `padded` (function, line 114) `std::vector<float> padded(padded_width);`
  - `window` (function, line 115) `std::vector<float> window(filter_width);`
  - `result_row` (function, line 116) `std::vector<float> result_row(width);`
  - `weights` (function, line 200) `std::vector<float> weights(total_size);`
  - `matrix` (function, line 250) `std::vector<float> matrix(n_steps * encoder_frames, 0.0f);`
  - `neg_matrix` (function, line 270) `std::vector<float> neg_matrix(matrix.size());`
- Depends on: `core/word-alignment.h`

## core/word-alignment.h
- Layer: utility
- Language: h
- Symbols:
  - `TranscriberWord` (struct, line 9)
  - `dtw` (function, line 18) `void dtw(const std::vector<float>& cost_matrix, int N, int M, std::vector<int>& text_indices_out, std::vector<int>& time_indices_out);`
  - `median_filter` (function, line 24) `void median_filter(std::vector<float>& data, int channels, int height, int width, int filter_width);`
  - `WORD_ALIGNMENT_H` (macro, line 2) `#define WORD_ALIGNMENT_H`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`
- Imported by: `core/moonshine-model.h`, `core/moonshine-streaming-model.h`, `core/word-alignment.cpp`
