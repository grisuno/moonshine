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
  - `SetActivationParams` (function, line 42) `SetActivationParams(data->output_activation_min_f32, data->output_activation_max_f32, &op_params);`
  - `BroadcastAdd4DSlow` (function, line 45) `reference_ops::BroadcastAdd4DSlow( op_params, tflite::micro::GetTensorShape(input1), tflite::micro::GetTensorData<float>(input1), tflite::micro::GetTensorShape(input2), tflite::micro::GetTensorData<fl`
  - `Add` (function, line 53) `reference_ops::Add(op_params, tflite::micro::GetTensorShape(input1), tflite::micro::GetTensorData<float>(input1), tflite::micro::GetTensorShape(input2), tflite::micro::GetTensorData<float>(input2), tf`
  - `MicroPrintf` (function, line 82) `default: MicroPrintf("Type %s (%d) not supported.", TfLiteTypeGetName(output->type), output->type);`
  - `GetTensorShape` (function, line 110) `tflite::micro::GetTensorShape(input1), tflite::micro::GetTensorShape(input2), &op_params);`
  - `TFLITE_DCHECK` (function, line 164) `TFLITE_DCHECK(context->AllocatePersistentBuffer != nullptr);`
  - `GetEvalInput` (function, line 175) `tflite::micro::GetEvalInput(context, node, kAddInputTensor1);`
  - `GetEvalOutput` (function, line 179) `tflite::micro::GetEvalOutput(context, node, kAddOutputTensor);`
  - `TF_LITE_ENSURE_OK` (function, line 182) `TF_LITE_ENSURE_OK( context, EvalAdd(context, node, params, data, input1, input2, output));`
  - `RegisterOp` (function, line 197) `return tflite::micro::RegisterOp(AddInit, AddPrepare, AddEval);`

## micro/neural-tts/host/tflm_ref/conv.cpp
- Layer: utility
- Doc: Copyright 2024 The TensorFlow Authors. All Rights Reserved.
- Language: cpp
- Symbols:
  - `ConvEval` (function, line 37) `TfLiteStatus ConvEval(TfLiteContext* context, TfLiteNode* node)`
  - `Register_CONV_2D` (function, line 128) `TFLMRegistration Register_CONV_2D()`
  - `GetEvalInput` (function, line 40) `tflite::micro::GetEvalInput(context, node, kConvInputTensor);`
  - `GetEvalOutput` (function, line 48) `tflite::micro::GetEvalOutput(context, node, kConvOutputTensor);`
  - `TFLITE_DCHECK` (function, line 49) `TFLITE_DCHECK(node->builtin_data != nullptr);`
  - `Conv` (function, line 58) `tflite::reference_ops::Conv( ConvParamsFloat(params, data), tflite::micro::GetTensorShape(input), tflite::micro::GetTensorData<float>(input), tflite::micro::GetTensorShape(filter), tflite::micro::GetT`
  - `MicroPrintf` (function, line 72) `MicroPrintf("Filter type %s (%d) not supported.", TfLiteTypeGetName(filter->type), filter->type);`
  - `ConvPerChannel` (function, line 76) `reference_integer_ops::ConvPerChannel( ConvParamsQuantized(params, data), data.per_channel_output_multiplier, data.per_channel_output_shift, tflite::micro::GetTensorShape(input), tflite::micro::GetTen`
  - `RegisterOp` (function, line 130) `return tflite::micro::RegisterOp(ConvInit, ConvPrepare, ConvEval);`

## micro/neural-tts/host/tflm_ref/host_platform.cpp
- Layer: data_access
- Doc: Host (desktop) implementations of the TFLM platform hooks the RP2350 build gets from pico-tflmicro's system_setup.cpp / 
- Language: cpp
- Symbols:
  - `InitializeTarget` (function, line 25) `void InitializeTarget()`
  - `ticks_per_second` (function, line 27) `uint32_t ticks_per_second()`
  - `GetCurrentTimeTicks` (function, line 29) `uint32_t GetCurrentTimeTicks()`
  - `vfprintf` (function, line 16) `vfprintf(stderr, format, args);`
  - `vsnprintf` (function, line 21) `return vsnprintf(buffer, buf_size, format, vlist);`

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
  - `TF_LITE_ENSURE` (function, line 78) `TF_LITE_ENSURE(context, has_bias || node->inputs->size == 3);`
  - `TF_LITE_ENSURE_EQ` (function, line 79) `TF_LITE_ENSURE_EQ(context, node->outputs->size, 1);`
  - `TF_LITE_ENSURE_STATUS` (function, line 112) `TF_LITE_ENSURE_STATUS(tflite::PopulateConvolutionQuantizationParams( context, input, filter, bias, output, params->activation, &data->params.output_multiplier, &data->params.output_shift, &data->param`
  - `TFLITE_DCHECK` (function, line 124) `TFLITE_DCHECK(filter->type == kTfLiteInt8);`
  - `TF_LITE_ENSURE_MSG` (function, line 171) `TF_LITE_ENSURE_MSG( context, input->type == filter->type || (input->type == kTfLiteInt16 && filter->type == kTfLiteInt8), "Hybrid models are not supported on TFLite Micro.");`
  - `GetEvalInput` (function, line 263) `tflite::micro::GetEvalInput(context, node, kTransposeConvInputTensor);`
  - `GetEvalOutput` (function, line 271) `tflite::micro::GetEvalOutput(context, node, kTransposeConvOutputTensor);`
  - `CalculateActivationRange` (function, line 294) `CalculateActivationRange(params.activation, &op_params.float_activation_min, &op_params.float_activation_max);`
  - `TransposeConv` (function, line 297) `reference_ops::TransposeConv( op_params, tflite::micro::GetTensorShape(input), tflite::micro::GetTensorData<float>(input), tflite::micro::GetTensorShape(filter), #ifdef USE_TFLM_COMPRESSION tflite::mi`
  - `MicroPrintf` (function, line 400) `default: MicroPrintf("Type %s (%d) not supported.", TfLiteTypeGetName(input->type), input->type);`
  - `RegisterOp` (function, line 411) `return tflite::micro::RegisterOp(TransposeConvInit, TransposeConvPrepare, TransposeConvEval);`
