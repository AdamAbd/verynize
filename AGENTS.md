# Workspace guidance

This repository coordinates the Verynize product, marketing, and skill repositories.

- Product source lives in the `verynize-product/` Git submodule. Read its `AGENTS.md` before editing product code.
- Run product commands and tests from `verynize-product/`.
- Commit product changes inside the submodule, then commit its updated pointer in this repository.
- Marketing lives in the `verynize-marketing/` Git submodule. Read its `AGENTS.md` and run marketing commands from that directory.
- Skill documentation and distribution live in `verynize-skills/`. Read its `AGENTS.md` before editing. Sync from committed product sources; commit and push skill changes inside the submodule before updating its parent pointer.
- Never commit dependencies or generated build output to the parent repository.
