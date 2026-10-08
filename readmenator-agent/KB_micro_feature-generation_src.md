# Subsystem: micro_feature-generation_src

## micro/feature-generation/src/fft_scratch.cc
- Layer: utility
- Language: cc
- Depends on: `micro/feature-generation/src/fft_scratch.h`

## micro/feature-generation/src/fft_scratch.h
- Doc: Shared FFT scratch pool for the on-device log-mel front-ends.
- Layer: utility
- Language: h
- Symbols:
  - `g_fft_scratch_frame` (variable, line 32) `extern float g_fft_scratch_frame[kFftScratchNFft];`
  - `g_fft_scratch_spec` (variable, line 33) `extern kiss_fft_cpx g_fft_scratch_spec[kFftScratchNFreq];`
  - `g_fft_scratch_pow` (variable, line 34) `extern float g_fft_scratch_pow[kFftScratchNFreq];`
  - `FEATURE_GENERATION_FFT_SCRATCH_H_` (macro, line 21) `#define FEATURE_GENERATION_FFT_SCRATCH_H_`
- Imported by: `micro/feature-generation/src/fft_scratch.cc`, `micro/feature-generation/src/log_mel.cc`, `micro/feature-generation/src/mel_streamer.cc`

## micro/feature-generation/src/log_mel.cc
- Doc: Heap-free log-mel spectrogram for the on-device build.
- Layer: utility
- Language: cc
- Symbols:
  - `ReflectIndex` (function, line 69) `inline int ReflectIndex(int i, int n)`
  - `ToFloatSample` (function, line 87) `inline float ToFloatSample(float s)`
  - `ToFloatSample` (function, line 88) `inline float ToFloatSample(int16_t s)`
  - `HzToMelSlaney` (function, line 93) `float HzToMelSlaney(float hz)`
  - `MelToHzSlaney` (function, line 100) `float MelToHzSlaney(float mel)`
  - `HannWindowPeriodic` (function, line 107) `std::vector<float> HannWindowPeriodic(int length)`
  - `MakeMelFilterbank` (function, line 121) `std::vector<float> MakeMelFilterbank(int n_freq, int n_mels, int sample_rate,
                   ...`
  - `LogMelSpectrogram` (function, line 163) `LogMelSpectrogram::LogMelSpectrogram(const LogMelParams& params)
    : params_(params), n_freq_(p...`
  - `ComputeImpl` (function, line 313) `template <typename SampleT>
void LogMelSpectrogram::ComputeImpl(const SampleT* waveform,
        ...`
  - `Compute` (function, line 439) `void LogMelSpectrogram::Compute(const float* waveform, std::size_t n_samples,
                   ...`
  - `Compute` (function, line 444) `void LogMelSpectrogram::Compute(const int16_t* waveform, std::size_t n_samples,
                 ...`
  - `exp` (function, line 102) `return kMinLogHz * std::exp(kLogStep * (mel - kMinLogMel));`
  - `w` (function, line 112) `std::vector<float> w(length);`
  - `mel_pts` (function, line 126) `std::vector<float> mel_pts(static_cast<std::size_t>(n_mels + 2));`
  - `hz_pts` (function, line 132) `std::vector<float> hz_pts(mel_pts.size());`
  - `bin_hz` (function, line 136) `std::vector<float> bin_hz(static_cast<std::size_t>(n_freq));`
  - `fb` (function, line 142) `std::vector<float> fb( static_cast<std::size_t>(n_mels) * static_cast<std::size_t>(n_freq), 0.0f);`
- Depends on: `micro/feature-generation/include/feature_generation/feature_generation.h`, `micro/feature-generation/src/fft_scratch.h`

## micro/feature-generation/src/mel_streamer.cc
- Layer: utility
- Language: cc
- Symbols:
  - `MelStreamer` (function, line 10) `MelStreamer::MelStreamer(int n_mels, int window_frames, int n_fft,
                         const...`
  - `Reset` (function, line 39) `void MelStreamer::Reset()`
  - `PushHop` (function, line 53) `void MelStreamer::PushHop(const float* hop_samples)`
  - `BuildModelInput` (function, line 93) `void MelStreamer::BuildModelInput(float* out) const`
- Depends on: `micro/feature-generation/include/feature_generation/feature_generation.h`, `micro/feature-generation/src/fft_scratch.h`
