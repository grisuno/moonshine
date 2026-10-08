# Subsystem: micro_vad_src

## micro/vad/src/vad.cc
- Doc: TFLM-based on-device VAD inference.
- Layer: utility
- Language: cc
- Symbols:
  - `Saturate8` (function, line 22) `inline int8_t Saturate8(float v)`
  - `Vad` (function, line 38) `Vad::Vad(const unsigned char* model_data, unsigned int /*model_size*/,
         uint8_t* tensor_a...`
  - `Predict` (function, line 171) `float Vad::Predict(const float* features) const`
- Depends on: `micro/vad/include/vad/vad.h`

## micro/vad/src/vad_segmenter.cc
- Layer: utility
- Language: cc
- Symbols:
  - `VadSegmenter` (function, line 6) `VadSegmenter::VadSegmenter(float threshold, int window_frames, int hop,
                         ...`
  - `Start` (function, line 22) `void VadSegmenter::Start()`
  - `ProcessFrame` (function, line 32) `VadEvent VadSegmenter::ProcessFrame(float raw_probability)`
  - `Finish` (function, line 84) `VadEvent VadSegmenter::Finish()`
  - `ExtractClipFrontAligned` (function, line 93) `void ExtractClipFrontAligned(const float* src, std::size_t src_len,
                             ...`
  - `EnergyCentroidIndex` (function, line 106) `std::size_t EnergyCentroidIndex(const int16_t* buf, std::size_t start,
                          ...`
- Depends on: `micro/vad/include/vad/vad.h`
