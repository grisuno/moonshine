# micro/stt/scripts

*Community 13 | 3 files | cohesion 1.00*

## Definition

This community groups 3 file(s) rooted at `micro/stt/scripts` with dominant language py (cohesion 1.00). Central symbols: `_auto_tflite`, `_f32`, `_format_byte_array`, `_format_float32_array`, `_format_int16_array`, `_format_plain_int_array`, `_fp32_to_int16_pcm`, `_include_guard`. Core file: `micro/stt/scripts/generate_embedded_data.py` (20 symbols). Documented purpose: Desktop regression check for the moonshine-micro on-device embedded-clip test loop.  The Pico firmware runs an int8 mel-mode ``.tflite`` over a fixed set of emb.

## Files

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `micro/stt/scripts/desktop_parity.py` | py | utility | 5 | yes |
| `micro/stt/scripts/generate_embedded_data.py` | py | data_access | 20 | yes |
| `micro/vad/scripts/generate_vad_embedded_data.py` | py | data_access | 6 | yes |

## Key Symbols

- `_resolve_meta` (function, `micro/stt/scripts/desktop_parity.py:60`) `def _resolve_meta(tflite)` - Load whichever metadata sidecar sits next to the model.
- `_int16_roundtrip` (function, `micro/stt/scripts/desktop_parity.py:76`) `def _int16_roundtrip(samples)` - Replicate the embedded int16 blob and the firmware's inverse.
- `_softmax_prob` (function, `micro/stt/scripts/desktop_parity.py:92`) `def _softmax_prob(logits, idx)`
- `_parse_device_log` (function, `micro/stt/scripts/desktop_parity.py:98`) `def _parse_device_log(path)` - Pull ``(exp, got)`` pairs from a pico_monitor.log per-clip table.
- `main` (function, `micro/stt/scripts/desktop_parity.py:111`) `def main(argv)`
- `_include_guard` (function, `micro/stt/scripts/generate_embedded_data.py:63`) `def _include_guard(stem)` - Traditional include-guard macro for a generated header stem (no ext).
- `_resolve_int8_mel_tflite` (function, `micro/stt/scripts/generate_embedded_data.py:68`) `def _resolve_int8_mel_tflite(explicit)` - Return the checked-in SpellingCNN int8 model under moonshine-micro/models/.
- `_meta_sidecar` (function, `micro/stt/scripts/generate_embedded_data.py:90`) `def _meta_sidecar(tflite)`
- `_load_meta` (function, `micro/stt/scripts/generate_embedded_data.py:103`) `def _load_meta(tflite)` - Load the model's audio metadata, or die loudly if it's missing.
- `_format_byte_array` (function, `micro/stt/scripts/generate_embedded_data.py:142`) `def _format_byte_array(data, width)` - Render `data` as comma-separated 0x.. literals, wrapping every `width`.
- `_format_int16_array` (function, `micro/stt/scripts/generate_embedded_data.py:151`) `def _format_int16_array(samples, width)` - Render signed int16 samples as comma-separated literals.
- `_f32` (function, `micro/stt/scripts/generate_embedded_data.py:160`) `def _f32(x)` - Round a Python float (f64) to the nearest IEEE-754 float32 value.
- `_format_float32_array` (function, `micro/stt/scripts/generate_embedded_data.py:171`) `def _format_float32_array(vals, width)` - Render floats as comma-separated C ``float`` literals (``...f``).
- `_format_plain_int_array` (function, `micro/stt/scripts/generate_embedded_data.py:180`) `def _format_plain_int_array(vals, width)` - Render ints as comma-separated literals (no width padding).
- `_fp32_to_int16_pcm` (function, `micro/stt/scripts/generate_embedded_data.py:189`) `def _fp32_to_int16_pcm(samples)` - Symmetric 16-bit quantization with saturation.
- `_is_riff_wav` (function, `micro/stt/scripts/generate_embedded_data.py:207`) `def _is_riff_wav(path)` - True when ``path`` looks like a real PCM wav (not a Git LFS pointer).
- `_load_clip` (function, `micro/stt/scripts/generate_embedded_data.py:216`) `def _load_clip(path, sample_rate, n_samples)` - Read a wav, conform to (sample_rate, n_samples), return int16 PCM.
- `_write_model_files` (function, `micro/stt/scripts/generate_embedded_data.py:228`) `def _write_model_files(out_dir, tflite)`
- `_write_audio_config_file` (function, `micro/stt/scripts/generate_embedded_data.py:268`) `def _write_audio_config_file(out_dir)` - Emit ``audio_config.h`` with the model's mel-front-end constants.
- `_write_mel_tables_file` (function, `micro/stt/scripts/generate_embedded_data.py:327`) `def _write_mel_tables_file(out_dir)` - Emit ``mel_tables.{h,cc}``: the precomputed Hann window + CSR mel
- `_write_classes_files` (function, `micro/stt/scripts/generate_embedded_data.py:465`) `def _write_classes_files(out_dir, classes)`
- `_write_clips_files` (function, `micro/stt/scripts/generate_embedded_data.py:501`) `def _write_clips_files(out_dir, decoded, sample_rate, n_samples)` - Write one ``int16`` array per clip plus a small descriptor table.
- `_pick_clips` (function, `micro/stt/scripts/generate_embedded_data.py:586`) `def _pick_clips(wavs_roots, classes, clips_per_class, max_classes)` - Pick a deterministic per-class subset (alphabetical by filename).
- `_pick_clips_hub` (function, `micro/stt/scripts/generate_embedded_data.py:617`) `def _pick_clips_hub(repo_id, configs, classes, clips_per_class, max_classes, sam` - Pick a deterministic per-class subset from packed HF speech shards.
- `main` (function, `micro/stt/scripts/generate_embedded_data.py:680`) `def main(argv)`
- `_smooth_window_frames` (function, `micro/vad/scripts/generate_vad_embedded_data.py:66`) `def _smooth_window_frames()`
- `_write_vad_config` (function, `micro/vad/scripts/generate_vad_embedded_data.py:72`) `def _write_vad_config(out_dir)`
- `_write_vad_mel_tables` (function, `micro/vad/scripts/generate_vad_embedded_data.py:117`) `def _write_vad_mel_tables(out_dir)`
- `_write_vad_model` (function, `micro/vad/scripts/generate_vad_embedded_data.py:190`) `def _write_vad_model(out_dir, tflite)`
- `_auto_tflite` (function, `micro/vad/scripts/generate_vad_embedded_data.py:224`) `def _auto_tflite()`

## Internal vs External Edges

- Internal resolved imports (EXTRACTED): 2
- Cross-boundary resolved imports (EXTRACTED): 0

## Connections

- No cross-community bridges recorded. This community is self-contained.

## Risks

- No scoped security, taint, cycle, or layer risks.

## Open Questions

- What would break if the most connected file in micro/stt/scripts changed?
- Should micro/stt/scripts be split, given cohesion 1.00?

## Sources

- `micro/stt/scripts/desktop_parity.py`
- `micro/stt/scripts/generate_embedded_data.py`
- `micro/vad/scripts/generate_vad_embedded_data.py`
