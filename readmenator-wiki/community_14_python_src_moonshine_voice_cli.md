# python/src/moonshine_voice: cli

*Community 14 | 2 files | cohesion 1.00*

## Definition

This community groups 2 file(s) rooted at `python/src/moonshine_voice` with dominant language py (cohesion 1.00). Central symbols: `_package_version`, `_usage`, `console_script`, `describe`, `main`, `run`, `test_console_scripts_are_installed`, `test_help_lists_every_command`. Core file: `python/tests/test_cli.py` (8 symbols). Documented purpose: Console-script entry point for the ``moonshine-voice`` package.  Installed as the ``moonshine-voice`` and ``moonshine`` commands via the ``[project.scripts]`` t.

## Files

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `python/src/moonshine_voice/cli.py` | py | utility | 3 | yes |
| `python/tests/test_cli.py` | py | testing | 8 | yes |

## Key Symbols

- `_package_version` (function, `python/src/moonshine_voice/cli.py:50`) `def _package_version()`
- `_usage` (function, `python/src/moonshine_voice/cli.py:68`) `def _usage()`
- `main` (function, `python/src/moonshine_voice/cli.py:91`) `def main(argv)` - Dispatch to a subcommand. Returns a process exit code.
- `console_script` (function, `python/tests/test_cli.py:24`) `def console_script(name)` - Locate the installed console script, falling back to ``python -m``.
- `run` (function, `python/tests/test_cli.py:40`) `def run()`
- `describe` (function, `python/tests/test_cli.py:49`) `def describe(result)`
- `test_console_scripts_are_installed` (function, `python/tests/test_cli.py:58`) `def test_console_scripts_are_installed(name)` - Both the primary command and the short alias must be on PATH.
- `test_help_lists_every_command` (function, `python/tests/test_cli.py:65`) `def test_help_lists_every_command()`
- `test_version_reports_package_name` (function, `python/tests/test_cli.py:72`) `def test_version_reports_package_name()`
- `test_unknown_command_is_a_usage_error` (function, `python/tests/test_cli.py:78`) `def test_unknown_command_is_a_usage_error()`
- `test_subcommand_help_parses` (function, `python/tests/test_cli.py:84`) `def test_subcommand_help_parses(command)` - ``<command> --help`` must succeed and show the friendly command prefix.

## Internal vs External Edges

- Internal resolved imports (EXTRACTED): 1
- Cross-boundary resolved imports (EXTRACTED): 0

## Connections

- No cross-community bridges recorded. This community is self-contained.

## Risks

- No scoped security, taint, cycle, or layer risks.

## Open Questions

- What would break if the most connected file in python/src/moonshine_voice: cli changed?
- Should python/src/moonshine_voice: cli be split, given cohesion 1.00?

## Sources

- `python/src/moonshine_voice/cli.py`
- `python/tests/test_cli.py`
