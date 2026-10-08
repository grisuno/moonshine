# Subsystem: micro_stt_src

## micro/stt/src/classifier.cc
- Doc: TFLM-based on-device classifier.
- Layer: utility
- Language: cc
- Symbols:
  - `Saturate8` (function, line 26) `inline int8_t Saturate8(float v)`
  - `Classifier` (function, line 53) `Classifier::Classifier(const unsigned char* model_data,
                       unsigned int /*mod...`
  - `Run` (function, line 226) `void Classifier::Run(const float* features, float* logits_out) const`
- Depends on: `micro/stt/include/stt/stt.h`

## micro/stt/src/predictor.cc
- Layer: utility
- Language: cc
- Symbols:
  - `Argmax` (function, line 7) `int Argmax(const float* logits, int n_logits)`
  - `SoftmaxProb` (function, line 20) `float SoftmaxProb(const float* logits, int n_logits, int index)`
- Depends on: `micro/stt/include/stt/stt.h`
