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
  - `MicroPrintf` (function, line 44) `MicroPrintf("VAD model schema version %d != supported %d", static_cast<int>(model->version()), static_cast<int>(TFLITE_SCHEMA_VERSION));`
  - `new` (function, line 71) `new (place_at(off, sizeof(tflite::MicroMutableOpResolver<8>))) tflite::MicroMutableOpResolver<8>();`
  - `MicroInterpreter` (function, line 95) `tflite::MicroInterpreter(model, *impl_->resolver, working_arena, working_size, /*resource_variables=*/nullptr, profiler);`
- Depends on: `micro/vad/include/vad/vad.h`

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
- Depends on: `micro/vad/include/vad/vad.h`
