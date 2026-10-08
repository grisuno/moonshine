# Recipe: Reduce File Complexity

Target hotspot: `core/moonshine-c-api.cpp`
(complexity 0.6, centrality 0.9)

1. Read dependents: `grep -n 'core/moonshine-c-api.cpp' readmenator-agent/ARCHITECTURE*.md`
2. Extract functions/classes into new files in the same subsystem
3. Update imports
4. Regenerate: `readmenator .`
