# Subsystem: ort-utils

## core/ort-utils/moonshine-ort-allocator.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `MoonshineAlloc` (function, line 7) `void *MoonshineAlloc(struct OrtAllocator *this_, size_t size)`
  - `MoonshineFree` (function, line 15) `void MoonshineFree(struct OrtAllocator *this_, void *p)`
  - `MoonshineInfo` (function, line 22) `const struct OrtMemoryInfo *MoonshineInfo(const struct OrtAllocator *this_)`
  - `MoonshineReserve` (function, line 29) `void *MoonshineReserve(struct OrtAllocator *this_, size_t size)`
  - `MoonshineAllocOnStream` (function, line 35) `void *MoonshineAllocOnStream(struct OrtAllocator *this_, size_t size,
                           ...`
  - `friendlySizeString` (function, line 50) `void friendlySizeString(size_t byte_count, char *output, size_t output_size)`
  - `printFriendlySize` (function, line 65) `void printFriendlySize(const char *prefix, size_t number)`
  - `MoonshineOrtAllocator` (function, line 72) `MoonshineOrtAllocator::MoonshineOrtAllocator(const OrtMemoryInfo *memory_info)`
  - `print_stats` (function, line 93) `void MoonshineOrtAllocator::print_stats()`
  - `DEBUG_ALLOC_ENABLED` (macro, line 3) `#define DEBUG_ALLOC_ENABLED`
- Depends on: `core/moonshine-utils/debug-utils.h`, `core/ort-utils/moonshine-ort-allocator.h`

## core/ort-utils/moonshine-ort-allocator.h
- Layer: utility
- Language: h
- Symbols:
  - `MoonshineOrtAllocator` (struct, line 8)
  - `print_stats` (function, line 24) `void print_stats();`
  - `MOONSHINE_ORT_ALLOCATOR_H` (macro, line 2) `#define MOONSHINE_ORT_ALLOCATOR_H`
- Imported by: `core/gemma-embedding-model.h`, `core/moonshine-c-api.cpp`, `core/moonshine-model.cpp`, `core/moonshine-model.h`, `core/moonshine-streaming-model.cpp`, `core/moonshine-streaming-model.h`, `core/ort-utils/moonshine-ort-allocator.cpp`

## core/ort-utils/moonshine-tensor-view.cpp
- Layer: presentation
- Language: cpp
- Symbols:
  - `checked_mul` (function, line 18) `bool checked_mul(size_t a, size_t b, size_t *out)`
  - `moonshine_tensor_from_shape_and_dtype` (function, line 26) `moonshine_tensor_t *moonshine_tensor_from_shape_and_dtype(
    const std::vector<int64_t> &shape,...`
  - `moonshine_tensor_from_ort_tensor` (function, line 100) `moonshine_tensor_t *moonshine_tensor_from_ort_tensor(const OrtApi *ort_api,
                     ...`
  - `MoonshineTensorView` (function, line 117) `MoonshineTensorView::MoonshineTensorView()
    : _tensor(nullptr), name("anonymous")`
  - `MoonshineTensorView` (function, line 120) `MoonshineTensorView::MoonshineTensorView(moonshine_tensor_t *tensor,
                            ...`
  - `MoonshineTensorView` (function, line 132) `MoonshineTensorView::MoonshineTensorView(const std::vector<int64_t> &shape,
                     ...`
  - `MoonshineTensorView` (function, line 139) `MoonshineTensorView::MoonshineTensorView(const MoonshineTensorView &other)
    : _shape(other._sh...`
  - `MoonshineTensorView` (function, line 146) `MoonshineTensorView::MoonshineTensorView(const OrtApi *ort_api,
                                 ...`
  - `shape` (function, line 178) `std::vector<int64_t> &MoonshineTensorView::shape()`
  - `element_count` (function, line 180) `size_t MoonshineTensorView::element_count()`
  - `bytes_count` (function, line 185) `size_t MoonshineTensorView::bytes_count()`
  - `dtype` (function, line 191) `uint32_t MoonshineTensorView::dtype()`
  - `reshape` (function, line 193) `void MoonshineTensorView::reshape(const std::vector<int64_t> &shape)`
  - `cast_f16_to_f32` (function, line 202) `MoonshineTensorView MoonshineTensorView::cast_f16_to_f32()`
  - `argmax` (function, line 214) `int64_t MoonshineTensorView::argmax()`
  - `ort_dtype_to_moonshine_dtype` (function, line 230) `moonshine_dtype_t ort_dtype_to_moonshine_dtype(
    ONNXTensorElementDataType ort_dtype)`
  - `moonshine_dtype_to_ort_dtype` (function, line 258) `ONNXTensorElementDataType moonshine_dtype_to_ort_dtype(
    uint32_t moonshine_dtype)`
  - `ort_dtype_to_bytes_per_element` (function, line 283) `size_t ort_dtype_to_bytes_per_element(ONNXTensorElementDataType ort_dtype)`
  - `moonshine_dtype_to_bytes_per_element` (function, line 311) `size_t moonshine_dtype_to_bytes_per_element(uint32_t moonshine_dtype)`
  - `moonshine_tensor_from_token_vector` (function, line 317) `MoonshineTensorView *moonshine_tensor_from_token_vector(
    std::vector<int32_t> &vector)`
  - `token_vector_from_moonshine_tensor` (function, line 325) `std::vector<int32_t> token_vector_from_moonshine_tensor(
    MoonshineTensorView *moonshine_tensor)`
  - `create_ort_value` (function, line 332) `OrtValue *MoonshineTensorView::create_ort_value(const OrtApi *ort_api,
                          ...`
  - `float16_to_float32` (function, line 345) `void float16_to_float32(const uint16_t *f16_array, float *f32_array,
                        size...`
  - `to_string` (function, line 387) `std::string MoonshineTensorView::to_string()`
- Depends on: `core/moonshine-utils/debug-utils.h`, `core/ort-utils/moonshine-tensor-view.h`, `core/ort-utils/ort-utils.h`

## core/ort-utils/moonshine-tensor-view.h
- Layer: presentation
- Language: h
- Symbols:
  - `MoonshineTensorView` (struct, line 32)
  - `MoonshineTensorView` (struct, line 55)
  - `data` (function, line 78) `template <typename T>
  T *data()`
  - `moonshine_dtype_to_bytes_per_element` (function, line 34) `size_t moonshine_dtype_to_bytes_per_element(uint32_t moonshine_dtype);`
  - `ort_dtype_to_moonshine_dtype` (function, line 36) `moonshine_dtype_t ort_dtype_to_moonshine_dtype( ONNXTensorElementDataType ort_dtype);`
  - `ort_dtype_to_bytes_per_element` (function, line 42) `size_t ort_dtype_to_bytes_per_element(ONNXTensorElementDataType ort_dtype);`
  - `moonshine_tensor_from_token_vector` (function, line 44) `MoonshineTensorView *moonshine_tensor_from_token_vector( std::vector<int32_t> &vector);`
  - `token_vector_from_moonshine_tensor` (function, line 47) `std::vector<int32_t> token_vector_from_moonshine_tensor( MoonshineTensorView *moonshine_tensor);`
  - `float16_to_float32` (function, line 50) `void float16_to_float32(const uint16_t *f16_array, float *f32_array, size_t count);`
  - `log_leaked_tensor_views` (function, line 53) `void log_leaked_tensor_views();`
  - `shape` (function, line 82) `std::vector<int64_t> &shape();`
  - `element_count` (function, line 84) `size_t element_count();`
  - `bytes_count` (function, line 86) `size_t bytes_count();`
  - `dtype` (function, line 88) `uint32_t dtype();`
  - `reshape` (function, line 90) `void reshape(const std::vector<int64_t> &shape);`
  - `argmax` (function, line 94) `int64_t argmax();`
  - `create_ort_value` (function, line 98) `OrtValue *create_ort_value(const OrtApi *ort_api, OrtMemoryInfo *memory_info);`
  - `MOONSHINE_TENSOR_VIEW_H` (macro, line 2) `#define MOONSHINE_TENSOR_VIEW_H`
  - `CHECK_SHAPE_RANK` (macro, line 14) `#define CHECK_SHAPE_RANK(tensor, rank)`
  - `CHECK_DTYPE` (macro, line 21) `#define CHECK_DTYPE(tensor, expected_dtype)`
  - `TENSOR_NAME` (macro, line 28) `#define TENSOR_NAME(name)`
- Depends on: `core/ort-utils/moonshine-tensor.h`
- Imported by: `core/moonshine-c-api.cpp`, `core/moonshine-model.cpp`, `core/ort-utils/moonshine-tensor-view.cpp`, `core/reliability/fuzz-tensor-view.cpp`, `core/spelling-model.cpp`

## core/ort-utils/moonshine-tensor.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `return` (variable, line 6) `extern "C" void moonshine_free_tensor(moonshine_tensor_t *tensor) { if (tensor == NULL) { return;`
  - `return` (variable, line 15) `extern "C" void moonshine_free_tensor_list( moonshine_tensor_list_t *tensor_list) { if (tensor_list == nullptr) { return;`
- Depends on: `core/moonshine-utils/debug-utils.h`, `core/ort-utils/moonshine-tensor.h`, `core/ort-utils/ort-utils.h`

## core/ort-utils/moonshine-tensor.h
- Layer: utility
- Language: h
- Symbols:
  - `moonshine_tensor_t` (struct, line 27)
  - `moonshine_tensor_list_t` (struct, line 34)
  - `moonshine_dtype_t` (enum, line 11)
  - `moonshine_free_tensor` (function, line 39) `void moonshine_free_tensor(moonshine_tensor_t *tensor);`
  - `moonshine_free_tensor_list` (function, line 41) `void moonshine_free_tensor_list(moonshine_tensor_list_t *tensor_list);`
  - `moonshine_dtype_t` (variable, line 8) `extern "C" { #endif typedef enum moonshine_dtype_t { MOONSHINE_DTYPE_FLOAT16 = 0, MOONSHINE_DTYPE_FLOAT32 = 1, MOONSHINE_DTYPE_FLOAT64 = 2, MOONSHINE_DTYPE_INT8 = 3, MOONSHINE_DTYPE_INT16 = 4, MOONSHI`
  - `MOONSHINE_TENSOR_H` (macro, line 2) `#define MOONSHINE_TENSOR_H`
- Imported by: `core/ort-utils/moonshine-tensor-view.h`, `core/ort-utils/moonshine-tensor.cpp`

## core/ort-utils/ort-utils-cxx.h
- Layer: utility
- Language: h
- Symbols:
  - `ORT_UTILS_CXX_H` (macro, line 2) `#define ORT_UTILS_CXX_H`
- Depends on: `core/ort-utils/ort-utils.h`
- Imported by: `core/moonshine-tts/src/ort-session-options.cpp`

## core/ort-utils/ort-utils-ep-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 10) `TEST_CASE("ort_parse_provider_names")`
  - `SUBCASE` (function, line 11) `SUBCASE("empty string")`
  - `SUBCASE` (function, line 16) `SUBCASE("comma-separated aliases")`
  - `SUBCASE` (function, line 23) `SUBCASE("execution provider suffix aliases")`
  - `SUBCASE` (function, line 31) `SUBCASE("empty token is rejected")`
  - `TEST_CASE` (function, line 37) `TEST_CASE("ort_append_execution_providers")`
  - `SUBCASE` (function, line 48) `SUBCASE("unknown provider returns error status")`
  - `SUBCASE` (function, line 57) `SUBCASE("cpu provider appends successfully")`
  - `SUBCASE` (function, line 64) `SUBCASE("coreml provider appends successfully")`
  - `SUBCASE` (function, line 72) `SUBCASE("nnapi provider appends successfully")`
  - `TEST_CASE` (function, line 83) `TEST_CASE("ort session with execution providers")`
  - `SUBCASE` (function, line 99) `SUBCASE("cpu-only session creation")`
  - `SUBCASE` (function, line 118) `SUBCASE("coreml session creation")`
  - `SUBCASE` (function, line 138) `SUBCASE("nnapi session creation")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 3) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/ort-utils/ort-utils.h`

## core/ort-utils/ort-utils-ep.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `trim_copy` (function, line 17) `std::string trim_copy(const std::string &s)`
  - `lowercase_copy` (function, line 29) `std::string lowercase_copy(std::string s)`
  - `normalize_provider_name` (function, line 36) `std::string normalize_provider_name(const std::string &name)`
  - `make_invalid_argument_status` (function, line 51) `OrtStatus *make_invalid_argument_status(const OrtApi *ort_api,
                                  ...`
  - `append_one_provider` (function, line 56) `OrtStatus *append_one_provider(
    const OrtApi *ort_api, OrtSessionOptions *session_options,
  ...`
  - `ort_parse_provider_names` (function, line 102) `std::vector<std::string> ort_parse_provider_names(const std::string &csv)`
  - `ort_append_execution_providers` (function, line 126) `OrtStatus *ort_append_execution_providers(
    const OrtApi *ort_api, OrtSessionOptions *session_...`
- Depends on: `core/ort-utils/ort-utils.h`

## core/ort-utils/ort-utils-test.cpp
- Layer: testing
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 7) `TEST_CASE("ort-utils")`
  - `SUBCASE` (function, line 8) `SUBCASE("ort_session_from_path")`
  - `SUBCASE` (function, line 12) `SUBCASE("ort_session_from_memory")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 3) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/ort-utils/ort-utils.h`

## core/ort-utils/ort-utils.cpp
- Layer: utility
- Doc: No memory mapping on Windows and wchar for the file path.
- Language: cpp
- Symbols:
  - `ort_session_from_path` (function, line 18) `int ort_session_from_path(const OrtApi *ort_api, OrtEnv *env,
                          OrtSessio...`
  - `ort_session_from_path` (function, line 37) `int ort_session_from_path(const OrtApi *ort_api, OrtEnv *env,
                          OrtSessio...`
  - `ort_session_from_memory` (function, line 82) `int ort_session_from_memory(const OrtApi *ort_api, OrtEnv *env,
                            OrtSe...`
  - `ort_maybe_force_single_thread` (function, line 94) `void ort_maybe_force_single_thread(const OrtApi *ort_api,
                                   OrtS...`
  - `ort_session_from_asset` (function, line 107) `int ort_session_from_asset(const OrtApi *ort_api, OrtEnv *env,
                           OrtSess...`
  - `ort_get_shape` (function, line 152) `std::vector<int64_t> ort_get_shape(const OrtApi *ort_api,
                                   OrtT...`
  - `ort_get_type` (function, line 169) `ONNXTensorElementDataType ort_get_type(const OrtApi *ort_api,
                                   ...`
  - `ort_get_input_shape` (function, line 179) `std::vector<int64_t> ort_get_input_shape(const OrtApi *ort_api,
                                 ...`
  - `ort_get_input_type` (function, line 189) `ONNXTensorElementDataType ort_get_input_type(const OrtApi *ort_api,
                             ...`
  - `ort_get_output_shape` (function, line 199) `std::vector<int64_t> ort_get_output_shape(const OrtApi *ort_api,
                                ...`
  - `ort_get_output_type` (function, line 209) `ONNXTensorElementDataType ort_get_output_type(const OrtApi *ort_api,
                            ...`
  - `ort_get_value_shape` (function, line 219) `std::vector<int64_t> ort_get_value_shape(const OrtApi *ort_api,
                                 ...`
  - `ort_get_value_type` (function, line 228) `ONNXTensorElementDataType ort_get_value_type(const OrtApi *ort_api,
                             ...`
  - `ort_run` (function, line 237) `OrtStatus *ort_run(const OrtApi *ort_api, OrtSession *session,
                   const char *con...`
  - `shape` (function, line 163) `std::vector<int64_t> shape(num_dims);`
- Depends on: `core/ort-utils/ort-utils.h`

## core/ort-utils/ort-utils.h
- Layer: utility
- Language: h
- Symbols:
  - `OrtExecutionProviderOptions` (struct, line 15)
  - `ort_configure_execution_providers` (function, line 114) `inline void ort_configure_execution_providers(
    const OrtApi *ort_api, OrtSessionOptions *sess...`
  - `ort_session_from_path` (function, line 40) `int ort_session_from_path(const OrtApi *ort_api, OrtEnv *env, OrtSessionOptions *session_options, const char *path, OrtSession **session, const char **mmapped_data, size_t *mmapped_data_size);`
  - `ort_session_from_memory` (function, line 45) `int ort_session_from_memory(const OrtApi *ort_api, OrtEnv *env, OrtSessionOptions *session_options, const uint8_t *data, size_t data_size, OrtSession **session);`
  - `ort_session_from_asset` (function, line 51) `int ort_session_from_asset(const OrtApi *ort_api, OrtEnv *env, OrtSessionOptions *session_options, AAssetManager *assetManager, const char *path, OrtSession **session, const char **mmapped_data, size_`
  - `ort_get_shape` (function, line 58) `std::vector<int64_t> ort_get_shape(const OrtApi *ort_api, OrtTypeInfo *type_info);`
  - `ort_get_input_shape` (function, line 64) `std::vector<int64_t> ort_get_input_shape(const OrtApi *ort_api, OrtSession *session, int index);`
  - `ort_get_output_shape` (function, line 70) `std::vector<int64_t> ort_get_output_shape(const OrtApi *ort_api, OrtSession *session, int index);`
  - `ort_get_value_shape` (function, line 76) `std::vector<int64_t> ort_get_value_shape(const OrtApi *ort_api, const OrtValue *value);`
  - `ort_maybe_force_single_thread` (function, line 104) `void ort_maybe_force_single_thread(const OrtApi *ort_api, OrtSessionOptions *session_options);`
  - `ort_append_execution_providers` (function, line 109) `OrtStatus *ort_append_execution_providers( const OrtApi *ort_api, OrtSessionOptions *session_options, const std::vector<std::string> &provider_names, const OrtExecutionProviderOptions *config);`
  - `ORT_UTILS_H` (macro, line 2) `#define ORT_UTILS_H`
  - `RETURN_ON_ORT_ERROR` (macro, line 19) `#define RETURN_ON_ORT_ERROR(ort_api, expr)`
  - `LOG_ORT_ERROR` (macro, line 30) `#define LOG_ORT_ERROR(ort_api, expr)`
  - `ORT_RUN` (macro, line 82) `#define ORT_RUN(ort_api, session, input_names, inputs, input_count,         \
                output_names, output_count, outputs)`
- Depends on: `core/moonshine-utils/debug-utils.h`
- Imported by: `core/gemma-embedding-model.cpp`, `core/moonshine-c-api.cpp`, `core/moonshine-model.cpp`, `core/moonshine-streaming-model.cpp`, `core/moonshine-tts/src/moonshine-g2p-options.cpp`, `core/moonshine-tts/src/moonshine-tts-options.cpp`, `core/moonshine-tts/src/ort-session-options.h`, `core/ort-utils/moonshine-tensor-view.cpp`, `core/ort-utils/moonshine-tensor.cpp`, `core/ort-utils/ort-utils-cxx.h`, `core/ort-utils/ort-utils-ep-test.cpp`, `core/ort-utils/ort-utils-ep.cpp`, `core/ort-utils/ort-utils-test.cpp`, `core/ort-utils/ort-utils.cpp`, `core/silero-vad.cpp`, `core/spelling-model.cpp`
