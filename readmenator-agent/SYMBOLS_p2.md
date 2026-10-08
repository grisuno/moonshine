# Symbols (page 2 of 12)
Previous: [SYMBOLS.md](SYMBOLS.md)

| Symbol | Kind | File:Line | Signature |
|--------|------|-----------|-----------|
| `CppAnnote` | class | `core/cpp-annote/src/cpp-annote.h:33` | `` |
| `DiarizationResults` | struct | `core/cpp-annote/src/cpp-annote.h:22` | `` |
| `DiarizationTurn` | struct | `core/cpp-annote/src/cpp-annote.h:16` | `` |
| `Impl` | struct | `core/cpp-annote/src/cpp-annote.h:81` | `` |
| `add_audio_to_stream` | function | `core/cpp-annote/src/cpp-annote.h:73` | `void add_audio_to_stream(int32_t stream_id, const float *audio_data, uint64_t audio_length, int32_t sample_rate);` |
| `create_stream` | function | `core/cpp-annote/src/cpp-annote.h:58` | `int32_t create_stream(double cluster_cadence = 2.0, double analyze_cadence = 0.0);` |
| `free_stream` | function | `core/cpp-annote/src/cpp-annote.h:62` | `void free_stream(int32_t stream_id);` |
| `start_stream` | function | `core/cpp-annote/src/cpp-annote.h:65` | `void start_stream(int32_t stream_id);` |
| `write_json` | function | `core/cpp-annote/src/cpp-annote.h:25` | `void write_json(const std::string &path) const;` |
| `any_non_finite_embedding` | function | `core/cpp-annote/src/embedding_ort_infer.cpp:16` | `bool any_non_finite_embedding(const float* e, int dim)` |
| `discover_min_num_samples_embedding` | function | `core/cpp-annote/src/embedding_ort_infer.cpp:78` | `int discover_min_num_samples_embedding(Ort::Session& sess, Ort::MemoryInfo& mem,                 ...` |
| `emb` | function | `core/cpp-annote/src/embedding_ort_infer.cpp:103` | `std::vector<float> emb(static_cast<size_t>(embed_dim));` |
| `embedding_json_inputs_fbank_first` | function | `core/cpp-annote/src/embedding_ort_infer.cpp:27` | `bool embedding_json_inputs_fbank_first(const std::string& emb_json)` |
| `fbank_num_frames_for_samples` | function | `core/cpp-annote/src/embedding_ort_infer.cpp:115` | `int fbank_num_frames_for_samples(int embed_sr, int mel_bins, float fl_ms,                        ...` |
| `noise` | function | `core/cpp-annote/src/embedding_ort_infer.cpp:87` | `std::vector<float> noise(static_cast<size_t>(middle));` |
| `run_embedding_ort` | function | `core/cpp-annote/src/embedding_ort_infer.cpp:40` | `void run_embedding_ort(Ort::Session& sess, Ort::MemoryInfo& mem,                        Ort::Allo...` |
| `seg_to_fbank_nearest_index` | function | `core/cpp-annote/src/embedding_ort_infer.cpp:130` | `int seg_to_fbank_nearest_index(int tf, int num_seg_frames,                                int num...` |
| `wts` | function | `core/cpp-annote/src/embedding_ort_infer.cpp:102` | `std::vector<float> wts(static_cast<size_t>(Tf), 1.f);` |
| `EMBEDDING_ORT_INFER_H_` | macro | `core/cpp-annote/src/embedding_ort_infer.h:6` | `#define EMBEDDING_ORT_INFER_H_` |
| `discover_min_num_samples_embedding` | function | `core/cpp-annote/src/embedding_ort_infer.h:22` | `int discover_min_num_samples_embedding(Ort::Session& sess, Ort::MemoryInfo& mem, Ort::AllocatorWithDefaultOptions&...` |
| `embedding_json_inputs_fbank_first` | function | `core/cpp-annote/src/embedding_ort_infer.h:14` | `bool embedding_json_inputs_fbank_first(const std::string& emb_json);` |
| `fbank_num_frames_for_samples` | function | `core/cpp-annote/src/embedding_ort_infer.h:28` | `int fbank_num_frames_for_samples(int embed_sr, int mel_bins, float fl_ms, float fs_ms, int num_samples);` |
| `run_embedding_ort` | function | `core/cpp-annote/src/embedding_ort_infer.h:16` | `void run_embedding_ort(Ort::Session& sess, Ort::MemoryInfo& mem, Ort::AllocatorWithDefaultOptions& alloc, bool...` |
| `seg_to_fbank_nearest_index` | function | `core/cpp-annote/src/embedding_ort_infer.h:31` | `int seg_to_fbank_nearest_index(int tf, int num_seg_frames, int num_fbank_frames);` |
| `filter_embeddings_train` | function | `core/cpp-annote/src/filter_train.cpp:10` | `void filter_embeddings_train(int num_chunks, int num_frames, int num_speakers,                   ...` |
| `FILTER_TRAIN_H_` | macro | `core/cpp-annote/src/filter_train.h:5` | `#define FILTER_TRAIN_H_` |
| `filter_embeddings_train` | function | `core/cpp-annote/src/filter_train.h:15` | `void filter_embeddings_train(int num_chunks, int num_frames, int num_speakers, int dim, const float* embeddings...` |
| `HUNGARIAN_H_` | macro | `core/cpp-annote/src/hungarian.h:6` | `#define HUNGARIAN_H_` |
| `assignment` | function | `core/cpp-annote/src/hungarian.h:75` | `std::vector<int> assignment(static_cast<std::size_t>(n), -1);` |
| `minv` | function | `core/cpp-annote/src/hungarian.h:36` | `std::vector<double> minv(big_m, inf);` |
| `p` | function | `core/cpp-annote/src/hungarian.h:31` | `std::vector<int> p(big_m, 0);` |
| `u` | function | `core/cpp-annote/src/hungarian.h:29` | `std::vector<double> u(big_n, 0.0);` |
| `used` | function | `core/cpp-annote/src/hungarian.h:37` | `std::vector<char> used(big_m, 0);` |
| `v` | function | `core/cpp-annote/src/hungarian.h:30` | `std::vector<double> v(big_m, 0.0);` |
| `way` | function | `core/cpp-annote/src/hungarian.h:32` | `std::vector<int> way(big_m, 0);` |
| `ensure_parity_out_dir` | function | `core/cpp-annote/src/parity_log.cpp:51` | `void ensure_parity_out_dir()` |
| `env_parity_level` | function | `core/cpp-annote/src/parity_log.cpp:19` | `int env_parity_level()` |
| `env_parity_out_dir` | function | `core/cpp-annote/src/parity_log.cpp:33` | `const char* env_parity_out_dir()` |
| `fingerprint_float32` | function | `core/cpp-annote/src/parity_log.cpp:74` | `std::string fingerprint_float32(const float* data, std::size_t n,                                ...` |
| `heavy_dumps_enabled` | function | `core/cpp-annote/src/parity_log.cpp:47` | `bool heavy_dumps_enabled()` |
| `log_light` | function | `core/cpp-annote/src/parity_log.cpp:41` | `void log_light(const std::string& line)` |
| `parity_clustering_npz_path` | function | `core/cpp-annote/src/parity_log.cpp:64` | `std::string parity_clustering_npz_path()` |
| `PARITY_LOG_H_` | macro | `core/cpp-annote/src/parity_log.h:6` | `#define PARITY_LOG_H_` |
| `ensure_parity_out_dir` | function | `core/cpp-annote/src/parity_log.h:29` | `void ensure_parity_out_dir();` |
| `env_parity_level` | function | `core/cpp-annote/src/parity_log.h:16` | `int env_parity_level();` |
| `env_parity_out_dir` | function | `core/cpp-annote/src/parity_log.h:20` | `const char* env_parity_out_dir();` |
| `heavy_dumps_enabled` | function | `core/cpp-annote/src/parity_log.h:26` | `bool heavy_dumps_enabled();` |
| `log_light` | function | `core/cpp-annote/src/parity_log.h:23` | `void log_light(const std::string& line);` |
| `align_eigen_evecs_to_scipy_wccn_row0_for_community1_plda` | function | `core/cpp-annote/src/plda_vbx.cpp:67` | `void align_eigen_evecs_to_scipy_wccn_row0_for_community1_plda(     const RowMatrixXd& tr_file, Ei...` |
| `cluster_vbx` | function | `core/cpp-annote/src/plda_vbx.cpp:299` | `void cluster_vbx(const std::vector<int>& ahc_init, const Eigen::MatrixXd& fea,                  c...` |
| `load` | function | `core/cpp-annote/src/plda_vbx.cpp:161` | `void PldaModel::load(const std::string& xvec_transform_npz,                      const std::strin...` |
| `load_from_arrays` | function | `core/cpp-annote/src/plda_vbx.cpp:118` | `void PldaModel::load_from_arrays(const double* mean1_p, int n_mean1,                             ...` |
| `logsumexp_rowwise` | function | `core/cpp-annote/src/plda_vbx.cpp:97` | `void logsumexp_rowwise(const Eigen::MatrixXd& M, Eigen::VectorXd& lse,                        Eig...` |
| `operator` | function | `core/cpp-annote/src/plda_vbx.cpp:282` | `Eigen::MatrixXd PldaModel::operator()(const Eigen::MatrixXd& embeddings) const` |
| `plda_tf` | function | `core/cpp-annote/src/plda_vbx.cpp:272` | `Eigen::MatrixXd PldaModel::plda_tf(const Eigen::MatrixXd& x0,                                    ...` |
| `row_l2_normalize` | function | `core/cpp-annote/src/plda_vbx.cpp:88` | `void row_l2_normalize(Eigen::MatrixXd& M)` |
| `softmax_rows` | function | `core/cpp-annote/src/plda_vbx.cpp:286` | `void softmax_rows(const Eigen::MatrixXd& logits, Eigen::MatrixXd& out)` |
| `xvec_tf` | function | `core/cpp-annote/src/plda_vbx.cpp:257` | `Eigen::MatrixXd PldaModel::xvec_tf(const Eigen::MatrixXd& embeddings) const` |
| `PLDA_VBX_H_` | macro | `core/cpp-annote/src/plda_vbx.h:5` | `#define PLDA_VBX_H_` |
| `PldaModel` | struct | `core/cpp-annote/src/plda_vbx.h:16` | `` |
| `cluster_vbx` | function | `core/cpp-annote/src/plda_vbx.h:52` | `void cluster_vbx(const std::vector<int>& ahc_init, const Eigen::MatrixXd& fea, const Eigen::VectorXd& Phi, double...` |
| `load_from_arrays` | function | `core/cpp-annote/src/plda_vbx.h:34` | `void load_from_arrays(const double* mean1, int n_mean1, const float* mean2, int n_mean2, const float* lda, int...` |
| `softmax_rows` | function | `core/cpp-annote/src/plda_vbx.h:44` | `void softmax_rows(const Eigen::MatrixXd& logits, Eigen::MatrixXd& out);` |
| `centroid_update` | function | `core/cpp-annote/src/scipy_linkage.cpp:16` | `inline double centroid_update(double d_xi, double d_yi, double d_xy, int size_x,                 ...` |
| `cluster_monocrit` | function | `core/cpp-annote/src/scipy_linkage.cpp:93` | `void cluster_monocrit(const double* Z, int n, const std::vector<double>& MC,                     ...` |
| `curr_node` | function | `core/cpp-annote/src/scipy_linkage.cpp:49` | `std::vector<int> curr_node(static_cast<std::size_t>(n));` |
| `fcluster_distance` | function | `core/cpp-annote/src/scipy_linkage.cpp:237` | `void fcluster_distance(const std::vector<double>& Z, int n, double cutoff,                       ...` |
| `get_max_dist_for_each_cluster` | function | `core/cpp-annote/src/scipy_linkage.cpp:46` | `void get_max_dist_for_each_cluster(const double* Z, int n,                                    std...` |
| `id_map` | function | `core/cpp-annote/src/scipy_linkage.cpp:173` | `std::vector<int> id_map(static_cast<std::size_t>(n));` |
| `is_visited` | function | `core/cpp-annote/src/scipy_linkage.cpp:34` | `inline bool is_visited(const std::vector<unsigned char>& bitset, int i)` |
| `linkage_centroid_naive` | function | `core/cpp-annote/src/scipy_linkage.cpp:169` | `void linkage_centroid_naive(const std::vector<double>& dist, int n,                             s...` |
| `pdist_euclidean` | function | `core/cpp-annote/src/scipy_linkage.cpp:151` | `void pdist_euclidean(const std::vector<double>& X, int n, int d,                      std::vector...` |
| `remap_labels_contiguous` | function | `core/cpp-annote/src/scipy_linkage.cpp:244` | `void remap_labels_contiguous(const std::vector<int>& labels_one_based,                           ...` |
| `set_visited` | function | `core/cpp-annote/src/scipy_linkage.cpp:39` | `inline void set_visited(std::vector<unsigned char>& bitset, int i)` |
| `visited` | function | `core/cpp-annote/src/scipy_linkage.cpp:50` | `std::vector<unsigned char> visited(static_cast<std::size_t>(visited_bytes(n)), 0);` |
| `visited_bytes` | function | `core/cpp-annote/src/scipy_linkage.cpp:44` | `inline int visited_bytes(int n)` |
| `z` | function | `core/cpp-annote/src/scipy_linkage.cpp:247` | `std::vector<int> z(static_cast<std::size_t>(n));` |
| `SCIPY_LINKAGE_H_` | macro | `core/cpp-annote/src/scipy_linkage.h:6` | `#define SCIPY_LINKAGE_H_` |
| `condensed_index` | function | `core/cpp-annote/src/scipy_linkage.h:14` | `inline std::size_t condensed_index(int n, int i, int j)` |
| `fcluster_distance` | function | `core/cpp-annote/src/scipy_linkage.h:35` | `void fcluster_distance(const std::vector<double>& Z, int n, double cutoff, std::vector<int>& T);` |
| `linkage_centroid_naive` | function | `core/cpp-annote/src/scipy_linkage.h:29` | `void linkage_centroid_naive(const std::vector<double>& dist, int n, std::vector<double>& Z);` |
| `pdist_euclidean` | function | `core/cpp-annote/src/scipy_linkage.h:23` | `void pdist_euclidean(const std::vector<double>& X, int n, int d, std::vector<double>& dist);` |
| `remap_labels_contiguous` | function | `core/cpp-annote/src/scipy_linkage.h:39` | `void remap_labels_contiguous(const std::vector<int>& labels_one_based, std::vector<int>& out);` |
| `WAV_PCM_FLOAT32_H_` | macro | `core/cpp-annote/src/wav_pcm_float32.h:6` | `#define WAV_PCM_FLOAT32_H_` |
| `buf` | function | `core/cpp-annote/src/wav_pcm_float32.h:29` | `std::vector<std::uint8_t> buf(static_cast<size_t>(sz));` |
| `linear_resample` | function | `core/cpp-annote/src/wav_pcm_float32.h:120` | `inline std::vector<float> linear_resample(const std::vector<float>& x,                           ...` |
| `load_wav_pcm16_mono_float32` | function | `core/cpp-annote/src/wav_pcm_float32.h:51` | `inline std::vector<float> load_wav_pcm16_mono_float32(const std::string& path,                   ...` |
| `mono` | function | `core/cpp-annote/src/wav_pcm_float32.h:104` | `std::vector<float> mono(num_frames);` |
| `read_file_bytes` | function | `core/cpp-annote/src/wav_pcm_float32.h:18` | `inline std::vector<std::uint8_t> read_file_bytes(const std::string& path)` |
| `u16` | function | `core/cpp-annote/src/wav_pcm_float32.h:44` | `inline std::uint16_t u16(const std::uint8_t* p)` |
| `u32` | function | `core/cpp-annote/src/wav_pcm_float32.h:37` | `inline std::uint32_t u32(const std::uint8_t* p)` |
| `y` | function | `core/cpp-annote/src/wav_pcm_float32.h:132` | `std::vector<float> y(n_out);` |
| `EMBEDDING_MODEL_H` | macro | `core/embedding-model.h:2` | `#define EMBEDDING_MODEL_H` |
| `EmbeddingModel` | class | `core/embedding-model.h:12` | `` |
| `cosine_similarity` | function | `core/embedding-model.h:65` | `float cosine_similarity(const std::vector<float> &a,                           const std::vector<...` |
| `get_similarity` | function | `core/embedding-model.h:29` | `float get_similarity(const std::string &a, const std::string &b)` |
| `get_similarity` | function | `core/embedding-model.h:41` | `float get_similarity(const std::string &text,                        const std::vector<float> &em...` |
| `get_similarity` | function | `core/embedding-model.h:53` | `float get_similarity(const std::vector<float> &embedding_a,                        const std::vec...` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/gemma-embedding-model-test.cpp:7` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `SUBCASE` | function | `core/gemma-embedding-model-test.cpp:18` | `SUBCASE("load model")` |
| `SUBCASE` | function | `core/gemma-embedding-model-test.cpp:26` | `SUBCASE("get embeddings")` |
| `SUBCASE` | function | `core/gemma-embedding-model-test.cpp:46` | `SUBCASE("identical strings have similarity 1.0")` |
| `SUBCASE` | function | `core/gemma-embedding-model-test.cpp:55` | `SUBCASE("similar strings have high similarity")` |
| `SUBCASE` | function | `core/gemma-embedding-model-test.cpp:67` | `SUBCASE("different strings have lower similarity")` |
| `SUBCASE` | function | `core/gemma-embedding-model-test.cpp:79` | `SUBCASE("query and document embeddings")` |
| `SUBCASE` | function | `core/gemma-embedding-model-test.cpp:99` | `SUBCASE("truncate embedding with MRL")` |
| `SUBCASE` | function | `core/gemma-embedding-model-test.cpp:126` | `SUBCASE("config values")` |
| `SUBCASE` | function | `core/gemma-embedding-model-test.cpp:139` | `SUBCASE("load nonexistent model")` |
| `SUBCASE` | function | `core/gemma-embedding-model-test.cpp:146` | `SUBCASE("get embeddings without loading")` |
| `SUBCASE` | function | `core/gemma-embedding-model-test.cpp:152` | `SUBCASE("load invalid variant")` |
| `TEST_CASE` | function | `core/gemma-embedding-model-test.cpp:10` | `TEST_CASE("gemma-embedding-model")` |
| `TEST_CASE` | function | `core/gemma-embedding-model-test.cpp:138` | `TEST_CASE("gemma-embedding-model error handling")` |
| `DEBUG_ALLOC_ENABLED` | macro | `core/gemma-embedding-model.cpp:17` | `#define DEBUG_ALLOC_ENABLED` |
| `GemmaEmbeddingModel` | function | `core/gemma-embedding-model.cpp:21` | `GemmaEmbeddingModel::GemmaEmbeddingModel()     : ort_api_(nullptr),       ort_env_(nullptr),     ...` |
| `attention_mask` | function | `core/gemma-embedding-model.cpp:309` | `std::vector<int64_t> attention_mask(input_ids.size(), 1);` |
| `embedding` | function | `core/gemma-embedding-model.cpp:288` | `std::vector<float> embedding(output_data, output_data + output_size);` |
| `get_config` | function | `core/gemma-embedding-model.cpp:364` | `const GemmaEmbeddingConfig &GemmaEmbeddingModel::get_config() const` |
| `get_document_embeddings` | function | `core/gemma-embedding-model.cpp:325` | `std::vector<float> GemmaEmbeddingModel::get_document_embeddings(     const std::string &document)` |
| `get_embeddings` | function | `core/gemma-embedding-model.cpp:298` | `std::vector<float> GemmaEmbeddingModel::get_embeddings(     const std::string &text)` |
| `get_embeddings_with_prefix` | function | `core/gemma-embedding-model.cpp:315` | `std::vector<float> GemmaEmbeddingModel::get_embeddings_with_prefix(     const std::string &text, ...` |
| `get_query_embeddings` | function | `core/gemma-embedding-model.cpp:320` | `std::vector<float> GemmaEmbeddingModel::get_query_embeddings(     const std::string &query)` |
| `is_loaded` | function | `core/gemma-embedding-model.cpp:362` | `bool GemmaEmbeddingModel::is_loaded() const` |
| `load` | function | `core/gemma-embedding-model.cpp:67` | `int GemmaEmbeddingModel::load(const char *model_dir,                               const char *mo...` |
| `load_from_memory` | function | `core/gemma-embedding-model.cpp:111` | `int GemmaEmbeddingModel::load_from_memory(const uint8_t *model_data,                             ...` |
| `load_tokenizer` | function | `core/gemma-embedding-model.cpp:131` | `int GemmaEmbeddingModel::load_tokenizer(const char *tokenizer_path)` |
| `load_tokenizer_from_memory` | function | `core/gemma-embedding-model.cpp:142` | `int GemmaEmbeddingModel::load_tokenizer_from_memory(const uint8_t *data,                         ...` |
| `normalize_embedding` | function | `core/gemma-embedding-model.cpp:346` | `void GemmaEmbeddingModel::normalize_embedding(std::vector<float> &embedding)` |
| `output_shape` | function | `core/gemma-embedding-model.cpp:263` | `std::vector<int64_t> output_shape(num_dims);` |
| `run_inference` | function | `core/gemma-embedding-model.cpp:186` | `std::vector<float> GemmaEmbeddingModel::run_inference(     const std::vector<int64_t> &input_ids,...` |
| `tokenize` | function | `core/gemma-embedding-model.cpp:161` | `std::vector<int64_t> GemmaEmbeddingModel::tokenize(const std::string &text)` |
| `truncate_embedding` | function | `core/gemma-embedding-model.cpp:330` | `std::vector<float> GemmaEmbeddingModel::truncate_embedding(     const std::vector<float> &embeddi...` |
| `truncated` | function | `core/gemma-embedding-model.cpp:337` | `std::vector<float> truncated(embedding.begin(), embedding.begin() + target_dim);` |
| `GEMMA_EMBEDDING_MODEL_H` | macro | `core/gemma-embedding-model.h:2` | `#define GEMMA_EMBEDDING_MODEL_H` |
| `GemmaEmbeddingConfig` | struct | `core/gemma-embedding-model.h:17` | `` |
| `GemmaEmbeddingModel` | class | `core/gemma-embedding-model.h:31` | `` |
| `embeddings` | function | `core/gemma-embedding-model.h:83` | `* Get query embeddings (uses query prefix). * @param query The query text. * @return A vector of floats representing...` |
| `get_config` | function | `core/gemma-embedding-model.h:115` | `const GemmaEmbeddingConfig &get_config() const;` |
| `is_loaded` | function | `core/gemma-embedding-model.h:109` | `bool is_loaded() const;` |
| `load` | function | `core/gemma-embedding-model.h:51` | `int load(const char *model_dir, const char *model_variant = "q4");` |
| `load_from_memory` | function | `core/gemma-embedding-model.h:61` | `int load_from_memory(const uint8_t *model_data, size_t model_data_size, const uint8_t *tokenizer_data, size_t...` |
| `load_tokenizer` | function | `core/gemma-embedding-model.h:148` | `int load_tokenizer(const char *tokenizer_path);` |
| `load_tokenizer_from_memory` | function | `core/gemma-embedding-model.h:156` | `int load_tokenizer_from_memory(const uint8_t *data, size_t data_size);` |
| `normalize_embedding` | function | `core/gemma-embedding-model.h:178` | `static void normalize_embedding(std::vector<float> &embedding);` |
| `prefix` | function | `core/gemma-embedding-model.h:73` | `* Get embeddings with a specific prefix (for query vs document embeddings). * @param text The input text to embed. *...` |
| `run_inference` | function | `core/gemma-embedding-model.h:171` | `std::vector<float> run_inference(const std::vector<int64_t> &input_ids, const std::vector<int64_t> &attention_mask);` |
| `tokenize` | function | `core/gemma-embedding-model.h:163` | `std::vector<int64_t> tokenize(const std::string &text);` |
| `truncate_embedding` | function | `core/gemma-embedding-model.h:102` | `static std::vector<float> truncate_embedding( const std::vector<float> &embedding, int target_dim);` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/intent-recognizer-test.cpp:13` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `DiscriminationTest` | struct | `core/intent-recognizer-test.cpp:284` | `` |
| `IntentTestCase` | struct | `core/intent-recognizer-test.cpp:111` | `` |
| `PrecisionRecallResult` | struct | `core/intent-recognizer-test.cpp:116` | `` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:40` | `SUBCASE("register and count intents")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:50` | `SUBCASE("unregister intent")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:59` | `SUBCASE("unregister nonexistent intent")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:64` | `SUBCASE("clear intents")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:73` | `SUBCASE("rank_intents returns empty for empty utterance")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:78` | `SUBCASE("rank_intents sorts by similarity descending and respects max")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:96` | `SUBCASE("rank_intents with max_results limit")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:174` | `SUBCASE("basic intent matching")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:188` | `SUBCASE("precision/recall evaluation")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:283` | `SUBCASE("intent discrimination")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:326` | `SUBCASE("similarity scores for exact matches")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:356` | `SUBCASE("register with NULL embedding auto-computes")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:366` | `SUBCASE("register with pre-computed embedding")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:380` | `SUBCASE("update existing intent preserves count")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:398` | `SUBCASE("higher priority intent ranks first regardless of similarity")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:408` | `SUBCASE("equal priority falls back to similarity ordering")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:428` | `SUBCASE("returns non-empty embedding")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:434` | `SUBCASE("get_embedding_size returns correct dimension")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:441` | `SUBCASE("same text produces same embedding")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:463` | `SUBCASE("register with NULL embedding succeeds")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:469` | `SUBCASE("register with nullptr canonical_phrase fails")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:474` | `SUBCASE("register multiple intents with different priorities")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:482` | `SUBCASE("unregister and clear work")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:509` | `SUBCASE("basic embedding calculation")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:529` | `SUBCASE("null sentence returns error")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:537` | `SUBCASE("null out_embedding returns error")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:544` | `SUBCASE("null out_embedding_size returns error")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:551` | `SUBCASE("invalid handle returns error")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:559` | `SUBCASE("round-trip: compute embedding then register with it")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:590` | `SUBCASE("safe on nullptr")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:592` | `SUBCASE("frees malloc-allocated buffer")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:611` | `SUBCASE("identical embeddings have similarity ~1.0")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:627` | `SUBCASE("similar sentences have high similarity")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:648` | `SUBCASE("dissimilar sentences have low similarity")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:669` | `SUBCASE("null embedding_a returns error")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:677` | `SUBCASE("null embedding_b returns error")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:685` | `SUBCASE("null out_similarity returns error")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:692` | `SUBCASE("zero embedding_size returns error")` |
| `SUBCASE` | function | `core/intent-recognizer-test.cpp:700` | `SUBCASE("invalid handle returns error")` |
| `TEST_CASE` | function | `core/intent-recognizer-test.cpp:31` | `TEST_CASE("intent-recognizer unit tests")` |
| `TEST_CASE` | function | `core/intent-recognizer-test.cpp:147` | `TEST_CASE("intent-recognizer precision/recall with GemmaEmbeddingModel")` |
| `TEST_CASE` | function | `core/intent-recognizer-test.cpp:347` | `TEST_CASE("intent-recognizer register with pre-computed embedding")` |
| `TEST_CASE` | function | `core/intent-recognizer-test.cpp:389` | `TEST_CASE("intent-recognizer priority ranking")` |
| `TEST_CASE` | function | `core/intent-recognizer-test.cpp:419` | `TEST_CASE("intent-recognizer calculate_embedding")` |
| `TEST_CASE` | function | `core/intent-recognizer-test.cpp:451` | `TEST_CASE("C API intent registration with embedding and priority")` |
| `TEST_CASE` | function | `core/intent-recognizer-test.cpp:497` | `TEST_CASE("C API moonshine_calculate_intent_embedding")` |
| `TEST_CASE` | function | `core/intent-recognizer-test.cpp:589` | `TEST_CASE("C API moonshine_free_intent_embedding")` |
| `TEST_CASE` | function | `core/intent-recognizer-test.cpp:599` | `TEST_CASE("C API moonshine_calculate_embedding_distance")` |
| `TEST_CASE` | function | `core/intent-recognizer-test.cpp:711` | `TEST_CASE("C API moonshine_get_closest_intents with priority")` |
| `accuracy` | function | `core/intent-recognizer-test.cpp:138` | `float accuracy() const` |
| `embedding_model_available` | function | `core/intent-recognizer-test.cpp:27` | `bool embedding_model_available()` |
| `f1_score` | function | `core/intent-recognizer-test.cpp:132` | `float f1_score() const` |
| `make_options` | function | `core/intent-recognizer-test.cpp:19` | `IntentRecognizerOptions make_options()` |
| `precision` | function | `core/intent-recognizer-test.cpp:122` | `float precision() const` |
| `recall` | function | `core/intent-recognizer-test.cpp:127` | `float recall() const` |
| `IntentRecognizer` | function | `core/intent-recognizer.cpp:31` | `IntentRecognizer::IntentRecognizer(const IntentRecognizerOptions &options)     : embedding_model_...` |
| `RankedEntry` | struct | `core/intent-recognizer.cpp:86` | `` |
| `calculate_embedding` | function | `core/intent-recognizer.cpp:140` | `std::vector<float> IntentRecognizer::calculate_embedding(     const std::string &sentence) const` |
| `calculate_similarity` | function | `core/intent-recognizer.cpp:146` | `float IntentRecognizer::calculate_similarity(     const std::vector<float> &a, const std::vector<...` |
| `clear_intents` | function | `core/intent-recognizer.cpp:135` | `void IntentRecognizer::clear_intents()` |
| `create_embedding_model` | function | `core/intent-recognizer.cpp:11` | `std::unique_ptr<EmbeddingModel> create_embedding_model(     const IntentRecognizerOptions &options)` |
| `get_embedding_size` | function | `core/intent-recognizer.cpp:152` | `size_t IntentRecognizer::get_embedding_size() const` |
| `get_intent_count` | function | `core/intent-recognizer.cpp:130` | `size_t IntentRecognizer::get_intent_count() const` |
| `register_intent` | function | `core/intent-recognizer.cpp:36` | `void IntentRecognizer::register_intent(const std::string &trigger_phrase)` |
| `register_intent` | function | `core/intent-recognizer.cpp:40` | `void IntentRecognizer::register_intent(const std::string &trigger_phrase,                        ...` |
| `sort` | function | `core/intent-recognizer.cpp:115` | `std::sort(entries.begin(), entries.end(), [](const auto &a, const auto &b)` |
| `unregister_intent` | function | `core/intent-recognizer.cpp:68` | `bool IntentRecognizer::unregister_intent(const std::string &trigger_phrase)` |
| `EmbeddingModelArch` | enum | `core/intent-recognizer.h:16` | `` |
| `EmbeddingModelArch` | class | `core/intent-recognizer.h:16` | `` |
| `INTENT_RECOGNIZER_H` | macro | `core/intent-recognizer.h:2` | `#define INTENT_RECOGNIZER_H` |
| `Intent` | struct | `core/intent-recognizer.h:37` | `` |
| `IntentRecognizer` | class | `core/intent-recognizer.h:48` | `` |
| `IntentRecognizerOptions` | struct | `core/intent-recognizer.h:23` | `` |
| `calculate_embedding` | function | `core/intent-recognizer.h:115` | `std::vector<float> calculate_embedding(const std::string &sentence) const;` |
| `calculate_similarity` | function | `core/intent-recognizer.h:123` | `float calculate_similarity(const std::vector<float> &a, const std::vector<float> &b) const;` |
| `clear_intents` | function | `core/intent-recognizer.h:108` | `void clear_intents();` |
| `get_embedding_size` | function | `core/intent-recognizer.h:130` | `size_t get_embedding_size() const;` |
| `get_intent_count` | function | `core/intent-recognizer.h:103` | `size_t get_intent_count() const;` |
| `register_intent` | function | `core/intent-recognizer.h:66` | `void register_intent(const std::string &trigger_phrase);` |
| `unregister_intent` | function | `core/intent-recognizer.h:86` | `bool unregister_intent(const std::string &trigger_phrase);` |
| `DOCTEST_CONFIG_IMPLEMENT` | macro | `core/moonshine-c-api-memory-test.cpp:6` | `#define DOCTEST_CONFIG_IMPLEMENT` |
| `append_files_under` | function | `core/moonshine-c-api-memory-test.cpp:110` | `void append_files_under(     const std::filesystem::path& root, const std::filesystem::path& sub,...` |
| `build_kokoro_g2p_memory_bundle` | function | `core/moonshine-c-api-memory-test.cpp:140` | `void build_kokoro_g2p_memory_bundle(     const std::filesystem::path& data_root,     std::vector<...` |
| `kokoro_lang_for_voice_stem` | function | `core/moonshine-c-api-memory-test.cpp:44` | `const char* kokoro_lang_for_voice_stem(std::string_view stem)` |
| `main` | function | `core/moonshine-c-api-memory-test.cpp:266` | `int main(int argc, char** argv)` |
| `read_binary_file` | function | `core/moonshine-c-api-memory-test.cpp:34` | `std::vector<uint8_t> read_binary_file(const std::filesystem::path& p)` |
| `sample_text_for_kokoro_lang` | function | `core/moonshine-c-api-memory-test.cpp:79` | `const char* sample_text_for_kokoro_lang(const char* lang)` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-c-api-test.cpp:17` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `GraphemePhonemizerLangCase` | struct | `core/moonshine-c-api-test.cpp:100` | `` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:111` | `SUBCASE("transcribe-complete")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:154` | `SUBCASE("transcribe-stream")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:247` | `SUBCASE("transcribe-complete-from-memory")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:313` | `SUBCASE("transcribe-without-streaming-skip-transcription")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:357` | `SUBCASE("transcribe-without-streaming-vad-threshold-0")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:407` | `SUBCASE("transcribe-valid-options")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:438` | `SUBCASE("transcribe-invalid-option")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:451` | `SUBCASE("spelling-mode-flag-noop-without-model")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:478` | `SUBCASE("spelling-mode-replaces-line-text")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:524` | `SUBCASE("tts-synthesizer-valid-options")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:548` | `SUBCASE("tts-synthesizer-per-call-speed-kokoro")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:597` | `SUBCASE("tts-piper-german-from-memory")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:658` | `SUBCASE("invalid-handle")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:667` | `SUBCASE("invalid-arguments")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:696` | `SUBCASE("kokoro-matches-text-to-speech")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:785` | `SUBCASE("create-invalid-filenames-pointer")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:795` | `SUBCASE("text-to-phonemes-invalid-handle")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:802` | `SUBCASE("text-to-phonemes-invalid-arguments")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:829` | `SUBCASE("rule-based-languages-smoke")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:868` | `SUBCASE("chinese-when-onnx-bundle-present")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:885` | `SUBCASE("japanese-when-onnx-bundle-present")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:904` | `SUBCASE("arabic-when-onnx-bundle-present")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:924` | `SUBCASE("null-output-pointer")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:933` | `SUBCASE("options-count-without-options-pointer")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:943` | `SUBCASE("g2p-empty-means-all-languages")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:961` | `SUBCASE("g2p-arabic-onnx-model-key-matches-meta-onnx-filename")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:974` | `SUBCASE("g2p-french-lists-pos-csv-files-not-directory-prefix")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:988` | `SUBCASE("g2p-single-language")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:997` | `SUBCASE("g2p-unsupported-language")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1005` | `SUBCASE("g2p-multiple-languages")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1017` | `SUBCASE("g2p-appends-override-key-when-option-set")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1029` | `SUBCASE("tts-json-single-language")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1044` | `SUBCASE("tts-empty-all-languages-json")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1055` | `SUBCASE("tts-unsupported-language")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1063` | `SUBCASE("tts-multiple-languages")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1076` | `SUBCASE("tts-piper-engine-on-en_us")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1090` | `SUBCASE("tts-kokoro-engine-on-fr")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1104` | `SUBCASE("tts-explicit-piper-onnx-map-keys")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1119` | `SUBCASE("tts-piper-voice-selects-onnx-basename")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1132` | `SUBCASE("tts-voices-json-object-en_us")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1155` | `SUBCASE("tts-voices-kokoro-reports-missing-without-assets")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1169` | `SUBCASE("tts-voices-unsupported-language")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1176` | `SUBCASE("tts-voices-piper-de-includes-thorsten-stem")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1196` | `SUBCASE("tts-voices-piper-en_us-includes-saikat-stem")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1216` | `SUBCASE("tts-zipvoice-dependencies")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1234` | `SUBCASE("tts-zipvoice-voices-listing")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1254` | `SUBCASE("null-output-pointer")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1262` | `SUBCASE("options-count-without-options-pointer")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1271` | `SUBCASE("stt-empty-language-is-invalid")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1278` | `SUBCASE("stt-english-default-is-medium-streaming")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1296` | `SUBCASE("stt-english-tiny-non-streaming")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1317` | `SUBCASE("stt-non-english-omits-attention-extra")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1334` | `SUBCASE("stt-english-name-lookup")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1342` | `SUBCASE("stt-include-spelling-adds-group-for-english")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1359` | `SUBCASE("stt-include-spelling-noop-for-non-english")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1373` | `SUBCASE("stt-unknown-language")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1381` | `SUBCASE("stt-unknown-arch-for-language")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1391` | `SUBCASE("stt-invalid-arch-value")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1401` | `SUBCASE("intent-default-variant-is-q4")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1415` | `SUBCASE("intent-null-model-name-uses-default")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1424` | `SUBCASE("intent-q8-maps-to-model-quantized")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1441` | `SUBCASE("intent-fp32-uses-bare-model-onnx")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1455` | `SUBCASE("intent-unknown-model")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1462` | `SUBCASE("intent-unknown-variant")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1498` | `SUBCASE("builtin-voice-synthesizes-audio")` |
| `SUBCASE` | function | `core/moonshine-c-api-test.cpp:1522` | `SUBCASE("user-pcm-with-explicit-transcript")` |
| `TEST_CASE` | function | `core/moonshine-c-api-test.cpp:110` | `TEST_CASE("moonshine-test-v2")` |
| `TEST_CASE` | function | `core/moonshine-c-api-test.cpp:657` | `TEST_CASE("moonshine-phonemes-to-speech-c-api")` |
| `TEST_CASE` | function | `core/moonshine-c-api-test.cpp:784` | `TEST_CASE("grapheme-to-phonemizer-c-api")` |
| `TEST_CASE` | function | `core/moonshine-c-api-test.cpp:923` | `TEST_CASE("moonshine-tts-g2p-dependency-api")` |
| `TEST_CASE` | function | `core/moonshine-c-api-test.cpp:1253` | `TEST_CASE("moonshine-stt-intent-dependency-api")` |
| `csv` | function | `core/moonshine-c-api-test.cpp:948` | `const std::string csv(out);` |
| `find_de_piper_voices_dir` | function | `core/moonshine-c-api-test.cpp:22` | `std::filesystem::path find_de_piper_voices_dir()` |
| `find_moonshine_tts_data_dir` | function | `core/moonshine-c-api-test.cpp:48` | `std::optional<std::filesystem::path> find_moonshine_tts_data_dir()` |
| `free_phonemes_output` | function | `core/moonshine-c-api-test.cpp:72` | `void free_phonemes_output(const char* ipa)` |
| `grapheme_phonemizer_smoke` | function | `core/moonshine-c-api-test.cpp:78` | `void grapheme_phonemizer_smoke(const std::filesystem::path& data_root,                           ...` |
| `json` | function | `core/moonshine-c-api-test.cpp:1034` | `const std::string json(out);` |
| `pcm` | function | `core/moonshine-c-api-test.cpp:1525` | `std::vector<float> pcm(24000, 0.f);` |
| `read_binary_file` | function | `core/moonshine-c-api-test.cpp:37` | `std::vector<uint8_t> read_binary_file(const std::filesystem::path& p)` |
| `CHECK_GRAPHEME_PHONEMIZER_HANDLE` | macro | `core/moonshine-c-api.cpp:1853` | `#define CHECK_GRAPHEME_PHONEMIZER_HANDLE(g2p_handle)` |
| `CHECK_INTENT_RECOGNIZER_HANDLE` | macro | `core/moonshine-c-api.cpp:462` | `#define CHECK_INTENT_RECOGNIZER_HANDLE(handle)` |
| `CHECK_TRANSCRIBER_HANDLE` | macro | `core/moonshine-c-api.cpp:70` | `#define CHECK_TRANSCRIBER_HANDLE(handle)` |
| `CHECK_TTS_SYNTHESIZER_HANDLE` | macro | `core/moonshine-c-api.cpp:857` | `#define CHECK_TTS_SYNTHESIZER_HANDLE(synth_handle)` |
| `OptionPair` | type_alias | `core/moonshine-c-api.cpp:79` | `typedef std::pair<std::string, std::string> OptionPair;` |
| `OptionVector` | type_alias | `core/moonshine-c-api.cpp:81` | `typedef std::vector<OptionPair> OptionVector;` |
| `a` | function | `core/moonshine-c-api.cpp:735` | `std::vector<float> a(embedding_a, embedding_a + embedding_size);` |
| `allocate_grapheme_phonemizer_handle` | function | `core/moonshine-c-api.cpp:1802` | `int32_t allocate_grapheme_phonemizer_handle(moonshine_tts::MoonshineG2P *g2p)` |
| `allocate_intent_recognizer_handle` | function | `core/moonshine-c-api.cpp:448` | `int32_t allocate_intent_recognizer_handle(IntentRecognizer *recognizer)` |
| `allocate_text_to_speech_synthesizer_handle` | function | `core/moonshine-c-api.cpp:755` | `int32_t allocate_text_to_speech_synthesizer_handle(     moonshine_tts::MoonshineTTS *synthesizer)` |
| `allocate_transcriber_handle` | function | `core/moonshine-c-api.cpp:171` | `int32_t allocate_transcriber_handle(Transcriber *transcriber)` |
| `append_g2p_explicit_override_keys_from_c_options` | function | `core/moonshine-c-api.cpp:1356` | `void append_g2p_explicit_override_keys_from_c_options(     const moonshine_option_t *options, uin...` |
| `append_unique_in_order` | function | `core/moonshine-c-api.cpp:1178` | `void append_unique_in_order(std::vector<std::string> &acc,                             const std:...` |
| `apply_g2p_dependency_query_c_options` | function | `core/moonshine-c-api.cpp:1306` | `void apply_g2p_dependency_query_c_options(     const moonshine_option_t *options, uint64_t option...` |
| `b` | function | `core/moonshine-c-api.cpp:736` | `std::vector<float> b(embedding_b, embedding_b + embedding_size);` |
| `duplicate_c_string` | function | `core/moonshine-c-api.cpp:471` | `char *duplicate_c_string(const char *s)` |
| `finalize_g2p_options_for_phonemizer_create` | function | `core/moonshine-c-api.cpp:1846` | `void finalize_g2p_options_for_phonemizer_create(     moonshine_tts::MoonshineG2POptions &g2p_opt)` |
| `free_intent_recognizer_handle` | function | `core/moonshine-c-api.cpp:455` | `void free_intent_recognizer_handle(int32_t handle)` |
| `free_transcriber_handle` | function | `core/moonshine-c-api.cpp:178` | `void free_transcriber_handle(int32_t handle)` |
| `json_flat_string_array` | function | `core/moonshine-c-api.cpp:1230` | `std::string json_flat_string_array(const std::vector<std::string> &items)` |
| `json_model_dependencies` | function | `core/moonshine-c-api.cpp:1247` | `std::string json_model_dependencies(const moonshine::ModelDependencies &deps)` |
| `json_tts_voice_entry` | function | `core/moonshine-c-api.cpp:1264` | `std::string json_tts_voice_entry(     const moonshine_tts::MoonshineTtsVoiceAvailability &v)` |
| `json_tts_voices_lang_array` | function | `core/moonshine-c-api.cpp:1274` | `std::string json_tts_voices_lang_array(     const std::vector<moonshine_tts::MoonshineTtsVoiceAva...` |
| `json_tts_voices_root_object` | function | `core/moonshine-c-api.cpp:1288` | `std::string json_tts_voices_root_object(     const std::vector<std::pair<         std::string, st...` |
| `json_utf8_string_literal` | function | `core/moonshine-c-api.cpp:1188` | `std::string json_utf8_string_literal(const std::string &s)` |
| `key` | function | `core/moonshine-c-api.cpp:946` | `const std::string key(filenames[i]);` |
| `malloc_string_copy` | function | `core/moonshine-c-api.cpp:1144` | `char *malloc_string_copy(const std::string &s)` |
| `maybe_autotranscribe_zipvoice_clone` | function | `core/moonshine-c-api.cpp:778` | `void maybe_autotranscribe_zipvoice_clone(     const OptionVector &options,     moonshine_tts::Moo...` |
| `moonshine_calculate_embedding_distance` | function | `core/moonshine-c-api.cpp:716` | `int32_t moonshine_calculate_embedding_distance(int32_t intent_recognizer_handle,                 ...` |
| `moonshine_calculate_intent_embedding` | function | `core/moonshine-c-api.cpp:673` | `int32_t moonshine_calculate_intent_embedding(int32_t intent_recognizer_handle,                   ...` |
| `moonshine_clear_intents` | function | `core/moonshine-c-api.cpp:659` | `int32_t moonshine_clear_intents(int32_t intent_recognizer_handle)` |
| `moonshine_create_grapheme_to_phonemizer_from_files` | function | `core/moonshine-c-api.cpp:1869` | `int32_t moonshine_create_grapheme_to_phonemizer_from_files(     const char *language, const char ...` |
| `moonshine_create_grapheme_to_phonemizer_from_memory` | function | `core/moonshine-c-api.cpp:1928` | `int32_t moonshine_create_grapheme_to_phonemizer_from_memory(     const char *language, const char...` |
| `moonshine_create_intent_recognizer` | function | `core/moonshine-c-api.cpp:485` | `int32_t moonshine_create_intent_recognizer(const char *model_path,                               ...` |
| `moonshine_create_stream` | function | `core/moonshine-c-api.cpp:322` | `int32_t moonshine_create_stream(int32_t transcriber_handle, uint32_t flags)` |
| `moonshine_create_tts_synthesizer_from_files` | function | `core/moonshine-c-api.cpp:870` | `int32_t moonshine_create_tts_synthesizer_from_files(     const char *language, const char **filen...` |
| `moonshine_create_tts_synthesizer_from_memory` | function | `core/moonshine-c-api.cpp:911` | `int32_t moonshine_create_tts_synthesizer_from_memory(     const char *language, const char **file...` |
| `moonshine_free_grapheme_to_phonemizer` | function | `core/moonshine-c-api.cpp:1995` | `void moonshine_free_grapheme_to_phonemizer(     int32_t grapheme_to_phonemizer_handle)` |
| `moonshine_free_intent_embedding` | function | `core/moonshine-c-api.cpp:714` | `void moonshine_free_intent_embedding(float *embedding)` |
| `moonshine_free_intent_matches` | function | `core/moonshine-c-api.cpp:636` | `void moonshine_free_intent_matches(moonshine_intent_match_t *matches,                            ...` |
| `moonshine_free_intent_recognizer` | function | `core/moonshine-c-api.cpp:516` | `void moonshine_free_intent_recognizer(int32_t intent_recognizer_handle)` |
| `moonshine_free_stream` | function | `core/moonshine-c-api.cpp:336` | `int32_t moonshine_free_stream(int32_t transcriber_handle,                               int32_t s...` |
| `moonshine_free_transcriber` | function | `core/moonshine-c-api.cpp:291` | `void moonshine_free_transcriber(int32_t transcriber_handle)` |
| `moonshine_free_tts_synthesizer` | function | `core/moonshine-c-api.cpp:1000` | `void moonshine_free_tts_synthesizer(int32_t tts_synthesizer_handle)` |
| `moonshine_get_closest_intents` | function | `core/moonshine-c-api.cpp:578` | `int32_t moonshine_get_closest_intents(int32_t intent_recognizer_handle,                          ...` |
| `moonshine_get_g2p_dependencies` | function | `core/moonshine-c-api.cpp:1387` | `int32_t moonshine_get_g2p_dependencies(const char *languages,                                    ...` |
| `moonshine_get_intent_count` | function | `core/moonshine-c-api.cpp:647` | `int32_t moonshine_get_intent_count(int32_t intent_recognizer_handle)` |
| `moonshine_get_intent_dependencies` | function | `core/moonshine-c-api.cpp:1743` | `int32_t moonshine_get_intent_dependencies(const char *model_name,                                ...` |
| `moonshine_get_stt_dependencies` | function | `core/moonshine-c-api.cpp:1681` | `int32_t moonshine_get_stt_dependencies(const char *language,                                     ...` |
| `moonshine_get_tts_dependencies` | function | `core/moonshine-c-api.cpp:1451` | `int32_t moonshine_get_tts_dependencies(const char *languages,                                    ...` |
| `moonshine_get_tts_voices` | function | `core/moonshine-c-api.cpp:1548` | `int32_t moonshine_get_tts_voices(const char *languages,                                  const mo...` |
| `moonshine_load_transcriber_from_memory` | function | `core/moonshine-c-api.cpp:240` | `int32_t moonshine_load_transcriber_from_memory(     const uint8_t *encoder_model_data, size_t enc...` |
| `moonshine_phonemes_to_speech` | function | `core/moonshine-c-api.cpp:1089` | `int32_t moonshine_phonemes_to_speech(int32_t tts_synthesizer_handle,                             ...` |
| `moonshine_register_intent` | function | `core/moonshine-c-api.cpp:527` | `int32_t moonshine_register_intent(int32_t intent_recognizer_handle,                              ...` |
| `moonshine_start_stream` | function | `core/moonshine-c-api.cpp:352` | `int32_t moonshine_start_stream(int32_t transcriber_handle,                                int32_t...` |
| `moonshine_stop_stream` | function | `core/moonshine-c-api.cpp:368` | `int32_t moonshine_stop_stream(int32_t transcriber_handle,                               int32_t s...` |
| `moonshine_text_to_phonemes` | function | `core/moonshine-c-api.cpp:2012` | `int32_t moonshine_text_to_phonemes(int32_t grapheme_to_phonemizer_handle,                        ...` |
| `moonshine_text_to_speech` | function | `core/moonshine-c-api.cpp:1041` | `int32_t moonshine_text_to_speech(int32_t tts_synthesizer_handle,                                 ...` |
| `moonshine_transcribe_add_audio_to_stream` | function | `core/moonshine-c-api.cpp:394` | `int32_t moonshine_transcribe_add_audio_to_stream(int32_t transcriber_handle,                     ...` |
| `moonshine_transcribe_stream` | function | `core/moonshine-c-api.cpp:420` | `int32_t moonshine_transcribe_stream(int32_t transcriber_handle,                                  ...` |
| `moonshine_transcribe_without_streaming` | function | `core/moonshine-c-api.cpp:299` | `int32_t moonshine_transcribe_without_streaming(     int32_t transcriber_handle, float *audio_data...` |
| `moonshine_transcript_to_string` | function | `core/moonshine-c-api.cpp:384` | `const char *moonshine_transcript_to_string(     const struct transcript_t *transcript)` |
| `moonshine_unregister_intent` | function | `core/moonshine-c-api.cpp:553` | `int32_t moonshine_unregister_intent(int32_t intent_recognizer_handle,                            ...` |
| `normalize_option_key` | function | `core/moonshine-c-api.cpp:1654` | `std::string normalize_option_key(const char *name)` |
| `parse_common_options` | function | `core/moonshine-c-api.cpp:98` | `OptionVector parse_common_options(const OptionVector &options)` |
| `parse_grapheme_phonemizer_options` | function | `core/moonshine-c-api.cpp:1809` | `void parse_grapheme_phonemizer_options(     const moonshine_option_t *in_options, uint64_t in_opt...` |
| `parse_int_option` | function | `core/moonshine-c-api.cpp:1662` | `std::optional<int32_t> parse_int_option(const std::string &value)` |
| `parse_option_vector` | function | `core/moonshine-c-api.cpp:83` | `OptionVector parse_option_vector(const moonshine_option_t *options,                              ...` |
| `parse_transcriber_options` | function | `core/moonshine-c-api.cpp:110` | `void parse_transcriber_options(const OptionVector &options,                                Transc...` |
| `parse_tts_options` | function | `core/moonshine-c-api.cpp:763` | `void parse_tts_options(const OptionVector &options,                        moonshine_tts::Moonshi...` |
| `pcm` | function | `core/moonshine-c-api.cpp:815` | `std::vector<float> pcm(n);` |
| `split_comma_nonempty_language_tokens` | function | `core/moonshine-c-api.cpp:1153` | `std::vector<std::string> split_comma_nonempty_language_tokens(const char *s)` |
| `MOONSHINE_C_API_H` | macro | `core/moonshine-c-api.h:2` | `#define MOONSHINE_C_API_H` |
| `MOONSHINE_EMBEDDING_MODEL_ARCH_GEMMA_300M` | macro | `core/moonshine-c-api.h:604` | `#define MOONSHINE_EMBEDDING_MODEL_ARCH_GEMMA_300M` |
| `MOONSHINE_ERROR_INVALID_ARGUMENT` | macro | `core/moonshine-c-api.h:109` | `#define MOONSHINE_ERROR_INVALID_ARGUMENT` |
| `MOONSHINE_ERROR_INVALID_HANDLE` | macro | `core/moonshine-c-api.h:108` | `#define MOONSHINE_ERROR_INVALID_HANDLE` |
| `MOONSHINE_ERROR_NONE` | macro | `core/moonshine-c-api.h:106` | `#define MOONSHINE_ERROR_NONE` |
| `MOONSHINE_ERROR_UNKNOWN` | macro | `core/moonshine-c-api.h:107` | `#define MOONSHINE_ERROR_UNKNOWN` |
| `MOONSHINE_EXPORT` | macro | `core/moonshine-c-api.h:78` | `#define MOONSHINE_EXPORT` |
| `MOONSHINE_EXPORT` | macro | `core/moonshine-c-api.h:80` | `#define MOONSHINE_EXPORT` |
| `MOONSHINE_FLAG_FORCE_UPDATE` | macro | `core/moonshine-c-api.h:112` | `#define MOONSHINE_FLAG_FORCE_UPDATE` |
| `MOONSHINE_FLAG_SPELLING_MODE` | macro | `core/moonshine-c-api.h:126` | `#define MOONSHINE_FLAG_SPELLING_MODE` |
| `MOONSHINE_HEADER_VERSION` | macro | `core/moonshine-c-api.h:95` | `#define MOONSHINE_HEADER_VERSION` |
| `MOONSHINE_INTENT_MAX_MATCHES` | macro | `core/moonshine-c-api.h:608` | `#define MOONSHINE_INTENT_MAX_MATCHES` |
| `MOONSHINE_MODEL_ARCH_BASE` | macro | `core/moonshine-c-api.h:99` | `#define MOONSHINE_MODEL_ARCH_BASE` |
| `MOONSHINE_MODEL_ARCH_BASE_STREAMING` | macro | `core/moonshine-c-api.h:101` | `#define MOONSHINE_MODEL_ARCH_BASE_STREAMING` |
| `MOONSHINE_MODEL_ARCH_MEDIUM_STREAMING` | macro | `core/moonshine-c-api.h:103` | `#define MOONSHINE_MODEL_ARCH_MEDIUM_STREAMING` |
| `MOONSHINE_MODEL_ARCH_SMALL_STREAMING` | macro | `core/moonshine-c-api.h:102` | `#define MOONSHINE_MODEL_ARCH_SMALL_STREAMING` |
| `MOONSHINE_MODEL_ARCH_TINY` | macro | `core/moonshine-c-api.h:98` | `#define MOONSHINE_MODEL_ARCH_TINY` |
| `MOONSHINE_MODEL_ARCH_TINY_STREAMING` | macro | `core/moonshine-c-api.h:100` | `#define MOONSHINE_MODEL_ARCH_TINY_STREAMING` |
| `effect` | variable | `core/moonshine-c-api.h:84` | `extern "C" { #endif /* ------------------------------ CONSTANTS -------------------------------- */ /* What version...` |
| `main` | function | `core/moonshine-c-api.h:38` | `int main(int argc, char *argv[])` |
| `moonshine_calculate_embedding_distance` | function | `core/moonshine-c-api.h:725` | `MOONSHINE_EXPORT int32_t moonshine_calculate_embedding_distance( int32_t intent_recognizer_handle, const float...` |
| `moonshine_calculate_intent_embedding` | function | `core/moonshine-c-api.h:708` | `MOONSHINE_EXPORT int32_t moonshine_calculate_intent_embedding( int32_t intent_recognizer_handle, const char...` |
| `moonshine_clear_intents` | function | `core/moonshine-c-api.h:698` | `MOONSHINE_EXPORT int32_t moonshine_clear_intents(int32_t intent_recognizer_handle);` |
| `moonshine_create_stream` | function | `core/moonshine-c-api.h:507` | `MOONSHINE_EXPORT int32_t moonshine_create_stream(int32_t transcriber_handle, uint32_t flags);` |
| `moonshine_create_tts_synthesizer_from_memory` | function | `core/moonshine-c-api.h:784` | `MOONSHINE_EXPORT int32_t moonshine_create_tts_synthesizer_from_memory( const char *language, const char **filenames...` |
| `moonshine_error_to_string` | function | `core/moonshine-c-api.h:290` | `MOONSHINE_EXPORT const char *moonshine_error_to_string(int32_t error);` |
| `moonshine_free_grapheme_to_phonemizer` | function | `core/moonshine-c-api.h:1013` | `MOONSHINE_EXPORT void moonshine_free_grapheme_to_phonemizer( int32_t grapheme_to_phonemizer_handle);` |
| `moonshine_free_intent_embedding` | function | `core/moonshine-c-api.h:715` | `MOONSHINE_EXPORT void moonshine_free_intent_embedding(float *embedding);` |
| `moonshine_free_intent_matches` | function | `core/moonshine-c-api.h:685` | `MOONSHINE_EXPORT void moonshine_free_intent_matches( struct moonshine_intent_match_t *matches, uint64_t count);` |
| `moonshine_free_intent_recognizer` | function | `core/moonshine-c-api.h:638` | `MOONSHINE_EXPORT void moonshine_free_intent_recognizer( int32_t intent_recognizer_handle);` |
| `moonshine_free_stream` | function | `core/moonshine-c-api.h:513` | `MOONSHINE_EXPORT int32_t moonshine_free_stream(int32_t transcriber_handle, int32_t stream_handle);` |
| `moonshine_free_transcriber` | function | `core/moonshine-c-api.h:388` | `MOONSHINE_EXPORT void moonshine_free_transcriber(int32_t transcriber_handle);` |
| `moonshine_free_tts_synthesizer` | function | `core/moonshine-c-api.h:793` | `MOONSHINE_EXPORT void moonshine_free_tts_synthesizer( int32_t tts_synthesizer_handle);` |
| `moonshine_get_g2p_dependencies` | function | `core/moonshine-c-api.h:813` | `MOONSHINE_EXPORT int32_t moonshine_get_g2p_dependencies( const char *languages, const struct moonshine_option_t...` |
| `moonshine_get_intent_dependencies` | function | `core/moonshine-c-api.h:915` | `MOONSHINE_EXPORT int32_t moonshine_get_intent_dependencies( const char *model_name, const struct moonshine_option_t...` |
| `moonshine_get_stt_dependencies` | function | `core/moonshine-c-api.h:892` | `MOONSHINE_EXPORT int32_t moonshine_get_stt_dependencies( const char *language, const struct moonshine_option_t...` |
| `moonshine_get_tts_dependencies` | function | `core/moonshine-c-api.h:830` | `MOONSHINE_EXPORT int32_t moonshine_get_tts_dependencies( const char *languages, const struct moonshine_option_t...` |
| `moonshine_get_tts_voices` | function | `core/moonshine-c-api.h:858` | `MOONSHINE_EXPORT int32_t moonshine_get_tts_voices( const char *languages, const struct moonshine_option_t *options...` |
| `moonshine_get_version` | function | `core/moonshine-c-api.h:286` | `MOONSHINE_EXPORT int32_t moonshine_get_version(void);` |
| `moonshine_intent_match_t` | struct | `core/moonshine-c-api.h:611` | `` |
| `moonshine_load_transcriber_from_files` | function | `core/moonshine-c-api.h:357` | `MOONSHINE_EXPORT int32_t moonshine_load_transcriber_from_files( const char *path, uint32_t model_arch, const struct...` |
| `moonshine_option_t` | struct | `core/moonshine-c-api.h:137` | `` |
| `moonshine_phonemes_to_speech` | function | `core/moonshine-c-api.h:953` | `MOONSHINE_EXPORT int32_t moonshine_phonemes_to_speech( int32_t tts_synthesizer_handle, const char *phonemes, const...` |
| `moonshine_register_intent` | function | `core/moonshine-c-api.h:652` | `MOONSHINE_EXPORT int32_t moonshine_register_intent( int32_t intent_recognizer_handle, const char *canonical_phrase...` |
| `moonshine_start_stream` | function | `core/moonshine-c-api.h:524` | `MOONSHINE_EXPORT int32_t moonshine_start_stream(int32_t transcriber_handle, int32_t stream_handle);` |
| `moonshine_stop_stream` | function | `core/moonshine-c-api.h:531` | `MOONSHINE_EXPORT int32_t moonshine_stop_stream(int32_t transcriber_handle, int32_t stream_handle);` |
| `moonshine_text_to_phonemes` | function | `core/moonshine-c-api.h:1019` | `MOONSHINE_EXPORT int32_t moonshine_text_to_phonemes( int32_t grapheme_to_phonemizer_handle, const char *text, const...` |
| `moonshine_text_to_speech` | function | `core/moonshine-c-api.h:929` | `MOONSHINE_EXPORT int32_t moonshine_text_to_speech( int32_t tts_synthesizer_handle, const char *text, const struct...` |
| `moonshine_transcribe_add_audio_to_stream` | function | `core/moonshine-c-api.h:564` | `MOONSHINE_EXPORT int32_t moonshine_transcribe_add_audio_to_stream( int32_t transcriber_handle, int32_t...` |
| `moonshine_transcribe_stream` | function | `core/moonshine-c-api.h:597` | `MOONSHINE_EXPORT int32_t moonshine_transcribe_stream( int32_t transcriber_handle, int32_t stream_handle, uint32_t...` |
| `moonshine_transcribe_without_streaming` | function | `core/moonshine-c-api.h:425` | `MOONSHINE_EXPORT int32_t moonshine_transcribe_without_streaming( int32_t transcriber_handle, float *audio_data...` |
| `moonshine_transcript_to_string` | function | `core/moonshine-c-api.h:295` | `MOONSHINE_EXPORT const char *moonshine_transcript_to_string( const struct transcript_t *transcript);` |
| `moonshine_unregister_intent` | function | `core/moonshine-c-api.h:659` | `MOONSHINE_EXPORT int32_t moonshine_unregister_intent( int32_t intent_recognizer_handle, const char *canonical_phrase);` |
| `speaker_span_t` | struct | `core/moonshine-c-api.h:212` | `` |
| `transcript_line_t` | struct | `core/moonshine-c-api.h:231` | `` |
| `transcript_t` | struct | `core/moonshine-c-api.h:276` | `` |
| `transcript_word_t` | struct | `core/moonshine-c-api.h:194` | `` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-cpp-test.cpp:7` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `SUBCASE` | function | `core/moonshine-cpp-test.cpp:164` | `SUBCASE("transcribe-without-streaming")` |
| `SUBCASE` | function | `core/moonshine-cpp-test.cpp:193` | `SUBCASE("transcribe-with-streaming")` |
| `SUBCASE` | function | `core/moonshine-cpp-test.cpp:288` | `SUBCASE("g2p")` |
| `SUBCASE` | function | `core/moonshine-cpp-test.cpp:306` | `SUBCASE("intent recognizer invalid model path throws")` |
| `SUBCASE` | function | `core/moonshine-cpp-test.cpp:312` | `SUBCASE("spelling-mode-replaces-line-text-via-cpp-ctor")` |
| `SUBCASE` | function | `core/moonshine-cpp-test.cpp:347` | `SUBCASE("loadFromMemory-with-spelling-buffer")` |
| `SUBCASE` | function | `core/moonshine-cpp-test.cpp:395` | `SUBCASE("intent recognizer closest intents when embedding model present")` |
| `TEST_CASE` | function | `core/moonshine-cpp-test.cpp:163` | `TEST_CASE("moonshine-cpp-test")` |
| `file_exists` | function | `core/moonshine-cpp-test.cpp:132` | `bool file_exists(const std::string &path)` |
| `load_wav_data` | function | `core/moonshine-cpp-test.cpp:13` | `bool load_wav_data(const char *path, float **out_float_data,                    size_t *out_num_s...` |
| `onLineCompleted` | function | `core/moonshine-cpp-test.cpp:156` | `void onLineCompleted(const moonshine::LineCompleted &) override` |
| `onLineStarted` | function | `core/moonshine-cpp-test.cpp:147` | `void onLineStarted(const moonshine::LineStarted &) override` |
| `onLineTextChanged` | function | `core/moonshine-cpp-test.cpp:153` | `void onLineTextChanged(const moonshine::LineTextChanged &) override` |
| `onLineUpdated` | function | `core/moonshine-cpp-test.cpp:150` | `void onLineUpdated(const moonshine::LineUpdated &) override` |
| `EmbeddingModelArch` | enum | `core/moonshine-cpp.h:76` | `` |
| `Error` | class | `core/moonshine-cpp.h:363` | `` |
| `Error` | function | `core/moonshine-cpp.h:368` | `Error(const std::string &errorMessage, int32_t streamHandle)       : TranscriptEvent(TranscriptLi...` |
| `Error` | function | `core/moonshine-cpp.h:372` | `Error(const std::string &errorMessage, const TranscriptLine &line,         int32_t streamHandle) ...` |
| `GraphemeToPhonemizer` | class | `core/moonshine-cpp.h:800` | `` |
| `GraphemeToPhonemizer` | function | `core/moonshine-cpp.h:1523` | `inline GraphemeToPhonemizer::GraphemeToPhonemizer(     const std::string &language, const std::ve...` |
| `GraphemeToPhonemizer` | function | `core/moonshine-cpp.h:1534` | `inline GraphemeToPhonemizer::GraphemeToPhonemizer(GraphemeToPhonemizer &&other)     : handle_(oth...` |
| `IntentMatch` | struct | `core/moonshine-cpp.h:858` | `` |
| `IntentMatch` | function | `core/moonshine-cpp.h:863` | `IntentMatch(std::string phrase, float sim)       : canonicalPhrase(std::move(phrase)), similarity...` |
| `IntentRecognizer` | class | `core/moonshine-cpp.h:868` | `` |
| `IntentRecognizer` | function | `core/moonshine-cpp.h:1601` | `inline IntentRecognizer::IntentRecognizer(const std::string &model_path,                         ...` |
| `IntentRecognizer` | function | `core/moonshine-cpp.h:1612` | `inline IntentRecognizer::IntentRecognizer(IntentRecognizer &&other) noexcept     : handle_(other....` |
| `LineCompleted` | class | `core/moonshine-cpp.h:356` | `` |
| `LineCompleted` | function | `core/moonshine-cpp.h:358` | `public:   LineCompleted(const TranscriptLine &line, int32_t streamHandle)       : TranscriptEvent...` |
| `LineSpeakersChanged` | class | `core/moonshine-cpp.h:349` | `` |
| `LineSpeakersChanged` | function | `core/moonshine-cpp.h:351` | `public:   LineSpeakersChanged(const TranscriptLine &line, int32_t streamHandle)       : Transcrip...` |
| `LineStarted` | class | `core/moonshine-cpp.h:325` | `` |
| `LineStarted` | function | `core/moonshine-cpp.h:327` | `public:   LineStarted(const TranscriptLine &line, int32_t streamHandle)       : TranscriptEvent(l...` |
| `LineTextChanged` | class | `core/moonshine-cpp.h:339` | `` |
| `LineTextChanged` | function | `core/moonshine-cpp.h:341` | `public:   LineTextChanged(const TranscriptLine &line, int32_t streamHandle)       : TranscriptEve...` |
| `LineUpdated` | class | `core/moonshine-cpp.h:332` | `` |
| `LineUpdated` | function | `core/moonshine-cpp.h:334` | `public:   LineUpdated(const TranscriptLine &line, int32_t streamHandle)       : TranscriptEvent(l...` |
| `MOONSHINE_CPP_H` | macro | `core/moonshine-cpp.h:2` | `#define MOONSHINE_CPP_H` |
| `ModelArch` | enum | `core/moonshine-cpp.h:66` | `` |
| `ModelArch` | class | `core/moonshine-cpp.h:66` | `` |
| `MoonshineException` | function | `core/moonshine-cpp.h:414` | `public:   MoonshineException(const std::string &message)       : std::runtime_error(message)` |
| `OptionsBuffer` | struct | `core/moonshine-cpp.h:1181` | `` |
| `SpeakerSpan` | struct | `core/moonshine-cpp.h:104` | `` |
| `SpeakerSpan` | function | `core/moonshine-cpp.h:120` | `SpeakerSpan()       : startTime(0.0f),         duration(0.0f),         speakerId(0),         spea...` |
| `SpeakerSpan` | function | `core/moonshine-cpp.h:127` | `SpeakerSpan(float startTime, float duration, uint64_t speakerId,               uint32_t speakerIn...` |

Next: [SYMBOLS_p3.md](SYMBOLS_p3.md)
