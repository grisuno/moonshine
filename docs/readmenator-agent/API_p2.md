# API (page 2 of 10)
Previous: [API.md](API.md)

## core/cpp-annote/src/embedding_ort_infer.cpp
Depends on: `core/cpp-annote/src/compute_fbank.h`, `core/cpp-annote/src/embedding_ort_infer.h`
- `any_non_finite_embedding` (function) `core/cpp-annote/src/embedding_ort_infer.cpp:16` `bool any_non_finite_embedding(const float* e, int dim)`
- `embedding_json_inputs_fbank_first` (function) `core/cpp-annote/src/embedding_ort_infer.cpp:27` `bool embedding_json_inputs_fbank_first(const std::string& emb_json)`
- `run_embedding_ort` (function) `core/cpp-annote/src/embedding_ort_infer.cpp:40` `void run_embedding_ort(Ort::Session& sess, Ort::MemoryInfo& mem,
                       Ort::Allo...`
- `discover_min_num_samples_embedding` (function) `core/cpp-annote/src/embedding_ort_infer.cpp:78` `int discover_min_num_samples_embedding(Ort::Session& sess, Ort::MemoryInfo& mem,
                ...`
- `noise` (function) `core/cpp-annote/src/embedding_ort_infer.cpp:87` `std::vector<float> noise(static_cast<size_t>(middle));`
- `wts` (function) `core/cpp-annote/src/embedding_ort_infer.cpp:102` `std::vector<float> wts(static_cast<size_t>(Tf), 1.f);`
- `emb` (function) `core/cpp-annote/src/embedding_ort_infer.cpp:103` `std::vector<float> emb(static_cast<size_t>(embed_dim));`
- `fbank_num_frames_for_samples` (function) `core/cpp-annote/src/embedding_ort_infer.cpp:115` `int fbank_num_frames_for_samples(int embed_sr, int mel_bins, float fl_ms,
                       ...`
- `seg_to_fbank_nearest_index` (function) `core/cpp-annote/src/embedding_ort_infer.cpp:130` `int seg_to_fbank_nearest_index(int tf, int num_seg_frames,
                               int num...`

## core/cpp-annote/src/embedding_ort_infer.h
Imported by: `core/cpp-annote/src/cpp-annote.cpp`, `core/cpp-annote/src/embedding_ort_infer.cpp`
- `embedding_json_inputs_fbank_first` (function) `core/cpp-annote/src/embedding_ort_infer.h:14` `bool embedding_json_inputs_fbank_first(const std::string& emb_json);`
- `run_embedding_ort` (function) `core/cpp-annote/src/embedding_ort_infer.h:16` `void run_embedding_ort(Ort::Session& sess, Ort::MemoryInfo& mem, Ort::AllocatorWithDefaultOptions& alloc, bool...`
- `discover_min_num_samples_embedding` (function) `core/cpp-annote/src/embedding_ort_infer.h:22` `int discover_min_num_samples_embedding(Ort::Session& sess, Ort::MemoryInfo& mem, Ort::AllocatorWithDefaultOptions&...`
- `fbank_num_frames_for_samples` (function) `core/cpp-annote/src/embedding_ort_infer.h:28` `int fbank_num_frames_for_samples(int embed_sr, int mel_bins, float fl_ms, float fs_ms, int num_samples);`
- `seg_to_fbank_nearest_index` (function) `core/cpp-annote/src/embedding_ort_infer.h:31` `int seg_to_fbank_nearest_index(int tf, int num_seg_frames, int num_fbank_frames);`

## core/cpp-annote/src/filter_train.cpp
Depends on: `core/cpp-annote/src/filter_train.h`
- `filter_embeddings_train` (function) `core/cpp-annote/src/filter_train.cpp:10` `void filter_embeddings_train(int num_chunks, int num_frames, int num_speakers,
                  ...`

## core/cpp-annote/src/filter_train.h
Imported by: `core/cpp-annote/src/clustering_vbx.cpp`, `core/cpp-annote/src/filter_train.cpp`
- `filter_embeddings_train` (function) `core/cpp-annote/src/filter_train.h:15` `void filter_embeddings_train(int num_chunks, int num_frames, int num_speakers, int dim, const float* embeddings...` -- Row-major ``embeddings`` length ``num_chunks * num_speakers * dim``; ``binarized`` length ``num_chunks * num_frames...

## core/cpp-annote/src/hungarian.h
Imported by: `core/cpp-annote/src/clustering_vbx.cpp`
- `u` (function) `core/cpp-annote/src/hungarian.h:29` `std::vector<double> u(big_n, 0.0);`
- `v` (function) `core/cpp-annote/src/hungarian.h:30` `std::vector<double> v(big_m, 0.0);`
- `p` (function) `core/cpp-annote/src/hungarian.h:31` `std::vector<int> p(big_m, 0);`
- `way` (function) `core/cpp-annote/src/hungarian.h:32` `std::vector<int> way(big_m, 0);`
- `minv` (function) `core/cpp-annote/src/hungarian.h:36` `std::vector<double> minv(big_m, inf);`
- `used` (function) `core/cpp-annote/src/hungarian.h:37` `std::vector<char> used(big_m, 0);`
- `assignment` (function) `core/cpp-annote/src/hungarian.h:75` `std::vector<int> assignment(static_cast<std::size_t>(n), -1);`

## core/cpp-annote/src/parity_log.cpp
Depends on: `core/cpp-annote/src/parity_log.h`
- `env_parity_level` (function) `core/cpp-annote/src/parity_log.cpp:19` `int env_parity_level()`
- `env_parity_out_dir` (function) `core/cpp-annote/src/parity_log.cpp:33` `const char* env_parity_out_dir()`
- `log_light` (function) `core/cpp-annote/src/parity_log.cpp:41` `void log_light(const std::string& line)`
- `heavy_dumps_enabled` (function) `core/cpp-annote/src/parity_log.cpp:47` `bool heavy_dumps_enabled()`
- `ensure_parity_out_dir` (function) `core/cpp-annote/src/parity_log.cpp:51` `void ensure_parity_out_dir()`
- `parity_clustering_npz_path` (function) `core/cpp-annote/src/parity_log.cpp:64` `std::string parity_clustering_npz_path()`
- `fingerprint_float32` (function) `core/cpp-annote/src/parity_log.cpp:74` `std::string fingerprint_float32(const float* data, std::size_t n,
                               ...`

## core/cpp-annote/src/parity_log.h
Imported by: `core/cpp-annote/src/clustering_vbx.cpp`, `core/cpp-annote/src/cpp-annote.cpp`, `core/cpp-annote/src/parity_log.cpp`
- `env_parity_level` (function) `core/cpp-annote/src/parity_log.h:16` `int env_parity_level();` -- ``PYANNOTE_CPP_PARITY``: unset or ``0`` = off; ``1`` = stderr light log; ``2`` = heavy dumps (needs out dir).
- `env_parity_out_dir` (function) `core/cpp-annote/src/parity_log.h:20` `const char* env_parity_out_dir();` -- ``PYANNOTE_CPP_PARITY_OUT``: directory for level-2 NPZ bundle (created if missing).
- `log_light` (function) `core/cpp-annote/src/parity_log.h:23` `void log_light(const std::string& line);` -- One stderr line when ``env_parity_level() >= 1``.
- `heavy_dumps_enabled` (function) `core/cpp-annote/src/parity_log.h:26` `bool heavy_dumps_enabled();` -- True when level >= 2 and ``PYANNOTE_CPP_PARITY_OUT`` is non-empty.
- `ensure_parity_out_dir` (function) `core/cpp-annote/src/parity_log.h:29` `void ensure_parity_out_dir();` -- Create output directory (recursive).

## core/cpp-annote/src/plda_vbx.cpp
Depends on: `core/cpp-annote/src/plda_vbx.h`
- `align_eigen_evecs_to_scipy_wccn_row0_for_community1_plda` (function) `core/cpp-annote/src/plda_vbx.cpp:67` `void align_eigen_evecs_to_scipy_wccn_row0_for_community1_plda(
    const RowMatrixXd& tr_file, Ei...`
- `row_l2_normalize` (function) `core/cpp-annote/src/plda_vbx.cpp:88` `void row_l2_normalize(Eigen::MatrixXd& M)`
- `logsumexp_rowwise` (function) `core/cpp-annote/src/plda_vbx.cpp:97` `void logsumexp_rowwise(const Eigen::MatrixXd& M, Eigen::VectorXd& lse,
                       Eig...`
- `load_from_arrays` (function) `core/cpp-annote/src/plda_vbx.cpp:118` `void PldaModel::load_from_arrays(const double* mean1_p, int n_mean1,
                            ...`
- `load` (function) `core/cpp-annote/src/plda_vbx.cpp:161` `void PldaModel::load(const std::string& xvec_transform_npz,
                     const std::strin...` -- The upstream file-based PldaModel::load() (cnpy NPZ loading) is removed in this vendored copy; see plda_vbx.h. if 0
- `xvec_tf` (function) `core/cpp-annote/src/plda_vbx.cpp:257` `Eigen::MatrixXd PldaModel::xvec_tf(const Eigen::MatrixXd& embeddings) const`
- `plda_tf` (function) `core/cpp-annote/src/plda_vbx.cpp:272` `Eigen::MatrixXd PldaModel::plda_tf(const Eigen::MatrixXd& x0,
                                   ...`
- `operator` (function) `core/cpp-annote/src/plda_vbx.cpp:282` `Eigen::MatrixXd PldaModel::operator()(const Eigen::MatrixXd& embeddings) const`
- `softmax_rows` (function) `core/cpp-annote/src/plda_vbx.cpp:286` `void softmax_rows(const Eigen::MatrixXd& logits, Eigen::MatrixXd& out)`
- `cluster_vbx` (function) `core/cpp-annote/src/plda_vbx.cpp:299` `void cluster_vbx(const std::vector<int>& ahc_init, const Eigen::MatrixXd& fea,
                 c...`

## core/cpp-annote/src/plda_vbx.h
Imported by: `core/cpp-annote/src/clustering_vbx.h`, `core/cpp-annote/src/cpp-annote-engine.h`, `core/cpp-annote/src/cpp-annote.cpp`, `core/cpp-annote/src/plda_vbx.cpp`
- `load_from_arrays` (function) `core/cpp-annote/src/plda_vbx.h:34` `void load_from_arrays(const double* mean1, int n_mean1, const float* mean2, int n_mean2, const float* lda, int...` -- Load from raw NumPy-export tensors (same layout as HF ``xvec_transform.npz`` / ``plda.npz``).
- `softmax_rows` (function) `core/cpp-annote/src/plda_vbx.h:44` `void softmax_rows(const Eigen::MatrixXd& logits, Eigen::MatrixXd& out);`
- `cluster_vbx` (function) `core/cpp-annote/src/plda_vbx.h:52` `void cluster_vbx(const std::vector<int>& ahc_init, const Eigen::MatrixXd& fea, const Eigen::VectorXd& Phi, double...` -- ``cluster_vbx`` from ``vbx.py`` (``return_model=True`` path).

## core/cpp-annote/src/scipy_linkage.cpp
Depends on: `core/cpp-annote/src/scipy_linkage.h`
- `centroid_update` (function) `core/cpp-annote/src/scipy_linkage.cpp:16` `inline double centroid_update(double d_xi, double d_yi, double d_xy, int size_x,
                ...`
- `is_visited` (function) `core/cpp-annote/src/scipy_linkage.cpp:34` `inline bool is_visited(const std::vector<unsigned char>& bitset, int i)`
- `set_visited` (function) `core/cpp-annote/src/scipy_linkage.cpp:39` `inline void set_visited(std::vector<unsigned char>& bitset, int i)`
- `visited_bytes` (function) `core/cpp-annote/src/scipy_linkage.cpp:44` `inline int visited_bytes(int n)`
- `get_max_dist_for_each_cluster` (function) `core/cpp-annote/src/scipy_linkage.cpp:46` `void get_max_dist_for_each_cluster(const double* Z, int n,
                                   std...`
- `curr_node` (function) `core/cpp-annote/src/scipy_linkage.cpp:49` `std::vector<int> curr_node(static_cast<std::size_t>(n));`
- `visited` (function) `core/cpp-annote/src/scipy_linkage.cpp:50` `std::vector<unsigned char> visited(static_cast<std::size_t>(visited_bytes(n)), 0);`
- `cluster_monocrit` (function) `core/cpp-annote/src/scipy_linkage.cpp:93` `void cluster_monocrit(const double* Z, int n, const std::vector<double>& MC,
                    ...`
- `pdist_euclidean` (function) `core/cpp-annote/src/scipy_linkage.cpp:151` `void pdist_euclidean(const std::vector<double>& X, int n, int d,
                     std::vector...`
- `linkage_centroid_naive` (function) `core/cpp-annote/src/scipy_linkage.cpp:169` `void linkage_centroid_naive(const std::vector<double>& dist, int n,
                            s...`
- `id_map` (function) `core/cpp-annote/src/scipy_linkage.cpp:173` `std::vector<int> id_map(static_cast<std::size_t>(n));`
- `fcluster_distance` (function) `core/cpp-annote/src/scipy_linkage.cpp:237` `void fcluster_distance(const std::vector<double>& Z, int n, double cutoff,
                      ...`
- `remap_labels_contiguous` (function) `core/cpp-annote/src/scipy_linkage.cpp:244` `void remap_labels_contiguous(const std::vector<int>& labels_one_based,
                          ...`
- `z` (function) `core/cpp-annote/src/scipy_linkage.cpp:247` `std::vector<int> z(static_cast<std::size_t>(n));`

## core/cpp-annote/src/scipy_linkage.h
Imported by: `core/cpp-annote/src/clustering_vbx.cpp`, `core/cpp-annote/src/scipy_linkage.cpp`
- `condensed_index` (function) `core/cpp-annote/src/scipy_linkage.h:14` `inline std::size_t condensed_index(int n, int i, int j)`
- `pdist_euclidean` (function) `core/cpp-annote/src/scipy_linkage.h:23` `void pdist_euclidean(const std::vector<double>& X, int n, int d, std::vector<double>& dist);` -- Row-major `X`: `n` rows, `d` cols → condensed pairwise Euclidean distances (length n*(n-1)/2).
- `linkage_centroid_naive` (function) `core/cpp-annote/src/scipy_linkage.h:29` `void linkage_centroid_naive(const std::vector<double>& dist, int n, std::vector<double>& Z);` -- SciPy `linkage(..., method='centroid')` via the generic O(n³) SciPy C implementation (small `n` only).
- `fcluster_distance` (function) `core/cpp-annote/src/scipy_linkage.h:35` `void fcluster_distance(const std::vector<double>& Z, int n, double cutoff, std::vector<int>& T);` -- ``fcluster(Z, t, criterion='distance')`` → labels in **SciPy convention** (1..K inclusive).
- `remap_labels_contiguous` (function) `core/cpp-annote/src/scipy_linkage.h:39` `void remap_labels_contiguous(const std::vector<int>& labels_one_based, std::vector<int>& out);` -- `np.unique(labels - 1, return_inverse=True)[1]` — contiguous 0..K-1.

## core/cpp-annote/src/wav_pcm_float32.h
Imported by: `core/cpp-annote/src/cpp-annote-streaming.cpp`, `core/cpp-annote/src/cpp-annote.cpp`, `core/reliability/fuzz-wav-pcm.cpp`
- `read_file_bytes` (function) `core/cpp-annote/src/wav_pcm_float32.h:18` `inline std::vector<std::uint8_t> read_file_bytes(const std::string& path)`
- `buf` (function) `core/cpp-annote/src/wav_pcm_float32.h:29` `std::vector<std::uint8_t> buf(static_cast<size_t>(sz));`
- `u32` (function) `core/cpp-annote/src/wav_pcm_float32.h:37` `inline std::uint32_t u32(const std::uint8_t* p)`
- `u16` (function) `core/cpp-annote/src/wav_pcm_float32.h:44` `inline std::uint16_t u16(const std::uint8_t* p)`
- `load_wav_pcm16_mono_float32` (function) `core/cpp-annote/src/wav_pcm_float32.h:51` `inline std::vector<float> load_wav_pcm16_mono_float32(const std::string& path,
                  ...` -- PCM 16 LE mono or stereo (mean to mono) → float32 mono, sample_rate_out set from header.
- `mono` (function) `core/cpp-annote/src/wav_pcm_float32.h:104` `std::vector<float> mono(num_frames);`
- `linear_resample` (function) `core/cpp-annote/src/wav_pcm_float32.h:120` `inline std::vector<float> linear_resample(const std::vector<float>& x,
                          ...`
- `y` (function) `core/cpp-annote/src/wav_pcm_float32.h:132` `std::vector<float> y(n_out);`

## core/embedding-model.h
Imported by: `core/gemma-embedding-model.h`, `core/intent-recognizer.h`
- `get_similarity` (function) `core/embedding-model.h:29` `float get_similarity(const std::string &a, const std::string &b)` -- Compute the similarity between two text strings. @param a The first text string. @param b The second text string....
- `get_similarity` (function) `core/embedding-model.h:41` `float get_similarity(const std::string &text,
                       const std::vector<float> &em...` -- Compute the similarity between a text string and a precomputed embedding. @param text The text string to compare....
- `get_similarity` (function) `core/embedding-model.h:53` `float get_similarity(const std::vector<float> &embedding_a,
                       const std::vec...` -- Compute the similarity between two precomputed embeddings. @param embedding_a The first embedding vector. @param...
- `cosine_similarity` (function) `core/embedding-model.h:65` `float cosine_similarity(const std::vector<float> &a,
                          const std::vector<...` -- Compute the cosine similarity between two vectors. @param a The first vector. @param b The second vector. @return...

## core/gemma-embedding-model-test.cpp
Depends on: `core/gemma-embedding-model.h`
- `TEST_CASE` (function) `core/gemma-embedding-model-test.cpp:10` `TEST_CASE("gemma-embedding-model")`
- `SUBCASE` (function) `core/gemma-embedding-model-test.cpp:18` `SUBCASE("load model")`
- `SUBCASE` (function) `core/gemma-embedding-model-test.cpp:26` `SUBCASE("get embeddings")`
- `SUBCASE` (function) `core/gemma-embedding-model-test.cpp:46` `SUBCASE("identical strings have similarity 1.0")`
- `SUBCASE` (function) `core/gemma-embedding-model-test.cpp:55` `SUBCASE("similar strings have high similarity")`
- `SUBCASE` (function) `core/gemma-embedding-model-test.cpp:67` `SUBCASE("different strings have lower similarity")`
- `SUBCASE` (function) `core/gemma-embedding-model-test.cpp:79` `SUBCASE("query and document embeddings")`
- `SUBCASE` (function) `core/gemma-embedding-model-test.cpp:99` `SUBCASE("truncate embedding with MRL")`
- `SUBCASE` (function) `core/gemma-embedding-model-test.cpp:126` `SUBCASE("config values")`
- `TEST_CASE` (function) `core/gemma-embedding-model-test.cpp:138` `TEST_CASE("gemma-embedding-model error handling")`
- `SUBCASE` (function) `core/gemma-embedding-model-test.cpp:139` `SUBCASE("load nonexistent model")`
- `SUBCASE` (function) `core/gemma-embedding-model-test.cpp:146` `SUBCASE("get embeddings without loading")`
- `SUBCASE` (function) `core/gemma-embedding-model-test.cpp:152` `SUBCASE("load invalid variant")`

## core/gemma-embedding-model.cpp
Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/gemma-embedding-model.h`, `core/moonshine-utils/debug-utils.h`, `core/moonshine-utils/string-utils.h`, `core/ort-utils/ort-utils.h`
- `GemmaEmbeddingModel` (function) `core/gemma-embedding-model.cpp:21` `GemmaEmbeddingModel::GemmaEmbeddingModel()
    : ort_api_(nullptr),
      ort_env_(nullptr),
    ...`
- `load` (function) `core/gemma-embedding-model.cpp:67` `int GemmaEmbeddingModel::load(const char *model_dir,
                              const char *mo...`
- `load_from_memory` (function) `core/gemma-embedding-model.cpp:111` `int GemmaEmbeddingModel::load_from_memory(const uint8_t *model_data,
                            ...`
- `load_tokenizer` (function) `core/gemma-embedding-model.cpp:131` `int GemmaEmbeddingModel::load_tokenizer(const char *tokenizer_path)`
- `load_tokenizer_from_memory` (function) `core/gemma-embedding-model.cpp:142` `int GemmaEmbeddingModel::load_tokenizer_from_memory(const uint8_t *data,
                        ...`
- `tokenize` (function) `core/gemma-embedding-model.cpp:161` `std::vector<int64_t> GemmaEmbeddingModel::tokenize(const std::string &text)`
- `run_inference` (function) `core/gemma-embedding-model.cpp:186` `std::vector<float> GemmaEmbeddingModel::run_inference(
    const std::vector<int64_t> &input_ids,...`
- `output_shape` (function) `core/gemma-embedding-model.cpp:263` `std::vector<int64_t> output_shape(num_dims);`
- `embedding` (function) `core/gemma-embedding-model.cpp:288` `std::vector<float> embedding(output_data, output_data + output_size);`
- `get_embeddings` (function) `core/gemma-embedding-model.cpp:298` `std::vector<float> GemmaEmbeddingModel::get_embeddings(
    const std::string &text)`
- `attention_mask` (function) `core/gemma-embedding-model.cpp:309` `std::vector<int64_t> attention_mask(input_ids.size(), 1);` -- Create attention mask (all 1s for actual tokens)
- `get_embeddings_with_prefix` (function) `core/gemma-embedding-model.cpp:315` `std::vector<float> GemmaEmbeddingModel::get_embeddings_with_prefix(
    const std::string &text, ...`
- `get_query_embeddings` (function) `core/gemma-embedding-model.cpp:320` `std::vector<float> GemmaEmbeddingModel::get_query_embeddings(
    const std::string &query)`
- `get_document_embeddings` (function) `core/gemma-embedding-model.cpp:325` `std::vector<float> GemmaEmbeddingModel::get_document_embeddings(
    const std::string &document)`
- `truncate_embedding` (function) `core/gemma-embedding-model.cpp:330` `std::vector<float> GemmaEmbeddingModel::truncate_embedding(
    const std::vector<float> &embeddi...`
- `truncated` (function) `core/gemma-embedding-model.cpp:337` `std::vector<float> truncated(embedding.begin(), embedding.begin() + target_dim);` -- Truncate to target dimension (MRL - Matryoshka Representation Learning)
- `normalize_embedding` (function) `core/gemma-embedding-model.cpp:346` `void GemmaEmbeddingModel::normalize_embedding(std::vector<float> &embedding)`
- `is_loaded` (function) `core/gemma-embedding-model.cpp:362` `bool GemmaEmbeddingModel::is_loaded() const`
- `get_config` (function) `core/gemma-embedding-model.cpp:364` `const GemmaEmbeddingConfig &GemmaEmbeddingModel::get_config() const`

## core/gemma-embedding-model.h
Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/embedding-model.h`, `core/ort-utils/moonshine-ort-allocator.h`
Imported by: `core/gemma-embedding-model-test.cpp`, `core/gemma-embedding-model.cpp`, `core/intent-recognizer-test.cpp`, `core/intent-recognizer.cpp`
- `load` (function) `core/gemma-embedding-model.h:51` `int load(const char *model_dir, const char *model_variant = "q4");` -- Load the model from a directory containing model files. @param model_dir Directory containing model.onnx (or...
- `load_from_memory` (function) `core/gemma-embedding-model.h:61` `int load_from_memory(const uint8_t *model_data, size_t model_data_size, const uint8_t *tokenizer_data, size_t...` -- Load the model from memory buffers. @param model_data Pointer to ONNX model data. @param model_data_size Size of...
- `prefix` (function) `core/gemma-embedding-model.h:73` `* Get embeddings with a specific prefix (for query vs document embeddings). * @param text The input text to embed. *...`
- `embeddings` (function) `core/gemma-embedding-model.h:83` `* Get query embeddings (uses query prefix). * @param query The query text. * @return A vector of floats representing...`
- `truncate_embedding` (function) `core/gemma-embedding-model.h:102` `static std::vector<float> truncate_embedding( const std::vector<float> &embedding, int target_dim);` -- Truncate an embedding to a smaller dimension using MRL. @param embedding The original embedding. @param target_dim...
- `is_loaded` (function) `core/gemma-embedding-model.h:109` `bool is_loaded() const;` -- Check if the model is loaded. @return True if the model is loaded and ready for inference.
- `get_config` (function) `core/gemma-embedding-model.h:115` `const GemmaEmbeddingConfig &get_config() const;` -- Get the model configuration. @return The model configuration.
- `load_tokenizer` (function) `core/gemma-embedding-model.h:148` `int load_tokenizer(const char *tokenizer_path);` -- Load the tokenizer from a file path. @param tokenizer_path Path to tokenizer.bin. @return 0 on success, non-zero on...
- `load_tokenizer_from_memory` (function) `core/gemma-embedding-model.h:156` `int load_tokenizer_from_memory(const uint8_t *data, size_t data_size);` -- Load the tokenizer from memory. @param data Pointer to tokenizer.bin data. @param data_size Size of data in bytes....
- `tokenize` (function) `core/gemma-embedding-model.h:163` `std::vector<int64_t> tokenize(const std::string &text);` -- Tokenize input text to token IDs. @param text The input text. @return Vector of token IDs.
- `run_inference` (function) `core/gemma-embedding-model.h:171` `std::vector<float> run_inference(const std::vector<int64_t> &input_ids, const std::vector<int64_t> &attention_mask);` -- Run inference to get embeddings for token IDs. @param input_ids The token IDs. @param attention_mask The attention...
- `normalize_embedding` (function) `core/gemma-embedding-model.h:178` `static void normalize_embedding(std::vector<float> &embedding);` -- Normalize an embedding vector to unit length. @param embedding The embedding to normalize (modified in place).

## core/intent-recognizer.cpp
Depends on: `core/gemma-embedding-model.h`, `core/intent-recognizer.h`
- `create_embedding_model` (function) `core/intent-recognizer.cpp:11` `std::unique_ptr<EmbeddingModel> create_embedding_model(
    const IntentRecognizerOptions &options)`
- `IntentRecognizer` (function) `core/intent-recognizer.cpp:31` `IntentRecognizer::IntentRecognizer(const IntentRecognizerOptions &options)
    : embedding_model_...`
- `register_intent` (function) `core/intent-recognizer.cpp:36` `void IntentRecognizer::register_intent(const std::string &trigger_phrase)`
- `register_intent` (function) `core/intent-recognizer.cpp:40` `void IntentRecognizer::register_intent(const std::string &trigger_phrase,
                       ...`
- `unregister_intent` (function) `core/intent-recognizer.cpp:68` `bool IntentRecognizer::unregister_intent(const std::string &trigger_phrase)`
- `sort` (function) `core/intent-recognizer.cpp:115` `std::sort(entries.begin(), entries.end(), [](const auto &a, const auto &b)`
- `get_intent_count` (function) `core/intent-recognizer.cpp:130` `size_t IntentRecognizer::get_intent_count() const`
- `clear_intents` (function) `core/intent-recognizer.cpp:135` `void IntentRecognizer::clear_intents()`
- `calculate_embedding` (function) `core/intent-recognizer.cpp:140` `std::vector<float> IntentRecognizer::calculate_embedding(
    const std::string &sentence) const`
- `calculate_similarity` (function) `core/intent-recognizer.cpp:146` `float IntentRecognizer::calculate_similarity(
    const std::vector<float> &a, const std::vector<...`
- `get_embedding_size` (function) `core/intent-recognizer.cpp:152` `size_t IntentRecognizer::get_embedding_size() const`

## core/intent-recognizer.h
Depends on: `core/embedding-model.h`
Imported by: `core/intent-recognizer-test.cpp`, `core/intent-recognizer.cpp`, `core/moonshine-c-api.cpp`
- `register_intent` (function) `core/intent-recognizer.h:66` `void register_intent(const std::string &trigger_phrase);` -- Register an intent with a trigger phrase. @param trigger_phrase The canonical phrase for this intent.
- `unregister_intent` (function) `core/intent-recognizer.h:86` `bool unregister_intent(const std::string &trigger_phrase);` -- Remove a registered intent. @param trigger_phrase The trigger phrase of the intent to remove. @return True if the...
- `get_intent_count` (function) `core/intent-recognizer.h:103` `size_t get_intent_count() const;` -- Get the number of registered intents. @return The number of registered intents.
- `clear_intents` (function) `core/intent-recognizer.h:108` `void clear_intents();` -- Clear all registered intents.
- `calculate_embedding` (function) `core/intent-recognizer.h:115` `std::vector<float> calculate_embedding(const std::string &sentence) const;` -- Calculate the embedding for a given sentence using the loaded model. @param sentence The input text. @return The...
- `calculate_similarity` (function) `core/intent-recognizer.h:123` `float calculate_similarity(const std::vector<float> &a, const std::vector<float> &b) const;` -- Compute cosine similarity between two precomputed embeddings. @param a The first embedding vector. @param b The...
- `get_embedding_size` (function) `core/intent-recognizer.h:130` `size_t get_embedding_size() const;` -- Get the embedding dimension of the loaded model. @return The number of floats per embedding.

## core/moonshine-c-api-memory-test.cpp
Depends on: `core/moonshine-c-api.h`
- `read_binary_file` (function) `core/moonshine-c-api-memory-test.cpp:34` `std::vector<uint8_t> read_binary_file(const std::filesystem::path& p)`
- `kokoro_lang_for_voice_stem` (function) `core/moonshine-c-api-memory-test.cpp:44` `const char* kokoro_lang_for_voice_stem(std::string_view stem)` -- Kokoro voice ids use a two-letter family prefix (e.g. af_alloy -> en_us).
- `sample_text_for_kokoro_lang` (function) `core/moonshine-c-api-memory-test.cpp:79` `const char* sample_text_for_kokoro_lang(const char* lang)`
- `append_files_under` (function) `core/moonshine-c-api-memory-test.cpp:110` `void append_files_under(
    const std::filesystem::path& root, const std::filesystem::path& sub,...` -- Subtrees needed for Kokoro + rule G2P (Spanish is rule-only; no lexicon files).
- `build_kokoro_g2p_memory_bundle` (function) `core/moonshine-c-api-memory-test.cpp:140` `void build_kokoro_g2p_memory_bundle(
    const std::filesystem::path& data_root,
    std::vector<...`
- `main` (function) `core/moonshine-c-api-memory-test.cpp:266` `int main(int argc, char** argv)`

## core/moonshine-c-api-test.cpp
Depends on: `core/moonshine-c-api.h`, `core/moonshine-utils/debug-utils.h`, `core/moonshine-utils/string-utils.h`
- `find_de_piper_voices_dir` (function) `core/moonshine-c-api-test.cpp:22` `std::filesystem::path find_de_piper_voices_dir()`
- `read_binary_file` (function) `core/moonshine-c-api-test.cpp:37` `std::vector<uint8_t> read_binary_file(const std::filesystem::path& p)`
- `find_moonshine_tts_data_dir` (function) `core/moonshine-c-api-test.cpp:48` `std::optional<std::filesystem::path> find_moonshine_tts_data_dir()` -- Resolve ``moonshine-tts/data`` for tests run from ``test-assets/``, repo root, or ``core/build``.
- `free_phonemes_output` (function) `core/moonshine-c-api-test.cpp:72` `void free_phonemes_output(const char* ipa)`
- `grapheme_phonemizer_smoke` (function) `core/moonshine-c-api-test.cpp:78` `void grapheme_phonemizer_smoke(const std::filesystem::path& data_root,
                          ...` -- Creates a phonemizer with ``g2p_root`` = *data_root*, runs ``text`` → IPA, frees output.
- `TEST_CASE` (function) `core/moonshine-c-api-test.cpp:110` `TEST_CASE("moonshine-test-v2")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:111` `SUBCASE("transcribe-complete")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:154` `SUBCASE("transcribe-stream")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:247` `SUBCASE("transcribe-complete-from-memory")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:313` `SUBCASE("transcribe-without-streaming-skip-transcription")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:357` `SUBCASE("transcribe-without-streaming-vad-threshold-0")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:407` `SUBCASE("transcribe-valid-options")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:438` `SUBCASE("transcribe-invalid-option")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:451` `SUBCASE("spelling-mode-flag-noop-without-model")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:478` `SUBCASE("spelling-mode-replaces-line-text")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:524` `SUBCASE("tts-synthesizer-valid-options")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:548` `SUBCASE("tts-synthesizer-per-call-speed-kokoro")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:597` `SUBCASE("tts-piper-german-from-memory")`
- `TEST_CASE` (function) `core/moonshine-c-api-test.cpp:657` `TEST_CASE("moonshine-phonemes-to-speech-c-api")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:658` `SUBCASE("invalid-handle")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:667` `SUBCASE("invalid-arguments")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:696` `SUBCASE("kokoro-matches-text-to-speech")`
- `TEST_CASE` (function) `core/moonshine-c-api-test.cpp:784` `TEST_CASE("grapheme-to-phonemizer-c-api")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:785` `SUBCASE("create-invalid-filenames-pointer")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:795` `SUBCASE("text-to-phonemes-invalid-handle")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:802` `SUBCASE("text-to-phonemes-invalid-arguments")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:829` `SUBCASE("rule-based-languages-smoke")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:868` `SUBCASE("chinese-when-onnx-bundle-present")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:885` `SUBCASE("japanese-when-onnx-bundle-present")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:904` `SUBCASE("arabic-when-onnx-bundle-present")`
- `TEST_CASE` (function) `core/moonshine-c-api-test.cpp:923` `TEST_CASE("moonshine-tts-g2p-dependency-api")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:924` `SUBCASE("null-output-pointer")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:933` `SUBCASE("options-count-without-options-pointer")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:943` `SUBCASE("g2p-empty-means-all-languages")`
- `csv` (function) `core/moonshine-c-api-test.cpp:948` `const std::string csv(out);`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:961` `SUBCASE("g2p-arabic-onnx-model-key-matches-meta-onnx-filename")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:974` `SUBCASE("g2p-french-lists-pos-csv-files-not-directory-prefix")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:988` `SUBCASE("g2p-single-language")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:997` `SUBCASE("g2p-unsupported-language")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1005` `SUBCASE("g2p-multiple-languages")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1017` `SUBCASE("g2p-appends-override-key-when-option-set")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1029` `SUBCASE("tts-json-single-language")`
- `json` (function) `core/moonshine-c-api-test.cpp:1034` `const std::string json(out);`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1044` `SUBCASE("tts-empty-all-languages-json")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1055` `SUBCASE("tts-unsupported-language")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1063` `SUBCASE("tts-multiple-languages")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1076` `SUBCASE("tts-piper-engine-on-en_us")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1090` `SUBCASE("tts-kokoro-engine-on-fr")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1104` `SUBCASE("tts-explicit-piper-onnx-map-keys")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1119` `SUBCASE("tts-piper-voice-selects-onnx-basename")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1132` `SUBCASE("tts-voices-json-object-en_us")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1155` `SUBCASE("tts-voices-kokoro-reports-missing-without-assets")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1169` `SUBCASE("tts-voices-unsupported-language")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1176` `SUBCASE("tts-voices-piper-de-includes-thorsten-stem")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1196` `SUBCASE("tts-voices-piper-en_us-includes-saikat-stem")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1216` `SUBCASE("tts-zipvoice-dependencies")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1234` `SUBCASE("tts-zipvoice-voices-listing")`
- `TEST_CASE` (function) `core/moonshine-c-api-test.cpp:1253` `TEST_CASE("moonshine-stt-intent-dependency-api")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1254` `SUBCASE("null-output-pointer")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1262` `SUBCASE("options-count-without-options-pointer")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1271` `SUBCASE("stt-empty-language-is-invalid")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1278` `SUBCASE("stt-english-default-is-medium-streaming")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1296` `SUBCASE("stt-english-tiny-non-streaming")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1317` `SUBCASE("stt-non-english-omits-attention-extra")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1334` `SUBCASE("stt-english-name-lookup")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1342` `SUBCASE("stt-include-spelling-adds-group-for-english")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1359` `SUBCASE("stt-include-spelling-noop-for-non-english")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1373` `SUBCASE("stt-unknown-language")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1381` `SUBCASE("stt-unknown-arch-for-language")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1391` `SUBCASE("stt-invalid-arch-value")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1401` `SUBCASE("intent-default-variant-is-q4")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1415` `SUBCASE("intent-null-model-name-uses-default")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1424` `SUBCASE("intent-q8-maps-to-model-quantized")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1441` `SUBCASE("intent-fp32-uses-bare-model-onnx")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1455` `SUBCASE("intent-unknown-model")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1462` `SUBCASE("intent-unknown-variant")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1498` `SUBCASE("builtin-voice-synthesizes-audio")`
- `SUBCASE` (function) `core/moonshine-c-api-test.cpp:1522` `SUBCASE("user-pcm-with-explicit-transcript")`
- `pcm` (function) `core/moonshine-c-api-test.cpp:1525` `std::vector<float> pcm(24000, 0.f);` -- A short synthetic reference clip (silence + tone) suffices to exercise the memory + clone path.

## core/moonshine-c-api.cpp
Depends on: `core/bin-tokenizer/bin-tokenizer.h`, `core/intent-recognizer.h`, `core/moonshine-c-api.h`, `core/moonshine-model-catalog.h`, `core/moonshine-model.h`, `core/moonshine-tts/src/moonshine-asset-catalog.h`, `core/moonshine-tts/src/moonshine-g2p.h`, `core/moonshine-tts/src/moonshine-tts.h`, `core/moonshine-utils/debug-utils.h`, `core/moonshine-utils/string-utils.h`, `core/ort-utils/moonshine-ort-allocator.h`, `core/ort-utils/moonshine-tensor-view.h`, `core/ort-utils/ort-utils.h`
- `parse_option_vector` (function) `core/moonshine-c-api.cpp:83` `OptionVector parse_option_vector(const moonshine_option_t *options,
                             ...`
- `parse_common_options` (function) `core/moonshine-c-api.cpp:98` `OptionVector parse_common_options(const OptionVector &options)` -- Handles common options that are not specific to any particular API.
- `parse_transcriber_options` (function) `core/moonshine-c-api.cpp:110` `void parse_transcriber_options(const OptionVector &options,
                               Transc...`
- `allocate_transcriber_handle` (function) `core/moonshine-c-api.cpp:171` `int32_t allocate_transcriber_handle(Transcriber *transcriber)`
- `free_transcriber_handle` (function) `core/moonshine-c-api.cpp:178` `void free_transcriber_handle(int32_t handle)`
- `moonshine_load_transcriber_from_memory` (function) `core/moonshine-c-api.cpp:240` `int32_t moonshine_load_transcriber_from_memory(
    const uint8_t *encoder_model_data, size_t enc...`
- `moonshine_free_transcriber` (function) `core/moonshine-c-api.cpp:291` `void moonshine_free_transcriber(int32_t transcriber_handle)`
- `moonshine_transcribe_without_streaming` (function) `core/moonshine-c-api.cpp:299` `int32_t moonshine_transcribe_without_streaming(
    int32_t transcriber_handle, float *audio_data...`
- `moonshine_create_stream` (function) `core/moonshine-c-api.cpp:322` `int32_t moonshine_create_stream(int32_t transcriber_handle, uint32_t flags)`
- `moonshine_free_stream` (function) `core/moonshine-c-api.cpp:336` `int32_t moonshine_free_stream(int32_t transcriber_handle,
                              int32_t s...`
- `moonshine_start_stream` (function) `core/moonshine-c-api.cpp:352` `int32_t moonshine_start_stream(int32_t transcriber_handle,
                               int32_t...`
- `moonshine_stop_stream` (function) `core/moonshine-c-api.cpp:368` `int32_t moonshine_stop_stream(int32_t transcriber_handle,
                              int32_t s...`
- `moonshine_transcript_to_string` (function) `core/moonshine-c-api.cpp:384` `const char *moonshine_transcript_to_string(
    const struct transcript_t *transcript)`
- `moonshine_transcribe_add_audio_to_stream` (function) `core/moonshine-c-api.cpp:394` `int32_t moonshine_transcribe_add_audio_to_stream(int32_t transcriber_handle,
                    ...`
- `moonshine_transcribe_stream` (function) `core/moonshine-c-api.cpp:420` `int32_t moonshine_transcribe_stream(int32_t transcriber_handle,
                                 ...`
- `allocate_intent_recognizer_handle` (function) `core/moonshine-c-api.cpp:448` `int32_t allocate_intent_recognizer_handle(IntentRecognizer *recognizer)`
- `free_intent_recognizer_handle` (function) `core/moonshine-c-api.cpp:455` `void free_intent_recognizer_handle(int32_t handle)`
- `duplicate_c_string` (function) `core/moonshine-c-api.cpp:471` `char *duplicate_c_string(const char *s)`
- `moonshine_create_intent_recognizer` (function) `core/moonshine-c-api.cpp:485` `int32_t moonshine_create_intent_recognizer(const char *model_path,
                              ...`
- `moonshine_free_intent_recognizer` (function) `core/moonshine-c-api.cpp:516` `void moonshine_free_intent_recognizer(int32_t intent_recognizer_handle)`
- `moonshine_register_intent` (function) `core/moonshine-c-api.cpp:527` `int32_t moonshine_register_intent(int32_t intent_recognizer_handle,
                             ...`
- `moonshine_unregister_intent` (function) `core/moonshine-c-api.cpp:553` `int32_t moonshine_unregister_intent(int32_t intent_recognizer_handle,
                           ...`
- `moonshine_get_closest_intents` (function) `core/moonshine-c-api.cpp:578` `int32_t moonshine_get_closest_intents(int32_t intent_recognizer_handle,
                         ...`
- `moonshine_free_intent_matches` (function) `core/moonshine-c-api.cpp:636` `void moonshine_free_intent_matches(moonshine_intent_match_t *matches,
                           ...`
- `moonshine_get_intent_count` (function) `core/moonshine-c-api.cpp:647` `int32_t moonshine_get_intent_count(int32_t intent_recognizer_handle)`
- `moonshine_clear_intents` (function) `core/moonshine-c-api.cpp:659` `int32_t moonshine_clear_intents(int32_t intent_recognizer_handle)`
- `moonshine_calculate_intent_embedding` (function) `core/moonshine-c-api.cpp:673` `int32_t moonshine_calculate_intent_embedding(int32_t intent_recognizer_handle,
                  ...`
- `moonshine_free_intent_embedding` (function) `core/moonshine-c-api.cpp:714` `void moonshine_free_intent_embedding(float *embedding)`
- `moonshine_calculate_embedding_distance` (function) `core/moonshine-c-api.cpp:716` `int32_t moonshine_calculate_embedding_distance(int32_t intent_recognizer_handle,
                ...`
- `a` (function) `core/moonshine-c-api.cpp:735` `std::vector<float> a(embedding_a, embedding_a + embedding_size);`
- `b` (function) `core/moonshine-c-api.cpp:736` `std::vector<float> b(embedding_b, embedding_b + embedding_size);`
- `allocate_text_to_speech_synthesizer_handle` (function) `core/moonshine-c-api.cpp:755` `int32_t allocate_text_to_speech_synthesizer_handle(
    moonshine_tts::MoonshineTTS *synthesizer)`
- `parse_tts_options` (function) `core/moonshine-c-api.cpp:763` `void parse_tts_options(const OptionVector &options,
                       moonshine_tts::Moonshi...`
- `maybe_autotranscribe_zipvoice_clone` (function) `core/moonshine-c-api.cpp:778` `void maybe_autotranscribe_zipvoice_clone(
    const OptionVector &options,
    moonshine_tts::Moo...` -- When the ZipVoice engine is selected with a caller-supplied clone reference clip (memory key...
- `pcm` (function) `core/moonshine-c-api.cpp:815` `std::vector<float> pcm(n);`
- `moonshine_create_tts_synthesizer_from_files` (function) `core/moonshine-c-api.cpp:870` `int32_t moonshine_create_tts_synthesizer_from_files(
    const char *language, const char **filen...`
- `moonshine_create_tts_synthesizer_from_memory` (function) `core/moonshine-c-api.cpp:911` `int32_t moonshine_create_tts_synthesizer_from_memory(
    const char *language, const char **file...`
- `key` (function) `core/moonshine-c-api.cpp:946` `const std::string key(filenames[i]);`
- `moonshine_free_tts_synthesizer` (function) `core/moonshine-c-api.cpp:1000` `void moonshine_free_tts_synthesizer(int32_t tts_synthesizer_handle)` -- Releases the resources used by a text to speech synthesizer.
- `moonshine_text_to_speech` (function) `core/moonshine-c-api.cpp:1041` `int32_t moonshine_text_to_speech(int32_t tts_synthesizer_handle,
                                ...` -- Synthesizes text to speech.
- `moonshine_phonemes_to_speech` (function) `core/moonshine-c-api.cpp:1089` `int32_t moonshine_phonemes_to_speech(int32_t tts_synthesizer_handle,
                            ...`
- `malloc_string_copy` (function) `core/moonshine-c-api.cpp:1144` `char *malloc_string_copy(const std::string &s)`
- `split_comma_nonempty_language_tokens` (function) `core/moonshine-c-api.cpp:1153` `std::vector<std::string> split_comma_nonempty_language_tokens(const char *s)`
- `append_unique_in_order` (function) `core/moonshine-c-api.cpp:1178` `void append_unique_in_order(std::vector<std::string> &acc,
                            const std:...`
- `json_utf8_string_literal` (function) `core/moonshine-c-api.cpp:1188` `std::string json_utf8_string_literal(const std::string &s)`
- `json_flat_string_array` (function) `core/moonshine-c-api.cpp:1230` `std::string json_flat_string_array(const std::vector<std::string> &items)`
- `json_model_dependencies` (function) `core/moonshine-c-api.cpp:1247` `std::string json_model_dependencies(const moonshine::ModelDependencies &deps)` -- Serializes a model download manifest as a JSON object with a "groups" array.
- `json_tts_voice_entry` (function) `core/moonshine-c-api.cpp:1264` `std::string json_tts_voice_entry(
    const moonshine_tts::MoonshineTtsVoiceAvailability &v)`
- `json_tts_voices_lang_array` (function) `core/moonshine-c-api.cpp:1274` `std::string json_tts_voices_lang_array(
    const std::vector<moonshine_tts::MoonshineTtsVoiceAva...`
- `json_tts_voices_root_object` (function) `core/moonshine-c-api.cpp:1288` `std::string json_tts_voices_root_object(
    const std::vector<std::pair<
        std::string, st...`
- `apply_g2p_dependency_query_c_options` (function) `core/moonshine-c-api.cpp:1306` `void apply_g2p_dependency_query_c_options(
    const moonshine_option_t *options, uint64_t option...`
- `append_g2p_explicit_override_keys_from_c_options` (function) `core/moonshine-c-api.cpp:1356` `void append_g2p_explicit_override_keys_from_c_options(
    const moonshine_option_t *options, uin...`
- `moonshine_get_g2p_dependencies` (function) `core/moonshine-c-api.cpp:1387` `int32_t moonshine_get_g2p_dependencies(const char *languages,
                                   ...`
- `moonshine_get_tts_dependencies` (function) `core/moonshine-c-api.cpp:1451` `int32_t moonshine_get_tts_dependencies(const char *languages,
                                   ...`
- `moonshine_get_tts_voices` (function) `core/moonshine-c-api.cpp:1548` `int32_t moonshine_get_tts_voices(const char *languages,
                                 const mo...`
- `normalize_option_key` (function) `core/moonshine-c-api.cpp:1654` `std::string normalize_option_key(const char *name)`
- `parse_int_option` (function) `core/moonshine-c-api.cpp:1662` `std::optional<int32_t> parse_int_option(const std::string &value)` -- Parses an integer option value; returns std::nullopt on empty/invalid input.
- `moonshine_get_stt_dependencies` (function) `core/moonshine-c-api.cpp:1681` `int32_t moonshine_get_stt_dependencies(const char *language,
                                    ...`
- `moonshine_get_intent_dependencies` (function) `core/moonshine-c-api.cpp:1743` `int32_t moonshine_get_intent_dependencies(const char *model_name,
                               ...`
- `allocate_grapheme_phonemizer_handle` (function) `core/moonshine-c-api.cpp:1802` `int32_t allocate_grapheme_phonemizer_handle(moonshine_tts::MoonshineG2P *g2p)`
- `parse_grapheme_phonemizer_options` (function) `core/moonshine-c-api.cpp:1809` `void parse_grapheme_phonemizer_options(
    const moonshine_option_t *in_options, uint64_t in_opt...`
- `finalize_g2p_options_for_phonemizer_create` (function) `core/moonshine-c-api.cpp:1846` `void finalize_g2p_options_for_phonemizer_create(
    moonshine_tts::MoonshineG2POptions &g2p_opt)`
- `moonshine_create_grapheme_to_phonemizer_from_files` (function) `core/moonshine-c-api.cpp:1869` `int32_t moonshine_create_grapheme_to_phonemizer_from_files(
    const char *language, const char ...` -- Creates a grapheme to phonemizer from files on disk.
- `moonshine_create_grapheme_to_phonemizer_from_memory` (function) `core/moonshine-c-api.cpp:1928` `int32_t moonshine_create_grapheme_to_phonemizer_from_memory(
    const char *language, const char...` -- Creates a grapheme to phonemizer from memory.
- `moonshine_free_grapheme_to_phonemizer` (function) `core/moonshine-c-api.cpp:1995` `void moonshine_free_grapheme_to_phonemizer(
    int32_t grapheme_to_phonemizer_handle)` -- Releases the resources used by a grapheme to phonemizer.
- `moonshine_text_to_phonemes` (function) `core/moonshine-c-api.cpp:2012` `int32_t moonshine_text_to_phonemes(int32_t grapheme_to_phonemizer_handle,
                       ...` -- Converts a text into the equivalent International Phonetic Alphabet (IPA) phonemes.

## core/moonshine-c-api.h
Imported by: `android/moonshine-jni/moonshine-jni.cpp`, `core/intent-recognizer-test.cpp`, `core/moonshine-c-api-memory-test.cpp`, `core/moonshine-c-api-test.cpp`, `core/moonshine-c-api.cpp`, `core/moonshine-cpp.h`, `core/moonshine-download-smoke.cpp`, `core/moonshine-model-catalog.cpp`, `core/moonshine-model.h`, `core/tts-repeated-memory-test.cpp`, `core/word-alignment-benchmark.cpp`, `core/word-alignment-test.cpp`
- `main` (function) `core/moonshine-c-api.h:38` `int main(int argc, char *argv[])`
- `moonshine_get_version` (function) `core/moonshine-c-api.h:286` `MOONSHINE_EXPORT int32_t moonshine_get_version(void);` -- Returns the loaded moonshine library version.
- `moonshine_error_to_string` (function) `core/moonshine-c-api.h:290` `MOONSHINE_EXPORT const char *moonshine_error_to_string(int32_t error);` -- Converts an error code number returned from an API call into a human-readable string.
- `moonshine_transcript_to_string` (function) `core/moonshine-c-api.h:295` `MOONSHINE_EXPORT const char *moonshine_transcript_to_string( const struct transcript_t *transcript);` -- Converts a transcript_t struct into a human-readable string for debugging purposes.
- `moonshine_load_transcriber_from_files` (function) `core/moonshine-c-api.h:357` `MOONSHINE_EXPORT int32_t moonshine_load_transcriber_from_files( const char *path, uint32_t model_arch, const struct...` -- ``MOONSHINE_FLAG_SPELLING_MODE``; if not set, the spelling model is not loaded and the flag is a no-op.
- `moonshine_free_transcriber` (function) `core/moonshine-c-api.h:388` `MOONSHINE_EXPORT void moonshine_free_transcriber(int32_t transcriber_handle);` -- Releases all resources used by the transcriber.
- `moonshine_transcribe_without_streaming` (function) `core/moonshine-c-api.h:425` `MOONSHINE_EXPORT int32_t moonshine_transcribe_without_streaming( int32_t transcriber_handle, float *audio_data...` -- to completed lines (requires the transcriber to have been loaded with a spelling model; otherwise the flag is a no-op).
- `moonshine_create_stream` (function) `core/moonshine-c-api.h:507` `MOONSHINE_EXPORT int32_t moonshine_create_stream(int32_t transcriber_handle, uint32_t flags);` -- Creates a stream.
- `moonshine_free_stream` (function) `core/moonshine-c-api.h:513` `MOONSHINE_EXPORT int32_t moonshine_free_stream(int32_t transcriber_handle, int32_t stream_handle);` -- Releases the resources used by a stream.
- `moonshine_start_stream` (function) `core/moonshine-c-api.h:524` `MOONSHINE_EXPORT int32_t moonshine_start_stream(int32_t transcriber_handle, int32_t stream_handle);` -- Starts a stream.
- `moonshine_stop_stream` (function) `core/moonshine-c-api.h:531` `MOONSHINE_EXPORT int32_t moonshine_stop_stream(int32_t transcriber_handle, int32_t stream_handle);` -- Stops a stream.
- `moonshine_transcribe_add_audio_to_stream` (function) `core/moonshine-c-api.h:564` `MOONSHINE_EXPORT int32_t moonshine_transcribe_add_audio_to_stream( int32_t transcriber_handle, int32_t...` -- `new_audio_data` should be a pointer to an array of PCM audio data, between -1.0 and 1.0, at a sample rate of...
- `moonshine_transcribe_stream` (function) `core/moonshine-c-api.h:597` `MOONSHINE_EXPORT int32_t moonshine_transcribe_stream( int32_t transcriber_handle, int32_t stream_handle, uint32_t...` -- `flags` should be a bitwise OR of flags.
- `moonshine_free_intent_recognizer` (function) `core/moonshine-c-api.h:638` `MOONSHINE_EXPORT void moonshine_free_intent_recognizer( int32_t intent_recognizer_handle);` -- `model_variant` specifies which model variant to load: "fp32", "fp16", "q8", "q4", or "q4f16".
- `moonshine_register_intent` (function) `core/moonshine-c-api.h:652` `MOONSHINE_EXPORT int32_t moonshine_register_intent( int32_t intent_recognizer_handle, const char *canonical_phrase...` -- Registers a canonical intent phrase (no callback).
- `moonshine_unregister_intent` (function) `core/moonshine-c-api.h:659` `MOONSHINE_EXPORT int32_t moonshine_unregister_intent( int32_t intent_recognizer_handle, const char *canonical_phrase);` -- Unregisters an intent by its canonical phrase.
- `moonshine_free_intent_matches` (function) `core/moonshine-c-api.h:685` `MOONSHINE_EXPORT void moonshine_free_intent_matches( struct moonshine_intent_match_t *matches, uint64_t count);` -- Frees an array returned by moonshine_get_closest_intents (safe on NULL / zero count).
- `moonshine_clear_intents` (function) `core/moonshine-c-api.h:698` `MOONSHINE_EXPORT int32_t moonshine_clear_intents(int32_t intent_recognizer_handle);`
- `moonshine_calculate_intent_embedding` (function) `core/moonshine-c-api.h:708` `MOONSHINE_EXPORT int32_t moonshine_calculate_intent_embedding( int32_t intent_recognizer_handle, const char...` -- Calculates the intent embedding for a given sentence.
- `moonshine_free_intent_embedding` (function) `core/moonshine-c-api.h:715` `MOONSHINE_EXPORT void moonshine_free_intent_embedding(float *embedding);` -- Frees an intent embedding returned by moonshine_calculate_intent_embedding.
- `moonshine_calculate_embedding_distance` (function) `core/moonshine-c-api.h:725` `MOONSHINE_EXPORT int32_t moonshine_calculate_embedding_distance( int32_t intent_recognizer_handle, const float...` -- Calculates the cosine similarity between two embedding vectors.
- `moonshine_create_tts_synthesizer_from_memory` (function) `core/moonshine-c-api.h:784` `MOONSHINE_EXPORT int32_t moonshine_create_tts_synthesizer_from_memory( const char *language, const char **filenames...` -- optionally, ``zipvoice_clone_transcript``.
- `moonshine_free_tts_synthesizer` (function) `core/moonshine-c-api.h:793` `MOONSHINE_EXPORT void moonshine_free_tts_synthesizer( int32_t tts_synthesizer_handle);` -- Releases the resources used by a text to speech synthesizer.
- `moonshine_get_g2p_dependencies` (function) `core/moonshine-c-api.h:813` `MOONSHINE_EXPORT int32_t moonshine_get_g2p_dependencies( const char *languages, const struct moonshine_option_t...` -- keys).
- `moonshine_get_tts_dependencies` (function) `core/moonshine-c-api.h:830` `MOONSHINE_EXPORT int32_t moonshine_get_tts_dependencies( const char *languages, const struct moonshine_option_t...` -- Returns merged G2P + TTS vocoder canonical asset keys as a JSON array of strings (flat list).
- `moonshine_get_tts_voices` (function) `core/moonshine-c-api.h:858` `MOONSHINE_EXPORT int32_t moonshine_get_tts_voices( const char *languages, const struct moonshine_option_t *options...` -- ``MoonshineTTSOptions::parse_options``).
- `moonshine_get_stt_dependencies` (function) `core/moonshine-c-api.h:892` `MOONSHINE_EXPORT int32_t moonshine_get_stt_dependencies( const char *language, const struct moonshine_option_t...` -- for the language, its files are appended as an extra group.
- `moonshine_get_intent_dependencies` (function) `core/moonshine-c-api.h:915` `MOONSHINE_EXPORT int32_t moonshine_get_intent_dependencies( const char *model_name, const struct moonshine_option_t...` -- ``"embeddinggemma-300m"``); pass NULL or an empty string to use the default model.
- `moonshine_text_to_speech` (function) `core/moonshine-c-api.h:929` `MOONSHINE_EXPORT int32_t moonshine_text_to_speech( int32_t tts_synthesizer_handle, const char *text, const struct...` -- Synthesizes text to speech.
- `moonshine_phonemes_to_speech` (function) `core/moonshine-c-api.h:953` `MOONSHINE_EXPORT int32_t moonshine_phonemes_to_speech( int32_t tts_synthesizer_handle, const char *phonemes, const...` -- grapheme-to-phonemizer created for the matching language).
- `moonshine_free_grapheme_to_phonemizer` (function) `core/moonshine-c-api.h:1013` `MOONSHINE_EXPORT void moonshine_free_grapheme_to_phonemizer( int32_t grapheme_to_phonemizer_handle);` -- Releases the resources used by a grapheme to phonemizer.
- `moonshine_text_to_phonemes` (function) `core/moonshine-c-api.h:1019` `MOONSHINE_EXPORT int32_t moonshine_text_to_phonemes( int32_t grapheme_to_phonemizer_handle, const char *text, const...` -- Converts a text into the equivalent International Phonetic Alphabet (IPA) phonemes.


Next: [API_p3.md](API_p3.md)
