# Subsystem: core

## core/benchmark.cpp
- Layer: utility
- Doc: include <chrono> include <cstdio> include <iostream> include <string> include <vector>  include "file-utils.h" include "
- Language: cpp
- Symbols:
  - `AudioProducer` (class, line 11)
  - `AudioProducer` (function, line 12) `public:
  AudioProducer(std::string wav_path, float chunk_duration_seconds = 0.0214f)
      : cur...`
  - `getNextAudio` (function, line 18) `bool getNextAudio(std::vector<float> &out_audio_data)`
  - `sample_rate` (function, line 30) `int32_t sample_rate() const`
  - `audio_data_size` (function, line 31) `size_t audio_data_size() const`
  - `main` (function, line 42) `int main(int argc, char *argv[])`
  - `loadWavData` (function, line 108) `void AudioProducer::loadWavData(std::string wav_path)`
  - `min` (function, line 23) `std::min(current_index_ + chunk_size_, audio_data_.size());`
  - `audio_producer` (function, line 63) `AudioProducer audio_producer(wav_path);`
  - `transcriber` (function, line 65) `moonshine::Transcriber transcriber(model_path, model_arch);`
  - `now` (function, line 68) `std::chrono::high_resolution_clock::now();`
  - `fprintf` (function, line 100) `fprintf(stderr, "%s\n", transcript.toString().c_str());`
  - `perror` (function, line 116) `std::perror("Failed to open WAV file");`
  - `fclose` (function, line 124) `std::fclose(file);`
  - `runtime_error` (function, line 125) `throw std::runtime_error("Not a RIFF file");`
  - `fseek` (function, line 129) `std::fseek(file, 4, SEEK_CUR);`
  - `fread_exact` (function, line 162) `fread_exact(&audio_format, sizeof(uint16_t), 1, file, "WAV fmt chunk");`
- Depends on: `core/moonshine-cpp.h`, `core/moonshine-utils/file-utils.h`

## core/cosine-distance-test.cpp
- Layer: infrastructure
- Doc: include "cosine-distance.h"  include <stdexcept>  define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN include <doctest.h>
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 7) `TEST_CASE("cosine-distance")`
  - `SUBCASE` (function, line 9) `SUBCASE("identical vectors give zero distance")`
  - `SUBCASE` (function, line 14) `SUBCASE("orthogonal vectors give distance one")`
  - `SUBCASE` (function, line 20) `SUBCASE("opposite vectors give distance two")`
  - `SUBCASE` (function, line 26) `SUBCASE("mismatched length throws")`
  - `SUBCASE` (function, line 32) `SUBCASE("zero vector gives zero distance")`
  - `SUBCASE` (function, line 38) `SUBCASE("matches scipy implementation")`
  - `CHECK` (function, line 12) `CHECK(cosine_distance(a, b) == doctest::Approx(0.0f));`
  - `CHECK_THROWS_AS` (function, line 30) `CHECK_THROWS_AS(cosine_distance(a, b), std::invalid_argument);`
  - `REQUIRE` (function, line 53) `REQUIRE(actual_distance == doctest::Approx(expected_distance));`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 4) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/cosine-distance.h`

## core/cosine-distance.cpp
- Layer: infrastructure
- Doc: include "cosine-distance.h"  include <cmath> include <stdexcept>
- Language: cpp
- Symbols:
  - `cosine_distance` (function, line 5) `float cosine_distance(const std::vector<float>& a,
                      const std::vector<float>...`
  - `invalid_argument` (function, line 9) `throw std::invalid_argument( "cosine distance: vectors must have the same length");`
- Depends on: `core/cosine-distance.h`

## core/cosine-distance.h
- Layer: infrastructure
- Doc: ifndef COSINE_DISTANCE_H_ define COSINE_DISTANCE_H_  include <vector>  Computes cosine distance between two vectors: 1 -
- Language: h
- Symbols:
  - `cosine_distance` (function, line 9) `float cosine_distance(const std::vector<float>& a, const std::vector<float>& b);`
  - `COSINE_DISTANCE_H_` (macro, line 2) `#define COSINE_DISTANCE_H_`
- Imported by: `core/cosine-distance-test.cpp`, `core/cosine-distance.cpp`

## core/embedding-model.h
- Layer: business_logic
- Doc: ifndef EMBEDDING_MODEL_H define EMBEDDING_MODEL_H  include <cmath> include <string> include <vector>
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
- Doc: include "gemma-embedding-model.h"  include <cmath> include <filesystem> include <iostream>  define DOCTEST_CONFIG_IMPLEM
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 9) `TEST_CASE("gemma-embedding-model")`
  - `SUBCASE` (function, line 17) `SUBCASE("load model")`
  - `SUBCASE` (function, line 25) `SUBCASE("get embeddings")`
  - `SUBCASE` (function, line 45) `SUBCASE("identical strings have similarity 1.0")`
  - `SUBCASE` (function, line 54) `SUBCASE("similar strings have high similarity")`
  - `SUBCASE` (function, line 66) `SUBCASE("different strings have lower similarity")`
  - `SUBCASE` (function, line 78) `SUBCASE("query and document embeddings")`
  - `SUBCASE` (function, line 98) `SUBCASE("truncate embedding with MRL")`
  - `SUBCASE` (function, line 125) `SUBCASE("config values")`
  - `TEST_CASE` (function, line 137) `TEST_CASE("gemma-embedding-model error handling")`
  - `SUBCASE` (function, line 139) `SUBCASE("load nonexistent model")`
  - `SUBCASE` (function, line 145) `SUBCASE("get embeddings without loading")`
  - `SUBCASE` (function, line 151) `SUBCASE("load invalid variant")`
  - `MESSAGE` (function, line 14) `MESSAGE("Skipping Gemma embedding tests - model not found at: ", model_dir);`
  - `CHECK` (function, line 22) `CHECK(result == 0);`
  - `REQUIRE` (function, line 29) `REQUIRE(result == 0);`
  - `truncate_embedding` (function, line 112) `GemmaEmbeddingModel::truncate_embedding(full_embedding, target_dim);`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 6) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/gemma-embedding-model.h`

## core/gemma-embedding-model.cpp
- Layer: business_logic
- Doc: include "gemma-embedding-model.h"  include <algorithm> include <cmath> include <cstring>  ifndef _WIN32 include <fcntl.h
- Language: cpp
- Symbols:
  - `GemmaEmbeddingModel` (function, line 20) `GemmaEmbeddingModel::GemmaEmbeddingModel()
    : ort_api_(nullptr),
      ort_env_(nullptr),
    ...`
  - `load` (function, line 66) `int GemmaEmbeddingModel::load(const char *model_dir,
                              const char *mo...`
  - `load_from_memory` (function, line 110) `int GemmaEmbeddingModel::load_from_memory(const uint8_t *model_data,
                            ...`
  - `load_tokenizer` (function, line 130) `int GemmaEmbeddingModel::load_tokenizer(const char *tokenizer_path)`
  - `load_tokenizer_from_memory` (function, line 141) `int GemmaEmbeddingModel::load_tokenizer_from_memory(const uint8_t *data,
                        ...`
  - `tokenize` (function, line 160) `std::vector<int64_t> GemmaEmbeddingModel::tokenize(const std::string &text)`
  - `run_inference` (function, line 185) `std::vector<float> GemmaEmbeddingModel::run_inference(
    const std::vector<int64_t> &input_ids,...`
  - `get_embeddings` (function, line 297) `std::vector<float> GemmaEmbeddingModel::get_embeddings(
    const std::string &text)`
  - `get_embeddings_with_prefix` (function, line 314) `std::vector<float> GemmaEmbeddingModel::get_embeddings_with_prefix(
    const std::string &text, ...`
  - `get_query_embeddings` (function, line 319) `std::vector<float> GemmaEmbeddingModel::get_query_embeddings(
    const std::string &query)`
  - `get_document_embeddings` (function, line 324) `std::vector<float> GemmaEmbeddingModel::get_document_embeddings(
    const std::string &document)`
  - `truncate_embedding` (function, line 329) `std::vector<float> GemmaEmbeddingModel::truncate_embedding(
    const std::vector<float> &embeddi...`
  - `normalize_embedding` (function, line 345) `void GemmaEmbeddingModel::normalize_embedding(std::vector<float> &embedding)`
  - `is_loaded` (function, line 361) `bool GemmaEmbeddingModel::is_loaded() const`
  - `get_config` (function, line 363) `const GemmaEmbeddingConfig &GemmaEmbeddingModel::get_config() const`
  - `LOG_ORT_ERROR` (function, line 32) `LOG_ORT_ERROR(ort_api_, ort_api_->CreateEnv(ORT_LOGGING_LEVEL_WARNING, "GemmaEmbeddingModel", &ort_env_));`
  - `munmap` (function, line 62) `munmap(const_cast<char *>(mmapped_data_), mmapped_data_size_);`
  - `LOG` (function, line 70) `LOG("Model directory is null\n");`
  - `LOGF` (function, line 89) `LOGF("Unknown model variant: %s\n", variant.c_str());`
  - `append_path_component` (function, line 94) `append_path_component(model_dir, model_filename.c_str());`
  - `RETURN_ON_ERROR` (function, line 100) `RETURN_ON_ERROR(ort_session_from_path( ort_api_, ort_env_, ort_session_options_, model_path.c_str(), &session_, &mmapped_data_, &mmapped_data_size_));`
  - `RETURN_ON_NULL` (function, line 103) `RETURN_ON_NULL(session_);`
  - `lock` (function, line 189) `std::lock_guard<std::mutex> lock(mutex_);`
  - `output_shape` (function, line 262) `std::vector<int64_t> output_shape(num_dims);`
  - `embedding` (function, line 287) `std::vector<float> embedding(output_data, output_data + output_size);`
  - `attention_mask` (function, line 309) `std::vector<int64_t> attention_mask(input_ids.size(), 1);`
  - `truncated` (function, line 337) `std::vector<float> truncated(embedding.begin(), embedding.begin() + target_dim);`
  - `DEBUG_ALLOC_ENABLED` (macro, line 16) `#define DEBUG_ALLOC_ENABLED`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/gemma-embedding-model.h`, `core/moonshine-utils/debug-utils.h`, `core/moonshine-utils/string-utils.h`, `core/ort-utils/ort-utils.h`

## core/gemma-embedding-model.h
- Layer: business_logic
- Doc: ifndef GEMMA_EMBEDDING_MODEL_H define GEMMA_EMBEDDING_MODEL_H  include <memory> include <mutex> include <string> include
- Language: h
- Symbols:
  - `GemmaEmbeddingConfig` (struct, line 17)
  - `GemmaEmbeddingModel` (class, line 31)
  - `GemmaEmbeddingModel` (function, line 36) `GemmaEmbeddingModel();`
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
- Doc: include "intent-recognizer.h"  include <cmath> include <cstring> include <filesystem> include <iostream> include <map> i
- Language: cpp
- Symbols:
  - `IntentTestCase` (struct, line 111)
  - `PrecisionRecallResult` (struct, line 116)
  - `DiscriminationTest` (struct, line 284)
  - `make_options` (function, line 18) `IntentRecognizerOptions make_options()`
  - `embedding_model_available` (function, line 26) `bool embedding_model_available()`
  - `TEST_CASE` (function, line 30) `TEST_CASE("intent-recognizer unit tests")`
  - `SUBCASE` (function, line 39) `SUBCASE("register and count intents")`
  - `SUBCASE` (function, line 49) `SUBCASE("unregister intent")`
  - `SUBCASE` (function, line 58) `SUBCASE("unregister nonexistent intent")`
  - `SUBCASE` (function, line 63) `SUBCASE("clear intents")`
  - `SUBCASE` (function, line 72) `SUBCASE("rank_intents returns empty for empty utterance")`
  - `SUBCASE` (function, line 77) `SUBCASE("rank_intents sorts by similarity descending and respects max")`
  - `SUBCASE` (function, line 95) `SUBCASE("rank_intents with max_results limit")`
  - `precision` (function, line 121) `float precision() const`
  - `recall` (function, line 126) `float recall() const`
  - `f1_score` (function, line 131) `float f1_score() const`
  - `accuracy` (function, line 137) `float accuracy() const`
  - `TEST_CASE` (function, line 146) `TEST_CASE("intent-recognizer precision/recall with GemmaEmbeddingModel")`
  - `SUBCASE` (function, line 173) `SUBCASE("basic intent matching")`
  - `SUBCASE` (function, line 187) `SUBCASE("precision/recall evaluation")`
  - `SUBCASE` (function, line 282) `SUBCASE("intent discrimination")`
  - `SUBCASE` (function, line 325) `SUBCASE("similarity scores for exact matches")`
  - `TEST_CASE` (function, line 346) `TEST_CASE("intent-recognizer register with pre-computed embedding")`
  - `SUBCASE` (function, line 355) `SUBCASE("register with NULL embedding auto-computes")`
  - `SUBCASE` (function, line 365) `SUBCASE("register with pre-computed embedding")`
  - `SUBCASE` (function, line 379) `SUBCASE("update existing intent preserves count")`
  - `TEST_CASE` (function, line 388) `TEST_CASE("intent-recognizer priority ranking")`
  - `SUBCASE` (function, line 397) `SUBCASE("higher priority intent ranks first regardless of similarity")`
  - `SUBCASE` (function, line 407) `SUBCASE("equal priority falls back to similarity ordering")`
  - `TEST_CASE` (function, line 418) `TEST_CASE("intent-recognizer calculate_embedding")`
  - `SUBCASE` (function, line 427) `SUBCASE("returns non-empty embedding")`
  - `SUBCASE` (function, line 433) `SUBCASE("get_embedding_size returns correct dimension")`
  - `SUBCASE` (function, line 440) `SUBCASE("same text produces same embedding")`
  - `TEST_CASE` (function, line 450) `TEST_CASE("C API intent registration with embedding and priority")`
  - `SUBCASE` (function, line 462) `SUBCASE("register with NULL embedding succeeds")`
  - `SUBCASE` (function, line 468) `SUBCASE("register with nullptr canonical_phrase fails")`
  - `SUBCASE` (function, line 473) `SUBCASE("register multiple intents with different priorities")`
  - `SUBCASE` (function, line 481) `SUBCASE("unregister and clear work")`
  - `TEST_CASE` (function, line 496) `TEST_CASE("C API moonshine_calculate_intent_embedding")`
  - `SUBCASE` (function, line 508) `SUBCASE("basic embedding calculation")`
  - `SUBCASE` (function, line 528) `SUBCASE("null sentence returns error")`
  - `SUBCASE` (function, line 536) `SUBCASE("null out_embedding returns error")`
  - `SUBCASE` (function, line 543) `SUBCASE("null out_embedding_size returns error")`
  - `SUBCASE` (function, line 550) `SUBCASE("invalid handle returns error")`
  - `SUBCASE` (function, line 558) `SUBCASE("round-trip: compute embedding then register with it")`
  - `TEST_CASE` (function, line 588) `TEST_CASE("C API moonshine_free_intent_embedding")`
  - `SUBCASE` (function, line 590) `SUBCASE("safe on nullptr")`
  - `SUBCASE` (function, line 591) `SUBCASE("frees malloc-allocated buffer")`
  - `TEST_CASE` (function, line 598) `TEST_CASE("C API moonshine_calculate_embedding_distance")`
  - `SUBCASE` (function, line 610) `SUBCASE("identical embeddings have similarity ~1.0")`
  - `SUBCASE` (function, line 626) `SUBCASE("similar sentences have high similarity")`
  - `SUBCASE` (function, line 647) `SUBCASE("dissimilar sentences have low similarity")`
  - `SUBCASE` (function, line 668) `SUBCASE("null embedding_a returns error")`
  - `SUBCASE` (function, line 676) `SUBCASE("null embedding_b returns error")`
  - `SUBCASE` (function, line 684) `SUBCASE("null out_similarity returns error")`
  - `SUBCASE` (function, line 691) `SUBCASE("zero embedding_size returns error")`
  - `SUBCASE` (function, line 699) `SUBCASE("invalid handle returns error")`
  - `TEST_CASE` (function, line 710) `TEST_CASE("C API moonshine_get_closest_intents with priority")`
  - `exists` (function, line 28) `return std::filesystem::exists(EMBEDDING_MODEL_DIR);`
  - `MESSAGE` (function, line 33) `MESSAGE("Skipping tests - embedding model not found at: ", EMBEDDING_MODEL_DIR);`
  - `recognizer` (function, line 37) `IntentRecognizer recognizer(make_options());`
  - `CHECK` (function, line 41) `CHECK(recognizer.get_intent_count() == 0);`
  - `REQUIRE` (function, line 176) `REQUIRE(ranked.size() >= 1);`
  - `moonshine_register_intent` (function, line 483) `moonshine_register_intent(handle, "a", nullptr, 0, 0);`
  - `moonshine_free_intent_recognizer` (function, line 493) `moonshine_free_intent_recognizer(handle);`
  - `moonshine_free_intent_embedding` (function, line 526) `moonshine_free_intent_embedding(embedding);`
  - `moonshine_free_intent_matches` (function, line 583) `moonshine_free_intent_matches(matches, count);`
  - `moonshine_calculate_intent_embedding` (function, line 631) `moonshine_calculate_intent_embedding(handle, "turn on the lights", &emb_a, &size_a, nullptr);`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 12) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/gemma-embedding-model.h`, `core/intent-recognizer.h`, `core/moonshine-c-api.h`

## core/intent-recognizer.cpp
- Layer: utility
- Doc: include "intent-recognizer.h"  include <algorithm> include <limits> include <stdexcept>  include "gemma-embedding-model.
- Language: cpp
- Symbols:
  - `RankedEntry` (struct, line 86)
  - `create_embedding_model` (function, line 10) `std::unique_ptr<EmbeddingModel> create_embedding_model(
    const IntentRecognizerOptions &options)`
  - `IntentRecognizer` (function, line 30) `IntentRecognizer::IntentRecognizer(const IntentRecognizerOptions &options)
    : embedding_model_...`
  - `register_intent` (function, line 35) `void IntentRecognizer::register_intent(const std::string &trigger_phrase)`
  - `register_intent` (function, line 39) `void IntentRecognizer::register_intent(const std::string &trigger_phrase,
                       ...`
  - `unregister_intent` (function, line 67) `bool IntentRecognizer::unregister_intent(const std::string &trigger_phrase)`
  - `sort` (function, line 114) `std::sort(entries.begin(), entries.end(), [](const auto &a, const auto &b)`
  - `get_intent_count` (function, line 129) `size_t IntentRecognizer::get_intent_count() const`
  - `clear_intents` (function, line 134) `void IntentRecognizer::clear_intents()`
  - `calculate_embedding` (function, line 139) `std::vector<float> IntentRecognizer::calculate_embedding(
    const std::string &sentence) const`
  - `calculate_similarity` (function, line 145) `float IntentRecognizer::calculate_similarity(
    const std::vector<float> &a, const std::vector<...`
  - `get_embedding_size` (function, line 151) `size_t IntentRecognizer::get_embedding_size() const`
  - `runtime_error` (function, line 19) `throw std::runtime_error("Failed to load embedding model from: " + options.model_path);`
  - `lock` (function, line 44) `std::lock_guard<std::mutex> lock(mutex_);`
- Depends on: `core/gemma-embedding-model.h`, `core/intent-recognizer.h`

## core/intent-recognizer.h
- Layer: utility
- Doc: ifndef INTENT_RECOGNIZER_H define INTENT_RECOGNIZER_H  include <cstdint> include <memory> include <mutex> include <strin
- Language: h
- Symbols:
  - `IntentRecognizerOptions` (struct, line 23)
  - `Intent` (struct, line 37)
  - `EmbeddingModelArch` (enum, line 16)
  - `EmbeddingModelArch` (class, line 16)
  - `IntentRecognizer` (class, line 48)
  - `IntentRecognizer` (function, line 55) `explicit IntentRecognizer(const IntentRecognizerOptions &options);`
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
  - `read_binary_file` (function, line 33) `std::vector<uint8_t> read_binary_file(const std::filesystem::path& p)`
  - `kokoro_lang_for_voice_stem` (function, line 44) `const char* kokoro_lang_for_voice_stem(std::string_view stem)`
  - `sample_text_for_kokoro_lang` (function, line 78) `const char* sample_text_for_kokoro_lang(const char* lang)`
  - `append_files_under` (function, line 110) `void append_files_under(
    const std::filesystem::path& root, const std::filesystem::path& sub,...`
  - `build_kokoro_g2p_memory_bundle` (function, line 139) `void build_kokoro_g2p_memory_bundle(
    const std::filesystem::path& data_root,
    std::vector<...`
  - `main` (function, line 265) `int main(int argc, char** argv)`
  - `f` (function, line 35) `std::ifstream f(p, std::ios::binary);`
  - `REQUIRE_FALSE` (function, line 163) `REQUIRE_FALSE(g_data_root.empty());`
  - `REQUIRE` (function, line 164) `REQUIRE(std::filesystem::is_directory(g_data_root));`
  - `REQUIRE_MESSAGE` (function, line 200) `REQUIRE_MESSAGE( kokoro_lang_for_voice_stem(stem) != nullptr, "Unrecognized Kokoro voice id (add prefix mapping): " << stem);`
  - `sort` (function, line 205) `std::sort(voice_stems.begin(), voice_stems.end());`
  - `free` (function, line 261) `std::free(audio);`
  - `moonshine_free_tts_synthesizer` (function, line 262) `moonshine_free_tts_synthesizer(h);`
  - `weakly_canonical` (function, line 277) `std::filesystem::weakly_canonical(std::filesystem::path(argv[1]), ec);`
  - `create_directories` (function, line 296) `fs::create_directories(sandbox);`
  - `current_path` (function, line 297) `fs::current_path(sandbox);`
  - `remove_all` (function, line 310) `std::filesystem::remove_all(sandbox, ec);`
  - `DOCTEST_CONFIG_IMPLEMENT` (macro, line 6) `#define DOCTEST_CONFIG_IMPLEMENT`
- Depends on: `core/moonshine-c-api.h`

## core/moonshine-c-api-test.cpp
- Layer: presentation
- Doc: include "moonshine-c-api.h"  include <algorithm> include <array> include <cmath> include <cstdlib> include <cstring> inc
- Language: cpp
- Symbols:
  - `GraphemePhonemizerLangCase` (struct, line 100)
  - `find_de_piper_voices_dir` (function, line 21) `std::filesystem::path find_de_piper_voices_dir()`
  - `read_binary_file` (function, line 36) `std::vector<uint8_t> read_binary_file(const std::filesystem::path& p)`
  - `find_moonshine_tts_data_dir` (function, line 48) `std::optional<std::filesystem::path> find_moonshine_tts_data_dir()`
  - `free_phonemes_output` (function, line 71) `void free_phonemes_output(const char* ipa)`
  - `grapheme_phonemizer_smoke` (function, line 78) `void grapheme_phonemizer_smoke(const std::filesystem::path& data_root,
                          ...`
  - `TEST_CASE` (function, line 109) `TEST_CASE("moonshine-test-v2")`
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
  - `TEST_CASE` (function, line 656) `TEST_CASE("moonshine-phonemes-to-speech-c-api")`
  - `SUBCASE` (function, line 658) `SUBCASE("invalid-handle")`
  - `SUBCASE` (function, line 666) `SUBCASE("invalid-arguments")`
  - `SUBCASE` (function, line 695) `SUBCASE("kokoro-matches-text-to-speech")`
  - `TEST_CASE` (function, line 783) `TEST_CASE("grapheme-to-phonemizer-c-api")`
  - `SUBCASE` (function, line 785) `SUBCASE("create-invalid-filenames-pointer")`
  - `SUBCASE` (function, line 794) `SUBCASE("text-to-phonemes-invalid-handle")`
  - `SUBCASE` (function, line 801) `SUBCASE("text-to-phonemes-invalid-arguments")`
  - `SUBCASE` (function, line 828) `SUBCASE("rule-based-languages-smoke")`
  - `SUBCASE` (function, line 867) `SUBCASE("chinese-when-onnx-bundle-present")`
  - `SUBCASE` (function, line 884) `SUBCASE("japanese-when-onnx-bundle-present")`
  - `SUBCASE` (function, line 903) `SUBCASE("arabic-when-onnx-bundle-present")`
  - `TEST_CASE` (function, line 922) `TEST_CASE("moonshine-tts-g2p-dependency-api")`
  - `SUBCASE` (function, line 924) `SUBCASE("null-output-pointer")`
  - `SUBCASE` (function, line 932) `SUBCASE("options-count-without-options-pointer")`
  - `SUBCASE` (function, line 942) `SUBCASE("g2p-empty-means-all-languages")`
  - `SUBCASE` (function, line 960) `SUBCASE("g2p-arabic-onnx-model-key-matches-meta-onnx-filename")`
  - `SUBCASE` (function, line 973) `SUBCASE("g2p-french-lists-pos-csv-files-not-directory-prefix")`
  - `SUBCASE` (function, line 987) `SUBCASE("g2p-single-language")`
  - `SUBCASE` (function, line 996) `SUBCASE("g2p-unsupported-language")`
  - `SUBCASE` (function, line 1004) `SUBCASE("g2p-multiple-languages")`
  - `SUBCASE` (function, line 1016) `SUBCASE("g2p-appends-override-key-when-option-set")`
  - `SUBCASE` (function, line 1028) `SUBCASE("tts-json-single-language")`
  - `SUBCASE` (function, line 1043) `SUBCASE("tts-empty-all-languages-json")`
  - `SUBCASE` (function, line 1054) `SUBCASE("tts-unsupported-language")`
  - `SUBCASE` (function, line 1062) `SUBCASE("tts-multiple-languages")`
  - `SUBCASE` (function, line 1075) `SUBCASE("tts-piper-engine-on-en_us")`
  - `SUBCASE` (function, line 1089) `SUBCASE("tts-kokoro-engine-on-fr")`
  - `SUBCASE` (function, line 1103) `SUBCASE("tts-explicit-piper-onnx-map-keys")`
  - `SUBCASE` (function, line 1118) `SUBCASE("tts-piper-voice-selects-onnx-basename")`
  - `SUBCASE` (function, line 1131) `SUBCASE("tts-voices-json-object-en_us")`
  - `SUBCASE` (function, line 1154) `SUBCASE("tts-voices-kokoro-reports-missing-without-assets")`
  - `SUBCASE` (function, line 1168) `SUBCASE("tts-voices-unsupported-language")`
  - `SUBCASE` (function, line 1175) `SUBCASE("tts-voices-piper-de-includes-thorsten-stem")`
  - `SUBCASE` (function, line 1195) `SUBCASE("tts-voices-piper-en_us-includes-saikat-stem")`
  - `SUBCASE` (function, line 1215) `SUBCASE("tts-zipvoice-dependencies")`
  - `SUBCASE` (function, line 1233) `SUBCASE("tts-zipvoice-voices-listing")`
  - `TEST_CASE` (function, line 1252) `TEST_CASE("moonshine-stt-intent-dependency-api")`
  - `SUBCASE` (function, line 1254) `SUBCASE("null-output-pointer")`
  - `SUBCASE` (function, line 1261) `SUBCASE("options-count-without-options-pointer")`
  - `SUBCASE` (function, line 1270) `SUBCASE("stt-empty-language-is-invalid")`
  - `SUBCASE` (function, line 1277) `SUBCASE("stt-english-default-is-medium-streaming")`
  - `SUBCASE` (function, line 1295) `SUBCASE("stt-english-tiny-non-streaming")`
  - `SUBCASE` (function, line 1316) `SUBCASE("stt-non-english-omits-attention-extra")`
  - `SUBCASE` (function, line 1333) `SUBCASE("stt-english-name-lookup")`
  - `SUBCASE` (function, line 1341) `SUBCASE("stt-include-spelling-adds-group-for-english")`
  - `SUBCASE` (function, line 1358) `SUBCASE("stt-include-spelling-noop-for-non-english")`
  - `SUBCASE` (function, line 1372) `SUBCASE("stt-unknown-language")`
  - `SUBCASE` (function, line 1380) `SUBCASE("stt-unknown-arch-for-language")`
  - `SUBCASE` (function, line 1390) `SUBCASE("stt-invalid-arch-value")`
  - `SUBCASE` (function, line 1400) `SUBCASE("intent-default-variant-is-q4")`
  - `SUBCASE` (function, line 1414) `SUBCASE("intent-null-model-name-uses-default")`
  - `SUBCASE` (function, line 1423) `SUBCASE("intent-q8-maps-to-model-quantized")`
  - `SUBCASE` (function, line 1440) `SUBCASE("intent-fp32-uses-bare-model-onnx")`
  - `SUBCASE` (function, line 1454) `SUBCASE("intent-unknown-model")`
  - `SUBCASE` (function, line 1461) `SUBCASE("intent-unknown-variant")`
  - `SUBCASE` (function, line 1497) `SUBCASE("builtin-voice-synthesizes-audio")`
  - `SUBCASE` (function, line 1521) `SUBCASE("user-pcm-with-explicit-transcript")`
  - `f` (function, line 38) `std::ifstream f(p, std::ios::binary);`
  - `free` (function, line 73) `std::free(const_cast<char*>(ipa));`
  - `REQUIRE` (function, line 88) `REQUIRE(h >= 0);`
  - `moonshine_free_grapheme_to_phonemizer` (function, line 97) `moonshine_free_grapheme_to_phonemizer(h);`
  - `moonshine_transcribe_add_audio_to_stream` (function, line 194) `moonshine_transcribe_add_audio_to_stream(transcriber_handle, stream_id, chunk_data, chunk_data_size, wav_sample_rate, 0);`
  - `LOGF` (function, line 221) `LOGF( "Incomplete line %zu ('%s', %.2fs) is not the last line " "%" PRId64, j, line.text, line.start_time, transcript->line_count - 1);`
  - `moonshine_free_stream` (function, line 245) `moonshine_free_stream(transcriber_handle, stream_id);`
  - `append_path_component` (function, line 263) `append_path_component(root_model_path, "encoder_model.ort");`
  - `load_file_into_memory` (function, line 272) `load_file_into_memory(encoder_model_path);`
  - `moonshine_free_transcriber` (function, line 475) `moonshine_free_transcriber(transcriber_handle);`
  - `MESSAGE` (function, line 485) `MESSAGE("skip: spelling_cnn.ort not in test-assets");`
  - `CHECK` (function, line 520) `CHECK(std::string(line.text) == "a");`
  - `moonshine_create_tts_synthesizer_from_files` (function, line 543) `moonshine_create_tts_synthesizer_from_files("en_us", nullptr, 0, options, options_count, MOONSHINE_HEADER_VERSION);`
  - `moonshine_free_tts_synthesizer` (function, line 595) `moonshine_free_tts_synthesizer(h);`
  - `INFO` (function, line 863) `INFO("grapheme phonemizer language: " << c.language);`
  - `csv` (function, line 948) `const std::string csv(out);`
  - `json` (function, line 1034) `const std::string json(out);`
  - `is_regular_file` (function, line 1486) `std::filesystem::is_regular_file(zv / "text_encoder.onnx")) && (std::filesystem::is_regular_file(zv / "fm_decoder.ort") || std::filesystem::is_regular_file(zv / "fm_decoder.onnx")) && (std::filesystem`
  - `pcm` (function, line 1525) `std::vector<float> pcm(24000, 0.f);`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 16) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-c-api.h`, `core/moonshine-utils/debug-utils.h`, `core/moonshine-utils/string-utils.h`

## core/moonshine-c-api.cpp
- Layer: presentation
- Language: cpp
- Symbols:
  - `OptionPair` (type_alias, line 79) `typedef std::pair<std::string, std::string> OptionPair;`
  - `OptionVector` (type_alias, line 81) `typedef std::vector<OptionPair> OptionVector;`
  - `parse_option_vector` (function, line 82) `OptionVector parse_option_vector(const moonshine_option_t *options,
                             ...`
  - `parse_common_options` (function, line 98) `OptionVector parse_common_options(const OptionVector &options)`
  - `parse_transcriber_options` (function, line 109) `void parse_transcriber_options(const OptionVector &options,
                               Transc...`
  - `allocate_transcriber_handle` (function, line 170) `int32_t allocate_transcriber_handle(Transcriber *transcriber)`
  - `free_transcriber_handle` (function, line 177) `void free_transcriber_handle(int32_t handle)`
  - `moonshine_load_transcriber_from_memory` (function, line 239) `int32_t moonshine_load_transcriber_from_memory(
    const uint8_t *encoder_model_data, size_t enc...`
  - `moonshine_free_transcriber` (function, line 290) `void moonshine_free_transcriber(int32_t transcriber_handle)`
  - `moonshine_transcribe_without_streaming` (function, line 298) `int32_t moonshine_transcribe_without_streaming(
    int32_t transcriber_handle, float *audio_data...`
  - `moonshine_create_stream` (function, line 321) `int32_t moonshine_create_stream(int32_t transcriber_handle, uint32_t flags)`
  - `moonshine_free_stream` (function, line 335) `int32_t moonshine_free_stream(int32_t transcriber_handle,
                              int32_t s...`
  - `moonshine_start_stream` (function, line 351) `int32_t moonshine_start_stream(int32_t transcriber_handle,
                               int32_t...`
  - `moonshine_stop_stream` (function, line 367) `int32_t moonshine_stop_stream(int32_t transcriber_handle,
                              int32_t s...`
  - `moonshine_transcript_to_string` (function, line 383) `const char *moonshine_transcript_to_string(
    const struct transcript_t *transcript)`
  - `moonshine_transcribe_add_audio_to_stream` (function, line 393) `int32_t moonshine_transcribe_add_audio_to_stream(int32_t transcriber_handle,
                    ...`
  - `moonshine_transcribe_stream` (function, line 419) `int32_t moonshine_transcribe_stream(int32_t transcriber_handle,
                                 ...`
  - `allocate_intent_recognizer_handle` (function, line 447) `int32_t allocate_intent_recognizer_handle(IntentRecognizer *recognizer)`
  - `free_intent_recognizer_handle` (function, line 454) `void free_intent_recognizer_handle(int32_t handle)`
  - `duplicate_c_string` (function, line 470) `char *duplicate_c_string(const char *s)`
  - `moonshine_create_intent_recognizer` (function, line 484) `int32_t moonshine_create_intent_recognizer(const char *model_path,
                              ...`
  - `moonshine_free_intent_recognizer` (function, line 515) `void moonshine_free_intent_recognizer(int32_t intent_recognizer_handle)`
  - `moonshine_register_intent` (function, line 526) `int32_t moonshine_register_intent(int32_t intent_recognizer_handle,
                             ...`
  - `moonshine_unregister_intent` (function, line 552) `int32_t moonshine_unregister_intent(int32_t intent_recognizer_handle,
                           ...`
  - `moonshine_get_closest_intents` (function, line 577) `int32_t moonshine_get_closest_intents(int32_t intent_recognizer_handle,
                         ...`
  - `moonshine_free_intent_matches` (function, line 635) `void moonshine_free_intent_matches(moonshine_intent_match_t *matches,
                           ...`
  - `moonshine_get_intent_count` (function, line 646) `int32_t moonshine_get_intent_count(int32_t intent_recognizer_handle)`
  - `moonshine_clear_intents` (function, line 658) `int32_t moonshine_clear_intents(int32_t intent_recognizer_handle)`
  - `moonshine_calculate_intent_embedding` (function, line 672) `int32_t moonshine_calculate_intent_embedding(int32_t intent_recognizer_handle,
                  ...`
  - `moonshine_free_intent_embedding` (function, line 713) `void moonshine_free_intent_embedding(float *embedding)`
  - `moonshine_calculate_embedding_distance` (function, line 715) `int32_t moonshine_calculate_embedding_distance(int32_t intent_recognizer_handle,
                ...`
  - `allocate_text_to_speech_synthesizer_handle` (function, line 754) `int32_t allocate_text_to_speech_synthesizer_handle(
    moonshine_tts::MoonshineTTS *synthesizer)`
  - `parse_tts_options` (function, line 762) `void parse_tts_options(const OptionVector &options,
                       moonshine_tts::Moonshi...`
  - `maybe_autotranscribe_zipvoice_clone` (function, line 778) `void maybe_autotranscribe_zipvoice_clone(
    const OptionVector &options,
    moonshine_tts::Moo...`
  - `moonshine_create_tts_synthesizer_from_files` (function, line 869) `int32_t moonshine_create_tts_synthesizer_from_files(
    const char *language, const char **filen...`
  - `moonshine_create_tts_synthesizer_from_memory` (function, line 910) `int32_t moonshine_create_tts_synthesizer_from_memory(
    const char *language, const char **file...`
  - `moonshine_free_tts_synthesizer` (function, line 1000) `void moonshine_free_tts_synthesizer(int32_t tts_synthesizer_handle)`
  - `moonshine_text_to_speech` (function, line 1041) `int32_t moonshine_text_to_speech(int32_t tts_synthesizer_handle,
                                ...`
  - `moonshine_phonemes_to_speech` (function, line 1088) `int32_t moonshine_phonemes_to_speech(int32_t tts_synthesizer_handle,
                            ...`
  - `malloc_string_copy` (function, line 1143) `char *malloc_string_copy(const std::string &s)`
  - `split_comma_nonempty_language_tokens` (function, line 1152) `std::vector<std::string> split_comma_nonempty_language_tokens(const char *s)`
  - `append_unique_in_order` (function, line 1177) `void append_unique_in_order(std::vector<std::string> &acc,
                            const std:...`
  - `json_utf8_string_literal` (function, line 1187) `std::string json_utf8_string_literal(const std::string &s)`
  - `json_flat_string_array` (function, line 1229) `std::string json_flat_string_array(const std::vector<std::string> &items)`
  - `json_model_dependencies` (function, line 1247) `std::string json_model_dependencies(const moonshine::ModelDependencies &deps)`
  - `json_tts_voice_entry` (function, line 1263) `std::string json_tts_voice_entry(
    const moonshine_tts::MoonshineTtsVoiceAvailability &v)`
  - `json_tts_voices_lang_array` (function, line 1273) `std::string json_tts_voices_lang_array(
    const std::vector<moonshine_tts::MoonshineTtsVoiceAva...`
  - `json_tts_voices_root_object` (function, line 1287) `std::string json_tts_voices_root_object(
    const std::vector<std::pair<
        std::string, st...`
  - `apply_g2p_dependency_query_c_options` (function, line 1305) `void apply_g2p_dependency_query_c_options(
    const moonshine_option_t *options, uint64_t option...`
  - `append_g2p_explicit_override_keys_from_c_options` (function, line 1355) `void append_g2p_explicit_override_keys_from_c_options(
    const moonshine_option_t *options, uin...`
  - `moonshine_get_g2p_dependencies` (function, line 1386) `int32_t moonshine_get_g2p_dependencies(const char *languages,
                                   ...`
  - `moonshine_get_tts_dependencies` (function, line 1450) `int32_t moonshine_get_tts_dependencies(const char *languages,
                                   ...`
  - `moonshine_get_tts_voices` (function, line 1547) `int32_t moonshine_get_tts_voices(const char *languages,
                                 const mo...`
  - `normalize_option_key` (function, line 1653) `std::string normalize_option_key(const char *name)`
  - `parse_int_option` (function, line 1662) `std::optional<int32_t> parse_int_option(const std::string &value)`
  - `moonshine_get_stt_dependencies` (function, line 1680) `int32_t moonshine_get_stt_dependencies(const char *language,
                                    ...`
  - `moonshine_get_intent_dependencies` (function, line 1742) `int32_t moonshine_get_intent_dependencies(const char *model_name,
                               ...`
  - `allocate_grapheme_phonemizer_handle` (function, line 1801) `int32_t allocate_grapheme_phonemizer_handle(moonshine_tts::MoonshineG2P *g2p)`
  - `parse_grapheme_phonemizer_options` (function, line 1808) `void parse_grapheme_phonemizer_options(
    const moonshine_option_t *in_options, uint64_t in_opt...`
  - `finalize_g2p_options_for_phonemizer_create` (function, line 1845) `void finalize_g2p_options_for_phonemizer_create(
    moonshine_tts::MoonshineG2POptions &g2p_opt)`
  - `moonshine_create_grapheme_to_phonemizer_from_files` (function, line 1869) `int32_t moonshine_create_grapheme_to_phonemizer_from_files(
    const char *language, const char ...`
  - `moonshine_create_grapheme_to_phonemizer_from_memory` (function, line 1928) `int32_t moonshine_create_grapheme_to_phonemizer_from_memory(
    const char *language, const char...`
  - `moonshine_free_grapheme_to_phonemizer` (function, line 1995) `void moonshine_free_grapheme_to_phonemizer(
    int32_t grapheme_to_phonemizer_handle)`
  - `moonshine_text_to_phonemes` (function, line 2012) `int32_t moonshine_text_to_phonemes(int32_t grapheme_to_phonemizer_handle,
                       ...`
  - `LOGF` (function, line 73) `LOGF("Moonshine transcriber handle is invalid: handle %d", handle);`
  - `size_t_from_string` (function, line 133) `size_t_from_string(option.second);`
  - `float_from_string` (function, line 146) `float_from_string(option_value);`
  - `runtime_error` (function, line 161) `throw std::runtime_error("Unknown transcriber option: '" + option_name + "', value=" + option_value);`
  - `lock` (function, line 172) `std::lock_guard<std::mutex> lock(transcriber_map_mutex);`
  - `LOG` (function, line 189) `LOG("moonshine_get_version");`
  - `CHECK_TRANSCRIBER_HANDLE` (function, line 311) `CHECK_TRANSCRIBER_HANDLE(transcriber_handle);`
  - `memcpy` (function, line 478) `std::memcpy(out, s, n);`
  - `CHECK_INTENT_RECOGNIZER_HANDLE` (function, line 538) `CHECK_INTENT_RECOGNIZER_HANDLE(intent_recognizer_handle);`
  - `malloc` (function, line 612) `std::malloc(n * sizeof(moonshine_intent_match_t)));`
  - `free` (function, line 621) `std::free(arr[j].canonical_phrase);`
  - `a` (function, line 735) `std::vector<float> a(embedding_a, embedding_a + embedding_size);`
  - `b` (function, line 736) `std::vector<float> b(embedding_b, embedding_b + embedding_size);`
  - `pcm` (function, line 815) `std::vector<float> pcm(n);`
  - `string` (function, line 898) `: std::string("en_us");`
  - `key` (function, line 946) `const std::string key(filenames[i]);`
  - `CHECK_TTS_SYNTHESIZER_HANDLE` (function, line 1062) `CHECK_TTS_SYNTHESIZER_HANDLE(tts_synthesizer_handle);`
  - `tts_option_pairs_from_c` (function, line 1067) `tts_option_pairs_from_c(options, options_count);`
  - `seen` (function, line 1180) `std::unordered_set<std::string> seen(acc.begin(), acc.end());`
  - `snprintf` (function, line 1217) `std::snprintf(buf, sizeof(buf), "\\u%04x", static_cast<unsigned int>(c));`
  - `replace_all` (function, line 1371) `replace_all(to_lowercase(std::string(options[i].name)), "-", "_");`
  - `moonshine_asset_catalog_all_g2p_dependency_keys_union` (function, line 1409) `moonshine_asset_catalog_all_g2p_dependency_keys_union();`
  - `moonshine_asset_catalog_g2p_dependency_keys` (function, line 1419) `moonshine_tts::moonshine_asset_catalog_g2p_dependency_keys(part);`
  - `moonshine_asset_catalog_all_registered_language_tags` (function, line 1489) `moonshine_tts::moonshine_asset_catalog_all_registered_language_tags();`
  - `moonshine_catalog_tts_vocoder_only_dependency_keys` (function, line 1521) `moonshine_tts::moonshine_catalog_tts_vocoder_only_dependency_keys( part, tts_opt);`
  - `moonshine_list_tts_voices_with_availability` (function, line 1588) `moonshine_tts::moonshine_list_tts_voices_with_availability(tag, tts_opt);`
  - `stt_model_dependencies` (function, line 1721) `moonshine::stt_model_dependencies(trim(language_str), model_arch, include_spelling);`
  - `intent_model_dependencies` (function, line 1773) `moonshine::intent_model_dependencies(resolved_model_name, variant);`
  - `CHECK_GRAPHEME_PHONEMIZER_HANDLE` (function, line 2037) `CHECK_GRAPHEME_PHONEMIZER_HANDLE(grapheme_to_phonemizer_handle);`
  - `CHECK_TRANSCRIBER_HANDLE` (macro, line 70) `#define CHECK_TRANSCRIBER_HANDLE(handle)`
  - `CHECK_INTENT_RECOGNIZER_HANDLE` (macro, line 461) `#define CHECK_INTENT_RECOGNIZER_HANDLE(handle)`
  - `CHECK_TTS_SYNTHESIZER_HANDLE` (macro, line 856) `#define CHECK_TTS_SYNTHESIZER_HANDLE(synth_handle)`
  - `CHECK_GRAPHEME_PHONEMIZER_HANDLE` (macro, line 1852) `#define CHECK_GRAPHEME_PHONEMIZER_HANDLE(g2p_handle)`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/intent-recognizer.h`, `core/moonshine-c-api.h`, `core/moonshine-model-catalog.h`, `core/moonshine-model.h`, `core/moonshine-tts/src/moonshine-asset-catalog.h`, `core/moonshine-tts/src/moonshine-g2p.h`, `core/moonshine-tts/src/moonshine-tts.h`, `core/moonshine-utils/debug-utils.h`, `core/moonshine-utils/string-utils.h`, `core/ort-utils/moonshine-ort-allocator.h`, `core/ort-utils/moonshine-tensor-view.h`, `core/ort-utils/ort-utils.h`

## core/moonshine-c-api.h
- Layer: presentation
- Doc: ifndef MOONSHINE_C_API_H define MOONSHINE_C_API_H  Moonshine is a library for building interactive voice applications. I
- Language: h
- Symbols:
  - `moonshine_option_t` (struct, line 137)
  - `transcript_word_t` (struct, line 194)
  - `speaker_span_t` (struct, line 212)
  - `transcript_line_t` (struct, line 231)
  - `transcript_t` (struct, line 276)
  - `moonshine_intent_match_t` (struct, line 611)
  - `main` (function, line 37) `int main(int argc, char *argv[])`
  - `fprintf` (function, line 43) `fprintf(stderr, "Failed to load transcriber\n");`
  - `printf` (function, line 57) `printf( "Line %zu at %f seconds: %s\n", i, transcript->lines[i].start, transcript->lines[i].text);`
  - `moonshine_free_transcriber` (function, line 60) `moonshine_free_transcriber(transcriber_handle);`
  - `moonshine_get_version` (function, line 286) `MOONSHINE_EXPORT int32_t moonshine_get_version(void);`
  - `moonshine_error_to_string` (function, line 290) `MOONSHINE_EXPORT const char *moonshine_error_to_string(int32_t error);`
  - `moonshine_transcript_to_string` (function, line 295) `MOONSHINE_EXPORT const char *moonshine_transcript_to_string( const struct transcript_t *transcript);`
  - `moonshine_load_transcriber_from_files` (function, line 357) `MOONSHINE_EXPORT int32_t moonshine_load_transcriber_from_files( const char *path, uint32_t model_arch, const struct moonshine_option_t *options, uint64_t options_count, int32_t moonshine_version);`
  - `transcriber` (function, line 369) `the buffer must outlive the transcriber (it is *not* copied) and the transcriber will run spelling fusion whenever ``MOONSHINE_FLAG_SPELLING_MODE`` is passed to ``moonshine_transcribe_stream`` or ``mo`
  - `moonshine_transcribe_without_streaming` (function, line 425) `MOONSHINE_EXPORT int32_t moonshine_transcribe_without_streaming( int32_t transcriber_handle, float *audio_data, uint64_t audio_length, int32_t sample_rate, uint32_t flags, struct transcript_t **out_tr`
  - `moonshine_start_stream` (function, line 458) `moonshine_start_stream(transcriber_handle, stream_handle);`
  - `moonshine_transcribe_add_audio_to_stream` (function, line 464) `moonshine_transcribe_add_audio_to_stream(transcriber_handle, stream_handle, latest_audio_data, latest_audio_data_length, microphone_sample_rate, 0);`
  - `moonshine_transcribe_stream` (function, line 471) `moonshine_transcribe_stream(transcriber_handle, stream_handle, 0, &partial_transcript);`
  - `print_transcript` (function, line 473) `print_transcript(out_transcript);`
  - `moonshine_stop_stream` (function, line 475) `moonshine_stop_stream(transcriber_handle, stream_handle);`
  - `moonshine_free_stream` (function, line 481) `moonshine_free_stream(transcriber_handle, stream_handle);`
  - `moonshine_create_stream` (function, line 507) `MOONSHINE_EXPORT int32_t moonshine_create_stream(int32_t transcriber_handle, uint32_t flags);`
  - `files` (function, line 619) `model files (ONNX model and tokenizer.bin). `model_arch` should be one of the MOONSHINE_EMBEDDING_MODEL_ARCH_* constants. Currently only MOONSHINE_EMBEDDING_MODEL_ARCH_GEMMA_300M is supported. `model_`
  - `moonshine_free_intent_recognizer` (function, line 638) `MOONSHINE_EXPORT void moonshine_free_intent_recognizer( int32_t intent_recognizer_handle);`
  - `moonshine_register_intent` (function, line 652) `MOONSHINE_EXPORT int32_t moonshine_register_intent( int32_t intent_recognizer_handle, const char *canonical_phrase, float *embedding, uint64_t embedding_size, int32_t priority);`
  - `moonshine_unregister_intent` (function, line 659) `MOONSHINE_EXPORT int32_t moonshine_unregister_intent( int32_t intent_recognizer_handle, const char *canonical_phrase);`
  - `matches` (function, line 668) `of matches (0 to MOONSHINE_INTENT_MAX_MATCHES), and sets `*out_matches` to a heap-allocated array sorted by descending similarity. Each `canonical_phrase` is a separate heap allocation. When `*out_cou`
  - `moonshine_free_intent_matches` (function, line 685) `MOONSHINE_EXPORT void moonshine_free_intent_matches( struct moonshine_intent_match_t *matches, uint64_t count);`
  - `success` (function, line 689) `Returns the count on success (>= 0), or a negative error code on failure. */ MOONSHINE_EXPORT int32_t moonshine_get_intent_count(int32_t intent_recognizer_handle);`
  - `moonshine_clear_intents` (function, line 697) `MOONSHINE_EXPORT int32_t moonshine_clear_intents(int32_t intent_recognizer_handle);`
  - `moonshine_calculate_intent_embedding` (function, line 708) `MOONSHINE_EXPORT int32_t moonshine_calculate_intent_embedding( int32_t intent_recognizer_handle, const char *sentence, float **out_embedding, uint64_t *out_embedding_size, const char *model_name);`
  - `moonshine_free_intent_embedding` (function, line 715) `MOONSHINE_EXPORT void moonshine_free_intent_embedding(float *embedding);`
  - `moonshine_calculate_embedding_distance` (function, line 725) `MOONSHINE_EXPORT int32_t moonshine_calculate_embedding_distance( int32_t intent_recognizer_handle, const float *embedding_a, const float *embedding_b, uint64_t embedding_size, float *out_similarity);`
  - `choice` (function, line 737) `choice (and other TTS paths via ``moonshine_option_t`` as documented for ``MoonshineTTSOptions``). ``engine`` / ``vocoder_engine`` options are ignored. ZipVoice (zero-shot voice cloning) is selected w`
  - `moonshine_create_tts_synthesizer_from_memory` (function, line 784) `MOONSHINE_EXPORT int32_t moonshine_create_tts_synthesizer_from_memory( const char *language, const char **filenames, const uint64_t filenames_count, const uint8_t **memory, const uint64_t *memory_size`
  - `moonshine_free_tts_synthesizer` (function, line 793) `MOONSHINE_EXPORT void moonshine_free_tts_synthesizer( int32_t tts_synthesizer_handle);`
  - `moonshine_get_g2p_dependencies` (function, line 813) `MOONSHINE_EXPORT int32_t moonshine_get_g2p_dependencies( const char *languages, const struct moonshine_option_t *options, uint64_t options_count, char **out_dependencies_json);`
  - `moonshine_get_tts_dependencies` (function, line 830) `MOONSHINE_EXPORT int32_t moonshine_get_tts_dependencies( const char *languages, const struct moonshine_option_t *options, uint64_t options_count, char **out_dependencies_json);`
  - `moonshine_get_tts_voices` (function, line 858) `MOONSHINE_EXPORT int32_t moonshine_get_tts_voices( const char *languages, const struct moonshine_option_t *options, uint64_t options_count, char **out_voices_json);`
  - `CDN` (function, line 866) `files a model needs from the CDN (https://download.moonshine.ai) without hardcoding the file layout, then load the model from the resulting directory with moonshine_load_transcriber_from_files. ``lang`
  - `moonshine_get_stt_dependencies` (function, line 892) `MOONSHINE_EXPORT int32_t moonshine_get_stt_dependencies( const char *language, const struct moonshine_option_t *options, uint64_t options_count, char **out_dependencies_json);`
  - `moonshine_get_intent_dependencies` (function, line 915) `MOONSHINE_EXPORT int32_t moonshine_get_intent_dependencies( const char *model_name, const struct moonshine_option_t *options, uint64_t options_count, char **out_dependencies_json);`
  - `moonshine_text_to_speech` (function, line 929) `MOONSHINE_EXPORT int32_t moonshine_text_to_speech( int32_t tts_synthesizer_handle, const char *text, const struct moonshine_option_t *options, uint64_t options_count, float **out_audio_data, uint64_t `
  - `moonshine_phonemes_to_speech` (function, line 953) `MOONSHINE_EXPORT int32_t moonshine_phonemes_to_speech( int32_t tts_synthesizer_handle, const char *phonemes, const struct moonshine_option_t *options, uint64_t options_count, float **out_audio_data, u`
  - `bytes` (function, line 990) `used as the asset bytes (not copied—keep valid until the phonemizer is freed). When ``memory[i]`` is NULL or size zero, the key is also used as a path relative to ``g2p_root``, like path-only map entr`
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
- Doc: include "moonshine-cpp.h"  include <cinttypes> include <filesystem> include <fstream>  define DOCTEST_CONFIG_IMPLEMENT_W
- Language: cpp
- Symbols:
  - `load_wav_data` (function, line 13) `bool load_wav_data(const char *path, float **out_float_data,
                   size_t *out_num_s...`
  - `file_exists` (function, line 132) `bool file_exists(const std::string &path)`
  - `onLineStarted` (function, line 147) `void onLineStarted(const moonshine::LineStarted &) override`
  - `onLineUpdated` (function, line 150) `void onLineUpdated(const moonshine::LineUpdated &) override`
  - `onLineTextChanged` (function, line 153) `void onLineTextChanged(const moonshine::LineTextChanged &) override`
  - `onLineCompleted` (function, line 156) `void onLineCompleted(const moonshine::LineCompleted &) override`
  - `TEST_CASE` (function, line 162) `TEST_CASE("moonshine-cpp-test")`
  - `SUBCASE` (function, line 164) `SUBCASE("transcribe-without-streaming")`
  - `SUBCASE` (function, line 193) `SUBCASE("transcribe-with-streaming")`
  - `SUBCASE` (function, line 288) `SUBCASE("g2p")`
  - `SUBCASE` (function, line 306) `SUBCASE("intent recognizer invalid model path throws")`
  - `SUBCASE` (function, line 312) `SUBCASE("spelling-mode-replaces-line-text-via-cpp-ctor")`
  - `SUBCASE` (function, line 347) `SUBCASE("loadFromMemory-with-spelling-buffer")`
  - `SUBCASE` (function, line 395) `SUBCASE("intent recognizer closest intents when embedding model present")`
  - `perror` (function, line 21) `std::perror("Failed to open WAV file");`
  - `fclose` (function, line 29) `std::fclose(file);`
  - `fprintf` (function, line 30) `std::fprintf(stderr, "Not a RIFF file\n");`
  - `fseek` (function, line 35) `std::fseek(file, 4, SEEK_CUR);`
  - `REQUIRE` (function, line 166) `REQUIRE(file_exists(wav_path));`
  - `transcriber` (function, line 175) `moonshine::Transcriber transcriber(root_model_path, moonshine::ModelArch::TINY);`
  - `MESSAGE` (function, line 295) `MESSAGE("skip: en_us G2P lexicon not in moonshine-tts/data");`
  - `REQUIRE_THROWS_AS` (function, line 307) `REQUIRE_THROWS_AS((void)moonshine::IntentRecognizer( "/nonexistent/moonshine/embedding/model", moonshine::EmbeddingModelArch::GEMMA_300M), moonshine::MoonshineException);`
  - `CHECK` (function, line 344) `CHECK(transcript.lines[0].text == "a");`
  - `free` (function, line 345) `free(wav_data);`
  - `f` (function, line 363) `std::ifstream f(path, std::ios::binary);`
  - `slurp` (function, line 368) `slurp(root_model_path + "/encoder_model.ort");`
  - `recognizer` (function, line 400) `moonshine::IntentRecognizer recognizer( dir, moonshine::EmbeddingModelArch::GEMMA_300M);`
  - `REQUIRE_FALSE` (function, line 408) `REQUIRE_FALSE(recognizer.unregisterIntent("unknown phrase"));`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 6) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-cpp.h`

## core/moonshine-cpp.h
- Layer: utility
- Doc: ifndef MOONSHINE_CPP_H define MOONSHINE_CPP_H  Moonshine C++ API - Header-only library
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
  - `onLineStarted` (function, line 15) `* public:
 *     void onLineStarted(const moonshine::LineStarted& event) override`
  - `onLineCompleted` (function, line 19) `*     void onLineCompleted(const moonshine::LineCompleted& event) override`
  - `main` (function, line 23) `*
 * int main()`
  - `WordTiming` (function, line 92) `WordTiming() : start(0.0f), end(0.0f), confidence(0.0f)`
  - `WordTiming` (function, line 94) `WordTiming(const std::string &word, float start, float end, float confidence)
      : word(word),...`
  - `SpeakerSpan` (function, line 119) `SpeakerSpan()
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
  - `toString` (function, line 232) `std::string toString() const`
  - `Transcript` (function, line 269) `Transcript()`
  - `Transcript` (function, line 272) `Transcript(const transcript_t *transcript_c)`
  - `toString` (function, line 282) `std::string toString() const`
  - `TranscriptEvent` (function, line 318) `protected:
  TranscriptEvent(const TranscriptLine &line, int32_t streamHandle, Type type)
      :...`
  - `LineStarted` (function, line 326) `public:
  LineStarted(const TranscriptLine &line, int32_t streamHandle)
      : TranscriptEvent(l...`
  - `LineUpdated` (function, line 333) `public:
  LineUpdated(const TranscriptLine &line, int32_t streamHandle)
      : TranscriptEvent(l...`
  - `LineTextChanged` (function, line 340) `public:
  LineTextChanged(const TranscriptLine &line, int32_t streamHandle)
      : TranscriptEve...`
  - `LineSpeakersChanged` (function, line 350) `public:
  LineSpeakersChanged(const TranscriptLine &line, int32_t streamHandle)
      : Transcrip...`
  - `LineCompleted` (function, line 357) `public:
  LineCompleted(const TranscriptLine &line, int32_t streamHandle)
      : TranscriptEvent...`
  - `Error` (function, line 367) `Error(const std::string &errorMessage, int32_t streamHandle)
      : TranscriptEvent(TranscriptLi...`
  - `Error` (function, line 371) `Error(const std::string &errorMessage, const TranscriptLine &line,
        int32_t streamHandle)
...`
  - `onLineStarted` (function, line 390) `virtual void onLineStarted(const LineStarted &)`
  - `onLineUpdated` (function, line 393) `virtual void onLineUpdated(const LineUpdated &)`
  - `onLineTextChanged` (function, line 396) `virtual void onLineTextChanged(const LineTextChanged &)`
  - `onLineSpeakersChanged` (function, line 400) `virtual void onLineSpeakersChanged(const LineSpeakersChanged &)`
  - `onLineCompleted` (function, line 403) `virtual void onLineCompleted(const LineCompleted &)`
  - `onError` (function, line 406) `virtual void onError(const Error &)`
  - `MoonshineException` (function, line 413) `public:
  MoonshineException(const std::string &message)
      : std::runtime_error(message)`
  - `getHandle` (function, line 489) `int32_t getHandle() const`
  - `getHandle` (function, line 641) `int32_t getHandle() const`
  - `Transcriber` (function, line 646) `Transcriber(int32_t handle, ModelArch modelArch, double updateInterval)
      : handle_(handle),
...`
  - `TtsSynthesisResult` (function, line 672) `TtsSynthesisResult() : sampleRateHz(0)`
  - `TtsSynthesisResult` (function, line 674) `TtsSynthesisResult(std::vector<float> samples, int32_t sampleRateHz)
      : samples(std::move(sa...`
  - `getLanguage` (function, line 748) `const std::string &getLanguage() const`
  - `getHandle` (function, line 751) `int32_t getHandle() const`
  - `getLanguage` (function, line 834) `const std::string &getLanguage() const`
  - `getHandle` (function, line 837) `int32_t getHandle() const`
  - `IntentMatch` (function, line 863) `IntentMatch(std::string phrase, float sim)
      : canonicalPhrase(std::move(phrase)), similarity...`
  - `getHandle` (function, line 919) `int32_t getHandle() const`
  - `Stream` (function, line 932) `inline Stream::Stream(Transcriber *transcriber, double updateInterval,
                      uint...`
  - `Stream` (function, line 944) `inline Stream::Stream(Stream &&other)
    : transcriber_(other.transcriber_),
      handle_(other...`
  - `start` (function, line 970) `inline void Stream::start()`
  - `stop` (function, line 974) `inline void Stream::stop()`
  - `addAudio` (function, line 985) `inline void Stream::addAudio(const std::vector<float> &audioData,
                             in...`
  - `updateTranscription` (function, line 1001) `inline Transcript Stream::updateTranscription(uint32_t flags)`
  - `addListener` (function, line 1010) `inline void Stream::addListener(TranscriptEventListener *listener)`
  - `addListener` (function, line 1016) `inline void Stream::addListener(
    std::function<void(const TranscriptEvent &)> listener)`
  - `removeListener` (function, line 1021) `inline void Stream::removeListener(TranscriptEventListener *listener)`
  - `removeListener` (function, line 1027) `inline void Stream::removeListener(
    std::function<void(const TranscriptEvent &)> listener)`
  - `remove_if` (function, line 1034) `std::remove_if(
          functionListeners_.begin(), functionListeners_.end(),
          [&liste...`
  - `removeAllListeners` (function, line 1050) `inline void Stream::removeAllListeners()`
  - `close` (function, line 1055) `inline void Stream::close()`
  - `notifyFromTranscript` (function, line 1063) `inline void Stream::notifyFromTranscript(const Transcript &transcript)`
  - `emit` (function, line 1083) `inline void Stream::emit(const TranscriptEvent &event)`
  - `emitError` (function, line 1167) `inline void Stream::emitError(const std::string &errorMessage)`
  - `buildOptions` (function, line 1186) `inline OptionsBuffer buildOptions(
    const std::string &spellingModelPath,
    const std::vecto...`
  - `Transcriber` (function, line 1213) `inline Transcriber::Transcriber(const std::string &modelPath,
                                Mod...`
  - `Transcriber` (function, line 1225) `inline Transcriber::Transcriber(
    const std::string &modelPath, ModelArch modelArch, double up...`
  - `loadFromMemory` (function, line 1241) `inline Transcriber Transcriber::loadFromMemory(
    const uint8_t *encoderData, size_t encoderDat...`
  - `Transcriber` (function, line 1266) `inline Transcriber::Transcriber(Transcriber &&other)
    : handle_(other.handle_),
      modelPat...`
  - `close` (function, line 1294) `inline void Transcriber::close()`
  - `transcribeWithoutStreaming` (function, line 1302) `inline Transcript Transcriber::transcribeWithoutStreaming(
    const std::vector<float> &audioDat...`
  - `getVersion` (function, line 1317) `inline int32_t Transcriber::getVersion() const`
  - `createStream` (function, line 1321) `inline Stream Transcriber::createStream(double updateInterval, uint32_t flags)`
  - `getDefaultStream` (function, line 1325) `inline Stream &Transcriber::getDefaultStream()`
  - `start` (function, line 1332) `inline void Transcriber::start()`
  - `stop` (function, line 1334) `inline void Transcriber::stop()`
  - `addAudio` (function, line 1340) `inline void Transcriber::addAudio(const std::vector<float> &audioData,
                          ...`
  - `updateTranscription` (function, line 1345) `inline Transcript Transcriber::updateTranscription(uint32_t flags)`
  - `addListener` (function, line 1349) `inline void Transcriber::addListener(TranscriptEventListener *listener)`
  - `addListener` (function, line 1353) `inline void Transcriber::addListener(
    std::function<void(const TranscriptEvent &)> listener)`
  - `removeListener` (function, line 1358) `inline void Transcriber::removeListener(TranscriptEventListener *listener)`
  - `removeListener` (function, line 1364) `inline void Transcriber::removeListener(
    std::function<void(const TranscriptEvent &)> listener)`
  - `removeAllListeners` (function, line 1371) `inline void Transcriber::removeAllListeners()`
  - `parseTranscript` (function, line 1377) `inline Transcript Transcriber::parseTranscript(
    const transcript_t *transcript_c)`
  - `checkError` (function, line 1382) `inline void Transcriber::checkError(int32_t error) const`
  - `checkError` (function, line 1390) `inline void Stream::checkError(int32_t error) const`
  - `TextToSpeech` (function, line 1400) `inline TextToSpeech::TextToSpeech(
    const std::string &language, const std::vector<moonshine_o...`
  - `TextToSpeech` (function, line 1410) `inline TextToSpeech::TextToSpeech(TextToSpeech &&other)
    : handle_(other.handle_), language_(s...`
  - `synthesize` (function, line 1425) `inline TtsSynthesisResult TextToSpeech::synthesize(
    const std::string &text, const std::vecto...`
  - `synthesizeFromPhonemes` (function, line 1445) `inline TtsSynthesisResult TextToSpeech::synthesizeFromPhonemes(
    const std::string &phonemes,
...`
  - `close` (function, line 1466) `inline void TextToSpeech::close()`
  - `getVoices` (function, line 1473) `inline std::string TextToSpeech::getVoices(
    const std::string &languages,
    const std::vect...`
  - `getDependencies` (function, line 1493) `inline std::string TextToSpeech::getDependencies(
    const std::string &languages,
    const std...`
  - `checkError` (function, line 1513) `inline void TextToSpeech::checkError(int32_t error) const`
  - `GraphemeToPhonemizer` (function, line 1523) `inline GraphemeToPhonemizer::GraphemeToPhonemizer(
    const std::string &language, const std::ve...`
  - `GraphemeToPhonemizer` (function, line 1533) `inline GraphemeToPhonemizer::GraphemeToPhonemizer(GraphemeToPhonemizer &&other)
    : handle_(oth...`
  - `toIpa` (function, line 1549) `inline std::string GraphemeToPhonemizer::toIpa(
    const std::string &text, const std::vector<mo...`
  - `close` (function, line 1565) `inline void GraphemeToPhonemizer::close()`
  - `getDependencies` (function, line 1572) `inline std::string GraphemeToPhonemizer::getDependencies(
    const std::string &languages,
    c...`
  - `checkError` (function, line 1592) `inline void GraphemeToPhonemizer::checkError(int32_t error) const`
  - `IntentRecognizer` (function, line 1600) `inline IntentRecognizer::IntentRecognizer(const std::string &model_path,
                        ...`
  - `IntentRecognizer` (function, line 1611) `inline IntentRecognizer::IntentRecognizer(IntentRecognizer &&other) noexcept
    : handle_(other....`
  - `registerIntent` (function, line 1626) `inline void IntentRecognizer::registerIntent(
    const std::string &canonical_phrase, float *emb...`
  - `unregisterIntent` (function, line 1633) `inline bool IntentRecognizer::unregisterIntent(
    const std::string &canonical_phrase)`
  - `getClosestIntents` (function, line 1646) `inline std::vector<IntentMatch> IntentRecognizer::getClosestIntents(
    const std::string &utter...`
  - `intentCount` (function, line 1670) `inline int32_t IntentRecognizer::intentCount() const`
  - `clearIntents` (function, line 1680) `inline void IntentRecognizer::clearIntents()`
  - `calculateEmbedding` (function, line 1684) `inline std::vector<float> IntentRecognizer::calculateEmbedding(
    const std::string &sentence, ...`
  - `close` (function, line 1698) `inline void IntentRecognizer::close()`
  - `checkError` (function, line 1705) `inline void IntentRecognizer::checkError(int32_t error) const`
  - `transcriber` (function, line 25) `* moonshine::Transcriber transcriber("path/to/models", * moonshine::ModelArch::BASE);`
  - `to_string` (function, line 243) `std::to_string(span.duration) + "s speaker " + std::to_string(span.speakerIndex) + " (" + std::to_string(span.speakerId) + ") chars " + std::to_string(span.startChar) + "-" + std::to_string(span.endCh`
  - `line` (function, line 278) `TranscriptLine line(transcript_c->lines[i]);`
  - `remove` (function, line 1024) `std::remove(objectListeners_.begin(), objectListeners_.end(), listener), objectListeners_.end());`
  - `moonshine_free_stream` (function, line 1058) `moonshine_free_stream(transcriber_->handle_, handle_);`
  - `errorEvent` (function, line 1114) `Error errorEvent(e.what(), handle_);`
  - `funcListener` (function, line 1126) `funcListener(errorEvent);`
  - `listener` (function, line 1140) `listener(event);`
  - `otherFuncListener` (function, line 1155) `otherFuncListener(errorEvent);`
  - `moonshine_free_transcriber` (function, line 1298) `moonshine_free_transcriber(handle_);`
  - `moonshine_get_version` (function, line 1319) `return moonshine_get_version();`
  - `free` (function, line 1440) `std::free(out_audio);`
  - `moonshine_free_tts_synthesizer` (function, line 1469) `moonshine_free_tts_synthesizer(handle_);`
  - `string` (function, line 1561) `return std::string(out_phonemes, out_count);`
  - `moonshine_free_grapheme_to_phonemizer` (function, line 1568) `moonshine_free_grapheme_to_phonemizer(handle_);`
  - `moonshine_free_intent_matches` (function, line 1656) `moonshine_free_intent_matches(matches, count);`
  - `moonshine_free_intent_embedding` (function, line 1694) `moonshine_free_intent_embedding(out_embedding);`
  - `moonshine_free_intent_recognizer` (function, line 1701) `moonshine_free_intent_recognizer(handle_);`
  - `MOONSHINE_CPP_H` (macro, line 2) `#define MOONSHINE_CPP_H`
- Depends on: `core/moonshine-c-api.h`
- Imported by: `core/benchmark.cpp`, `core/moonshine-cpp-test.cpp`, `examples/windows/cli-transcriber/cli-transcriber.cpp`

## core/moonshine-download-smoke.cpp
- Layer: utility
- Doc: moonshine-download-smoke: a tiny CLI used by scripts/test-model-downloads.sh to verify that the native download manifest
- Language: cpp
- Symbols:
  - `print_usage` (function, line 44) `void print_usage()`
  - `url_encode_path` (function, line 52) `std::string url_encode_path(const std::string& key)`
  - `fail` (function, line 72) `int fail(const std::string& message)`
  - `print_group_manifest` (function, line 82) `void print_group_manifest(const std::string& json_text)`
  - `manifest_stt` (function, line 92) `int manifest_stt(const std::vector<std::string>& spec)`
  - `manifest_intent` (function, line 114) `int manifest_intent(const std::vector<std::string>& spec)`
  - `manifest_tts` (function, line 134) `int manifest_tts(const std::vector<std::string>& spec)`
  - `manifest_g2p` (function, line 165) `int manifest_g2p(const std::vector<std::string>& spec)`
  - `load_speech_or_tone` (function, line 196) `std::vector<float> load_speech_or_tone()`
  - `is_streaming_arch` (function, line 233) `bool is_streaming_arch(uint32_t arch)`
  - `run_stt` (function, line 240) `int run_stt(const std::string& root, const std::vector<std::string>& spec)`
  - `run_intent` (function, line 294) `int run_intent(const std::string& root, const std::vector<std::string>& spec)`
  - `run_tts` (function, line 322) `int run_tts(const std::string& root, const std::vector<std::string>& spec)`
  - `run_g2p` (function, line 360) `int run_g2p(const std::string& root, const std::vector<std::string>& spec)`
  - `main` (function, line 387) `int main(int argc, char** argv)`
  - `free` (function, line 111) `std::free(out);`
  - `moonshine_get_g2p_dependencies` (function, line 172) `moonshine_get_g2p_dependencies(spec[0].c_str(), nullptr, 0, &out);`
  - `csv` (function, line 176) `const std::string csv(out);`
  - `audio` (function, line 218) `std::vector<float> audio(data, data + used);`
  - `moonshine_free_transcriber` (function, line 262) `moonshine_free_transcriber(handle);`
  - `moonshine_start_stream` (function, line 265) `moonshine_start_stream(handle, stream);`
  - `moonshine_stop_stream` (function, line 276) `moonshine_stop_stream(handle, stream);`
  - `moonshine_free_stream` (function, line 277) `moonshine_free_stream(handle, stream);`
  - `moonshine_register_intent` (function, line 304) `moonshine_register_intent(handle, "turn on the lights", nullptr, 0, 0);`
  - `moonshine_free_intent_recognizer` (function, line 306) `moonshine_free_intent_recognizer(handle);`
  - `moonshine_free_intent_matches` (function, line 318) `moonshine_free_intent_matches(matches, count);`
  - `moonshine_free_tts_synthesizer` (function, line 351) `moonshine_free_tts_synthesizer(handle);`
  - `moonshine_free_grapheme_to_phonemizer` (function, line 378) `moonshine_free_grapheme_to_phonemizer(handle);`
- Depends on: `core/moonshine-c-api.h`, `core/moonshine-utils/debug-utils.h`

## core/moonshine-model-catalog.cpp
- Layer: business_logic
- Doc: include "moonshine-model-catalog.h"  include <algorithm> include <cctype>  include "moonshine-c-api.h"
- Language: cpp
- Symbols:
  - `SttModelEntry` (struct, line 17)
  - `SttLanguageEntry` (struct, line 22)
  - `SpellingModelEntry` (struct, line 28)
  - `EmbeddingModelEntry` (struct, line 33)
  - `to_lower` (function, line 39) `std::string to_lower(std::string s)`
  - `transform` (function, line 41) `std::transform(s.begin(), s.end(), s.begin(), [](unsigned char c)`
  - `is_streaming_arch` (function, line 46) `bool is_streaming_arch(int32_t model_arch)`
  - `stt_catalog` (function, line 56) `const std::vector<SttLanguageEntry>& stt_catalog()`
  - `embedding_catalog` (function, line 123) `const std::vector<EmbeddingModelEntry>& embedding_catalog()`
  - `find_stt_language` (function, line 132) `const SttLanguageEntry* find_stt_language(const std::string& language)`
  - `stt_component_files` (function, line 147) `std::vector<std::string> stt_component_files(const std::string& language_code,
                  ...`
  - `find_spelling_model` (function, line 169) `const SpellingModelEntry* find_spelling_model(const std::string& language_code)`
  - `find_embedding_model` (function, line 178) `const EmbeddingModelEntry* find_embedding_model(const std::string& model_name)`
  - `embedding_component_files` (function, line 194) `std::vector<std::string> embedding_component_files(const std::string& variant)`
  - `stt_model_dependencies` (function, line 213) `std::optional<ModelDependencies> stt_model_dependencies(
    const std::string& language, std::op...`
  - `intent_model_dependencies` (function, line 250) `std::optional<ModelDependencies> intent_model_dependencies(
    const std::string& model_name, co...`
  - `stt_supported_languages` (function, line 272) `std::vector<std::string> stt_supported_languages()`
  - `intent_supported_models` (function, line 280) `std::vector<std::string> intent_supported_models()`
  - `intent_supported_variants` (function, line 288) `std::vector<std::string> intent_supported_variants(
    const std::string& model_name)`
- Depends on: `core/moonshine-c-api.h`, `core/moonshine-model-catalog.h`

## core/moonshine-model-catalog.h
- Layer: business_logic
- Doc: ifndef MOONSHINE_MODEL_CATALOG_H define MOONSHINE_MODEL_CATALOG_H  Native catalog of downloadable model assets (speech-t
- Language: h
- Symbols:
  - `ModelDependencyGroup` (struct, line 24)
  - `ModelDependencies` (struct, line 29)
  - `stt_model_dependencies` (function, line 44) `std::optional<ModelDependencies> stt_model_dependencies( const std::string& language, std::optional<int32_t> model_arch, bool include_spelling);`
  - `intent_model_dependencies` (function, line 54) `std::optional<ModelDependencies> intent_model_dependencies( const std::string& model_name, const std::string& variant);`
  - `stt_supported_languages` (function, line 58) `std::vector<std::string> stt_supported_languages();`
  - `intent_supported_models` (function, line 61) `std::vector<std::string> intent_supported_models();`
  - `intent_supported_variants` (function, line 64) `std::vector<std::string> intent_supported_variants(const std::string& model_name);`
  - `MOONSHINE_MODEL_CATALOG_H` (macro, line 2) `#define MOONSHINE_MODEL_CATALOG_H`
- Imported by: `core/moonshine-c-api.cpp`, `core/moonshine-model-catalog.cpp`

## core/moonshine-model.cpp
- Layer: business_logic
- Doc: include "moonshine-model.h"  include <fcntl.h>  include <cassert> include <cctype> include <cerrno> include <cerrno>  //
- Language: cpp
- Symbols:
  - `set_model_options_from_arch` (function, line 60) `int set_model_options_from_arch(MoonshineModel *model, int32_t model_arch)`
  - `MoonshineModel` (function, line 81) `MoonshineModel::MoonshineModel(
    bool log_ort_run, float max_tokens_per_second,
    const std:...`
  - `load` (function, line 144) `int MoonshineModel::load(const char *encoder_model_path,
                         const char *dec...`
  - `load_from_memory` (function, line 162) `int MoonshineModel::load_from_memory(const uint8_t *encoder_model_data,
                         ...`
  - `load_from_assets` (function, line 186) `int MoonshineModel::load_from_assets(const char *encoder_model_path,
                            ...`
  - `transcribe` (function, line 215) `int MoonshineModel::transcribe(const float *input_audio_data,
                               size...`
  - `transcribe_wav` (function, line 564) `int MoonshineModel::transcribe_wav(const char *wav_path, char **out_text)`
  - `load_alignment_model` (function, line 579) `int MoonshineModel::load_alignment_model(const char *alignment_model_path)`
  - `compute_word_timestamps` (function, line 590) `int MoonshineModel::compute_word_timestamps(
    float audio_duration, std::vector<TranscriberWor...`
  - `LOGF` (function, line 72) `LOGF( "Invalid model architecture: %d, must be MOONSHINE_MODEL_ARCH_TINY (0) " "or MOONSHINE_MODEL_ARCH_BASE (1)\n", model_arch);`
  - `LOG_ORT_ERROR` (function, line 92) `LOG_ORT_ERROR(ort_api, ort_api->CreateEnv(ORT_LOGGING_LEVEL_WARNING, "MoonshineModel", &ort_env));`
  - `ort_maybe_force_single_thread` (function, line 106) `ort_maybe_force_single_thread(ort_api, ort_session_options);`
  - `ort_configure_execution_providers` (function, line 122) `ort_configure_execution_providers(ort_api, ort_session_options, ort_provider_names, coreml_cache_dir);`
  - `munmap` (function, line 137) `munmap(const_cast<char *>(encoder_mmapped_data), encoder_mmapped_data_size);`
  - `RETURN_ON_ERROR` (function, line 148) `RETURN_ON_ERROR(set_model_options_from_arch(this, model_type));`
  - `RETURN_ON_NULL` (function, line 153) `RETURN_ON_NULL(encoder_session);`
  - `LOG` (function, line 222) `LOG("Audio data is nullptr or empty");`
  - `RETURN_ON_ORT_ERROR` (function, line 226) `RETURN_ON_ORT_ERROR(ort_api, ort_api->SessionGetInputCount( encoder_session, &encoder_input_count));`
  - `encoder_input_names` (function, line 231) `std::vector<char *> encoder_input_names(encoder_input_count);`
  - `encoder_output_names` (function, line 232) `std::vector<char *> encoder_output_names(encoder_output_count);`
  - `ort_get_input_shape` (function, line 246) `ort_get_input_shape(ort_api, encoder_session, 0);`
  - `encoder_outputs` (function, line 268) `std::vector<OrtValue *> encoder_outputs(encoder_output_count);`
  - `memcpy` (function, line 300) `memcpy(last_encoder_hidden_states.data(), last_hidden_state_tensor->data<float>(), total * sizeof(float));`
  - `decoder_input_names` (function, line 325) `std::vector<const char *> decoder_input_names(decoder_input_count);`
  - `decoder_output_names` (function, line 338) `std::vector<const char *> decoder_output_names(decoder_output_count);`
  - `TENSOR_NAME` (function, line 364) `TENSOR_NAME(past_key_values_name));`
  - `decoder_inputs_data` (function, line 382) `std::vector<MoonshineTensorView *> decoder_inputs_data(decoder_input_count);`
  - `MoonshineTensorView` (function, line 388) `new MoonshineTensorView(input_ids_shape, MOONSHINE_DTYPE_INT64, inputIDs.data(), TENSOR_NAME("input_ids"));`
  - `RETURN_ON_FALSE` (function, line 418) `RETURN_ON_FALSE(decoder_input_name_to_index.find(key) != decoder_input_name_to_index.end());`
  - `decoder_outputs` (function, line 442) `std::vector<OrtValue *> decoder_outputs(decoder_output_count);`
  - `assert` (function, line 467) `assert(decoder_output_name_to_index.find(present_key_values_name) != decoder_output_name_to_index.end());`
  - `attn_view` (function, line 486) `MoonshineTensorView attn_view(ort_api, decoder_outputs[attn_index], "cross_attn");`
  - `tokens_int` (function, line 601) `std::vector<int> tokens_int(last_tokens.begin(), last_tokens.end());`
  - `rearranged` (function, line 613) `std::vector<float> rearranged(L * H * total_steps * E);`
  - `output_names_alloc` (function, line 679) `std::vector<char *> output_names_alloc(align_output_count);`
  - `output_names` (function, line 686) `std::vector<const char *> output_names(align_output_count);`
  - `outputs` (function, line 692) `std::vector<OrtValue *> outputs(align_output_count, nullptr);`
  - `ORT_RUN` (function, line 695) `ORT_RUN(ort_api, alignment_session, input_names.data(), inputs, 2, output_names.data(), align_output_count, outputs.data());`
  - `attn_shape` (function, line 732) `std::vector<int64_t> attn_shape(attn_ndims);`
  - `cross_attention_data` (function, line 744) `std::vector<float> cross_attention_data(attn_layers * per_layer);`
  - `align_words` (function, line 769) `align_words(cross_attention_data.data(), attn_layers, num_heads, dec_len, enc_len, tokens_int, time_per_frame, tokenizer);`
  - `DEBUG_ALLOC_ENABLED` (macro, line 35) `#define DEBUG_ALLOC_ENABLED`
  - `MOONSHINE_TINY_NUM_LAYERS` (macro, line 41) `#define MOONSHINE_TINY_NUM_LAYERS`
  - `MOONSHINE_TINY_NUM_KV_HEADS` (macro, line 42) `#define MOONSHINE_TINY_NUM_KV_HEADS`
  - `MOONSHINE_TINY_HEAD_DIM` (macro, line 43) `#define MOONSHINE_TINY_HEAD_DIM`
  - `MOONSHINE_TINY_PAST_ELEMENT_COUNT` (macro, line 44) `#define MOONSHINE_TINY_PAST_ELEMENT_COUNT`
  - `MOONSHINE_BASE_NUM_LAYERS` (macro, line 49) `#define MOONSHINE_BASE_NUM_LAYERS`
  - `MOONSHINE_BASE_NUM_KV_HEADS` (macro, line 50) `#define MOONSHINE_BASE_NUM_KV_HEADS`
  - `MOONSHINE_BASE_HEAD_DIM` (macro, line 51) `#define MOONSHINE_BASE_HEAD_DIM`
  - `MOONSHINE_BASE_PAST_ELEMENT_COUNT` (macro, line 52) `#define MOONSHINE_BASE_PAST_ELEMENT_COUNT`
  - `MOONSHINE_DECODER_START_TOKEN_ID` (macro, line 55) `#define MOONSHINE_DECODER_START_TOKEN_ID`
  - `MOONSHINE_EOS_TOKEN_ID` (macro, line 57) `#define MOONSHINE_EOS_TOKEN_ID`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/moonshine-model.h`, `core/moonshine-utils/debug-utils.h`, `core/moonshine-utils/string-utils.h`, `core/ort-utils/moonshine-ort-allocator.h`, `core/ort-utils/moonshine-tensor-view.h`, `core/ort-utils/ort-utils.h`

## core/moonshine-model.h
- Layer: business_logic
- Doc: ifndef MOONSHINE_MODEL_H define MOONSHINE_MODEL_H  include <stddef.h> include <stdint.h>  include <mutex> include <strin
- Language: h
- Symbols:
  - `MoonshineModel` (struct, line 17)
  - `load` (function, line 71) `int load(const char *encoder_model_path, const char *decoder_model_path, const char *tokenizer_path, int32_t model_type);`
  - `load_alignment_model` (function, line 74) `int load_alignment_model(const char *alignment_model_path);`
  - `load_from_memory` (function, line 76) `int load_from_memory(const uint8_t *encoder_model_data, size_t encoder_model_data_size, const uint8_t *decoder_model_data, size_t decoder_model_data_size, const uint8_t *tokenizer_data, size_t tokeniz`
  - `load_from_assets` (function, line 85) `int load_from_assets(const char *encoder_model_path, const char *decoder_model_path, const char *tokenizer_path, int32_t model_type, AAssetManager *assetManager);`
  - `transcribe` (function, line 90) `int transcribe(const float *input_audio_data, size_t input_audio_data_size, char **out_text);`
  - `transcribe_wav` (function, line 93) `int transcribe_wav(const char *wav_path, char **out_text);`
  - `compute_word_timestamps` (function, line 101) `int compute_word_timestamps(float audio_duration, std::vector<TranscriberWord> &words_out);`
  - `MOONSHINE_MODEL_H` (macro, line 2) `#define MOONSHINE_MODEL_H`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/moonshine-c-api.h`, `core/ort-utils/moonshine-ort-allocator.h`, `core/word-alignment.h`
- Imported by: `core/moonshine-c-api.cpp`, `core/moonshine-model.cpp`

## core/moonshine-streaming-model.cpp
- Layer: business_logic
- Doc: include "moonshine-streaming-model.h"  include <fcntl.h>  include <cassert> include <cmath> include <cstdio> include <cs
- Language: cpp
- Symbols:
  - `read_file_to_string` (function, line 48) `static std::string read_file_to_string(const std::string &path)`
  - `parse_config_json` (function, line 58) `static bool parse_config_json(const std::string &json,
                              MoonshineStr...`
  - `reset` (function, line 106) `void MoonshineStreamingState::reset(const MoonshineStreamingConfig &cfg)`
  - `MoonshineStreamingModel` (function, line 145) `MoonshineStreamingModel::MoonshineStreamingModel(
    bool log_ort_run, const std::vector<std::st...`
  - `load_config` (function, line 199) `int MoonshineStreamingModel::load_config(const char *config_path)`
  - `load_config_from_string` (function, line 208) `int MoonshineStreamingModel::load_config_from_string(const std::string &json)`
  - `load` (function, line 216) `int MoonshineStreamingModel::load(const char *model_dir,
                                  const ...`
  - `load_from_memory` (function, line 289) `int MoonshineStreamingModel::load_from_memory(
    const uint8_t *frontend_model_data, size_t fro...`
  - `load_from_assets` (function, line 332) `int MoonshineStreamingModel::load_from_assets(const char *model_dir,
                            ...`
  - `create_state` (function, line 404) `MoonshineStreamingState *MoonshineStreamingModel::create_state()`
  - `tokens_to_text` (function, line 410) `std::string MoonshineStreamingModel::tokens_to_text(
    const std::vector<int64_t> &tokens)`
  - `process_audio_chunk` (function, line 420) `int MoonshineStreamingModel::process_audio_chunk(MoonshineStreamingState *state,
                ...`
  - `encode` (function, line 583) `int MoonshineStreamingModel::encode(MoonshineStreamingState *state,
                             ...`
  - `compute_cross_kv` (function, line 758) `int MoonshineStreamingModel::compute_cross_kv(MoonshineStreamingState *state)`
  - `run_decoder_with_cross_kv` (function, line 846) `int MoonshineStreamingModel::run_decoder_with_cross_kv(
    MoonshineStreamingState *state, const...`
  - `decode_step` (function, line 1068) `int MoonshineStreamingModel::decode_step(MoonshineStreamingState *state,
                        ...`
  - `decode_tokens` (function, line 1115) `int MoonshineStreamingModel::decode_tokens(MoonshineStreamingState *state,
                      ...`
  - `decode_full` (function, line 1171) `int MoonshineStreamingModel::decode_full(MoonshineStreamingState *state,
                        ...`
  - `decoder_reset` (function, line 1343) `void MoonshineStreamingModel::decoder_reset(MoonshineStreamingState *state)`
  - `f` (function, line 50) `std::ifstream f(path);`
  - `LOG_ORT_ERROR` (function, line 157) `LOG_ORT_ERROR(ort_api, ort_api->CreateEnv(ORT_LOGGING_LEVEL_WARNING, "MoonshineStreamingModel", &ort_env));`
  - `ort_maybe_force_single_thread` (function, line 166) `ort_maybe_force_single_thread(ort_api, ort_session_options);`
  - `ort_configure_execution_providers` (function, line 169) `ort_configure_execution_providers(ort_api, ort_session_options, ort_provider_names, coreml_cache_dir);`
  - `memset` (function, line 171) `memset(&config, 0, sizeof(config));`
  - `munmap` (function, line 188) `munmap(const_cast<char *>(frontend_mmapped_data), frontend_mmapped_data_size);`
  - `LOGF` (function, line 203) `LOGF("Failed to read config file: %s\n", config_path);`
  - `LOG` (function, line 211) `LOG("Failed to parse streaming config JSON\n");`
  - `append_path_component` (function, line 230) `append_path_component(model_dir, "streaming_config.json");`
  - `RETURN_ON_ERROR` (function, line 233) `RETURN_ON_ERROR(load_config(config_path.c_str()));`
  - `RETURN_ON_NULL` (function, line 239) `RETURN_ON_NULL(frontend_session);`
  - `AAssetManager_open` (function, line 353) `AAssetManager_open(assetManager, config_path.c_str(), AASSET_MODE_BUFFER);`
  - `config_json` (function, line 359) `std::string config_json(config_size, '\0');`
  - `AAsset_read` (function, line 360) `AAsset_read(config_asset, &config_json[0], config_size);`
  - `AAsset_close` (function, line 361) `AAsset_close(config_asset);`
  - `lock` (function, line 438) `std::lock_guard<std::mutex> lock(processing_mutex);`
  - `audio_vec` (function, line 442) `std::vector<float> audio_vec(audio_chunk, audio_chunk + chunk_len);`
  - `RETURN_ON_ORT_ERROR` (function, line 452) `RETURN_ON_ORT_ERROR( ort_api, ort_api->CreateTensorWithDataAsOrtValue( ort_memory_info, audio_vec.data(), audio_vec.size() * sizeof(float), audio_shape.data(), audio_shape.size(), ONNX_TENSOR_ELEMENT_`
  - `feat_shape` (function, line 529) `std::vector<int64_t> feat_shape(num_dims);`
  - `memcpy` (function, line 552) `memcpy(state->sample_buffer.data(), sample_buffer_out, 79 * sizeof(float));`
  - `max` (function, line 606) `: std::max(0, total_features - config.total_lookahead);`
  - `ORT_RUN` (function, line 650) `ORT_RUN(ort_api, encoder_session, enc_input_names, &features_tensor, 1, enc_output_names, 1, enc_outputs);`
  - `enc_shape` (function, line 667) `std::vector<int64_t> enc_shape(num_dims);`
  - `new_encoded` (function, line 685) `std::vector<float> new_encoded(new_frames * config.encoder_dim);`
  - `k_shape` (function, line 803) `std::vector<int64_t> k_shape(num_dims);`
  - `token_data` (function, line 865) `std::vector<int64_t> token_data(tokens.begin(), tokens.end());`
  - `output_names_alloc` (function, line 932) `std::vector<char *> output_names_alloc(decoder_output_count);`
  - `outputs` (function, line 945) `std::vector<OrtValue *> outputs(decoder_output_count, nullptr);`
  - `attn_shape` (function, line 1022) `std::vector<int64_t> attn_shape(attn_ndims);`
  - `token_vec` (function, line 1137) `std::vector<int64_t> token_vec(tokens_len);`
  - `continue_ar_decoding` (function, line 1290) `continue_ar_decoding(final_pred);`
  - `DEBUG_ALLOC_ENABLED` (macro, line 23) `#define DEBUG_ALLOC_ENABLED`
  - `MOONSHINE_STREAMING_TINY_ENCODER_DIM` (macro, line 29) `#define MOONSHINE_STREAMING_TINY_ENCODER_DIM`
  - `MOONSHINE_STREAMING_TINY_DECODER_DIM` (macro, line 30) `#define MOONSHINE_STREAMING_TINY_DECODER_DIM`
  - `MOONSHINE_STREAMING_TINY_DEPTH` (macro, line 31) `#define MOONSHINE_STREAMING_TINY_DEPTH`
  - `MOONSHINE_STREAMING_TINY_NHEADS` (macro, line 32) `#define MOONSHINE_STREAMING_TINY_NHEADS`
  - `MOONSHINE_STREAMING_TINY_HEAD_DIM` (macro, line 33) `#define MOONSHINE_STREAMING_TINY_HEAD_DIM`
  - `MOONSHINE_STREAMING_BASE_ENCODER_DIM` (macro, line 34) `#define MOONSHINE_STREAMING_BASE_ENCODER_DIM`
  - `MOONSHINE_STREAMING_BASE_DECODER_DIM` (macro, line 36) `#define MOONSHINE_STREAMING_BASE_DECODER_DIM`
  - `MOONSHINE_STREAMING_BASE_DEPTH` (macro, line 37) `#define MOONSHINE_STREAMING_BASE_DEPTH`
  - `MOONSHINE_STREAMING_BASE_NHEADS` (macro, line 38) `#define MOONSHINE_STREAMING_BASE_NHEADS`
  - `MOONSHINE_STREAMING_BASE_HEAD_DIM` (macro, line 39) `#define MOONSHINE_STREAMING_BASE_HEAD_DIM`
  - `MOONSHINE_DECODER_START_TOKEN_ID` (macro, line 40) `#define MOONSHINE_DECODER_START_TOKEN_ID`
  - `MOONSHINE_EOS_TOKEN_ID` (macro, line 42) `#define MOONSHINE_EOS_TOKEN_ID`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/moonshine-streaming-model.h`, `core/moonshine-utils/debug-utils.h`, `core/moonshine-utils/string-utils.h`, `core/ort-utils/moonshine-ort-allocator.h`, `core/ort-utils/ort-utils.h`

## core/moonshine-streaming-model.h
- Layer: business_logic
- Doc: ifndef MOONSHINE_STREAMING_MODEL_H define MOONSHINE_STREAMING_MODEL_H  include <stddef.h> include <stdint.h>  include <m
- Language: h
- Symbols:
  - `MoonshineStreamingConfig` (struct, line 17)
  - `MoonshineStreamingState` (struct, line 35)
  - `MoonshineStreamingModel` (struct, line 72)
  - `reset` (function, line 68) `void reset(const MoonshineStreamingConfig &cfg);`
  - `load` (function, line 116) `int load(const char *model_dir, const char *tokenizer_path, int32_t model_type);`
  - `load_from_memory` (function, line 119) `int load_from_memory( const uint8_t *frontend_model_data, size_t frontend_model_data_size, const uint8_t *encoder_model_data, size_t encoder_model_data_size, const uint8_t *adapter_model_data, size_t `
  - `load_from_assets` (function, line 130) `int load_from_assets(const char *model_dir, const char *tokenizer_path, int32_t model_type, AAssetManager *assetManager);`
  - `transcribe` (function, line 135) `int transcribe(const float *input_audio_data, size_t input_audio_data_size, char **out_text);`
  - `process_audio_chunk` (function, line 139) `int process_audio_chunk(MoonshineStreamingState *state, const float *audio_chunk, size_t chunk_len, int *features_out);`
  - `encode` (function, line 142) `int encode(MoonshineStreamingState *state, bool is_final, int *new_frames_out);`
  - `decode_step` (function, line 147) `int decode_step(MoonshineStreamingState *state, int token, float *logits_out);`
  - `decode_full` (function, line 161) `int decode_full(MoonshineStreamingState *state, const int *speculative_tokens, int speculative_len, int **tokens_out, int *tokens_len_out);`
  - `decoder_reset` (function, line 163) `void decoder_reset(MoonshineStreamingState *state);`
  - `create_state` (function, line 167) `MoonshineStreamingState *create_state();`
  - `tokens_to_text` (function, line 170) `std::string tokens_to_text(const std::vector<int64_t> &tokens);`
  - `load_config` (function, line 171) `private: int load_config(const char *config_path);`
  - `load_config_from_string` (function, line 174) `int load_config_from_string(const std::string &json);`
  - `run_decoder_with_cross_kv` (function, line 177) `int run_decoder_with_cross_kv(MoonshineStreamingState *state, const std::vector<int64_t> &tokens, std::vector<float> &logits_out);`
  - `compute_cross_kv` (function, line 182) `int compute_cross_kv(MoonshineStreamingState *state);`
  - `MOONSHINE_STREAMING_MODEL_H` (macro, line 2) `#define MOONSHINE_STREAMING_MODEL_H`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/ort-utils/moonshine-ort-allocator.h`, `core/word-alignment.h`
- Imported by: `core/moonshine-streaming-model.cpp`

## core/resampler-test.cpp
- Layer: testing
- Doc: include "resampler.h"  include <filesystem> include <numeric> include <string>  include "debug-utils.h"  define DOCTEST_
- Language: cpp
- Symbols:
  - `test_resample_audio` (function, line 13) `void test_resample_audio(const std::vector<float> &input_audio,
                         int32_t ...`
  - `TEST_CASE` (function, line 43) `TEST_CASE("resampler-test")`
  - `SUBCASE` (function, line 45) `SUBCASE("resample-audio")`
  - `resample_audio` (function, line 17) `resample_audio(input_audio, input_sample_rate, output_sample_rate);`
  - `max_element` (function, line 20) `*std::max_element(input_audio.begin(), input_audio.end());`
  - `LOGF` (function, line 23) `LOGF("Original max: %f, Resampled max: %f", original_max, resampled_max);`
  - `REQUIRE` (function, line 24) `REQUIRE(original_max == doctest::Approx(resampled_max).epsilon(0.005f));`
  - `min_element` (function, line 27) `*std::min_element(input_audio.begin(), input_audio.end());`
  - `accumulate` (function, line 34) `std::accumulate(input_audio.begin(), input_audio.end(), 0.0f) / input_audio.size();`
  - `wav_data_vector` (function, line 55) `const std::vector<float> wav_data_vector(wav_data, wav_data + wav_data_size);`
  - `LOG` (function, line 57) `LOG("Downsampling to 16000 Hz");`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 8) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-utils/debug-utils.h`, `core/resampler.h`

## core/resampler.cpp
- Layer: utility
- Doc: include "resampler.h"  include "debug-utils.h"
- Language: cpp
- Symbols:
  - `resample_audio` (function, line 4) `const std::vector<float> resample_audio(const std::vector<float> &audio,
                        ...`
  - `downsample_audio` (function, line 16) `const std::vector<float> downsample_audio(const std::vector<float> &audio,
                      ...`
  - `upsample_audio` (function, line 55) `const std::vector<float> upsample_audio(const std::vector<float> &audio,
                        ...`
  - `output_audio` (function, line 23) `std::vector<float> output_audio(output_audio_size);`
- Depends on: `core/moonshine-utils/debug-utils.h`, `core/resampler.h`

## core/resampler.h
- Layer: utility
- Doc: ifndef RESAMPLER_H define RESAMPLER_H  include <vector>
- Language: h
- Symbols:
  - `resample_audio` (function, line 5) `const std::vector<float> resample_audio(const std::vector<float> &audio, float input_sample_rate, float output_sample_rate);`
  - `downsample_audio` (function, line 9) `const std::vector<float> downsample_audio(const std::vector<float> &audio, float input_sample_rate, float output_sample_rate);`
  - `upsample_audio` (function, line 13) `const std::vector<float> upsample_audio(const std::vector<float> &audio, float input_sample_rate, float output_sample_rate);`
  - `RESAMPLER_H` (macro, line 2) `#define RESAMPLER_H`
- Imported by: `core/reliability/fuzz-resampler.cpp`, `core/resampler-test.cpp`, `core/resampler.cpp`, `core/voice-activity-detector.cpp`

## core/silero-vad.cpp
- Layer: utility
- Doc: include "silero-vad.h"  include "ort-utils.h" include "silero-vad-model-data.h"
- Language: cpp
- Symbols:
  - `init_onnx_env` (function, line 5) `void SileroVad::init_onnx_env()`
  - `init_engine_threads` (function, line 21) `void SileroVad::init_engine_threads(int inter_threads, int intra_threads)`
  - `SileroVad` (function, line 29) `SileroVad::SileroVad(int sample_rate, int windows_frame_size, float threshold,
                  ...`
  - `load_from_memory` (function, line 59) `int SileroVad::load_from_memory(const uint8_t *model_data,
                                size_t...`
  - `predict` (function, line 78) `void SileroVad::predict(const std::vector<float> &data_chunk,
                        float *out_...`
  - `LOG_ORT_ERROR` (function, line 8) `LOG_ORT_ERROR(ort_api, ort_api->CreateEnv(ORT_LOGGING_LEVEL_WARNING, "SileroVAD", &env));`
  - `ort_session_from_memory` (function, line 63) `return ort_session_from_memory(ort_api, env, session_options, model_data, model_data_size, &session);`
  - `copy` (function, line 83) `std::copy(_context.begin(), _context.end(), input.begin());`
  - `fprintf` (function, line 99) `fprintf(stderr, "CreateTensorWithDataAsOrtValue (input) failed: %s\n", msg);`
  - `memcpy` (function, line 158) `std::memcpy(_state.data(), stateN, size_state * sizeof(float));`
- Depends on: `core/ort-utils/ort-utils.h`, `core/silero-vad.h`

## core/silero-vad.h
- Layer: utility
- Doc: include <chrono> include <cmath>  // for std::rint include <cstdarg> include <cstdio> include <cstring> include <iomanip
- Language: h
- Symbols:
  - `SileroVad` (class, line 22)
  - `is_loaded` (function, line 84) `bool is_loaded() const`
  - `init_onnx_env` (function, line 68) `void init_onnx_env();`
  - `init_engine_threads` (function, line 71) `void init_engine_threads(int inter_threads, int intra_threads);`
  - `SileroVad` (function, line 72) `public: SileroVad( int sample_rate = 16000, int windows_frame_size = 32, float threshold = 0.5, int min_silence_duration_ms = 100, int speech_pad_ms = 30, int min_speech_duration_ms = 250, float max_s`
  - `load_from_memory` (function, line 83) `int load_from_memory(const uint8_t *model_data, size_t model_data_size);`
  - `predict` (function, line 86) `void predict(const std::vector<float> &data_chunk, float *out_probability, int *out_flag);`
- Imported by: `core/silero-vad.cpp`, `core/voice-activity-detector.h`

## core/speaker-diarizer.cpp
- Layer: infrastructure
- Doc: include "speaker-diarizer.h"  include <algorithm> include <map> include <mutex> include <random> include <stdexcept> inc
- Language: cpp
- Symbols:
  - `StreamState` (struct, line 43)
  - `turn_overlap_seconds` (function, line 17) `double turn_overlap_seconds(
    const std::vector<cppannote::StreamingDiarizationTurn> &a, int32...`
  - `Impl` (function, line 66) `explicit Impl(const SpeakerDiarizerOptions &options_in)
      : engine(), options(options_in)`
  - `session_config` (function, line 74) `cppannote::StreamingDiarizationConfig session_config() const`
  - `get_stream` (function, line 82) `StreamState &get_stream(int32_t stream_id)`
  - `allocate_stable_id` (function, line 91) `uint64_t allocate_stable_id()`
  - `map_snapshot_to_stable_ids` (function, line 102) `void map_snapshot_to_stable_ids(
      StreamState &state,
      const cppannote::StreamingDiariz...`
  - `sort` (function, line 135) `std::sort(candidates.begin(), candidates.end(),
              [](const auto &a, const auto &b)`
  - `SpeakerDiarizer` (function, line 170) `SpeakerDiarizer::SpeakerDiarizer(const SpeakerDiarizerOptions &options)
    : impl(std::make_uniq...`
  - `create_stream` (function, line 175) `int32_t SpeakerDiarizer::create_stream()`
  - `free_stream` (function, line 185) `void SpeakerDiarizer::free_stream(int32_t stream_id)`
  - `start_stream` (function, line 190) `void SpeakerDiarizer::start_stream(int32_t stream_id)`
  - `add_audio_to_stream` (function, line 200) `void SpeakerDiarizer::add_audio_to_stream(int32_t stream_id,
                                    ...`
  - `get_turns` (function, line 217) `std::vector<SpeakerTurn> SpeakerDiarizer::get_turns(int32_t stream_id)`
  - `finish_stream` (function, line 224) `std::vector<SpeakerTurn> SpeakerDiarizer::finish_stream(int32_t stream_id)`
  - `diarize` (function, line 235) `std::vector<SpeakerTurn> SpeakerDiarizer::diarize(const float *audio_data,
                      ...`
  - `min` (function, line 31) `std::min(ta.end, tb.end) - std::max(ta.start, tb.start);`
  - `runtime_error` (function, line 86) `throw std::runtime_error("SpeakerDiarizer: invalid stream ID " + std::to_string(stream_id));`
  - `lock` (function, line 177) `std::lock_guard<std::mutex> lock(this->impl->mutex);`
  - `LOGF` (function, line 214) `LOGF("Speaker diarization refresh failed (will retry): %s", e.what());`
- Depends on: `core/cpp-annote/src/cpp-annote-engine.h`, `core/cpp-annote/src/cpp-annote-streaming.h`, `core/moonshine-utils/debug-utils.h`, `core/speaker-diarizer.h`

## core/speaker-diarizer.h
- Layer: infrastructure
- Doc: ifndef SPEAKER_DIARIZER_H define SPEAKER_DIARIZER_H  include <cstdint> include <memory> include <vector>  One contiguous
- Language: h
- Symbols:
  - `SpeakerTurn` (struct, line 10)
  - `SpeakerDiarizerOptions` (struct, line 24)
  - `Impl` (struct, line 74)
  - `SpeakerDiarizer` (class, line 42)
  - `SpeakerDiarizer` (function, line 43) `public: explicit SpeakerDiarizer( const SpeakerDiarizerOptions &options = SpeakerDiarizerOptions());`
  - `create_stream` (function, line 50) `int32_t create_stream();`
  - `free_stream` (function, line 52) `void free_stream(int32_t stream_id);`
  - `start_stream` (function, line 53) `void start_stream(int32_t stream_id);`
  - `add_audio_to_stream` (function, line 58) `void add_audio_to_stream(int32_t stream_id, const float *audio_data, uint64_t audio_length, int32_t sample_rate);`
  - `get_turns` (function, line 63) `std::vector<SpeakerTurn> get_turns(int32_t stream_id);`
  - `finish_stream` (function, line 67) `std::vector<SpeakerTurn> finish_stream(int32_t stream_id);`
  - `diarize` (function, line 70) `std::vector<SpeakerTurn> diarize(const float *audio_data, uint64_t audio_length, int32_t sample_rate);`
  - `SPEAKER_DIARIZER_H` (macro, line 2) `#define SPEAKER_DIARIZER_H`
- Imported by: `core/speaker-diarizer.cpp`

## core/spelling-fusion-data.cpp
- Layer: data_access
- Doc: include "spelling-fusion-data.h"  include <algorithm>  include "spelling-fusion.h"
- Language: cpp
- Symbols:
  - `build_set` (function, line 27) `std::unordered_set<std::string> build_set(
    std::initializer_list<const char *> phrases)`
  - `upper_modifiers` (function, line 267) `const std::unordered_set<std::string> &upper_modifiers()`
  - `upper_modifiers_by_length` (function, line 280) `const std::vector<std::string> &upper_modifiers_by_length()`
  - `sort` (function, line 287) `std::sort(v.begin(), v.end(),
              [](const std::string &a, const std::string &b)`
  - `undo_words` (function, line 295) `const std::unordered_set<std::string> &undo_words()`
  - `clear_words` (function, line 308) `const std::unordered_set<std::string> &clear_words()`
  - `stop_words` (function, line 318) `const std::unordered_set<std::string> &stop_words()`
  - `default_weak_homonyms` (function, line 337) `const std::unordered_set<std::string> &default_weak_homonyms()`
  - `default_meta` (function, line 355) `const DefaultSpellingMeta &default_meta()`
  - `v` (function, line 286) `std::vector<std::string> v(set.begin(), set.end());`
- Depends on: `core/spelling-fusion-data.h`, `core/spelling-fusion.h`

## core/spelling-fusion-data.h
- Layer: data_access
- Doc: ifndef SPELLING_FUSION_DATA_H define SPELLING_FUSION_DATA_H  include <string> include <unordered_map> include <unordered
- Language: h
- Symbols:
  - `DefaultSpellingMeta` (struct, line 53)
  - `sources` (function, line 10) `from the Python sources (alphanumeric_listener.py);`
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
- Doc: include "spelling-fusion.h"  include <string>  include "spelling-fusion-data.h"  define DOCTEST_CONFIG_IMPLEMENT_WITH_MA
- Language: cpp
- Symbols:
  - `char_match` (function, line 13) `SpellingMatch char_match(const std::string &c)`
  - `no_match` (function, line 21) `SpellingMatch no_match()`
  - `TEST_CASE` (function, line 24) `TEST_CASE("spelling-fusion: normalize")`
  - `TEST_CASE` (function, line 38) `TEST_CASE("spelling-fusion: matcher classifies plain letters")`
  - `TEST_CASE` (function, line 49) `TEST_CASE("spelling-fusion: matcher classifies NATO codewords")`
  - `TEST_CASE` (function, line 60) `TEST_CASE("spelling-fusion: matcher classifies digits")`
  - `TEST_CASE` (function, line 72) `TEST_CASE("spelling-fusion: matcher parses 10..1000 number words")`
  - `TEST_CASE` (function, line 84) `TEST_CASE("spelling-fusion: matcher applies upper-case modifier")`
  - `TEST_CASE` (function, line 93) `TEST_CASE("spelling-fusion: matcher recognizes speller patterns")`
  - `TEST_CASE` (function, line 102) `TEST_CASE("spelling-fusion: matcher classifies command words")`
  - `TEST_CASE` (function, line 113) `TEST_CASE("spelling-fusion: matcher classifies special characters")`
  - `TEST_CASE` (function, line 148) `TEST_CASE("spelling-fusion: weak-homonym detection")`
  - `TEST_CASE` (function, line 157) `TEST_CASE("spelling-fusion: fuse without prediction")`
  - `TEST_CASE` (function, line 165) `TEST_CASE("spelling-fusion: fuse drops unrecognized + no prediction")`
  - `TEST_CASE` (function, line 172) `TEST_CASE("spelling-fusion: fuse passes through command words")`
  - `TEST_CASE` (function, line 182) `TEST_CASE(
    "spelling-fusion: special-character match is preserved when the "
    "spelling mo...`
  - `TEST_CASE` (function, line 203) `TEST_CASE("spelling-fusion: weak-homonym demotion")`
  - `TEST_CASE` (function, line 224) `TEST_CASE("spelling-fusion: cross-class routing")`
  - `TEST_CASE` (function, line 237) `TEST_CASE("spelling-fusion: same-class disagreement uses threshold")`
  - `TEST_CASE` (function, line 250) `TEST_CASE("spelling-fusion: multi-digit ASR vs single-digit spelling")`
  - `TEST_CASE` (function, line 274) `TEST_CASE("spelling-fusion: agreement preserves matcher casing")`
  - `TEST_CASE` (function, line 283) `TEST_CASE("spelling-fusion: spelling-only when matcher misses")`
  - `TEST_CASE` (function, line 292) `TEST_CASE("spelling-fusion: data tables are non-empty")`
  - `CHECK` (function, line 26) `CHECK(spelling_normalize("") == "");`
  - `CHECK_FALSE` (function, line 91) `CHECK_FALSE(matcher.classify("capital").is_recognized());`
  - `fuse_default` (function, line 199) `fuse_default("dollar sign", char_match("$"), nullptr, matcher);`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 6) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/spelling-fusion-data.h`, `core/spelling-fusion.h`

## core/spelling-fusion.cpp
- Layer: utility
- Doc: include "spelling-fusion.h"  include <algorithm> include <array> include <cctype> include <cstdint> include <cstring> in
- Language: cpp
- Symbols:
  - `is_ascii_drop` (function, line 24) `bool is_ascii_drop(char c)`
  - `is_ascii_letter` (function, line 34) `bool is_ascii_letter(char c)`
  - `ascii_to_lower` (function, line 38) `char ascii_to_lower(char c)`
  - `consume_curly_quote` (function, line 46) `size_t consume_curly_quote(const std::string &input, size_t i)`
  - `split_on_whitespace` (function, line 62) `std::vector<std::string> split_on_whitespace(const std::string &s)`
  - `parse_number_words` (function, line 107) `std::optional<int> parse_number_words(const std::string &text)`
  - `is_ascii_digit_string` (function, line 180) `bool is_ascii_digit_string(const std::string &s)`
  - `is_printable_ascii` (function, line 188) `bool is_printable_ascii(char c)`
  - `spelling_normalize` (function, line 194) `std::string spelling_normalize(const std::string &text)`
  - `SpellingMatcher` (function, line 233) `SpellingMatcher::SpellingMatcher()
    : lookup_(&spelling_fusion_data::lookup_table()),
      up...`
  - `classify` (function, line 243) `SpellingMatch SpellingMatcher::classify(const std::string &raw_text) const`
  - `is_weak_homonym` (function, line 299) `bool SpellingMatcher::is_weak_homonym(const std::string &raw_text) const`
  - `resolve` (function, line 304) `std::optional<std::string> SpellingMatcher::resolve(
    const std::string &text) const`
  - `resolve_spelled_letter` (function, line 325) `std::optional<std::string> SpellingMatcher::resolve_spelled_letter(
    const std::string &text) ...`
  - `string_is_letter` (function, line 373) `bool string_is_letter(const std::string &c)`
  - `string_is_digit` (function, line 380) `bool string_is_digit(const std::string &c)`
  - `single_char_is_letter` (function, line 388) `bool single_char_is_letter(const std::string &c)`
  - `apply_case` (function, line 392) `std::string apply_case(const std::string &ch, const std::string &hint)`
  - `fuse_default` (function, line 406) `FusedResult fuse_default(const std::string &raw_text,
                         const SpellingMatc...`
  - `to_string` (function, line 315) `return std::to_string(*num);`
  - `trim` (function, line 348) `trim(left);`
- Depends on: `core/spelling-fusion-data.h`, `core/spelling-fusion.h`

## core/spelling-fusion.h
- Layer: utility
- Doc: ifndef SPELLING_FUSION_H define SPELLING_FUSION_H  include <optional> include <string> include <unordered_map> include <
- Language: h
- Symbols:
  - `SpellingMatch` (struct, line 34)
  - `SpellingPrediction` (struct, line 47)
  - `FusedResult` (struct, line 88)
  - `SpellingMatchType` (enum, line 26)
  - `SpellingMatchType` (class, line 26)
  - `SpellingMatcher` (class, line 53)
  - `is_character` (function, line 40) `bool is_character() const`
  - `is_recognized` (function, line 42) `bool is_recognized() const`
  - `is_character` (function, line 91) `bool is_character() const`
  - `SpellingMatcher` (function, line 54) `public: SpellingMatcher();`
  - `classify` (function, line 59) `SpellingMatch classify(const std::string &raw_text) const;`
  - `is_weak_homonym` (function, line 66) `bool is_weak_homonym(const std::string &raw_text) const;`
  - `resolve` (function, line 77) `std::optional<std::string> resolve(const std::string &text) const;`
  - `resolve_spelled_letter` (function, line 79) `std::optional<std::string> resolve_spelled_letter( const std::string &text) const;`
  - `fuse_default` (function, line 108) `FusedResult fuse_default(const std::string &raw_text, const SpellingMatch &match, const SpellingPrediction *prediction, const SpellingMatcher &matcher);`
  - `spelling_normalize` (function, line 116) `std::string spelling_normalize(const std::string &text);`
  - `SPELLING_FUSION_H` (macro, line 2) `#define SPELLING_FUSION_H`
- Imported by: `core/spelling-fusion-data.cpp`, `core/spelling-fusion-test.cpp`, `core/spelling-fusion.cpp`, `core/spelling-model-test.cpp`, `core/spelling-model.h`

## core/spelling-model-test.cpp
- Layer: business_logic
- Doc: include "spelling-model.h"  include <cstdio> include <filesystem> include <fstream> include <string> include <vector>  i
- Language: cpp
- Symbols:
  - `Clip` (struct, line 99)
  - `find_model_path` (function, line 21) `std::string find_model_path()`
  - `find_wav` (function, line 32) `std::string find_wav(const std::string &label, const std::string &filename)`
  - `read_file` (function, line 47) `std::vector<uint8_t> read_file(const std::string &path)`
  - `TEST_CASE` (function, line 59) `TEST_CASE("spelling-model: load from path")`
  - `TEST_CASE` (function, line 72) `TEST_CASE("spelling-model: load from memory")`
  - `TEST_CASE` (function, line 85) `TEST_CASE("spelling-model: predict on bundled clips")`
  - `TEST_CASE` (function, line 132) `TEST_CASE("spelling-model: invalid arguments are rejected")`
  - `stream` (function, line 48) `std::ifstream stream(path, std::ios::binary | std::ios::ate);`
  - `buffer` (function, line 53) `std::vector<uint8_t> buffer(static_cast<size_t>(size));`
  - `REQUIRE` (function, line 67) `REQUIRE(model.load(path.c_str()) == 0);`
  - `CHECK` (function, line 68) `CHECK(model.sample_rate() == 16000);`
  - `REQUIRE_FALSE` (function, line 80) `REQUIRE_FALSE(data.empty());`
  - `free` (function, line 120) `free(audio);`
  - `INFO` (function, line 123) `INFO("clip=" << clip.label << " predicted=" << prediction.character << " p=" << prediction.probability);`
  - `dummy` (function, line 143) `std::vector<float> dummy(16000, 0.0f);`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 11) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-utils/debug-utils.h`, `core/spelling-fusion.h`, `core/spelling-model.h`

## core/spelling-model.cpp
- Layer: business_logic
- Doc: include "spelling-model.h"  ifndef _WIN32 include <sys/mman.h> include <sys/stat.h> include <unistd.h> endif  include <a
- Language: cpp
- Symbols:
  - `lookup_metadata` (function, line 26) `std::optional<std::string> lookup_metadata(const OrtApi *ort_api,
                               ...`
  - `trim` (function, line 45) `std::string trim(const std::string &s)`
  - `parse_class_list_json` (function, line 59) `std::vector<std::string> parse_class_list_json(const std::string &raw)`
  - `SpellingModel` (function, line 94) `SpellingModel::SpellingModel(bool log_ort_run,
                             const std::vector<std...`
  - `initialize_session_options` (function, line 136) `void SpellingModel::initialize_session_options()`
  - `apply_default_metadata` (function, line 156) `void SpellingModel::apply_default_metadata()`
  - `load` (function, line 168) `int SpellingModel::load(const char *model_path)`
  - `load_from_memory` (function, line 176) `int SpellingModel::load_from_memory(const uint8_t *model_data,
                                  ...`
  - `populate_metadata_from_session` (function, line 185) `int SpellingModel::populate_metadata_from_session()`
  - `predict` (function, line 242) `int SpellingModel::predict(const float *audio, size_t audio_size,
                           int3...`
  - `out` (function, line 38) `std::string out(raw);`
  - `LOG_ORT_ERROR` (function, line 102) `LOG_ORT_ERROR(ort_api_, ort_api_->CreateEnv(ORT_LOGGING_LEVEL_WARNING, "SpellingModel", &ort_env_));`
  - `munmap` (function, line 130) `munmap(const_cast<char *>(mmapped_data_), mmapped_data_size_);`
  - `ort_maybe_force_single_thread` (function, line 140) `ort_maybe_force_single_thread(ort_api_, ort_session_options_);`
  - `ort_configure_execution_providers` (function, line 153) `ort_configure_execution_providers(ort_api_, ort_session_options_, ort_provider_names_, coreml_cache_dir_);`
  - `RETURN_ON_ERROR` (function, line 170) `RETURN_ON_ERROR(ort_session_from_path( ort_api_, ort_env_, ort_session_options_, model_path, &ort_session_, &mmapped_data_, &mmapped_data_size_));`
  - `RETURN_ON_NULL` (function, line 173) `RETURN_ON_NULL(ort_session_);`
  - `LOGF` (function, line 253) `LOGF("SpellingModel::predict sample_rate mismatch: got %d, expected %d", sample_rate, sample_rate_);`
  - `lock` (function, line 257) `std::lock_guard<std::mutex> lock(processing_mutex_);`
  - `clip` (function, line 259) `std::vector<float> clip(target_samples_, 0.0f);`
  - `copy` (function, line 262) `std::copy(audio, audio + copy_count, clip.begin());`
  - `ORT_RUN` (function, line 276) `ORT_RUN(ort_api_, ort_session_, input_names, &input_value, 1, output_names, 1, &output_value);`
  - `output_view` (function, line 289) `MoonshineTensorView output_view(ort_api_, output_value, "spelling_logits");`
  - `probs` (function, line 307) `std::vector<float> probs(row_size);`
  - `to_string` (function, line 326) `: std::to_string(best_idx);`
- Depends on: `core/moonshine-utils/debug-utils.h`, `core/ort-utils/moonshine-tensor-view.h`, `core/ort-utils/ort-utils.h`, `core/spelling-fusion-data.h`, `core/spelling-model.h`

## core/spelling-model.h
- Layer: business_logic
- Doc: ifndef SPELLING_MODEL_H define SPELLING_MODEL_H  include <stddef.h> include <stdint.h>  include <mutex> include <string>
- Language: h
- Symbols:
  - `SpellingModel` (class, line 24)
  - `sample_rate` (function, line 56) `int32_t sample_rate() const`
  - `clip_seconds` (function, line 57) `float clip_seconds() const`
  - `classes` (function, line 58) `const std::vector<std::string> &classes() const`
  - `load` (function, line 39) `int load(const char *model_path);`
  - `load_from_memory` (function, line 43) `int load_from_memory(const uint8_t *model_data, size_t model_data_size);`
  - `predict` (function, line 52) `int predict(const float *audio, size_t audio_size, int32_t sample_rate, SpellingPrediction *out_prediction);`
  - `initialize_session_options` (function, line 59) `private: void initialize_session_options();`
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
  - `read_rss_kb` (function, line 53) `size_t read_rss_kb()`
  - `median` (function, line 89) `size_t median(std::vector<size_t> values)`
  - `env_size` (function, line 98) `size_t env_size(const char *name, size_t default_value)`
  - `detect_continual_growth` (function, line 117) `bool detect_continual_growth(const std::vector<size_t> &samples,
                             siz...`
  - `create_synth` (function, line 222) `int32_t create_synth(const EngineSpec &spec)`
  - `synth_once` (function, line 235) `bool synth_once(int32_t handle, size_t text_index)`
  - `reload_strict` (function, line 247) `bool reload_strict()`
  - `run_growth_phase` (function, line 259) `void run_growth_phase(const std::string &label, size_t iterations,
                      const st...`
  - `exercise_engine` (function, line 293) `void exercise_engine(const EngineSpec &spec)`
  - `run_growth_phase` (function, line 306) `run_growth_phase(
        std::string(spec.name) + " synth", synth_iterations,
        [handle](s...`
  - `run_growth_phase` (function, line 322) `run_growth_phase(
      std::string(spec.name) + " reload", reload_iterations,
      [&spec](size...`
  - `file_present` (function, line 338) `bool file_present(const fs::path &p)`
  - `kokoro_spec` (function, line 343) `std::optional<EngineSpec> kokoro_spec()`
  - `piper_spec` (function, line 354) `std::optional<EngineSpec> piper_spec()`
  - `zipvoice_spec` (function, line 388) `std::optional<EngineSpec> zipvoice_spec()`
  - `TEST_CASE` (function, line 406) `TEST_CASE("tts-repeated-memory-kokoro")`
  - `TEST_CASE` (function, line 415) `TEST_CASE("tts-repeated-memory-piper")`
  - `TEST_CASE` (function, line 425) `TEST_CASE("tts-repeated-memory-zipvoice")`
  - `discover_data_root` (function, line 439) `std::optional<fs::path> discover_data_root()`
  - `main` (function, line 463) `int main(int argc, char **argv)`
  - `fclose` (function, line 75) `std::fclose(f);`
  - `nth_element` (function, line 95) `std::nth_element(values.begin(), values.begin() + mid, values.end());`
  - `max` (function, line 155) `std::max(absolute_tolerance, relative_tolerance);`
  - `moonshine_create_tts_synthesizer_from_files` (function, line 230) `return moonshine_create_tts_synthesizer_from_files( spec.language, nullptr, 0, opts, static_cast<uint64_t>(sizeof(opts) / sizeof(opts[0])), MOONSHINE_HEADER_VERSION);`
  - `moonshine_text_to_speech` (function, line 241) `moonshine_text_to_speech(handle, kTexts[text_index % kTextCount], nullptr, 0, &audio, &audio_n, &sr);`
  - `free` (function, line 244) `std::free(audio);`
  - `REQUIRE_MESSAGE` (function, line 267) `REQUIRE_MESSAGE(body(i), label << ": iteration " << i << " failed");`
  - `MESSAGE` (function, line 275) `MESSAGE(label << ": " << report);`
  - `printf` (function, line 278) `std::printf(" %s sample[%zu]: rss=%zu KiB\n", label.c_str(), i, rss_samples[i]);`
  - `fflush` (function, line 281) `std::fflush(stdout);`
  - `CHECK_FALSE_MESSAGE` (function, line 290) `CHECK_FALSE_MESSAGE(growing, label << " shows sustained RSS growth: " << report);`
  - `moonshine_free_tts_synthesizer` (function, line 313) `moonshine_free_tts_synthesizer(handle);`
  - `is_regular_file` (function, line 341) `return fs::is_regular_file(p, ec);`
  - `fprintf` (function, line 487) `std::fprintf(stderr, "error: could not locate core/moonshine-tts/data. Pass its " "absolute path as the first argument, or run from the repo " "root / test-assets.\n");`
  - `DOCTEST_CONFIG_IMPLEMENT` (macro, line 26) `#define DOCTEST_CONFIG_IMPLEMENT`
- Depends on: `core/moonshine-c-api.h`

## core/voice-activity-detector-test.cpp
- Layer: testing
- Doc: include "voice-activity-detector.h"  include <filesystem> include <string>  include "debug-utils.h"  define DOCTEST_CONF
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 10) `TEST_CASE("voice-activity-detector-test")`
  - `SUBCASE` (function, line 15) `SUBCASE("vad-block")`
  - `SUBCASE` (function, line 54) `SUBCASE("vad-stream")`
  - `SUBCASE` (function, line 122) `SUBCASE("vad-threshold-0")`
  - `create_directory` (function, line 13) `std::filesystem::create_directory("output");`
  - `REQUIRE` (function, line 17) `REQUIRE(std::filesystem::exists(wav_path));`
  - `save_wav_data` (function, line 30) `save_wav_data("output/vad_block_original.wav", wav_data, wav_data_size, wav_sample_rate);`
  - `LOGF` (function, line 35) `LOGF("Segments count: %zu", segments->size());`
  - `vad` (function, line 123) `VoiceActivityDetector vad(0.0f);`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 7) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-utils/debug-utils.h`, `core/voice-activity-detector.h`

## core/voice-activity-detector.cpp
- Layer: utility
- Doc: include "voice-activity-detector.h"  include <cassert> include <mutex> include <numeric>  include "debug-utils.h" includ
- Language: cpp
- Symbols:
  - `seconds_from_sample_count` (function, line 14) `float seconds_from_sample_count(size_t sample_count)`
  - `VoiceActivityDetector` (function, line 23) `VoiceActivityDetector::VoiceActivityDetector(float threshold,
                                   ...`
  - `start` (function, line 49) `void VoiceActivityDetector::start()`
  - `stop` (function, line 61) `void VoiceActivityDetector::stop()`
  - `process_audio` (function, line 68) `void VoiceActivityDetector::process_audio(const float *audio_data,
                              ...`
  - `clear_completed_segment_audio_data` (function, line 98) `void VoiceActivityDetector::clear_completed_segment_audio_data()`
  - `retained_segment_audio_byte_count` (function, line 106) `size_t VoiceActivityDetector::retained_segment_audio_byte_count() const`
  - `completed_segment_audio_byte_count` (function, line 114) `size_t VoiceActivityDetector::completed_segment_audio_byte_count() const`
  - `process_audio_chunk` (function, line 124) `void VoiceActivityDetector::process_audio_chunk(const float *audio_data,
                        ...`
  - `on_voice_start` (function, line 195) `void VoiceActivityDetector::on_voice_start()`
  - `on_voice_continuing` (function, line 209) `void VoiceActivityDetector::on_voice_continuing()`
  - `on_voice_end` (function, line 218) `void VoiceActivityDetector::on_voice_end()`
  - `to_string` (function, line 227) `std::string VoiceActivitySegment::to_string() const`
  - `to_string` (function, line 237) `std::string VoiceActivityDetector::to_string() const`
  - `input_audio_vector` (function, line 79) `std::vector<float> input_audio_vector(audio_data, audio_data + audio_data_size);`
  - `resample_audio` (function, line 83) `resample_audio(input_audio_vector, sample_rate, vad_sample_rate);`
  - `assert` (function, line 127) `assert(audio_data_size == (size_t)(hop_size));`
  - `move` (function, line 131) `std::move(look_behind_audio_buffer.begin() + audio_data_size, look_behind_audio_buffer.end(), look_behind_audio_buffer.begin());`
  - `copy` (function, line 133) `std::copy(audio_data, audio_data + audio_data_size, look_behind_audio_buffer.end() - audio_data_size);`
  - `audio_vec` (function, line 135) `std::vector<float> audio_vec(audio_data, audio_data + audio_data_size);`
  - `lock` (function, line 142) `std::lock_guard<std::mutex> lock(vad_mutex);`
  - `min` (function, line 174) `std::min(look_behind_sample_count, samples_processed_count);`
- Depends on: `core/moonshine-utils/debug-utils.h`, `core/resampler.h`, `core/voice-activity-detector.h`

## core/voice-activity-detector.h
- Layer: utility
- Doc: ifndef VOICE_ACTIVITY_DETECTOR_H define VOICE_ACTIVITY_DETECTOR_H  include <string> include <vector>  include "silero-va
- Language: h
- Symbols:
  - `VoiceActivitySegment` (struct, line 9)
  - `VoiceActivityDetector` (class, line 22)
  - `is_active` (function, line 53) `bool is_active() const`
  - `get_segments` (function, line 56) `const std::vector<VoiceActivitySegment> *get_segments() const`
  - `to_string` (function, line 19) `std::string to_string() const;`
  - `VoiceActivityDetector` (function, line 43) `public: VoiceActivityDetector(float threshold = 0.5f, int32_t window_size = 32, int32_t hop_size = 512, size_t look_behind_sample_count = 4096, size_t max_segment_sample_count = 15 * 16000);`
  - `start` (function, line 50) `void start();`
  - `stop` (function, line 52) `void stop();`
  - `process_audio` (function, line 54) `void process_audio(const float *audio_data, size_t audio_data_size, int32_t sample_rate);`
  - `retained_segment_audio_byte_count` (function, line 59) `size_t retained_segment_audio_byte_count() const;`
  - `completed_segment_audio_byte_count` (function, line 60) `size_t completed_segment_audio_byte_count() const;`
  - `clear_completed_segment_audio_data` (function, line 61) `void clear_completed_segment_audio_data();`
  - `clear` (function, line 63) `private: void clear();`
  - `on_voice_start` (function, line 66) `void on_voice_start();`
  - `on_voice_end` (function, line 67) `void on_voice_end();`
  - `on_voice_continuing` (function, line 68) `void on_voice_continuing();`
  - `process_audio_chunk` (function, line 69) `void process_audio_chunk(const float *audio_data, size_t audio_data_size);`
  - `VOICE_ACTIVITY_DETECTOR_H` (macro, line 2) `#define VOICE_ACTIVITY_DETECTOR_H`
- Depends on: `core/silero-vad.h`
- Imported by: `core/voice-activity-detector-test.cpp`, `core/voice-activity-detector.cpp`

## core/word-alignment-benchmark.cpp
- Layer: utility
- Doc: include <chrono> include <cstdio> include <cstdlib> include <cstring> include <vector>  include "file-utils.h" include "
- Language: cpp
- Symbols:
  - `BenchResult` (struct, line 31)
  - `load_wav` (function, line 9) `static float* load_wav(const char* path, long* num_samples_out)`
  - `run_benchmark` (function, line 37) `static BenchResult run_benchmark(const char* model_path, const char* wav_path,
                  ...`
  - `main` (function, line 96) `int main(int argc, char** argv)`
  - `fprintf` (function, line 13) `fprintf(stderr, "Cannot open %s\n", path);`
  - `exit` (function, line 14) `exit(1);`
  - `fseek` (function, line 16) `fseek(f, 0, SEEK_END);`
  - `fread_exact` (function, line 21) `fread_exact(raw, 1, data_size, f, "WAV PCM data");`
  - `fclose` (function, line 22) `fclose(f);`
  - `free` (function, line 26) `free(raw);`
  - `moonshine_transcribe_without_streaming` (function, line 62) `moonshine_transcribe_without_streaming(handle, audio, num_samples, 16000, 0, &t);`
  - `moonshine_free_transcriber` (function, line 86) `moonshine_free_transcriber(handle);`
  - `printf` (function, line 115) `printf("Audio: %s (%.2fs)\n", wav_path, dur);`
- Depends on: `core/moonshine-c-api.h`, `core/moonshine-utils/file-utils.h`

## core/word-alignment-test.cpp
- Layer: testing
- Doc: include <cstdio> include <cstdlib> include <filesystem> include <string>  include "debug-utils.h" include "moonshine-c-a
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 11) `TEST_CASE("word-timestamps")`
  - `SUBCASE` (function, line 13) `SUBCASE("non-streaming-transcribe-with-word-timestamps")`
  - `REQUIRE` (function, line 16) `REQUIRE(std::filesystem::exists(model_path));`
  - `moonshine_get_version` (function, line 27) `moonshine_get_version());`
  - `moonshine_free_transcriber` (function, line 69) `moonshine_free_transcriber(handle);`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 8) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/moonshine-c-api.h`, `core/moonshine-utils/debug-utils.h`

## core/word-alignment.cpp
- Layer: utility
- Doc: include "word-alignment.h"  include <algorithm> include <cmath> include <cstring> include <limits> include <numeric> inc
- Language: cpp
- Symbols:
  - `WordGroup` (struct, line 304)
  - `dtw` (function, line 11) `void dtw(const std::vector<float>& cost_matrix, int N, int M,
         std::vector<int>& text_ind...`
  - `compute_median` (function, line 92) `static float compute_median(std::vector<float>& window)`
  - `median_filter` (function, line 98) `void median_filter(std::vector<float>& data, int channels, int height,
                   int wid...`
  - `token_starts_new_word` (function, line 158) `static bool token_starts_new_word(BinTokenizer* tokenizer, int token_id)`
  - `decode_tokens` (function, line 173) `static std::string decode_tokens(BinTokenizer* tokenizer,
                                 const ...`
  - `align_words` (function, line 180) `std::vector<TranscriberWord> align_words(const float* cross_attention_data,
                     ...`
  - `D` (function, line 16) `std::vector<float> D((N + 1) * (M + 1), std::numeric_limits<float>::infinity());`
  - `trace` (function, line 22) `std::vector<int> trace(N * M, 0);`
  - `nth_element` (function, line 95) `std::nth_element(window.begin(), window.begin() + n / 2, window.end());`
  - `padded` (function, line 114) `std::vector<float> padded(padded_width);`
  - `window` (function, line 115) `std::vector<float> window(filter_width);`
  - `result_row` (function, line 116) `std::vector<float> result_row(width);`
  - `weights` (function, line 200) `std::vector<float> weights(total_size);`
  - `memcpy` (function, line 201) `std::memcpy(weights.data(), cross_attention_data, total_size * sizeof(float));`
  - `matrix` (function, line 250) `std::vector<float> matrix(n_steps * encoder_frames, 0.0f);`
  - `neg_matrix` (function, line 270) `std::vector<float> neg_matrix(matrix.size());`
- Depends on: `core/word-alignment.h`

## core/word-alignment.h
- Layer: utility
- Doc: ifndef WORD_ALIGNMENT_H define WORD_ALIGNMENT_H  include <string> include <vector>  include "bin-tokenizer/bin-tokenizer
- Language: h
- Symbols:
  - `TranscriberWord` (struct, line 9)
  - `dtw` (function, line 18) `void dtw(const std::vector<float>& cost_matrix, int N, int M, std::vector<int>& text_indices_out, std::vector<int>& time_indices_out);`
  - `median_filter` (function, line 24) `void median_filter(std::vector<float>& data, int channels, int height, int width, int filter_width);`
  - `align_words` (function, line 38) `std::vector<TranscriberWord> align_words(const float* cross_attention_data, int num_layers, int num_heads, int num_tokens, int encoder_frames, const std::vector<int>& tokens, float time_per_frame, Bin`
  - `WORD_ALIGNMENT_H` (macro, line 2) `#define WORD_ALIGNMENT_H`
- Depends on: `core/bin-tokenizer/bin-tokenizer.h`
- Imported by: `core/moonshine-model.h`, `core/moonshine-streaming-model.h`, `core/word-alignment.cpp`
