# Reader's Guide — ohmyzsh (Oh My Zsh)

## What this project is

**Oh My Zsh** is the community-driven **framework for managing your Zsh
configuration**. Instead of hand-writing a fragile `.zshrc`, you install the
framework, pick a theme, enable the plugins you want, and get a polished,
productive shell — prompts with git status, hundreds of aliases and helper
functions, completions and sensible defaults — maintained by thousands of
contributors.

## How the content is organised

- `oh-my-zsh.sh` — the entry point your `.zshrc` sources; it loads everything
  else in the right order.
- `lib/` — the core library (22 files): the framework's own functions,
  completion setup, key bindings, prompt plumbing and defaults.
- `plugins/` — **372 bundled plugins**, one folder each, adding aliases,
  completions and integrations for tools and platforms (git tooling, package
  managers, cloud CLIs, languages, and much more). You enable them by name.
- `themes/` — **143 prompt themes**, one `.zsh-theme` file each (the README
  links the theme gallery; `agnoster` is the classic example).
- `templates/` — the starter `zshrc` template the installer copies to
  `~/.zshrc`.
- `tools/` — the install/upgrade helper scripts.
- `custom/` — where *your* own plugins, themes and overrides live, kept
  separate so framework updates never clobber them.
- [`README.md`](README.md) — the manual: **Getting Started** (OS
  compatibility, prerequisites, basic installation), **Using Oh My Zsh**
  (enabling and using plugins, selecting themes, FAQ), and **Advanced
  Topics** (custom directory, unattended/manual installs, custom plugins and
  themes, troubleshooting).

## How to use it

1. Install per the README's Basic Installation (or the manual steps under
   Advanced Topics), which clones the framework and creates your `.zshrc`
   from `templates/`.
2. Edit `~/.zshrc`: set `ZSH_THEME` to a theme from `themes/`, and add plugin
   names to the `plugins=(...)` list.
3. Open a new shell — and put personal extras in `custom/` so upgrades stay
   painless.

## About this standalone edition

This repository is a standalone edition of
[ohmyzsh/ohmyzsh](https://github.com/ohmyzsh/ohmyzsh), converted from a fork
into its own repository and enhanced in place. See
[`ENHANCEMENTS.md`](ENHANCEMENTS.md) for what this edition adds and
[`CHANGELOG.md`](CHANGELOG.md) for its version history (v1.0.0 upstream
baseline, v1.1.0 enhancements). All original work belongs to the Oh My Zsh
community and the upstream contributors; licence MIT (see `LICENSE.txt`).
