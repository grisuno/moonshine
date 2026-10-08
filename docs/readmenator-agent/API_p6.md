# API (page 6 of 10)
Previous: [API_p5.md](API_p5.md)

## core/moonshine-utils/debug-utils.h
Imported by: `core/bin-tokenizer/bin-tokenizer-test.cpp`, `core/bin-tokenizer/bin-tokenizer.cpp`, `core/gemma-embedding-model.cpp`, `core/moonshine-c-api-test.cpp`, `core/moonshine-c-api.cpp`, `core/moonshine-download-smoke.cpp`, `core/moonshine-model.cpp`, `core/moonshine-streaming-model.cpp`, `core/moonshine-tts/src/lang-specific/korean.cpp`, `core/moonshine-tts/src/moonshine-g2p.cpp`, `core/moonshine-tts/src/moonshine-tts.cpp`, `core/moonshine-tts/src/piper-tts.cpp`, `core/moonshine-tts/src/zipvoice-tts.cpp`, `core/moonshine-utils/debug-utils-test.cpp`, `core/moonshine-utils/debug-utils.cpp`, `core/moonshine-utils/file-utils.cpp`, `core/moonshine-utils/test-utils.h`, `core/ort-utils/moonshine-ort-allocator.cpp`, `core/ort-utils/moonshine-tensor-view.cpp`, `core/ort-utils/moonshine-tensor.cpp`, `core/ort-utils/ort-utils.h`, `core/reliability/fuzz-wav-pcm.cpp`, `core/resampler-test.cpp`, `core/resampler.cpp`, `core/speaker-diarizer.cpp`, `core/spelling-model-test.cpp`, `core/spelling-model.cpp`, `core/voice-activity-detector-test.cpp`, `core/voice-activity-detector.cpp`, `core/word-alignment-test.cpp`
- `debug_calloc` (function) `core/moonshine-utils/debug-utils.h:139` `debug_calloc(size, count, FILENAME_ONLY, __LINE__, __FUNCTION__)

static inline void *debug_callo...` -- define DEBUG_CALLOC(size, count) \
- `debug_free` (function) `core/moonshine-utils/debug-utils.h:156` `static inline void debug_free(void *voidMemPtr, const char *file, int line,
                     ...`
- `debug_alloc_get_size` (function) `core/moonshine-utils/debug-utils.h:176` `static inline size_t debug_alloc_get_size(void *voidMemPtr)`
- `log_backtrace` (function) `core/moonshine-utils/debug-utils.h:253` `void log_backtrace();`
- `load_wav_data` (function) `core/moonshine-utils/debug-utils.h:255` `bool load_wav_data(const char *path, float **out_float_data, size_t *out_num_samples, int32_t *out_sample_rate =...`
- `save_wav_data` (function) `core/moonshine-utils/debug-utils.h:258` `bool save_wav_data(const char *path, const float *audio_data, size_t num_samples, uint32_t sample_rate = 16000);`
- `load_file_into_memory` (function) `core/moonshine-utils/debug-utils.h:263` `std::vector<uint8_t> load_file_into_memory(const std::string &path);`
- `save_memory_to_file` (function) `core/moonshine-utils/debug-utils.h:264` `void save_memory_to_file(const std::string &path, const std::vector<uint8_t> &data);`
- `gate` (function) `core/moonshine-utils/debug-utils.h:268` `template <typename T>
T gate(T value, T min, T max)`

## core/moonshine-utils/file-utils.cpp
Depends on: `core/moonshine-utils/debug-utils.h`, `core/moonshine-utils/file-utils.h`
- `fread_exact` (function) `core/moonshine-utils/file-utils.cpp:10` `std::size_t fread_exact(void *ptr, std::size_t size, std::size_t count,
                        s...`

## core/moonshine-utils/file-utils.h
Imported by: `core/benchmark.cpp`, `core/bin-tokenizer/bin-tokenizer.cpp`, `core/moonshine-utils/file-utils-test.cpp`, `core/moonshine-utils/file-utils.cpp`, `core/word-alignment-benchmark.cpp`
- `fread_exact` (function) `core/moonshine-utils/file-utils.h:12` `std::size_t fread_exact(void *ptr, std::size_t size, std::size_t count, std::FILE *stream, const char *what = "file");` -- Wrapper around std::fread that throws std::runtime_error unless the full requested number of elements is read.

## core/moonshine-utils/string-utils.cpp
Depends on: `core/moonshine-utils/string-utils.h`
- `replace_all` (function) `core/moonshine-utils/string-utils.cpp:9` `std::string replace_all(std::string str, const std::string &from,
                        const s...` -- See https://stackoverflow.com/questions/2896600/how-to-replace-all-occurrences-of-a-character-in-string
- `trim` (function) `core/moonshine-utils/string-utils.cpp:21` `std::string trim(const std::string &str, const std::string &whitespace)` -- See https://stackoverflow.com/questions/1798112/removing-leading-and-trailing-spaces-from-a-string
- `split` (function) `core/moonshine-utils/string-utils.cpp:31` `std::vector<std::string> split(const std::string &str,
                               const std::...`
- `starts_with` (function) `core/moonshine-utils/string-utils.cpp:44` `bool starts_with(const std::string &str, const std::string &prefix)`
- `ends_with` (function) `core/moonshine-utils/string-utils.cpp:49` `bool ends_with(const std::string &str, const std::string &suffix)`
- `append_path_component` (function) `core/moonshine-utils/string-utils.cpp:63` `std::string append_path_component(const std::string &path,
                                  cons...`
- `to_lowercase` (function) `core/moonshine-utils/string-utils.cpp:86` `std::string to_lowercase(const std::string &str)`
- `bool_from_string` (function) `core/moonshine-utils/string-utils.cpp:92` `bool bool_from_string(const char *input)`
- `bool_from_string` (function) `core/moonshine-utils/string-utils.cpp:99` `bool bool_from_string(const std::string &input)`
- `float_from_string` (function) `core/moonshine-utils/string-utils.cpp:109` `float float_from_string(const char *input)`
- `float_from_string` (function) `core/moonshine-utils/string-utils.cpp:116` `float float_from_string(const std::string &input)`
- `int32_from_string` (function) `core/moonshine-utils/string-utils.cpp:127` `int32_t int32_from_string(const char *input)`
- `int32_from_string` (function) `core/moonshine-utils/string-utils.cpp:134` `int32_t int32_from_string(const std::string &input)`
- `size_t_from_string` (function) `core/moonshine-utils/string-utils.cpp:145` `size_t size_t_from_string(const char *input)`
- `size_t_from_string` (function) `core/moonshine-utils/string-utils.cpp:152` `size_t size_t_from_string(const std::string &input)`

## core/moonshine-utils/string-utils.h
Imported by: `core/bin-tokenizer/bin-tokenizer.cpp`, `core/gemma-embedding-model.cpp`, `core/moonshine-c-api-test.cpp`, `core/moonshine-c-api.cpp`, `core/moonshine-model.cpp`, `core/moonshine-streaming-model.cpp`, `core/moonshine-tts/src/moonshine-g2p-options.cpp`, `core/moonshine-tts/src/moonshine-tts-options.cpp`, `core/moonshine-tts/src/moonshine-tts.cpp`, `core/moonshine-utils/string-utils-test.cpp`, `core/moonshine-utils/string-utils.cpp`, `core/reliability/fuzz-string-utils.cpp`
- `starts_with` (function) `core/moonshine-utils/string-utils.h:17` `bool starts_with(const std::string &str, const std::string &prefix);`
- `ends_with` (function) `core/moonshine-utils/string-utils.h:19` `bool ends_with(const std::string &str, const std::string &suffix);`
- `bool_from_string` (function) `core/moonshine-utils/string-utils.h:29` `bool bool_from_string(const std::string &input);`
- `float_from_string` (function) `core/moonshine-utils/string-utils.h:32` `float float_from_string(const std::string &input);`
- `int32_from_string` (function) `core/moonshine-utils/string-utils.h:35` `int32_t int32_from_string(const std::string &input);`
- `size_t_from_string` (function) `core/moonshine-utils/string-utils.h:38` `size_t size_t_from_string(const std::string &input);`

## core/ort-utils/moonshine-ort-allocator.cpp
Depends on: `core/moonshine-utils/debug-utils.h`, `core/ort-utils/moonshine-ort-allocator.h`
- `MoonshineAlloc` (function) `core/ort-utils/moonshine-ort-allocator.cpp:7` `void *MoonshineAlloc(struct OrtAllocator *this_, size_t size)`
- `MoonshineFree` (function) `core/ort-utils/moonshine-ort-allocator.cpp:15` `void MoonshineFree(struct OrtAllocator *this_, void *p)`
- `MoonshineInfo` (function) `core/ort-utils/moonshine-ort-allocator.cpp:22` `const struct OrtMemoryInfo *MoonshineInfo(const struct OrtAllocator *this_)`
- `MoonshineReserve` (function) `core/ort-utils/moonshine-ort-allocator.cpp:29` `void *MoonshineReserve(struct OrtAllocator *this_, size_t size)`
- `MoonshineAllocOnStream` (function) `core/ort-utils/moonshine-ort-allocator.cpp:35` `void *MoonshineAllocOnStream(struct OrtAllocator *this_, size_t size,
                           ...`
- `friendlySizeString` (function) `core/ort-utils/moonshine-ort-allocator.cpp:50` `void friendlySizeString(size_t byte_count, char *output, size_t output_size)`
- `printFriendlySize` (function) `core/ort-utils/moonshine-ort-allocator.cpp:65` `void printFriendlySize(const char *prefix, size_t number)`
- `MoonshineOrtAllocator` (function) `core/ort-utils/moonshine-ort-allocator.cpp:72` `MoonshineOrtAllocator::MoonshineOrtAllocator(const OrtMemoryInfo *memory_info)`
- `print_stats` (function) `core/ort-utils/moonshine-ort-allocator.cpp:93` `void MoonshineOrtAllocator::print_stats()`

## core/ort-utils/moonshine-ort-allocator.h
Imported by: `core/gemma-embedding-model.h`, `core/moonshine-c-api.cpp`, `core/moonshine-model.cpp`, `core/moonshine-model.h`, `core/moonshine-streaming-model.cpp`, `core/moonshine-streaming-model.h`, `core/ort-utils/moonshine-ort-allocator.cpp`
- `print_stats` (function) `core/ort-utils/moonshine-ort-allocator.h:24` `void print_stats();`

## core/ort-utils/moonshine-tensor-view.cpp
Depends on: `core/moonshine-utils/debug-utils.h`, `core/ort-utils/moonshine-tensor-view.h`, `core/ort-utils/ort-utils.h`
- `checked_mul` (function) `core/ort-utils/moonshine-tensor-view.cpp:18` `bool checked_mul(size_t a, size_t b, size_t *out)` -- Portable checked multiply for size_t: returns false on overflow (leaving *out untouched), otherwise stores a * b.
- `moonshine_tensor_from_shape_and_dtype` (function) `core/ort-utils/moonshine-tensor-view.cpp:26` `moonshine_tensor_t *moonshine_tensor_from_shape_and_dtype(
    const std::vector<int64_t> &shape,...`
- `moonshine_tensor_from_ort_tensor` (function) `core/ort-utils/moonshine-tensor-view.cpp:100` `moonshine_tensor_t *moonshine_tensor_from_ort_tensor(const OrtApi *ort_api,
                     ...`
- `MoonshineTensorView` (function) `core/ort-utils/moonshine-tensor-view.cpp:117` `MoonshineTensorView::MoonshineTensorView()
    : _tensor(nullptr), name("anonymous")`
- `MoonshineTensorView` (function) `core/ort-utils/moonshine-tensor-view.cpp:120` `MoonshineTensorView::MoonshineTensorView(moonshine_tensor_t *tensor,
                            ...`
- `MoonshineTensorView` (function) `core/ort-utils/moonshine-tensor-view.cpp:132` `MoonshineTensorView::MoonshineTensorView(const std::vector<int64_t> &shape,
                     ...`
- `MoonshineTensorView` (function) `core/ort-utils/moonshine-tensor-view.cpp:139` `MoonshineTensorView::MoonshineTensorView(const MoonshineTensorView &other)
    : _shape(other._sh...`
- `MoonshineTensorView` (function) `core/ort-utils/moonshine-tensor-view.cpp:146` `MoonshineTensorView::MoonshineTensorView(const OrtApi *ort_api,
                                 ...`
- `shape` (function) `core/ort-utils/moonshine-tensor-view.cpp:178` `std::vector<int64_t> &MoonshineTensorView::shape()`
- `element_count` (function) `core/ort-utils/moonshine-tensor-view.cpp:180` `size_t MoonshineTensorView::element_count()`
- `bytes_count` (function) `core/ort-utils/moonshine-tensor-view.cpp:185` `size_t MoonshineTensorView::bytes_count()`
- `dtype` (function) `core/ort-utils/moonshine-tensor-view.cpp:191` `uint32_t MoonshineTensorView::dtype()`
- `reshape` (function) `core/ort-utils/moonshine-tensor-view.cpp:193` `void MoonshineTensorView::reshape(const std::vector<int64_t> &shape)`
- `cast_f16_to_f32` (function) `core/ort-utils/moonshine-tensor-view.cpp:202` `MoonshineTensorView MoonshineTensorView::cast_f16_to_f32()`
- `argmax` (function) `core/ort-utils/moonshine-tensor-view.cpp:214` `int64_t MoonshineTensorView::argmax()`
- `ort_dtype_to_moonshine_dtype` (function) `core/ort-utils/moonshine-tensor-view.cpp:230` `moonshine_dtype_t ort_dtype_to_moonshine_dtype(
    ONNXTensorElementDataType ort_dtype)`
- `moonshine_dtype_to_ort_dtype` (function) `core/ort-utils/moonshine-tensor-view.cpp:258` `ONNXTensorElementDataType moonshine_dtype_to_ort_dtype(
    uint32_t moonshine_dtype)`
- `ort_dtype_to_bytes_per_element` (function) `core/ort-utils/moonshine-tensor-view.cpp:283` `size_t ort_dtype_to_bytes_per_element(ONNXTensorElementDataType ort_dtype)`
- `moonshine_dtype_to_bytes_per_element` (function) `core/ort-utils/moonshine-tensor-view.cpp:311` `size_t moonshine_dtype_to_bytes_per_element(uint32_t moonshine_dtype)`
- `moonshine_tensor_from_token_vector` (function) `core/ort-utils/moonshine-tensor-view.cpp:317` `MoonshineTensorView *moonshine_tensor_from_token_vector(
    std::vector<int32_t> &vector)`
- `token_vector_from_moonshine_tensor` (function) `core/ort-utils/moonshine-tensor-view.cpp:325` `std::vector<int32_t> token_vector_from_moonshine_tensor(
    MoonshineTensorView *moonshine_tensor)`
- `create_ort_value` (function) `core/ort-utils/moonshine-tensor-view.cpp:332` `OrtValue *MoonshineTensorView::create_ort_value(const OrtApi *ort_api,
                          ...`
- `float16_to_float32` (function) `core/ort-utils/moonshine-tensor-view.cpp:345` `void float16_to_float32(const uint16_t *f16_array, float *f32_array,
                        size...` -- Thank you Claude.
- `to_string` (function) `core/ort-utils/moonshine-tensor-view.cpp:387` `std::string MoonshineTensorView::to_string()`

## core/ort-utils/moonshine-tensor-view.h
Depends on: `core/ort-utils/moonshine-tensor.h`
Imported by: `core/moonshine-c-api.cpp`, `core/moonshine-model.cpp`, `core/ort-utils/moonshine-tensor-view.cpp`, `core/reliability/fuzz-tensor-view.cpp`, `core/spelling-model.cpp`
- `moonshine_dtype_to_bytes_per_element` (function) `core/ort-utils/moonshine-tensor-view.h:34` `size_t moonshine_dtype_to_bytes_per_element(uint32_t moonshine_dtype);`
- `ort_dtype_to_moonshine_dtype` (function) `core/ort-utils/moonshine-tensor-view.h:36` `moonshine_dtype_t ort_dtype_to_moonshine_dtype( ONNXTensorElementDataType ort_dtype);`
- `ort_dtype_to_bytes_per_element` (function) `core/ort-utils/moonshine-tensor-view.h:42` `size_t ort_dtype_to_bytes_per_element(ONNXTensorElementDataType ort_dtype);`
- `moonshine_tensor_from_token_vector` (function) `core/ort-utils/moonshine-tensor-view.h:44` `MoonshineTensorView *moonshine_tensor_from_token_vector( std::vector<int32_t> &vector);`
- `token_vector_from_moonshine_tensor` (function) `core/ort-utils/moonshine-tensor-view.h:47` `std::vector<int32_t> token_vector_from_moonshine_tensor( MoonshineTensorView *moonshine_tensor);`
- `float16_to_float32` (function) `core/ort-utils/moonshine-tensor-view.h:50` `void float16_to_float32(const uint16_t *f16_array, float *f32_array, size_t count);`
- `log_leaked_tensor_views` (function) `core/ort-utils/moonshine-tensor-view.h:53` `void log_leaked_tensor_views();`
- `data` (function) `core/ort-utils/moonshine-tensor-view.h:78` `template <typename T>
  T *data()`
- `shape` (function) `core/ort-utils/moonshine-tensor-view.h:82` `std::vector<int64_t> &shape();`
- `element_count` (function) `core/ort-utils/moonshine-tensor-view.h:84` `size_t element_count();`
- `bytes_count` (function) `core/ort-utils/moonshine-tensor-view.h:86` `size_t bytes_count();`
- `dtype` (function) `core/ort-utils/moonshine-tensor-view.h:88` `uint32_t dtype();`
- `reshape` (function) `core/ort-utils/moonshine-tensor-view.h:90` `void reshape(const std::vector<int64_t> &shape);`
- `argmax` (function) `core/ort-utils/moonshine-tensor-view.h:94` `int64_t argmax();`
- `create_ort_value` (function) `core/ort-utils/moonshine-tensor-view.h:98` `OrtValue *create_ort_value(const OrtApi *ort_api, OrtMemoryInfo *memory_info);` -- You need to call ort_api->ReleaseValue(output_ort_tensor) to release this OrtValue.

## core/ort-utils/moonshine-tensor.h
Imported by: `core/ort-utils/moonshine-tensor-view.h`, `core/ort-utils/moonshine-tensor.cpp`
- `moonshine_free_tensor` (function) `core/ort-utils/moonshine-tensor.h:39` `void moonshine_free_tensor(moonshine_tensor_t *tensor);`
- `moonshine_free_tensor_list` (function) `core/ort-utils/moonshine-tensor.h:41` `void moonshine_free_tensor_list(moonshine_tensor_list_t *tensor_list);`

## core/ort-utils/ort-utils-ep.cpp
Depends on: `core/ort-utils/ort-utils.h`
- `trim_copy` (function) `core/ort-utils/ort-utils-ep.cpp:17` `std::string trim_copy(const std::string &s)`
- `lowercase_copy` (function) `core/ort-utils/ort-utils-ep.cpp:29` `std::string lowercase_copy(std::string s)`
- `normalize_provider_name` (function) `core/ort-utils/ort-utils-ep.cpp:36` `std::string normalize_provider_name(const std::string &name)`
- `make_invalid_argument_status` (function) `core/ort-utils/ort-utils-ep.cpp:51` `OrtStatus *make_invalid_argument_status(const OrtApi *ort_api,
                                  ...`
- `append_one_provider` (function) `core/ort-utils/ort-utils-ep.cpp:56` `OrtStatus *append_one_provider(
    const OrtApi *ort_api, OrtSessionOptions *session_options,
  ...`
- `ort_parse_provider_names` (function) `core/ort-utils/ort-utils-ep.cpp:102` `std::vector<std::string> ort_parse_provider_names(const std::string &csv)`
- `ort_append_execution_providers` (function) `core/ort-utils/ort-utils-ep.cpp:126` `OrtStatus *ort_append_execution_providers(
    const OrtApi *ort_api, OrtSessionOptions *session_...`

## core/ort-utils/ort-utils.cpp
Depends on: `core/ort-utils/ort-utils.h`
- `ort_session_from_path` (function) `core/ort-utils/ort-utils.cpp:18` `int ort_session_from_path(const OrtApi *ort_api, OrtEnv *env,
                          OrtSessio...` -- ifdef _WIN32 No memory mapping on Windows and wchar for the file path.
- `ort_session_from_path` (function) `core/ort-utils/ort-utils.cpp:37` `int ort_session_from_path(const OrtApi *ort_api, OrtEnv *env,
                          OrtSessio...` -- else
- `ort_session_from_memory` (function) `core/ort-utils/ort-utils.cpp:82` `int ort_session_from_memory(const OrtApi *ort_api, OrtEnv *env,
                            OrtSe...`
- `ort_maybe_force_single_thread` (function) `core/ort-utils/ort-utils.cpp:94` `void ort_maybe_force_single_thread(const OrtApi *ort_api,
                                   OrtS...`
- `ort_session_from_asset` (function) `core/ort-utils/ort-utils.cpp:107` `int ort_session_from_asset(const OrtApi *ort_api, OrtEnv *env,
                           OrtSess...` -- if defined(ANDROID)
- `ort_get_shape` (function) `core/ort-utils/ort-utils.cpp:152` `std::vector<int64_t> ort_get_shape(const OrtApi *ort_api,
                                   OrtT...`
- `shape` (function) `core/ort-utils/ort-utils.cpp:163` `std::vector<int64_t> shape(num_dims);`
- `ort_get_type` (function) `core/ort-utils/ort-utils.cpp:169` `ONNXTensorElementDataType ort_get_type(const OrtApi *ort_api,
                                   ...`
- `ort_get_input_shape` (function) `core/ort-utils/ort-utils.cpp:179` `std::vector<int64_t> ort_get_input_shape(const OrtApi *ort_api,
                                 ...`
- `ort_get_input_type` (function) `core/ort-utils/ort-utils.cpp:189` `ONNXTensorElementDataType ort_get_input_type(const OrtApi *ort_api,
                             ...`
- `ort_get_output_shape` (function) `core/ort-utils/ort-utils.cpp:199` `std::vector<int64_t> ort_get_output_shape(const OrtApi *ort_api,
                                ...`
- `ort_get_output_type` (function) `core/ort-utils/ort-utils.cpp:209` `ONNXTensorElementDataType ort_get_output_type(const OrtApi *ort_api,
                            ...`
- `ort_get_value_shape` (function) `core/ort-utils/ort-utils.cpp:219` `std::vector<int64_t> ort_get_value_shape(const OrtApi *ort_api,
                                 ...`
- `ort_get_value_type` (function) `core/ort-utils/ort-utils.cpp:228` `ONNXTensorElementDataType ort_get_value_type(const OrtApi *ort_api,
                             ...`
- `ort_run` (function) `core/ort-utils/ort-utils.cpp:237` `OrtStatus *ort_run(const OrtApi *ort_api, OrtSession *session,
                   const char *con...`

## core/ort-utils/ort-utils.h
Depends on: `core/moonshine-utils/debug-utils.h`
Imported by: `core/gemma-embedding-model.cpp`, `core/moonshine-c-api.cpp`, `core/moonshine-model.cpp`, `core/moonshine-streaming-model.cpp`, `core/moonshine-tts/src/moonshine-g2p-options.cpp`, `core/moonshine-tts/src/moonshine-tts-options.cpp`, `core/moonshine-tts/src/ort-session-options.h`, `core/ort-utils/moonshine-tensor-view.cpp`, `core/ort-utils/moonshine-tensor.cpp`, `core/ort-utils/ort-utils-cxx.h`, `core/ort-utils/ort-utils-ep-test.cpp`, `core/ort-utils/ort-utils-ep.cpp`, `core/ort-utils/ort-utils-test.cpp`, `core/ort-utils/ort-utils.cpp`, `core/silero-vad.cpp`, `core/spelling-model.cpp`
- `ort_session_from_path` (function) `core/ort-utils/ort-utils.h:40` `int ort_session_from_path(const OrtApi *ort_api, OrtEnv *env, OrtSessionOptions *session_options, const char *path...`
- `ort_session_from_memory` (function) `core/ort-utils/ort-utils.h:45` `int ort_session_from_memory(const OrtApi *ort_api, OrtEnv *env, OrtSessionOptions *session_options, const uint8_t...`
- `ort_session_from_asset` (function) `core/ort-utils/ort-utils.h:51` `int ort_session_from_asset(const OrtApi *ort_api, OrtEnv *env, OrtSessionOptions *session_options, AAssetManager...` -- if defined(ANDROID)
- `ort_get_shape` (function) `core/ort-utils/ort-utils.h:58` `std::vector<int64_t> ort_get_shape(const OrtApi *ort_api, OrtTypeInfo *type_info);`
- `ort_get_input_shape` (function) `core/ort-utils/ort-utils.h:64` `std::vector<int64_t> ort_get_input_shape(const OrtApi *ort_api, OrtSession *session, int index);`
- `ort_get_output_shape` (function) `core/ort-utils/ort-utils.h:70` `std::vector<int64_t> ort_get_output_shape(const OrtApi *ort_api, OrtSession *session, int index);`
- `ort_get_value_shape` (function) `core/ort-utils/ort-utils.h:76` `std::vector<int64_t> ort_get_value_shape(const OrtApi *ort_api, const OrtValue *value);`
- `ort_maybe_force_single_thread` (function) `core/ort-utils/ort-utils.h:104` `void ort_maybe_force_single_thread(const OrtApi *ort_api, OrtSessionOptions *session_options);` -- Reliability-only escape hatch: when the MOONSHINE_ORT_SINGLE_THREAD environment variable is set to a non-empty value...
- `ort_append_execution_providers` (function) `core/ort-utils/ort-utils.h:109` `OrtStatus *ort_append_execution_providers( const OrtApi *ort_api, OrtSessionOptions *session_options, const...`
- `ort_configure_execution_providers` (function) `core/ort-utils/ort-utils.h:114` `inline void ort_configure_execution_providers(
    const OrtApi *ort_api, OrtSessionOptions *sess...`

## core/reliability/fuzz-bin-tokenizer.cpp
Depends on: `core/bin-tokenizer/bin-tokenizer.h`
- `text` (function) `core/reliability/fuzz-bin-tokenizer.cpp:25` `const std::string text(data, data + text_size);`

## core/reliability/fuzz-resampler.cpp
Depends on: `core/resampler.h`
- `sane_rate` (function) `core/reliability/fuzz-resampler.cpp:17` `float sane_rate(float rate)`
- `audio` (function) `core/reliability/fuzz-resampler.cpp:45` `std::vector<float> audio(num_samples);`

## core/reliability/fuzz-string-utils.cpp
Depends on: `core/moonshine-utils/string-utils.h`
- `input` (function) `core/reliability/fuzz-string-utils.cpp:15` `const std::string input(data, data + size);`

## core/reliability/fuzz-tensor-view.cpp
Depends on: `core/ort-utils/moonshine-tensor-view.h`
- `next_u8` (function) `core/reliability/fuzz-tensor-view.cpp:26` `uint8_t next_u8()`
- `next_i64` (function) `core/reliability/fuzz-tensor-view.cpp:28` `int64_t next_i64()`
- `source` (function) `core/reliability/fuzz-tensor-view.cpp:82` `std::vector<uint8_t> source(element_count * 8, 0);` -- 8 bytes/element is the widest dtype, so this source is always at least as large as the copy the constructor performs.

## core/resampler.cpp
Depends on: `core/moonshine-utils/debug-utils.h`, `core/resampler.h`
- `resample_audio` (function) `core/resampler.cpp:5` `const std::vector<float> resample_audio(const std::vector<float> &audio,
                        ...`
- `downsample_audio` (function) `core/resampler.cpp:17` `const std::vector<float> downsample_audio(const std::vector<float> &audio,
                      ...`
- `output_audio` (function) `core/resampler.cpp:23` `std::vector<float> output_audio(output_audio_size);`
- `upsample_audio` (function) `core/resampler.cpp:56` `const std::vector<float> upsample_audio(const std::vector<float> &audio,
                        ...`

## core/resampler.h
Imported by: `core/reliability/fuzz-resampler.cpp`, `core/resampler-test.cpp`, `core/resampler.cpp`, `core/voice-activity-detector.cpp`
- `resample_audio` (function) `core/resampler.h:6` `const std::vector<float> resample_audio(const std::vector<float> &audio, float input_sample_rate, float...`
- `downsample_audio` (function) `core/resampler.h:10` `const std::vector<float> downsample_audio(const std::vector<float> &audio, float input_sample_rate, float...`
- `upsample_audio` (function) `core/resampler.h:14` `const std::vector<float> upsample_audio(const std::vector<float> &audio, float input_sample_rate, float...`

## core/silero-vad.cpp
Depends on: `core/ort-utils/ort-utils.h`, `core/silero-vad.h`
- `init_onnx_env` (function) `core/silero-vad.cpp:6` `void SileroVad::init_onnx_env()`
- `init_engine_threads` (function) `core/silero-vad.cpp:21` `void SileroVad::init_engine_threads(int inter_threads, int intra_threads)` -- Initializes threading settings.
- `SileroVad` (function) `core/silero-vad.cpp:30` `SileroVad::SileroVad(int sample_rate, int windows_frame_size, float threshold,
                  ...`
- `load_from_memory` (function) `core/silero-vad.cpp:60` `int SileroVad::load_from_memory(const uint8_t *model_data,
                                size_t...`
- `predict` (function) `core/silero-vad.cpp:78` `void SileroVad::predict(const std::vector<float> &data_chunk,
                        float *out_...` -- Inference: runs inference on one chunk of input data. data_chunk is expected to have window_size_samples samples...

## core/silero-vad.h
Imported by: `core/silero-vad.cpp`, `core/voice-activity-detector.h`
- `init_onnx_env` (function) `core/silero-vad.h:68` `void init_onnx_env();` -- Initializes the common ONNX runtime environment (env, session_options, memory_info, allocator).
- `init_engine_threads` (function) `core/silero-vad.h:71` `void init_engine_threads(int inter_threads, int intra_threads);` -- Initializes threading settings.
- `load_from_memory` (function) `core/silero-vad.h:83` `int load_from_memory(const uint8_t *model_data, size_t model_data_size);` -- Load model from memory buffer.
- `is_loaded` (function) `core/silero-vad.h:85` `bool is_loaded() const`
- `predict` (function) `core/silero-vad.h:87` `void predict(const std::vector<float> &data_chunk, float *out_probability, int *out_flag);`

## core/speaker-diarizer.cpp
Depends on: `core/cpp-annote/src/cpp-annote-engine.h`, `core/cpp-annote/src/cpp-annote-streaming.h`, `core/moonshine-utils/debug-utils.h`, `core/speaker-diarizer.h`
- `turn_overlap_seconds` (function) `core/speaker-diarizer.cpp:17` `double turn_overlap_seconds(
    const std::vector<cppannote::StreamingDiarizationTurn> &a, int32...` -- Total seconds of overlap between the spans of two turn lists.
- `Impl` (function) `core/speaker-diarizer.cpp:67` `explicit Impl(const SpeakerDiarizerOptions &options_in)
      : engine(), options(options_in)`
- `session_config` (function) `core/speaker-diarizer.cpp:75` `cppannote::StreamingDiarizationConfig session_config() const`
- `get_stream` (function) `core/speaker-diarizer.cpp:83` `StreamState &get_stream(int32_t stream_id)`
- `allocate_stable_id` (function) `core/speaker-diarizer.cpp:92` `uint64_t allocate_stable_id()`
- `map_snapshot_to_stable_ids` (function) `core/speaker-diarizer.cpp:102` `void map_snapshot_to_stable_ids(
      StreamState &state,
      const cppannote::StreamingDiariz...` -- Maps the clustering labels in `snapshot` onto stable speaker IDs by greedily matching each label against the labels...
- `sort` (function) `core/speaker-diarizer.cpp:135` `std::sort(candidates.begin(), candidates.end(),
              [](const auto &a, const auto &b)`
- `SpeakerDiarizer` (function) `core/speaker-diarizer.cpp:171` `SpeakerDiarizer::SpeakerDiarizer(const SpeakerDiarizerOptions &options)
    : impl(std::make_uniq...`
- `create_stream` (function) `core/speaker-diarizer.cpp:176` `int32_t SpeakerDiarizer::create_stream()`
- `free_stream` (function) `core/speaker-diarizer.cpp:186` `void SpeakerDiarizer::free_stream(int32_t stream_id)`
- `start_stream` (function) `core/speaker-diarizer.cpp:191` `void SpeakerDiarizer::start_stream(int32_t stream_id)`
- `add_audio_to_stream` (function) `core/speaker-diarizer.cpp:201` `void SpeakerDiarizer::add_audio_to_stream(int32_t stream_id,
                                    ...`
- `get_turns` (function) `core/speaker-diarizer.cpp:218` `std::vector<SpeakerTurn> SpeakerDiarizer::get_turns(int32_t stream_id)`
- `finish_stream` (function) `core/speaker-diarizer.cpp:225` `std::vector<SpeakerTurn> SpeakerDiarizer::finish_stream(int32_t stream_id)`
- `diarize` (function) `core/speaker-diarizer.cpp:236` `std::vector<SpeakerTurn> SpeakerDiarizer::diarize(const float *audio_data,
                      ...`

## core/speaker-diarizer.h
Imported by: `core/speaker-diarizer.cpp`
- `create_stream` (function) `core/speaker-diarizer.h:51` `int32_t create_stream();`
- `free_stream` (function) `core/speaker-diarizer.h:52` `void free_stream(int32_t stream_id);`
- `start_stream` (function) `core/speaker-diarizer.h:53` `void start_stream(int32_t stream_id);`
- `add_audio_to_stream` (function) `core/speaker-diarizer.h:58` `void add_audio_to_stream(int32_t stream_id, const float *audio_data, uint64_t audio_length, int32_t sample_rate);` -- Appends audio to the stream.

## core/spelling-fusion-data.cpp
Depends on: `core/spelling-fusion-data.h`, `core/spelling-fusion.h`
- `build_set` (function) `core/spelling-fusion-data.cpp:28` `std::unordered_set<std::string> build_set(
    std::initializer_list<const char *> phrases)`
- `upper_modifiers` (function) `core/spelling-fusion-data.cpp:268` `const std::unordered_set<std::string> &upper_modifiers()`
- `upper_modifiers_by_length` (function) `core/spelling-fusion-data.cpp:281` `const std::vector<std::string> &upper_modifiers_by_length()`
- `sort` (function) `core/spelling-fusion-data.cpp:287` `std::sort(v.begin(), v.end(),
              [](const std::string &a, const std::string &b)`
- `undo_words` (function) `core/spelling-fusion-data.cpp:296` `const std::unordered_set<std::string> &undo_words()`
- `clear_words` (function) `core/spelling-fusion-data.cpp:309` `const std::unordered_set<std::string> &clear_words()`
- `stop_words` (function) `core/spelling-fusion-data.cpp:319` `const std::unordered_set<std::string> &stop_words()`
- `default_weak_homonyms` (function) `core/spelling-fusion-data.cpp:338` `const std::unordered_set<std::string> &default_weak_homonyms()`
- `default_meta` (function) `core/spelling-fusion-data.cpp:356` `const DefaultSpellingMeta &default_meta()`

## core/spelling-fusion-data.h
Imported by: `core/spelling-fusion-data.cpp`, `core/spelling-fusion-test.cpp`, `core/spelling-fusion.cpp`, `core/spelling-model.cpp`
- `upper_modifiers` (function) `core/spelling-fusion-data.h:27` `const std::unordered_set<std::string> &upper_modifiers();` -- Set of normalized "make next letter upper" modifier phrases.
- `upper_modifiers_by_length` (function) `core/spelling-fusion-data.h:28` `const std::vector<std::string> &upper_modifiers_by_length();`
- `undo_words` (function) `core/spelling-fusion-data.h:32` `const std::unordered_set<std::string> &undo_words();` -- Normalized command-word vocabularies.
- `clear_words` (function) `core/spelling-fusion-data.h:33` `const std::unordered_set<std::string> &clear_words();`
- `stop_words` (function) `core/spelling-fusion-data.h:34` `const std::unordered_set<std::string> &stop_words();`
- `default_weak_homonyms` (function) `core/spelling-fusion-data.h:40` `const std::unordered_set<std::string> &default_weak_homonyms();` -- Default weak-homonym phrases (``okay`` / ``ok`` / ``you``).
- `default_meta` (function) `core/spelling-fusion-data.h:60` `const DefaultSpellingMeta &default_meta();`

## core/spelling-fusion.cpp
Depends on: `core/spelling-fusion-data.h`, `core/spelling-fusion.h`
- `is_ascii_drop` (function) `core/spelling-fusion.cpp:25` `bool is_ascii_drop(char c)`
- `is_ascii_letter` (function) `core/spelling-fusion.cpp:35` `bool is_ascii_letter(char c)`
- `ascii_to_lower` (function) `core/spelling-fusion.cpp:39` `char ascii_to_lower(char c)`
- `consume_curly_quote` (function) `core/spelling-fusion.cpp:46` `size_t consume_curly_quote(const std::string &input, size_t i)` -- Try to consume a 3-byte UTF-8 curly quote starting at ``input[i]``.
- `split_on_whitespace` (function) `core/spelling-fusion.cpp:62` `std::vector<std::string> split_on_whitespace(const std::string &s)` -- Split ``s`` on ASCII whitespace, dropping empty tokens.
- `parse_number_words` (function) `core/spelling-fusion.cpp:108` `std::optional<int> parse_number_words(const std::string &text)`
- `is_ascii_digit_string` (function) `core/spelling-fusion.cpp:181` `bool is_ascii_digit_string(const std::string &s)`
- `is_printable_ascii` (function) `core/spelling-fusion.cpp:189` `bool is_printable_ascii(char c)`
- `spelling_normalize` (function) `core/spelling-fusion.cpp:195` `std::string spelling_normalize(const std::string &text)`
- `SpellingMatcher` (function) `core/spelling-fusion.cpp:234` `SpellingMatcher::SpellingMatcher()
    : lookup_(&spelling_fusion_data::lookup_table()),
      up...`
- `classify` (function) `core/spelling-fusion.cpp:244` `SpellingMatch SpellingMatcher::classify(const std::string &raw_text) const`
- `is_weak_homonym` (function) `core/spelling-fusion.cpp:300` `bool SpellingMatcher::is_weak_homonym(const std::string &raw_text) const`
- `resolve` (function) `core/spelling-fusion.cpp:305` `std::optional<std::string> SpellingMatcher::resolve(
    const std::string &text) const`
- `resolve_spelled_letter` (function) `core/spelling-fusion.cpp:326` `std::optional<std::string> SpellingMatcher::resolve_spelled_letter(
    const std::string &text) ...`
- `string_is_letter` (function) `core/spelling-fusion.cpp:373` `bool string_is_letter(const std::string &c)` -- Mirror Python's ``str.isalpha()`` / ``str.isdigit()`` semantics on the ASCII strings that the matcher emits.
- `string_is_digit` (function) `core/spelling-fusion.cpp:381` `bool string_is_digit(const std::string &c)`
- `single_char_is_letter` (function) `core/spelling-fusion.cpp:389` `bool single_char_is_letter(const std::string &c)`
- `apply_case` (function) `core/spelling-fusion.cpp:393` `std::string apply_case(const std::string &ch, const std::string &hint)`
- `fuse_default` (function) `core/spelling-fusion.cpp:407` `FusedResult fuse_default(const std::string &raw_text,
                         const SpellingMatc...`

## core/spelling-fusion.h
Imported by: `core/spelling-fusion-data.cpp`, `core/spelling-fusion-test.cpp`, `core/spelling-fusion.cpp`, `core/spelling-model-test.cpp`, `core/spelling-model.h`
- `is_character` (function) `core/spelling-fusion.h:41` `bool is_character() const`
- `is_recognized` (function) `core/spelling-fusion.h:42` `bool is_recognized() const`
- `is_weak_homonym` (function) `core/spelling-fusion.h:66` `bool is_weak_homonym(const std::string &raw_text) const;` -- True iff ``raw_text`` normalizes to one of the weak-homonym phrases (``okay`` / ``ok`` / ``you``).
- `is_character` (function) `core/spelling-fusion.h:91` `bool is_character() const`

## core/spelling-model-test.cpp
Depends on: `core/moonshine-utils/debug-utils.h`, `core/spelling-fusion.h`, `core/spelling-model.h`
- `find_model_path` (function) `core/spelling-model-test.cpp:21` `std::string find_model_path()` -- Locate the bundled spelling model.
- `find_wav` (function) `core/spelling-model-test.cpp:33` `std::string find_wav(const std::string &label, const std::string &filename)`
- `read_file` (function) `core/spelling-model-test.cpp:47` `std::vector<uint8_t> read_file(const std::string &path)` -- Read entire file into a byte buffer.
- `buffer` (function) `core/spelling-model-test.cpp:53` `std::vector<uint8_t> buffer(static_cast<size_t>(size));`
- `TEST_CASE` (function) `core/spelling-model-test.cpp:60` `TEST_CASE("spelling-model: load from path")`
- `TEST_CASE` (function) `core/spelling-model-test.cpp:73` `TEST_CASE("spelling-model: load from memory")`
- `TEST_CASE` (function) `core/spelling-model-test.cpp:86` `TEST_CASE("spelling-model: predict on bundled clips")`
- `TEST_CASE` (function) `core/spelling-model-test.cpp:133` `TEST_CASE("spelling-model: invalid arguments are rejected")`
- `dummy` (function) `core/spelling-model-test.cpp:143` `std::vector<float> dummy(16000, 0.0f);` -- Wrong sample rate.

## core/spelling-model.cpp
Depends on: `core/moonshine-utils/debug-utils.h`, `core/ort-utils/moonshine-tensor-view.h`, `core/ort-utils/ort-utils.h`, `core/spelling-fusion-data.h`, `core/spelling-model.h`
- `lookup_metadata` (function) `core/spelling-model.cpp:26` `std::optional<std::string> lookup_metadata(const OrtApi *ort_api,
                               ...` -- Read a single key from the model's custom_metadata_map, returning nullopt when the key isn't present or any ORT call...
- `trim` (function) `core/spelling-model.cpp:45` `std::string trim(const std::string &s)` -- Trim ASCII whitespace.
- `parse_class_list_json` (function) `core/spelling-model.cpp:59` `std::vector<std::string> parse_class_list_json(const std::string &raw)` -- Parse a JSON string array of class labels (e.g.
- `SpellingModel` (function) `core/spelling-model.cpp:95` `SpellingModel::SpellingModel(bool log_ort_run,
                             const std::vector<std...`
- `initialize_session_options` (function) `core/spelling-model.cpp:137` `void SpellingModel::initialize_session_options()`
- `apply_default_metadata` (function) `core/spelling-model.cpp:157` `void SpellingModel::apply_default_metadata()`
- `load` (function) `core/spelling-model.cpp:169` `int SpellingModel::load(const char *model_path)`
- `load_from_memory` (function) `core/spelling-model.cpp:177` `int SpellingModel::load_from_memory(const uint8_t *model_data,
                                  ...`
- `populate_metadata_from_session` (function) `core/spelling-model.cpp:186` `int SpellingModel::populate_metadata_from_session()`
- `predict` (function) `core/spelling-model.cpp:243` `int SpellingModel::predict(const float *audio, size_t audio_size,
                           int3...`
- `clip` (function) `core/spelling-model.cpp:260` `std::vector<float> clip(target_samples_, 0.0f);`
- `probs` (function) `core/spelling-model.cpp:307` `std::vector<float> probs(row_size);`

## core/spelling-model.h
Depends on: `core/spelling-fusion.h`
Imported by: `core/spelling-model-test.cpp`, `core/spelling-model.cpp`
- `load` (function) `core/spelling-model.h:39` `int load(const char *model_path);` -- Load from a ``.ort`` file on disk.
- `load_from_memory` (function) `core/spelling-model.h:43` `int load_from_memory(const uint8_t *model_data, size_t model_data_size);` -- Load from a memory buffer.
- `predict` (function) `core/spelling-model.h:52` `int predict(const float *audio, size_t audio_size, int32_t sample_rate, SpellingPrediction *out_prediction);` -- Run the model on a single audio clip and write the top-1 prediction to ``out_prediction``.
- `sample_rate` (function) `core/spelling-model.h:56` `int32_t sample_rate() const` -- Accessors.
- `clip_seconds` (function) `core/spelling-model.h:57` `float clip_seconds() const`
- `classes` (function) `core/spelling-model.h:58` `const std::vector<std::string> &classes() const`
- `initialize_session_options` (function) `core/spelling-model.h:61` `private: void initialize_session_options();`
- `populate_metadata_from_session` (function) `core/spelling-model.h:62` `int populate_metadata_from_session();`
- `apply_default_metadata` (function) `core/spelling-model.h:63` `void apply_default_metadata();`

## core/voice-activity-detector.cpp
Depends on: `core/moonshine-utils/debug-utils.h`, `core/resampler.h`, `core/voice-activity-detector.h`
- `seconds_from_sample_count` (function) `core/voice-activity-detector.cpp:15` `float seconds_from_sample_count(size_t sample_count)`
- `VoiceActivityDetector` (function) `core/voice-activity-detector.cpp:24` `VoiceActivityDetector::VoiceActivityDetector(float threshold,
                                   ...`
- `start` (function) `core/voice-activity-detector.cpp:50` `void VoiceActivityDetector::start()`
- `stop` (function) `core/voice-activity-detector.cpp:62` `void VoiceActivityDetector::stop()`
- `process_audio` (function) `core/voice-activity-detector.cpp:69` `void VoiceActivityDetector::process_audio(const float *audio_data,
                              ...`
- `input_audio_vector` (function) `core/voice-activity-detector.cpp:79` `std::vector<float> input_audio_vector(audio_data, audio_data + audio_data_size);`
- `clear_completed_segment_audio_data` (function) `core/voice-activity-detector.cpp:99` `void VoiceActivityDetector::clear_completed_segment_audio_data()`
- `retained_segment_audio_byte_count` (function) `core/voice-activity-detector.cpp:107` `size_t VoiceActivityDetector::retained_segment_audio_byte_count() const`
- `completed_segment_audio_byte_count` (function) `core/voice-activity-detector.cpp:115` `size_t VoiceActivityDetector::completed_segment_audio_byte_count() const`
- `process_audio_chunk` (function) `core/voice-activity-detector.cpp:125` `void VoiceActivityDetector::process_audio_chunk(const float *audio_data,
                        ...`
- `audio_vec` (function) `core/voice-activity-detector.cpp:136` `std::vector<float> audio_vec(audio_data, audio_data + audio_data_size);`
- `on_voice_start` (function) `core/voice-activity-detector.cpp:196` `void VoiceActivityDetector::on_voice_start()`
- `on_voice_continuing` (function) `core/voice-activity-detector.cpp:210` `void VoiceActivityDetector::on_voice_continuing()`
- `on_voice_end` (function) `core/voice-activity-detector.cpp:219` `void VoiceActivityDetector::on_voice_end()`
- `to_string` (function) `core/voice-activity-detector.cpp:228` `std::string VoiceActivitySegment::to_string() const`
- `to_string` (function) `core/voice-activity-detector.cpp:238` `std::string VoiceActivityDetector::to_string() const`

## core/voice-activity-detector.h
Depends on: `core/silero-vad.h`
Imported by: `core/voice-activity-detector-test.cpp`, `core/voice-activity-detector.cpp`
- `start` (function) `core/voice-activity-detector.h:51` `void start();`
- `stop` (function) `core/voice-activity-detector.h:52` `void stop();`
- `is_active` (function) `core/voice-activity-detector.h:53` `bool is_active() const`
- `process_audio` (function) `core/voice-activity-detector.h:54` `void process_audio(const float *audio_data, size_t audio_data_size, int32_t sample_rate);`
- `get_segments` (function) `core/voice-activity-detector.h:56` `const std::vector<VoiceActivitySegment> *get_segments() const`
- `retained_segment_audio_byte_count` (function) `core/voice-activity-detector.h:59` `size_t retained_segment_audio_byte_count() const;`
- `completed_segment_audio_byte_count` (function) `core/voice-activity-detector.h:60` `size_t completed_segment_audio_byte_count() const;`
- `clear_completed_segment_audio_data` (function) `core/voice-activity-detector.h:61` `void clear_completed_segment_audio_data();`
- `clear` (function) `core/voice-activity-detector.h:65` `private: void clear();`
- `on_voice_start` (function) `core/voice-activity-detector.h:66` `void on_voice_start();`
- `on_voice_end` (function) `core/voice-activity-detector.h:67` `void on_voice_end();`
- `on_voice_continuing` (function) `core/voice-activity-detector.h:68` `void on_voice_continuing();`
- `process_audio_chunk` (function) `core/voice-activity-detector.h:69` `void process_audio_chunk(const float *audio_data, size_t audio_data_size);`

## core/word-alignment-benchmark.cpp
Depends on: `core/moonshine-c-api.h`, `core/moonshine-utils/file-utils.h`
- `load_wav` (function) `core/word-alignment-benchmark.cpp:10` `static float* load_wav(const char* path, long* num_samples_out)`
- `run_benchmark` (function) `core/word-alignment-benchmark.cpp:38` `static BenchResult run_benchmark(const char* model_path, const char* wav_path,
                  ...`
- `main` (function) `core/word-alignment-benchmark.cpp:97` `int main(int argc, char** argv)`

## core/word-alignment.cpp
Depends on: `core/word-alignment.h`
- `dtw` (function) `core/word-alignment.cpp:12` `void dtw(const std::vector<float>& cost_matrix, int N, int M,
         std::vector<int>& text_ind...`
- `D` (function) `core/word-alignment.cpp:16` `std::vector<float> D((N + 1) * (M + 1), std::numeric_limits<float>::infinity());` -- Cumulative cost matrix D of size (N+1) x (M+1), initialized to infinity
- `trace` (function) `core/word-alignment.cpp:22` `std::vector<int> trace(N * M, 0);` -- Trace matrix of size N x M, stores which predecessor was chosen (0, 1, or 2)
- `compute_median` (function) `core/word-alignment.cpp:93` `static float compute_median(std::vector<float>& window)`
- `median_filter` (function) `core/word-alignment.cpp:99` `void median_filter(std::vector<float>& data, int channels, int height,
                   int wid...`
- `padded` (function) `core/word-alignment.cpp:114` `std::vector<float> padded(padded_width);` -- Work buffer for one row (padded with reflected values)
- `window` (function) `core/word-alignment.cpp:115` `std::vector<float> window(filter_width);`
- `result_row` (function) `core/word-alignment.cpp:116` `std::vector<float> result_row(width);`
- `token_starts_new_word` (function) `core/word-alignment.cpp:159` `static bool token_starts_new_word(BinTokenizer* tokenizer, int token_id)`
- `decode_tokens` (function) `core/word-alignment.cpp:174` `static std::string decode_tokens(BinTokenizer* tokenizer,
                                 const ...`
- `align_words` (function) `core/word-alignment.cpp:181` `std::vector<TranscriberWord> align_words(const float* cross_attention_data,
                     ...`
- `weights` (function) `core/word-alignment.cpp:200` `std::vector<float> weights(total_size);`
- `matrix` (function) `core/word-alignment.cpp:250` `std::vector<float> matrix(n_steps * encoder_frames, 0.0f);`
- `neg_matrix` (function) `core/word-alignment.cpp:270` `std::vector<float> neg_matrix(matrix.size());`

## core/word-alignment.h
Depends on: `core/bin-tokenizer/bin-tokenizer.h`
Imported by: `core/moonshine-model.h`, `core/moonshine-streaming-model.h`, `core/word-alignment.cpp`
- `dtw` (function) `core/word-alignment.h:18` `void dtw(const std::vector<float>& cost_matrix, int N, int M, std::vector<int>& text_indices_out, std::vector<int>&...` -- Dynamic Time Warping on a cost matrix [N x M] Returns aligned (text_indices, time_indices) arrays
- `median_filter` (function) `core/word-alignment.h:24` `void median_filter(std::vector<float>& data, int channels, int height, int width, int filter_width);` -- Apply median filter along the last axis of a 3D array [C x H x W] filter_width should be odd

## examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/AssetDirectoryCopy.kt
- `copyDirIfNeeded` (function) `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/AssetDirectoryCopy.kt:10` -- package ai.moonshine.examples.intentrecognizer import android.content.Context import java.io.File import...

## examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/PhraseAdapter.kt
- `resetToDefaults` (function) `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/PhraseAdapter.kt:27`
- `addEmptyRow` (function) `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/PhraseAdapter.kt:40`
- `removeRow` (function) `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/PhraseAdapter.kt:46`
- `flashHighlight` (function) `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/PhraseAdapter.kt:54`
- `currentPhrases` (function) `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/PhraseAdapter.kt:71` -- val idx = items.indexOfFirst { it.id == id } if (idx >= 0) { notifyItemChanged(idx) }...
- `rowIdMatchingCanonical` (function) `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/PhraseAdapter.kt:72`
- `bind` (function) `examples/android/IntentRecognizer/app/src/main/java/ai/moonshine/examples/intentrecognizer/PhraseAdapter.kt:89`

## examples/android/TextToSpeech/app/src/main/java/ai/moonshine/examples/texttospeech/AssetDirectoryCopy.kt
- `copyDirIfNeeded` (function) `examples/android/TextToSpeech/app/src/main/java/ai/moonshine/examples/texttospeech/AssetDirectoryCopy.kt:10` -- package ai.moonshine.examples.texttospeech import android.content.Context import java.io.File import...

## examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java
Depends on: `android/java/main/java/ai/moonshine/voice/JNI.java`, `android/java/main/java/ai/moonshine/voice/TranscriptEvent.java`
- `MainActivity.onCreate` (method) `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java:50`
- `MainActivity.TranscriptEventListener` (method) `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java:62`
- `MainActivity.onLineTextChanged` (method) `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java:64`
- `MainActivity.onLineCompleted` (method) `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java:75`
- `MainActivity.onDestroy` (method) `examples/android/Transcriber/app/src/main/java/ai/moonshine/androidtranscriber/MainActivity.java:133`


Next: [API_p7.md](API_p7.md)
