# Omarchy Mocha Theme

Catppuccin Mocha theme pack for Omarchy, tuned for a soft glass/clay look with Mauve accents.

## Preview

![Omarchy Mocha preview](preview.png)

## Install

```bash
omarchy-theme-install https://github.com/gitcoder89431/omarchy-mocha-theme
omarchy-theme-set mocha
```

## What Is Included

- Hyprland: `hyprland.conf`
- Hyprlock: `hyprlock.conf`
- Waybar: `waybar.css`, `waybar-theme/config.jsonc`, `waybar-theme/style.css`
- Walker: `walker.css`
- Mako: `mako.ini`
- SwayOSD: `swayosd.css`
- Fastfetch: `fastfetch.jsonc`
- Starship: `starship.toml`
- Browser accent: `chromium.theme`
- Terminal/app themes: `alacritty.toml`, `kitty.conf`, `ghostty.conf`, `warp.yaml`, `gtk.css`, `wofi.css`, `btop.theme`, `vscode.json`, `aether.zed.json`, `vencord.theme.css`, `neovim.lua`

## Notes

- This repo is intended to be the source of truth for the `mocha` theme.
- Omarchy reads files from `~/.config/omarchy/current/theme/` after `omarchy-theme-set mocha`.
- `starship.toml` and `fastfetch.jsonc` are theme-owned and can be switched by your Omarchy `theme-set` hook.
- Chromium uses `chromium.theme` (RGB string). Current value is dark Mantle-style.

## Optional Extras

Extra reference files are in `extras/` (Catppuccin/Base16 resources and app snippets).

## Attribution and Credits

This theme is a derivative/customized setup built on top of other projects. Major credits:

- Omarchy base/theme system:
  - Omarchy project and config conventions power this theme layout and runtime behavior.
  - Project: https://omarchy.org
- Waybar base (major upstream for this theme):
  - `waybar-theme/` in this repo was adapted from HANCORE's Waybar work, especially the V4.2 direction you referenced during this build.
  - Source repo: https://github.com/HANCORE-linux/waybar-themes
- Catppuccin palette and ecosystem:
  - Core palette definitions and flavor standards come from Catppuccin.
  - Source repo: https://github.com/catppuccin/catppuccin
- Catppuccin downstream config sources used for extras/adaptations:
  - Starship: https://github.com/catppuccin/starship
  - Hyprlock: https://github.com/catppuccin/hyprlock
  - fzf: https://github.com/catppuccin/fzf
  - eza: https://github.com/catppuccin/eza
  - Helix: https://github.com/catppuccin/helix
  - Zellij: https://github.com/catppuccin/zellij
  - Zed: https://github.com/catppuccin/zed
  - Base16 mappings: https://github.com/catppuccin/base16

If any attribution is incomplete or incorrect, open an issue and it will be fixed.

## License and Third-Party Notes

- This repo contains original edits plus adapted configs from upstream projects.
- Third-party names, palettes, and derived snippets remain under their respective upstream licenses and terms.
- `backgrounds/` assets are curated wallpapers; original rights stay with their creators.

## Recommended Fonts

- Nerd Font Propo variant for prompt/icons
- DSEG (optional) for segmented clock styling

## Local Development

```bash
# Apply current repo changes
omarchy-theme-set mocha

# Re-apply browser color after changing chromium.theme
omarchy-theme-set-browser
```
