# Subsystem: stt_training

## micro/stt-training/stt_training/__init__.py
- Layer: utility
- Language: py
- Depends on: `micro/stt-training/stt_training/words.py`

## micro/stt-training/stt_training/augment.py
- Layer: utility
- Language: py
- Symbols:
  - `WaveformAugment` (class, line 25) `class WaveformAugment(Module)`
  - `__init__` (method, line 36) `def __init__(self, sample_rate, musan_noise_dir, rir_dir, gain_db, noise_snr_min, noise_snr_max, bandpass_p, max_rirs, max_noise_seconds, seed)`
  - `_load_concat_noise` (method, line 82) `def _load_concat_noise(self, noise_dir, max_seconds)`
  - `_load_rirs` (method, line 106) `def _load_rirs(self, rir_dir, max_rirs)`
  - `n_transforms` (method, line 139) `def n_transforms(self)`
  - `has_external_data` (method, line 143) `def has_external_data(self)`
  - `_mask` (method, line 148) `def _mask(p, b, dev)`
  - `_rms` (method, line 152) `def _rms(x)`
  - `_gain` (method, line 155) `def _gain(self, x, b, dev)`
  - `_polarity` (method, line 161) `def _polarity(self, x, b, dev)`
  - `_shift` (method, line 165) `def _shift(self, x, b, t, dev)`
  - `_snr_scale` (method, line 174) `def _snr_scale(self, sig, noise, b, dev)`
  - `_colored_noise` (method, line 181) `def _colored_noise(self, x, b, t, dev)`
  - `_bandpass` (method, line 194) `def _bandpass(self, x, b, t, dev)`
  - `_bg_noise` (method, line 210) `def _bg_noise(self, x, b, t, dev)`
  - `_rir` (method, line 219) `def _rir(self, x, b, t, dev)`
  - `forward` (method, line 238) `def forward(self, waveform)`
- Imported by: `micro/stt-training/stt_training/train.py`

## micro/stt-training/stt_training/checkpoint.py
- Layer: utility
- Language: py
- Symbols:
  - `resolve_checkpoint` (function, line 17) `def resolve_checkpoint(path)`
  - `load_model` (function, line 35) `def load_model(path, device)`
  - `load_representative_waveforms` (function, line 61) `def load_representative_waveforms(data_roots, n, target_samples, sample_rate, seed)`
- Depends on: `micro/stt-training/stt_training/model.py`
- Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/export.py`

## micro/stt-training/stt_training/dataset.py
- Layer: data_access
- Language: py
- Symbols:
  - `_warn_decode_failure` (function, line 27) `def _warn_decode_failure(src, exc)`
  - `voice_id_from_path` (function, line 39) `def voice_id_from_path(path)`
  - `SpeechCommandsDataset` (class, line 51) `class SpeechCommandsDataset(Dataset)`
  - `speaker_independent_split` (method, line 120) `def speaker_independent_split(dataset, val_fraction, seed)`
  - `build_class_balanced_sampler` (method, line 142) `def build_class_balanced_sampler(labels, power)`
  - `report_class_coverage` (method, line 163) `def report_class_coverage(dataset, classes)`
  - `mixup` (method, line 190) `def mixup(x, y, num_classes, alpha)`
  - `soft_cross_entropy` (method, line 205) `def soft_cross_entropy(logits, soft_targets, smoothing)`
  - `__init__` (method, line 54) `def __init__(self, roots, classes, sample_rate, clip_seconds)`
  - `__len__` (method, line 89) `def __len__(self)`
  - `_load_wav` (method, line 92) `def _load_wav(self, path)`
  - `__getitem__` (method, line 109) `def __getitem__(self, idx)`
  - `voice_ids` (method, line 113) `def voice_ids(self)`
  - `load_waveform` (method, line 116) `def load_waveform(self, idx)`
- Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/train.py`

## micro/stt-training/stt_training/evaluate.py
- Layer: utility
- Language: py
- Symbols:
  - `_confusions` (function, line 30) `def _confusions(y_true, y_pred, classes, top)`
  - `main` (function, line 38) `def main()`
  - `_report` (function, line 102) `def _report(name, y_true, y_pred, classes)`
- Depends on: `micro/stt-training/stt_training/checkpoint.py`, `micro/stt-training/stt_training/dataset.py`, `micro/stt-training/stt_training/export.py`, `micro/stt-training/stt_training/features.py`, `micro/stt-training/stt_training/train.py`

## micro/stt-training/stt_training/export.py
- Layer: utility
- Language: py
- Symbols:
  - `_inline_buffers` (function, line 37) `def _inline_buffers(buf)`
  - `_interpreter` (function, line 62) `def _interpreter(path)`
  - `_run_tflite` (function, line 70) `def _run_tflite(interp, feats)`
  - `export` (function, line 86) `def export(args)`
  - `_default_calibration_roots` (function, line 197) `def _default_calibration_roots(args)`
  - `build_argparser` (function, line 207) `def build_argparser()`
  - `main` (function, line 220) `def main()`
- Depends on: `micro/stt-training/stt_training/checkpoint.py`, `micro/stt-training/stt_training/features.py`
- Imported by: `micro/stt-training/stt_training/evaluate.py`

## micro/stt-training/stt_training/features.py
- Layer: utility
- Language: py
- Symbols:
  - `LogMelSpectrogram` (class, line 16) `class LogMelSpectrogram(Module)`
  - `SpecAugment` (class, line 70) `class SpecAugment(Module)`
  - `__init__` (method, line 23) `def __init__(self, sample_rate, n_fft, hop_length, n_mels, f_min, f_max, target_frames, eps)`
  - `_fix_length` (method, line 50) `def _fix_length(self, x)`
  - `forward` (method, line 58) `def forward(self, waveform)`
  - `__init__` (method, line 73) `def __init__(self, freq_mask_param, time_mask_param, n_freq_masks, n_time_masks)`
  - `forward` (method, line 86) `def forward(self, x)`
- Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/export.py`, `micro/stt-training/stt_training/train.py`

## micro/stt-training/stt_training/model.py
- Layer: business_logic
- Language: py
- Symbols:
  - `_make_divisible` (function, line 19) `def _make_divisible(v, divisor)`
  - `normalize_stride` (function, line 27) `def normalize_stride(v)`
  - `ConvBNAct` (class, line 46) `class ConvBNAct(Sequential)`
  - `InvertedResidual` (class, line 58) `class InvertedResidual(Module)`
  - `WordCNN` (class, line 82) `class WordCNN(Module)`
  - `build_model` (method, line 167) `def build_model(num_classes)`
  - `__init__` (method, line 47) `def __init__(self, in_c, out_c, kernel, stride, groups, act)`
  - `__init__` (method, line 61) `def __init__(self, in_c, out_c, stride, expand_ratio)`
  - `forward` (method, line 77) `def forward(self, x)`
  - `__init__` (method, line 100) `def __init__(self, num_classes, width_mult, dropout, stem_stride, pad_to_odd)`
  - `_init_weights` (method, line 146) `def _init_weights(self)`
  - `forward` (method, line 157) `def forward(self, x)`
- Imported by: `micro/stt-training/stt_training/checkpoint.py`, `micro/stt-training/stt_training/train.py`

## micro/stt-training/stt_training/train.py
- Layer: utility
- Language: py
- Symbols:
  - `default_data_roots` (function, line 49) `def default_data_roots(tts_dir, ps_dir)`
  - `evaluate` (function, line 60) `def evaluate(model, feature_fn, loader, device)`
  - `train` (function, line 88) `def train(args)`
  - `build_argparser` (function, line 275) `def build_argparser()`
  - `main` (function, line 317) `def main()`
  - `lr_at` (function, line 193) `def lr_at(step)`
- Depends on: `micro/stt-training/stt_training/augment.py`, `micro/stt-training/stt_training/dataset.py`, `micro/stt-training/stt_training/features.py`, `micro/stt-training/stt_training/model.py`, `micro/stt-training/stt_training/words.py`
- Imported by: `micro/stt-training/stt_training/evaluate.py`

## micro/stt-training/stt_training/words.py
- Layer: utility
- Language: py
- Symbols:
  - `folder_for_word` (function, line 18) `def folder_for_word(word)`
  - `load_words` (function, line 31) `def load_words(path)`
  - `resolve_classes` (function, line 53) `def resolve_classes(path, include_unknown)`
- Imported by: `micro/stt-training/stt_training/__init__.py`, `micro/stt-training/stt_training/train.py`, `micro/stt-training/tools/extract_clips.py`, `micro/stt-training/tools/mine_peoples_speech.py`, `micro/stt-training/tools/synthesize.py`
