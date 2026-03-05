# Horizon 222831 Themes for VS Code

Color themes for Visual Studio Code built around:

- Base: `#222831`
- Accent: `#F2F2F2`
- Highlights: `#FF6B6B`, `#FFD93D`, `#6BCB77`, `#4D96FF`

This extension includes two variants:

- `Dark 222831`
- `Light 222831`

![222831 Icon](./img/icon.png)

## Why this theme?

- High readability for long coding sessions.
- Better token separation for real-world code (`const/let/var`, `function`, `return`, properties, parameters).
- Semantic highlighting enabled for smarter color mapping by language.
- Balanced UI contrast: clean panels, visible tabs, non-distracting borders.

## Palette

| Token | Hex |
|---|---|
| Base background | `#222831` |
| Base foreground | `#F2F2F2` |
| Red | `#FF6B6B` |
| Yellow | `#FFD93D` |
| Green | `#6BCB77` |
| Blue | `#4D96FF` |
| Purple | `#BB8ED0` |
| Cyan | `#ABDADC` |
| Orange | `#FAAC68` |
| Muted | `#BFC9D1` |
| Border | `#44444E` |

## Install (Local Development)

1. Open this project in VS Code.
2. Press `F5` to run the extension host.
3. In the new window, open Command Palette:
   - `Preferences: Color Theme`
4. Select:
   - `Dark 222831` or
   - `Light 222831`

## Install from VSIX

1. Package the extension:

   ```bash
   vsce package
   ```

2. In VS Code:
   - `Extensions: Install from VSIX...`
3. Select the generated `.vsix`.

## Recommended font setup (MonoLisa)

For best visual balance with this theme:

```json
{
  "editor.fontFamily": "MonoLisa, Menlo, Monaco, 'Courier New', monospace",
  "editor.fontLigatures": true,
  "editor.semanticHighlighting.enabled": true,
  "editor.lineHeight": 1.55
}
```

## Project structure

```text
.
├── icon.png
├── package.json
└── themes
    ├── dark-222831-color-theme.json
    └── light-222831-color-theme.json
```

## Notes

- If theme changes do not appear immediately, run `Developer: Reload Window`.
- If using VSIX, repackage and reinstall after each change.
