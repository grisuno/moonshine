# Subsystem: src

## micro/vad/src/vad.cc
- Layer: utility
- Doc: TFLM-based on-device VAD inference. See vad.h for the contract.  Op set is identical to the SpellingCNN's (the TinyVadCN
- Language: cc
- Symbols:
  - `Saturate8` (function, line 21) `inline int8_t Saturate8(float v)`
  - `Vad` (function, line 37) `Vad::Vad(const unsigned char* model_data, unsigned int /*model_size*/,
         uint8_t* tensor_a...`
  - `Predict` (function, line 170) `float Vad::Predict(const float* features) const`

## micro/vad/src/vad_segmenter.cc
- Layer: utility
- Doc: include "tensorflow/lite/micro/micro_log.h" include "vad/vad.h"
- Language: cc
- Symbols:
  - `VadSegmenter` (function, line 5) `VadSegmenter::VadSegmenter(float threshold, int window_frames, int hop,
                         ...`
  - `Start` (function, line 21) `void VadSegmenter::Start()`
  - `ProcessFrame` (function, line 31) `VadEvent VadSegmenter::ProcessFrame(float raw_probability)`
  - `Finish` (function, line 83) `VadEvent VadSegmenter::Finish()`
  - `ExtractClipFrontAligned` (function, line 92) `void ExtractClipFrontAligned(const float* src, std::size_t src_len,
                             ...`
  - `EnergyCentroidIndex` (function, line 105) `std::size_t EnergyCentroidIndex(const int16_t* buf, std::size_t start,
                          ...`
