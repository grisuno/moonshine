# Subsystem: host

## micro/neural-tts/host/tts_cli.cc
- Layer: utility
- Doc: Native (desktop) driver for the on-device neural TTS engine.  Runs the EXACT C++ pipeline the RP2350 firmware runs -- sh
- Language: cc
- Symbols:
  - `Sink` (struct, line 67)
  - `ReadFile` (function, line 31) `std::vector<uint8_t> ReadFile(const char* path)`
  - `WriteWavHeader` (function, line 46) `void WriteWavHeader(FILE* f, int rate, int nsamples)`
  - `Emit` (function, line 70) `void Emit(void* user, const int16_t* samples, int n)`
  - `main` (function, line 77) `int main(int argc, char** argv)`
  - `fseek` (function, line 36) `std::fseek(f, 0, SEEK_END);`
  - `fclose` (function, line 43) `std::fclose(f);`
  - `fwrite` (function, line 52) `std::fwrite("RIFF", 1, 4, f);`
  - `w32` (function, line 53) `w32(36u + data_bytes);`
  - `w16` (function, line 57) `w16(1);`
  - `fprintf` (function, line 93) `std::fprintf(stderr, "usage: %s [--pack PACK.bin] [--ipa] [-o OUT.wav|-] TEXT\n", argv[0]);`
  - `arena` (function, line 118) `std::vector<uint8_t> arena(1u << 20);`
  - `tts` (function, line 119) `neural_tts::NeuralTts tts(pack.data(), arena.data(), arena.size());`
- Depends on: `micro/neural-tts/include/neural_tts/neural_tts.h`

## micro/neural-tts/host/worldlite_synth_cli.cc
- Layer: utility
- Doc: Host harness for WorldLiteSynth: reads raw [T,61] float32 WORLD-lite controls (f0, benv[48], bap[12]) from stdin, writes
- Language: cc
- Symbols:
  - `Ctx` (struct, line 39)
  - `main` (function, line 14) `int main(int argc, char** argv)`
  - `fprintf` (function, line 26) `fprintf(stderr, "no frames on stdin\n");`
  - `frames` (function, line 29) `std::vector<neural_tts::WorldFrame> frames(num_frames);`
  - `memcpy` (function, line 34) `memcpy(frames[t].benv, r + 1, sizeof(float) * neural_tts::kWorldNumBenv);`
  - `fwrite` (function, line 50) `fwrite(samples, sizeof(int16_t), count, stdout);`
- Depends on: `micro/neural-tts/include/neural_tts/worldlite_synth.h`
