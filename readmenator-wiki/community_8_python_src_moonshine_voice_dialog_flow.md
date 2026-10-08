# python/src/moonshine_voice: dialog_flow

*Community 8 | 18 files | cohesion 1.00*

## Definition

This community groups 18 file(s) rooted at `python/src/moonshine_voice` with dominant language py (cohesion 1.00). Central symbols: `AlphanumericEvent`, `AlphanumericEventType`, `AlphanumericListener`, `AlphanumericMatch`, `AlphanumericMatcher`, `Ask`, `CachedEmbeddings`, `Choose`. Core file: `python/src/moonshine_voice/dialog_flow.py` (94 symbols). Documented purpose: Moonshine Voice - Fast, accurate, on-device AI library for building interactive voice applications.  This package provides Python bindings for the Moonshine Voi.

## Files

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `python/src/moonshine_voice/__init__.py` | py | utility | 1 | yes |
| `python/src/moonshine_voice/alphanumeric_listener.py` | py | utility | 31 | yes |
| `python/src/moonshine_voice/cached_embeddings.py` | py | infrastructure | 19 | yes |
| `python/src/moonshine_voice/dialog_flow.py` | py | utility | 94 | yes |
| `python/src/moonshine_voice/download.py` | py | utility | 43 | no |
| `python/src/moonshine_voice/download_file.py` | py | utility | 4 | no |
| `python/src/moonshine_voice/errors.py` | py | utility | 15 | yes |
| `python/src/moonshine_voice/g2p.py` | py | utility | 10 | yes |
| `python/src/moonshine_voice/intent_recognizer.py` | py | utility | 29 | yes |
| `python/src/moonshine_voice/mic_transcriber.py` | py | utility | 30 | no |
| `python/src/moonshine_voice/moonshine_api.py` | py | presentation | 37 | no |
| `python/src/moonshine_voice/tts.py` | py | utility | 44 | yes |
| `python/src/moonshine_voice/utils.py` | py | utility | 3 | yes |
| `python/tests/test_modules.py` | py | testing | 11 | yes |
| `scripts/analyze_ko_stress.py` | py | utility | 8 | yes |
| `scripts/compare_ko_phonemes.py` | py | utility | 5 | yes |
| `scripts/eval-alphanumeric.py` | py | utility | 5 | yes |
| `scripts/tts_g2p_intelligibility.py` | py | utility | 62 | yes |

## Key Symbols

- `__getattr__` (function, `python/src/moonshine_voice/__init__.py:81`) `def __getattr__(name)` - Lazy import for transcriber, mic_transcriber, and intent_recognizer modules.
- `AlphanumericEventType` (class, `python/src/moonshine_voice/alphanumeric_listener.py:40`) `class AlphanumericEventType(Enum)`
- `AlphanumericEvent` (class, `python/src/moonshine_voice/alphanumeric_listener.py:49`) `class AlphanumericEvent` - Event delivered to the callback each time something happens.
- `AlphanumericMatch` (class, `python/src/moonshine_voice/alphanumeric_listener.py:69`) `class AlphanumericMatch` - Pure classification result produced by :class:`AlphanumericMatcher`.
- `is_character` (method, `python/src/moonshine_voice/alphanumeric_listener.py:80`) `def is_character(self)`
- `is_terminator` (method, `python/src/moonshine_voice/alphanumeric_listener.py:84`) `def is_terminator(self)`
- `is_recognized` (method, `python/src/moonshine_voice/alphanumeric_listener.py:88`) `def is_recognized(self)`
- `spoken_form` (method, `python/src/moonshine_voice/alphanumeric_listener.py:306`) `def spoken_form(char)` - Return a TTS-friendly phrase for a single character.
- `_normalize` (method, `python/src/moonshine_voice/alphanumeric_listener.py:355`) `def _normalize(text)` - Return *text* lower-cased with quotes/punctuation removed.
- `_build_lookup` (method, `python/src/moonshine_voice/alphanumeric_listener.py:370`) `def _build_lookup()` - Merge all character vocabularies into a single lookup table.
- `_parse_number_words` (method, `python/src/moonshine_voice/alphanumeric_listener.py:424`) `def _parse_number_words(text)` - Parse English number words in the range 10 – 1 000.
- `AlphanumericMatcher` (class, `python/src/moonshine_voice/alphanumeric_listener.py:512`) `class AlphanumericMatcher` - Stateless classifier for spelled letter / digit / command utterances.
- `__init__` (method, `python/src/moonshine_voice/alphanumeric_listener.py:542`) `def __init__(self)`
- `classify` (method, `python/src/moonshine_voice/alphanumeric_listener.py:570`) `def classify(self, raw_text)` - Classify a single utterance into an :class:`AlphanumericMatch`.
- `classify_sequence` (method, `python/src/moonshine_voice/alphanumeric_listener.py:606`) `def classify_sequence(self, raw_text)` - Classify a potentially multi-token utterance.
- `_resolve` (method, `python/src/moonshine_voice/alphanumeric_listener.py:637`) `def _resolve(self, text)`
- `_resolve_spelled_letter` (method, `python/src/moonshine_voice/alphanumeric_listener.py:652`) `def _resolve_spelled_letter(self, text)` - Recognise speller patterns like ``"A for Alpha"`` / ``"B as in Boy"``.
- `_char_accepted` (method, `python/src/moonshine_voice/alphanumeric_listener.py:705`) `def _char_accepted(self, char)`
- `letters_only_matcher` (method, `python/src/moonshine_voice/alphanumeric_listener.py:716`) `def letters_only_matcher()`
- `digits_only_matcher` (method, `python/src/moonshine_voice/alphanumeric_listener.py:720`) `def digits_only_matcher()`
- `AlphanumericListener` (class, `python/src/moonshine_voice/alphanumeric_listener.py:738`) `class AlphanumericListener` - Listens for single-character dictation and assembles the result.
- `__init__` (method, `python/src/moonshine_voice/alphanumeric_listener.py:808`) `def __init__(self, callback)`
- `__call__` (method, `python/src/moonshine_voice/alphanumeric_listener.py:829`) `def __call__(self, event)`
- `text` (method, `python/src/moonshine_voice/alphanumeric_listener.py:840`) `def text(self)` - The currently assembled text.
- `stopped` (method, `python/src/moonshine_voice/alphanumeric_listener.py:845`) `def stopped(self)` - Whether a stop command has been received.
- `matcher` (method, `python/src/moonshine_voice/alphanumeric_listener.py:850`) `def matcher(self)` - The underlying :class:`AlphanumericMatcher`.
- `clear` (method, `python/src/moonshine_voice/alphanumeric_listener.py:854`) `def clear(self)` - Programmatically clear the buffer.
- `undo` (method, `python/src/moonshine_voice/alphanumeric_listener.py:865`) `def undo(self)` - Remove and return the last character, or ``None`` if empty.
- `_process_utterance` (method, `python/src/moonshine_voice/alphanumeric_listener.py:879`) `def _process_utterance(self, line)`
- `_speak_character` (method, `python/src/moonshine_voice/alphanumeric_listener.py:941`) `def _speak_character(self, char)` - Speak the TTS phrase for ``char`` if a TTS backend is wired.

## Internal vs External Edges

- Internal resolved imports (EXTRACTED): 40
- Cross-boundary resolved imports (EXTRACTED): 0

## Connections

- [INFERRED] shares_context community 0 <-> 8 (strength 0.5): Inferred shared context (layer utility) with no import path between community 0 (core: moonshine-cpp) and community 8 (python/src/moonshine_voice: dialog_flow).

## Risks

- [layer strict] `python/tests/test_modules.py` (testing) -> `python/src/moonshine_voice/moonshine_api.py` (presentation)

## Open Questions

- Why do 4 file(s) lack file-level docs (e.g. `python/src/moonshine_voice/download.py`)? What purpose do they serve?
- What would break if the most connected file in python/src/moonshine_voice: dialog_flow changed?
- Should python/src/moonshine_voice: dialog_flow be split, given cohesion 1.00?

## Sources

- `python/src/moonshine_voice/__init__.py`
- `python/src/moonshine_voice/alphanumeric_listener.py`
- `python/src/moonshine_voice/cached_embeddings.py`
- `python/src/moonshine_voice/dialog_flow.py`
- `python/src/moonshine_voice/download.py`
- `python/src/moonshine_voice/download_file.py`
- `python/src/moonshine_voice/errors.py`
- `python/src/moonshine_voice/g2p.py`
- `python/src/moonshine_voice/intent_recognizer.py`
- `python/src/moonshine_voice/mic_transcriber.py`
- `python/src/moonshine_voice/moonshine_api.py`
- `python/src/moonshine_voice/tts.py`
- `python/src/moonshine_voice/utils.py`
- `python/tests/test_modules.py`
- `scripts/analyze_ko_stress.py`
- `scripts/compare_ko_phonemes.py`
- `scripts/eval-alphanumeric.py`
- `scripts/tts_g2p_intelligibility.py`
