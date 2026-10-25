# Changelog

## REL-CALLERS-PROMPTS-1 (2026-10-24)

- The skills, README, INSTALL and `smoke-test.sh` name the `memory_save` MCP tool (G140: the old save tools are deleted, no aliases). `/remember` calls `memory_save(content="<text>")`: that tool has no `origin` argument, so the `origin="cli:add"` instruction and the tier-1 confirmation line are gone (the server sets an `mcp:` origin, tier 2, still recallable and searchable), and the confirmation now shows the save status (`saved`, `queued`, `held`, `failed`). The smoke test's tool-reference check now looks for `memory_save`.
