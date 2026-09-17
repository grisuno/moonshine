# Subsystem: scripts

## micro/stt/scripts/desktop_parity.py
- Layer: utility
- Doc: Desktop regression check for the moonshine-micro on-device embedded-clip test loop.  The Pico firmware runs an int8 mel-
- Language: py
- Symbols:
  - `_resolve_meta` (function, line 60) `def _resolve_meta(tflite)`
  - `_int16_roundtrip` (function, line 76) `def _int16_roundtrip(samples)`
  - `_softmax_prob` (function, line 92) `def _softmax_prob(logits, idx)`
  - `_parse_device_log` (function, line 98) `def _parse_device_log(path)`
  - `main` (function, line 111) `def main(argv)`
- Depends on: `micro/stt/scripts/generate_embedded_data.py`

## micro/stt/scripts/generate_embedded_data.py
- Layer: data_access
- Doc: Generate the compiled-in data blobs for the moonshine-micro Pico build.  The Pico has no filesystem, so the model file a
- Language: py
- Symbols:
  - `_include_guard` (function, line 63) `def _include_guard(stem)`
  - `_resolve_int8_mel_tflite` (function, line 68) `def _resolve_int8_mel_tflite(explicit)`
  - `_meta_sidecar` (function, line 90) `def _meta_sidecar(tflite)`
  - `_load_meta` (function, line 103) `def _load_meta(tflite)`
  - `_format_byte_array` (function, line 142) `def _format_byte_array(data, width)`
  - `_format_int16_array` (function, line 151) `def _format_int16_array(samples, width)`
  - `_f32` (function, line 160) `def _f32(x)`
  - `_format_float32_array` (function, line 171) `def _format_float32_array(vals, width)`
  - `_format_plain_int_array` (function, line 180) `def _format_plain_int_array(vals, width)`
  - `_fp32_to_int16_pcm` (function, line 189) `def _fp32_to_int16_pcm(samples)`
  - `_is_riff_wav` (function, line 207) `def _is_riff_wav(path)`
  - `_load_clip` (function, line 216) `def _load_clip(path, sample_rate, n_samples)`
  - `_write_model_files` (function, line 228) `def _write_model_files(out_dir, tflite)`
  - `_write_audio_config_file` (function, line 268) `def _write_audio_config_file(out_dir)`
  - `_write_mel_tables_file` (function, line 327) `def _write_mel_tables_file(out_dir)`
  - `_write_classes_files` (function, line 465) `def _write_classes_files(out_dir, classes)`
  - `_write_clips_files` (function, line 501) `def _write_clips_files(out_dir, decoded, sample_rate, n_samples)`
  - `_pick_clips` (function, line 586) `def _pick_clips(wavs_roots, classes, clips_per_class, max_classes)`
  - `_pick_clips_hub` (function, line 617) `def _pick_clips_hub(repo_id, configs, classes, clips_per_class, max_classes, sample_rate, n_samples, cache_dir)`
  - `main` (function, line 680) `def main(argv)`
- Imported by: `micro/stt/scripts/desktop_parity.py`, `micro/vad/scripts/generate_vad_embedded_data.py`
