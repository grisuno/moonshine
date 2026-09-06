# Subsystem: tflm_ref

## micro/neural-tts/host/tflm_ref/add.cpp
- Layer: utility
- Doc: Copyright 2021 The TensorFlow Authors. All Rights Reserved.
- Language: cpp
- Symbols:
  - `EvalAdd` (function, line 34) `TfLiteStatus EvalAdd(TfLiteContext* context, TfLiteNode* node,
                     TfLiteAddPara...`
  - `EvalAddQuantized` (function, line 90) `TfLiteStatus EvalAddQuantized(TfLiteContext* context, TfLiteNode* node,
                         ...`
  - `AddInit` (function, line 162) `void* AddInit(TfLiteContext* context, const char* buffer, size_t length)`
  - `AddEval` (function, line 167) `TfLiteStatus AddEval(TfLiteContext* context, TfLiteNode* node)`
  - `Register_ADD` (function, line 195) `TFLMRegistration Register_ADD()`

## micro/neural-tts/host/tflm_ref/conv.cpp
- Layer: utility
- Doc: Copyright 2024 The TensorFlow Authors. All Rights Reserved.
- Language: cpp
- Symbols:
  - `ConvEval` (function, line 37) `TfLiteStatus ConvEval(TfLiteContext* context, TfLiteNode* node)`
  - `Register_CONV_2D` (function, line 128) `TFLMRegistration Register_CONV_2D()`

## micro/neural-tts/host/tflm_ref/host_platform.cpp
- Layer: data_access
- Doc: Host (desktop) implementations of the TFLM platform hooks the RP2350 build gets from pico-tflmicro's system_setup.cpp / 
- Language: cpp
- Symbols:
  - `InitializeTarget` (function, line 25) `void InitializeTarget()`
  - `ticks_per_second` (function, line 27) `uint32_t ticks_per_second()`
  - `GetCurrentTimeTicks` (function, line 29) `uint32_t GetCurrentTimeTicks()`

## micro/neural-tts/host/tflm_ref/transpose_conv.cpp
- Layer: utility
- Doc: Copyright 2024 The TensorFlow Authors. All Rights Reserved.
- Language: cpp
- Symbols:
  - `OpData` (struct, line 36)
  - `RuntimePaddingType` (function, line 59) `inline PaddingType RuntimePaddingType(TfLitePadding padding)`
  - `CalculateOpData` (function, line 71) `TfLiteStatus CalculateOpData(TfLiteContext* context, TfLiteNode* node,
                          ...`
  - `TransposeConvInit` (function, line 145) `void* TransposeConvInit(TfLiteContext* context, const char* buffer,
                        size_...`
  - `TransposeConvPrepare` (function, line 151) `TfLiteStatus TransposeConvPrepare(TfLiteContext* context, TfLiteNode* node)`
  - `TransposeConvEval` (function, line 260) `TfLiteStatus TransposeConvEval(TfLiteContext* context, TfLiteNode* node)`
  - `Register_TRANSPOSE_CONV` (function, line 409) `TFLMRegistration Register_TRANSPOSE_CONV()`
