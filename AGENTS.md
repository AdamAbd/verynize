# Workspace guidance

This repository coordinates the Better Design product and future marketing repositories.

- Product source lives in the `better-design-product/` Git submodule. Read its `AGENTS.md` before editing product code.
- Run product commands and tests from `better-design-product/`.
- Commit product changes inside the submodule, then commit its updated pointer in this repository.
- Marketing will be added as a separate submodule when its repository is available.
- Never commit dependencies or generated build output to the parent repository.
