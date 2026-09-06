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
  - `DEBUG_ALLOC_ENABLED` (macro, line 2)

## core/ort-utils/moonshine-ort-allocator.h
- Layer: utility
- Doc: ifndef MOONSHINE_ORT_ALLOCATOR_H define MOONSHINE_ORT_ALLOCATOR_H  include <map>  include "onnxruntime_c_api.h"
- Language: h
- Symbols:
  - `MoonshineOrtAllocator` (struct, line 8)
  - `MOONSHINE_ORT_ALLOCATOR_H` (macro, line 2)

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

## core/ort-utils/moonshine-tensor-view.h
- Layer: presentation
- Doc: ifndef MOONSHINE_TENSOR_VIEW_H define MOONSHINE_TENSOR_VIEW_H  include <stdint.h>  include <cassert> include <numeric> i
- Language: h
- Symbols:
  - `MoonshineTensorView` (struct, line 32)
  - `MoonshineTensorView` (struct, line 55)
  - `data` (function, line 77) `template <typename T>
  T *data()`
  - `MOONSHINE_TENSOR_VIEW_H` (macro, line 2)
  - `CHECK_SHAPE_RANK` (macro, line 13)
  - `CHECK_DTYPE` (macro, line 20)
  - `TENSOR_NAME` (macro, line 27)

## core/ort-utils/moonshine-tensor.cpp
- Layer: utility
- Doc: include "moonshine-tensor.h"  include "debug-utils.h" include "ort-utils.h"
- Language: cpp

## core/ort-utils/moonshine-tensor.h
- Layer: utility
- Doc: ifndef MOONSHINE_TENSOR_H define MOONSHINE_TENSOR_H  include <stddef.h> include <stdint.h>  ifdef __cplusplus
- Language: h
- Symbols:
  - `MOONSHINE_TENSOR_H` (macro, line 2)

## core/ort-utils/ort-utils-cxx.h
- Layer: utility
- Doc: ifndef ORT_UTILS_CXX_H define ORT_UTILS_CXX_H  include "onnxruntime_cxx_api.h" include "ort-utils.h"
- Language: h
- Symbols:
  - `ORT_UTILS_CXX_H` (macro, line 2)

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
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 2)

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

## core/ort-utils/ort-utils-test.cpp
- Layer: testing
- Doc: include "ort-utils.h"  define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN  include <doctest.h>
- Language: cpp
- Symbols:
  - `TEST_CASE` (function, line 6) `TEST_CASE("ort-utils")`
  - `SUBCASE` (function, line 8) `SUBCASE("ort_session_from_path")`
  - `SUBCASE` (function, line 12) `SUBCASE("ort_session_from_memory")`
  - `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` (macro, line 2)

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

## core/ort-utils/ort-utils.h
- Layer: utility
- Doc: ifndef ORT_UTILS_H define ORT_UTILS_H  include <filesystem> include <string> include <vector>  if defined(ANDROID) inclu
- Language: h
- Symbols:
  - `OrtExecutionProviderOptions` (struct, line 15)
  - `ort_configure_execution_providers` (function, line 113) `inline void ort_configure_execution_providers(
    const OrtApi *ort_api, OrtSessionOptions *sess...`
  - `ORT_UTILS_H` (macro, line 2)
  - `RETURN_ON_ORT_ERROR` (macro, line 18)
  - `LOG_ORT_ERROR` (macro, line 29)
  - `ORT_RUN` (macro, line 81)
