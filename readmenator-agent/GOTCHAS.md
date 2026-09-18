# Gotchas

## God Nodes (high connectivity)

These files have the most connections. Changes here have high blast radius.

- `core/moonshine-tts/src/utf8-utils.h` (score: 91.00)
- `core/moonshine-utils/debug-utils.h` (score: 65.20)
- `core/moonshine-tts/src/rule-based-g2p-factory.cpp` (score: 46.60)
- `core/moonshine-tts/tests/rule-g2p-test-support.h` (score: 42.90)
- `core/moonshine-tts/src/moonshine-g2p.cpp` (score: 42.70)
- `core/moonshine-tts/src/moonshine-g2p-options.h` (score: 38.60)
- `core/moonshine-tts/src/g2p-word-log.h` (score: 38.50)
- `core/moonshine-tts/src/rule-based-g2p.h` (score: 38.30)
- `core/ort-utils/ort-utils.h` (score: 35.50)
- `core/moonshine-c-api.cpp` (score: 33.20)

## Hotspots (complexity + centrality)

- `core/moonshine-c-api.cpp` -- complexity: 0.6, centrality: 0.9, combined: 0.8
- `core/moonshine-tts/src/moonshine-tts.cpp` -- complexity: 0.6, centrality: 0.8, combined: 0.7
- `core/moonshine-tts/src/rule-based-g2p-factory.cpp` -- complexity: 0.2, centrality: 1.0, combined: 0.7
- `core/cpp-annote/src/cpp-annote.cpp` -- complexity: 0.5, centrality: 0.8, combined: 0.7
- `core/moonshine-tts/src/utf8-utils.h` -- complexity: 0.1, centrality: 0.9, combined: 0.6
- `core/moonshine-utils/debug-utils.h` -- complexity: 0.4, centrality: 0.7, combined: 0.6
- `core/moonshine-tts/src/zipvoice-tts.cpp` -- complexity: 0.4, centrality: 0.7, combined: 0.6
- `scripts/tts_g2p_intelligibility.py` -- complexity: 0.5, centrality: 0.6, combined: 0.5
- `core/moonshine-cpp.h` -- complexity: 1.0, centrality: 0.2, combined: 0.5
- `python/src/moonshine_voice/dialog_flow.py` -- complexity: 0.7, centrality: 0.4, combined: 0.5

## Layer Violations

- `core/intent-recognizer-test.cpp` (testing) -> `core/moonshine-c-api.h` (presentation): testing must not import presentation
- `core/tts-repeated-memory-test.cpp` (testing) -> `core/moonshine-c-api.h` (presentation): testing must not import presentation
- `core/word-alignment-test.cpp` (testing) -> `core/moonshine-c-api.h` (presentation): testing must not import presentation
- `python/tests/test_modules.py` (testing) -> `python/src/moonshine_voice/moonshine_api.py` (presentation): testing must not import presentation

## Dataflow Issues (INFERRED, review each lead)

- `android/java/androidTest/java/ai/moonshine/voice/Utils.java:131` `loadWavFromAssets` [UNCHECKED_ALLOC] `is`: Result of allocator stored in `is` is never checked against NULL.
- `android/java/androidTest/java/ai/moonshine/voice/Utils.java:177` `loadAsset` [UNCHECKED_ALLOC] `is`: Result of allocator stored in `is` is never checked against NULL.
- `android/java/androidTest/java/ai/moonshine/voice/Utils.java:190` `copyAssetToTempDir` [UNCHECKED_ALLOC] `is`: Result of allocator stored in `is` is never checked against NULL.
- `android/java/main/java/ai/moonshine/voice/Transcriber.java:294` `readAllBytes` [UNCHECKED_ALLOC] `is`: Result of allocator stored in `is` is never checked against NULL.
- `core/cpp-annote/src/clustering_vbx.cpp:53` `kmeans_fit_predict` [DEAD_STORE] `d`: `d` assigned at line 53 but never read afterwards.
- `core/cpp-annote/src/clustering_vbx.cpp:137` `hungarian_maximize` [DEAD_STORE] `m`: `m` assigned at line 137 but never read afterwards.
- `core/cpp-annote/src/clustering_vbx.cpp:144` `hungarian_maximize` [DEAD_STORE] `pad`: `pad` assigned at line 144 but never read afterwards.
- `core/cpp-annote/src/compute_fbank.cpp:30` `wespeaker_like_fbank` [DEAD_STORE] `scale`: `scale` assigned at line 30 but never read afterwards.
- `core/cpp-annote/src/cpp-annote-engine.h:100` `embedding_dimension` [DEAD_STORE] `sr_model`: `sr_model` assigned at line 100 but never read afterwards.
- `core/cpp-annote/src/cpp-annote-engine.h:101` `embedding_dimension` [DEAD_STORE] `num_channels`: `num_channels` assigned at line 101 but never read afterwards.
