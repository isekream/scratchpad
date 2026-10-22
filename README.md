# Scratchpad

A lightweight, single-file note collector for long Claude Code sessions.

Collect points from Claude’s answers, group them (questions, to-dos, concerns, plain notes), reorder them, and copy them back in the format you need. Optionally connect to your local `.claude` folder so notes stay tied to individual sessions.

## Features

- **Notes view** — add, select, multi-select, drag-reorder, inline-edit, mark as copied, undo deletes
- **Claude’s answer view** — splits the latest (or previous) assistant reply into clickable blocks; click to turn them into notes
- **Session integration** — connect once to your `.claude` folder (File System Access API); follows the active Claude Code session or lets you pin one; stores notes in `.claude/scratchpad/`
- **Copy formats** — one line, bullets, numbered list, or Markdown (with optional intro line and grouping by type)
- **Polish** — light/dark theme, presentation mode, keyboard shortcuts, toasts

## Usage

1. Open `scratchpad.html` in a modern browser (Chrome, Edge, or any browser with File System Access API support for the optional session feature).
2. Type notes in the composer, or switch to the “Claude’s answer” tab after connecting a folder.
3. Select notes and copy them in your preferred format.
4. (Optional) Click “Connect” and pick your `.claude` folder to enable per-session persistence and the answer parser.

Notes fall back to `localStorage` when no folder is connected.

## Requirements

- Modern browser
- Optional: local Claude Code installation with a `.claude` folder (for session features)

## License

MIT — see [LICENSE](LICENSE).
