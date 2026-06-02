# AGENTS.md — dotfiles

## What this is

Personal dotfiles managed via [GNU Stow](https://www.gnu.org/software/stow/).
Contents: `.zshrc` (Oh My Zsh + NVM + Bun), `.config/zed/settings.json`, and `.config/ghostty/config.ghostty` with shaders.

## Commands

```sh
stow .           # symlink everything into $HOME
stow -D .        # remove symlinks
```

Stow ignores: `.DS_Store`, `.git`, `.gitignore`, `.luarc.json`, `README.md`, `LICENSE` (see `.stow-local-ignore`).

## Notes

- No build, test, lint, or CI — plain config files only.
- `.zshrc` sources `$HOME/.local/bin/env` and adds OpenCode + Bun to `$PATH`.
- Zed config uses Claude Sonnet 4.6 (ACP), Aura Dark theme, VSCode keymap.
