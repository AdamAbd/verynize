# Workspace guidance

This repository coordinates the Better Design product and marketing repositories.

- Product source lives in the `better-design-product/` Git submodule. Read its `AGENTS.md` before editing product code.
- Run product commands and tests from `better-design-product/`.
- Commit product changes inside the submodule, then commit its updated pointer in this repository.
- Marketing lives in the `better-design-marketing/` Git submodule. Read its `AGENTS.md` and run marketing commands from that directory.
- Never commit dependencies or generated build output to the parent repository.
