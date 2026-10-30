# Open-source readiness — 2026-10-30

All three GitHub repositories were already public when inspected. No visibility change was made.

Completed:
- Owner selected MIT; LICENSE, contribution terms, and scope notices added in all three repositories; package license metadata synchronized in product and marketing.
- Enabled GitHub secret scanning, push protection, and private vulnerability reporting in all three repositories.
- Added local secret/state ignore rules, contribution and security policies, CODEOWNERS, and PR templates.
- Added an opt-in manual product deployment workflow with canonical repository/main guards, read-only GitHub token permissions, pinned action commits, no persisted checkout credentials, and production environment secrets limited to the deployment step.
- Product `npm run deploy:check` passed without uploading.
- Gitleaks 8.30.1 scanned locally available Git history with `--all` in each repository. Parent and marketing: zero findings. Product: four generic-key candidates in tests/fixtures, requiring context review; this is not proof no secret exists. No remote-only refs, GitHub artifacts/logs, screenshot pixels, or credential validity were audited.

Pending:
- Resolve redistribution rights of third-party reference screenshots and verbatim vendor text; see product THIRD_PARTY_NOTICES.md. No history rewrite or deletion performed.
- Production environment, required reviewer/main restrictions, scoped deployment credentials before enabling `ENABLE_PRODUCTION_DEPLOY`. Existing local cf deployment remains available.
- Production environment configuration and third-party provenance follow-up remain separate from the branch-policy rollout.

No production deployment was performed. No Cloudflare token was copied, generated, or exposed.
