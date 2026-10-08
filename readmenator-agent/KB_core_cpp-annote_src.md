# Subsystem: core_cpp-annote_src (page 1 of 2)
Pages: [KB_core_cpp-annote_src.md](KB_core_cpp-annote_src.md), [KB_core_cpp-annote_src_p2.md](KB_core_cpp-annote_src_p2.md)

## core/cpp-annote/src/annotation_support.h
- Doc: segment_union: Union (|): covers both segments including any gap between them.
- Layer: utility
- Language: h
- Symbols:
  - `Segment` (struct, line 24)
  - `empty` (function, line 28) `bool empty() const`
  - `duration` (function, line 30) `double duration() const`
  - `segment_union` (function, line 37) `inline Segment segment_union(const Segment& a, const Segment& b)`
  - `segment_gap` (function, line 49) `inline Segment segment_gap(const Segment& self_, const Segment& other)`
  - `timeline_support_sorted` (function, line 60) `inline std::vector<Segment> timeline_support_sorted(
    const std::vector<Segment>& segments, do...`
  - `sort` (function, line 66) `std::sort(segs.begin(), segs.end(), [](const Segment& x, const Segment& y)`
  - `ANNOTATION_SUPPORT_H_` (macro, line 10) `#define ANNOTATION_SUPPORT_H_`
- Imported by: `core/cpp-annote/src/cpp-annote.cpp`

## core/cpp-annote/src/clustering_vbx.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `row_normalize` (function, line 22) `void row_normalize(Eigen::MatrixXd& M)`
  - `cdist_cosine` (function, line 31) `void cdist_cosine(const Eigen::MatrixXd& X, const Eigen::MatrixXd& C,
                  Eigen::Ma...`
  - `kmeans_fit_predict` (function, line 50) `std::vector<int> kmeans_fit_predict(const Eigen::MatrixXd& Xnorm, int k,
                        ...`
  - `centroids_from_labels` (function, line 115) `Eigen::MatrixXd centroids_from_labels(const Eigen::MatrixXd& train,
                             ...`
  - `hungarian_maximize` (function, line 133) `void hungarian_maximize(const Eigen::MatrixXd& score,
                        std::vector<int>& a...`
  - `vbx_clustering_hard` (function, line 166) `void vbx_clustering_hard(const plda_vbx::PldaModel& plda,
                         const VbxClust...`
  - `r` (function, line 55) `std::vector<int> r(static_cast<std::size_t>(n));`
  - `uni` (function, line 60) `std::uniform_int_distribution<int> uni(0, n - 1);`
  - `best_labs` (function, line 62) `std::vector<int> best_labs(static_cast<std::size_t>(n), 0);`
  - `labels` (function, line 68) `std::vector<int> labels(static_cast<std::size_t>(n), 0);`
  - `cnt` (function, line 87) `std::vector<int> cnt(static_cast<std::size_t>(k), 0);`
  - `cost` (function, line 145) `std::vector<std::vector<double>> cost( static_cast<std::size_t>(m), std::vector<double>(static_cast<std::size_t>(m)...`
  - `xflat` (function, line 192) `std::vector<double> xflat( static_cast<std::size_t>(train_n.rows() * train_n.cols()));`
  - `fea_f` (function, line 357) `std::vector<float> fea_f(static_cast<size_t>(fea.rows() * fea.cols()));`
- Depends on: `core/cpp-annote/src/clustering_vbx.h`, `core/cpp-annote/src/filter_train.h`, `core/cpp-annote/src/hungarian.h`, `core/cpp-annote/src/parity_log.h`, `core/cpp-annote/src/scipy_linkage.h`

## core/cpp-annote/src/clustering_vbx.h
- Doc: vbx_clustering_hard: ``embeddings`` row-major ``(num_chunks * num_speakers * dim)``...
- Layer: utility
- Language: h
- Symbols:
  - `VbxClusteringParams` (struct, line 15)
  - `vbx_clustering_hard` (function, line 34) `void vbx_clustering_hard(const plda_vbx::PldaModel& plda, const VbxClusteringParams& pr, int num_chunks, int...`
  - `CLUSTERING_VBX_H_` (macro, line 6) `#define CLUSTERING_VBX_H_`
- Depends on: `core/cpp-annote/src/plda_vbx.h`
- Imported by: `core/cpp-annote/src/clustering_vbx.cpp`, `core/cpp-annote/src/cpp-annote-engine.h`, `core/cpp-annote/src/cpp-annote.cpp`

## core/cpp-annote/src/community1_cpp_annote_embedded.cpp
- Layer: utility
- Language: cpp

## core/cpp-annote/src/community1_cpp_annote_embedded.h
- Layer: utility
- Language: h
- Symbols:
  - `receptive_field_json` (variable, line 11) `extern const char receptive_field_json[];`
  - `receptive_field_json_size` (variable, line 12) `extern const std::size_t receptive_field_json_size;`
  - `pipeline_snapshot_json` (variable, line 13) `extern const char pipeline_snapshot_json[];`
  - `pipeline_snapshot_json_size` (variable, line 14) `extern const std::size_t pipeline_snapshot_json_size;`
  - `golden_speaker_bounds_json` (variable, line 15) `extern const char golden_speaker_bounds_json[];`
  - `golden_speaker_bounds_json_size` (variable, line 16) `extern const std::size_t golden_speaker_bounds_json_size;`
  - `xvec_mean1` (variable, line 18) `extern const double xvec_mean1[256];`
  - `xvec_mean2` (variable, line 19) `extern const float xvec_mean2[128];`
  - `xvec_lda` (variable, line 20) `extern const float xvec_lda[32768];`
  - `plda_mu` (variable, line 21) `extern const double plda_mu[128];`
  - `plda_tr` (variable, line 22) `extern const double plda_tr[16384];`
  - `plda_psi` (variable, line 23) `extern const double plda_psi[128];`
  - `COMMUNITY1_CPP_ANNOTE_EMBEDDED_H_` (macro, line 5) `#define COMMUNITY1_CPP_ANNOTE_EMBEDDED_H_`
- Imported by: `core/cpp-annote/src/cpp-annote.cpp`

## core/cpp-annote/src/community1_ort_embedded.cpp
- Layer: utility
- Language: cpp

## core/cpp-annote/src/community1_ort_embedded.h
- Layer: utility
- Language: h
- Symbols:
  - `segmentation_ort_data` (variable, line 10) `extern const unsigned char segmentation_ort_data[];`
  - `segmentation_ort_data_size` (variable, line 11) `extern const std::size_t segmentation_ort_data_size;`
  - `embedding_ort_data` (variable, line 13) `extern const unsigned char embedding_ort_data[];`
  - `embedding_ort_data_size` (variable, line 14) `extern const std::size_t embedding_ort_data_size;`
  - `segmentation_json` (variable, line 16) `extern const char segmentation_json[];`
  - `segmentation_json_size` (variable, line 17) `extern const std::size_t segmentation_json_size;`
  - `embedding_json` (variable, line 19) `extern const char embedding_json[];`
  - `embedding_json_size` (variable, line 20) `extern const std::size_t embedding_json_size;`
  - `COMMUNITY1_ORT_EMBEDDED_H_` (macro, line 4) `#define COMMUNITY1_ORT_EMBEDDED_H_`
- Imported by: `core/cpp-annote/src/cpp-annote.cpp`

## core/cpp-annote/src/compute_fbank.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `wespeaker_like_fbank` (function, line 13) `void wespeaker_like_fbank(float sample_hz, int num_mel_bins,
                          float fram...`
  - `scaled` (function, line 31) `std::vector<float> scaled(static_cast<std::size_t>(std::max(0, num_samples)));`
- Depends on: `core/cpp-annote/src/compute_fbank.h`

## core/cpp-annote/src/compute_fbank.h
- Doc: wespeaker_like_fbank: Mono waveform ``[-1,1]`` → log-fbank, shape ``(T * num_mel_bins)`` row-major.
- Layer: utility
- Language: h
- Symbols:
  - `wespeaker_like_fbank` (function, line 16) `void wespeaker_like_fbank(float sample_hz, int num_mel_bins, float frame_length_ms, float frame_shift_ms, const...`
  - `COMPUTE_FBANK_H_` (macro, line 6) `#define COMPUTE_FBANK_H_`
- Imported by: `core/cpp-annote/src/compute_fbank.cpp`, `core/cpp-annote/src/cpp-annote.cpp`, `core/cpp-annote/src/embedding_ort_infer.cpp`

## core/cpp-annote/src/cpp-annote-engine.h
- Layer: utility
- Language: h
- Symbols:
  - `DiarizationProfile` (struct, line 23)
  - `SegConfig` (struct, line 99)
  - `CppAnnoteEngine` (class, line 58)
  - `print` (function, line 33) `void print(std::ostream& os, const char* prefix = "  ") const`
  - `accumulate` (function, line 49) `void accumulate(const DiarizationProfile& o)`
  - `segmentation_model_sample_rate` (function, line 89) `int segmentation_model_sample_rate() const`
  - `segmentation_num_channels` (function, line 90) `int segmentation_num_channels() const`
  - `segmentation_chunk_num_samples` (function, line 91) `int segmentation_chunk_num_samples() const`
  - `segmentation_chunk_step_sec` (function, line 92) `double segmentation_chunk_step_sec() const`
  - `segmentation_chunk_duration_sec` (function, line 93) `double segmentation_chunk_duration_sec() const`
  - `seg_frames_per_chunk` (function, line 94) `int seg_frames_per_chunk() const`
  - `seg_classes` (function, line 95) `int seg_classes() const`
  - `embedding_dimension` (function, line 96) `int embedding_dimension() const`
  - `extract_chunk_audio` (function, line 73) `static std::vector<float> extract_chunk_audio(const float* audio, int64_t num_samples, int64_t offset, int...`
  - `run_segmentation_ort_single` (function, line 79) `std::vector<float> run_segmentation_ort_single(const float* chunk_buf);`
  - `run_embedding_ort_single` (function, line 81) `std::vector<float> run_embedding_ort_single(const float* chunk_mono, const float* seg_binarized);`
  - `init_config_and_models` (function, line 140) `void init_config_and_models(const std::string& embedding_onnx_path);`
  - `CPP_ANNOTE_ENGINE_H_` (macro, line 6) `#define CPP_ANNOTE_ENGINE_H_`
- Depends on: `core/cpp-annote/src/clustering_vbx.h`, `core/cpp-annote/src/cpp-annote.h`, `core/cpp-annote/src/plda_vbx.h`
- Imported by: `core/cpp-annote/src/cpp-annote-streaming.h`, `core/cpp-annote/src/cpp-annote.cpp`, `core/speaker-diarizer.cpp`

## core/cpp-annote/src/cpp-annote-streaming.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `segment_iou` (function, line 22) `double segment_iou(double a0, double a1, double b0, double b1)`
  - `turns_match` (function, line 31) `bool turns_match(const StreamingDiarizationTurn& a,
                 const StreamingDiarizationTu...`
  - `StreamingDiarizationSession` (function, line 40) `StreamingDiarizationSession::StreamingDiarizationSession(
    CppAnnoteEngine& engine, StreamingD...`
  - `start_session` (function, line 63) `void StreamingDiarizationSession::start_session()`
  - `cluster_overlap_margin_sec` (function, line 79) `double StreamingDiarizationSession::cluster_overlap_margin_sec() const`
  - `cluster_decode_margin_sec` (function, line 83) `double StreamingDiarizationSession::cluster_decode_margin_sec() const`
  - `active_cluster_window_start_sec` (function, line 93) `double StreamingDiarizationSession::active_cluster_window_start_sec() const`
  - `cluster_decode_window_start_sec` (function, line 100) `double StreamingDiarizationSession::cluster_decode_window_start_sec() const`
  - `abs_sample_offset_for_sec` (function, line 113) `int64_t StreamingDiarizationSession::abs_sample_offset_for_sec(double sec) const`
  - `evict_chunk_cache_if_needed` (function, line 121) `void StreamingDiarizationSession::evict_chunk_cache_if_needed()`
  - `trim_buffer_if_needed` (function, line 137) `void StreamingDiarizationSession::trim_buffer_if_needed()`
  - `cache_new_chunks` (function, line 168) `void StreamingDiarizationSession::cache_new_chunks()`
  - `add_audio_chunk` (function, line 200) `void StreamingDiarizationSession::add_audio_chunk(const float* pcm,
                             ...`
  - `carry_last_updated_times` (function, line 226) `void StreamingDiarizationSession::carry_last_updated_times(
    std::vector<StreamingDiarizationT...`
  - `append_frozen_turn_if_new` (function, line 250) `void StreamingDiarizationSession::append_frozen_turn_if_new(
    std::vector<StreamingDiarization...`
  - `relabel_active_turns` (function, line 261) `void StreamingDiarizationSession::relabel_active_turns(
    std::vector<StreamingDiarizationTurn>...`
  - `sort` (function, line 314) `std::sort(candidates.begin(), candidates.end(),
              [](const auto& a, const auto& b)`
  - `merge_frozen_and_active_turns` (function, line 343) `void StreamingDiarizationSession::merge_frozen_and_active_turns(
    std::vector<StreamingDiariza...`
  - `sort` (function, line 381) `std::sort(merged.begin(), merged.end(),
            [](const StreamingDiarizationTurn& a,
       ...`
  - `maybe_refresh` (function, line 395) `void StreamingDiarizationSession::maybe_refresh(bool force)`
  - `snapshot` (function, line 549) `StreamingDiarizationSnapshot StreamingDiarizationSession::snapshot() const`
  - `refresh_and_snapshot` (function, line 554) `StreamingDiarizationSnapshot
StreamingDiarizationSession::refresh_and_snapshot()`
  - `end_session` (function, line 561) `StreamingDiarizationSnapshot StreamingDiarizationSession::end_session()`
  - `chunk` (function, line 212) `std::vector<float> chunk(pcm, pcm + num_samples);`
  - `seg_out` (function, line 486) `std::vector<float> seg_out(static_cast<size_t>(C_full) * static_cast<size_t>(FK));`
  - `emb_all` (function, line 488) `std::vector<float> emb_all(static_cast<size_t>(C_full) * static_cast<size_t>(K) * static_cast<size_t>(dim)...`
- Depends on: `core/cpp-annote/src/cpp-annote-streaming.h`, `core/cpp-annote/src/wav_pcm_float32.h`

## core/cpp-annote/src/cpp-annote-streaming.h
- Doc: StreamingDiarizationSession: Session bound to a ``CppAnnoteEngine``; the engine must outlive the...
- Layer: utility
- Language: h
- Symbols:
  - `StreamingDiarizationConfig` (struct, line 20)
  - `StreamingDiarizationSnapshot` (struct, line 43)
  - `CachedChunk` (struct, line 102)
  - `StreamingDiarizationSession` (class, line 55)
  - `start_session` (function, line 60) `void start_session();`
  - `add_audio_chunk` (function, line 63) `void add_audio_chunk(const float* pcm, std::size_t num_samples, int sample_rate);`
  - `cache_new_chunks` (function, line 80) `private: void cache_new_chunks();`
  - `trim_buffer_if_needed` (function, line 81) `void trim_buffer_if_needed();`
  - `evict_chunk_cache_if_needed` (function, line 82) `void evict_chunk_cache_if_needed();`
  - `maybe_refresh` (function, line 83) `void maybe_refresh(bool force);`
  - `carry_last_updated_times` (function, line 84) `static void carry_last_updated_times( std::vector<StreamingDiarizationTurn>& next, const...`
  - `append_frozen_turn_if_new` (function, line 87) `static void append_frozen_turn_if_new( std::vector<StreamingDiarizationTurn>& frozen, const...`
  - `merge_frozen_and_active_turns` (function, line 90) `void merge_frozen_and_active_turns( std::vector<StreamingDiarizationTurn> active_turns);`
  - `relabel_active_turns` (function, line 95) `void relabel_active_turns(std::vector<StreamingDiarizationTurn>& active_turns);`
  - `cluster_overlap_margin_sec` (function, line 96) `double cluster_overlap_margin_sec() const;`
  - `cluster_decode_margin_sec` (function, line 97) `double cluster_decode_margin_sec() const;`
  - `active_cluster_window_start_sec` (function, line 98) `double active_cluster_window_start_sec() const;`
  - `cluster_decode_window_start_sec` (function, line 99) `double cluster_decode_window_start_sec() const;`
  - `abs_sample_offset_for_sec` (function, line 100) `int64_t abs_sample_offset_for_sec(double sec) const;`
  - `CPP_ANNOTE_STREAMING_H_` (macro, line 8) `#define CPP_ANNOTE_STREAMING_H_`
- Depends on: `core/cpp-annote/src/cpp-annote-engine.h`
- Imported by: `core/cpp-annote/src/cpp-annote-streaming.cpp`, `core/cpp-annote/src/cpp-annote.cpp`, `core/speaker-diarizer.cpp`

## core/cpp-annote/src/cpp-annote.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `json_double` (function, line 40) `double json_double(const std::string &json, const char *key)`
  - `json_bool` (function, line 50) `bool json_bool(const std::string &json, const char *key)`
  - `closest_frame` (function, line 60) `int closest_frame(double t, double sw_start, double sw_duration,
                  double sw_step)`
  - `trim_warmup_inplace` (function, line 66) `void trim_warmup_inplace(std::vector<float> &data, size_t num_chunks,
                         si...`
  - `inference_aggregate` (function, line 93) `void inference_aggregate(const std::vector<float> &scores, size_t num_chunks,
                   ...`
  - `speaker_count_initial_uint8` (function, line 166) `std::vector<std::uint8_t> speaker_count_initial_uint8(
    std::vector<float> binarized, size_t n...`
  - `cap_count` (function, line 198) `std::vector<std::int8_t> cap_count(const std::vector<std::uint8_t> &u8,
                         ...`
  - `crop_loose_frame_range` (function, line 208) `void crop_loose_frame_range(double focus_start, double focus_end,
                            dou...`
  - `extent_of_frames` (function, line 219) `void extent_of_frames(double sw_start, double sw_step, size_t n_rows,
                      doubl...`
  - `crop_feature_loose` (function, line 225) `void crop_feature_loose(const std::vector<float> &data, int n_samples,
                        in...`
  - `argsort_desc_stable` (function, line 256) `std::vector<int> argsort_desc_stable(const float *row, int k)`
  - `stable_sort` (function, line 259) `std::stable_sort(idx.begin(), idx.end(), [row](int a, int b)`
  - `reconstruct_to_diarization` (function, line 268) `std::vector<float> reconstruct_to_diarization(
    const std::vector<float> &segmentations, int C...`
  - `binarize_column` (function, line 401) `void binarize_column(const float *k_scores, int num_frames, double sw_start,
                    ...`
  - `try_regex_double` (function, line 437) `bool try_regex_double(const std::string &json, const std::string &key_esc,
                      ...`
  - `filter_min_duration_on` (function, line 449) `void filter_min_duration_on(std::vector<std::pair<double, double>> &regs,
                       ...`
  - `try_json_bool_field` (function, line 463) `bool try_json_bool_field(const std::string &json, const char *key_esc,
                         b...`
  - `try_regex_int` (function, line 476) `bool try_regex_int(const std::string &json, const std::string &key_esc,
                   int &out)`
  - `make_segmentation_session` (function, line 490) `Ort::Session make_segmentation_session(Ort::Env &env,
                                       Ort:...`
  - `make_embedding_session` (function, line 504) `std::unique_ptr<Ort::Session> make_embedding_session(
    Ort::Env &env, Ort::SessionOptions &opt...`
  - `init_config_and_models` (function, line 515) `void CppAnnoteEngine::init_config_and_models(
    const std::string &embedding_onnx_path)`
  - `in_name_` (function, line 611) `in_name_(session_.GetInputNameAllocated(0, alloc_)),
      out_name_(session_.GetOutputNameAlloca...`
  - `in_name_` (function, line 624) `in_name_(session_.GetInputNameAllocated(0, alloc_)),
      out_name_(session_.GetOutputNameAlloca...`
  - `extract_chunk_audio` (function, line 633) `std::vector<float> CppAnnoteEngine::extract_chunk_audio(const float *audio,
                     ...`
  - `run_segmentation_ort_single` (function, line 653) `std::vector<float> CppAnnoteEngine::run_segmentation_ort_single(
    const float *chunk_buf)`
  - `run_embedding_ort_single` (function, line 682) `std::vector<float> CppAnnoteEngine::run_embedding_ort_single(
    const float *chunk_mono, const ...`
  - `cluster_and_decode` (function, line 753) `std::vector<DiarizationTurn> CppAnnoteEngine::cluster_and_decode(
    const std::vector<float> &s...`
  - `sort` (function, line 893) `std::sort(turns.begin(), turns.end(),
            [](const DiarizationTurn &a, const DiarizationT...`
  - `write_json` (function, line 915) `void DiarizationResults::write_json(std::ostream &os) const`
  - `write_json` (function, line 931) `void DiarizationResults::write_json(const std::string &path) const`
  - `Impl` (function, line 950) `Impl() : engine()`
  - `Impl` (function, line 951) `Impl(const std::string& seg_path, const std::string& emb_path)
      : engine(seg_path, emb_path)`
  - `get_stream` (function, line 954) `StreamingDiarizationSession &get_stream(int32_t id)`
  - `to_results` (function, line 963) `static DiarizationResults to_results(
      const StreamingDiarizationSnapshot &snap)`
  - `CppAnnote` (function, line 974) `CppAnnote::CppAnnote() : impl_(std::make_unique<Impl>())`
  - `CppAnnote` (function, line 976) `CppAnnote::CppAnnote(const std::string& segmentation_onnx_path,
                      const std::...`
  - `create_stream` (function, line 985) `int32_t CppAnnote::create_stream(double cluster_cadence,
                                 double ...`
  - `free_stream` (function, line 997) `void CppAnnote::free_stream(int32_t stream_id)`
  - `start_stream` (function, line 1002) `void CppAnnote::start_stream(int32_t stream_id)`
  - `stop_stream` (function, line 1006) `DiarizationResults CppAnnote::stop_stream(int32_t stream_id)`
  - `add_audio_to_stream` (function, line 1011) `void CppAnnote::add_audio_to_stream(int32_t stream_id, const float *audio_data,
                 ...`
  - `diarize` (function, line 1019) `DiarizationResults CppAnnote::diarize(const float *audio_data,
                                  ...`
  - `diarize_stream` (function, line 1033) `DiarizationResults CppAnnote::diarize_stream(int32_t stream_id)`
  - `out` (function, line 78) `std::vector<float> out(num_chunks * new_frames * num_classes);`
  - `agg` (function, line 113) `std::vector<float> agg(static_cast<size_t>(num_out_frames) * num_classes, 0.f);`
  - `occ` (function, line 115) `std::vector<float> occ(static_cast<size_t>(num_out_frames) * num_classes, 0.f);`
  - `mask_max` (function, line 117) `std::vector<float> mask_max(static_cast<size_t>(num_out_frames) * num_classes, 0.f);`
  - `summed` (function, line 174) `std::vector<float> summed(num_chunks * nf * 1);`
  - `idx` (function, line 257) `std::vector<int> idx(static_cast<size_t>(k));`
  - `clustered` (function, line 283) `std::vector<float> clustered(static_cast<size_t>(C) * static_cast<size_t>(F) * static_cast<size_t>(num_clusters)...`
  - `seen_k` (function, line 291) `std::vector<char> seen_k(static_cast<size_t>(num_clusters), 0);`
  - `padded` (function, line 345) `std::vector<float> padded( static_cast<size_t>(T) * static_cast<size_t>(max_spf), 0.f);`
  - `cnt_2d` (function, line 370) `std::vector<float> cnt_2d(static_cast<size_t>(Tcnt));`
  - `binary` (function, line 383) `std::vector<float> binary( static_cast<size_t>(act_rows) * static_cast<size_t>(K), 0.f);`
  - `ts` (function, line 408) `std::vector<double> ts(static_cast<size_t>(num_frames));`
  - `seg_json` (function, line 517) `const std::string seg_json( cppannote::embedded_community1::segmentation_json...`
  - `rf_txt` (function, line 536) `const std::string rf_txt( cppannote::embedded_community1::receptive_field_json...`
  - `sj` (function, line 543) `const std::string sj( cppannote::embedded_community1::pipeline_snapshot_json...`
  - `emb_json` (function, line 566) `const std::string emb_json( cppannote::embedded_community1::embedding_json...`
  - `buf` (function, line 638) `std::vector<float> buf(static_cast<size_t>(num_channels) * static_cast<size_t>(chunk_num_samples), 0.f);`
  - `chunk_for_fbank` (function, line 694) `std::vector<float> chunk_for_fbank(chunk_mono, chunk_mono + chunk_num_samples);`
  - `result` (function, line 722) `std::vector<float> result(static_cast<size_t>(K) * static_cast<size_t>(dim));`
  - `clean_col` (function, line 724) `std::vector<float> clean_col(static_cast<size_t>(F), 0.f);`
  - `full_col` (function, line 725) `std::vector<float> full_col(static_cast<size_t>(F), 0.f);`
  - `col` (function, line 859) `std::vector<float> col(static_cast<size_t>(rows));`
- Depends on: `core/cpp-annote/src/annotation_support.h`, `core/cpp-annote/src/clustering_vbx.h`, `core/cpp-annote/src/community1_cpp_annote_embedded.h`, `core/cpp-annote/src/community1_ort_embedded.h`, `core/cpp-annote/src/compute_fbank.h`, `core/cpp-annote/src/cpp-annote-engine.h`, `core/cpp-annote/src/cpp-annote-streaming.h`, `core/cpp-annote/src/cpp-annote.h`, `core/cpp-annote/src/embedding_ort_infer.h`, `core/cpp-annote/src/parity_log.h`, `core/cpp-annote/src/plda_vbx.h`, `core/cpp-annote/src/wav_pcm_float32.h`

## core/cpp-annote/src/cpp-annote.h
- Doc: CppAnnote: Loads segmentation and embedding ORT models from compiled-in data and manages...
- Layer: utility
- Language: h
- Symbols:
  - `DiarizationTurn` (struct, line 16)
  - `DiarizationResults` (struct, line 22)
  - `Impl` (struct, line 81)
  - `CppAnnote` (class, line 33)
  - `write_json` (function, line 25) `void write_json(const std::string &path) const;`
  - `create_stream` (function, line 58) `int32_t create_stream(double cluster_cadence = 2.0, double analyze_cadence = 0.0);`
  - `free_stream` (function, line 62) `void free_stream(int32_t stream_id);`
  - `start_stream` (function, line 65) `void start_stream(int32_t stream_id);`
  - `add_audio_to_stream` (function, line 73) `void add_audio_to_stream(int32_t stream_id, const float *audio_data, uint64_t audio_length, int32_t sample_rate);`
  - `CPP_ANNOTE_H_` (macro, line 7) `#define CPP_ANNOTE_H_`
- Imported by: `core/cpp-annote/src/cpp-annote-engine.h`, `core/cpp-annote/src/cpp-annote.cpp`

## core/cpp-annote/src/embedding_ort_infer.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `any_non_finite_embedding` (function, line 16) `bool any_non_finite_embedding(const float* e, int dim)`
  - `embedding_json_inputs_fbank_first` (function, line 27) `bool embedding_json_inputs_fbank_first(const std::string& emb_json)`
  - `run_embedding_ort` (function, line 40) `void run_embedding_ort(Ort::Session& sess, Ort::MemoryInfo& mem,
                       Ort::Allo...`
  - `discover_min_num_samples_embedding` (function, line 78) `int discover_min_num_samples_embedding(Ort::Session& sess, Ort::MemoryInfo& mem,
                ...`
  - `fbank_num_frames_for_samples` (function, line 115) `int fbank_num_frames_for_samples(int embed_sr, int mel_bins, float fl_ms,
                       ...`
  - `seg_to_fbank_nearest_index` (function, line 130) `int seg_to_fbank_nearest_index(int tf, int num_seg_frames,
                               int num...`
  - `noise` (function, line 87) `std::vector<float> noise(static_cast<size_t>(middle));`
  - `wts` (function, line 102) `std::vector<float> wts(static_cast<size_t>(Tf), 1.f);`
  - `emb` (function, line 103) `std::vector<float> emb(static_cast<size_t>(embed_dim));`
- Depends on: `core/cpp-annote/src/compute_fbank.h`, `core/cpp-annote/src/embedding_ort_infer.h`

## core/cpp-annote/src/embedding_ort_infer.h
- Layer: utility
- Language: h
- Symbols:
  - `embedding_json_inputs_fbank_first` (function, line 14) `bool embedding_json_inputs_fbank_first(const std::string& emb_json);`
  - `run_embedding_ort` (function, line 16) `void run_embedding_ort(Ort::Session& sess, Ort::MemoryInfo& mem, Ort::AllocatorWithDefaultOptions& alloc, bool...`
  - `discover_min_num_samples_embedding` (function, line 22) `int discover_min_num_samples_embedding(Ort::Session& sess, Ort::MemoryInfo& mem, Ort::AllocatorWithDefaultOptions&...`
  - `fbank_num_frames_for_samples` (function, line 28) `int fbank_num_frames_for_samples(int embed_sr, int mel_bins, float fl_ms, float fs_ms, int num_samples);`
  - `seg_to_fbank_nearest_index` (function, line 31) `int seg_to_fbank_nearest_index(int tf, int num_seg_frames, int num_fbank_frames);`
  - `EMBEDDING_ORT_INFER_H_` (macro, line 6) `#define EMBEDDING_ORT_INFER_H_`
- Imported by: `core/cpp-annote/src/cpp-annote.cpp`, `core/cpp-annote/src/embedding_ort_infer.cpp`

## core/cpp-annote/src/filter_train.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `filter_embeddings_train` (function, line 10) `void filter_embeddings_train(int num_chunks, int num_frames, int num_speakers,
                  ...`
- Depends on: `core/cpp-annote/src/filter_train.h`

## core/cpp-annote/src/filter_train.h
- Doc: filter_embeddings_train: Row-major ``embeddings`` length ``num_chunks * num_speakers * dim``...
- Layer: utility
- Language: h
- Symbols:
  - `filter_embeddings_train` (function, line 15) `void filter_embeddings_train(int num_chunks, int num_frames, int num_speakers, int dim, const float* embeddings...`
  - `FILTER_TRAIN_H_` (macro, line 5) `#define FILTER_TRAIN_H_`
- Imported by: `core/cpp-annote/src/clustering_vbx.cpp`, `core/cpp-annote/src/filter_train.cpp`

## core/cpp-annote/src/hungarian.h
- Layer: utility
- Language: h
- Symbols:
  - `u` (function, line 29) `std::vector<double> u(big_n, 0.0);`
  - `v` (function, line 30) `std::vector<double> v(big_m, 0.0);`
  - `p` (function, line 31) `std::vector<int> p(big_m, 0);`
  - `way` (function, line 32) `std::vector<int> way(big_m, 0);`
  - `minv` (function, line 36) `std::vector<double> minv(big_m, inf);`
  - `used` (function, line 37) `std::vector<char> used(big_m, 0);`
  - `assignment` (function, line 75) `std::vector<int> assignment(static_cast<std::size_t>(n), -1);`
  - `HUNGARIAN_H_` (macro, line 6) `#define HUNGARIAN_H_`
- Imported by: `core/cpp-annote/src/clustering_vbx.cpp`

## core/cpp-annote/src/parity_log.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `env_parity_level` (function, line 19) `int env_parity_level()`
  - `env_parity_out_dir` (function, line 33) `const char* env_parity_out_dir()`
  - `log_light` (function, line 41) `void log_light(const std::string& line)`
  - `heavy_dumps_enabled` (function, line 47) `bool heavy_dumps_enabled()`
  - `ensure_parity_out_dir` (function, line 51) `void ensure_parity_out_dir()`
  - `parity_clustering_npz_path` (function, line 64) `std::string parity_clustering_npz_path()`
  - `fingerprint_float32` (function, line 74) `std::string fingerprint_float32(const float* data, std::size_t n,
                               ...`
- Depends on: `core/cpp-annote/src/parity_log.h`

## core/cpp-annote/src/parity_log.h
- Doc: env_parity_level: ``PYANNOTE_CPP_PARITY``: unset or ``0`` = off; ``1`` = stderr light log; ``2``...
- Layer: utility
- Language: h
- Symbols:
  - `env_parity_level` (function, line 16) `int env_parity_level();`
  - `env_parity_out_dir` (function, line 20) `const char* env_parity_out_dir();`
  - `log_light` (function, line 23) `void log_light(const std::string& line);`
  - `heavy_dumps_enabled` (function, line 26) `bool heavy_dumps_enabled();`
  - `ensure_parity_out_dir` (function, line 29) `void ensure_parity_out_dir();`
  - `PARITY_LOG_H_` (macro, line 6) `#define PARITY_LOG_H_`
- Imported by: `core/cpp-annote/src/clustering_vbx.cpp`, `core/cpp-annote/src/cpp-annote.cpp`, `core/cpp-annote/src/parity_log.cpp`

## core/cpp-annote/src/plda_vbx.cpp
- Doc: load: The upstream file-based PldaModel::load() (cnpy NPZ loading) is removed in this vendored...
- Layer: utility
- Language: cpp
- Symbols:
  - `align_eigen_evecs_to_scipy_wccn_row0_for_community1_plda` (function, line 67) `void align_eigen_evecs_to_scipy_wccn_row0_for_community1_plda(
    const RowMatrixXd& tr_file, Ei...`
  - `row_l2_normalize` (function, line 88) `void row_l2_normalize(Eigen::MatrixXd& M)`
  - `logsumexp_rowwise` (function, line 97) `void logsumexp_rowwise(const Eigen::MatrixXd& M, Eigen::VectorXd& lse,
                       Eig...`
  - `load_from_arrays` (function, line 118) `void PldaModel::load_from_arrays(const double* mean1_p, int n_mean1,
                            ...`
  - `load` (function, line 161) `void PldaModel::load(const std::string& xvec_transform_npz,
                     const std::strin...`
  - `xvec_tf` (function, line 257) `Eigen::MatrixXd PldaModel::xvec_tf(const Eigen::MatrixXd& embeddings) const`
  - `plda_tf` (function, line 272) `Eigen::MatrixXd PldaModel::plda_tf(const Eigen::MatrixXd& x0,
                                   ...`
  - `operator` (function, line 282) `Eigen::MatrixXd PldaModel::operator()(const Eigen::MatrixXd& embeddings) const`
  - `softmax_rows` (function, line 286) `void softmax_rows(const Eigen::MatrixXd& logits, Eigen::MatrixXd& out)`
  - `cluster_vbx` (function, line 299) `void cluster_vbx(const std::vector<int>& ahc_init, const Eigen::MatrixXd& fea,
                 c...`
- Depends on: `core/cpp-annote/src/plda_vbx.h`

## core/cpp-annote/src/plda_vbx.h
- Doc: load_from_arrays: Load from raw NumPy-export tensors (same layout as HF ``xvec_transform.npz`` /...
- Layer: utility
- Language: h
- Symbols:
  - `PldaModel` (struct, line 16)
  - `load_from_arrays` (function, line 34) `void load_from_arrays(const double* mean1, int n_mean1, const float* mean2, int n_mean2, const float* lda, int...`
  - `softmax_rows` (function, line 44) `void softmax_rows(const Eigen::MatrixXd& logits, Eigen::MatrixXd& out);`
  - `cluster_vbx` (function, line 52) `void cluster_vbx(const std::vector<int>& ahc_init, const Eigen::MatrixXd& fea, const Eigen::VectorXd& Phi, double...`
  - `PLDA_VBX_H_` (macro, line 5) `#define PLDA_VBX_H_`
- Imported by: `core/cpp-annote/src/clustering_vbx.h`, `core/cpp-annote/src/cpp-annote-engine.h`, `core/cpp-annote/src/cpp-annote.cpp`, `core/cpp-annote/src/plda_vbx.cpp`

## core/cpp-annote/src/scipy_linkage.cpp
- Layer: utility
- Language: cpp
- Symbols:
  - `centroid_update` (function, line 16) `inline double centroid_update(double d_xi, double d_yi, double d_xy, int size_x,
                ...`
  - `is_visited` (function, line 34) `inline bool is_visited(const std::vector<unsigned char>& bitset, int i)`
  - `set_visited` (function, line 39) `inline void set_visited(std::vector<unsigned char>& bitset, int i)`
  - `visited_bytes` (function, line 44) `inline int visited_bytes(int n)`
  - `get_max_dist_for_each_cluster` (function, line 46) `void get_max_dist_for_each_cluster(const double* Z, int n,
                                   std...`
  - `cluster_monocrit` (function, line 93) `void cluster_monocrit(const double* Z, int n, const std::vector<double>& MC,
                    ...`
  - `pdist_euclidean` (function, line 151) `void pdist_euclidean(const std::vector<double>& X, int n, int d,
                     std::vector...`
  - `linkage_centroid_naive` (function, line 169) `void linkage_centroid_naive(const std::vector<double>& dist, int n,
                            s...`
  - `fcluster_distance` (function, line 237) `void fcluster_distance(const std::vector<double>& Z, int n, double cutoff,
                      ...`
  - `remap_labels_contiguous` (function, line 244) `void remap_labels_contiguous(const std::vector<int>& labels_one_based,
                          ...`
  - `curr_node` (function, line 49) `std::vector<int> curr_node(static_cast<std::size_t>(n));`
  - `visited` (function, line 50) `std::vector<unsigned char> visited(static_cast<std::size_t>(visited_bytes(n)), 0);`
  - `id_map` (function, line 173) `std::vector<int> id_map(static_cast<std::size_t>(n));`
  - `z` (function, line 247) `std::vector<int> z(static_cast<std::size_t>(n));`
- Depends on: `core/cpp-annote/src/scipy_linkage.h`

## core/cpp-annote/src/scipy_linkage.h
- Doc: pdist_euclidean: Row-major `X`: `n` rows, `d` cols → condensed pairwise Euclidean distances...
- Layer: utility
- Language: h
- Symbols:
  - `condensed_index` (function, line 14) `inline std::size_t condensed_index(int n, int i, int j)`
  - `pdist_euclidean` (function, line 23) `void pdist_euclidean(const std::vector<double>& X, int n, int d, std::vector<double>& dist);`
  - `linkage_centroid_naive` (function, line 29) `void linkage_centroid_naive(const std::vector<double>& dist, int n, std::vector<double>& Z);`
  - `fcluster_distance` (function, line 35) `void fcluster_distance(const std::vector<double>& Z, int n, double cutoff, std::vector<int>& T);`
  - `remap_labels_contiguous` (function, line 39) `void remap_labels_contiguous(const std::vector<int>& labels_one_based, std::vector<int>& out);`
  - `SCIPY_LINKAGE_H_` (macro, line 6) `#define SCIPY_LINKAGE_H_`
- Imported by: `core/cpp-annote/src/clustering_vbx.cpp`, `core/cpp-annote/src/scipy_linkage.cpp`


Next: [KB_core_cpp-annote_src_p2.md](KB_core_cpp-annote_src_p2.md)
