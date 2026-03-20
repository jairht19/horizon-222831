# Horizon 222831 Theme UI Notes

## Goal

Backlog of improvements for colors, UI coverage, and visual consistency in the `Horizon 222831` VS Code theme.

## Current direction

The theme already has a solid base palette and better workbench coverage than the initial version, but it can still improve in three areas:

- stronger UI completeness
- more consistent semantic color rules
- better support for real-world editing flows beyond JS and TS

## Priority improvements

### 1. Diagnostics and state colors

Improve visual hierarchy for:

- `error`
- `warning`
- `info`
- `hint`

Areas to review:

- editor markers
- Problems panel
- peek references
- overview ruler
- minimap diagnostics

Desired outcome:

- clearer severity separation
- softer backgrounds with readable foreground accents
- consistent state language across dark and light variants

### 2. Diff and Git colors

Expand support for:

- `diffEditor.insertedTextBackground`
- `diffEditor.removedTextBackground`
- `diffEditor.insertedLineBackground`
- `diffEditor.removedLineBackground`
- `gitDecoration.renamedResourceForeground`
- `gitDecoration.untrackedResourceForeground`
- `gitDecoration.ignoredResourceForeground`
- merge conflict colors

Desired outcome:

- git state is easier to scan
- diffs feel integrated with the theme instead of partially default
- added/removed/modified states are more legible in editor and explorer

### 3. Terminal palette refinement

Review ANSI terminal colors for:

- shell prompts
- logs
- test output
- CLI tools with bright variants

Focus especially on:

- red contrast
- yellow readability
- blue clarity on dark backgrounds

Desired outcome:

- terminal feels first-class, not secondary
- logs are readable without harsh saturation

### 4. Search and match highlighting

Review contrast and differentiation for:

- `findMatch`
- `findMatchHighlight`
- `selectionHighlight`
- `wordHighlight`
- `wordHighlightStrong`
- `rangeHighlight`

Desired outcome:

- active search hit is unmistakable
- passive highlights do not compete with selections
- highlight language feels intentional, not flat

### 5. Tabs and editor groups

Refine identity for:

- active tabs
- inactive tabs
- hover tabs
- unfocused tabs
- dirty states
- split editor groups

Suggested keys to review:

- `tab.unfocusedInactiveForeground`
- `tab.unfocusedInactiveBackground`
- `tab.lastPinnedBorder`
- `editorGroupHeader.noTabsBackground`
- `editorGroup.dropBackground`

Desired outcome:

- active file is easier to identify
- split editors feel more structured
- tab bar has stronger hierarchy without becoming noisy

### 6. Explorer and list behavior

Improve list and tree behavior for:

- hover
- active selection
- inactive selection
- focused selection
- filter states
- indentation guides

Suggested keys to review:

- `list.inactiveSelectionBackground`
- `list.inactiveSelectionForeground`
- `list.focusAndSelectionOutline`
- `listFilterWidget.background`
- `listFilterWidget.outline`
- `tree.indentGuidesStroke`

Desired outcome:

- explorer feels more polished
- selected items remain clear when focus changes

### 7. Minimap and overview ruler

Review how these surfaces display:

- search hits
- diagnostics
- git changes
- modified regions

Desired outcome:

- useful signal at a glance
- less visual clutter
- stronger consistency with editor gutters

### 8. Special panels and workbench areas

Add or refine support for:

- `settings.*`
- `welcomePage.*`
- `debugToolBar.*`
- `editorMarkerNavigation.*`
- `merge.*`
- `testing.*`

Desired outcome:

- the theme feels complete in more workflows
- fewer fallback/default VS Code colors appear

### 9. Markdown and prose experience

Improve readability for documentation-heavy work:

- headings
- links
- blockquotes
- inline code
- code fences
- bullets and lists

Desired outcome:

- README files look deliberate
- prose and code blocks feel distinct but cohesive

### 10. Better language coverage

The theme is already strongest in JS and TS. Next languages and syntaxes to refine:

- HTML
- CSS
- JSON
- Markdown

Important distinctions to preserve:

- tags vs attributes
- CSS properties vs values
- JSON keys vs string values
- Markdown headings vs inline code vs links

Desired outcome:

- more predictable behavior across common frontend workflows

### 11. Strict semantic palette rules

Define and preserve a stable semantic system such as:

- declarations: orange
- control flow: coral
- functions: blue
- types: purple
- properties: cyan
- strings: green
- numbers: yellow

Desired outcome:

- users learn the theme quickly
- symbols keep similar meaning across languages
- semantic tokens and TextMate tokens stay aligned

### 12. Additional variants

Potential product expansion:

- `Horizon 222831 Dark Soft`
- `Horizon 222831 Dark High Contrast`
- `Horizon 222831 Light Soft`

Desired outcome:

- broader appeal without losing core identity
- easier choice for users who prefer softer or stronger contrast

## Suggested next iteration

Recommended implementation order:

1. Improve diagnostics, diff, Git, and search highlighting.
2. Refine HTML, CSS, JSON, and Markdown token coverage.
3. Add one extra variant such as `Soft` or `High Contrast`.

## Publishing notes

Before publishing to the Marketplace:

- add screenshots of real code samples
- show both dark and light variants
- include examples from TS, JSON, Markdown, and terminal views

This will communicate the theme better than palette tables alone.
