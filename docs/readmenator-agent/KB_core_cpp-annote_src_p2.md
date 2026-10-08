# Subsystem: core_cpp-annote_src (page 2 of 2)
Previous: [KB_core_cpp-annote_src.md](KB_core_cpp-annote_src.md)

## core/cpp-annote/src/wav_pcm_float32.h
- Doc: load_wav_pcm16_mono_float32: PCM 16 LE mono or stereo (mean to mono) → float32 mono...
- Layer: utility
- Language: h
- Symbols:
  - `read_file_bytes` (function, line 18) `inline std::vector<std::uint8_t> read_file_bytes(const std::string& path)`
  - `u32` (function, line 37) `inline std::uint32_t u32(const std::uint8_t* p)`
  - `u16` (function, line 44) `inline std::uint16_t u16(const std::uint8_t* p)`
  - `load_wav_pcm16_mono_float32` (function, line 51) `inline std::vector<float> load_wav_pcm16_mono_float32(const std::string& path,
                  ...`
  - `linear_resample` (function, line 120) `inline std::vector<float> linear_resample(const std::vector<float>& x,
                          ...`
  - `buf` (function, line 29) `std::vector<std::uint8_t> buf(static_cast<size_t>(sz));`
  - `mono` (function, line 104) `std::vector<float> mono(num_frames);`
  - `y` (function, line 132) `std::vector<float> y(n_out);`
  - `WAV_PCM_FLOAT32_H_` (macro, line 6) `#define WAV_PCM_FLOAT32_H_`
- Imported by: `core/cpp-annote/src/cpp-annote-streaming.cpp`, `core/cpp-annote/src/cpp-annote.cpp`, `core/reliability/fuzz-wav-pcm.cpp`

