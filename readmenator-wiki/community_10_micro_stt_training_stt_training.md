# micro/stt-training/stt_training

*Community 10 | 13 files | cohesion 1.00*

## Definition

This community groups 13 file(s) rooted at `micro/stt-training/stt_training` with dominant language py (cohesion 1.00). Central symbols: `AlignedWord`, `ConvBNAct`, `InvertedResidual`, `LogMelSpectrogram`, `MMSAligner`, `SpecAugment`, `SpeechCommandsDataset`, `WaveformAugment`. Core file: `micro/stt-training/stt_training/augment.py` (17 symbols). Documented purpose: Standalone training recipe for the moonshine-micro on-device word classifier.  This package trains a compact MobileNetV2-style log-mel classifier (``WordCNN``) .

## Files

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `micro/stt-training/stt_training/__init__.py` | py | utility | 0 | yes |
| `micro/stt-training/stt_training/augment.py` | py | utility | 17 | yes |
| `micro/stt-training/stt_training/checkpoint.py` | py | utility | 3 | yes |
| `micro/stt-training/stt_training/dataset.py` | py | data_access | 14 | yes |
| `micro/stt-training/stt_training/evaluate.py` | py | utility | 3 | yes |
| `micro/stt-training/stt_training/export.py` | py | utility | 7 | yes |
| `micro/stt-training/stt_training/features.py` | py | utility | 7 | yes |
| `micro/stt-training/stt_training/model.py` | py | business_logic | 12 | yes |
| `micro/stt-training/stt_training/train.py` | py | utility | 6 | yes |
| `micro/stt-training/stt_training/words.py` | py | utility | 3 | yes |
| `micro/stt-training/tools/extract_clips.py` | py | utility | 11 | yes |
| `micro/stt-training/tools/mine_peoples_speech.py` | py | utility | 16 | yes |
| `micro/stt-training/tools/synthesize.py` | py | utility | 3 | yes |

## Key Symbols

- `WaveformAugment` (class, `micro/stt-training/stt_training/augment.py:25`) `class WaveformAugment(Module)` - Batched waveform augmentation pipeline.
- `__init__` (method, `micro/stt-training/stt_training/augment.py:36`) `def __init__(self, sample_rate, musan_noise_dir, rir_dir, gain_db, noise_snr_min`
- `_load_concat_noise` (method, `micro/stt-training/stt_training/augment.py:82`) `def _load_concat_noise(self, noise_dir, max_seconds)`
- `_load_rirs` (method, `micro/stt-training/stt_training/augment.py:106`) `def _load_rirs(self, rir_dir, max_rirs)`
- `n_transforms` (method, `micro/stt-training/stt_training/augment.py:139`) `def n_transforms(self)`
- `has_external_data` (method, `micro/stt-training/stt_training/augment.py:143`) `def has_external_data(self)`
- `_mask` (method, `micro/stt-training/stt_training/augment.py:148`) `def _mask(p, b, dev)`
- `_rms` (method, `micro/stt-training/stt_training/augment.py:152`) `def _rms(x)`
- `_gain` (method, `micro/stt-training/stt_training/augment.py:155`) `def _gain(self, x, b, dev)`
- `_polarity` (method, `micro/stt-training/stt_training/augment.py:161`) `def _polarity(self, x, b, dev)`
- `_shift` (method, `micro/stt-training/stt_training/augment.py:165`) `def _shift(self, x, b, t, dev)`
- `_snr_scale` (method, `micro/stt-training/stt_training/augment.py:174`) `def _snr_scale(self, sig, noise, b, dev)`
- `_colored_noise` (method, `micro/stt-training/stt_training/augment.py:181`) `def _colored_noise(self, x, b, t, dev)`
- `_bandpass` (method, `micro/stt-training/stt_training/augment.py:194`) `def _bandpass(self, x, b, t, dev)`
- `_bg_noise` (method, `micro/stt-training/stt_training/augment.py:210`) `def _bg_noise(self, x, b, t, dev)`
- `_rir` (method, `micro/stt-training/stt_training/augment.py:219`) `def _rir(self, x, b, t, dev)`
- `forward` (method, `micro/stt-training/stt_training/augment.py:238`) `def forward(self, waveform)`
- `resolve_checkpoint` (function, `micro/stt-training/stt_training/checkpoint.py:17`) `def resolve_checkpoint(path)` - Accept a ``.pt`` file, a run directory, or the checkpoints parent.
- `load_model` (function, `micro/stt-training/stt_training/checkpoint.py:35`) `def load_model(path, device)` - Load a checkpoint. Returns ``(model, classes, cfg)``.
- `load_representative_waveforms` (function, `micro/stt-training/stt_training/checkpoint.py:61`) `def load_representative_waveforms(data_roots, n, target_samples, sample_rate, se` - Sample up to ``n`` fixed-length mono waveforms from ``<root>/<class>/*.wav``.
- `_warn_decode_failure` (function, `micro/stt-training/stt_training/dataset.py:27`) `def _warn_decode_failure(src, exc)`
- `voice_id_from_path` (function, `micro/stt-training/stt_training/dataset.py:39`) `def voice_id_from_path(path)` - Stable per-voice id for speaker-independent splits.
- `SpeechCommandsDataset` (class, `micro/stt-training/stt_training/dataset.py:51`) `class SpeechCommandsDataset(Dataset)` - Loads wavs from ``<root>/<class>/*.wav`` across one or more corpus roots.
- `__init__` (method, `micro/stt-training/stt_training/dataset.py:54`) `def __init__(self, roots, classes, sample_rate, clip_seconds)`
- `__len__` (method, `micro/stt-training/stt_training/dataset.py:89`) `def __len__(self)`
- `_load_wav` (method, `micro/stt-training/stt_training/dataset.py:92`) `def _load_wav(self, path)`
- `__getitem__` (method, `micro/stt-training/stt_training/dataset.py:109`) `def __getitem__(self, idx)`
- `voice_ids` (method, `micro/stt-training/stt_training/dataset.py:113`) `def voice_ids(self)`
- `load_waveform` (method, `micro/stt-training/stt_training/dataset.py:116`) `def load_waveform(self, idx)`
- `speaker_independent_split` (method, `micro/stt-training/stt_training/dataset.py:120`) `def speaker_independent_split(dataset, val_fraction, seed)` - Split indices so no voice appears in both train and val.

## Internal vs External Edges

- Internal resolved imports (EXTRACTED): 17
- Cross-boundary resolved imports (EXTRACTED): 0

## Connections

- [INFERRED] shares_context community 0 <-> 10 (strength 0.5): Inferred shared context (layer utility) with no import path between community 0 (core: moonshine-cpp) and community 10 (micro/stt-training/stt_training).

## Risks

- No scoped security, taint, cycle, or layer risks.

## Open Questions

- What would break if the most connected file in micro/stt-training/stt_training changed?
- Should micro/stt-training/stt_training be split, given cohesion 1.00?

## Sources

- `micro/stt-training/stt_training/__init__.py`
- `micro/stt-training/stt_training/augment.py`
- `micro/stt-training/stt_training/checkpoint.py`
- `micro/stt-training/stt_training/dataset.py`
- `micro/stt-training/stt_training/evaluate.py`
- `micro/stt-training/stt_training/export.py`
- `micro/stt-training/stt_training/features.py`
- `micro/stt-training/stt_training/model.py`
- `micro/stt-training/stt_training/train.py`
- `micro/stt-training/stt_training/words.py`
- `micro/stt-training/tools/extract_clips.py`
- `micro/stt-training/tools/mine_peoples_speech.py`
- `micro/stt-training/tools/synthesize.py`
