# Omarchy Mocha Extras (Catppuccin Sources)

These are optional integrations from Catppuccin upstream repositories.

## Included

- `fzf/catppuccin-fzf-mocha.sh`
- `eza/catppuccin-mocha-mauve.yml` (Mocha flavor, Mauve accent)
- `helix/themes/catppuccin_mocha.toml`
- `zellij/catppuccin.kdl`
- `zed/catppuccin-mauve.json`
- `hypr/mocha.conf` (Catppuccin Hyprland variables)
- `hypr/hyprlock-catppuccin.conf` (Catppuccin Hyprlock example)
- `base16/catppuccin-mocha.yaml`

## Source Attribution (Per Extras File)

All extras are adapted/copied from Catppuccin-maintained repositories and retain upstream credit.

- `fzf/catppuccin-fzf-mocha.sh`
  - Source: https://github.com/catppuccin/fzf
- `eza/catppuccin-mocha-mauve.yml`
  - Source: https://github.com/catppuccin/eza
- `helix/themes/catppuccin_mocha.toml`
  - Source: https://github.com/catppuccin/helix
- `zellij/catppuccin.kdl`
  - Source: https://github.com/catppuccin/zellij
- `zed/catppuccin-mauve.json`
  - Source: https://github.com/catppuccin/zed
- `hypr/mocha.conf`
  - Source: https://github.com/catppuccin/catppuccin (palette values)
- `hypr/hyprlock-catppuccin.conf`
  - Source: https://github.com/catppuccin/hyprlock
- `base16/catppuccin-mocha.yaml`
  - Source: https://github.com/catppuccin/base16

Palette authority:
- https://github.com/catppuccin/catppuccin

## Quick Apply

```bash
# fzf (Bash/Zsh)
grep -qxF 'source ~/.config/fzf/catppuccin-fzf-mocha.sh' ~/.bashrc || echo 'source ~/.config/fzf/catppuccin-fzf-mocha.sh' >> ~/.bashrc
mkdir -p ~/.config/fzf
cp extras/fzf/catppuccin-fzf-mocha.sh ~/.config/fzf/catppuccin-fzf-mocha.sh

# eza
mkdir -p ~/.config/eza
cp extras/eza/catppuccin-mocha-mauve.yml ~/.config/eza/theme.yml

# helix
mkdir -p ~/.config/helix/themes
cp extras/helix/themes/catppuccin_mocha.toml ~/.config/helix/themes/
# set in ~/.config/helix/config.toml: theme = "catppuccin_mocha"

# zellij
mkdir -p ~/.config/zellij/themes
cp extras/zellij/catppuccin.kdl ~/.config/zellij/themes/
# set in ~/.config/zellij/config.kdl: theme "catppuccin-mocha"

# zed
mkdir -p ~/.config/zed/themes
cp extras/zed/catppuccin-mauve.json ~/.config/zed/themes/
# then choose "Catppuccin Mocha" in Zed

# hyprlock sample (optional)
cp extras/hypr/mocha.conf ~/.config/hypr/mocha.conf
cp extras/hypr/hyprlock-catppuccin.conf ~/.config/hypr/hyprlock.conf
```

## Notes

- `vscode.json` at repo root is set to `Catppuccin Mocha` with extension `catppuccin.catppuccin-vsc`.
- Omarchy only auto-manages VSCode/Codium/Cursor via `vscode.json`.
- Zed/Helix/Zellij/fzf/eza are optional manual extras unless you wire them in a theme hook.
