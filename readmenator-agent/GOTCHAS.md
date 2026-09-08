# Gotchas

## God Nodes (high connectivity)

These files have the most connections. Changes here have high blast radius.

- `core/moonshine-tts/src/utf8-utils.h` (score: 91.50)
- `core/moonshine-utils/debug-utils.h` (score: 66.20)
- `core/moonshine-tts/src/rule-based-g2p-factory.cpp` (score: 48.50)
- `core/moonshine-tts/src/moonshine-g2p.cpp` (score: 43.40)
- `core/moonshine-tts/tests/rule-g2p-test-support.h` (score: 43.40)
- `core/moonshine-tts/src/moonshine-g2p-options.h` (score: 39.00)
- `core/moonshine-tts/src/g2p-word-log.h` (score: 38.60)
- `core/moonshine-tts/src/rule-based-g2p.h` (score: 38.30)
- `core/ort-utils/ort-utils.h` (score: 36.30)
- `core/moonshine-c-api.cpp` (score: 35.70)

## Hotspots (complexity + centrality)

- `core/moonshine-c-api.cpp` -- complexity: 0.7, centrality: 0.9, combined: 0.8
- `core/moonshine-tts/src/moonshine-tts.cpp` -- complexity: 0.8, centrality: 0.8, combined: 0.8
- `core/moonshine-tts/src/rule-based-g2p-factory.cpp` -- complexity: 0.3, centrality: 1.0, combined: 0.7
- `core/cpp-annote/src/cpp-annote.cpp` -- complexity: 0.6, centrality: 0.8, combined: 0.7
- `core/moonshine-tts/src/utf8-utils.h` -- complexity: 0.1, centrality: 0.9, combined: 0.6
- `core/moonshine-utils/debug-utils.h` -- complexity: 0.4, centrality: 0.7, combined: 0.6
- `core/moonshine-tts/src/zipvoice-tts.cpp` -- complexity: 0.5, centrality: 0.7, combined: 0.6
- `core/moonshine-cpp.h` -- complexity: 1.0, centrality: 0.2, combined: 0.5
- `scripts/tts_g2p_intelligibility.py` -- complexity: 0.4, centrality: 0.6, combined: 0.5
- `core/moonshine-tts/src/moonshine-g2p.cpp` -- complexity: 0.1, centrality: 0.8, combined: 0.5

## Layer Violations

- `core/intent-recognizer-test.cpp` (testing) -> `core/moonshine-c-api.h` (presentation): testing must not import presentation
- `core/tts-repeated-memory-test.cpp` (testing) -> `core/moonshine-c-api.h` (presentation): testing must not import presentation
- `core/word-alignment-test.cpp` (testing) -> `core/moonshine-c-api.h` (presentation): testing must not import presentation
- `python/tests/test_modules.py` (testing) -> `python/src/moonshine_voice/moonshine_api.py` (presentation): testing must not import presentation
