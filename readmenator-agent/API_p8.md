# API (page 8 of 10)
Previous: [API_p7.md](API_p7.md)

## micro/feature-generation/src/log_mel.cc
Depends on: `micro/feature-generation/include/feature_generation/feature_generation.h`, `micro/feature-generation/src/fft_scratch.h`
- `ReflectIndex` (function) `micro/feature-generation/src/log_mel.cc:69` `inline int ReflectIndex(int i, int n)` -- Reflect index without duplicating the boundary.
- `ToFloatSample` (function) `micro/feature-generation/src/log_mel.cc:87` `inline float ToFloatSample(float s)` -- Per-sample input conversion for ComputeImpl.
- `ToFloatSample` (function) `micro/feature-generation/src/log_mel.cc:88` `inline float ToFloatSample(int16_t s)`
- `HzToMelSlaney` (function) `micro/feature-generation/src/log_mel.cc:93` `float HzToMelSlaney(float hz)`
- `MelToHzSlaney` (function) `micro/feature-generation/src/log_mel.cc:100` `float MelToHzSlaney(float mel)`
- `exp` (function) `micro/feature-generation/src/log_mel.cc:102` `return kMinLogHz * std::exp(kLogStep * (mel - kMinLogMel));`
- `HannWindowPeriodic` (function) `micro/feature-generation/src/log_mel.cc:107` `std::vector<float> HannWindowPeriodic(int length)`
- `w` (function) `micro/feature-generation/src/log_mel.cc:112` `std::vector<float> w(length);`
- `MakeMelFilterbank` (function) `micro/feature-generation/src/log_mel.cc:121` `std::vector<float> MakeMelFilterbank(int n_freq, int n_mels, int sample_rate,
                   ...`
- `mel_pts` (function) `micro/feature-generation/src/log_mel.cc:126` `std::vector<float> mel_pts(static_cast<std::size_t>(n_mels + 2));`
- `hz_pts` (function) `micro/feature-generation/src/log_mel.cc:132` `std::vector<float> hz_pts(mel_pts.size());`
- `bin_hz` (function) `micro/feature-generation/src/log_mel.cc:136` `std::vector<float> bin_hz(static_cast<std::size_t>(n_freq));`
- `fb` (function) `micro/feature-generation/src/log_mel.cc:142` `std::vector<float> fb( static_cast<std::size_t>(n_mels) * static_cast<std::size_t>(n_freq), 0.0f);`
- `LogMelSpectrogram` (function) `micro/feature-generation/src/log_mel.cc:163` `LogMelSpectrogram::LogMelSpectrogram(const LogMelParams& params)
    : params_(params), n_freq_(p...`
- `ComputeImpl` (function) `micro/feature-generation/src/log_mel.cc:313` `template <typename SampleT>
void LogMelSpectrogram::ComputeImpl(const SampleT* waveform,
        ...`
- `Compute` (function) `micro/feature-generation/src/log_mel.cc:439` `void LogMelSpectrogram::Compute(const float* waveform, std::size_t n_samples,
                   ...` -- Public entry points: fp32 (unchanged API) and int16 (the on-device STT clip buffer).
- `Compute` (function) `micro/feature-generation/src/log_mel.cc:444` `void LogMelSpectrogram::Compute(const int16_t* waveform, std::size_t n_samples,
                 ...`

## micro/feature-generation/src/mel_streamer.cc
Depends on: `micro/feature-generation/include/feature_generation/feature_generation.h`, `micro/feature-generation/src/fft_scratch.h`
- `MelStreamer` (function) `micro/feature-generation/src/mel_streamer.cc:10` `MelStreamer::MelStreamer(int n_mels, int window_frames, int n_fft,
                         const...`
- `Reset` (function) `micro/feature-generation/src/mel_streamer.cc:39` `void MelStreamer::Reset()`
- `PushHop` (function) `micro/feature-generation/src/mel_streamer.cc:53` `void MelStreamer::PushHop(const float* hop_samples)`
- `BuildModelInput` (function) `micro/feature-generation/src/mel_streamer.cc:93` `void MelStreamer::BuildModelInput(float* out) const`

## micro/g2p/include/g2p/g2p_dict.h
Imported by: `micro/g2p/include/g2p/g2p.h`, `micro/g2p/include/g2p/g2p_phones.h`, `micro/g2p/src/g2p.cc`, `micro/g2p/src/g2p_dict.cc`, `micro/g2p/src/g2p_phones.cc`, `micro/klatt-tts/include/tts/synth_stream.h`
- `DictLookup` (function) `micro/g2p/include/g2p/g2p_dict.h:26` `bool DictLookup(std::string_view word, std::string* ipa);` -- Look up `word` (case-insensitive; only a-z letters are significant) in the baked flash dictionary.
- `LoadFromFile` (function) `micro/g2p/include/g2p/g2p_dict.h:35` `bool LoadFromFile(const std::string& path);` -- Parse a "word<TAB>IPA" TSV: one entry per line, '#'-comments and blank lines ignored, later duplicates win.
- `Add` (function) `micro/g2p/include/g2p/g2p_dict.h:38` `void Add(std::string_view word, std::string_view ipa);` -- Add/replace a single entry (word is lowercased, a-z only).
- `Lookup` (function) `micro/g2p/include/g2p/g2p_dict.h:41` `bool Lookup(std::string_view word, std::string* ipa) const;` -- On a hit, writes IPA to *ipa and returns true.
- `size` (function) `micro/g2p/include/g2p/g2p_dict.h:43` `size_t size() const`
- `empty` (function) `micro/g2p/include/g2p/g2p_dict.h:44` `bool empty() const`
- `EnsureSorted` (function) `micro/g2p/include/g2p/g2p_dict.h:47` `private: void EnsureSorted() const;`

## micro/g2p/include/g2p/g2p_phones.h
Depends on: `micro/g2p/include/g2p/g2p_dict.h`
Imported by: `micro/g2p/src/g2p_phones.cc`, `micro/neural-tts/src/neural_tts.cc`
- `push` (function) `micro/g2p/include/g2p/g2p_phones.h:21` `bool push(const char* tok);`
- `TextToPhoneList` (function) `micro/g2p/include/g2p/g2p_phones.h:27` `bool TextToPhoneList(const char* text, PhoneTokenList* out, const Lexicon* overrides = nullptr);` -- Plain-text -> base-phone tokens without std::vector/std::string output.
- `TokenizeIpaToList` (function) `micro/g2p/include/g2p/g2p_phones.h:31` `bool TokenizeIpaToList(const char* ipa, PhoneTokenList* out);` -- IPA string -> base-phone tokens (heap-free output).

## micro/g2p/src/g2p.cc
Depends on: `micro/g2p/include/g2p/g2p.h`, `micro/g2p/include/g2p/g2p_dict.h`, `micro/g2p/src/g2p_numbers.h`, `micro/g2p/src/g2p_rules.h`
- `HasDigit` (function) `micro/g2p/src/g2p.cc:14` `bool HasDigit(const std::string& s)`
- `ResolveToken` (function) `micro/g2p/src/g2p.cc:22` `std::string ResolveToken(const std::string& tok, const Lexicon* overrides)` -- Resolve a single token to an IPA string via the lookup pipeline.
- `TextToPhones` (function) `micro/g2p/src/g2p.cc:33` `std::vector<std::string> TextToPhones(const std::string& text,
                                  ...`

## micro/g2p/src/g2p_dict.cc
Depends on: `micro/g2p/include/g2p/g2p_dict.h`, `micro/g2p/src/g2p_dict_data.h`
- `DecodeIpa` (function) `micro/g2p/src/g2p_dict.cc:16` `std::string DecodeIpa(uint32_t start, unsigned count)` -- Decode `count` packed phone ids starting at body offset `start` into IPA.
- `RestartKey` (function) `micro/g2p/src/g2p_dict.cc:27` `std::string RestartKey(int block)` -- The restart (first) key of a block: its entry always has sharedPrefixLen == 0.
- `NormalizeWordKey` (function) `micro/g2p/src/g2p_dict.cc:35` `std::string NormalizeWordKey(std::string_view word)`
- `DictLookup` (function) `micro/g2p/src/g2p_dict.cc:51` `bool DictLookup(std::string_view word, std::string* ipa)`
- `Add` (function) `micro/g2p/src/g2p_dict.cc:106` `void Lexicon::Add(std::string_view word, std::string_view ipa)`
- `EnsureSorted` (function) `micro/g2p/src/g2p_dict.cc:113` `void Lexicon::EnsureSorted() const`
- `stable_sort` (function) `micro/g2p/src/g2p_dict.cc:115` `std::stable_sort(
      entries_.begin(), entries_.end(),
      [](const auto& a, const auto& b)`
- `Lookup` (function) `micro/g2p/src/g2p_dict.cc:132` `bool Lexicon::Lookup(std::string_view word, std::string* ipa) const`
- `LoadFromFile` (function) `micro/g2p/src/g2p_dict.cc:145` `bool Lexicon::LoadFromFile(const std::string& path)`

## micro/g2p/src/g2p_numbers.cc
Depends on: `micro/g2p/src/g2p_numbers.h`
- `DigitSequenceIpa` (function) `micro/g2p/src/g2p_numbers.cc:40` `std::string DigitSequenceIpa(std::string_view digits)`
- `Under100Ipa` (function) `micro/g2p/src/g2p_numbers.cc:51` `std::string Under100Ipa(int n)`
- `Under1000Ipa` (function) `micro/g2p/src/g2p_numbers.cc:61` `std::string Under1000Ipa(int n)`
- `CardinalNonNegativeIpa` (function) `micro/g2p/src/g2p_numbers.cc:70` `bool CardinalNonNegativeIpa(long long n, std::string* out)`
- `IntegerDecimalStringIpa` (function) `micro/g2p/src/g2p_numbers.cc:108` `bool IntegerDecimalStringIpa(std::string s, std::string* out)`
- `NumberWordToIpa` (function) `micro/g2p/src/g2p_numbers.cc:184` `bool NumberWordToIpa(std::string_view token, std::string* ipa)`

## micro/g2p/src/g2p_numbers.h
Imported by: `micro/g2p/src/g2p.cc`, `micro/g2p/src/g2p_numbers.cc`, `micro/g2p/src/g2p_phones.cc`
- `NumberWordToIpa` (function) `micro/g2p/src/g2p_numbers.h:17` `bool NumberWordToIpa(std::string_view token, std::string* ipa);` -- If `token` is a supported plain numeral (e.g. "123", "-4", "3.5", "007"), writes its IPA to *ipa and returns true...

## micro/g2p/src/g2p_phones.cc
Depends on: `micro/g2p/include/g2p/g2p.h`, `micro/g2p/include/g2p/g2p_dict.h`, `micro/g2p/include/g2p/g2p_phones.h`, `micro/g2p/src/g2p_numbers.h`, `micro/g2p/src/g2p_rules.h`
- `HasDigit` (function) `micro/g2p/src/g2p_phones.cc:16` `bool HasDigit(const char* s)`
- `ResolveTokenBuf` (function) `micro/g2p/src/g2p_phones.cc:27` `bool ResolveTokenBuf(const char* tok, char* out, std::size_t cap,
                     const Lexi...` -- Resolve one word token to IPA in `out` (capacity includes NUL).
- `push` (function) `micro/g2p/src/g2p_phones.cc:45` `bool PhoneTokenList::push(const char* tok)`
- `TokenizeIpaToList` (function) `micro/g2p/src/g2p_phones.cc:53` `bool TokenizeIpaToList(const char* ipa, PhoneTokenList* out)`
- `TextToPhoneList` (function) `micro/g2p/src/g2p_phones.cc:61` `bool TextToPhoneList(const char* text, PhoneTokenList* out,
                     const Lexicon* o...`

## micro/g2p/src/g2p_rules.cc
Depends on: `micro/g2p/src/g2p_rules.h`
- `Utf8StartsWith` (function) `micro/g2p/src/g2p_rules.cc:19` `bool Utf8StartsWith(const std::string& s, std::string_view p)`
- `LastUtf8Char` (function) `micro/g2p/src/g2p_rules.cc:23` `std::string_view LastUtf8Char(std::string_view s)`
- `LastIpaUnitIsVowel` (function) `micro/g2p/src/g2p_rules.cc:34` `bool LastIpaUnitIsVowel(std::string_view prev)`
- `IsVowel` (function) `micro/g2p/src/g2p_rules.cc:47` `constexpr bool IsVowel(char c)`
- `IsConsonant` (function) `micro/g2p/src/g2p_rules.cc:51` `constexpr bool IsConsonant(char c)`
- `NextVowelIndex` (function) `micro/g2p/src/g2p_rules.cc:55` `int NextVowelIndex(std::string_view w, int start)`
- `MagicELengthens` (function) `micro/g2p/src/g2p_rules.cc:62` `bool MagicELengthens(std::string_view w, int vowel_i)`
- `ThVoicedWord` (function) `micro/g2p/src/g2p_rules.cc:201` `bool ThVoicedWord(std::string_view w)`
- `SingleConsonant` (function) `micro/g2p/src/g2p_rules.cc:207` `std::string SingleConsonant(char c, std::string_view w, int i)`
- `AddPrimaryStressIfMissing` (function) `micro/g2p/src/g2p_rules.cc:352` `std::string AddPrimaryStressIfMissing(std::string s)`
- `p` (function) `micro/g2p/src/g2p_rules.cc:359` `const std::string_view p(pref);`
- `GraphemeToIpa` (function) `micro/g2p/src/g2p_rules.cc:371` `std::string GraphemeToIpa(std::string_view word)`
- `RulesWordToIpa` (function) `micro/g2p/src/g2p_rules.cc:451` `std::string RulesWordToIpa(std::string_view word)`
- `LetterHomophoneToIpa` (function) `micro/g2p/src/g2p_rules.cc:467` `bool LetterHomophoneToIpa(std::string_view word, std::string* ipa)`

## micro/g2p/src/g2p_rules.h
Imported by: `micro/g2p/src/g2p.cc`, `micro/g2p/src/g2p_phones.cc`, `micro/g2p/src/g2p_rules.cc`
- `LetterHomophoneToIpa` (function) `micro/g2p/src/g2p_rules.h:26` `bool LetterHomophoneToIpa(std::string_view word, std::string* ipa);` -- Curated IPA for SpellingCNN letter readback homophones (spelling_labels.h).

## micro/g2p/src/ipa_tokens.cc
Depends on: `micro/g2p/include/g2p/g2p.h`
- `IsDirectAscii` (function) `micro/g2p/src/ipa_tokens.cc:81` `bool IsDirectAscii(char c)` -- Single ASCII phones that map straight to a table key (and aren't covered by the rule table above).
- `Utf8Len` (function) `micro/g2p/src/ipa_tokens.cc:108` `size_t Utf8Len(unsigned char lead)`
- `TokenizeIpa` (function) `micro/g2p/src/ipa_tokens.cc:118` `std::vector<std::string> TokenizeIpa(const std::string& ipa)`

## micro/klatt-tts/include/tts/config.h
Depends on: `micro/klatt-tts/include/tts/phonemes.h`
Imported by: `micro/klatt-tts/include/tts/synth_internal.h`, `micro/klatt-tts/include/tts/synth_stream.h`, `micro/klatt-tts/include/tts/tts.h`, `micro/klatt-tts/src/config.cc`, `micro/neural-tts/src/neural_tts.cc`
- `Lookup` (function) `micro/klatt-tts/include/tts/config.h:128` `const Phone* Lookup(const std::string& ipa) const;`
- `LoadVoiceConfig` (function) `micro/klatt-tts/include/tts/config.h:136` `bool LoadVoiceConfig(const std::string& path, VoiceParams& vp);` -- Apply overrides from a config file on top of `vp`.
- `DumpVoiceConfig` (function) `micro/klatt-tts/include/tts/config.h:140` `bool DumpVoiceConfig(const std::string& path, const VoiceParams& vp);` -- Write the full current parameter set to `path` in the file format above (round-trips through LoadVoiceConfig).

## micro/klatt-tts/include/tts/klatt.h
Imported by: `micro/klatt-tts/include/tts/synth_internal.h`, `micro/klatt-tts/include/tts/synth_stream.h`, `micro/klatt-tts/src/klatt.cc`
- `SetParams` (function) `micro/klatt-tts/include/tts/klatt.h:50` `void SetParams(float freq_hz, float bw_hz, float sample_rate);`
- `Step` (function) `micro/klatt-tts/include/tts/klatt.h:51` `inline float Step(float x)`
- `Reset` (function) `micro/klatt-tts/include/tts/klatt.h:57` `void Reset()`
- `SetBandpass` (function) `micro/klatt-tts/include/tts/klatt.h:107` `void SetBandpass(float freq_hz, float q, float sample_rate);` -- RBJ band-pass with constant 0 dB peak gain (level is independent of Q, so it stays constant as the centre frequency...
- `Step` (function) `micro/klatt-tts/include/tts/klatt.h:108` `inline float Step(float x)`
- `Reset` (function) `micro/klatt-tts/include/tts/klatt.h:116` `void Reset()`
- `Step` (function) `micro/klatt-tts/include/tts/klatt.h:125` `inline float Step(float x)`
- `Reset` (function) `micro/klatt-tts/include/tts/klatt.h:131` `void Reset()`
- `Render` (function) `micro/klatt-tts/include/tts/klatt.h:141` `std::vector<float> Render(const std::vector<SynthFrame>& frames, int samples_per_frame);` -- Render an entire parameter track.
- `RenderFrame` (function) `micro/klatt-tts/include/tts/klatt.h:150` `void RenderFrame(const SynthFrame& cur, const SynthFrame& nxt, int samples_per_frame, float* out);` -- Streaming primitive: render exactly `samples_per_frame` samples for a single control frame into `out` (caller-owned...
- `NextNoise` (function) `micro/klatt-tts/include/tts/klatt.h:154` `private: float NextNoise();`
- `EnsureLfShape` (function) `micro/klatt-tts/include/tts/klatt.h:157` `void EnsureLfShape(float rd);` -- Recompute the normalized LF shape if the Rd parameter changed.
- `LfDeriv` (function) `micro/klatt-tts/include/tts/klatt.h:160` `inline float LfDeriv(float phase) const;` -- Normalized LF flow-derivative at glottal phase in [0,1); negative peak == -1.

## micro/klatt-tts/include/tts/phonemes.h
Imported by: `micro/klatt-tts/include/tts/config.h`, `micro/klatt-tts/src/phonemes.cc`, `micro/klatt-tts/src/synth_internal.cc`, `micro/klatt-tts/src/synth_stream.cc`
- `LookupPhone` (function) `micro/klatt-tts/include/tts/phonemes.h:72` `const Phone* LookupPhone(const std::string& ipa);` -- Look up a phone by exact IPA key in the built-in default table.

## micro/klatt-tts/include/tts/synth_internal.h
Depends on: `micro/klatt-tts/include/tts/config.h`, `micro/klatt-tts/include/tts/klatt.h`
Imported by: `micro/klatt-tts/include/tts/synth_stream.h`, `micro/klatt-tts/src/synth_internal.cc`, `micro/neural-tts/src/neural_tts.cc`
- `SmoothBidir` (function) `micro/klatt-tts/include/tts/synth_internal.h:45` `void SmoothBidir(float* v, size_t n, float tau_ms);` -- Forward+backward (zero-phase) / forward-only / asymmetric one-pole smoothing over a per-frame track stored as a raw...
- `SmoothFwd` (function) `micro/klatt-tts/include/tts/synth_internal.h:46` `void SmoothFwd(float* v, size_t n, float tau_ms);`
- `SmoothAsym` (function) `micro/klatt-tts/include/tts/synth_internal.h:47` `void SmoothAsym(float* v, size_t n, float attack_ms, float release_ms);`
- `BuildSegments` (function) `micro/klatt-tts/include/tts/synth_internal.h:56` `int BuildSegments(const char* const* phones, int n_phones, const VoiceParams& vp, Segment* out, int max_out);` -- Heap-free variant: writes into caller-owned `out` (e.g. tensor-arena bump).
- `CountFrames` (function) `micro/klatt-tts/include/tts/synth_internal.h:60` `size_t CountFrames(const std::vector<Segment>& segs, float dur_scale);` -- Number of frames a segment list rasterizes to at a given duration scale.
- `FillParamTracks` (function) `micro/klatt-tts/include/tts/synth_internal.h:88` `void FillParamTracks(const std::vector<Segment>& segs, const VoiceParams& vp, float dur_scale, bool question...` -- Steps 2-4b: rasterize segments into `t` (which must already point at arrays of length t.n == CountFrames(segs...

## micro/klatt-tts/include/tts/synth_stream.h
Depends on: `micro/g2p/include/g2p/g2p_dict.h`, `micro/klatt-tts/include/tts/config.h`, `micro/klatt-tts/include/tts/klatt.h`, `micro/klatt-tts/include/tts/synth_internal.h`
Imported by: `micro/klatt-tts/include/tts/tts.h`, `micro/klatt-tts/src/synth_stream.cc`
- `BeginText` (function) `micro/klatt-tts/include/tts/synth_stream.h:61` `int BeginText(const char* text, const StreamOptions& opts, const g2p::Lexicon* overrides = nullptr);` -- Begin a new utterance from plain text (on-device G2P).
- `BeginIpa` (function) `micro/klatt-tts/include/tts/synth_stream.h:66` `int BeginIpa(const char* ipa, const StreamOptions& opts);` -- Begin a new utterance from an IPA string (bypasses the G2P; for isolating the synthesizer).
- `Read` (function) `micro/klatt-tts/include/tts/synth_stream.h:71` `int Read(float* out, int max_samples);` -- Pull up to `max_samples` mono float samples (roughly [-1, 1]) into `out`.
- `done` (function) `micro/klatt-tts/include/tts/synth_stream.h:73` `bool done() const`
- `sample_rate` (function) `micro/klatt-tts/include/tts/synth_stream.h:76` `int sample_rate() const`
- `total_samples` (function) `micro/klatt-tts/include/tts/synth_stream.h:77` `int total_samples() const`
- `BeginPhones` (function) `micro/klatt-tts/include/tts/synth_stream.h:82` `private: int BeginPhones(const std::vector<std::string>& phones, const StreamOptions& opts);`
- `ArenaReset` (function) `micro/klatt-tts/include/tts/synth_stream.h:84` `void ArenaReset()`
- `ArenaFloats` (function) `micro/klatt-tts/include/tts/synth_stream.h:85` `float* ArenaFloats(size_t count);`
- `ArenaBytes` (function) `micro/klatt-tts/include/tts/synth_stream.h:86` `uint8_t* ArenaBytes(size_t count, size_t align);`
- `RenderNextFrame` (function) `micro/klatt-tts/include/tts/synth_stream.h:87` `void RenderNextFrame();`

## micro/klatt-tts/src/config.cc
Depends on: `micro/klatt-tts/include/tts/config.h`
- `ClassName` (function) `micro/klatt-tts/src/config.cc:14` `const char* ClassName(PhoneClass c)`
- `SourceName` (function) `micro/klatt-tts/src/config.cc:34` `const char* SourceName(Source s)`
- `SetPhoneField` (function) `micro/klatt-tts/src/config.cc:105` `bool SetPhoneField(Phone& p, const std::string& field, float v)` -- Apply one "<field> <value>" override to a phone.
- `Lookup` (function) `micro/klatt-tts/src/config.cc:139` `const Phone* VoiceParams::Lookup(const std::string& ipa) const`
- `DefaultVoiceParams` (function) `micro/klatt-tts/src/config.cc:146` `VoiceParams DefaultVoiceParams()`
- `LoadVoiceConfig` (function) `micro/klatt-tts/src/config.cc:152` `bool LoadVoiceConfig(const std::string& path, VoiceParams& vp)`
- `DumpVoiceConfig` (function) `micro/klatt-tts/src/config.cc:216` `bool DumpVoiceConfig(const std::string& path, const VoiceParams& vp)`

## micro/klatt-tts/src/klatt.cc
Depends on: `micro/klatt-tts/include/tts/klatt.h`
- `GlottalPulse` (function) `micro/klatt-tts/src/klatt.cc:16` `inline float GlottalPulse(float phase, float open, float close)` -- Rosenberg-style glottal flow pulse as a function of phase in [0, 1).
- `TiltCoef` (function) `micro/klatt-tts/src/klatt.cc:29` `float TiltCoef(float tilt_db, float sample_rate)` -- One-pole low-pass coefficient `c` (y = (1-c)x + c*y1) such that the response is `tilt_db` down at 3 kHz.
- `SetParams` (function) `micro/klatt-tts/src/klatt.cc:48` `void Resonator::SetParams(float freq_hz, float bw_hz, float sample_rate)`
- `SetBandpass` (function) `micro/klatt-tts/src/klatt.cc:55` `void Biquad::SetBandpass(float freq_hz, float q, float sample_rate)`
- `SetParams` (function) `micro/klatt-tts/src/klatt.cc:70` `void Antiresonator::SetParams(float freq_hz, float bw_hz, float sample_rate)`
- `KlattSynth` (function) `micro/klatt-tts/src/klatt.cc:82` `KlattSynth::KlattSynth(float sample_rate, const KlattParams& params)
    : sample_rate_(sample_ra...`
- `EnsureLfShape` (function) `micro/klatt-tts/src/klatt.cc:94` `void KlattSynth::EnsureLfShape(float rd)` -- Map Fant's single Rd parameter to the LF glottal-flow-derivative shape, in time normalized to one pitch period (T0 = 1).
- `LfDeriv` (function) `micro/klatt-tts/src/klatt.cc:165` `inline float KlattSynth::LfDeriv(float phase) const` -- Normalized LF flow derivative; the negative excitation peak (at te) == -1.
- `NextNoise` (function) `micro/klatt-tts/src/klatt.cc:173` `float KlattSynth::NextNoise()`
- `RenderFrame` (function) `micro/klatt-tts/src/klatt.cc:181` `void KlattSynth::RenderFrame(const SynthFrame& cur, const SynthFrame& nxt,
                      ...`
- `Render` (function) `micro/klatt-tts/src/klatt.cc:296` `std::vector<float> KlattSynth::Render(const std::vector<SynthFrame>& frames,
                    ...`

## micro/klatt-tts/src/phonemes.cc
Depends on: `micro/klatt-tts/include/tts/phonemes.h`
- `LookupPhone` (function) `micro/klatt-tts/src/phonemes.cc:90` `const Phone* LookupPhone(const std::string& ipa)`
- `DefaultPhoneTable` (function) `micro/klatt-tts/src/phonemes.cc:96` `std::vector<Phone> DefaultPhoneTable()`

## micro/klatt-tts/src/synth_internal.cc
Depends on: `micro/klatt-tts/include/tts/phonemes.h`, `micro/klatt-tts/include/tts/synth_internal.h`
- `SegFromPhone` (function) `micro/klatt-tts/src/synth_internal.cc:15` `Segment SegFromPhone(const Phone& p)`
- `AppendStop` (function) `micro/klatt-tts/src/synth_internal.cc:38` `void AppendStop(const Phone& p, const VoiceParams& vp, int src_token,
                Segment* ou...` -- Expand a stop into closure -> burst -> (aspiration) sub-segments so that voice-onset-time distinguishes /p t k/ from...
- `BuildSegments` (function) `micro/klatt-tts/src/synth_internal.cc:75` `int BuildSegments(const char* const* phones, int n_phones, const VoiceParams& vp,
               ...`
- `BuildSegments` (function) `micro/klatt-tts/src/synth_internal.cc:176` `std::vector<Segment> BuildSegments(const std::vector<std::string>& phones,
                      ...`
- `SmoothBidir` (function) `micro/klatt-tts/src/synth_internal.cc:190` `void SmoothBidir(float* v, size_t n, float tau_ms)`
- `SmoothFwd` (function) `micro/klatt-tts/src/synth_internal.cc:201` `void SmoothFwd(float* v, size_t n, float tau_ms)`
- `SmoothAsym` (function) `micro/klatt-tts/src/synth_internal.cc:209` `void SmoothAsym(float* v, size_t n, float attack_ms, float release_ms)`
- `CountFrames` (function) `micro/klatt-tts/src/synth_internal.cc:222` `size_t CountFrames(const std::vector<Segment>& segs, float dur_scale)`
- `FillParamTracks` (function) `micro/klatt-tts/src/synth_internal.cc:232` `void FillParamTracks(const std::vector<Segment>& segs, const VoiceParams& vp,
                   ...`
- `FrameAt` (function) `micro/klatt-tts/src/synth_internal.cc:339` `SynthFrame FrameAt(const ParamTracks& t, size_t i)`
- `MakeKlattParams` (function) `micro/klatt-tts/src/synth_internal.cc:358` `KlattParams MakeKlattParams(const VoiceParams& vp)`

## micro/klatt-tts/src/synth_stream.cc
Depends on: `micro/g2p/include/g2p/g2p.h`, `micro/klatt-tts/include/tts/phonemes.h`, `micro/klatt-tts/include/tts/synth_stream.h`
- `SoftClip` (function) `micro/klatt-tts/src/synth_stream.cc:18` `inline float SoftClip(float x)` -- Soft limiter: perfectly linear up to a knee (so the RMS body of the signal is untouched), then a saturating soft...
- `StreamSynth` (function) `micro/klatt-tts/src/synth_stream.cc:30` `StreamSynth::StreamSynth(const VoiceParams& vp, uint8_t* arena,
                         size_t a...`
- `ArenaBytes` (function) `micro/klatt-tts/src/synth_stream.cc:34` `uint8_t* StreamSynth::ArenaBytes(size_t count, size_t align)`
- `ArenaFloats` (function) `micro/klatt-tts/src/synth_stream.cc:41` `float* StreamSynth::ArenaFloats(size_t count)`
- `BeginText` (function) `micro/klatt-tts/src/synth_stream.cc:46` `int StreamSynth::BeginText(const char* text, const StreamOptions& opts,
                         ...`
- `BeginIpa` (function) `micro/klatt-tts/src/synth_stream.cc:54` `int StreamSynth::BeginIpa(const char* ipa, const StreamOptions& opts)`
- `BeginPhones` (function) `micro/klatt-tts/src/synth_stream.cc:60` `int StreamSynth::BeginPhones(const std::vector<std::string>& phones,
                            ...`
- `RenderNextFrame` (function) `micro/klatt-tts/src/synth_stream.cc:125` `void StreamSynth::RenderNextFrame()`
- `Read` (function) `micro/klatt-tts/src/synth_stream.cc:140` `int StreamSynth::Read(float* out, int max_samples)`

## micro/neural-tts/host/tflm_ref/add.cpp
- `EvalAdd` (function) `micro/neural-tts/host/tflm_ref/add.cpp:35` `TfLiteStatus EvalAdd(TfLiteContext* context, TfLiteNode* node,
                     TfLiteAddPara...`
- `EvalAddQuantized` (function) `micro/neural-tts/host/tflm_ref/add.cpp:91` `TfLiteStatus EvalAddQuantized(TfLiteContext* context, TfLiteNode* node,
                         ...`
- `AddInit` (function) `micro/neural-tts/host/tflm_ref/add.cpp:163` `void* AddInit(TfLiteContext* context, const char* buffer, size_t length)`
- `AddEval` (function) `micro/neural-tts/host/tflm_ref/add.cpp:168` `TfLiteStatus AddEval(TfLiteContext* context, TfLiteNode* node)`
- `Register_ADD` (function) `micro/neural-tts/host/tflm_ref/add.cpp:196` `TFLMRegistration Register_ADD()`

## micro/neural-tts/host/tflm_ref/conv.cpp
- `ConvEval` (function) `micro/neural-tts/host/tflm_ref/conv.cpp:38` `TfLiteStatus ConvEval(TfLiteContext* context, TfLiteNode* node)`
- `Register_CONV_2D` (function) `micro/neural-tts/host/tflm_ref/conv.cpp:129` `TFLMRegistration Register_CONV_2D()`

## micro/neural-tts/host/tflm_ref/host_platform.cpp
- `InitializeTarget` (function) `micro/neural-tts/host/tflm_ref/host_platform.cpp:26` `void InitializeTarget()`
- `ticks_per_second` (function) `micro/neural-tts/host/tflm_ref/host_platform.cpp:28` `uint32_t ticks_per_second()`
- `GetCurrentTimeTicks` (function) `micro/neural-tts/host/tflm_ref/host_platform.cpp:30` `uint32_t GetCurrentTimeTicks()`

## micro/neural-tts/host/tflm_ref/transpose_conv.cpp
- `RuntimePaddingType` (function) `micro/neural-tts/host/tflm_ref/transpose_conv.cpp:60` `inline PaddingType RuntimePaddingType(TfLitePadding padding)`
- `CalculateOpData` (function) `micro/neural-tts/host/tflm_ref/transpose_conv.cpp:72` `TfLiteStatus CalculateOpData(TfLiteContext* context, TfLiteNode* node,
                          ...`
- `TransposeConvInit` (function) `micro/neural-tts/host/tflm_ref/transpose_conv.cpp:146` `void* TransposeConvInit(TfLiteContext* context, const char* buffer,
                        size_...`
- `TransposeConvPrepare` (function) `micro/neural-tts/host/tflm_ref/transpose_conv.cpp:152` `TfLiteStatus TransposeConvPrepare(TfLiteContext* context, TfLiteNode* node)`
- `TransposeConvEval` (function) `micro/neural-tts/host/tflm_ref/transpose_conv.cpp:261` `TfLiteStatus TransposeConvEval(TfLiteContext* context, TfLiteNode* node)`
- `Register_TRANSPOSE_CONV` (function) `micro/neural-tts/host/tflm_ref/transpose_conv.cpp:410` `TFLMRegistration Register_TRANSPOSE_CONV()`

## micro/neural-tts/host/tts_cli.cc
Depends on: `micro/neural-tts/include/neural_tts/neural_tts.h`
- `ReadFile` (function) `micro/neural-tts/host/tts_cli.cc:32` `std::vector<uint8_t> ReadFile(const char* path)`
- `WriteWavHeader` (function) `micro/neural-tts/host/tts_cli.cc:47` `void WriteWavHeader(FILE* f, int rate, int nsamples)`
- `Emit` (function) `micro/neural-tts/host/tts_cli.cc:71` `void Emit(void* user, const int16_t* samples, int n)`
- `main` (function) `micro/neural-tts/host/tts_cli.cc:78` `int main(int argc, char** argv)`
- `arena` (function) `micro/neural-tts/host/tts_cli.cc:118` `std::vector<uint8_t> arena(1u << 20);` -- Arena: the engine's transient working set (TFLM tensors + planning).

## micro/neural-tts/host/worldlite_synth_cli.cc
Depends on: `micro/neural-tts/include/neural_tts/worldlite_synth.h`
- `main` (function) `micro/neural-tts/host/worldlite_synth_cli.cc:15` `int main(int argc, char** argv)`

## micro/neural-tts/include/neural_tts/neural_tts.h
Depends on: `micro/neural-tts/include/neural_tts/pack_format.h`
Imported by: `micro/examples/rp2350/src/audio_service.cc`, `micro/examples/rp2350/src/main_i2s_audio_test.cc`, `micro/examples/rp2350/src/tts_service.cc`, `micro/neural-tts/host/tts_cli.cc`, `micro/neural-tts/src/neural_tts.cc`
- `ok` (function) `micro/neural-tts/include/neural_tts/neural_tts.h:49` `bool ok() const`
- `Synthesize` (function) `micro/neural-tts/include/neural_tts/neural_tts.h:57` `int Synthesize(const char* text, EmitFn emit, void* user);` -- Synthesize plain English text (on-device G2P).
- `SynthesizeIpa` (function) `micro/neural-tts/include/neural_tts/neural_tts.h:60` `int SynthesizeIpa(const char* ipa, EmitFn emit, void* user);` -- Same, from an IPA string (bypasses the G2P word front end).
- `EstimateSamples` (function) `micro/neural-tts/include/neural_tts/neural_tts.h:65` `int EstimateSamples(const char* text);` -- Exact sample count Synthesize(text) will produce, without decoding or rendering (runs the deterministic planning...
- `EstimateSamplesIpa` (function) `micro/neural-tts/include/neural_tts/neural_tts.h:66` `int EstimateSamplesIpa(const char* ipa);`
- `stats` (function) `micro/neural-tts/include/neural_tts/neural_tts.h:84` `const Stats& stats() const`
- `SynthesizeTokens` (function) `micro/neural-tts/include/neural_tts/neural_tts.h:87` `private: int SynthesizeTokens(void* tokens_vec, EmitFn emit, void* user, bool plan_only);`

## micro/neural-tts/include/neural_tts/pack_format.h
Imported by: `micro/neural-tts/include/neural_tts/neural_tts.h`
- `Pack` (function) `micro/neural-tts/include/neural_tts/pack_format.h:143` `public:
  explicit Pack(const uint8_t* base)
      : base_(base),
        h_(reinterpret_cast<con...`
- `ok` (function) `micro/neural-tts/include/neural_tts/pack_format.h:147` `bool ok() const`
- `h` (function) `micro/neural-tts/include/neural_tts/pack_format.h:151` `const PackHeader& h() const`
- `raw` (function) `micro/neural-tts/include/neural_tts/pack_format.h:152` `const uint8_t* raw(uint32_t off) const`
- `model` (function) `micro/neural-tts/include/neural_tts/pack_format.h:154` `const unsigned char* model() const`
- `codebook` (function) `micro/neural-tts/include/neural_tts/pack_format.h:155` `const int8_t* codebook(int s) const`
- `codebook_scale` (function) `micro/neural-tts/include/neural_tts/pack_format.h:158` `const float* codebook_scale(int s) const`
- `dtypes` (function) `micro/neural-tts/include/neural_tts/pack_format.h:161` `const DiphoneTypeRec* dtypes() const`
- `dunits` (function) `micro/neural-tts/include/neural_tts/pack_format.h:164` `const DiphoneUnitRec* dunits() const`
- `wunits` (function) `micro/neural-tts/include/neural_tts/pack_format.h:167` `const WordUnitRec* wunits() const`
- `wkeys` (function) `micro/neural-tts/include/neural_tts/pack_format.h:170` `const uint8_t* wkeys() const`
- `centroid` (function) `micro/neural-tts/include/neural_tts/pack_format.h:171` `const int8_t* centroid(int type_idx) const`
- `codes` (function) `micro/neural-tts/include/neural_tts/pack_format.h:175` `const uint8_t* codes(uint32_t off) const`
- `f0_stream` (function) `micro/neural-tts/include/neural_tts/pack_format.h:178` `const uint8_t* f0_stream(uint32_t off) const`
- `phone_token` (function) `micro/neural-tts/include/neural_tts/pack_format.h:181` `const char* phone_token(int id) const`
- `dur_ratio` (function) `micro/neural-tts/include/neural_tts/pack_format.h:184` `const float* dur_ratio() const`
- `phone_class` (function) `micro/neural-tts/include/neural_tts/pack_format.h:187` `const uint8_t* phone_class() const`
- `func_idx` (function) `micro/neural-tts/include/neural_tts/pack_format.h:188` `const uint16_t* func_idx() const`
- `func_blob` (function) `micro/neural-tts/include/neural_tts/pack_format.h:191` `const uint8_t* func_blob() const`

## micro/neural-tts/include/neural_tts/pb_decoder.h
Depends on: `micro/neural-tts/include/neural_tts/worldlite_synth.h`
Imported by: `micro/examples/rp2350/src/main_step6_decoder.cc`, `micro/examples/rp2350/src/main_step7_synthesize.cc`, `micro/examples/rp2350/src/main_step7b_framesweep.cc`, `micro/examples/rp2350/src/main_tts_ladder_test.cc`, `micro/neural-tts/src/neural_tts.cc`, `micro/neural-tts/src/pb_decoder.cc`
- `ok` (function) `micro/neural-tts/include/neural_tts/pb_decoder.h:55` `bool ok() const`
- `arena_used_bytes` (function) `micro/neural-tts/include/neural_tts/pb_decoder.h:56` `size_t arena_used_bytes() const;`
- `BeginUtterance` (function) `micro/neural-tts/include/neural_tts/pb_decoder.h:58` `void BeginUtterance(const PbCodedUtterance* utt);`
- `GetFrameThunk` (function) `micro/neural-tts/include/neural_tts/pb_decoder.h:61` `static void GetFrameThunk(void* user, int t, WorldFrame* frame);` -- WorldLiteSynth::GetFrameFn-compatible; `user` is the PbDecoder*.
- `GetFrame` (function) `micro/neural-tts/include/neural_tts/pb_decoder.h:62` `void GetFrame(int t, WorldFrame* frame);`
- `ReadRows` (function) `micro/neural-tts/include/neural_tts/pb_decoder.h:72` `void ReadRows(int t0, int n, int16_t* out);` -- Batch-read rows [t0, t0+n) of the current utterance's RAW int16 graph output ([60] = benv dB/20 then bap, quantized...
- `decode_us` (function) `micro/neural-tts/include/neural_tts/pb_decoder.h:75` `uint64_t decode_us() const` -- cumulative microseconds spent inside TFLM Invoke() + latent prep
- `tiles_decoded` (function) `micro/neural-tts/include/neural_tts/pb_decoder.h:76` `int tiles_decoded() const`
- `DecodeTileAt` (function) `micro/neural-tts/include/neural_tts/pb_decoder.h:81` `bool DecodeTileAt(int latent_start);` -- false = Invoke failed (window state unchanged); callers must not retry in a loop.

## micro/neural-tts/include/neural_tts/worldlite_synth.h
Imported by: `micro/examples/rp2350/src/main_step5_synth.cc`, `micro/examples/rp2350/src/main_step6_decoder.cc`, `micro/examples/rp2350/src/main_step7_synthesize.cc`, `micro/examples/rp2350/src/main_step7c_synthonly.cc`, `micro/examples/rp2350/src/main_tts_ladder_test.cc`, `micro/neural-tts/host/worldlite_synth_cli.cc`, `micro/neural-tts/include/neural_tts/pb_decoder.h`, `micro/neural-tts/src/neural_tts.cc`, `micro/neural-tts/src/worldlite_synth.cc`
- `KissFftrPlanBytes` (function) `micro/neural-tts/include/neural_tts/worldlite_synth.h:39` `inline size_t KissFftrPlanBytes(int nfft, int inverse_fft)` -- Bytes kiss_fftr_alloc needs for one real-FFT plan (query with mem=nullptr).
- `KissFftrPairBytes` (function) `micro/neural-tts/include/neural_tts/worldlite_synth.h:46` `inline size_t KissFftrPairBytes(int nfft)` -- Forward + inverse plan storage for Synthesize() (typically ~21 KiB at nfft=1024).
- `Synthesize` (function) `micro/neural-tts/include/neural_tts/worldlite_synth.h:77` `void Synthesize(GetFrameFn get_frame, void* frame_user, int num_frames, float gain, EmitFn emit, void* emit_user);` -- Renders num_frames control frames (num_frames * 80 output samples).
- `ok` (function) `micro/neural-tts/include/neural_tts/worldlite_synth.h:82` `bool ok() const` -- False if kissfft plan setup failed; using the synth in that state chases garbage plan state forever.
- `fwd_plan` (function) `micro/neural-tts/include/neural_tts/worldlite_synth.h:87` `const void* fwd_plan() const` -- Bring-up: plan pointers + a self-test that runs one forward+inverse FFT pair through the plans (the on-device...
- `inv_plan` (function) `micro/neural-tts/include/neural_tts/worldlite_synth.h:88` `const void* inv_plan() const`
- `FftSelfTest` (function) `micro/neural-tts/include/neural_tts/worldlite_synth.h:89` `float FftSelfTest();`
- `InitTables` (function) `micro/neural-tts/include/neural_tts/worldlite_synth.h:97` `void InitTables();`
- `ExpandFrame` (function) `micro/neural-tts/include/neural_tts/worldlite_synth.h:98` `void ExpandFrame(const WorldFrame& f, float* spec_pow, float* ap) const;`
- `MinimumPhase` (function) `micro/neural-tts/include/neural_tts/worldlite_synth.h:99` `void MinimumPhase(const float* log_amp_half, kiss_fft_cpx* min_phase);`
- `RenderPulse` (function) `micro/neural-tts/include/neural_tts/worldlite_synth.h:100` `void RenderPulse(const float* spec_pow, const float* ap, bool voiced, int noise_size, float frac_shift_s, float*...`
- `FlushTo` (function) `micro/neural-tts/include/neural_tts/worldlite_synth.h:102` `void FlushTo(int abs_pos, float gain, EmitFn emit, void* emit_user);`
- `Randn` (function) `micro/neural-tts/include/neural_tts/worldlite_synth.h:103` `float Randn();`

## micro/neural-tts/src/neural_tts.cc
Depends on: `micro/g2p/include/g2p/g2p.h`, `micro/g2p/include/g2p/g2p_phones.h`, `micro/klatt-tts/include/tts/config.h`, `micro/klatt-tts/include/tts/synth_internal.h`, `micro/neural-tts/include/neural_tts/neural_tts.h`, `micro/neural-tts/include/neural_tts/pb_decoder.h`, `micro/neural-tts/include/neural_tts/worldlite_synth.h`
- `NowUs` (function) `micro/neural-tts/src/neural_tts.cc:55` `inline uint64_t NowUs()`
- `Exp10` (function) `micro/neural-tts/src/neural_tts.cc:91` `inline float Exp10(float x)`
- `BitReader` (function) `micro/neural-tts/src/neural_tts.cc:122` `public:
  explicit BitReader(const uint8_t* p) : p_(p)`
- `get` (function) `micro/neural-tts/src/neural_tts.cc:123` `uint32_t get(int bits)`
- `ReadVarU8` (function) `micro/neural-tts/src/neural_tts.cc:140` `int ReadVarU8(const uint8_t*& p)`
- `DecodeF0Stream` (function) `micro/neural-tts/src/neural_tts.cc:163` `void DecodeF0Stream(const uint8_t* p, int n_frames, float* out,
                    F0RunSpan* runs)` -- Decode a unit's f0 side stream into per-frame Hz (0 = unvoiced).
- `exp2f` (function) `micro/neural-tts/src/neural_tts.cc:205` `kPackF0BaseHz * exp2f(code / kPackF0StepsPerOctave);`
- `F0FromCode` (function) `micro/neural-tts/src/neural_tts.cc:213` `inline float F0FromCode(uint8_t q)`
- `Bump` (function) `micro/neural-tts/src/neural_tts.cc:236` `public:
  Bump(uint8_t* base, size_t size) : base_(base), size_(size)`
- `Alloc` (function) `micro/neural-tts/src/neural_tts.cc:237` `void* Alloc(size_t bytes, size_t align = 4)`
- `AllocArray` (function) `micro/neural-tts/src/neural_tts.cc:244` `template <typename T>
  T* AllocArray(size_t n, size_t align = 4)`
- `Mark` (function) `micro/neural-tts/src/neural_tts.cc:247` `size_t Mark() const`
- `Reset` (function) `micro/neural-tts/src/neural_tts.cc:248` `void Reset(size_t mark)`
- `remaining` (function) `micro/neural-tts/src/neural_tts.cc:249` `size_t remaining() const`
- `Engine` (function) `micro/neural-tts/src/neural_tts.cc:262` `public:
  Engine(const Pack& pk, uint8_t* arena, size_t arena_size,
         NeuralTts::Stats* st...`
- `IsSil` (function) `micro/neural-tts/src/neural_tts.cc:292` `bool IsSil(int pid) const`
- `IsGap` (function) `micro/neural-tts/src/neural_tts.cc:296` `bool IsGap(int pid) const`
- `Canon` (function) `micro/neural-tts/src/neural_tts.cc:299` `int Canon(int pid) const`
- `TimedEmit` (function) `micro/neural-tts/src/neural_tts.cc:342` `static void TimedEmit(void* user, const int16_t* samples, int n)`
- `BlendLenUnit` (function) `micro/neural-tts/src/neural_tts.cc:352` `static int BlendLenUnit(int rule_n, int nat_n)`
- `PhoneId` (function) `micro/neural-tts/src/neural_tts.cc:438` `int Engine::PhoneId(const char* token) const`
- `BuildRunsFromPtrs` (function) `micro/neural-tts/src/neural_tts.cc:447` `int Engine::BuildRunsFromPtrs(const char* const* tokens, int n_tokens)`
- `BuildRuns` (function) `micro/neural-tts/src/neural_tts.cc:492` `int Engine::BuildRuns(const std::vector<std::string>& tokens)`
- `FindDiphoneType` (function) `micro/neural-tts/src/neural_tts.cc:499` `int Engine::FindDiphoneType(int a, int b) const`
- `KeyCompare` (function) `micro/neural-tts/src/neural_tts.cc:516` `static int KeyCompare(const uint8_t* a, int la, const uint8_t* b, int lb)` -- Lexicographic compare of two phone-id keys.
- `FindWord` (function) `micro/neural-tts/src/neural_tts.cc:524` `int Engine::FindWord(const uint8_t* key, int len) const`
- `RunAfterBuild` (function) `micro/neural-tts/src/neural_tts.cc:547` `int Engine::RunAfterBuild(NeuralTts::EmitFn emit, void* user, bool plan_only)`
- `Run` (function) `micro/neural-tts/src/neural_tts.cc:597` `int Engine::Run(std::vector<std::string>* tokens, NeuralTts::EmitFn emit,
                void* u...`
- `Run` (function) `micro/neural-tts/src/neural_tts.cc:609` `int Engine::Run(const g2p::PhoneTokenList* phones, NeuralTts::EmitFn emit,
                void* ...` -- if defined(PICO_BUILD)
- `ComputeProsodyBuckets` (function) `micro/neural-tts/src/neural_tts.cc:622` `void Engine::ComputeProsodyBuckets(int n)`
- `ProsOff` (function) `micro/neural-tts/src/neural_tts.cc:698` `float Engine::ProsOff(const float* table, int chunk_start) const`
- `SegOff` (function) `micro/neural-tts/src/neural_tts.cc:703` `float Engine::SegOff(const float* table, int seg) const`
- `MatchWords` (function) `micro/neural-tts/src/neural_tts.cc:707` `void Engine::MatchWords(int n)`
- `SelectDiphones` (function) `micro/neural-tts/src/neural_tts.cc:807` `void Engine::SelectDiphones(int n)`
- `BuildParts` (function) `micro/neural-tts/src/neural_tts.cc:928` `void Engine::BuildParts(int n)`
- `UnpackCodes` (function) `micro/neural-tts/src/neural_tts.cc:1081` `void Engine::UnpackCodes(uint32_t codes_off, int n_latents, uint16_t* out)`
- `DecodedRows` (function) `micro/neural-tts/src/neural_tts.cc:1097` `const int16_t* Engine::DecodedRows(bool word, int idx, int frame_base,
                          ...`
- `WarpPositions` (function) `micro/neural-tts/src/neural_tts.cc:1129` `static void WarpPositions(int m, int n, float* pos)` -- warp positions (synth_diphone_world.py warp / warp_anchored)
- `WarpAnchoredPositions` (function) `micro/neural-tts/src/neural_tts.cc:1139` `static void WarpAnchoredPositions(int m, int n, bool anchor_end,
                                ...`
- `BuildRanges` (function) `micro/neural-tts/src/neural_tts.cc:1167` `int Engine::BuildRanges(const Part& p, int T, Range ranges[2]) const`
- `MaterializeF0` (function) `micro/neural-tts/src/neural_tts.cc:1187` `void Engine::MaterializeF0()` -- f0 prepass: the pitch track comes entirely from the flash-side f0 streams (never from the TFLM decoder), so the...
- `MaterializePartTrack` (function) `micro/neural-tts/src/neural_tts.cc:1243` `void Engine::MaterializePartTrack(int pi)` -- Write the track rows (benv/bap, NOT f0_: that's already final) of one part.
- `GainEqAt` (function) `micro/neural-tts/src/neural_tts.cc:1344` `void Engine::GainEqAt(int pi)`
- `SmoothJoinAt` (function) `micro/neural-tts/src/neural_tts.cc:1392` `void Engine::SmoothJoinAt(int j)`
- `FrameLnEnergy` (function) `micro/neural-tts/src/neural_tts.cc:1423` `float Engine::FrameLnEnergy(int t) const`
- `LoudKnotAt` (function) `micro/neural-tts/src/neural_tts.cc:1433` `static float LoudKnotAt(const int8_t* k, float scale, float u)` -- Interpolate a unit's baked loudness knots at unit fraction u in [0, 1], returning LSA (natural-log summed-band...
- `PlanLoudness` (function) `micro/neural-tts/src/neural_tts.cc:1444` `void Engine::PlanLoudness()`
- `AdvanceJoins` (function) `micro/neural-tts/src/neural_tts.cc:1547` `void Engine::AdvanceJoins()`
- `EnsureFinal` (function) `micro/neural-tts/src/neural_tts.cc:1580` `void Engine::EnsureFinal(int t)`
- `F0Pass` (function) `micro/neural-tts/src/neural_tts.cc:1600` `void Engine::F0Pass()`
- `RenderGetFrame` (function) `micro/neural-tts/src/neural_tts.cc:1695` `static void RenderGetFrame(void* user, int t, WorldFrame* frame)`
- `SynthesizeChunk` (function) `micro/neural-tts/src/neural_tts.cc:1720` `int Engine::SynthesizeChunk(int lo, int hi, bool first, bool last,
                            Ne...`
- `NeuralTts` (function) `micro/neural-tts/src/neural_tts.cc:1970` `NeuralTts::NeuralTts(const uint8_t* pack, uint8_t* arena, size_t arena_size)
    : pack_(pack), a...`
- `SynthesizeTokens` (function) `micro/neural-tts/src/neural_tts.cc:1975` `int NeuralTts::SynthesizeTokens(void* tokens_vec, EmitFn emit, void* user,
                      ...`
- `Synthesize` (function) `micro/neural-tts/src/neural_tts.cc:1984` `int NeuralTts::Synthesize(const char* text, EmitFn emit, void* user)`
- `SynthesizeIpa` (function) `micro/neural-tts/src/neural_tts.cc:2001` `int NeuralTts::SynthesizeIpa(const char* ipa, EmitFn emit, void* user)`
- `EstimateSamples` (function) `micro/neural-tts/src/neural_tts.cc:2018` `int NeuralTts::EstimateSamples(const char* text)`
- `EstimateSamplesIpa` (function) `micro/neural-tts/src/neural_tts.cc:2035` `int NeuralTts::EstimateSamplesIpa(const char* ipa)`

## micro/neural-tts/src/pb_decoder.cc
Depends on: `micro/neural-tts/include/neural_tts/pb_decoder.h`
- `NowUs` (function) `micro/neural-tts/src/pb_decoder.cc:37` `uint64_t NowUs()`
- `Exp10` (function) `micro/neural-tts/src/pb_decoder.cc:47` `inline float Exp10(float x)` -- exp10f(x) = 10^x for the benv dB/20 -> amplitude conversion
- `BeginEvent` (function) `micro/neural-tts/src/pb_decoder.cc:57` `public:
  uint32_t BeginEvent(const char*) override`
- `EndEvent` (function) `micro/neural-tts/src/pb_decoder.cc:62` `void EndEvent(uint32_t) override`
- `Reset` (function) `micro/neural-tts/src/pb_decoder.cc:63` `void Reset()`
- `PbDecoder` (function) `micro/neural-tts/src/pb_decoder.cc:73` `PbDecoder::PbDecoder(const Config& config, uint8_t* arena,
                     size_t arena_byte...`
- `arena_used_bytes` (function) `micro/neural-tts/src/pb_decoder.cc:131` `size_t PbDecoder::arena_used_bytes() const`
- `BeginUtterance` (function) `micro/neural-tts/src/pb_decoder.cc:135` `void PbDecoder::BeginUtterance(const PbCodedUtterance* utt)`
- `DecodeTileAt` (function) `micro/neural-tts/src/pb_decoder.cc:144` `bool PbDecoder::DecodeTileAt(int latent_start)`
- `GetFrame` (function) `micro/neural-tts/src/pb_decoder.cc:201` `void PbDecoder::GetFrame(int t, WorldFrame* frame)`
- `GetFrameThunk` (function) `micro/neural-tts/src/pb_decoder.cc:235` `void PbDecoder::GetFrameThunk(void* user, int t, WorldFrame* frame)`
- `ReadRows` (function) `micro/neural-tts/src/pb_decoder.cc:239` `void PbDecoder::ReadRows(int t0, int n, int16_t* out)`

## micro/neural-tts/src/worldlite_synth.cc
Depends on: `micro/neural-tts/include/neural_tts/worldlite_synth.h`
- `HzToMel` (function) `micro/neural-tts/src/worldlite_synth.cc:48` `float HzToMel(float hz)`
- `InitTables` (function) `micro/neural-tts/src/worldlite_synth.cc:52` `void WorldLiteSynth::InitTables()`
- `WorldLiteSynth` (function) `micro/neural-tts/src/worldlite_synth.cc:89` `WorldLiteSynth::WorldLiteSynth() : rng_state_(0x8f1bbcdcu), owns_fft_plans_(true)`
- `WorldLiteSynth` (function) `micro/neural-tts/src/worldlite_synth.cc:95` `WorldLiteSynth::WorldLiteSynth(void* plan_mem, size_t plan_mem_bytes)
    : rng_state_(0x8f1bbcdc...`
- `FftSelfTest` (function) `micro/neural-tts/src/worldlite_synth.cc:127` `float WorldLiteSynth::FftSelfTest()`
- `Randn` (function) `micro/neural-tts/src/worldlite_synth.cc:143` `float WorldLiteSynth::Randn()`
- `ExpandFrame` (function) `micro/neural-tts/src/worldlite_synth.cc:155` `void WorldLiteSynth::ExpandFrame(const WorldFrame& f, float* spec_pow,
                          ...`
- `MinimumPhase` (function) `micro/neural-tts/src/worldlite_synth.cc:171` `void WorldLiteSynth::MinimumPhase(const float* log_amp_half,
                                  ki...`
- `RenderPulse` (function) `micro/neural-tts/src/worldlite_synth.cc:200` `void WorldLiteSynth::RenderPulse(const float* spec_pow, const float* ap,
                        ...`
- `FlushTo` (function) `micro/neural-tts/src/worldlite_synth.cc:296` `void WorldLiteSynth::FlushTo(int abs_pos, float gain, EmitFn emit,
                             v...`
- `Synthesize` (function) `micro/neural-tts/src/worldlite_synth.cc:315` `void WorldLiteSynth::Synthesize(GetFrameFn get_frame, void* frame_user,
                         ...`

## micro/stt-training/stt_training/augment.py
Imported by: `micro/stt-training/stt_training/train.py`
- `WaveformAugment.__init__` (method) `micro/stt-training/stt_training/augment.py:36` `def __init__(self, sample_rate, musan_noise_dir, rir_dir, gain_db, noise_snr_min, noise_snr_max, bandpass_p...`
- `WaveformAugment.n_transforms` (method) `micro/stt-training/stt_training/augment.py:139` `def n_transforms(self)`
- `WaveformAugment.has_external_data` (method) `micro/stt-training/stt_training/augment.py:143` `def has_external_data(self)`
- `WaveformAugment.forward` (method) `micro/stt-training/stt_training/augment.py:238` `def forward(self, waveform)`

## micro/stt-training/stt_training/checkpoint.py
Depends on: `micro/stt-training/stt_training/model.py`
Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/export.py`
- `resolve_checkpoint` (function) `micro/stt-training/stt_training/checkpoint.py:17` `def resolve_checkpoint(path)` -- Accept a ``.pt`` file, a run directory, or the checkpoints parent.
- `load_model` (function) `micro/stt-training/stt_training/checkpoint.py:35` `def load_model(path, device)` -- Load a checkpoint.
- `load_representative_waveforms` (function) `micro/stt-training/stt_training/checkpoint.py:61` `def load_representative_waveforms(data_roots, n, target_samples, sample_rate, seed)` -- Sample up to ``n`` fixed-length mono waveforms from ``<root>/<class>/*.wav``.

## micro/stt-training/stt_training/dataset.py
Imported by: `micro/stt-training/stt_training/evaluate.py`, `micro/stt-training/stt_training/train.py`
- `voice_id_from_path` (function) `micro/stt-training/stt_training/dataset.py:39` `def voice_id_from_path(path)` -- Stable per-voice id for speaker-independent splits.
- `SpeechCommandsDataset.__init__` (method) `micro/stt-training/stt_training/dataset.py:54` `def __init__(self, roots, classes, sample_rate, clip_seconds)`
- `SpeechCommandsDataset.voice_ids` (method) `micro/stt-training/stt_training/dataset.py:113` `def voice_ids(self)`
- `SpeechCommandsDataset.load_waveform` (method) `micro/stt-training/stt_training/dataset.py:116` `def load_waveform(self, idx)`
- `SpeechCommandsDataset.speaker_independent_split` (method) `micro/stt-training/stt_training/dataset.py:120` `def speaker_independent_split(dataset, val_fraction, seed)` -- Split indices so no voice appears in both train and val.
- `SpeechCommandsDataset.build_class_balanced_sampler` (method) `micro/stt-training/stt_training/dataset.py:142` `def build_class_balanced_sampler(labels, power)` -- Weighted sampler that softens class imbalance.
- `SpeechCommandsDataset.report_class_coverage` (method) `micro/stt-training/stt_training/dataset.py:163` `def report_class_coverage(dataset, classes)` -- Print per-class clip counts and warn about empty classes.
- `SpeechCommandsDataset.mixup` (method) `micro/stt-training/stt_training/dataset.py:190` `def mixup(x, y, num_classes, alpha)` -- Standard mixup.
- `SpeechCommandsDataset.soft_cross_entropy` (method) `micro/stt-training/stt_training/dataset.py:205` `def soft_cross_entropy(logits, soft_targets, smoothing)`

## micro/stt-training/stt_training/evaluate.py
Depends on: `micro/stt-training/stt_training/checkpoint.py`, `micro/stt-training/stt_training/dataset.py`, `micro/stt-training/stt_training/export.py`, `micro/stt-training/stt_training/features.py`, `micro/stt-training/stt_training/train.py`
- `main` (function) `micro/stt-training/stt_training/evaluate.py:38` `def main()`

## micro/stt-training/stt_training/export.py
Depends on: `micro/stt-training/stt_training/checkpoint.py`, `micro/stt-training/stt_training/features.py`
Imported by: `micro/stt-training/stt_training/evaluate.py`
- `export` (function) `micro/stt-training/stt_training/export.py:86` `def export(args)`
- `build_argparser` (function) `micro/stt-training/stt_training/export.py:207` `def build_argparser()`
- `main` (function) `micro/stt-training/stt_training/export.py:220` `def main()`


Next: [API_p9.md](API_p9.md)
