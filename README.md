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
