# core/moonshine-tts/src

*Community 4 | 50 files | cohesion 0.65*

## Definition

This community groups 50 file(s) rooted at `core/moonshine-tts/src` with dominant language cpp (cohesion 0.65). Central symbols: `ArabicDiacOnnx`, `BasicTokCfg`, `BiasNormJob`, `BiasNormKernel`, `BypassJob`, `BypassKernel`, `ChineseTokPosOnnx`, `Compute`. Core file: `core/moonshine-tts/src/moonshine-tts.cpp` (82 symbols). Documented purpose: Bundled Piper ONNX stems, kept in sync with ``moonshine-tts/data/*/piper-voices/*.onnx``. Regenerate the initializer from that tree when adding voices (see repo.

## Files

### `core/moonshine-tts/src` (27 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `core/moonshine-tts/src/file-information.cpp` | cpp | utility | 5 | no |
| `core/moonshine-tts/src/file-information.h` | h | utility | 10 | no |
| `core/moonshine-tts/src/g2p-path.h` | h | utility | 5 | no |
| `core/moonshine-tts/src/moonshine-asset-catalog.cpp` | cpp | utility | 13 | no |
| `core/moonshine-tts/src/moonshine-asset-catalog.h` | h | utility | 2 | no |
| `core/moonshine-tts/src/moonshine-g2p-options.cpp` | cpp | utility | 14 | no |

### `core/moonshine-tts/src/lang-specific` (10 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp` | cpp | testing | 36 | no |
| `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.h` | h | testing | 4 | no |
| `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp` | cpp | testing | 35 | no |
| `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.h` | h | testing | 5 | no |
| `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.h` | h | testing | 4 | no |

### `core/moonshine-tts/tests` (9 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `core/moonshine-tts/tests/chinese-tok-pos-onnx-test.cpp` | cpp | testing | 3 | no |
| `core/moonshine-tts/tests/file-information-test.cpp` | cpp | testing | 7 | no |
| `core/moonshine-tts/tests/japanese-onnx-g2p-test.cpp` | cpp | testing | 2 | no |
| `core/moonshine-tts/tests/japanese-tok-pos-onnx-test.cpp` | cpp | testing | 4 | no |
| `core/moonshine-tts/tests/korean-tok-pos-onnx-test.cpp` | cpp | testing | 3 | no |

### `core/moonshine-tts/tools` (3 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `core/moonshine-tts/tools/japanese-onnx-g2p-cli.cpp` | cpp | utility | 3 | no |
| `core/moonshine-tts/tools/moonshine-tts-cli.cpp` | cpp | utility | 3 | yes |
| `core/moonshine-tts/tools/piper-phoneme-infer-cli.cpp` | cpp | utility | 2 | yes |

### `core/ort-utils` (1 files)

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `core/ort-utils/ort-utils-cxx.h` | h | utility | 1 | no |

*... and 30 more files in this community.*


## Key Symbols

- `FileInformation` (function, `core/moonshine-tts/src/file-information.cpp:8`) `FileInformation::FileInformation(const FileInformation& o)     : path(o.path), o`
- `load` (function, `core/moonshine-tts/src/file-information.cpp:35`) `void FileInformation::load(const uint8_t** out_memory, size_t* out_size)`
- `free` (function, `core/moonshine-tts/src/file-information.cpp:81`) `void FileInformation::free()`
- `set_memory` (function, `core/moonshine-tts/src/file-information.cpp:90`) `void FileInformationMap::set_memory(std::string_view key, const uint8_t* mem,`
- `parse_file_list` (function, `core/moonshine-tts/src/file-information.cpp:99`) `void FileInformationMap::parse_file_list(     const std::vector<std::pair<std::s`
- `MOONSHINE_TTS_FILE_INFORMATION_H` (macro, `core/moonshine-tts/src/file-information.h:2`) `#define MOONSHINE_TTS_FILE_INFORMATION_H`
- `FileInformation` (struct, `core/moonshine-tts/src/file-information.h:18`) - Describes a bundled asset: optional on-disk ``path`` (relative to a caller root unless absolute), op
- `FileInformation` (function, `core/moonshine-tts/src/file-information.h:24`) `FileInformation(std::filesystem::path p, const uint8_t* mem, size_t sz)       :`
- `load` (function, `core/moonshine-tts/src/file-information.h:35`) `void load(const uint8_t** out_memory, size_t* out_size);` - If ``memory`` / ``memory_size`` are set (client buffer), returns them. Otherwise reads ``path`` into
- `free` (function, `core/moonshine-tts/src/file-information.h:40`) `void free();` - Drops bytes read by ``load()`` from disk. Does not free client-supplied ``memory``; clears only this
- `FileInformationMap` (struct, `core/moonshine-tts/src/file-information.h:51`) - Maps canonical asset keys (typically default relative paths such as ``fr/dict.tsv``) to ``FileInform
- `set_path` (function, `core/moonshine-tts/src/file-information.h:54`) `void set_path(std::string_view key, std::filesystem::path path)`
- `erase_key` (function, `core/moonshine-tts/src/file-information.h:63`) `void erase_key(std::string_view key)`
- `contains` (function, `core/moonshine-tts/src/file-information.h:65`) `bool contains(std::string_view key) const`
- `parse_file_list` (function, `core/moonshine-tts/src/file-information.h:71`) `void parse_file_list( const std::vector<std::pair<std::string, std::string>>* ke` - Fills ``entries`` from ``(*key_list)[i].first`` → path ``root_path / (*key_list)[i].second``, with o
- `MOONSHINE_TTS_G2P_PATH_H` (macro, `core/moonshine-tts/src/g2p-path.h:2`) `#define MOONSHINE_TTS_G2P_PATH_H`
- `resolve_path_under_root` (function, `core/moonshine-tts/src/g2p-path.h:13`) `inline std::filesystem::path resolve_path_under_root(     const std::filesystem:` - If ``path`` is absolute, returns it unchanged. If ``root`` is empty, returns ``path`` (relative to t
- `resolve_prefer_ort_model` (function, `core/moonshine-tts/src/g2p-path.h:30`) `inline std::filesystem::path resolve_prefer_ort_model(     const std::filesystem` - Prefer ``stem.ort`` when present, else ``stem.onnx`` (``basename`` may end with ``.ort`` or ``.onnx`
- `b` (function, `core/moonshine-tts/src/g2p-path.h:33`) `const std::string b(basename);`
- `resolve_disk_model_file_path` (function, `core/moonshine-tts/src/g2p-path.h:56`) `inline void resolve_disk_model_file_path(std::filesystem::path& path)` - For a path whose basename ends with ``.ort`` or ``.onnx``, set ``path`` to the existing sibling pref
- `open_ar_session` (function, `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:34`) `std::unique_ptr<Ort::Session> open_ar_session(     Ort::Env& env, const std::fil`
- `open_ar_session_memory` (function, `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:51`) `std::unique_ptr<Ort::Session> open_ar_session_memory(     Ort::Env& env, const v`
- `slurp_utf8_file_ar` (function, `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:65`) `std::string slurp_utf8_file_ar(const std::filesystem::path& p)`
- `bundle_load_utf8_ar` (function, `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:75`) `bool bundle_load_utf8_ar(const MoonshineG2POptions* opt,`
- `bundle_load_binary_ar` (function, `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:94`) `bool bundle_load_binary_ar(const MoonshineG2POptions* opt,`
- `utf8_to_u32` (function, `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:127`) `std::u32string utf8_to_u32(std::string_view utf8)`
- `u32_to_utf8` (function, `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:140`) `std::string u32_to_utf8(const std::u32string& s)`
- `is_space_u32` (function, `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:148`) `bool is_space_u32(char32_t c)`
- `is_control_u32` (function, `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:157`) `bool is_control_u32(char32_t c)`
- `is_punctuation_u32` (function, `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:166`) `bool is_punctuation_u32(char32_t c)`

## Internal vs External Edges

- Internal resolved imports (EXTRACTED): 86
- Cross-boundary resolved imports (EXTRACTED): 47

## Connections

- [EXTRACTED] depends_on community 0 <-> 4 (strength 0.9): Extracted import edge crosses communities: core/moonshine-c-api.cpp imports core/moonshine-tts/src/moonshine-asset-catalog.h.
- [EXTRACTED] depends_on community 4 <-> 2 (strength 0.9): Extracted import edge crosses communities: core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp imports core/moonshine-tts/src/utf8-utils.h.
- [EXTRACTED] depends_on community 3 <-> 4 (strength 0.9): Extracted import edge crosses communities: core/moonshine-tts/src/lang-specific/arabic.h imports core/moonshine-tts/src/lang-specific/arabic-diac-onnx.h.
- [EXTRACTED] depends_on community 7 <-> 4 (strength 0.9): Extracted import edge crosses communities: core/moonshine-tts/src/lang-specific/onnx-g2p-models.cpp imports core/moonshine-tts/src/ort-session-options.h.

## Risks

- [dataflow DEAD_STORE] `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:316` `run_split_on_punc_u32` `do_lower_case`: `do_lower_case` assigned at line 316 but never read afterwards.
- [dataflow DEAD_STORE] `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:317` `run_split_on_punc_u32` `tokenize_chinese_chars`: `tokenize_chinese_chars` assigned at line 317 but never read afterwards.
- [dataflow DEAD_STORE] `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp:818` `diacritize` `keep`: `keep` assigned at line 818 but never read afterwards.

## Open Questions

- Why do 46 file(s) lack file-level docs (e.g. `core/moonshine-tts/src/file-information.cpp`)? What purpose do they serve?
- What would break if the most connected file in core/moonshine-tts/src changed?
- Should core/moonshine-tts/src be split, given cohesion 0.65?

## Sources

- `core/moonshine-tts/src/file-information.cpp`
- `core/moonshine-tts/src/file-information.h`
- `core/moonshine-tts/src/g2p-path.h`
- `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.cpp`
- `core/moonshine-tts/src/lang-specific/arabic-diac-onnx.h`
- `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.cpp`
- `core/moonshine-tts/src/lang-specific/chinese-tok-pos-onnx.h`
- `core/moonshine-tts/src/lang-specific/japanese-onnx-g2p.h`
- `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.cpp`
- `core/moonshine-tts/src/lang-specific/japanese-tok-pos-onnx.h`
- `core/moonshine-tts/src/lang-specific/japanese.cpp`
- `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.cpp`
- `core/moonshine-tts/src/lang-specific/korean-tok-pos-onnx.h`
- `core/moonshine-tts/src/moonshine-asset-catalog.cpp`
- `core/moonshine-tts/src/moonshine-asset-catalog.h`
- `core/moonshine-tts/src/moonshine-g2p-options.cpp`
- `core/moonshine-tts/src/moonshine-g2p-options.h`
- `core/moonshine-tts/src/moonshine-tts-options.cpp`
- `core/moonshine-tts/src/moonshine-tts-options.h`
- `core/moonshine-tts/src/moonshine-tts.cpp`
- *... and 30 more*
