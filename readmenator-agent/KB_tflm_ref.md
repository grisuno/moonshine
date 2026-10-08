# Subsystem: tflm_ref

## micro/neural-tts/host/tflm_ref/add.cpp
- Doc: Copyright 2021 The TensorFlow Authors.
- Layer: utility
- Language: cpp
- Symbols:
  - `EvalAdd` (function, line 35) `TfLiteStatus EvalAdd(TfLiteContext* context, TfLiteNode* node,
                     TfLiteAddPara...`
  - `EvalAddQuantized` (function, line 91) `TfLiteStatus EvalAddQuantized(TfLiteContext* context, TfLiteNode* node,
                         ...`
  - `AddInit` (function, line 163) `void* AddInit(TfLiteContext* context, const char* buffer, size_t length)`
  - `AddEval` (function, line 168) `TfLiteStatus AddEval(TfLiteContext* context, TfLiteNode* node)`
  - `Register_ADD` (function, line 196) `TFLMRegistration Register_ADD()`

## micro/neural-tts/host/tflm_ref/conv.cpp
- Doc: Copyright 2024 The TensorFlow Authors.
- Layer: utility
- Language: cpp
- Symbols:
  - `ConvEval` (function, line 38) `TfLiteStatus ConvEval(TfLiteContext* context, TfLiteNode* node)`
  - `Register_CONV_2D` (function, line 129) `TFLMRegistration Register_CONV_2D()`

## micro/neural-tts/host/tflm_ref/host_platform.cpp
- Doc: Host (desktop) implementations of the TFLM platform hooks the RP2350 build gets from...
- Layer: utility
- Language: cpp
- Symbols:
  - `InitializeTarget` (function, line 26) `void InitializeTarget()`
  - `ticks_per_second` (function, line 28) `uint32_t ticks_per_second()`
  - `GetCurrentTimeTicks` (function, line 30) `uint32_t GetCurrentTimeTicks()`

## micro/neural-tts/host/tflm_ref/transpose_conv.cpp
- Doc: Copyright 2024 The TensorFlow Authors.
- Layer: utility
- Language: cpp
- Symbols:
  - `OpData` (struct, line 36)
  - `RuntimePaddingType` (function, line 60) `inline PaddingType RuntimePaddingType(TfLitePadding padding)`
  - `CalculateOpData` (function, line 72) `TfLiteStatus CalculateOpData(TfLiteContext* context, TfLiteNode* node,
                          ...`
  - `TransposeConvInit` (function, line 146) `void* TransposeConvInit(TfLiteContext* context, const char* buffer,
                        size_...`
  - `TransposeConvPrepare` (function, line 152) `TfLiteStatus TransposeConvPrepare(TfLiteContext* context, TfLiteNode* node)`
  - `TransposeConvEval` (function, line 261) `TfLiteStatus TransposeConvEval(TfLiteContext* context, TfLiteNode* node)`
  - `Register_TRANSPOSE_CONV` (function, line 410) `TFLMRegistration Register_TRANSPOSE_CONV()`
