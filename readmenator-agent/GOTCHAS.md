# Gotchas

## God Nodes (high connectivity)

These files have the most connections. Changes here have high blast radius.

- `python/src/moonshine_voice/download.py` (score: 26.30)
- `python/src/moonshine_voice/moonshine_api.py` (score: 21.70)
- `python/src/moonshine_voice/dialog_flow.py` (score: 19.40)
- `python/src/moonshine_voice/__init__.py` (score: 16.10)
- `python/src/moonshine_voice/errors.py` (score: 15.50)
- `python/src/moonshine_voice/alphanumeric_listener.py` (score: 13.10)
- `python/src/moonshine_voice/intent_recognizer.py` (score: 12.90)
- `micro/stt-training/stt_training/train.py` (score: 12.60)
- `python/src/moonshine_voice/tts.py` (score: 12.40)
- `core/moonshine-cpp.h` (score: 12.30)

## Hotspots (complexity + centrality)

- `core/moonshine-c-api.cpp` -- complexity: 0.5, centrality: 1.0, combined: 0.8
- `scripts/tts_g2p_intelligibility.py` -- complexity: 0.5, centrality: 0.8, combined: 0.7
- `core/moonshine-tts/src/moonshine-tts.cpp` -- complexity: 0.5, centrality: 0.8, combined: 0.7
- `python/src/moonshine_voice/dialog_flow.py` -- complexity: 0.8, centrality: 0.6, combined: 0.6
- `core/cpp-annote/src/cpp-annote.cpp` -- complexity: 0.3, centrality: 0.8, combined: 0.6
- `python/src/moonshine_voice/tts.py` -- complexity: 0.4, centrality: 0.8, combined: 0.6
- `core/moonshine-tts/src/rule-based-g2p-factory.cpp` -- complexity: 0.2, centrality: 0.8, combined: 0.6
- `core/moonshine-cpp.h` -- complexity: 1.0, centrality: 0.2, combined: 0.5
- `python/src/moonshine_voice/download.py` -- complexity: 0.3, centrality: 0.6, combined: 0.5
- `core/moonshine-model.cpp` -- complexity: 0.2, centrality: 0.7, combined: 0.5

## Layer Violations

- `python/tests/test_modules.py` (testing) -> `python/src/moonshine_voice/moonshine_api.py` (presentation): testing must not import presentation
