# Enhancements — Standalone Edition Changelog

Upstream: <https://github.com/ohmyzsh/ohmyzsh>
Maintainer of this edition: Syed Mujtaba Abbas (@mujtbabbas)

## v1.1.0 — Enhancement release (2026-10-20)

- Added "About This Standalone Edition" section to README.md with upstream
  link, base version provenance, and credit.

- Added this changelog (ENHANCEMENTS.md).
- Added .markdownlint.json and .github/workflows/markdown-check.yml
  (markdown linting automation for the plugin/theme documentation;
  upstream CI (main.yml), installer.yml, dependencies.yml and project
  workflows, which run the real installer/test tooling, kept as-is —
  no additional code CI was needed).

- Dependabot: upstream already ships .github/dependabot.yml covering
  github-actions and pip (/.github/workflows/dependencies) — verified
  and kept exactly as-is.

- .editorconfig: upstream already ships one — kept, not added.

## v1.0.0 — Baseline (2026-10-20)

- Clean standalone baseline of ohmyzsh/ohmyzsh at upstream commit
  0650a250405af1e480b1ecf8c33bc960b9f333f5 (upstream HEAD dated
  2026-10-19; upstream default branch master, this edition uses main).

- Fork history severed; all 1185 files and the licences preserved as-is
  (root LICENSE.txt is MIT; bundled plugins carry their own licence
  files under plugins/*/LICENSE).

- Notes: 9 upstream symlinks preserved as symlinks (plugin/theme links,
  incl. themes/macovsky-ruby.zsh-theme -> macovsky.zsh-theme and the
  zsh-syntax-highlighting highlighter README links) — a connector
  snapshot push cannot carry symlinks.

- 5 tracked files ignored by upstream's own .gitignore (cache/.gitkeep,
  log/.gitkeep, custom/example.zsh, custom/plugins/example/,
  custom/themes/example.zsh-theme) were force-added so this baseline
  matches the upstream tree file-for-file.

- Binaries >1 MB: plugins/zsh-interactive-cd/demo.gif (1497944 bytes)
  and plugins/z/img/demo.gif (1271520 bytes), plus 21 smaller plugin
  images — a connector snapshot push cannot carry binaries.
