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
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 4)

## core/cosine-distance.cpp
- Layer: infrastructure
- Doc: include "cosine-distance.h"  include <cmath> include <stdexcept>
- Language: cpp
- Symbols:
  - `cosine_distance` (function, line 5) `float cosine_distance(const std::vector<float>& a,
                      const std::vector<float>...`

## core/cosine-distance.h
- Layer: infrastructure
- Doc: ifndef COSINE_DISTANCE_H_ define COSINE_DISTANCE_H_  include <vector>  Computes cosine distance between two vectors: 1 -
- Language: h
- Symbols:
  - `COSINE_DISTANCE_H_` (macro, line 2)

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
  - `EMBEDDING_MODEL_H` (macro, line 2)

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
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 6)

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
  - `DEBUG_ALLOC_ENABLED` (macro, line 16)

## core/gemma-embedding-model.h
- Layer: business_logic
- Doc: ifndef GEMMA_EMBEDDING_MODEL_H define GEMMA_EMBEDDING_MODEL_H  include <memory> include <mutex> include <string> include
- Language: h
- Symbols:
  - `GemmaEmbeddingConfig` (struct, line 17)
  - `GemmaEmbeddingModel` (class, line 31)
  - `GEMMA_EMBEDDING_MODEL_H` (macro, line 2)

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
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 12)

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

## core/intent-recognizer.h
- Layer: utility
- Doc: ifndef INTENT_RECOGNIZER_H define INTENT_RECOGNIZER_H  include <cstdint> include <memory> include <mutex> include <strin
- Language: h
- Symbols:
  - `IntentRecognizerOptions` (struct, line 23)
  - `Intent` (struct, line 37)
  - `EmbeddingModelArch` (class, line 16)
  - `IntentRecognizer` (class, line 48)
  - `INTENT_RECOGNIZER_H` (macro, line 2)

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
  - `DOCTEST_CONFIG_IMPLEMENT` (macro, line 6)

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
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 16)

## core/moonshine-c-api.cpp
- Layer: presentation
- Language: cpp
- Symbols:
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
  - `CHECK_TRANSCRIBER_HANDLE` (macro, line 70)
  - `CHECK_INTENT_RECOGNIZER_HANDLE` (macro, line 461)
  - `CHECK_TTS_SYNTHESIZER_HANDLE` (macro, line 856)
  - `CHECK_GRAPHEME_PHONEMIZER_HANDLE` (macro, line 1852)

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
  - `MOONSHINE_C_API_H` (macro, line 2)
  - `MOONSHINE_EXPORT` (macro, line 78)
  - `MOONSHINE_EXPORT` (macro, line 80)
  - `MOONSHINE_HEADER_VERSION` (macro, line 95)
  - `MOONSHINE_MODEL_ARCH_TINY` (macro, line 98)
  - `MOONSHINE_MODEL_ARCH_BASE` (macro, line 99)
  - `MOONSHINE_MODEL_ARCH_TINY_STREAMING` (macro, line 100)
  - `MOONSHINE_MODEL_ARCH_BASE_STREAMING` (macro, line 101)
  - `MOONSHINE_MODEL_ARCH_SMALL_STREAMING` (macro, line 102)
  - `MOONSHINE_MODEL_ARCH_MEDIUM_STREAMING` (macro, line 103)
  - `MOONSHINE_ERROR_NONE` (macro, line 106)
  - `MOONSHINE_ERROR_UNKNOWN` (macro, line 107)
  - `MOONSHINE_ERROR_INVALID_HANDLE` (macro, line 108)
  - `MOONSHINE_ERROR_INVALID_ARGUMENT` (macro, line 109)
  - `MOONSHINE_FLAG_FORCE_UPDATE` (macro, line 112)
  - `MOONSHINE_FLAG_SPELLING_MODE` (macro, line 126)
  - `MOONSHINE_EMBEDDING_MODEL_ARCH_GEMMA_300M` (macro, line 604)
  - `MOONSHINE_INTENT_MAX_MATCHES` (macro, line 608)

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
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 6)

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
  - `MOONSHINE_CPP_H` (macro, line 2)

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

## core/moonshine-model-catalog.h
- Layer: business_logic
- Doc: ifndef MOONSHINE_MODEL_CATALOG_H define MOONSHINE_MODEL_CATALOG_H  Native catalog of downloadable model assets (speech-t
- Language: h
- Symbols:
  - `ModelDependencyGroup` (struct, line 24)
  - `ModelDependencies` (struct, line 29)
  - `MOONSHINE_MODEL_CATALOG_H` (macro, line 2)

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
  - `DEBUG_ALLOC_ENABLED` (macro, line 35)
  - `MOONSHINE_TINY_NUM_LAYERS` (macro, line 41)
  - `MOONSHINE_TINY_NUM_KV_HEADS` (macro, line 42)
  - `MOONSHINE_TINY_HEAD_DIM` (macro, line 43)
  - `MOONSHINE_TINY_PAST_ELEMENT_COUNT` (macro, line 44)
  - `MOONSHINE_BASE_NUM_LAYERS` (macro, line 49)
  - `MOONSHINE_BASE_NUM_KV_HEADS` (macro, line 50)
  - `MOONSHINE_BASE_HEAD_DIM` (macro, line 51)
  - `MOONSHINE_BASE_PAST_ELEMENT_COUNT` (macro, line 52)
  - `MOONSHINE_DECODER_START_TOKEN_ID` (macro, line 55)
  - `MOONSHINE_EOS_TOKEN_ID` (macro, line 57)

## core/moonshine-model.h
- Layer: business_logic
- Doc: ifndef MOONSHINE_MODEL_H define MOONSHINE_MODEL_H  include <stddef.h> include <stdint.h>  include <mutex> include <strin
- Language: h
- Symbols:
  - `MoonshineModel` (struct, line 17)
  - `MOONSHINE_MODEL_H` (macro, line 2)

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
  - `DEBUG_ALLOC_ENABLED` (macro, line 23)
  - `MOONSHINE_STREAMING_TINY_ENCODER_DIM` (macro, line 29)
  - `MOONSHINE_STREAMING_TINY_DECODER_DIM` (macro, line 30)
  - `MOONSHINE_STREAMING_TINY_DEPTH` (macro, line 31)
  - `MOONSHINE_STREAMING_TINY_NHEADS` (macro, line 32)
  - `MOONSHINE_STREAMING_TINY_HEAD_DIM` (macro, line 33)
  - `MOONSHINE_STREAMING_BASE_ENCODER_DIM` (macro, line 34)
  - `MOONSHINE_STREAMING_BASE_DECODER_DIM` (macro, line 36)
  - `MOONSHINE_STREAMING_BASE_DEPTH` (macro, line 37)
  - `MOONSHINE_STREAMING_BASE_NHEADS` (macro, line 38)
  - `MOONSHINE_STREAMING_BASE_HEAD_DIM` (macro, line 39)
  - `MOONSHINE_DECODER_START_TOKEN_ID` (macro, line 40)
  - `MOONSHINE_EOS_TOKEN_ID` (macro, line 42)

## core/moonshine-streaming-model.h
- Layer: business_logic
- Doc: ifndef MOONSHINE_STREAMING_MODEL_H define MOONSHINE_STREAMING_MODEL_H  include <stddef.h> include <stdint.h>  include <m
- Language: h
- Symbols:
  - `MoonshineStreamingConfig` (struct, line 17)
  - `MoonshineStreamingState` (struct, line 35)
  - `MoonshineStreamingModel` (struct, line 72)
  - `MOONSHINE_STREAMING_MODEL_H` (macro, line 2)

## core/resampler-test.cpp
- Layer: testing
- Doc: include "resampler.h"  include <filesystem> include <numeric> include <string>  include "debug-utils.h"  define DOCTEST_
- Language: cpp
- Symbols:
  - `test_resample_audio` (function, line 13) `void test_resample_audio(const std::vector<float> &input_audio,
                         int32_t ...`
  - `TEST_CASE` (function, line 43) `TEST_CASE("resampler-test")`
  - `SUBCASE` (function, line 45) `SUBCASE("resample-audio")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 8)

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

## core/resampler.h
- Layer: utility
- Doc: ifndef RESAMPLER_H define RESAMPLER_H  include <vector>
- Language: h
- Symbols:
  - `RESAMPLER_H` (macro, line 2)

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

## core/silero-vad.h
- Layer: utility
- Doc: include <chrono> include <cmath>  // for std::rint include <cstdarg> include <cstdio> include <cstring> include <iomanip
- Language: h
- Symbols:
  - `SileroVad` (class, line 22)
  - `is_loaded` (function, line 84) `bool is_loaded() const`

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

## core/speaker-diarizer.h
- Layer: infrastructure
- Doc: ifndef SPEAKER_DIARIZER_H define SPEAKER_DIARIZER_H  include <cstdint> include <memory> include <vector>  One contiguous
- Language: h
- Symbols:
  - `SpeakerTurn` (struct, line 10)
  - `SpeakerDiarizerOptions` (struct, line 24)
  - `Impl` (struct, line 74)
  - `SpeakerDiarizer` (class, line 42)
  - `SPEAKER_DIARIZER_H` (macro, line 2)

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

## core/spelling-fusion-data.h
- Layer: data_access
- Doc: ifndef SPELLING_FUSION_DATA_H define SPELLING_FUSION_DATA_H  include <string> include <unordered_map> include <unordered
- Language: h
- Symbols:
  - `DefaultSpellingMeta` (struct, line 53)
  - `SPELLING_FUSION_DATA_H` (macro, line 2)

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
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 6)

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

## core/spelling-fusion.h
- Layer: utility
- Doc: ifndef SPELLING_FUSION_H define SPELLING_FUSION_H  include <optional> include <string> include <unordered_map> include <
- Language: h
- Symbols:
  - `SpellingMatch` (struct, line 34)
  - `SpellingPrediction` (struct, line 47)
  - `FusedResult` (struct, line 88)
  - `SpellingMatchType` (class, line 26)
  - `SpellingMatcher` (class, line 53)
  - `is_character` (function, line 40) `bool is_character() const`
  - `is_recognized` (function, line 42) `bool is_recognized() const`
  - `is_character` (function, line 91) `bool is_character() const`
  - `SPELLING_FUSION_H` (macro, line 2)

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
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 11)

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

## core/spelling-model.h
- Layer: business_logic
- Doc: ifndef SPELLING_MODEL_H define SPELLING_MODEL_H  include <stddef.h> include <stdint.h>  include <mutex> include <string>
- Language: h
- Symbols:
  - `SpellingModel` (class, line 24)
  - `sample_rate` (function, line 56) `int32_t sample_rate() const`
  - `clip_seconds` (function, line 57) `float clip_seconds() const`
  - `classes` (function, line 58) `const std::vector<std::string> &classes() const`
  - `SPELLING_MODEL_H` (macro, line 2)

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
  - `DOCTEST_CONFIG_IMPLEMENT` (macro, line 26)

## core/voice-activity-detector-test.cpp
- Layer: testing
- Doc: include "voice-activity-detector.h"  include <filesystem> include <string>  include "debug-utils.h"  define DOCTEST_CONF
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 10) `TEST_CASE("voice-activity-detector-test")`
  - `SUBCASE` (function, line 15) `SUBCASE("vad-block")`
  - `SUBCASE` (function, line 54) `SUBCASE("vad-stream")`
  - `SUBCASE` (function, line 122) `SUBCASE("vad-threshold-0")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 7)

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

## core/voice-activity-detector.h
- Layer: utility
- Doc: ifndef VOICE_ACTIVITY_DETECTOR_H define VOICE_ACTIVITY_DETECTOR_H  include <string> include <vector>  include "silero-va
- Language: h
- Symbols:
  - `VoiceActivitySegment` (struct, line 9)
  - `VoiceActivityDetector` (class, line 22)
  - `is_active` (function, line 53) `bool is_active() const`
  - `get_segments` (function, line 56) `const std::vector<VoiceActivitySegment> *get_segments() const`
  - `VOICE_ACTIVITY_DETECTOR_H` (macro, line 2)

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

## core/word-alignment-test.cpp
- Layer: testing
- Doc: include <cstdio> include <cstdlib> include <filesystem> include <string>  include "debug-utils.h" include "moonshine-c-a
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 11) `TEST_CASE("word-timestamps")`
  - `SUBCASE` (function, line 13) `SUBCASE("non-streaming-transcribe-with-word-timestamps")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 8)

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

## core/word-alignment.h
- Layer: utility
- Doc: ifndef WORD_ALIGNMENT_H define WORD_ALIGNMENT_H  include <string> include <vector>  include "bin-tokenizer/bin-tokenizer
- Language: h
- Symbols:
  - `TranscriberWord` (struct, line 9)
  - `WORD_ALIGNMENT_H` (macro, line 2)
