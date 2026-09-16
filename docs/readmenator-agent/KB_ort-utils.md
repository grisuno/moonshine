# Subsystem: ort-utils

## core/ort-utils/moonshine-ort-allocator.cpp
- Layer: utility
- Doc: include "moonshine-ort-allocator.h"  define DEBUG_ALLOC_ENABLED 1 include "debug-utils.h"
- Language: cpp
- Symbols:
  - `MoonshineAlloc` (function, line 7) `void *MoonshineAlloc(struct OrtAllocator *this_, size_t size)`
  - `MoonshineFree` (function, line 14) `void MoonshineFree(struct OrtAllocator *this_, void *p)`
  - `MoonshineInfo` (function, line 21) `const struct OrtMemoryInfo *MoonshineInfo(const struct OrtAllocator *this_)`
  - `MoonshineReserve` (function, line 28) `void *MoonshineReserve(struct OrtAllocator *this_, size_t size)`
  - `MoonshineAllocOnStream` (function, line 34) `void *MoonshineAllocOnStream(struct OrtAllocator *this_, size_t size,
                           ...`
  - `friendlySizeString` (function, line 49) `void friendlySizeString(size_t byte_count, char *output, size_t output_size)`
  - `printFriendlySize` (function, line 64) `void printFriendlySize(const char *prefix, size_t number)`
  - `MoonshineOrtAllocator` (function, line 71) `MoonshineOrtAllocator::MoonshineOrtAllocator(const OrtMemoryInfo *memory_info)`
  - `print_stats` (function, line 92) `void MoonshineOrtAllocator::print_stats()`
  - `DEBUG_FREE` (function, line 18) `DEBUG_FREE(p);`
  - `fprintf` (function, line 24) `fprintf(stderr, "MoonshineInfo: %p\n", (void *)(moonshine_allocator->memory_info));`
  - `DEBUG_CALLOC` (function, line 32) `return DEBUG_CALLOC(size, 1);`
  - `snprintf` (function, line 52) `snprintf(output, output_size, "%zu bytes", byte_count);`
  - `DEBUG_ALLOC_ENABLED` (macro, line 2) `#define DEBUG_ALLOC_ENABLED`
- Depends on: `core/moonshine-utils/debug-utils.h`, `core/ort-utils/moonshine-ort-allocator.h`

## core/ort-utils/moonshine-ort-allocator.h
- Layer: utility
- Doc: ifndef MOONSHINE_ORT_ALLOCATOR_H define MOONSHINE_ORT_ALLOCATOR_H  include <map>  include "onnxruntime_c_api.h"
- Language: h
- Symbols:
  - `MoonshineOrtAllocator` (struct, line 8)
  - `MoonshineOrtAllocator` (function, line 19) `MoonshineOrtAllocator(const OrtMemoryInfo *memory_info);`
  - `print_stats` (function, line 23) `void print_stats();`
  - `MOONSHINE_ORT_ALLOCATOR_H` (macro, line 2) `#define MOONSHINE_ORT_ALLOCATOR_H`
- Imported by: `core/gemma-embedding-model.h`, `core/moonshine-c-api.cpp`, `core/moonshine-model.cpp`, `core/moonshine-model.h`, `core/moonshine-streaming-model.cpp`, `core/moonshine-streaming-model.h`, `core/ort-utils/moonshine-ort-allocator.cpp`

## core/ort-utils/moonshine-tensor-view.cpp
- Layer: presentation
- Doc: include "moonshine-tensor-view.h"  include <cstdint> include <cstdlib> include <cstring> include <list>  include "debug-
- Language: cpp
- Symbols:
  - `checked_mul` (function, line 18) `bool checked_mul(size_t a, size_t b, size_t *out)`
  - `moonshine_tensor_from_shape_and_dtype` (function, line 25) `moonshine_tensor_t *moonshine_tensor_from_shape_and_dtype(
    const std::vector<int64_t> &shape,...`
  - `moonshine_tensor_from_ort_tensor` (function, line 99) `moonshine_tensor_t *moonshine_tensor_from_ort_tensor(const OrtApi *ort_api,
                     ...`
  - `MoonshineTensorView` (function, line 116) `MoonshineTensorView::MoonshineTensorView()
    : _tensor(nullptr), name("anonymous")`
  - `MoonshineTensorView` (function, line 119) `MoonshineTensorView::MoonshineTensorView(moonshine_tensor_t *tensor,
                            ...`
  - `MoonshineTensorView` (function, line 131) `MoonshineTensorView::MoonshineTensorView(const std::vector<int64_t> &shape,
                     ...`
  - `MoonshineTensorView` (function, line 138) `MoonshineTensorView::MoonshineTensorView(const MoonshineTensorView &other)
    : _shape(other._sh...`
  - `MoonshineTensorView` (function, line 145) `MoonshineTensorView::MoonshineTensorView(const OrtApi *ort_api,
                                 ...`
  - `shape` (function, line 177) `std::vector<int64_t> &MoonshineTensorView::shape()`
  - `element_count` (function, line 179) `size_t MoonshineTensorView::element_count()`
  - `bytes_count` (function, line 184) `size_t MoonshineTensorView::bytes_count()`
  - `dtype` (function, line 190) `uint32_t MoonshineTensorView::dtype()`
  - `reshape` (function, line 192) `void MoonshineTensorView::reshape(const std::vector<int64_t> &shape)`
  - `cast_f16_to_f32` (function, line 201) `MoonshineTensorView MoonshineTensorView::cast_f16_to_f32()`
  - `argmax` (function, line 213) `int64_t MoonshineTensorView::argmax()`
  - `ort_dtype_to_moonshine_dtype` (function, line 229) `moonshine_dtype_t ort_dtype_to_moonshine_dtype(
    ONNXTensorElementDataType ort_dtype)`
  - `moonshine_dtype_to_ort_dtype` (function, line 257) `ONNXTensorElementDataType moonshine_dtype_to_ort_dtype(
    uint32_t moonshine_dtype)`
  - `ort_dtype_to_bytes_per_element` (function, line 282) `size_t ort_dtype_to_bytes_per_element(ONNXTensorElementDataType ort_dtype)`
  - `moonshine_dtype_to_bytes_per_element` (function, line 310) `size_t moonshine_dtype_to_bytes_per_element(uint32_t moonshine_dtype)`
  - `moonshine_tensor_from_token_vector` (function, line 316) `MoonshineTensorView *moonshine_tensor_from_token_vector(
    std::vector<int32_t> &vector)`
  - `token_vector_from_moonshine_tensor` (function, line 324) `std::vector<int32_t> token_vector_from_moonshine_tensor(
    MoonshineTensorView *moonshine_tensor)`
  - `create_ort_value` (function, line 331) `OrtValue *MoonshineTensorView::create_ort_value(const OrtApi *ort_api,
                          ...`
  - `float16_to_float32` (function, line 345) `void float16_to_float32(const uint16_t *f16_array, float *f32_array,
                        size...`
  - `to_string` (function, line 386) `std::string MoonshineTensorView::to_string()`
  - `fprintf` (function, line 30) `fprintf(stderr, "Shape is empty\n");`
  - `DEBUG_CALLOC` (function, line 34) `DEBUG_CALLOC(1, sizeof(moonshine_tensor_t)));`
  - `memcpy` (function, line 38) `std::memcpy(moonshine_tensor->shape, shape.data(), shape.size() * sizeof(int64_t));`
  - `DEBUG_FREE` (function, line 52) `DEBUG_FREE(moonshine_tensor->shape);`
  - `LOG_ORT_ERROR` (function, line 110) `LOG_ORT_ERROR(ort_api, ort_api->GetTensorMutableData(ort_tensor, &ort_data));`
  - `assert` (function, line 126) `assert(false);`
  - `runtime_error` (function, line 152) `throw std::runtime_error("Failed to create moonshine tensor '" + name + "' from ort tensor");`
  - `moonshine_free_tensor` (function, line 169) `moonshine_free_tensor(_tensor);`
  - `accumulate` (function, line 181) `return std::accumulate(shape().begin(), shape().end(), 1, std::multiplies<int64_t>());`
  - `f32` (function, line 206) `MoonshineTensorView f32(_shape, MOONSHINE_DTYPE_FLOAT32);`
- Depends on: `core/moonshine-utils/debug-utils.h`, `core/ort-utils/moonshine-tensor-view.h`, `core/ort-utils/ort-utils.h`

## core/ort-utils/moonshine-tensor-view.h
- Layer: presentation
- Doc: ifndef MOONSHINE_TENSOR_VIEW_H define MOONSHINE_TENSOR_VIEW_H  include <stdint.h>  include <cassert> include <numeric> i
- Language: h
- Symbols:
  - `MoonshineTensorView` (struct, line 32)
  - `MoonshineTensorView` (struct, line 55)
  - `data` (function, line 77) `template <typename T>
  T *data()`
  - `fprintf` (function, line 16) `fprintf(stderr, #tensor " shape rank is not %d at %s:%d\n", rank, \ __FILE__, __LINE__);`
  - `moonshine_dtype_to_bytes_per_element` (function, line 33) `size_t moonshine_dtype_to_bytes_per_element(uint32_t moonshine_dtype);`
  - `ort_dtype_to_moonshine_dtype` (function, line 35) `moonshine_dtype_t ort_dtype_to_moonshine_dtype( ONNXTensorElementDataType ort_dtype);`
  - `moonshine_dtype_to_ort_dtype` (function, line 38) `ONNXTensorElementDataType moonshine_dtype_to_ort_dtype( uint32_t moonshine_dtype);`
  - `ort_dtype_to_bytes_per_element` (function, line 41) `size_t ort_dtype_to_bytes_per_element(ONNXTensorElementDataType ort_dtype);`
  - `moonshine_tensor_from_token_vector` (function, line 43) `MoonshineTensorView *moonshine_tensor_from_token_vector( std::vector<int32_t> &vector);`
  - `token_vector_from_moonshine_tensor` (function, line 46) `std::vector<int32_t> token_vector_from_moonshine_tensor( MoonshineTensorView *moonshine_tensor);`
  - `float16_to_float32` (function, line 49) `void float16_to_float32(const uint16_t *f16_array, float *f32_array, size_t count);`
  - `log_leaked_tensor_views` (function, line 52) `void log_leaked_tensor_views();`
  - `MoonshineTensorView` (function, line 59) `MoonshineTensorView();`
  - `shape` (function, line 81) `std::vector<int64_t> &shape();`
  - `element_count` (function, line 83) `size_t element_count();`
  - `bytes_count` (function, line 85) `size_t bytes_count();`
  - `dtype` (function, line 87) `uint32_t dtype();`
  - `reshape` (function, line 89) `void reshape(const std::vector<int64_t> &shape);`
  - `cast_f16_to_f32` (function, line 91) `MoonshineTensorView cast_f16_to_f32();`
  - `argmax` (function, line 93) `int64_t argmax();`
  - `create_ort_value` (function, line 98) `OrtValue *create_ort_value(const OrtApi *ort_api, OrtMemoryInfo *memory_info);`
  - `to_string` (function, line 99) `std::string to_string();`
  - `MOONSHINE_TENSOR_VIEW_H` (macro, line 2) `#define MOONSHINE_TENSOR_VIEW_H`
  - `CHECK_SHAPE_RANK` (macro, line 13) `#define CHECK_SHAPE_RANK(tensor, rank)`
  - `CHECK_DTYPE` (macro, line 20) `#define CHECK_DTYPE(tensor, expected_dtype)`
  - `TENSOR_NAME` (macro, line 27) `#define TENSOR_NAME(name)`
- Depends on: `core/ort-utils/moonshine-tensor.h`
- Imported by: `core/moonshine-c-api.cpp`, `core/moonshine-model.cpp`, `core/ort-utils/moonshine-tensor-view.cpp`, `core/reliability/fuzz-tensor-view.cpp`, `core/spelling-model.cpp`

## core/ort-utils/moonshine-tensor.cpp
- Layer: utility
- Doc: include "moonshine-tensor.h"  include "debug-utils.h" include "ort-utils.h"
- Language: cpp
- Symbols:
  - `DEBUG_FREE` (function, line 10) `DEBUG_FREE(tensor->shape);`
  - `return` (variable, line 5) `extern "C" void moonshine_free_tensor(moonshine_tensor_t *tensor) { if (tensor == NULL) { return;`
  - `return` (variable, line 14) `extern "C" void moonshine_free_tensor_list( moonshine_tensor_list_t *tensor_list) { if (tensor_list == nullptr) { return;`
- Depends on: `core/moonshine-utils/debug-utils.h`, `core/ort-utils/moonshine-tensor.h`, `core/ort-utils/ort-utils.h`

## core/ort-utils/moonshine-tensor.h
- Layer: utility
- Doc: ifndef MOONSHINE_TENSOR_H define MOONSHINE_TENSOR_H  include <stddef.h> include <stdint.h>  ifdef __cplusplus
- Language: h
- Symbols:
  - `moonshine_tensor_t` (struct, line 27)
  - `moonshine_tensor_list_t` (struct, line 34)
  - `moonshine_dtype_t` (enum, line 11)
  - `moonshine_free_tensor` (function, line 38) `void moonshine_free_tensor(moonshine_tensor_t *tensor);`
  - `moonshine_free_tensor_list` (function, line 40) `void moonshine_free_tensor_list(moonshine_tensor_list_t *tensor_list);`
  - `moonshine_dtype_t` (variable, line 8) `extern "C" { #endif typedef enum moonshine_dtype_t { MOONSHINE_DTYPE_FLOAT16 = 0, MOONSHINE_DTYPE_FLOAT32 = 1, MOONSHINE_DTYPE_FLOAT64 = 2, MOONSHINE_DTYPE_INT8 = 3, MOONSHINE_DTYPE_INT16 = 4, MOONSHI`
  - `MOONSHINE_TENSOR_H` (macro, line 2) `#define MOONSHINE_TENSOR_H`
- Imported by: `core/ort-utils/moonshine-tensor-view.h`, `core/ort-utils/moonshine-tensor.cpp`

## core/ort-utils/ort-utils-cxx.h
- Layer: utility
- Doc: ifndef ORT_UTILS_CXX_H define ORT_UTILS_CXX_H  include "onnxruntime_cxx_api.h" include "ort-utils.h"
- Language: h
- Symbols:
  - `ThrowOnError` (function, line 12) `Ort::ThrowOnError(status);`
  - `ORT_UTILS_CXX_H` (macro, line 2) `#define ORT_UTILS_CXX_H`
- Depends on: `core/ort-utils/ort-utils.h`
- Imported by: `core/moonshine-tts/src/ort-session-options.cpp`

## core/ort-utils/ort-utils-ep-test.cpp
- Layer: testing
- Doc: include "ort-utils.h"  define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN  include <doctest.h>  include <filesystem> include <str
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 9) `TEST_CASE("ort_parse_provider_names")`
  - `SUBCASE` (function, line 11) `SUBCASE("empty string")`
  - `SUBCASE` (function, line 15) `SUBCASE("comma-separated aliases")`
  - `SUBCASE` (function, line 22) `SUBCASE("execution provider suffix aliases")`
  - `SUBCASE` (function, line 30) `SUBCASE("empty token is rejected")`
  - `TEST_CASE` (function, line 36) `TEST_CASE("ort_append_execution_providers")`
  - `SUBCASE` (function, line 47) `SUBCASE("unknown provider returns error status")`
  - `SUBCASE` (function, line 56) `SUBCASE("cpu provider appends successfully")`
  - `SUBCASE` (function, line 64) `SUBCASE("coreml provider appends successfully")`
  - `SUBCASE` (function, line 72) `SUBCASE("nnapi provider appends successfully")`
  - `TEST_CASE` (function, line 82) `TEST_CASE("ort session with execution providers")`
  - `SUBCASE` (function, line 98) `SUBCASE("cpu-only session creation")`
  - `SUBCASE` (function, line 118) `SUBCASE("coreml session creation")`
  - `SUBCASE` (function, line 138) `SUBCASE("nnapi session creation")`
  - `CHECK` (function, line 12) `CHECK(ort_parse_provider_names("").empty());`
  - `REQUIRE` (function, line 18) `REQUIRE(names.size() == 2);`
  - `CHECK_THROWS_AS` (function, line 32) `CHECK_THROWS_AS(ort_parse_provider_names("CoreML,,CPU"), std::invalid_argument);`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 2) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/ort-utils/ort-utils.h`

## core/ort-utils/ort-utils-ep.cpp
- Layer: utility
- Doc: include "cpu_provider_factory.h" include "ort-utils.h"  if defined(__ANDROID__) include "nnapi_provider_factory.h" endif
- Language: cpp
- Symbols:
  - `trim_copy` (function, line 16) `std::string trim_copy(const std::string &s)`
  - `lowercase_copy` (function, line 28) `std::string lowercase_copy(std::string s)`
  - `normalize_provider_name` (function, line 35) `std::string normalize_provider_name(const std::string &name)`
  - `make_invalid_argument_status` (function, line 50) `OrtStatus *make_invalid_argument_status(const OrtApi *ort_api,
                                  ...`
  - `append_one_provider` (function, line 55) `OrtStatus *append_one_provider(
    const OrtApi *ort_api, OrtSessionOptions *session_options,
  ...`
  - `ort_parse_provider_names` (function, line 101) `std::vector<std::string> ort_parse_provider_names(const std::string &csv)`
  - `ort_append_execution_providers` (function, line 125) `OrtStatus *ort_append_execution_providers(
    const OrtApi *ort_api, OrtSessionOptions *session_...`
  - `OrtSessionOptionsAppendExecutionProvider_CPU` (function, line 61) `return OrtSessionOptionsAppendExecutionProvider_CPU(session_options, 0);`
  - `OrtSessionOptionsAppendExecutionProvider_Nnapi` (function, line 88) `return OrtSessionOptionsAppendExecutionProvider_Nnapi(session_options, 0);`
  - `invalid_argument` (function, line 114) `throw std::invalid_argument( "ort_providers contains an empty provider name");`
- Depends on: `core/ort-utils/ort-utils.h`

## core/ort-utils/ort-utils-test.cpp
- Layer: testing
- Doc: include "ort-utils.h"  define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN  include <doctest.h>
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 6) `TEST_CASE("ort-utils")`
  - `SUBCASE` (function, line 8) `SUBCASE("ort_session_from_path")`
  - `SUBCASE` (function, line 12) `SUBCASE("ort_session_from_memory")`
  - `REQUIRE` (function, line 9) `REQUIRE(ort_session_from_path(nullptr, nullptr, nullptr, "model.onnx", nullptr, nullptr, nullptr) < 0);`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 2) `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN`
- Depends on: `core/ort-utils/ort-utils.h`

## core/ort-utils/ort-utils.cpp
- Layer: utility
- Doc: include "ort-utils.h"  include <cstdlib> include <cstring> include <filesystem>  ifndef _WIN32 include <fcntl.h> include
- Language: cpp
- Symbols:
  - `ort_session_from_path` (function, line 18) `int ort_session_from_path(const OrtApi *ort_api, OrtEnv *env,
                          OrtSessio...`
  - `ort_session_from_path` (function, line 37) `int ort_session_from_path(const OrtApi *ort_api, OrtEnv *env,
                          OrtSessio...`
  - `ort_session_from_memory` (function, line 81) `int ort_session_from_memory(const OrtApi *ort_api, OrtEnv *env,
                            OrtSe...`
  - `ort_maybe_force_single_thread` (function, line 93) `void ort_maybe_force_single_thread(const OrtApi *ort_api,
                                   OrtS...`
  - `ort_session_from_asset` (function, line 107) `int ort_session_from_asset(const OrtApi *ort_api, OrtEnv *env,
                           OrtSess...`
  - `ort_get_shape` (function, line 151) `std::vector<int64_t> ort_get_shape(const OrtApi *ort_api,
                                   OrtT...`
  - `ort_get_type` (function, line 168) `ONNXTensorElementDataType ort_get_type(const OrtApi *ort_api,
                                   ...`
  - `ort_get_input_shape` (function, line 178) `std::vector<int64_t> ort_get_input_shape(const OrtApi *ort_api,
                                 ...`
  - `ort_get_input_type` (function, line 188) `ONNXTensorElementDataType ort_get_input_type(const OrtApi *ort_api,
                             ...`
  - `ort_get_output_shape` (function, line 198) `std::vector<int64_t> ort_get_output_shape(const OrtApi *ort_api,
                                ...`
  - `ort_get_output_type` (function, line 208) `ONNXTensorElementDataType ort_get_output_type(const OrtApi *ort_api,
                            ...`
  - `ort_get_value_shape` (function, line 218) `std::vector<int64_t> ort_get_value_shape(const OrtApi *ort_api,
                                 ...`
  - `ort_get_value_type` (function, line 227) `ONNXTensorElementDataType ort_get_value_type(const OrtApi *ort_api,
                             ...`
  - `ort_run` (function, line 236) `OrtStatus *ort_run(const OrtApi *ort_api, OrtSession *session,
                   const char *con...`
  - `fprintf` (function, line 23) `fprintf(stderr, "Model directory '%s' does not exist at %s:%d\n", path, __FILE__, __LINE__);`
  - `fs_path` (function, line 27) `std::filesystem::path fs_path(path);`
  - `RETURN_ON_ORT_ERROR` (function, line 29) `RETURN_ON_ORT_ERROR( ort_api, ort_api->CreateSession(env, wpath.c_str(), session_options, session));`
  - `cpp_path` (function, line 41) `std::string cpp_path(path);`
  - `mmap` (function, line 56) `mmap(nullptr, st.st_size, PROT_READ, MAP_PRIVATE, fd, 0));`
  - `close` (function, line 63) `close(fd);`
  - `RETURN_ON_NULL` (function, line 86) `RETURN_ON_NULL(ort_api);`
  - `LOG_ORT_ERROR` (function, line 100) `LOG_ORT_ERROR(ort_api, ort_api->SetIntraOpNumThreads(session_options, 1));`
  - `AAsset_close` (function, line 139) `AAsset_close(asset);`
  - `shape` (function, line 163) `std::vector<int64_t> shape(num_dims);`
  - `now` (function, line 248) `std::chrono::steady_clock::now();`
  - `LOGF` (function, line 255) `LOGF("ORT Run %s took %.2f ms for inputs:", session_name, duration.count());`
- Depends on: `core/ort-utils/ort-utils.h`

## core/ort-utils/ort-utils.h
- Layer: utility
- Doc: ifndef ORT_UTILS_H define ORT_UTILS_H  include <filesystem> include <string> include <vector>  if defined(ANDROID) inclu
- Language: h
- Symbols:
  - `OrtExecutionProviderOptions` (struct, line 15)
  - `ort_configure_execution_providers` (function, line 113) `inline void ort_configure_execution_providers(
    const OrtApi *ort_api, OrtSessionOptions *sess...`
  - `LOGF` (function, line 24) `LOGF("ORT Error: %s", msg);`
  - `ort_session_from_path` (function, line 39) `int ort_session_from_path(const OrtApi *ort_api, OrtEnv *env, OrtSessionOptions *session_options, const char *path, OrtSession **session, const char **mmapped_data, size_t *mmapped_data_size);`
  - `ort_session_from_memory` (function, line 44) `int ort_session_from_memory(const OrtApi *ort_api, OrtEnv *env, OrtSessionOptions *session_options, const uint8_t *data, size_t data_size, OrtSession **session);`
  - `ort_session_from_asset` (function, line 51) `int ort_session_from_asset(const OrtApi *ort_api, OrtEnv *env, OrtSessionOptions *session_options, AAssetManager *assetManager, const char *path, OrtSession **session, const char **mmapped_data, size_`
  - `ort_get_shape` (function, line 57) `std::vector<int64_t> ort_get_shape(const OrtApi *ort_api, OrtTypeInfo *type_info);`
  - `ort_get_type` (function, line 60) `ONNXTensorElementDataType ort_get_type(const OrtApi *ort_api, OrtTypeInfo *type_info);`
  - `ort_get_input_shape` (function, line 63) `std::vector<int64_t> ort_get_input_shape(const OrtApi *ort_api, OrtSession *session, int index);`
  - `ort_get_input_type` (function, line 66) `ONNXTensorElementDataType ort_get_input_type(const OrtApi *ort_api, OrtSession *session, int index);`
  - `ort_get_output_shape` (function, line 69) `std::vector<int64_t> ort_get_output_shape(const OrtApi *ort_api, OrtSession *session, int index);`
  - `ort_get_output_type` (function, line 72) `ONNXTensorElementDataType ort_get_output_type(const OrtApi *ort_api, OrtSession *session, int index);`
  - `ort_get_value_shape` (function, line 75) `std::vector<int64_t> ort_get_value_shape(const OrtApi *ort_api, const OrtValue *value);`
  - `ort_get_value_type` (function, line 78) `ONNXTensorElementDataType ort_get_value_type(const OrtApi *ort_api, const OrtValue *value);`
  - `ort_run` (function, line 84) `ort_run(ort_api, session, input_names, inputs, input_count, output_names, \ output_count, outputs, #session, this->log_ort_run) OrtStatus *ort_run(const OrtApi *ort_api, OrtSession *session, const cha`
  - `ort_maybe_force_single_thread` (function, line 104) `void ort_maybe_force_single_thread(const OrtApi *ort_api, OrtSessionOptions *session_options);`
  - `ort_parse_provider_names` (function, line 106) `std::vector<std::string> ort_parse_provider_names(const std::string &csv);`
  - `ort_append_execution_providers` (function, line 108) `OrtStatus *ort_append_execution_providers( const OrtApi *ort_api, OrtSessionOptions *session_options, const std::vector<std::string> &provider_names, const OrtExecutionProviderOptions *config);`
  - `LOG_ORT_ERROR` (function, line 125) `LOG_ORT_ERROR(ort_api, ort_append_execution_providers(ort_api, session_options, provider_names, &config));`
  - `ORT_UTILS_H` (macro, line 2) `#define ORT_UTILS_H`
  - `RETURN_ON_ORT_ERROR` (macro, line 18) `#define RETURN_ON_ORT_ERROR(ort_api, expr)`
  - `LOG_ORT_ERROR` (macro, line 29) `#define LOG_ORT_ERROR(ort_api, expr)`
  - `ORT_RUN` (macro, line 81) `#define ORT_RUN(ort_api, session, input_names, inputs, input_count,         \
                output_names, output_count, outputs)`
- Depends on: `core/moonshine-utils/debug-utils.h`
- Imported by: `core/gemma-embedding-model.cpp`, `core/moonshine-c-api.cpp`, `core/moonshine-model.cpp`, `core/moonshine-streaming-model.cpp`, `core/moonshine-tts/src/moonshine-g2p-options.cpp`, `core/moonshine-tts/src/moonshine-tts-options.cpp`, `core/moonshine-tts/src/ort-session-options.h`, `core/ort-utils/moonshine-tensor-view.cpp`, `core/ort-utils/moonshine-tensor.cpp`, `core/ort-utils/ort-utils-cxx.h`, `core/ort-utils/ort-utils-ep-test.cpp`, `core/ort-utils/ort-utils-ep.cpp`, `core/ort-utils/ort-utils-test.cpp`, `core/ort-utils/ort-utils.cpp`, `core/silero-vad.cpp`, `core/spelling-model.cpp`
