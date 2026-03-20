# Horizon 222831 Theme for VS Code

Horizon 222831 is a paired dark/light theme set for Visual Studio Code built around the `#222831` palette. It aims for strong code readability, cleaner semantic grouping, and a workbench that feels cohesive instead of overly decorated.

This extension includes:

- `Horizon 222831 Dark`
- `Horizon 222831 Light`

![222831 Icon](./img/icon.png)

## Design goals

- Clear token separation for everyday coding: declarations, flow keywords, functions, parameters, properties, and types.
- Consistent semantic and TextMate token behavior to reduce color drift across languages.
- Balanced UI contrast across tabs, panels, terminal, minimap, breadcrumbs, peek views, and notifications.
- Low-noise editor chrome with enough emphasis for focus states and diagnostics.

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
2. Press `F5` to launch an Extension Development Host.
3. Open `Preferences: Color Theme`.
4. Select `Horizon 222831 Dark` or `Horizon 222831 Light`.

## Install from VSIX

1. Run:

   ```bash
   vsce package
   ```

2. In VS Code, run `Extensions: Install from VSIX...`.
3. Choose the generated `.vsix` file.

## Recommended editor settings

```json
{
  "editor.fontFamily": "MonoLisa, Menlo, Monaco, 'Courier New', monospace",
  "editor.fontLigatures": true,
  "editor.semanticHighlighting.enabled": true,
  "editor.lineHeight": 1.55
}
```

## Notes

- If changes do not appear immediately, run `Developer: Reload Window`.
- After updating the extension, repackage and reinstall the VSIX.
- Add screenshots of real code samples before publishing to the Marketplace. Theme pages convert much better with previews than with palette tables alone.
