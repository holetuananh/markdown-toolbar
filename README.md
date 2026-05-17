# Markdown Toolbar & Shortcuts

Markdown Toolbar & Shortcuts is a VS Code extension that adds a formatting toolbar, keyboard shortcuts, and utilities for Markdown files.

## Features

- **Toolbar buttons** in the editor title bar (visible only for `.md` files)
- **Editor context menu** entries for `Bold`, `Italic`, and `Link`
- **Keyboard shortcuts** with direct shortcuts for `Bold`, `Italic`, and `Link`, plus `Ctrl+M` chord sequences for the full command set
- **Toggle behavior**: applying a format to already-formatted text removes it
- **Line-based commands**: headings, quotes, and lists apply to every selected line
- **Multi-cursor support** for inline formatting
- **Section number updater**: auto-numbers H1–H3 headings hierarchically

## Keyboard Shortcuts

All shortcuts only activate when editing a Markdown file.

### Direct Shortcuts

| Shortcut | Command |
|---|---|
| `Ctrl+B` | Bold |
| `Ctrl+I` | Italic |
| `Ctrl+K` | Link |

### `Ctrl+M` Chords

| Shortcut | Command |
|---|---|
| `Ctrl+M Ctrl+B` | Bold |
| `Ctrl+M Ctrl+I` | Italic |
| `Ctrl+M Ctrl+C` | Inline Code |
| `Ctrl+M Ctrl+S` | Strikethrough |
| `Ctrl+M Ctrl+1` | Heading 1 |
| `Ctrl+M Ctrl+2` | Heading 2 |
| `Ctrl+M Ctrl+3` | Heading 3 |
| `Ctrl+M Ctrl+Q` | Quote |
| `Ctrl+M Ctrl+U` | Unordered List |
| `Ctrl+M Ctrl+O` | Ordered List |
| `Ctrl+M Ctrl+X` | Task List (Unchecked) |
| `Ctrl+M Ctrl+Shift+X` | Task List (Checked) |
| `Ctrl+M Ctrl+L` | Link |
| `Ctrl+M Ctrl+G` | Image |
| `Ctrl+M Ctrl+M` | Inline Math |
| `Ctrl+M Ctrl+Shift+M` | Block Math |
| `Ctrl+M Ctrl+K` | Code Block |
| `Ctrl+M Ctrl+T` | Table |
| `Ctrl+M Ctrl+H` | Horizontal Rule |
| `Ctrl+M Ctrl+N` | Update Section Numbers |
| `Ctrl+M Ctrl+P` | Preview to Side |

## Behavior

- **Selection present**: wraps or transforms the selected text; applying again toggles it off
- **No selection**: inserts a placeholder with the cursor/tab stop positioned for immediate typing
- **Line commands** (headings, quote, lists): apply to every line touched by the selection
- **Link/Image with multi-line selections**: converts each non-empty line separately
- **Code Block / Block Math with a selection**: wraps the selection in fenced blocks
- **Table / Horizontal Rule**: inserts at the cursor and starts on a new line if the current line already has content

## Development

```bash
npm install
npm run compile   # one-time build
npm run watch     # rebuild on save
```

Press `F5` in VS Code to launch the Extension Development Host for testing.
