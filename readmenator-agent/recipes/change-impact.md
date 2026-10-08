# Recipe: Change a File Safely

Riskiest file: `core/moonshine-tts/src/rule-based-g2p.h` (51 dependents)

1. Who depends on it: `grep -n -- '-> `<file>`' readmenator-agent/ARCHITECTURE*.md`
2. Its public surface: `grep -n '`<file>:' readmenator-agent/API*.md`
3. Known risks: `grep -n '<file>' readmenator-agent/GOTCHAS.md readmenator-agent/SECURITY.md`
4. Keep signatures stable or update every importer found in step 1
5. Regenerate: `readmenator .`
