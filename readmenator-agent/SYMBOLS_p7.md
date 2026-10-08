# Symbols (page 7 of 12)
Previous: [SYMBOLS_p6.md](SYMBOLS_p6.md)

| Symbol | Kind | File:Line | Signature |
|--------|------|-----------|-----------|
| `TEST_CASE` | function | `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp:73` | `TEST_CASE(     "portuguese: wiki-text first 100 lines pt_br match reference IPA when data "     "...` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp:99` | `TEST_CASE(     "portuguese: wiki-text first 100 lines pt_pt match reference IPA when data "     "...` |
| `make_temp_tsv` | function | `core/moonshine-tts/tests/portuguese-rule-g2p-test.cpp:17` | `std::filesystem::path make_temp_tsv(const char* contents)` |
| `MOONSHINE_TTS_TESTS_RULE_G2P_TEST_SUPPORT_H` | macro | `core/moonshine-tts/tests/rule-g2p-test-support.h:2` | `#define MOONSHINE_TTS_TESTS_RULE_G2P_TEST_SUPPORT_H` |
| `load_ref_lines` | function | `core/moonshine-tts/tests/rule-g2p-test-support.h:76` | `inline std::vector<std::string> load_ref_lines(const std::filesystem::path& p)` |
| `load_ref_text_trimmed` | function | `core/moonshine-tts/tests/rule-g2p-test-support.h:66` | `inline std::string load_ref_text_trimmed(const std::filesystem::path& p)` |
| `moonshine_tts_bundled_data_dir_relative` | function | `core/moonshine-tts/tests/rule-g2p-test-support.h:114` | `inline std::filesystem::path moonshine_tts_bundled_data_dir_relative()` |
| `read_text_first_lines` | function | `core/moonshine-tts/tests/rule-g2p-test-support.h:96` | `inline std::vector<std::string> read_text_first_lines(     const std::filesystem::path& p, std::s...` |
| `ref_lines_prefix` | function | `core/moonshine-tts/tests/rule-g2p-test-support.h:85` | `inline std::vector<std::string> ref_lines_prefix(     const std::filesystem::path& golden, std::s...` |
| `repo_root_from_tests_cpp` | function | `core/moonshine-tts/tests/rule-g2p-test-support.h:21` | `inline std::filesystem::path repo_root_from_tests_cpp(     const char* tests_cpp_file)` |
| `split_unix_lines` | function | `core/moonshine-tts/tests/rule-g2p-test-support.h:53` | `inline std::vector<std::string> split_unix_lines(std::string block)` |
| `tests_data_dir` | function | `core/moonshine-tts/tests/rule-g2p-test-support.h:34` | `inline std::filesystem::path tests_data_dir(     const std::filesystem::path& repo_root)` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/russian-rule-g2p-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/russian-rule-g2p-test.cpp:33` | `TEST_CASE("russian: dialect_resolves_to_russian_rules")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/russian-rule-g2p-test.cpp:42` | `TEST_CASE("russian: lowercase homograph overrides capitalized")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/russian-rule-g2p-test.cpp:69` | `TEST_CASE("russian: litva matches reference IPA when data and golden exist")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/russian-rule-g2p-test.cpp:84` | `TEST_CASE(     "russian: Cyrillic preposition plus 1891 matches reference IPA when data "     "an...` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/russian-rule-g2p-test.cpp:102` | `TEST_CASE(     "russian: wiki-text first 100 lines match reference IPA when data and "     "golde...` |
| `make_temp_tsv` | function | `core/moonshine-tts/tests/russian-rule-g2p-test.cpp:21` | `std::filesystem::path make_temp_tsv(const char* contents)` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/spanish-rule-g2p-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/spanish-rule-g2p-test.cpp:35` | `TEST_CASE("spanish: En 1891 matches reference IPA when golden exists")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/spanish-rule-g2p-test.cpp:47` | `TEST_CASE("spanish: dialect ids include es-MX and es-ES")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/spanish-rule-g2p-test.cpp:53` | `TEST_CASE(     "spanish: wiki-text first 100 lines es_mx match reference IPA when data "     "and...` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/spanish-rule-g2p-test.cpp:65` | `TEST_CASE(     "spanish: wiki-text first 100 lines es_es match reference IPA when data "     "and...` |
| `check_wiki_parity` | function | `core/moonshine-tts/tests/spanish-rule-g2p-test.cpp:16` | `void check_wiki_parity(const std::filesystem::path& wiki,                        const std::files...` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/text-normalize-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/text-normalize-test.cpp:8` | `TEST_CASE("split_text_to_words")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/text-normalize-test.cpp:16` | `TEST_CASE("normalize_word_for_lookup")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/text-normalize-test.cpp:21` | `TEST_CASE("normalize_grapheme_key strips alternate suffix")` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/turkish-rule-g2p-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/turkish-rule-g2p-test.cpp:34` | `TEST_CASE("turkish: dağ and değer match reference IPA when golden exists")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/turkish-rule-g2p-test.cpp:46` | `TEST_CASE("turkish: dialect ids include tr and tr-TR")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/turkish-rule-g2p-test.cpp:52` | `TEST_CASE(     "turkish: wiki-text first 100 lines match reference IPA when data and "     "golde...` |
| `check_wiki_parity` | function | `core/moonshine-tts/tests/turkish-rule-g2p-test.cpp:16` | `void check_wiki_parity(const std::filesystem::path& wiki,                        const std::files...` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/ukrainian-rule-g2p-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/ukrainian-rule-g2p-test.cpp:34` | `TEST_CASE("ukrainian: m'ясо and кінь match reference IPA when golden exists")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/ukrainian-rule-g2p-test.cpp:46` | `TEST_CASE("ukrainian: dialect ids include uk and uk-UA")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/ukrainian-rule-g2p-test.cpp:52` | `TEST_CASE(     "ukrainian: wiki-text first 100 lines match reference IPA when data and "     "gol...` |
| `check_wiki_parity` | function | `core/moonshine-tts/tests/ukrainian-rule-g2p-test.cpp:16` | `void check_wiki_parity(const std::filesystem::path& wiki,                        const std::files...` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/utf8-utils-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/utf8-utils-test.cpp:8` | `TEST_CASE("utf8_split_codepoints ascii")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/utf8-utils-test.cpp:16` | `TEST_CASE("utf8_split_codepoints two-byte")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/utf8-utils-test.cpp:23` | `TEST_CASE("utf8_find_token_codepoints")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/utf8-utils-test.cpp:31` | `TEST_CASE("digit_ascii_span_expandable_python_w")` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/vietnamese-rule-g2p-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/vietnamese-rule-g2p-test.cpp:24` | `TEST_CASE("vietnamese: dialect_resolves_to_vietnamese_rules")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/vietnamese-rule-g2p-test.cpp:33` | `TEST_CASE("vietnamese: syllable OOV parity with Python samples")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/vietnamese-rule-g2p-test.cpp:42` | `TEST_CASE("vietnamese: lexicon line with data/vi/dict.tsv")` |
| `vi_dict_path` | function | `core/moonshine-tts/tests/vietnamese-rule-g2p-test.cpp:18` | `std::filesystem::path vi_dict_path()` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-tts/tests/zipvoice-tts-test.cpp:1` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/zipvoice-tts-test.cpp:14` | `TEST_CASE("zipvoice-builtin-voices")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/zipvoice-tts-test.cpp:46` | `TEST_CASE("zipvoice-vocos-fbank")` |
| `TEST_CASE` | function | `core/moonshine-tts/tests/zipvoice-tts-test.cpp:67` | `TEST_CASE("zipvoice-compress-long-pauses")` |
| `tone` | function | `core/moonshine-tts/tests/zipvoice-tts-test.cpp:50` | `std::vector<float> tone(static_cast<size_t>(sr));` |
| `x` | function | `core/moonshine-tts/tests/zipvoice-tts-test.cpp:70` | `std::vector<float> x(n);` |
| `main` | function | `core/moonshine-tts/tools/arabic-rule-g2p-cli.cpp:27` | `int main(int argc, char** argv)` |
| `read_all_stdin` | function | `core/moonshine-tts/tools/arabic-rule-g2p-cli.cpp:19` | `std::string read_all_stdin()` |
| `usage` | function | `core/moonshine-tts/tools/arabic-rule-g2p-cli.cpp:12` | `void usage(const char* argv0)` |
| `main` | function | `core/moonshine-tts/tools/chinese-rule-g2p-cli.cpp:28` | `int main(int argc, char** argv)` |
| `read_all_stdin` | function | `core/moonshine-tts/tools/chinese-rule-g2p-cli.cpp:20` | `std::string read_all_stdin()` |
| `usage` | function | `core/moonshine-tts/tools/chinese-rule-g2p-cli.cpp:13` | `void usage(const char* argv0)` |
| `main` | function | `core/moonshine-tts/tools/dutch-g2p-batch-cli.cpp:50` | `int main(int argc, char** argv)` |
| `read_all_stdin` | function | `core/moonshine-tts/tools/dutch-g2p-batch-cli.cpp:42` | `std::string read_all_stdin()` |
| `trim_sv` | function | `core/moonshine-tts/tools/dutch-g2p-batch-cli.cpp:30` | `std::string trim_sv(std::string s)` |
| `usage` | function | `core/moonshine-tts/tools/dutch-g2p-batch-cli.cpp:15` | `void usage(const char* argv0)` |
| `main` | function | `core/moonshine-tts/tools/dutch-rule-g2p-cli.cpp:30` | `int main(int argc, char** argv)` |
| `read_all_stdin` | function | `core/moonshine-tts/tools/dutch-rule-g2p-cli.cpp:22` | `std::string read_all_stdin()` |
| `usage` | function | `core/moonshine-tts/tools/dutch-rule-g2p-cli.cpp:13` | `void usage(const char* argv0)` |
| `main` | function | `core/moonshine-tts/tools/french-g2p-batch-cli.cpp:51` | `int main(int argc, char** argv)` |
| `read_all_stdin` | function | `core/moonshine-tts/tools/french-g2p-batch-cli.cpp:43` | `std::string read_all_stdin()` |
| `trim_sv` | function | `core/moonshine-tts/tools/french-g2p-batch-cli.cpp:31` | `std::string trim_sv(std::string s)` |
| `usage` | function | `core/moonshine-tts/tools/french-g2p-batch-cli.cpp:15` | `void usage(const char* argv0)` |
| `main` | function | `core/moonshine-tts/tools/german-rule-g2p-cli.cpp:29` | `int main(int argc, char** argv)` |
| `read_all_stdin` | function | `core/moonshine-tts/tools/german-rule-g2p-cli.cpp:21` | `std::string read_all_stdin()` |
| `usage` | function | `core/moonshine-tts/tools/german-rule-g2p-cli.cpp:13` | `void usage(const char* argv0)` |
| `main` | function | `core/moonshine-tts/tools/hindi-rule-g2p-cli.cpp:28` | `int main(int argc, char** argv)` |
| `read_all_stdin` | function | `core/moonshine-tts/tools/hindi-rule-g2p-cli.cpp:20` | `std::string read_all_stdin()` |
| `usage` | function | `core/moonshine-tts/tools/hindi-rule-g2p-cli.cpp:12` | `void usage(const char* argv0)` |
| `main` | function | `core/moonshine-tts/tools/italian-rule-g2p-cli.cpp:30` | `int main(int argc, char** argv)` |
| `read_all_stdin` | function | `core/moonshine-tts/tools/italian-rule-g2p-cli.cpp:22` | `std::string read_all_stdin()` |
| `usage` | function | `core/moonshine-tts/tools/italian-rule-g2p-cli.cpp:13` | `void usage(const char* argv0)` |
| `main` | function | `core/moonshine-tts/tools/japanese-onnx-g2p-cli.cpp:24` | `int main(int argc, char** argv)` |
| `read_all_stdin` | function | `core/moonshine-tts/tools/japanese-onnx-g2p-cli.cpp:16` | `std::string read_all_stdin()` |
| `usage` | function | `core/moonshine-tts/tools/japanese-onnx-g2p-cli.cpp:11` | `void usage(const char* argv0)` |
| `main` | function | `core/moonshine-tts/tools/korean-rule-g2p-cli.cpp:28` | `int main(int argc, char** argv)` |
| `read_all_stdin` | function | `core/moonshine-tts/tools/korean-rule-g2p-cli.cpp:20` | `std::string read_all_stdin()` |
| `usage` | function | `core/moonshine-tts/tools/korean-rule-g2p-cli.cpp:13` | `void usage(const char* argv0)` |
| `main` | function | `core/moonshine-tts/tools/moonshine-g2p-cli.cpp:160` | `int main(int argc, char **argv)` |
| `print_rule_based_dialect_catalog` | function | `core/moonshine-tts/tools/moonshine-g2p-cli.cpp:147` | `void print_rule_based_dialect_catalog(std::ostream &os)` |
| `read_all_stdin` | function | `core/moonshine-tts/tools/moonshine-g2p-cli.cpp:102` | `std::string read_all_stdin()` |
| `rule_based_kind_label` | function | `core/moonshine-tts/tools/moonshine-g2p-cli.cpp:108` | `const char *rule_based_kind_label(RuleBasedG2pKind k)` |
| `usage` | function | `core/moonshine-tts/tools/moonshine-g2p-cli.cpp:24` | `void usage(const char *argv0)` |
| `infer_lang_from_text_utf8` | function | `core/moonshine-tts/tools/moonshine-tts-cli.cpp:59` | `std::optional<std::string> infer_lang_from_text_utf8(const std::string& text)` |
| `main` | function | `core/moonshine-tts/tools/moonshine-tts-cli.cpp:85` | `int main(int argc, char** argv)` |
| `usage` | function | `core/moonshine-tts/tools/moonshine-tts-cli.cpp:15` | `void usage(const char* argv0)` |
| `load_keys` | function | `core/moonshine-tts/tools/piper-ipa-normalize-cli.cpp:22` | `bool load_keys(const std::string& path, std::unordered_set<std::string>& keys)` |
| `main` | function | `core/moonshine-tts/tools/piper-ipa-normalize-cli.cpp:42` | `int main(int argc, char** argv)` |
| `print_usage` | function | `core/moonshine-tts/tools/piper-ipa-normalize-cli.cpp:17` | `void print_usage()` |
| `main` | function | `core/moonshine-tts/tools/piper-phoneme-infer-cli.cpp:34` | `int main(int argc, char** argv)` |
| `usage` | function | `core/moonshine-tts/tools/piper-phoneme-infer-cli.cpp:18` | `void usage(const char* argv0)` |
| `main` | function | `core/moonshine-tts/tools/portuguese-rule-g2p-cli.cpp:30` | `int main(int argc, char** argv)` |
| `read_all_stdin` | function | `core/moonshine-tts/tools/portuguese-rule-g2p-cli.cpp:22` | `std::string read_all_stdin()` |
| `usage` | function | `core/moonshine-tts/tools/portuguese-rule-g2p-cli.cpp:13` | `void usage(const char* argv0)` |
| `main` | function | `core/moonshine-tts/tools/vietnamese-rule-g2p-cli.cpp:26` | `int main(int argc, char** argv)` |
| `read_all_stdin` | function | `core/moonshine-tts/tools/vietnamese-rule-g2p-cli.cpp:18` | `std::string read_all_stdin()` |
| `usage` | function | `core/moonshine-tts/tools/vietnamese-rule-g2p-cli.cpp:12` | `void usage(const char* argv0)` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-utils/debug-utils-test.cpp:6` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `SUBCASE` | function | `core/moonshine-utils/debug-utils-test.cpp:32` | `SUBCASE("LOG")` |
| `SUBCASE` | function | `core/moonshine-utils/debug-utils-test.cpp:36` | `SUBCASE("RETURN_ON_ERROR")` |
| `SUBCASE` | function | `core/moonshine-utils/debug-utils-test.cpp:37` | `SUBCASE("RETURN_ON_FALSE")` |
| `SUBCASE` | function | `core/moonshine-utils/debug-utils-test.cpp:38` | `SUBCASE("RETURN_ON_NULL")` |
| `SUBCASE` | function | `core/moonshine-utils/debug-utils-test.cpp:39` | `SUBCASE("RETURN_ON_NOT_EQUAL")` |
| `SUBCASE` | function | `core/moonshine-utils/debug-utils-test.cpp:40` | `SUBCASE("TIMER")` |
| `SUBCASE` | function | `core/moonshine-utils/debug-utils-test.cpp:45` | `SUBCASE("DEBUG_CALLOC")` |
| `SUBCASE` | function | `core/moonshine-utils/debug-utils-test.cpp:51` | `SUBCASE("TRACE")` |
| `SUBCASE` | function | `core/moonshine-utils/debug-utils-test.cpp:55` | `SUBCASE("LOG_VARS")` |
| `SUBCASE` | function | `core/moonshine-utils/debug-utils-test.cpp:76` | `SUBCASE("load_file_into_memory")` |
| `SUBCASE` | function | `core/moonshine-utils/debug-utils-test.cpp:87` | `SUBCASE("save_memory_to_file")` |
| `SUBCASE` | function | `core/moonshine-utils/debug-utils-test.cpp:100` | `SUBCASE("load_wav_data_beckett")` |
| `SUBCASE` | function | `core/moonshine-utils/debug-utils-test.cpp:114` | `SUBCASE("load_wav_data_two_cities")` |
| `SUBCASE` | function | `core/moonshine-utils/debug-utils-test.cpp:128` | `SUBCASE("save_wav_data")` |
| `TEST_CASE` | function | `core/moonshine-utils/debug-utils-test.cpp:31` | `TEST_CASE("debug-utils")` |
| `read_data` | function | `core/moonshine-utils/debug-utils-test.cpp:93` | `std::vector<uint8_t> read_data(data.size());` |
| `return_on_error_test` | function | `core/moonshine-utils/debug-utils-test.cpp:10` | `int return_on_error_test()` |
| `return_on_false_test` | function | `core/moonshine-utils/debug-utils-test.cpp:15` | `int return_on_false_test()` |
| `return_on_not_equal_test` | function | `core/moonshine-utils/debug-utils-test.cpp:25` | `int return_on_not_equal_test()` |
| `return_on_null_test` | function | `core/moonshine-utils/debug-utils-test.cpp:20` | `int return_on_null_test()` |
| `audio_int16` | function | `core/moonshine-utils/debug-utils.cpp:205` | `std::vector<int16_t> audio_int16(num_samples);` |
| `data` | function | `core/moonshine-utils/debug-utils.cpp:277` | `std::vector<uint8_t> data(size);` |
| `float_vector_stats_to_string` | function | `core/moonshine-utils/debug-utils.cpp:250` | `std::string float_vector_stats_to_string(const std::vector<float> &vector)` |
| `load_file_into_memory` | function | `core/moonshine-utils/debug-utils.cpp:269` | `std::vector<uint8_t> load_file_into_memory(const std::string &path)` |
| `load_wav_data` | function | `core/moonshine-utils/debug-utils.cpp:52` | `bool load_wav_data(const char *path, float **out_float_data,                    size_t *out_num_s...` |
| `log_backtrace` | function | `core/moonshine-utils/debug-utils.cpp:16` | `void log_backtrace()` |
| `save_memory_to_file` | function | `core/moonshine-utils/debug-utils.cpp:290` | `void save_memory_to_file(const std::string &path,                          const std::vector<uint...` |
| `save_wav_data` | function | `core/moonshine-utils/debug-utils.cpp:197` | `bool save_wav_data(const char *path, const float *audio_data,                    size_t num_sampl...` |
| `DEBUG_ALLOC_ALIGNMENT` | macro | `core/moonshine-utils/debug-utils.h:134` | `#define DEBUG_ALLOC_ALIGNMENT` |
| `DEBUG_ALLOC_LOG_MIN_SIZE` | macro | `core/moonshine-utils/debug-utils.h:136` | `#define DEBUG_ALLOC_LOG_MIN_SIZE` |
| `DEBUG_ALLOC_MAGIC` | macro | `core/moonshine-utils/debug-utils.h:132` | `#define DEBUG_ALLOC_MAGIC` |
| `DEBUG_CALLOC` | macro | `core/moonshine-utils/debug-utils.h:138` | `#define DEBUG_CALLOC(size, count)` |
| `DEBUG_CALLOC` | macro | `core/moonshine-utils/debug-utils.h:195` | `#define DEBUG_CALLOC(size, count)` |
| `DEBUG_FREE` | macro | `core/moonshine-utils/debug-utils.h:154` | `#define DEBUG_FREE(ptr)` |
| `DEBUG_FREE` | macro | `core/moonshine-utils/debug-utils.h:196` | `#define DEBUG_FREE(ptr)` |
| `ENABLE_TIMER` | macro | `core/moonshine-utils/debug-utils.h:95` | `#define ENABLE_TIMER` |
| `FILENAME_ONLY` | macro | `core/moonshine-utils/debug-utils.h:23` | `#define FILENAME_ONLY` |
| `LOG` | macro | `core/moonshine-utils/debug-utils.h:43` | `#define LOG(x)` |
| `LOGF` | macro | `core/moonshine-utils/debug-utils.h:27` | `#define LOGF(format, ...)` |
| `LOGF` | macro | `core/moonshine-utils/debug-utils.h:33` | `#define LOGF(format, ...)` |
| `LOGF_IF` | macro | `core/moonshine-utils/debug-utils.h:50` | `#define LOGF_IF(condition, format, ...)` |
| `LOG_BOOL` | macro | `core/moonshine-utils/debug-utils.h:234` | `#define LOG_BOOL(x)` |
| `LOG_BYTES` | macro | `core/moonshine-utils/debug-utils.h:235` | `#define LOG_BYTES(x, size)` |
| `LOG_FLOAT` | macro | `core/moonshine-utils/debug-utils.h:232` | `#define LOG_FLOAT(x)` |
| `LOG_IF` | macro | `core/moonshine-utils/debug-utils.h:45` | `#define LOG_IF(condition, x)` |
| `LOG_INT` | macro | `core/moonshine-utils/debug-utils.h:213` | `#define LOG_INT(x)` |
| `LOG_INT64` | macro | `core/moonshine-utils/debug-utils.h:214` | `#define LOG_INT64(x)` |
| `LOG_LONG` | macro | `core/moonshine-utils/debug-utils.h:216` | `#define LOG_LONG(x)` |
| `LOG_PTR` | macro | `core/moonshine-utils/debug-utils.h:218` | `#define LOG_PTR(x)` |
| `LOG_SIZET` | macro | `core/moonshine-utils/debug-utils.h:217` | `#define LOG_SIZET(x)` |
| `LOG_STRING` | macro | `core/moonshine-utils/debug-utils.h:233` | `#define LOG_STRING(x)` |
| `LOG_STRUCT_BYTES` | macro | `core/moonshine-utils/debug-utils.h:251` | `#define LOG_STRUCT_BYTES(x)` |
| `LOG_UINT64` | macro | `core/moonshine-utils/debug-utils.h:215` | `#define LOG_UINT64(x)` |
| `LOG_VECTOR` | macro | `core/moonshine-utils/debug-utils.h:219` | `#define LOG_VECTOR(x)` |
| `RETURN_ON_ERROR` | macro | `core/moonshine-utils/debug-utils.h:55` | `#define RETURN_ON_ERROR(error)` |
| `RETURN_ON_FALSE` | macro | `core/moonshine-utils/debug-utils.h:63` | `#define RETURN_ON_FALSE(expr)` |
| `RETURN_ON_FILE_DOES_NOT_EXIST` | macro | `core/moonshine-utils/debug-utils.h:87` | `#define RETURN_ON_FILE_DOES_NOT_EXIST(path)` |
| `RETURN_ON_NOT_EQUAL` | macro | `core/moonshine-utils/debug-utils.h:79` | `#define RETURN_ON_NOT_EQUAL(expr1, expr2)` |
| `RETURN_ON_NULL` | macro | `core/moonshine-utils/debug-utils.h:71` | `#define RETURN_ON_NULL(ptr)` |
| `THROW_WITH_LOG` | macro | `core/moonshine-utils/debug-utils.h:205` | `#define THROW_WITH_LOG(message)` |
| `TIMER_END` | macro | `core/moonshine-utils/debug-utils.h:102` | `#define TIMER_END(x)` |
| `TIMER_END` | macro | `core/moonshine-utils/debug-utils.h:120` | `#define TIMER_END(x)` |
| `TIMER_END_IF` | macro | `core/moonshine-utils/debug-utils.h:114` | `#define TIMER_END_IF(condition, x)` |
| `TIMER_END_IF` | macro | `core/moonshine-utils/debug-utils.h:122` | `#define TIMER_END_IF(condition, x)` |
| `TIMER_START` | macro | `core/moonshine-utils/debug-utils.h:99` | `#define TIMER_START(x)` |
| `TIMER_START` | macro | `core/moonshine-utils/debug-utils.h:119` | `#define TIMER_START(x)` |
| `TIMER_START_IF` | macro | `core/moonshine-utils/debug-utils.h:111` | `#define TIMER_START_IF(condition, x)` |
| `TIMER_START_IF` | macro | `core/moonshine-utils/debug-utils.h:121` | `#define TIMER_START_IF(condition, x)` |
| `TRACE` | macro | `core/moonshine-utils/debug-utils.h:200` | `#define TRACE()` |
| `UTILS_H` | macro | `core/moonshine-utils/debug-utils.h:2` | `#define UTILS_H` |
| `_moonshine_filename_without_path` | function | `core/moonshine-utils/debug-utils.h:15` | `static inline const char *_moonshine_filename_without_path(const char *path)` |
| `debug_alloc_get_size` | function | `core/moonshine-utils/debug-utils.h:176` | `static inline size_t debug_alloc_get_size(void *voidMemPtr)` |
| `debug_calloc` | function | `core/moonshine-utils/debug-utils.h:139` | `debug_calloc(size, count, FILENAME_ONLY, __LINE__, __FUNCTION__)  static inline void *debug_callo...` |
| `debug_free` | function | `core/moonshine-utils/debug-utils.h:156` | `static inline void debug_free(void *voidMemPtr, const char *file, int line,                      ...` |
| `gate` | function | `core/moonshine-utils/debug-utils.h:268` | `template <typename T> T gate(T value, T min, T max)` |
| `load_file_into_memory` | function | `core/moonshine-utils/debug-utils.h:263` | `std::vector<uint8_t> load_file_into_memory(const std::string &path);` |
| `load_wav_data` | function | `core/moonshine-utils/debug-utils.h:255` | `bool load_wav_data(const char *path, float **out_float_data, size_t *out_num_samples, int32_t *out_sample_rate =...` |
| `log_backtrace` | function | `core/moonshine-utils/debug-utils.h:253` | `void log_backtrace();` |
| `save_memory_to_file` | function | `core/moonshine-utils/debug-utils.h:264` | `void save_memory_to_file(const std::string &path, const std::vector<uint8_t> &data);` |
| `save_wav_data` | function | `core/moonshine-utils/debug-utils.h:258` | `bool save_wav_data(const char *path, const float *audio_data, size_t num_samples, uint32_t sample_rate = 16000);` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-utils/file-utils-test.cpp:9` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `SUBCASE` | function | `core/moonshine-utils/file-utils-test.cpp:28` | `SUBCASE("reads the full requested amount")` |
| `SUBCASE` | function | `core/moonshine-utils/file-utils-test.cpp:42` | `SUBCASE("reads multi-byte elements and preserves values")` |
| `SUBCASE` | function | `core/moonshine-utils/file-utils-test.cpp:59` | `SUBCASE("throws when fewer elements are available than requested")` |
| `SUBCASE` | function | `core/moonshine-utils/file-utils-test.cpp:72` | `SUBCASE("throws on a partial trailing element")` |
| `SUBCASE` | function | `core/moonshine-utils/file-utils-test.cpp:85` | `SUBCASE("throws when reading past end of file")` |
| `SUBCASE` | function | `core/moonshine-utils/file-utils-test.cpp:100` | `SUBCASE("zero count is a no-op that returns count")` |
| `SUBCASE` | function | `core/moonshine-utils/file-utils-test.cpp:109` | `SUBCASE("zero size is a no-op that returns count")` |
| `TEST_CASE` | function | `core/moonshine-utils/file-utils-test.cpp:25` | `TEST_CASE("fread_exact")` |
| `buffer` | function | `core/moonshine-utils/file-utils-test.cpp:34` | `std::vector<uint8_t> buffer(contents.size());` |
| `contents` | function | `core/moonshine-utils/file-utils-test.cpp:44` | `std::vector<uint8_t> contents(sizeof(values));` |
| `write_file` | function | `core/moonshine-utils/file-utils-test.cpp:14` | `void write_file(const char *path, const std::vector<uint8_t> &bytes)` |
| `fread_exact` | function | `core/moonshine-utils/file-utils.cpp:10` | `std::size_t fread_exact(void *ptr, std::size_t size, std::size_t count,                         s...` |
| `FILE_UTILS_H` | macro | `core/moonshine-utils/file-utils.h:2` | `#define FILE_UTILS_H` |
| `fread_exact` | function | `core/moonshine-utils/file-utils.h:12` | `std::size_t fread_exact(void *ptr, std::size_t size, std::size_t count, std::FILE *stream, const char *what = "file");` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/moonshine-utils/string-utils-test.cpp:5` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `SUBCASE` | function | `core/moonshine-utils/string-utils-test.cpp:9` | `SUBCASE("replace_all")` |
| `SUBCASE` | function | `core/moonshine-utils/string-utils-test.cpp:12` | `SUBCASE("trim")` |
| `SUBCASE` | function | `core/moonshine-utils/string-utils-test.cpp:13` | `SUBCASE("split")` |
| `SUBCASE` | function | `core/moonshine-utils/string-utils-test.cpp:17` | `SUBCASE("starts_with")` |
| `SUBCASE` | function | `core/moonshine-utils/string-utils-test.cpp:18` | `SUBCASE("starts_with_invalid")` |
| `SUBCASE` | function | `core/moonshine-utils/string-utils-test.cpp:21` | `SUBCASE("ends_with")` |
| `SUBCASE` | function | `core/moonshine-utils/string-utils-test.cpp:22` | `SUBCASE("ends_with_invalid")` |
| `SUBCASE` | function | `core/moonshine-utils/string-utils-test.cpp:25` | `SUBCASE("name_to_index")` |
| `SUBCASE` | function | `core/moonshine-utils/string-utils-test.cpp:29` | `SUBCASE("append_path_component")` |
| `SUBCASE` | function | `core/moonshine-utils/string-utils-test.cpp:35` | `SUBCASE("to_lowercase")` |
| `SUBCASE` | function | `core/moonshine-utils/string-utils-test.cpp:40` | `SUBCASE("bool_from_string")` |
| `SUBCASE` | function | `core/moonshine-utils/string-utils-test.cpp:46` | `SUBCASE("bool_from_string_invalid")` |
| `SUBCASE` | function | `core/moonshine-utils/string-utils-test.cpp:51` | `SUBCASE("float_from_string")` |
| `SUBCASE` | function | `core/moonshine-utils/string-utils-test.cpp:56` | `SUBCASE("float_from_string_invalid")` |
| `SUBCASE` | function | `core/moonshine-utils/string-utils-test.cpp:61` | `SUBCASE("int32_from_string")` |
| `SUBCASE` | function | `core/moonshine-utils/string-utils-test.cpp:66` | `SUBCASE("int32_from_string_invalid")` |
| `SUBCASE` | function | `core/moonshine-utils/string-utils-test.cpp:71` | `SUBCASE("size_t_from_string")` |
| `SUBCASE` | function | `core/moonshine-utils/string-utils-test.cpp:76` | `SUBCASE("size_t_from_string_invalid")` |
| `TEST_CASE` | function | `core/moonshine-utils/string-utils-test.cpp:8` | `TEST_CASE("string-utils")` |
| `append_path_component` | function | `core/moonshine-utils/string-utils.cpp:63` | `std::string append_path_component(const std::string &path,                                   cons...` |
| `bool_from_string` | function | `core/moonshine-utils/string-utils.cpp:92` | `bool bool_from_string(const char *input)` |
| `bool_from_string` | function | `core/moonshine-utils/string-utils.cpp:99` | `bool bool_from_string(const std::string &input)` |
| `ends_with` | function | `core/moonshine-utils/string-utils.cpp:49` | `bool ends_with(const std::string &str, const std::string &suffix)` |
| `float_from_string` | function | `core/moonshine-utils/string-utils.cpp:109` | `float float_from_string(const char *input)` |
| `float_from_string` | function | `core/moonshine-utils/string-utils.cpp:116` | `float float_from_string(const std::string &input)` |
| `int32_from_string` | function | `core/moonshine-utils/string-utils.cpp:127` | `int32_t int32_from_string(const char *input)` |
| `int32_from_string` | function | `core/moonshine-utils/string-utils.cpp:134` | `int32_t int32_from_string(const std::string &input)` |
| `replace_all` | function | `core/moonshine-utils/string-utils.cpp:9` | `std::string replace_all(std::string str, const std::string &from,                         const s...` |
| `size_t_from_string` | function | `core/moonshine-utils/string-utils.cpp:145` | `size_t size_t_from_string(const char *input)` |
| `size_t_from_string` | function | `core/moonshine-utils/string-utils.cpp:152` | `size_t size_t_from_string(const std::string &input)` |
| `split` | function | `core/moonshine-utils/string-utils.cpp:31` | `std::vector<std::string> split(const std::string &str,                                const std::...` |
| `starts_with` | function | `core/moonshine-utils/string-utils.cpp:44` | `bool starts_with(const std::string &str, const std::string &prefix)` |
| `to_lowercase` | function | `core/moonshine-utils/string-utils.cpp:86` | `std::string to_lowercase(const std::string &str)` |
| `trim` | function | `core/moonshine-utils/string-utils.cpp:21` | `std::string trim(const std::string &str, const std::string &whitespace)` |
| `STRING_UTILS_H` | macro | `core/moonshine-utils/string-utils.h:2` | `#define STRING_UTILS_H` |
| `bool_from_string` | function | `core/moonshine-utils/string-utils.h:29` | `bool bool_from_string(const std::string &input);` |
| `ends_with` | function | `core/moonshine-utils/string-utils.h:19` | `bool ends_with(const std::string &str, const std::string &suffix);` |
| `float_from_string` | function | `core/moonshine-utils/string-utils.h:32` | `float float_from_string(const std::string &input);` |
| `int32_from_string` | function | `core/moonshine-utils/string-utils.h:35` | `int32_t int32_from_string(const std::string &input);` |
| `size_t_from_string` | function | `core/moonshine-utils/string-utils.h:38` | `size_t size_t_from_string(const std::string &input);` |
| `starts_with` | function | `core/moonshine-utils/string-utils.h:17` | `bool starts_with(const std::string &str, const std::string &prefix);` |
| `MOONSHINE_TEST_UTILS_H` | macro | `core/moonshine-utils/test-utils.h:2` | `#define MOONSHINE_TEST_UTILS_H` |
| `REQUIRE_FILE_EXISTS` | macro | `core/moonshine-utils/test-utils.h:8` | `#define REQUIRE_FILE_EXISTS(filename)` |
| `DEBUG_ALLOC_ENABLED` | macro | `core/ort-utils/moonshine-ort-allocator.cpp:3` | `#define DEBUG_ALLOC_ENABLED` |
| `MoonshineAlloc` | function | `core/ort-utils/moonshine-ort-allocator.cpp:7` | `void *MoonshineAlloc(struct OrtAllocator *this_, size_t size)` |
| `MoonshineAllocOnStream` | function | `core/ort-utils/moonshine-ort-allocator.cpp:35` | `void *MoonshineAllocOnStream(struct OrtAllocator *this_, size_t size,                            ...` |
| `MoonshineFree` | function | `core/ort-utils/moonshine-ort-allocator.cpp:15` | `void MoonshineFree(struct OrtAllocator *this_, void *p)` |
| `MoonshineInfo` | function | `core/ort-utils/moonshine-ort-allocator.cpp:22` | `const struct OrtMemoryInfo *MoonshineInfo(const struct OrtAllocator *this_)` |
| `MoonshineOrtAllocator` | function | `core/ort-utils/moonshine-ort-allocator.cpp:72` | `MoonshineOrtAllocator::MoonshineOrtAllocator(const OrtMemoryInfo *memory_info)` |
| `MoonshineReserve` | function | `core/ort-utils/moonshine-ort-allocator.cpp:29` | `void *MoonshineReserve(struct OrtAllocator *this_, size_t size)` |
| `friendlySizeString` | function | `core/ort-utils/moonshine-ort-allocator.cpp:50` | `void friendlySizeString(size_t byte_count, char *output, size_t output_size)` |
| `printFriendlySize` | function | `core/ort-utils/moonshine-ort-allocator.cpp:65` | `void printFriendlySize(const char *prefix, size_t number)` |
| `print_stats` | function | `core/ort-utils/moonshine-ort-allocator.cpp:93` | `void MoonshineOrtAllocator::print_stats()` |
| `MOONSHINE_ORT_ALLOCATOR_H` | macro | `core/ort-utils/moonshine-ort-allocator.h:2` | `#define MOONSHINE_ORT_ALLOCATOR_H` |
| `MoonshineOrtAllocator` | struct | `core/ort-utils/moonshine-ort-allocator.h:8` | `` |
| `print_stats` | function | `core/ort-utils/moonshine-ort-allocator.h:24` | `void print_stats();` |
| `MoonshineTensorView` | function | `core/ort-utils/moonshine-tensor-view.cpp:117` | `MoonshineTensorView::MoonshineTensorView()     : _tensor(nullptr), name("anonymous")` |
| `MoonshineTensorView` | function | `core/ort-utils/moonshine-tensor-view.cpp:120` | `MoonshineTensorView::MoonshineTensorView(moonshine_tensor_t *tensor,                             ...` |
| `MoonshineTensorView` | function | `core/ort-utils/moonshine-tensor-view.cpp:132` | `MoonshineTensorView::MoonshineTensorView(const std::vector<int64_t> &shape,                      ...` |
| `MoonshineTensorView` | function | `core/ort-utils/moonshine-tensor-view.cpp:139` | `MoonshineTensorView::MoonshineTensorView(const MoonshineTensorView &other)     : _shape(other._sh...` |
| `MoonshineTensorView` | function | `core/ort-utils/moonshine-tensor-view.cpp:146` | `MoonshineTensorView::MoonshineTensorView(const OrtApi *ort_api,                                  ...` |
| `argmax` | function | `core/ort-utils/moonshine-tensor-view.cpp:214` | `int64_t MoonshineTensorView::argmax()` |
| `bytes_count` | function | `core/ort-utils/moonshine-tensor-view.cpp:185` | `size_t MoonshineTensorView::bytes_count()` |
| `cast_f16_to_f32` | function | `core/ort-utils/moonshine-tensor-view.cpp:202` | `MoonshineTensorView MoonshineTensorView::cast_f16_to_f32()` |
| `checked_mul` | function | `core/ort-utils/moonshine-tensor-view.cpp:18` | `bool checked_mul(size_t a, size_t b, size_t *out)` |
| `create_ort_value` | function | `core/ort-utils/moonshine-tensor-view.cpp:332` | `OrtValue *MoonshineTensorView::create_ort_value(const OrtApi *ort_api,                           ...` |
| `dtype` | function | `core/ort-utils/moonshine-tensor-view.cpp:191` | `uint32_t MoonshineTensorView::dtype()` |
| `element_count` | function | `core/ort-utils/moonshine-tensor-view.cpp:180` | `size_t MoonshineTensorView::element_count()` |
| `float16_to_float32` | function | `core/ort-utils/moonshine-tensor-view.cpp:345` | `void float16_to_float32(const uint16_t *f16_array, float *f32_array,                         size...` |
| `moonshine_dtype_to_bytes_per_element` | function | `core/ort-utils/moonshine-tensor-view.cpp:311` | `size_t moonshine_dtype_to_bytes_per_element(uint32_t moonshine_dtype)` |
| `moonshine_dtype_to_ort_dtype` | function | `core/ort-utils/moonshine-tensor-view.cpp:258` | `ONNXTensorElementDataType moonshine_dtype_to_ort_dtype(     uint32_t moonshine_dtype)` |
| `moonshine_tensor_from_ort_tensor` | function | `core/ort-utils/moonshine-tensor-view.cpp:100` | `moonshine_tensor_t *moonshine_tensor_from_ort_tensor(const OrtApi *ort_api,                      ...` |
| `moonshine_tensor_from_shape_and_dtype` | function | `core/ort-utils/moonshine-tensor-view.cpp:26` | `moonshine_tensor_t *moonshine_tensor_from_shape_and_dtype(     const std::vector<int64_t> &shape,...` |
| `moonshine_tensor_from_token_vector` | function | `core/ort-utils/moonshine-tensor-view.cpp:317` | `MoonshineTensorView *moonshine_tensor_from_token_vector(     std::vector<int32_t> &vector)` |
| `ort_dtype_to_bytes_per_element` | function | `core/ort-utils/moonshine-tensor-view.cpp:283` | `size_t ort_dtype_to_bytes_per_element(ONNXTensorElementDataType ort_dtype)` |
| `ort_dtype_to_moonshine_dtype` | function | `core/ort-utils/moonshine-tensor-view.cpp:230` | `moonshine_dtype_t ort_dtype_to_moonshine_dtype(     ONNXTensorElementDataType ort_dtype)` |
| `reshape` | function | `core/ort-utils/moonshine-tensor-view.cpp:193` | `void MoonshineTensorView::reshape(const std::vector<int64_t> &shape)` |
| `shape` | function | `core/ort-utils/moonshine-tensor-view.cpp:178` | `std::vector<int64_t> &MoonshineTensorView::shape()` |
| `to_string` | function | `core/ort-utils/moonshine-tensor-view.cpp:387` | `std::string MoonshineTensorView::to_string()` |
| `token_vector_from_moonshine_tensor` | function | `core/ort-utils/moonshine-tensor-view.cpp:325` | `std::vector<int32_t> token_vector_from_moonshine_tensor(     MoonshineTensorView *moonshine_tensor)` |
| `CHECK_DTYPE` | macro | `core/ort-utils/moonshine-tensor-view.h:21` | `#define CHECK_DTYPE(tensor, expected_dtype)` |
| `CHECK_SHAPE_RANK` | macro | `core/ort-utils/moonshine-tensor-view.h:14` | `#define CHECK_SHAPE_RANK(tensor, rank)` |
| `MOONSHINE_TENSOR_VIEW_H` | macro | `core/ort-utils/moonshine-tensor-view.h:2` | `#define MOONSHINE_TENSOR_VIEW_H` |
| `MoonshineTensorView` | struct | `core/ort-utils/moonshine-tensor-view.h:32` | `` |
| `MoonshineTensorView` | struct | `core/ort-utils/moonshine-tensor-view.h:55` | `` |
| `TENSOR_NAME` | macro | `core/ort-utils/moonshine-tensor-view.h:28` | `#define TENSOR_NAME(name)` |
| `argmax` | function | `core/ort-utils/moonshine-tensor-view.h:94` | `int64_t argmax();` |
| `bytes_count` | function | `core/ort-utils/moonshine-tensor-view.h:86` | `size_t bytes_count();` |
| `create_ort_value` | function | `core/ort-utils/moonshine-tensor-view.h:98` | `OrtValue *create_ort_value(const OrtApi *ort_api, OrtMemoryInfo *memory_info);` |
| `data` | function | `core/ort-utils/moonshine-tensor-view.h:78` | `template <typename T>   T *data()` |
| `dtype` | function | `core/ort-utils/moonshine-tensor-view.h:88` | `uint32_t dtype();` |
| `element_count` | function | `core/ort-utils/moonshine-tensor-view.h:84` | `size_t element_count();` |
| `float16_to_float32` | function | `core/ort-utils/moonshine-tensor-view.h:50` | `void float16_to_float32(const uint16_t *f16_array, float *f32_array, size_t count);` |
| `log_leaked_tensor_views` | function | `core/ort-utils/moonshine-tensor-view.h:53` | `void log_leaked_tensor_views();` |
| `moonshine_dtype_to_bytes_per_element` | function | `core/ort-utils/moonshine-tensor-view.h:34` | `size_t moonshine_dtype_to_bytes_per_element(uint32_t moonshine_dtype);` |
| `moonshine_tensor_from_token_vector` | function | `core/ort-utils/moonshine-tensor-view.h:44` | `MoonshineTensorView *moonshine_tensor_from_token_vector( std::vector<int32_t> &vector);` |
| `ort_dtype_to_bytes_per_element` | function | `core/ort-utils/moonshine-tensor-view.h:42` | `size_t ort_dtype_to_bytes_per_element(ONNXTensorElementDataType ort_dtype);` |
| `ort_dtype_to_moonshine_dtype` | function | `core/ort-utils/moonshine-tensor-view.h:36` | `moonshine_dtype_t ort_dtype_to_moonshine_dtype( ONNXTensorElementDataType ort_dtype);` |
| `reshape` | function | `core/ort-utils/moonshine-tensor-view.h:90` | `void reshape(const std::vector<int64_t> &shape);` |
| `shape` | function | `core/ort-utils/moonshine-tensor-view.h:82` | `std::vector<int64_t> &shape();` |
| `token_vector_from_moonshine_tensor` | function | `core/ort-utils/moonshine-tensor-view.h:47` | `std::vector<int32_t> token_vector_from_moonshine_tensor( MoonshineTensorView *moonshine_tensor);` |
| `return` | variable | `core/ort-utils/moonshine-tensor.cpp:6` | `extern "C" void moonshine_free_tensor(moonshine_tensor_t *tensor) { if (tensor == NULL) { return;` |
| `return` | variable | `core/ort-utils/moonshine-tensor.cpp:15` | `extern "C" void moonshine_free_tensor_list( moonshine_tensor_list_t *tensor_list) { if (tensor_list == nullptr) {...` |
| `MOONSHINE_TENSOR_H` | macro | `core/ort-utils/moonshine-tensor.h:2` | `#define MOONSHINE_TENSOR_H` |
| `moonshine_dtype_t` | variable | `core/ort-utils/moonshine-tensor.h:8` | `extern "C" { #endif typedef enum moonshine_dtype_t { MOONSHINE_DTYPE_FLOAT16 = 0, MOONSHINE_DTYPE_FLOAT32 = 1...` |
| `moonshine_dtype_t` | enum | `core/ort-utils/moonshine-tensor.h:11` | `` |
| `moonshine_free_tensor` | function | `core/ort-utils/moonshine-tensor.h:39` | `void moonshine_free_tensor(moonshine_tensor_t *tensor);` |
| `moonshine_free_tensor_list` | function | `core/ort-utils/moonshine-tensor.h:41` | `void moonshine_free_tensor_list(moonshine_tensor_list_t *tensor_list);` |
| `moonshine_tensor_list_t` | struct | `core/ort-utils/moonshine-tensor.h:34` | `` |
| `moonshine_tensor_t` | struct | `core/ort-utils/moonshine-tensor.h:27` | `` |
| `ORT_UTILS_CXX_H` | macro | `core/ort-utils/ort-utils-cxx.h:2` | `#define ORT_UTILS_CXX_H` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/ort-utils/ort-utils-ep-test.cpp:3` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `SUBCASE` | function | `core/ort-utils/ort-utils-ep-test.cpp:11` | `SUBCASE("empty string")` |
| `SUBCASE` | function | `core/ort-utils/ort-utils-ep-test.cpp:16` | `SUBCASE("comma-separated aliases")` |
| `SUBCASE` | function | `core/ort-utils/ort-utils-ep-test.cpp:23` | `SUBCASE("execution provider suffix aliases")` |
| `SUBCASE` | function | `core/ort-utils/ort-utils-ep-test.cpp:31` | `SUBCASE("empty token is rejected")` |
| `SUBCASE` | function | `core/ort-utils/ort-utils-ep-test.cpp:48` | `SUBCASE("unknown provider returns error status")` |
| `SUBCASE` | function | `core/ort-utils/ort-utils-ep-test.cpp:57` | `SUBCASE("cpu provider appends successfully")` |
| `SUBCASE` | function | `core/ort-utils/ort-utils-ep-test.cpp:64` | `SUBCASE("coreml provider appends successfully")` |
| `SUBCASE` | function | `core/ort-utils/ort-utils-ep-test.cpp:72` | `SUBCASE("nnapi provider appends successfully")` |
| `SUBCASE` | function | `core/ort-utils/ort-utils-ep-test.cpp:99` | `SUBCASE("cpu-only session creation")` |
| `SUBCASE` | function | `core/ort-utils/ort-utils-ep-test.cpp:118` | `SUBCASE("coreml session creation")` |
| `SUBCASE` | function | `core/ort-utils/ort-utils-ep-test.cpp:138` | `SUBCASE("nnapi session creation")` |
| `TEST_CASE` | function | `core/ort-utils/ort-utils-ep-test.cpp:10` | `TEST_CASE("ort_parse_provider_names")` |
| `TEST_CASE` | function | `core/ort-utils/ort-utils-ep-test.cpp:37` | `TEST_CASE("ort_append_execution_providers")` |
| `TEST_CASE` | function | `core/ort-utils/ort-utils-ep-test.cpp:83` | `TEST_CASE("ort session with execution providers")` |
| `append_one_provider` | function | `core/ort-utils/ort-utils-ep.cpp:56` | `OrtStatus *append_one_provider(     const OrtApi *ort_api, OrtSessionOptions *session_options,   ...` |
| `lowercase_copy` | function | `core/ort-utils/ort-utils-ep.cpp:29` | `std::string lowercase_copy(std::string s)` |
| `make_invalid_argument_status` | function | `core/ort-utils/ort-utils-ep.cpp:51` | `OrtStatus *make_invalid_argument_status(const OrtApi *ort_api,                                   ...` |
| `normalize_provider_name` | function | `core/ort-utils/ort-utils-ep.cpp:36` | `std::string normalize_provider_name(const std::string &name)` |
| `ort_append_execution_providers` | function | `core/ort-utils/ort-utils-ep.cpp:126` | `OrtStatus *ort_append_execution_providers(     const OrtApi *ort_api, OrtSessionOptions *session_...` |
| `ort_parse_provider_names` | function | `core/ort-utils/ort-utils-ep.cpp:102` | `std::vector<std::string> ort_parse_provider_names(const std::string &csv)` |
| `trim_copy` | function | `core/ort-utils/ort-utils-ep.cpp:17` | `std::string trim_copy(const std::string &s)` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/ort-utils/ort-utils-test.cpp:3` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `SUBCASE` | function | `core/ort-utils/ort-utils-test.cpp:8` | `SUBCASE("ort_session_from_path")` |
| `SUBCASE` | function | `core/ort-utils/ort-utils-test.cpp:12` | `SUBCASE("ort_session_from_memory")` |
| `TEST_CASE` | function | `core/ort-utils/ort-utils-test.cpp:7` | `TEST_CASE("ort-utils")` |
| `ort_get_input_shape` | function | `core/ort-utils/ort-utils.cpp:179` | `std::vector<int64_t> ort_get_input_shape(const OrtApi *ort_api,                                  ...` |
| `ort_get_input_type` | function | `core/ort-utils/ort-utils.cpp:189` | `ONNXTensorElementDataType ort_get_input_type(const OrtApi *ort_api,                              ...` |
| `ort_get_output_shape` | function | `core/ort-utils/ort-utils.cpp:199` | `std::vector<int64_t> ort_get_output_shape(const OrtApi *ort_api,                                 ...` |
| `ort_get_output_type` | function | `core/ort-utils/ort-utils.cpp:209` | `ONNXTensorElementDataType ort_get_output_type(const OrtApi *ort_api,                             ...` |
| `ort_get_shape` | function | `core/ort-utils/ort-utils.cpp:152` | `std::vector<int64_t> ort_get_shape(const OrtApi *ort_api,                                    OrtT...` |
| `ort_get_type` | function | `core/ort-utils/ort-utils.cpp:169` | `ONNXTensorElementDataType ort_get_type(const OrtApi *ort_api,                                    ...` |
| `ort_get_value_shape` | function | `core/ort-utils/ort-utils.cpp:219` | `std::vector<int64_t> ort_get_value_shape(const OrtApi *ort_api,                                  ...` |
| `ort_get_value_type` | function | `core/ort-utils/ort-utils.cpp:228` | `ONNXTensorElementDataType ort_get_value_type(const OrtApi *ort_api,                              ...` |
| `ort_maybe_force_single_thread` | function | `core/ort-utils/ort-utils.cpp:94` | `void ort_maybe_force_single_thread(const OrtApi *ort_api,                                    OrtS...` |
| `ort_run` | function | `core/ort-utils/ort-utils.cpp:237` | `OrtStatus *ort_run(const OrtApi *ort_api, OrtSession *session,                    const char *con...` |
| `ort_session_from_asset` | function | `core/ort-utils/ort-utils.cpp:107` | `int ort_session_from_asset(const OrtApi *ort_api, OrtEnv *env,                            OrtSess...` |
| `ort_session_from_memory` | function | `core/ort-utils/ort-utils.cpp:82` | `int ort_session_from_memory(const OrtApi *ort_api, OrtEnv *env,                             OrtSe...` |
| `ort_session_from_path` | function | `core/ort-utils/ort-utils.cpp:18` | `int ort_session_from_path(const OrtApi *ort_api, OrtEnv *env,                           OrtSessio...` |
| `ort_session_from_path` | function | `core/ort-utils/ort-utils.cpp:37` | `int ort_session_from_path(const OrtApi *ort_api, OrtEnv *env,                           OrtSessio...` |
| `shape` | function | `core/ort-utils/ort-utils.cpp:163` | `std::vector<int64_t> shape(num_dims);` |
| `LOG_ORT_ERROR` | macro | `core/ort-utils/ort-utils.h:30` | `#define LOG_ORT_ERROR(ort_api, expr)` |
| `ORT_RUN` | macro | `core/ort-utils/ort-utils.h:82` | `#define ORT_RUN(ort_api, session, input_names, inputs, input_count,         \                 output_names...` |
| `ORT_UTILS_H` | macro | `core/ort-utils/ort-utils.h:2` | `#define ORT_UTILS_H` |
| `OrtExecutionProviderOptions` | struct | `core/ort-utils/ort-utils.h:15` | `` |
| `RETURN_ON_ORT_ERROR` | macro | `core/ort-utils/ort-utils.h:19` | `#define RETURN_ON_ORT_ERROR(ort_api, expr)` |
| `ort_append_execution_providers` | function | `core/ort-utils/ort-utils.h:109` | `OrtStatus *ort_append_execution_providers( const OrtApi *ort_api, OrtSessionOptions *session_options, const...` |
| `ort_configure_execution_providers` | function | `core/ort-utils/ort-utils.h:114` | `inline void ort_configure_execution_providers(     const OrtApi *ort_api, OrtSessionOptions *sess...` |
| `ort_get_input_shape` | function | `core/ort-utils/ort-utils.h:64` | `std::vector<int64_t> ort_get_input_shape(const OrtApi *ort_api, OrtSession *session, int index);` |
| `ort_get_output_shape` | function | `core/ort-utils/ort-utils.h:70` | `std::vector<int64_t> ort_get_output_shape(const OrtApi *ort_api, OrtSession *session, int index);` |
| `ort_get_shape` | function | `core/ort-utils/ort-utils.h:58` | `std::vector<int64_t> ort_get_shape(const OrtApi *ort_api, OrtTypeInfo *type_info);` |
| `ort_get_value_shape` | function | `core/ort-utils/ort-utils.h:76` | `std::vector<int64_t> ort_get_value_shape(const OrtApi *ort_api, const OrtValue *value);` |
| `ort_maybe_force_single_thread` | function | `core/ort-utils/ort-utils.h:104` | `void ort_maybe_force_single_thread(const OrtApi *ort_api, OrtSessionOptions *session_options);` |
| `ort_session_from_asset` | function | `core/ort-utils/ort-utils.h:51` | `int ort_session_from_asset(const OrtApi *ort_api, OrtEnv *env, OrtSessionOptions *session_options, AAssetManager...` |
| `ort_session_from_memory` | function | `core/ort-utils/ort-utils.h:45` | `int ort_session_from_memory(const OrtApi *ort_api, OrtEnv *env, OrtSessionOptions *session_options, const uint8_t...` |
| `ort_session_from_path` | function | `core/ort-utils/ort-utils.h:40` | `int ort_session_from_path(const OrtApi *ort_api, OrtEnv *env, OrtSessionOptions *session_options, const char *path...` |
| `text` | function | `core/reliability/fuzz-bin-tokenizer.cpp:25` | `const std::string text(data, data + text_size);` |
| `0` | variable | `core/reliability/fuzz-resampler.cpp:32` | `extern "C" int LLVMFuzzerTestOneInput(const uint8_t *data, size_t size) { // Layout: [4 bytes input rate][4 bytes...` |
| `audio` | function | `core/reliability/fuzz-resampler.cpp:45` | `std::vector<float> audio(num_samples);` |
| `sane_rate` | function | `core/reliability/fuzz-resampler.cpp:17` | `float sane_rate(float rate)` |
| `input` | function | `core/reliability/fuzz-string-utils.cpp:15` | `const std::string input(data, data + size);` |
| `Reader` | struct | `core/reliability/fuzz-tensor-view.cpp:21` | `` |
| `next_i64` | function | `core/reliability/fuzz-tensor-view.cpp:28` | `int64_t next_i64()` |
| `next_u8` | function | `core/reliability/fuzz-tensor-view.cpp:26` | `uint8_t next_u8()` |
| `source` | function | `core/reliability/fuzz-tensor-view.cpp:82` | `std::vector<uint8_t> source(element_count * 8, 0);` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/resampler-test.cpp:9` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `SUBCASE` | function | `core/resampler-test.cpp:45` | `SUBCASE("resample-audio")` |
| `TEST_CASE` | function | `core/resampler-test.cpp:44` | `TEST_CASE("resampler-test")` |
| `max_element` | function | `core/resampler-test.cpp:20` | `*std::max_element(input_audio.begin(), input_audio.end());` |
| `min_element` | function | `core/resampler-test.cpp:27` | `*std::min_element(input_audio.begin(), input_audio.end());` |
| `test_resample_audio` | function | `core/resampler-test.cpp:13` | `void test_resample_audio(const std::vector<float> &input_audio,                          int32_t ...` |
| `wav_data_vector` | function | `core/resampler-test.cpp:55` | `const std::vector<float> wav_data_vector(wav_data, wav_data + wav_data_size);` |
| `downsample_audio` | function | `core/resampler.cpp:17` | `const std::vector<float> downsample_audio(const std::vector<float> &audio,                       ...` |
| `output_audio` | function | `core/resampler.cpp:23` | `std::vector<float> output_audio(output_audio_size);` |
| `resample_audio` | function | `core/resampler.cpp:5` | `const std::vector<float> resample_audio(const std::vector<float> &audio,                         ...` |
| `upsample_audio` | function | `core/resampler.cpp:56` | `const std::vector<float> upsample_audio(const std::vector<float> &audio,                         ...` |
| `RESAMPLER_H` | macro | `core/resampler.h:2` | `#define RESAMPLER_H` |
| `downsample_audio` | function | `core/resampler.h:10` | `const std::vector<float> downsample_audio(const std::vector<float> &audio, float input_sample_rate, float...` |
| `resample_audio` | function | `core/resampler.h:6` | `const std::vector<float> resample_audio(const std::vector<float> &audio, float input_sample_rate, float...` |
| `upsample_audio` | function | `core/resampler.h:14` | `const std::vector<float> upsample_audio(const std::vector<float> &audio, float input_sample_rate, float...` |
| `SileroVad` | function | `core/silero-vad.cpp:30` | `SileroVad::SileroVad(int sample_rate, int windows_frame_size, float threshold,                   ...` |
| `init_engine_threads` | function | `core/silero-vad.cpp:21` | `void SileroVad::init_engine_threads(int inter_threads, int intra_threads)` |
| `init_onnx_env` | function | `core/silero-vad.cpp:6` | `void SileroVad::init_onnx_env()` |
| `load_from_memory` | function | `core/silero-vad.cpp:60` | `int SileroVad::load_from_memory(const uint8_t *model_data,                                 size_t...` |
| `predict` | function | `core/silero-vad.cpp:78` | `void SileroVad::predict(const std::vector<float> &data_chunk,                         float *out_...` |
| `SileroVad` | class | `core/silero-vad.h:22` | `` |
| `init_engine_threads` | function | `core/silero-vad.h:71` | `void init_engine_threads(int inter_threads, int intra_threads);` |
| `init_onnx_env` | function | `core/silero-vad.h:68` | `void init_onnx_env();` |
| `is_loaded` | function | `core/silero-vad.h:85` | `bool is_loaded() const` |
| `load_from_memory` | function | `core/silero-vad.h:83` | `int load_from_memory(const uint8_t *model_data, size_t model_data_size);` |
| `predict` | function | `core/silero-vad.h:87` | `void predict(const std::vector<float> &data_chunk, float *out_probability, int *out_flag);` |
| `Impl` | function | `core/speaker-diarizer.cpp:67` | `explicit Impl(const SpeakerDiarizerOptions &options_in)       : engine(), options(options_in)` |
| `SpeakerDiarizer` | function | `core/speaker-diarizer.cpp:171` | `SpeakerDiarizer::SpeakerDiarizer(const SpeakerDiarizerOptions &options)     : impl(std::make_uniq...` |
| `StreamState` | struct | `core/speaker-diarizer.cpp:43` | `` |
| `add_audio_to_stream` | function | `core/speaker-diarizer.cpp:201` | `void SpeakerDiarizer::add_audio_to_stream(int32_t stream_id,                                     ...` |
| `allocate_stable_id` | function | `core/speaker-diarizer.cpp:92` | `uint64_t allocate_stable_id()` |
| `create_stream` | function | `core/speaker-diarizer.cpp:176` | `int32_t SpeakerDiarizer::create_stream()` |
| `diarize` | function | `core/speaker-diarizer.cpp:236` | `std::vector<SpeakerTurn> SpeakerDiarizer::diarize(const float *audio_data,                       ...` |
| `finish_stream` | function | `core/speaker-diarizer.cpp:225` | `std::vector<SpeakerTurn> SpeakerDiarizer::finish_stream(int32_t stream_id)` |
| `free_stream` | function | `core/speaker-diarizer.cpp:186` | `void SpeakerDiarizer::free_stream(int32_t stream_id)` |
| `get_stream` | function | `core/speaker-diarizer.cpp:83` | `StreamState &get_stream(int32_t stream_id)` |
| `get_turns` | function | `core/speaker-diarizer.cpp:218` | `std::vector<SpeakerTurn> SpeakerDiarizer::get_turns(int32_t stream_id)` |
| `map_snapshot_to_stable_ids` | function | `core/speaker-diarizer.cpp:102` | `void map_snapshot_to_stable_ids(       StreamState &state,       const cppannote::StreamingDiariz...` |
| `session_config` | function | `core/speaker-diarizer.cpp:75` | `cppannote::StreamingDiarizationConfig session_config() const` |
| `sort` | function | `core/speaker-diarizer.cpp:135` | `std::sort(candidates.begin(), candidates.end(),               [](const auto &a, const auto &b)` |
| `start_stream` | function | `core/speaker-diarizer.cpp:191` | `void SpeakerDiarizer::start_stream(int32_t stream_id)` |
| `turn_overlap_seconds` | function | `core/speaker-diarizer.cpp:17` | `double turn_overlap_seconds(     const std::vector<cppannote::StreamingDiarizationTurn> &a, int32...` |
| `Impl` | struct | `core/speaker-diarizer.h:74` | `` |
| `SPEAKER_DIARIZER_H` | macro | `core/speaker-diarizer.h:2` | `#define SPEAKER_DIARIZER_H` |
| `SpeakerDiarizer` | class | `core/speaker-diarizer.h:42` | `` |
| `SpeakerDiarizerOptions` | struct | `core/speaker-diarizer.h:24` | `` |
| `SpeakerTurn` | struct | `core/speaker-diarizer.h:10` | `` |
| `add_audio_to_stream` | function | `core/speaker-diarizer.h:58` | `void add_audio_to_stream(int32_t stream_id, const float *audio_data, uint64_t audio_length, int32_t sample_rate);` |
| `create_stream` | function | `core/speaker-diarizer.h:51` | `int32_t create_stream();` |
| `free_stream` | function | `core/speaker-diarizer.h:52` | `void free_stream(int32_t stream_id);` |
| `start_stream` | function | `core/speaker-diarizer.h:53` | `void start_stream(int32_t stream_id);` |
| `build_set` | function | `core/spelling-fusion-data.cpp:28` | `std::unordered_set<std::string> build_set(     std::initializer_list<const char *> phrases)` |
| `clear_words` | function | `core/spelling-fusion-data.cpp:309` | `const std::unordered_set<std::string> &clear_words()` |
| `default_meta` | function | `core/spelling-fusion-data.cpp:356` | `const DefaultSpellingMeta &default_meta()` |
| `default_weak_homonyms` | function | `core/spelling-fusion-data.cpp:338` | `const std::unordered_set<std::string> &default_weak_homonyms()` |
| `sort` | function | `core/spelling-fusion-data.cpp:287` | `std::sort(v.begin(), v.end(),               [](const std::string &a, const std::string &b)` |
| `stop_words` | function | `core/spelling-fusion-data.cpp:319` | `const std::unordered_set<std::string> &stop_words()` |
| `undo_words` | function | `core/spelling-fusion-data.cpp:296` | `const std::unordered_set<std::string> &undo_words()` |
| `upper_modifiers` | function | `core/spelling-fusion-data.cpp:268` | `const std::unordered_set<std::string> &upper_modifiers()` |
| `upper_modifiers_by_length` | function | `core/spelling-fusion-data.cpp:281` | `const std::vector<std::string> &upper_modifiers_by_length()` |
| `DefaultSpellingMeta` | struct | `core/spelling-fusion-data.h:53` | `` |
| `SPELLING_FUSION_DATA_H` | macro | `core/spelling-fusion-data.h:2` | `#define SPELLING_FUSION_DATA_H` |
| `clear_words` | function | `core/spelling-fusion-data.h:33` | `const std::unordered_set<std::string> &clear_words();` |
| `default_meta` | function | `core/spelling-fusion-data.h:60` | `const DefaultSpellingMeta &default_meta();` |
| `default_weak_homonyms` | function | `core/spelling-fusion-data.h:40` | `const std::unordered_set<std::string> &default_weak_homonyms();` |
| `stop_words` | function | `core/spelling-fusion-data.h:34` | `const std::unordered_set<std::string> &stop_words();` |
| `undo_words` | function | `core/spelling-fusion-data.h:32` | `const std::unordered_set<std::string> &undo_words();` |
| `upper_modifiers` | function | `core/spelling-fusion-data.h:27` | `const std::unordered_set<std::string> &upper_modifiers();` |
| `upper_modifiers_by_length` | function | `core/spelling-fusion-data.h:28` | `const std::vector<std::string> &upper_modifiers_by_length();` |
| `DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` | macro | `core/spelling-fusion-test.cpp:7` | `#define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN` |
| `TEST_CASE` | function | `core/spelling-fusion-test.cpp:25` | `TEST_CASE("spelling-fusion: normalize")` |
| `TEST_CASE` | function | `core/spelling-fusion-test.cpp:39` | `TEST_CASE("spelling-fusion: matcher classifies plain letters")` |
| `TEST_CASE` | function | `core/spelling-fusion-test.cpp:50` | `TEST_CASE("spelling-fusion: matcher classifies NATO codewords")` |
| `TEST_CASE` | function | `core/spelling-fusion-test.cpp:61` | `TEST_CASE("spelling-fusion: matcher classifies digits")` |
| `TEST_CASE` | function | `core/spelling-fusion-test.cpp:73` | `TEST_CASE("spelling-fusion: matcher parses 10..1000 number words")` |
| `TEST_CASE` | function | `core/spelling-fusion-test.cpp:85` | `TEST_CASE("spelling-fusion: matcher applies upper-case modifier")` |
| `TEST_CASE` | function | `core/spelling-fusion-test.cpp:94` | `TEST_CASE("spelling-fusion: matcher recognizes speller patterns")` |
| `TEST_CASE` | function | `core/spelling-fusion-test.cpp:103` | `TEST_CASE("spelling-fusion: matcher classifies command words")` |
| `TEST_CASE` | function | `core/spelling-fusion-test.cpp:114` | `TEST_CASE("spelling-fusion: matcher classifies special characters")` |
| `TEST_CASE` | function | `core/spelling-fusion-test.cpp:149` | `TEST_CASE("spelling-fusion: weak-homonym detection")` |
| `TEST_CASE` | function | `core/spelling-fusion-test.cpp:158` | `TEST_CASE("spelling-fusion: fuse without prediction")` |
| `TEST_CASE` | function | `core/spelling-fusion-test.cpp:166` | `TEST_CASE("spelling-fusion: fuse drops unrecognized + no prediction")` |
| `TEST_CASE` | function | `core/spelling-fusion-test.cpp:173` | `TEST_CASE("spelling-fusion: fuse passes through command words")` |
| `TEST_CASE` | function | `core/spelling-fusion-test.cpp:183` | `TEST_CASE(     "spelling-fusion: special-character match is preserved when the "     "spelling mo...` |
| `TEST_CASE` | function | `core/spelling-fusion-test.cpp:204` | `TEST_CASE("spelling-fusion: weak-homonym demotion")` |
| `TEST_CASE` | function | `core/spelling-fusion-test.cpp:225` | `TEST_CASE("spelling-fusion: cross-class routing")` |
| `TEST_CASE` | function | `core/spelling-fusion-test.cpp:238` | `TEST_CASE("spelling-fusion: same-class disagreement uses threshold")` |
| `TEST_CASE` | function | `core/spelling-fusion-test.cpp:251` | `TEST_CASE("spelling-fusion: multi-digit ASR vs single-digit spelling")` |
| `TEST_CASE` | function | `core/spelling-fusion-test.cpp:275` | `TEST_CASE("spelling-fusion: agreement preserves matcher casing")` |
| `TEST_CASE` | function | `core/spelling-fusion-test.cpp:284` | `TEST_CASE("spelling-fusion: spelling-only when matcher misses")` |
| `TEST_CASE` | function | `core/spelling-fusion-test.cpp:293` | `TEST_CASE("spelling-fusion: data tables are non-empty")` |
| `char_match` | function | `core/spelling-fusion-test.cpp:13` | `SpellingMatch char_match(const std::string &c)` |
| `no_match` | function | `core/spelling-fusion-test.cpp:21` | `SpellingMatch no_match()` |
| `SpellingMatcher` | function | `core/spelling-fusion.cpp:234` | `SpellingMatcher::SpellingMatcher()     : lookup_(&spelling_fusion_data::lookup_table()),       up...` |
| `apply_case` | function | `core/spelling-fusion.cpp:393` | `std::string apply_case(const std::string &ch, const std::string &hint)` |
| `ascii_to_lower` | function | `core/spelling-fusion.cpp:39` | `char ascii_to_lower(char c)` |
| `classify` | function | `core/spelling-fusion.cpp:244` | `SpellingMatch SpellingMatcher::classify(const std::string &raw_text) const` |
| `consume_curly_quote` | function | `core/spelling-fusion.cpp:46` | `size_t consume_curly_quote(const std::string &input, size_t i)` |
| `fuse_default` | function | `core/spelling-fusion.cpp:407` | `FusedResult fuse_default(const std::string &raw_text,                          const SpellingMatc...` |
| `is_ascii_digit_string` | function | `core/spelling-fusion.cpp:181` | `bool is_ascii_digit_string(const std::string &s)` |
| `is_ascii_drop` | function | `core/spelling-fusion.cpp:25` | `bool is_ascii_drop(char c)` |
| `is_ascii_letter` | function | `core/spelling-fusion.cpp:35` | `bool is_ascii_letter(char c)` |
| `is_printable_ascii` | function | `core/spelling-fusion.cpp:189` | `bool is_printable_ascii(char c)` |
| `is_weak_homonym` | function | `core/spelling-fusion.cpp:300` | `bool SpellingMatcher::is_weak_homonym(const std::string &raw_text) const` |
| `parse_number_words` | function | `core/spelling-fusion.cpp:108` | `std::optional<int> parse_number_words(const std::string &text)` |
| `resolve` | function | `core/spelling-fusion.cpp:305` | `std::optional<std::string> SpellingMatcher::resolve(     const std::string &text) const` |
| `resolve_spelled_letter` | function | `core/spelling-fusion.cpp:326` | `std::optional<std::string> SpellingMatcher::resolve_spelled_letter(     const std::string &text) ...` |
| `single_char_is_letter` | function | `core/spelling-fusion.cpp:389` | `bool single_char_is_letter(const std::string &c)` |
| `spelling_normalize` | function | `core/spelling-fusion.cpp:195` | `std::string spelling_normalize(const std::string &text)` |
| `split_on_whitespace` | function | `core/spelling-fusion.cpp:62` | `std::vector<std::string> split_on_whitespace(const std::string &s)` |
| `string_is_digit` | function | `core/spelling-fusion.cpp:381` | `bool string_is_digit(const std::string &c)` |
| `string_is_letter` | function | `core/spelling-fusion.cpp:373` | `bool string_is_letter(const std::string &c)` |
| `FusedResult` | struct | `core/spelling-fusion.h:88` | `` |
| `SPELLING_FUSION_H` | macro | `core/spelling-fusion.h:2` | `#define SPELLING_FUSION_H` |

Next: [SYMBOLS_p8.md](SYMBOLS_p8.md)
