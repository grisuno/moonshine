# core/cpp-annote/src

*Community 5 | 27 files | cohesion 0.95*

## Definition

This community groups 27 file(s) rooted at `core/cpp-annote/src` with dominant language h (cohesion 0.95). Central symbols: `ANNOTATION_SUPPORT_H_`, `CLUSTERING_VBX_H_`, `COMMUNITY1_CPP_ANNOTE_EMBEDDED_H_`, `COMMUNITY1_ORT_EMBEDDED_H_`, `COMPUTE_FBANK_H_`, `CPP_ANNOTE_ENGINE_H_`, `CPP_ANNOTE_H_`, `CPP_ANNOTE_STREAMING_H_`. Core file: `core/cpp-annote/src/cpp-annote.cpp` (65 symbols). Documented purpose: libFuzzer harness for the WAV/RIFF parsers.  Both readers take a file path, so we write the fuzz input to a temporary file and parse it with (1) the first-party.

## Files

### `core/cpp-annote/src` (24 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `core/cpp-annote/src/annotation_support.h` | h | utility | 8 | yes |
| `core/cpp-annote/src/clustering_vbx.cpp` | cpp | utility | 14 | yes |
| `core/cpp-annote/src/clustering_vbx.h` | h | utility | 3 | yes |
| `core/cpp-annote/src/community1_cpp_annote_embedded.h` | h | utility | 13 | yes |
| `core/cpp-annote/src/community1_ort_embedded.h` | h | utility | 9 | yes |
| `core/cpp-annote/src/compute_fbank.cpp` | cpp | utility | 2 | yes |
| `core/cpp-annote/src/compute_fbank.h` | h | utility | 2 | yes |
| `core/cpp-annote/src/cpp-annote-engine.h` | h | utility | 18 | yes |
| `core/cpp-annote/src/cpp-annote-streaming.cpp` | cpp | utility | 26 | yes |
| `core/cpp-annote/src/cpp-annote-streaming.h` | h | utility | 20 | yes |
| `core/cpp-annote/src/cpp-annote.cpp` | cpp | utility | 65 | yes |
| `core/cpp-annote/src/cpp-annote.h` | h | utility | 10 | yes |
| `core/cpp-annote/src/embedding_ort_infer.cpp` | cpp | utility | 9 | yes |
| `core/cpp-annote/src/embedding_ort_infer.h` | h | utility | 6 | yes |
| `core/cpp-annote/src/filter_train.cpp` | cpp | utility | 1 | yes |
| `core/cpp-annote/src/filter_train.h` | h | utility | 2 | yes |
| `core/cpp-annote/src/hungarian.h` | h | utility | 8 | yes |

### `core` (2 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `core/speaker-diarizer.cpp` | cpp | utility | 16 | no |
| `core/speaker-diarizer.h` | h | utility | 9 | yes |

### `core/reliability` (1 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `core/reliability/fuzz-wav-pcm.cpp` | cpp | utility | 0 | yes |

*... and 7 more files in this community.*


## Key Symbols

- `ANNOTATION_SUPPORT_H_` (macro, `core/cpp-annote/src/annotation_support.h:10`) `#define ANNOTATION_SUPPORT_H_`
- `Segment` (struct, `core/cpp-annote/src/annotation_support.h:24`)
- `empty` (function, `core/cpp-annote/src/annotation_support.h:28`) `bool empty() const`
- `duration` (function, `core/cpp-annote/src/annotation_support.h:30`) `double duration() const`
- `segment_union` (function, `core/cpp-annote/src/annotation_support.h:37`) `inline Segment segment_union(const Segment& a, const Segment& b)` - Union (\|): covers both segments including any gap between them.
- `segment_gap` (function, `core/cpp-annote/src/annotation_support.h:49`) `inline Segment segment_gap(const Segment& self_, const Segment& other)` - Gap (^): self is first operand, other is second (matches Python `self ^ other`).
- `timeline_support_sorted` (function, `core/cpp-annote/src/annotation_support.h:60`) `inline std::vector<Segment> timeline_support_sorted(     const std::vector<Segme` - Timeline.support_iter / Timeline.support(collar) `segments` must be sorted by increasing start (Time
- `sort` (function, `core/cpp-annote/src/annotation_support.h:66`) `std::sort(segs.begin(), segs.end(), [](const Segment& x, const Segment& y)`
- `row_normalize` (function, `core/cpp-annote/src/clustering_vbx.cpp:22`) `void row_normalize(Eigen::MatrixXd& M)`
- `cdist_cosine` (function, `core/cpp-annote/src/clustering_vbx.cpp:31`) `void cdist_cosine(const Eigen::MatrixXd& X, const Eigen::MatrixXd& C,`
- `kmeans_fit_predict` (function, `core/cpp-annote/src/clustering_vbx.cpp:50`) `std::vector<int> kmeans_fit_predict(const Eigen::MatrixXd& Xnorm, int k,`
- `r` (function, `core/cpp-annote/src/clustering_vbx.cpp:55`) `std::vector<int> r(static_cast<std::size_t>(n));`
- `uni` (function, `core/cpp-annote/src/clustering_vbx.cpp:60`) `std::uniform_int_distribution<int> uni(0, n - 1);`
- `best_labs` (function, `core/cpp-annote/src/clustering_vbx.cpp:62`) `std::vector<int> best_labs(static_cast<std::size_t>(n), 0);`
- `labels` (function, `core/cpp-annote/src/clustering_vbx.cpp:68`) `std::vector<int> labels(static_cast<std::size_t>(n), 0);`
- `cnt` (function, `core/cpp-annote/src/clustering_vbx.cpp:87`) `std::vector<int> cnt(static_cast<std::size_t>(k), 0);`
- `centroids_from_labels` (function, `core/cpp-annote/src/clustering_vbx.cpp:115`) `Eigen::MatrixXd centroids_from_labels(const Eigen::MatrixXd& train,`
- `hungarian_maximize` (function, `core/cpp-annote/src/clustering_vbx.cpp:133`) `void hungarian_maximize(const Eigen::MatrixXd& score,                         st`
- `cost` (function, `core/cpp-annote/src/clustering_vbx.cpp:145`) `std::vector<std::vector<double>> cost( static_cast<std::size_t>(m), std::vector<`
- `vbx_clustering_hard` (function, `core/cpp-annote/src/clustering_vbx.cpp:166`) `void vbx_clustering_hard(const plda_vbx::PldaModel& plda,`
- `xflat` (function, `core/cpp-annote/src/clustering_vbx.cpp:192`) `std::vector<double> xflat( static_cast<std::size_t>(train_n.rows() * train_n.col`
- `fea_f` (function, `core/cpp-annote/src/clustering_vbx.cpp:357`) `std::vector<float> fea_f(static_cast<size_t>(fea.rows() * fea.cols()));`
- `CLUSTERING_VBX_H_` (macro, `core/cpp-annote/src/clustering_vbx.h:6`) `#define CLUSTERING_VBX_H_`
- `VbxClusteringParams` (struct, `core/cpp-annote/src/clustering_vbx.h:15`)
- `vbx_clustering_hard` (function, `core/cpp-annote/src/clustering_vbx.h:34`) `void vbx_clustering_hard(const plda_vbx::PldaModel& plda, const VbxClusteringPar` - ``embeddings`` row-major ``(num_chunks * num_speakers * dim)``; ``binarized`` ``(num_chunks * num_fr
- `COMMUNITY1_CPP_ANNOTE_EMBEDDED_H_` (macro, `core/cpp-annote/src/community1_cpp_annote_embedded.h:5`) `#define COMMUNITY1_CPP_ANNOTE_EMBEDDED_H_`
- `receptive_field_json` (variable, `core/cpp-annote/src/community1_cpp_annote_embedded.h:11`) `extern const char receptive_field_json[];`
- `receptive_field_json_size` (variable, `core/cpp-annote/src/community1_cpp_annote_embedded.h:12`) `extern const std::size_t receptive_field_json_size;`
- `pipeline_snapshot_json` (variable, `core/cpp-annote/src/community1_cpp_annote_embedded.h:13`) `extern const char pipeline_snapshot_json[];`
- `pipeline_snapshot_json_size` (variable, `core/cpp-annote/src/community1_cpp_annote_embedded.h:14`) `extern const std::size_t pipeline_snapshot_json_size;`

## Internal vs External Edges

- Internal resolved imports (EXTRACTED): 35
- Cross-boundary resolved imports (EXTRACTED): 2

## Connections

- [EXTRACTED] depends_on community 5 <-> 0 (strength 0.9): Extracted import edge crosses communities: core/reliability/fuzz-wav-pcm.cpp imports core/moonshine-utils/debug-utils.h.

## Risks

- [dataflow DEAD_STORE] `core/cpp-annote/src/clustering_vbx.cpp:53` `kmeans_fit_predict` `d`: `d` assigned at line 53 but never read afterwards.
- [dataflow DEAD_STORE] `core/cpp-annote/src/clustering_vbx.cpp:137` `hungarian_maximize` `m`: `m` assigned at line 137 but never read afterwards.
- [dataflow DEAD_STORE] `core/cpp-annote/src/clustering_vbx.cpp:144` `hungarian_maximize` `pad`: `pad` assigned at line 144 but never read afterwards.
- [dataflow DEAD_STORE] `core/cpp-annote/src/compute_fbank.cpp:30` `wespeaker_like_fbank` `scale`: `scale` assigned at line 30 but never read afterwards.
- [dataflow DEAD_STORE] `core/cpp-annote/src/cpp-annote-engine.h:100` `embedding_dimension` `sr_model`: `sr_model` assigned at line 100 but never read afterwards.
- [dataflow DEAD_STORE] `core/cpp-annote/src/cpp-annote-engine.h:101` `embedding_dimension` `num_channels`: `num_channels` assigned at line 101 but never read afterwards.
- [dataflow DEAD_STORE] `core/cpp-annote/src/cpp-annote-engine.h:102` `embedding_dimension` `chunk_num_samples`: `chunk_num_samples` assigned at line 102 but never read afterwards.
- [dataflow DEAD_STORE] `core/cpp-annote/src/cpp-annote-engine.h:103` `embedding_dimension` `multilabel_export`: `multilabel_export` assigned at line 103 but never read afterwards.
- [dataflow DEAD_STORE] `core/cpp-annote/src/cpp-annote-engine.h:104` `embedding_dimension` `chunk_step_sec`: `chunk_step_sec` assigned at line 104 but never read afterwards.
- [dataflow DEAD_STORE] `core/cpp-annote/src/cpp-annote-engine.h:105` `embedding_dimension` `chunk_dur_sec`: `chunk_dur_sec` assigned at line 105 but never read afterwards.
- [dataflow DEAD_STORE] `core/cpp-annote/src/cpp-annote-streaming.cpp:211` `add_audio_chunk` `sr_model`: `sr_model` assigned at line 211 but never read afterwards.
- [dataflow DEAD_STORE] `core/cpp-annote/src/cpp-annote-streaming.cpp:479` `maybe_refresh` `dim`: `dim` assigned at line 479 but never read afterwards.
- [dataflow DEAD_STORE] `core/cpp-annote/src/cpp-annote-streaming.cpp:480` `maybe_refresh` `FK`: `FK` assigned at line 480 but never read afterwards.
- [dataflow DEAD_STORE] `core/cpp-annote/src/cpp-annote.cpp:77` `trim_warmup_inplace` `new_frames`: `new_frames` assigned at line 77 but never read afterwards.
- [dataflow DEAD_STORE] `core/cpp-annote/src/cpp-annote.cpp:111` `inference_aggregate` `nf`: `nf` assigned at line 111 but never read afterwards.

## Open Questions

- Why do 1 file(s) lack file-level docs (e.g. `core/speaker-diarizer.cpp`)? What purpose do they serve?
- What would break if the most connected file in core/cpp-annote/src changed?
- Should core/cpp-annote/src be split, given cohesion 0.95?

## Sources

- `core/cpp-annote/src/annotation_support.h`
- `core/cpp-annote/src/clustering_vbx.cpp`
- `core/cpp-annote/src/clustering_vbx.h`
- `core/cpp-annote/src/community1_cpp_annote_embedded.h`
- `core/cpp-annote/src/community1_ort_embedded.h`
- `core/cpp-annote/src/compute_fbank.cpp`
- `core/cpp-annote/src/compute_fbank.h`
- `core/cpp-annote/src/cpp-annote-engine.h`
- `core/cpp-annote/src/cpp-annote-streaming.cpp`
- `core/cpp-annote/src/cpp-annote-streaming.h`
- `core/cpp-annote/src/cpp-annote.cpp`
- `core/cpp-annote/src/cpp-annote.h`
- `core/cpp-annote/src/embedding_ort_infer.cpp`
- `core/cpp-annote/src/embedding_ort_infer.h`
- `core/cpp-annote/src/filter_train.cpp`
- `core/cpp-annote/src/filter_train.h`
- `core/cpp-annote/src/hungarian.h`
- `core/cpp-annote/src/parity_log.cpp`
- `core/cpp-annote/src/parity_log.h`
- `core/cpp-annote/src/plda_vbx.cpp`
- *... and 7 more*
