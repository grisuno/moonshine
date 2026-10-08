# Subsystem: micro_stt-training_tools

## micro/stt-training/tools/download_musan_rirs.py
- Doc: Download optional augmentation assets: MUSAN noise + OpenSLR-26 RIRs.
- Layer: utility
- Language: py
- Symbols:
  - `download_musan_noise` (function, line 37) `def download_musan_noise(out_dir, small, seed)`
  - `download_rirs` (function, line 67) `def download_rirs(out_dir, max_files, seed)`
  - `main` (function, line 94) `def main()`

## micro/stt-training/tools/extract_clips.py
- Doc: Cut per-word training clips from mined People's Speech utterances.
- Layer: utility
- Language: py
- Symbols:
  - `AlignedWord` (class, line 46) `class AlignedWord`
  - `MMSAligner` (class, line 53) `class MMSAligner`
  - `_cut_natural_clip` (method, line 116) `def _cut_natural_clip(audio, start_s, end_s)`
  - `_resolve_device` (method, line 144) `def _resolve_device(choice)`
  - `_load_rows` (method, line 156) `def _load_rows(path)`
  - `_safe` (method, line 167) `def _safe(s)`
  - `main` (method, line 171) `def main()`
  - `__init__` (method, line 56) `def __init__(self, device, with_star)`
  - `_ids` (method, line 71) `def _ids(self, word)`
  - `align` (method, line 74) `def align(self, audio_1d, words)`
  - `emit` (method, line 212) `def emit(label, clip_id, char_start, speaker, clip, sample_rate)`
- Depends on: `micro/stt-training/stt_training/words.py`

## micro/stt-training/tools/mine_peoples_speech.py
- Doc: Mine People's Speech for command words (and generic "unknown" speech).
- Layer: utility
- Language: py
- Symbols:
  - `_new_fs` (function, line 69) `def _new_fs()`
  - `_shard_paths` (function, line 75) `def _shard_paths(config, split)`
  - `_ShardReader` (class, line 80) `class _ShardReader`
  - `iter_peoples_speech` (method, line 131) `def iter_peoples_speech(config, split, offset, limit)`
  - `_tokens_with_pos` (method, line 187) `def _tokens_with_pos(text)`
  - `find_matches` (method, line 191) `def find_matches(text, targets)`
  - `_safe_name` (method, line 207) `def _safe_name(clip_id)`
  - `save_audio_16k` (method, line 211) `def save_audio_16k(fetch, out_path)`
  - `_load_seen_keys` (method, line 231) `def _load_seen_keys(path)`
  - `main` (method, line 247) `def main()`
  - `__init__` (method, line 90) `def __init__(self, shard, max_attempts)`
  - `_open` (method, line 98) `def _open(self)`
  - `num_row_groups` (method, line 103) `def num_row_groups(self)`
  - `row_group_num_rows` (method, line 106) `def row_group_num_rows(self, rg)`
  - `read_columns` (method, line 109) `def read_columns(self, rg, columns)`
  - `_fetch` (method, line 157) `def _fetch(_rg, _i)`
- Depends on: `micro/stt-training/stt_training/words.py`

## micro/stt-training/tools/synthesize.py
- Doc: Synthesize the command vocabulary with Moonshine Voice ZipVoice TTS.
- Layer: utility
- Language: py
- Symbols:
  - `discover_voices` (function, line 58) `def discover_voices(language)`
  - `_resample_to_16k` (function, line 76) `def _resample_to_16k(samples, sr)`
  - `main` (function, line 85) `def main()`
- Depends on: `micro/stt-training/stt_training/words.py`
