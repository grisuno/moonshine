# Subsystem: host

## micro/neural-tts/host/tts_cli.cc
- Doc: Native (desktop) driver for the on-device neural TTS engine.
- Layer: utility
- Language: cc
- Symbols:
  - `Sink` (struct, line 67)
  - `ReadFile` (function, line 32) `std::vector<uint8_t> ReadFile(const char* path)`
  - `WriteWavHeader` (function, line 47) `void WriteWavHeader(FILE* f, int rate, int nsamples)`
  - `Emit` (function, line 71) `void Emit(void* user, const int16_t* samples, int n)`
  - `main` (function, line 78) `int main(int argc, char** argv)`
  - `arena` (function, line 118) `std::vector<uint8_t> arena(1u << 20);`
- Depends on: `micro/neural-tts/include/neural_tts/neural_tts.h`

## micro/neural-tts/host/worldlite_synth_cli.cc
- Doc: Host harness for WorldLiteSynth: reads raw [T,61] float32 WORLD-lite controls (f0, benv[48]...
- Layer: utility
- Language: cc
- Symbols:
  - `Ctx` (struct, line 39)
  - `main` (function, line 15) `int main(int argc, char** argv)`
- Depends on: `micro/neural-tts/include/neural_tts/worldlite_synth.h`
