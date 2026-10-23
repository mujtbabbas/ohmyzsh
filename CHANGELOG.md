# Changelog

All notable changes to this standalone edition of Oh My Zsh are documented in this file.

## v1.1.0 — Standalone enhancements (2026-10-20)

- Converted the repository from a fork into a standalone edition with its own history, keeping full upstream credit.
- Added an "About This Standalone Edition" section to `README.md` with the upstream link, base-version provenance, and credit.
- Added `ENHANCEMENTS.md` documenting everything changed in this edition.
- Added markdown linting automation (`.markdownlint.json` and the Markdown check workflow) for the plugin/theme documentation; the check was later scoped via `.markdownlint-cli2.yaml` so it covers this edition's own documentation instead of failing on upstream content. Upstream CI (`main.yml`), `installer.yml`, `dependencies.yml` and project workflows, which run the real installer/test tooling, were kept as-is — no additional code CI was needed.
- Dependabot: upstream already ships `.github/dependabot.yml` covering github-actions and pip (`/.github/workflows/dependencies`) — verified and kept exactly as-is.
- `.editorconfig`: upstream already ships one — kept, not added.

## v1.0.0 — Upstream baseline (2026-10-20)

- Clean standalone baseline of [ohmyzsh/ohmyzsh](https://github.com/ohmyzsh/ohmyzsh) at upstream commit `0650a250405af1e480b1ecf8c33bc960b9f333f5` (upstream HEAD dated 2026-10-19; upstream default branch is master, this edition uses main).
- Fork history severed; all 1,185 files and the licences preserved as-is (root `LICENSE.txt` is MIT; bundled plugins carry their own licence files under `plugins/*/LICENSE`), including the 9 upstream symlinks and the large plugin demo binaries.
