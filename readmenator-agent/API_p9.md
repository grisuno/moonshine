# API (page 9 of 10)
Previous: [API_p8.md](API_p8.md)

## micro/stt-training/stt_training/features.py
Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/export.py`, `micro/stt-training/stt_training/train.py`
- `LogMelSpectrogram.__init__` (method) `micro/stt-training/stt_training/features.py:23` `def __init__(self, sample_rate, n_fft, hop_length, n_mels, f_min, f_max, target_frames, eps)`
- `LogMelSpectrogram.forward` (method) `micro/stt-training/stt_training/features.py:58` `def forward(self, waveform)`
- `SpecAugment.__init__` (method) `micro/stt-training/stt_training/features.py:73` `def __init__(self, freq_mask_param, time_mask_param, n_freq_masks, n_time_masks)`
- `SpecAugment.forward` (method) `micro/stt-training/stt_training/features.py:86` `def forward(self, x)`

## micro/stt-training/stt_training/model.py
Imported by: `micro/stt-training/stt_training/checkpoint.py`, `micro/stt-training/stt_training/train.py`
- `normalize_stride` (function) `micro/stt-training/stt_training/model.py:27` `def normalize_stride(v)` -- Coerce an int / ``"2,2"`` string / tuple into ``(freq_stride, time_stride)``.
- `ConvBNAct.__init__` (method) `micro/stt-training/stt_training/model.py:47` `def __init__(self, in_c, out_c, kernel, stride, groups, act)`
- `InvertedResidual.__init__` (method) `micro/stt-training/stt_training/model.py:61` `def __init__(self, in_c, out_c, stride, expand_ratio)`
- `InvertedResidual.forward` (method) `micro/stt-training/stt_training/model.py:77` `def forward(self, x)`
- `WordCNN.__init__` (method) `micro/stt-training/stt_training/model.py:100` `def __init__(self, num_classes, width_mult, dropout, stem_stride, pad_to_odd)`
- `WordCNN.forward` (method) `micro/stt-training/stt_training/model.py:157` `def forward(self, x)`
- `WordCNN.build_model` (method) `micro/stt-training/stt_training/model.py:167` `def build_model(num_classes)`

## micro/stt-training/stt_training/train.py
Depends on: `micro/stt-training/stt_training/augment.py`, `micro/stt-training/stt_training/dataset.py`, `micro/stt-training/stt_training/features.py`, `micro/stt-training/stt_training/model.py`, `micro/stt-training/stt_training/words.py`
Imported by: `micro/stt-training/stt_training/evaluate.py`
- `default_data_roots` (function) `micro/stt-training/stt_training/train.py:49` `def default_data_roots(tts_dir, ps_dir)` -- Discover training roots: one per ZipVoice speaker, plus People's Speech.
- `evaluate` (function) `micro/stt-training/stt_training/train.py:60` `def evaluate(model, feature_fn, loader, device)`
- `train` (function) `micro/stt-training/stt_training/train.py:88` `def train(args)`
- `lr_at` (function) `micro/stt-training/stt_training/train.py:193` `def lr_at(step)`
- `build_argparser` (function) `micro/stt-training/stt_training/train.py:275` `def build_argparser()`
- `main` (function) `micro/stt-training/stt_training/train.py:317` `def main()`

## micro/stt-training/stt_training/words.py
Imported by: `micro/stt-training/stt_training/__init__.py`, `micro/stt-training/stt_training/train.py`, `micro/stt-training/tools/extract_clips.py`, `micro/stt-training/tools/mine_peoples_speech.py`, `micro/stt-training/tools/synthesize.py`
- `folder_for_word` (function) `micro/stt-training/stt_training/words.py:18` `def folder_for_word(word)` -- Filesystem-safe label folder for a word.
- `load_words` (function) `micro/stt-training/stt_training/words.py:31` `def load_words(path)` -- Load command words from ``words.txt`` (one per line, ``#`` comments).
- `resolve_classes` (function) `micro/stt-training/stt_training/words.py:53` `def resolve_classes(path, include_unknown)` -- Return the ordered class list: command words plus the reject class.

## micro/stt-training/tools/download_musan_rirs.py
- `download_musan_noise` (function) `micro/stt-training/tools/download_musan_rirs.py:37` `def download_musan_noise(out_dir, small, seed)`
- `download_rirs` (function) `micro/stt-training/tools/download_musan_rirs.py:67` `def download_rirs(out_dir, max_files, seed)`
- `main` (function) `micro/stt-training/tools/download_musan_rirs.py:94` `def main()`

## micro/stt-training/tools/extract_clips.py
Depends on: `micro/stt-training/stt_training/words.py`
- `MMSAligner.__init__` (method) `micro/stt-training/tools/extract_clips.py:56` `def __init__(self, device, with_star)`
- `MMSAligner.align` (method) `micro/stt-training/tools/extract_clips.py:74` `def align(self, audio_1d, words)` -- Return one ``AlignedWord`` per input word (``None`` if unpronounceable).
- `MMSAligner.main` (method) `micro/stt-training/tools/extract_clips.py:171` `def main()`
- `MMSAligner.emit` (method) `micro/stt-training/tools/extract_clips.py:212` `def emit(label, clip_id, char_start, speaker, clip, sample_rate)`

## micro/stt-training/tools/mine_peoples_speech.py
Depends on: `micro/stt-training/stt_training/words.py`
- `_ShardReader.__init__` (method) `micro/stt-training/tools/mine_peoples_speech.py:90` `def __init__(self, shard, max_attempts)`
- `_ShardReader.num_row_groups` (method) `micro/stt-training/tools/mine_peoples_speech.py:103` `def num_row_groups(self)`
- `_ShardReader.row_group_num_rows` (method) `micro/stt-training/tools/mine_peoples_speech.py:106` `def row_group_num_rows(self, rg)`
- `_ShardReader.read_columns` (method) `micro/stt-training/tools/mine_peoples_speech.py:109` `def read_columns(self, rg, columns)`
- `_ShardReader.iter_peoples_speech` (method) `micro/stt-training/tools/mine_peoples_speech.py:131` `def iter_peoples_speech(config, split, offset, limit)` -- Yield ``(clip_id, transcript, speaker, fetch_audio)`` rows.
- `_ShardReader.find_matches` (method) `micro/stt-training/tools/mine_peoples_speech.py:191` `def find_matches(text, targets)` -- Return ``[(label, char_start, char_end), ...]`` for command words in text.
- `_ShardReader.save_audio_16k` (method) `micro/stt-training/tools/mine_peoples_speech.py:211` `def save_audio_16k(fetch, out_path)`
- `_ShardReader.main` (method) `micro/stt-training/tools/mine_peoples_speech.py:247` `def main()`

## micro/stt-training/tools/synthesize.py
Depends on: `micro/stt-training/stt_training/words.py`
- `discover_voices` (function) `micro/stt-training/tools/synthesize.py:58` `def discover_voices(language)` -- Return the installed ZipVoice speakers, falling back to the known list.
- `main` (function) `micro/stt-training/tools/synthesize.py:85` `def main()`

## micro/stt/include/stt/stt.h
Imported by: `micro/examples/rp2350/src/audio_service.cc`, `micro/examples/rp2350/src/test_app.cc`, `micro/stt/src/classifier.cc`, `micro/stt/src/predictor.cc`, `micro/stt/tests/predictor_test.cc`
- `Run` (function) `micro/stt/include/stt/stt.h:60` `void Run(const float* features, float* logits_out) const;` -- Run a single inference.
- `feature_scratch` (function) `micro/stt/include/stt/stt.h:65` `float* feature_scratch() const` -- Scratch for the fp32 log-mel features, carved from the arena's activation overlay (dead until Invoke()).
- `input_quant` (function) `micro/stt/include/stt/stt.h:67` `TensorQuant input_quant() const`
- `output_quant` (function) `micro/stt/include/stt/stt.h:68` `TensorQuant output_quant() const`
- `n_classes` (function) `micro/stt/include/stt/stt.h:69` `int n_classes() const`
- `input_count` (function) `micro/stt/include/stt/stt.h:70` `std::size_t input_count() const`
- `arena_used_bytes` (function) `micro/stt/include/stt/stt.h:71` `std::size_t arena_used_bytes() const`
- `Argmax` (function) `micro/stt/include/stt/stt.h:90` `int Argmax(const float* logits, int n_logits);` -- Index of the largest logit.
- `SoftmaxProb` (function) `micro/stt/include/stt/stt.h:93` `float SoftmaxProb(const float* logits, int n_logits, int index);` -- Stable-softmax probability of `index` (subtracts max(logits) before exp()).

## micro/stt/scripts/desktop_parity.py
Depends on: `micro/stt/scripts/generate_embedded_data.py`
- `main` (function) `micro/stt/scripts/desktop_parity.py:111` `def main(argv)`

## micro/stt/scripts/generate_embedded_data.py
Imported by: `micro/stt/scripts/desktop_parity.py`, `micro/vad/scripts/generate_vad_embedded_data.py`
- `main` (function) `micro/stt/scripts/generate_embedded_data.py:680` `def main(argv)`

## micro/stt/src/classifier.cc
Depends on: `micro/stt/include/stt/stt.h`
- `Saturate8` (function) `micro/stt/src/classifier.cc:26` `inline int8_t Saturate8(float v)` -- Saturating round-and-cast for the input-quantization step.
- `Classifier` (function) `micro/stt/src/classifier.cc:53` `Classifier::Classifier(const unsigned char* model_data,
                       unsigned int /*mod...`
- `Run` (function) `micro/stt/src/classifier.cc:226` `void Classifier::Run(const float* features, float* logits_out) const`

## micro/stt/src/predictor.cc
Depends on: `micro/stt/include/stt/stt.h`
- `Argmax` (function) `micro/stt/src/predictor.cc:7` `int Argmax(const float* logits, int n_logits)`
- `SoftmaxProb` (function) `micro/stt/src/predictor.cc:20` `float SoftmaxProb(const float* logits, int n_logits, int index)`

## micro/vad/include/vad/vad.h
Imported by: `micro/examples/rp2350/src/audio_service.cc`, `micro/examples/rp2350/src/test_app.cc`, `micro/vad/src/vad.cc`, `micro/vad/src/vad_segmenter.cc`, `micro/vad/tests/vad_segmenter_test.cc`
- `Predict` (function) `micro/vad/include/vad/vad.h:60` `float Predict(const float* features) const;` -- Run one inference on a (n_mels * window_frames) row-major fp32 log-mel window; returns the speech probability in [0...
- `feature_scratch` (function) `micro/vad/include/vad/vad.h:64` `float* feature_scratch() const` -- Scratch for the fp32 log-mel window, borrowed from the arena overlay (dead until Invoke()).
- `input_quant` (function) `micro/vad/include/vad/vad.h:66` `VadTensorQuant input_quant() const`
- `output_quant` (function) `micro/vad/include/vad/vad.h:67` `VadTensorQuant output_quant() const`
- `input_count` (function) `micro/vad/include/vad/vad.h:68` `std::size_t input_count() const`
- `arena_used_bytes` (function) `micro/vad/include/vad/vad.h:69` `std::size_t arena_used_bytes() const`
- `Start` (function) `micro/vad/include/vad/vad.h:103` `void Start();` -- Reset all state to begin a fresh stream.
- `segment_start_sample` (function) `micro/vad/include/vad/vad.h:113` `std::size_t segment_start_sample() const` -- Boundaries (absolute sample indices) of the most-recent segment.
- `segment_end_sample` (function) `micro/vad/include/vad/vad.h:114` `std::size_t segment_end_sample() const`
- `samples_processed` (function) `micro/vad/include/vad/vad.h:115` `std::size_t samples_processed() const`
- `ExtractClipFrontAligned` (function) `micro/vad/include/vad/vad.h:135` `void ExtractClipFrontAligned(const float* src, std::size_t src_len, std::size_t start, std::size_t end, float* out...` -- Front-aligned pad/truncate of src[start, end) into out[0, clip_len): take from the segment start, zero-pad the tail.
- `EnergyCentroidIndex` (function) `micro/vad/include/vad/vad.h:145` `std::size_t EnergyCentroidIndex(const int16_t* buf, std::size_t start, std::size_t end);` -- Power-weighted centroid sample index over buf[start, end): round( sum(i * buf[i]^2) / sum(buf[i]^2) ).

## micro/vad/scripts/generate_vad_embedded_data.py
Depends on: `micro/stt/scripts/generate_embedded_data.py`
- `main` (function) `micro/vad/scripts/generate_vad_embedded_data.py:229` `def main(argv)`

## micro/vad/src/vad.cc
Depends on: `micro/vad/include/vad/vad.h`
- `Saturate8` (function) `micro/vad/src/vad.cc:22` `inline int8_t Saturate8(float v)`
- `Vad` (function) `micro/vad/src/vad.cc:38` `Vad::Vad(const unsigned char* model_data, unsigned int /*model_size*/,
         uint8_t* tensor_a...`
- `Predict` (function) `micro/vad/src/vad.cc:171` `float Vad::Predict(const float* features) const`

## micro/vad/src/vad_segmenter.cc
Depends on: `micro/vad/include/vad/vad.h`
- `VadSegmenter` (function) `micro/vad/src/vad_segmenter.cc:6` `VadSegmenter::VadSegmenter(float threshold, int window_frames, int hop,
                         ...`
- `Start` (function) `micro/vad/src/vad_segmenter.cc:22` `void VadSegmenter::Start()`
- `ProcessFrame` (function) `micro/vad/src/vad_segmenter.cc:32` `VadEvent VadSegmenter::ProcessFrame(float raw_probability)`
- `Finish` (function) `micro/vad/src/vad_segmenter.cc:84` `VadEvent VadSegmenter::Finish()`
- `ExtractClipFrontAligned` (function) `micro/vad/src/vad_segmenter.cc:93` `void ExtractClipFrontAligned(const float* src, std::size_t src_len,
                             ...`
- `EnergyCentroidIndex` (function) `micro/vad/src/vad_segmenter.cc:106` `std::size_t EnergyCentroidIndex(const int16_t* buf, std::size_t start,
                          ...`

## python/setup.py
- `BinaryDistribution.has_ext_modules` (method) `python/setup.py:10` `def has_ext_modules(self)`
- `PlatformWheel.finalize_options` (method) `python/setup.py:15` `def finalize_options(self)`
- `PlatformWheel.get_tag` (method) `python/setup.py:20` `def get_tag(self)`
- `PlatformWheel.read_readme` (method) `python/setup.py:26` `def read_readme()`
- `PlatformWheel.read_license` (method) `python/setup.py:32` `def read_license()`
- `PlatformWheel.read_requirements` (method) `python/setup.py:39` `def read_requirements()`

## python/src/moonshine_voice/alphanumeric_listener.py
Depends on: `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/moonshine_api.py`
Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `scripts/eval-alphanumeric.py`
- `AlphanumericMatch.is_character` (method) `python/src/moonshine_voice/alphanumeric_listener.py:80` `def is_character(self)`
- `AlphanumericMatch.is_terminator` (method) `python/src/moonshine_voice/alphanumeric_listener.py:84` `def is_terminator(self)`
- `AlphanumericMatch.is_recognized` (method) `python/src/moonshine_voice/alphanumeric_listener.py:88` `def is_recognized(self)`
- `AlphanumericMatch.spoken_form` (method) `python/src/moonshine_voice/alphanumeric_listener.py:306` `def spoken_form(char)` -- Return a TTS-friendly phrase for a single character.
- `AlphanumericMatcher.__init__` (method) `python/src/moonshine_voice/alphanumeric_listener.py:542` `def __init__(self)`
- `AlphanumericMatcher.classify` (method) `python/src/moonshine_voice/alphanumeric_listener.py:570` `def classify(self, raw_text)` -- Classify a single utterance into an :class:`AlphanumericMatch`.
- `AlphanumericMatcher.classify_sequence` (method) `python/src/moonshine_voice/alphanumeric_listener.py:606` `def classify_sequence(self, raw_text)` -- Classify a potentially multi-token utterance.
- `AlphanumericMatcher.letters_only_matcher` (method) `python/src/moonshine_voice/alphanumeric_listener.py:716` `def letters_only_matcher()`
- `AlphanumericMatcher.digits_only_matcher` (method) `python/src/moonshine_voice/alphanumeric_listener.py:720` `def digits_only_matcher()`
- `AlphanumericListener.__init__` (method) `python/src/moonshine_voice/alphanumeric_listener.py:808` `def __init__(self, callback)`
- `AlphanumericListener.__call__` (method) `python/src/moonshine_voice/alphanumeric_listener.py:829` `def __call__(self, event)`
- `AlphanumericListener.text` (method) `python/src/moonshine_voice/alphanumeric_listener.py:840` `def text(self)` -- The currently assembled text.
- `AlphanumericListener.stopped` (method) `python/src/moonshine_voice/alphanumeric_listener.py:845` `def stopped(self)` -- Whether a stop command has been received.
- `AlphanumericListener.matcher` (method) `python/src/moonshine_voice/alphanumeric_listener.py:850` `def matcher(self)` -- The underlying :class:`AlphanumericMatcher`.
- `AlphanumericListener.clear` (method) `python/src/moonshine_voice/alphanumeric_listener.py:854` `def clear(self)` -- Programmatically clear the buffer.
- `AlphanumericListener.undo` (method) `python/src/moonshine_voice/alphanumeric_listener.py:865` `def undo(self)` -- Remove and return the last character, or ``None`` if empty.
- `AlphanumericListener.on_event` (method) `python/src/moonshine_voice/alphanumeric_listener.py:1063` `def on_event(event)`

## python/src/moonshine_voice/cached_embeddings.py
Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`
- `_EmbeddingBackend.calculate_embedding` (method) `python/src/moonshine_voice/cached_embeddings.py:52` `def calculate_embedding(self, sentence)`
- `_EmbeddingBackend.distance` (method) `python/src/moonshine_voice/cached_embeddings.py:54` `def distance(self, embedding_a, embedding_b)`
- `_EmbeddingBackend.default_cached_embeddings_path` (method) `python/src/moonshine_voice/cached_embeddings.py:62` `def default_cached_embeddings_path()` -- Return the absolute path of the packaged cached embeddings TSV.
- `CachedEmbeddings.__init__` (method) `python/src/moonshine_voice/cached_embeddings.py:95` `def __init__(self)`
- `CachedEmbeddings.active` (method) `python/src/moonshine_voice/cached_embeddings.py:150` `def active(self)` -- ``True`` when the cache has at least one usable entry.
- `CachedEmbeddings.path` (method) `python/src/moonshine_voice/cached_embeddings.py:155` `def path(self)`
- `CachedEmbeddings.metadata` (method) `python/src/moonshine_voice/cached_embeddings.py:159` `def metadata(self)`
- `CachedEmbeddings.phrases` (method) `python/src/moonshine_voice/cached_embeddings.py:163` `def phrases(self)` -- Return the list of cached phrases (normalized keys).
- `CachedEmbeddings.get` (method) `python/src/moonshine_voice/cached_embeddings.py:175` `def get(self, sentence)` -- Return the cached embedding or ``None`` if not present.
- `CachedEmbeddings.calculate_embedding` (method) `python/src/moonshine_voice/cached_embeddings.py:179` `def calculate_embedding(self, sentence)` -- Return the embedding for ``sentence``.
- `CachedEmbeddings.distance` (method) `python/src/moonshine_voice/cached_embeddings.py:195` `def distance(self, embedding_a, embedding_b)` -- Return the cosine similarity between two embedding vectors.
- `CachedEmbeddings.write_cached_embeddings_tsv` (method) `python/src/moonshine_voice/cached_embeddings.py:260` `def write_cached_embeddings_tsv(path, entries)` -- Write a TSV compatible with :class:`CachedEmbeddings`.

## python/src/moonshine_voice/cli.py
Imported by: `python/tests/test_cli.py`
- `main` (function) `python/src/moonshine_voice/cli.py:91` `def main(argv)` -- Dispatch to a subcommand.

## python/src/moonshine_voice/dialog_flow.py
Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/cached_embeddings.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/mic_transcriber.py`
- `EmbeddingBackend.calculate_embedding` (method) `python/src/moonshine_voice/dialog_flow.py:222` `def calculate_embedding(self, sentence)`
- `EmbeddingBackend.distance` (method) `python/src/moonshine_voice/dialog_flow.py:224` `def distance(self, embedding_a, embedding_b)`
- `PhraseMatcher.__init__` (method) `python/src/moonshine_voice/dialog_flow.py:255` `def __init__(self, backend, phrases_by_key)`
- `PhraseMatcher.threshold` (method) `python/src/moonshine_voice/dialog_flow.py:282` `def threshold(self)`
- `PhraseMatcher.match` (method) `python/src/moonshine_voice/dialog_flow.py:285` `def match(self, utterance)` -- Return the best-matching key, or *None* if below threshold.
- `PhraseMatcher.match_with_score` (method) `python/src/moonshine_voice/dialog_flow.py:290` `def match_with_score(self, utterance)` -- Return ``(key, similarity)`` of the best match above threshold.
- `Dialog.__init__` (method) `python/src/moonshine_voice/dialog_flow.py:345` `def __init__(self, trigger_phrase)`
- `Dialog.say` (method) `python/src/moonshine_voice/dialog_flow.py:350` `def say(self, text)`
- `Dialog.ask` (method) `python/src/moonshine_voice/dialog_flow.py:354` `def ask(self, prompt)`
- `Dialog.confirm` (method) `python/src/moonshine_voice/dialog_flow.py:374` `def confirm(self, prompt)`
- `Dialog.choose` (method) `python/src/moonshine_voice/dialog_flow.py:384` `def choose(self, prompt, options)`
- `Dialog.cancel` (method) `python/src/moonshine_voice/dialog_flow.py:402` `def cancel(self)`
- `Dialog.restart` (method) `python/src/moonshine_voice/dialog_flow.py:405` `def restart(self)`
- `Dialog.replay_last_prompt` (method) `python/src/moonshine_voice/dialog_flow.py:408` `def replay_last_prompt(self)` -- Return a :class:`Say` that re-speaks the most recent prompt.
- `_AlphaSession.__init__` (method) `python/src/moonshine_voice/dialog_flow.py:435` `def __init__(self, matcher)`
- `_ActiveFlow.__init__` (method) `python/src/moonshine_voice/dialog_flow.py:443` `def __init__(self, flow_fn, trigger_phrase)`
- `DialogFlow.__init__` (method) `python/src/moonshine_voice/dialog_flow.py:558` `def __init__(self)`
- `DialogFlow.register_flow` (method) `python/src/moonshine_voice/dialog_flow.py:662` `def register_flow(self, trigger_phrase, flow)` -- Register a flow function to be started when ``trigger_phrase`` fires.
- `DialogFlow.unregister_flow` (method) `python/src/moonshine_voice/dialog_flow.py:674` `def unregister_flow(self, trigger_phrase)`
- `DialogFlow.register_global` (method) `python/src/moonshine_voice/dialog_flow.py:680` `def register_global(self, trigger_phrase, handler)` -- Register a phrase that is always live, even while a flow runs.
- `DialogFlow.is_active` (method) `python/src/moonshine_voice/dialog_flow.py:697` `def is_active(self)`
- `DialogFlow.active_trigger` (method) `python/src/moonshine_voice/dialog_flow.py:702` `def active_trigger(self)`
- `DialogFlow.registered_flows` (method) `python/src/moonshine_voice/dialog_flow.py:707` `def registered_flows(self)`
- `DialogFlow.on_line_started` (method) `python/src/moonshine_voice/dialog_flow.py:712` `def on_line_started(self, event)` -- Tag any transcript line that opens while we're talking.
- `DialogFlow.on_line_completed` (method) `python/src/moonshine_voice/dialog_flow.py:746` `def on_line_completed(self, event)`
- `DialogFlow.on_error` (method) `python/src/moonshine_voice/dialog_flow.py:772` `def on_error(self, event)`
- `DialogFlow.process_utterance` (method) `python/src/moonshine_voice/dialog_flow.py:777` `def process_utterance(self, utterance)` -- Route an utterance.
- `DialogFlow.cancel_active` (method) `python/src/moonshine_voice/dialog_flow.py:1156` `def cancel_active(self)` -- Abandon any currently running flow.
- `DialogFlow.say` (method) `python/src/moonshine_voice/dialog_flow.py:1169` `def say(self, text)` -- Speak ``text`` through the configured TTS, outside any flow.
- `_Reprompt.__init__` (method) `python/src/moonshine_voice/dialog_flow.py:1620` `def __init__(self, text)`
- `_AbandonPrompt.__init__` (method) `python/src/moonshine_voice/dialog_flow.py:1625` `def __init__(self, exc)`
- `_SpelledPhrase.spell_out` (method) `python/src/moonshine_voice/dialog_flow.py:1656` `def spell_out(s)` -- Return ``s`` as a TTS-friendly spoken-form phrase.
- `_SpelledPhrase.wifi_setup` (method) `python/src/moonshine_voice/dialog_flow.py:1980` `def wifi_setup(d)`
- `_SpelledPhrase.mute` (method) `python/src/moonshine_voice/dialog_flow.py:2069` `def mute(should_mute)`
- `_SpelledPhrase.set_spelling_mode` (method) `python/src/moonshine_voice/dialog_flow.py:2073` `def set_spelling_mode(active)` -- Toggle the C++ spelling-CNN fusion path on the live mic stream.
- `_SpelledPhrase.speak` (method) `python/src/moonshine_voice/dialog_flow.py:2081` `def speak(text)` -- Log every spoken prompt and (optionally) pass it through TTS.
- `_CompletedLinePrinter.on_line_completed` (method) `python/src/moonshine_voice/dialog_flow.py:2105` `def on_line_completed(self, event)`

## python/src/moonshine_voice/download.py
Depends on: `python/src/moonshine_voice/download_file.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `scripts/analyze_ko_stress.py`, `scripts/compare_ko_phonemes.py`, `scripts/tts_g2p_intelligibility.py`
- `EmbeddingModelArch.find_model_info` (method) `python/src/moonshine_voice/download.py:168` `def find_model_info(language, model_arch)`
- `EmbeddingModelArch.supported_languages_friendly` (method) `python/src/moonshine_voice/download.py:197` `def supported_languages_friendly()`
- `EmbeddingModelArch.supported_languages` (method) `python/src/moonshine_voice/download.py:203` `def supported_languages()`
- `EmbeddingModelArch.get_components_for_model_info` (method) `python/src/moonshine_voice/download.py:207` `def get_components_for_model_info(model_info)`
- `EmbeddingModelArch.download_model_from_info` (method) `python/src/moonshine_voice/download.py:234` `def download_model_from_info(model_info)`
- `EmbeddingModelArch.supported_embedding_models` (method) `python/src/moonshine_voice/download.py:254` `def supported_embedding_models()` -- Return list of supported embedding model names.
- `EmbeddingModelArch.supported_embedding_models_friendly` (method) `python/src/moonshine_voice/download.py:259` `def supported_embedding_models_friendly()` -- Return a friendly string listing supported embedding models.
- `EmbeddingModelArch.get_embedding_model_variants` (method) `python/src/moonshine_voice/download.py:266` `def get_embedding_model_variants(model_name)` -- Return list of available variants for an embedding model.
- `EmbeddingModelArch.get_embedding_model` (method) `python/src/moonshine_voice/download.py:276` `def get_embedding_model(model_name, variant)` -- Download an embedding model and return (path, arch).
- `EmbeddingModelArch.download_spelling_model_for_language` (method) `python/src/moonshine_voice/download.py:365` `def download_spelling_model_for_language(language)` -- Download the alphanumeric spelling model for ``language`` if one is available, and return the path to the...
- `EmbeddingModelArch.get_spelling_model_path` (method) `python/src/moonshine_voice/download.py:395` `def get_spelling_model_path(language)` -- Return the on-disk path to the spelling model for ``language``.
- `EmbeddingModelArch.get_model_for_language` (method) `python/src/moonshine_voice/download.py:410` `def get_model_for_language(wanted_language, wanted_model_arch)`
- `EmbeddingModelArch.log_model_info` (method) `python/src/moonshine_voice/download.py:438` `def log_model_info(wanted_language, wanted_model_arch)`
- `EmbeddingModelArch.normalize_moonshine_language_tag` (method) `python/src/moonshine_voice/download.py:461` `def normalize_moonshine_language_tag(language)` -- Normalize a user language tag to the form expected by the Moonshine C API (e.g. en_us).
- `EmbeddingModelArch.dedupe_tts_language_tags_for_display` (method) `python/src/moonshine_voice/download.py:474` `def dedupe_tts_language_tags_for_display(tags)` -- Drop aliases that differ only by ``_`` vs ``-`` / spaces; return sorted hyphenated tags.
- `EmbeddingModelArch.tts_asset_cache_path` (method) `python/src/moonshine_voice/download.py:491` `def tts_asset_cache_path(cache_root)` -- Resolved directory for the TTS/G2P on-disk layout (same root `download_tts_assets` uses).
- `TtsVoicesByAvailability.list_tts_languages` (method) `python/src/moonshine_voice/download.py:588` `def list_tts_languages()` -- TTS language tags supported by the native catalog for the given path/voice options (same rules as...
- `TtsVoicesByAvailability.get_tts_voice_catalog` (method) `python/src/moonshine_voice/download.py:611` `def get_tts_voice_catalog()` -- Full map of language tag → voice entries (``id`` + ``state``: ``found`` or ``missing``).
- `TtsVoicesByAvailability.list_tts_voices` (method) `python/src/moonshine_voice/download.py:634` `def list_tts_voices(language)` -- Voice ids for one language, split by on-disk availability (raises `MoonshineTtsLanguageError` if ``language`` is...
- `TtsVoicesByAvailability.validate_tts_language` (method) `python/src/moonshine_voice/download.py:673` `def validate_tts_language(language)` -- Normalize and validate a TTS language tag against the native catalog.
- `TtsVoicesByAvailability.validate_tts_voice_downloaded` (method) `python/src/moonshine_voice/download.py:728` `def validate_tts_voice_downloaded(language, voice, asset_root)` -- Ensure ``voice`` is present (native ``state`` ``found``) for ``language`` under ``asset_root``.
- `TtsVoicesByAvailability.validate_tts_voice_known` (method) `python/src/moonshine_voice/download.py:760` `def validate_tts_voice_known(language, voice)` -- Ensure ``voice`` appears in the native TTS catalog for ``language``.
- `TtsVoicesByAvailability.ensure_tts_voice_downloaded` (method) `python/src/moonshine_voice/download.py:799` `def ensure_tts_voice_downloaded(language, voice, asset_root)` -- Ensure ``voice`` is on disk under ``asset_root``, like `validate_tts_voice_downloaded`.
- `TtsVoicesByAvailability.is_downloadable_tts_asset_key` (method) `python/src/moonshine_voice/download.py:842` `def is_downloadable_tts_asset_key(key)` -- Return False for G2P override labels (no path) returned when custom options are set.
- `TtsVoicesByAvailability.cdn_url_for_tts_asset_key` (method) `python/src/moonshine_voice/download.py:850` `def cdn_url_for_tts_asset_key(key)` -- HTTPS URL for a canonical asset key under ``TTS_CDN_BASE_URL``.
- `TtsVoicesByAvailability.list_tts_dependency_keys` (method) `python/src/moonshine_voice/download.py:857` `def list_tts_dependency_keys(languages)` -- Resolve required TTS asset paths via the native ``moonshine_get_tts_dependencies`` API.
- `TtsVoicesByAvailability.list_g2p_dependency_keys` (method) `python/src/moonshine_voice/download.py:882` `def list_g2p_dependency_keys(languages, options)` -- Resolve G2P-only asset paths via ``moonshine_get_g2p_dependencies`` (comma-separated from C).
- `TtsVoicesByAvailability.download_tts_assets` (method) `python/src/moonshine_voice/download.py:897` `def download_tts_assets(language)` -- Download every file required for TTS for the given language (and optional prefixed ``voice``) into the cache.
- `TtsVoicesByAvailability.download_g2p_assets` (method) `python/src/moonshine_voice/download.py:953` `def download_g2p_assets(language)` -- Download G2P lexicon/model files into the TTS asset cache layout (same CDN tree as TTS).

## python/src/moonshine_voice/download_file.py
Imported by: `python/src/moonshine_voice/download.py`
- `get_cache_dir` (function) `python/src/moonshine_voice/download_file.py:13` `def get_cache_dir(app_name)` -- Get the cache directory, respecting environment override.
- `hash_file` (function) `python/src/moonshine_voice/download_file.py:19` `def hash_file(path, algorithm)` -- Compute hash of a file.
- `download_file` (function) `python/src/moonshine_voice/download_file.py:28` `def download_file(url, dest, expected_sha256, resume, show_progress, timeout)` -- Download a file with progress bar, resume support, and integrity checking.
- `download_model` (function) `python/src/moonshine_voice/download_file.py:149` `def download_model(url, filename, expected_sha256, app_name)` -- Download a model file to the cache directory.

## python/src/moonshine_voice/errors.py
Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/tts.py`, `scripts/tts_g2p_intelligibility.py`
- `MoonshineError.__init__` (method) `python/src/moonshine_voice/errors.py:9` `def __init__(self, message, error_code)`
- `MoonshineUnknownError.__init__` (method) `python/src/moonshine_voice/errors.py:17` `def __init__(self, message)`
- `MoonshineInvalidHandleError.__init__` (method) `python/src/moonshine_voice/errors.py:24` `def __init__(self, message)`
- `MoonshineInvalidArgumentError.__init__` (method) `python/src/moonshine_voice/errors.py:31` `def __init__(self, message)`
- `MoonshineTtsLanguageError.__init__` (method) `python/src/moonshine_voice/errors.py:38` `def __init__(self, language, alternatives, message)`
- `MoonshineAudioOutputError.__init__` (method) `python/src/moonshine_voice/errors.py:57` `def __init__(self, message)`
- `MoonshineTtsVoiceError.__init__` (method) `python/src/moonshine_voice/errors.py:81` `def __init__(self, voice, language, alternatives)`
- `MoonshineTtsVoiceError.check_error` (method) `python/src/moonshine_voice/errors.py:107` `def check_error(error_code)` -- Check error code and raise appropriate exception if non-zero.

## python/src/moonshine_voice/g2p.py
Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
- `GraphemeToPhonemizer.__init__` (method) `python/src/moonshine_voice/g2p.py:30` `def __init__(self, language)`
- `GraphemeToPhonemizer.language` (method) `python/src/moonshine_voice/g2p.py:85` `def language(self)`
- `GraphemeToPhonemizer.asset_root` (method) `python/src/moonshine_voice/g2p.py:89` `def asset_root(self)`
- `GraphemeToPhonemizer.to_ipa` (method) `python/src/moonshine_voice/g2p.py:92` `def to_ipa(self, text, options)` -- Return IPA for ``text`` (single string from the native layer).
- `GraphemeToPhonemizer.close` (method) `python/src/moonshine_voice/g2p.py:100` `def close(self)`
- `GraphemeToPhonemizer.main` (method) `python/src/moonshine_voice/g2p.py:118` `def main()`

## python/src/moonshine_voice/intent_recognizer.py
Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`
Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/dialog_flow.py`
- `IntentMatch.trigger_phrase` (method) `python/src/moonshine_voice/intent_recognizer.py:37` `def trigger_phrase(self)` -- Alias for ``canonical_phrase`` (backward compatibility).
- `IntentRecognizer.__init__` (method) `python/src/moonshine_voice/intent_recognizer.py:61` `def __init__(self, model_path, model_arch, model_variant, threshold)` -- Initialize an intent recognizer.
- `IntentRecognizer.close` (method) `python/src/moonshine_voice/intent_recognizer.py:199` `def close(self)` -- Free the intent recognizer resources.
- `IntentRecognizer.register_intent` (method) `python/src/moonshine_voice/intent_recognizer.py:211` `def register_intent(self, trigger_phrase, handler)` -- Register an intent with a canonical phrase.
- `IntentRecognizer.unregister_intent` (method) `python/src/moonshine_voice/intent_recognizer.py:253` `def unregister_intent(self, trigger_phrase)` -- Remove a registered intent.
- `IntentRecognizer.get_closest_intents` (method) `python/src/moonshine_voice/intent_recognizer.py:274` `def get_closest_intents(self, utterance, tolerance_threshold)` -- Rank registered intents against ``utterance`` synchronously.
- `IntentRecognizer.process_utterance` (method) `python/src/moonshine_voice/intent_recognizer.py:331` `def process_utterance(self, utterance)` -- Process an utterance and invoke the handler of the most similar intent.
- `IntentRecognizer.threshold` (method) `python/src/moonshine_voice/intent_recognizer.py:358` `def threshold(self)` -- Minimum similarity used by ``process_utterance`` / default for ``get_closest_intents``.
- `IntentRecognizer.threshold` (method) `python/src/moonshine_voice/intent_recognizer.py:363` `def threshold(self, value)` -- Set the default similarity threshold (Python-side; passed per call to native code).
- `IntentRecognizer.intent_count` (method) `python/src/moonshine_voice/intent_recognizer.py:368` `def intent_count(self)` -- Get the number of registered intents.
- `IntentRecognizer.clear_intents` (method) `python/src/moonshine_voice/intent_recognizer.py:377` `def clear_intents(self)` -- Clear all registered intents.
- `IntentRecognizer.calculate_embedding` (method) `python/src/moonshine_voice/intent_recognizer.py:385` `def calculate_embedding(self, sentence)` -- Calculate the embedding vector for a sentence.
- `IntentRecognizer.distance` (method) `python/src/moonshine_voice/intent_recognizer.py:421` `def distance(self, embedding_a, embedding_b)` -- Compute the cosine similarity between two embedding vectors.
- `IntentRecognizer.set_on_intent` (method) `python/src/moonshine_voice/intent_recognizer.py:454` `def set_on_intent(self, callback)` -- Set a callback that is invoked for any recognized intent.
- `IntentRecognizer.on_line_completed` (method) `python/src/moonshine_voice/intent_recognizer.py:469` `def on_line_completed(self, event)` -- Called when a transcription line is completed.
- `IntentRecognizer.on_error` (method) `python/src/moonshine_voice/intent_recognizer.py:485` `def on_error(self, event)` -- Called when an error occurs.
- `IntentRecognizer.on_intent_triggered_on` (method) `python/src/moonshine_voice/intent_recognizer.py:555` `def on_intent_triggered_on(trigger, utterance, similarity)` -- Handler for when an intent is triggered.
- `TranscriptPrinter.__init__` (method) `python/src/moonshine_voice/intent_recognizer.py:564` `def __init__(self)`
- `TranscriptPrinter.update_last_terminal_line` (method) `python/src/moonshine_voice/intent_recognizer.py:567` `def update_last_terminal_line(self, new_text)`
- `TranscriptPrinter.on_line_started` (method) `python/src/moonshine_voice/intent_recognizer.py:574` `def on_line_started(self, event)`
- `TranscriptPrinter.on_line_text_changed` (method) `python/src/moonshine_voice/intent_recognizer.py:577` `def on_line_text_changed(self, event)`
- `TranscriptPrinter.on_line_completed` (method) `python/src/moonshine_voice/intent_recognizer.py:580` `def on_line_completed(self, event)`

## python/src/moonshine_voice/mic_transcriber.py
Depends on: `python/src/moonshine_voice/utils.py`
Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/dialog_flow.py`
- `MicTranscriber.__init__` (method) `python/src/moonshine_voice/mic_transcriber.py:22` `def __init__(self, model_path, model_arch, update_interval, device, samplerate, channels, blocksize, options...`
- `MicTranscriber.audio_callback` (method) `python/src/moonshine_voice/mic_transcriber.py:95` `def audio_callback(in_data, frames, time, status)`
- `MicTranscriber.start` (method) `python/src/moonshine_voice/mic_transcriber.py:202` `def start(self)`
- `MicTranscriber.stop` (method) `python/src/moonshine_voice/mic_transcriber.py:209` `def stop(self)`
- `MicTranscriber.close` (method) `python/src/moonshine_voice/mic_transcriber.py:216` `def close(self)`
- `MicTranscriber.transcribe_flags` (method) `python/src/moonshine_voice/mic_transcriber.py:223` `def transcribe_flags(self)` -- Flags currently applied to streamed ``update_transcription`` calls.
- `MicTranscriber.set_transcribe_flags` (method) `python/src/moonshine_voice/mic_transcriber.py:227` `def set_transcribe_flags(self, flags)` -- Update the per-update flags on the underlying mic stream.
- `MicTranscriber.add_listener` (method) `python/src/moonshine_voice/mic_transcriber.py:236` `def add_listener(self, listener)`
- `MicTranscriber.remove_listener` (method) `python/src/moonshine_voice/mic_transcriber.py:239` `def remove_listener(self, listener)`
- `MicTranscriber.remove_all_listeners` (method) `python/src/moonshine_voice/mic_transcriber.py:242` `def remove_all_listeners(self)`
- `MicTranscriber.push_listener` (method) `python/src/moonshine_voice/mic_transcriber.py:245` `def push_listener(self, listener)` -- Push a temporary listener, saving the current listeners on a stack.
- `MicTranscriber.pop_listener` (method) `python/src/moonshine_voice/mic_transcriber.py:249` `def pop_listener(self)` -- Restore the listeners that were active before the last push.
- `MicTranscriber.pop_all_listeners` (method) `python/src/moonshine_voice/mic_transcriber.py:253` `def pop_all_listeners(self)` -- Unwind the entire listener stack, restoring the original listeners.
- `TerminalListener.__init__` (method) `python/src/moonshine_voice/mic_transcriber.py:281` `def __init__(self)`
- `TerminalListener.update_last_terminal_line` (method) `python/src/moonshine_voice/mic_transcriber.py:286` `def update_last_terminal_line(self, line)`
- `TerminalListener.on_line_started` (method) `python/src/moonshine_voice/mic_transcriber.py:308` `def on_line_started(self, event)`
- `TerminalListener.on_line_text_changed` (method) `python/src/moonshine_voice/mic_transcriber.py:311` `def on_line_text_changed(self, event)`
- `TerminalListener.on_line_completed` (method) `python/src/moonshine_voice/mic_transcriber.py:314` `def on_line_completed(self, event)`
- `FileListener.on_line_completed` (method) `python/src/moonshine_voice/mic_transcriber.py:320` `def on_line_completed(self, event)`

## python/src/moonshine_voice/moonshine_api.py
Depends on: `python/src/moonshine_voice/errors.py`
Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/g2p.py`, `python/src/moonshine_voice/intent_recognizer.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`, `scripts/eval-alphanumeric.py`
- `moonshine_free` (function) `python/src/moonshine_voice/moonshine_api.py:65` `def moonshine_free(address)` -- Release memory allocated by the Moonshine C API (``malloc``).
- `ModelArch.model_arch_to_string` (method) `python/src/moonshine_voice/moonshine_api.py:199` `def model_arch_to_string(model_arch)` -- Convert a model architecture to a string.
- `ModelArch.string_to_model_arch` (method) `python/src/moonshine_voice/moonshine_api.py:217` `def string_to_model_arch(model_arch_string)` -- Convert a string to a model architecture.
- `Transcript.moonshine_options_array` (method) `python/src/moonshine_voice/moonshine_api.py:322` `def moonshine_options_array(options)` -- Build a ``moonshine_option_t`` array.
- `Transcript.moonshine_c_string_array` (method) `python/src/moonshine_voice/moonshine_api.py:339` `def moonshine_c_string_array(strings)` -- Build ``const char *filenames[]`` for TTS/G2P create-from-files helpers.
- `Transcript.moonshine_memory_arrays` (method) `python/src/moonshine_voice/moonshine_api.py:348` `def moonshine_memory_arrays(buffers)` -- Build parallel ``uint8_t*`` and ``uint64_t`` size arrays for in-memory TTS/G2P creation.
- `Transcript.moonshine_get_g2p_dependencies_string` (method) `python/src/moonshine_voice/moonshine_api.py:373` `def moonshine_get_g2p_dependencies_string(languages, options)` -- Call ``moonshine_get_g2p_dependencies`` and return the comma-separated key list (UTF-8).
- `Transcript.moonshine_get_tts_dependencies_string` (method) `python/src/moonshine_voice/moonshine_api.py:398` `def moonshine_get_tts_dependencies_string(languages, options)` -- Call ``moonshine_get_tts_dependencies`` and return the JSON array string (UTF-8).
- `Transcript.moonshine_try_get_tts_voices` (method) `python/src/moonshine_voice/moonshine_api.py:423` `def moonshine_try_get_tts_voices(languages, options)` -- Call ``moonshine_get_tts_voices`` without raising.
- `Transcript.moonshine_get_tts_voices_string` (method) `python/src/moonshine_voice/moonshine_api.py:452` `def moonshine_get_tts_voices_string(languages, options)` -- Call ``moonshine_get_tts_voices`` and return the JSON object string (UTF-8).
- `Transcript.moonshine_text_to_speech_samples` (method) `python/src/moonshine_voice/moonshine_api.py:468` `def moonshine_text_to_speech_samples(tts_synthesizer_handle, text, options)` -- Call ``moonshine_text_to_speech``; returns ``(samples, sample_rate_hz)``.
- `Transcript.moonshine_phonemes_to_speech_samples` (method) `python/src/moonshine_voice/moonshine_api.py:505` `def moonshine_phonemes_to_speech_samples(tts_synthesizer_handle, phonemes, options)` -- Call ``moonshine_phonemes_to_speech``; returns ``(samples, sample_rate_hz)``.
- `Transcript.moonshine_text_to_phonemes_string` (method) `python/src/moonshine_voice/moonshine_api.py:546` `def moonshine_text_to_phonemes_string(grapheme_to_phonemizer_handle, text, options)` -- Call ``moonshine_text_to_phonemes``; returns the IPA string (single segment).
- `_MoonshineLib.lib` (method) `python/src/moonshine_voice/moonshine_api.py:888` `def lib(self)` -- Get the loaded library.

## python/src/moonshine_voice/tts.py
Depends on: `python/src/moonshine_voice/download.py`, `python/src/moonshine_voice/errors.py`, `python/src/moonshine_voice/moonshine_api.py`, `python/src/moonshine_voice/utils.py`
- `_BeepRequest.list_output_devices` (method) `python/src/moonshine_voice/tts.py:163` `def list_output_devices()` -- Return human-readable output device descriptions for diagnostics.
- `TextToSpeech.__init__` (method) `python/src/moonshine_voice/tts.py:477` `def __init__(self, language)`
- `TextToSpeech.language` (method) `python/src/moonshine_voice/tts.py:828` `def language(self)`
- `TextToSpeech.asset_root` (method) `python/src/moonshine_voice/tts.py:832` `def asset_root(self)`
- `TextToSpeech.synthesize` (method) `python/src/moonshine_voice/tts.py:835` `def synthesize(self, text)` -- Synthesize ``text`` to PCM float samples ``(-1..1)`` and sample rate in Hz.
- `TextToSpeech.synthesize_from_phonemes` (method) `python/src/moonshine_voice/tts.py:856` `def synthesize_from_phonemes(self, phonemes)` -- Synthesize speech directly from IPA ``phonemes``, skipping grapheme-to-phoneme conversion.
- `TextToSpeech.say` (method) `python/src/moonshine_voice/tts.py:883` `def say(self, text)` -- Queue ``text`` for synthesis and playback, returning immediately.
- `TextToSpeech.play_error` (method) `python/src/moonshine_voice/tts.py:928` `def play_error(self)` -- Play the bundled "error" beep and return immediately.
- `TextToSpeech.play_success` (method) `python/src/moonshine_voice/tts.py:962` `def play_success(self)` -- Play the bundled "success" beep and return immediately.
- `TextToSpeech.is_talking` (method) `python/src/moonshine_voice/tts.py:1242` `def is_talking(self)` -- Return ``True`` if utterances are queued, being synthesized, or currently playing.
- `TextToSpeech.wait` (method) `python/src/moonshine_voice/tts.py:1255` `def wait(self)` -- Block until all queued utterances have been synthesized and played.
- `TextToSpeech.stop` (method) `python/src/moonshine_voice/tts.py:1260` `def stop(self)` -- Clear the utterance queue and stop any audio currently playing.
- `TextToSpeech.close` (method) `python/src/moonshine_voice/tts.py:1288` `def close(self)`

## python/src/moonshine_voice/utils.py
Imported by: `python/src/moonshine_voice/__init__.py`, `python/src/moonshine_voice/mic_transcriber.py`, `python/src/moonshine_voice/tts.py`, `python/tests/test_modules.py`
- `get_assets_path` (function) `python/src/moonshine_voice/utils.py:9` `def get_assets_path()` -- Get the path to the assets directory included in the package.
- `get_model_path` (function) `python/src/moonshine_voice/utils.py:27` `def get_model_path(model_name)` -- Get the path to a specific model directory in the assets folder.
- `load_wav_file` (function) `python/src/moonshine_voice/utils.py:47` `def load_wav_file(file_path)` -- Load a WAV file and return audio data as float array and sample rate.

## scripts/analyze_ko_phoneme_patterns.py
- `levenshtein_alignment` (function) `scripts/analyze_ko_phoneme_patterns.py:29` `def levenshtein_alignment(s, t)` -- Return (distance, list of (op, s_char, t_char)) edit operations.
- `extract_substitution_patterns` (function) `scripts/analyze_ko_phoneme_patterns.py:63` `def extract_substitution_patterns(ops, context_size)` -- Extract substitution/insertion/deletion patterns with surrounding context.
- `classify_phoneme` (function) `scripts/analyze_ko_phoneme_patterns.py:82` `def classify_phoneme(ch)` -- Classify a single IPA character into a broad category.
- `main` (function) `scripts/analyze_ko_phoneme_patterns.py:98` `def main()`

## scripts/analyze_ko_stress.py
Depends on: `python/src/moonshine_voice/download.py`
- `count_hangul_syllables` (function) `scripts/analyze_ko_stress.py:77` `def count_hangul_syllables(word)` -- Count Hangul syllable characters in a word.
- `extract_stress_positions` (function) `scripts/analyze_ko_stress.py:82` `def extract_stress_positions(ipa)` -- Extract the character positions of stress markers relative to the IPA string.
- `extract_stress_pattern` (function) `scripts/analyze_ko_stress.py:104` `def extract_stress_pattern(ipa, num_syllables)` -- Create a simplified stress pattern string. e.g., "1-0-2-0" means: primary on syl 1, none on syl 2, secondary on syl...
- `analyze_stress_position_type` (function) `scripts/analyze_ko_stress.py:140` `def analyze_stress_position_type(ipa)` -- Classify where primary stress ˈ appears relative to the word start.
- `setup_piper_phonemizer` (function) `scripts/analyze_ko_stress.py:158` `def setup_piper_phonemizer()` -- Set up Piper's eSpeak phonemizer with NFC patch.
- `phonemize_nfc` (function) `scripts/analyze_ko_stress.py:163` `def phonemize_nfc(self, voice, text)`
- `get_piper_ipa` (function) `scripts/analyze_ko_stress.py:188` `def get_piper_ipa(phonemizer, word)`
- `main` (function) `scripts/analyze_ko_stress.py:198` `def main()`

## scripts/check-banned-constructs.sh
- `scan` (function) `scripts/check-banned-constructs.sh:76` -- Print repo-relative paths of first-party files matching a regex, sorted.

## scripts/check-clang-tidy.sh
- `extract_keys` (function) `scripts/check-clang-tidy.sh:60` -- Extract a sorted, de-duplicated list of "<check>\t<relpath>" pairs from a clang-tidy log. run-clang-tidy prints one...

## scripts/compare_ko_phonemes.py
Depends on: `python/src/moonshine_voice/download.py`
- `get_piper_phonemes` (function) `scripts/compare_ko_phonemes.py:28` `def get_piper_phonemes(text, piper_voice)` -- Get phonemes from Piper's eSpeak phonemizer.
- `levenshtein_alignment` (function) `scripts/compare_ko_phonemes.py:42` `def levenshtein_alignment(s, t)` -- Return (distance, list of (op, s_char, t_char)) edit operations.
- `classify_char` (function) `scripts/compare_ko_phonemes.py:75` `def classify_char(ch)`
- `main` (function) `scripts/compare_ko_phonemes.py:87` `def main()`
- `phonemize_nfc` (function) `scripts/compare_ko_phonemes.py:136` `def phonemize_nfc(self, voice, text)`

## scripts/convert_tokenizer.py
- `write_bin_tokenizer` (function) `scripts/convert_tokenizer.py:29` `def write_bin_tokenizer(tokens, output_path)` -- Write tokens to BinTokenizer format.
- `convert_sentencepiece` (function) `scripts/convert_tokenizer.py:51` `def convert_sentencepiece(input_path, output_path)` -- Convert SentencePiece .model file to BinTokenizer format.
- `convert_huggingface_json` (function) `scripts/convert_tokenizer.py:84` `def convert_huggingface_json(input_path, output_path)` -- Convert HuggingFace tokenizer.json to BinTokenizer format.
- `main` (function) `scripts/convert_tokenizer.py:127` `def main()`

## scripts/eval-alphanumeric.py
Depends on: `python/src/moonshine_voice/alphanumeric_listener.py`, `python/src/moonshine_voice/moonshine_api.py`
- `folder_name_to_expected_char` (function) `scripts/eval-alphanumeric.py:46` `def folder_name_to_expected_char(name, matcher)` -- Resolve a folder name (e.g.
- `predict_character` (function) `scripts/eval-alphanumeric.py:54` `def predict_character(transcriber, audio, sample_rate, transcribe_flags)` -- Run transcription and return predictions for a single clip.
- `on_event` (function) `scripts/eval-alphanumeric.py:79` `def on_event(event)`
- `print_confusion_matrix` (function) `scripts/eval-alphanumeric.py:106` `def print_confusion_matrix(matrix, labels, title)` -- Pretty-print a confusion matrix with ``labels`` along both axes.
- `main` (function) `scripts/eval-alphanumeric.py:138` `def main()`

## scripts/eval-librispeech.py
- `parse_args` (function) `scripts/eval-librispeech.py:87` `def parse_args()`
- `detect_text_column` (function) `scripts/eval-librispeech.py:149` `def detect_text_column(sample)`
- `load_eval_dataset` (function) `scripts/eval-librispeech.py:158` `def load_eval_dataset(args)`
- `decode_audio` (function) `scripts/eval-librispeech.py:172` `def decode_audio(audio_field)` -- Return (float32 mono @16kHz, sample_rate) from a non-decoded audio field.
- `make_moonshine_c_backend` (function) `scripts/eval-librispeech.py:192` `def make_moonshine_c_backend(args, streaming)`
- `transcribe_batch` (function) `scripts/eval-librispeech.py:211` `def transcribe_batch(audio, sample_rate)`
- `transcribe_streaming` (function) `scripts/eval-librispeech.py:217` `def transcribe_streaming(audio, sample_rate)`
- `make_hf_backend` (function) `scripts/eval-librispeech.py:233` `def make_hf_backend(args)`
- `transcribe` (function) `scripts/eval-librispeech.py:268` `def transcribe(audio, sample_rate)`
- `main` (function) `scripts/eval-librispeech.py:282` `def main()`

## scripts/export-decoder-with-attention.py
- `main` (function) `scripts/export-decoder-with-attention.py:33` `def main()`

## scripts/export_zipvoice_model.py
- `run` (function) `scripts/export_zipvoice_model.py:53` `def run(cmd, cwd)`
- `convert_to_ort` (function) `scripts/export_zipvoice_model.py:58` `def convert_to_ort(python, onnx_path, custom_op_lib)`
- `main` (function) `scripts/export_zipvoice_model.py:72` `def main()`
- `deploy` (function) `scripts/export_zipvoice_model.py:134` `def deploy(src_onnx, canonical_stem)`

## scripts/export_zipvoice_voices_for_cpp.py
- `slug_from_voice_id` (function) `scripts/export_zipvoice_voices_for_cpp.py:55` `def slug_from_voice_id(voice_id)` -- ``voice_000_american_female`` -> ``american_female``.
- `select_voices` (function) `scripts/export_zipvoice_voices_for_cpp.py:60` `def select_voices(voices)` -- One masculine + one feminine speaker per accent (first of each in file order).
- `load_clip_pcm16` (function) `scripts/export_zipvoice_voices_for_cpp.py:127` `def load_clip_pcm16(path)`
- `_CloneTranscriber.__init__` (method) `scripts/export_zipvoice_voices_for_cpp.py:154` `def __init__(self)`
- `_CloneTranscriber.transcribe_pcm16` (method) `scripts/export_zipvoice_voices_for_cpp.py:165` `def transcribe_pcm16(self, pcm)`
- `_CloneTranscriber.close` (method) `scripts/export_zipvoice_voices_for_cpp.py:170` `def close(self)`
- `_CloneTranscriber.c_escape` (method) `scripts/export_zipvoice_voices_for_cpp.py:177` `def c_escape(s)`
- `_CloneTranscriber.main` (method) `scripts/export_zipvoice_voices_for_cpp.py:181` `def main()`

## scripts/generate-silero-vad-data.py
- `fetch_source_onnx` (function) `scripts/generate-silero-vad-data.py:88` `def fetch_source_onnx(dest_dir)` -- Download the pinned upstream Silero VAD .onnx and verify its SHA-256.
- `convert_onnx_to_ort` (function) `scripts/generate-silero-vad-data.py:105` `def convert_onnx_to_ort(onnx_path, out_dir, optimization)` -- Serialize an .onnx model to a .ort flatbuffer at the given opt level.
- `render_header` (function) `scripts/generate-silero-vad-data.py:130` `def render_header(data, source_name, optimization)`
- `main` (function) `scripts/generate-silero-vad-data.py:159` `def main()`

## scripts/patch-release.sh
- `main` (function) `scripts/patch-release.sh:32`

## scripts/prepare-release.sh
- `main` (function) `scripts/prepare-release.sh:67` -- All imperative work lives inside main() so bash parses the whole script before executing anything (mirrors...

## scripts/reliability-remote.sh
- `record_failure` (function) `scripts/reliability-remote.sh:69`
- `require_tool` (function) `scripts/reliability-remote.sh:89`
- `run_test` (function) `scripts/reliability-remote.sh:183`
- `run_fuzzer` (function) `scripts/reliability-remote.sh:439`

## scripts/run-benchmarks.py
- `WhisperListener.__init__` (method) `scripts/run-benchmarks.py:133` `def __init__(self)`
- `WhisperListener.on_line_completed` (method) `scripts/run-benchmarks.py:137` `def on_line_completed(self, event)`

## scripts/setup-android-ci.sh
- `log` (function) `scripts/setup-android-ci.sh:27`


Next: [API_p10.md](API_p10.md)
