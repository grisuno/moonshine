# Second Brain

*Last synthesized: 2026-10-07 | 567 files | 16 concept pages | offline, zero tokens*

> Raw sources -> readmenator wiki -> links (Karpathy LLM Wiki Pattern, deterministic).
> Start here, then open one community page. Prefer grep over full reads.

## Vault Overview

The codebase centres on `utf8-utils.h`, `debug-utils.h`, `rule-based-g2p-factory.cpp`. Architecturally it is 6 layers, dominant utility (305 files) across 16 import-based communities. Recorded risk surface: 0 security findings and 0 dependency cycles.

Surprising tissue lives between core: moonshine-cpp, micro/examples/rp2350/src: pack_format, core/moonshine-tts/src/lang-specific: french: 12 extracted cross-community imports and 8 inferred bridges. Follow `connections.json` sorted by strength before refactoring.

Open work clusters around documentation (44% file coverage), 0 security findings, 20 taint paths, and 5 suggested exploration questions in `queries.md`.

## Stats

| Metric | Value |
|--------|-------|
| Files | 567 |
| Symbols | 5438 |
| Resolved imports | 796 |
| Languages | S, cc, cpp, h, java, kt, kts, py, sh, swift |
| Communities | 16 |
| Doc coverage | 44% (252/567 files) |
| Security findings | 0 |
| Estimated read cost | ~105287 tokens (chars/4, offline so $0) |
| Large files (>256KB, maybe generated) | 6: `spanish-unicode-tables.cpp`, `model_data.cc`, `neural_tts_demo_data.cc`, `test_clips.cc`, `vad_model_data.cc` (+1 more) |

## Reading Order

1. Skim Stats and God Nodes below for blast radius.
2. Open the largest community page first, then follow Connections.
3. Use `queries.md` for the next question; log the answer there.

```
grep -rn '<keyword>' index.md community_*.md
readmenator query "<question>" --target readmenator_moonshine_6538iihw
```

## Concept Wiki

- [core: moonshine-cpp (72 files, cohesion 0.88)](./community_0_core_moonshine_cpp.md)
- [micro/examples/rp2350/src: pack_format (71 files, cohesion 0.99)](./community_1_micro_examples_rp2350_src_pack_format.md)
- [core/moonshine-tts/src/lang-specific: french (51 files, cohesion 0.60)](./community_2_core_moonshine_tts_src_lang_specific_french.md)
- [core/moonshine-tts/src/lang-specific: dutch (51 files, cohesion 0.69)](./community_3_core_moonshine_tts_src_lang_specific_dutch.md)
- [core/moonshine-tts/src (50 files, cohesion 0.65)](./community_4_core_moonshine_tts_src.md)
- [core/cpp-annote/src (27 files, cohesion 0.95)](./community_5_core_cpp_annote_src.md)
- [micro/g2p/src (25 files, cohesion 0.93)](./community_6_micro_g2p_src.md)
- [core/moonshine-tts/src/lang-specific: english-hand-oov (18 files, cohesion 0.78)](./community_7_core_moonshine_tts_src_lang_specific_english_hand_oov.md)
- [python/src/moonshine_voice: dialog_flow (18 files, cohesion 1.00)](./community_8_python_src_moonshine_voice_dialog_flow.md)
- [micro/examples/rp2350/src: worldlite_synth (14 files, cohesion 0.90)](./community_9_micro_examples_rp2350_src_worldlite_synth.md)
- [micro/stt-training/stt_training (13 files, cohesion 1.00)](./community_10_micro_stt_training_stt_training.md)
- [android/java/main/java/ai/moonshine/voice (12 files, cohesion 1.00)](./community_11_android_java_main_java_ai_moonshine_voice.md)
- [core: cosine-distance-test (3 files, cohesion 1.00)](./community_12_core_cosine_distance_test.md)
- [micro/stt/scripts (3 files, cohesion 1.00)](./community_13_micro_stt_scripts.md)
- [python/src/moonshine_voice: cli (2 files, cohesion 1.00)](./community_14_python_src_moonshine_voice_cli.md)
- [orphans (137 files, cohesion 0.00)](./community_15_orphans.md)

## God Nodes

| File | Score |
|------|-------|
| `core/moonshine-tts/src/utf8-utils.h` | 91.0 |
| `core/moonshine-utils/debug-utils.h` | 65.2 |
| `core/moonshine-tts/src/rule-based-g2p-factory.cpp` | 46.6 |
| `core/moonshine-tts/tests/rule-g2p-test-support.h` | 42.9 |
| `core/moonshine-tts/src/moonshine-g2p.cpp` | 42.7 |

## Strongest Connections

- 0 -> 4: depends_on (strength 0.9, EXTRACTED)
- 0 -> 3: depends_on (strength 0.9, EXTRACTED)
- 4 -> 2: depends_on (strength 0.9, EXTRACTED)
- 2 -> 3: depends_on (strength 0.9, EXTRACTED)
- 3 -> 4: depends_on (strength 0.9, EXTRACTED)
- 7 -> 3: depends_on (strength 0.9, EXTRACTED)
- 7 -> 2: depends_on (strength 0.9, EXTRACTED)
- 2 -> 0: depends_on (strength 0.9, EXTRACTED)
- 7 -> 4: depends_on (strength 0.9, EXTRACTED)
- 5 -> 0: depends_on (strength 0.9, EXTRACTED)

## Navigation Tips

- Obsidian Graph View works: every community page links back here.
- `connections.json` is machine-readable for GraphRAG pipelines.
- `REPORT.md` states what was extracted vs inferred and current limits.
- Regenerate offline: `readmenator . --rebuild` (no network, no tokens).
