# streamtype

A minimal stream-of-consciousness writing app. Only the word you're typing is shown — once you hit space, it disappears. Keeps you moving forward instead of editing what's already there.

Single HTML file. No build step. Works offline. Hostable on GitHub Pages.

## Use it

Live: https://lvdagilis.github.io/streamtype

Or just download [`index.html`](index.html) and open it in any browser.

## Features

- **Word-at-a-time display** — your current word is the only thing visible, then fades on space/enter
- **Sentence mode** — optional dim line above the word showing the sentence you're building
- **Backspace recovery** — erase the current word, then keep going back to bring previous words back
- **Peek mode** — hold the peek button (or `Tab`) to reveal the full text rendered as markdown
- **Markdown support** — headings, bold, italic, with live preview in peek
- **Writing goals** — word targets (250 / 500 / 750 — the last is roughly Julia Cameron's three morning pages) or timed sessions (5–30 min)
- **Save as `.md`** — with timestamp, optional geolocation, and optional tags in YAML frontmatter
- **Adjustable font size** — small for working in public, large for distraction-free home use

## Keyboard shortcuts

| Key | Action |
| --- | --- |
| `Space` / `Enter` | commit word / new line |
| `Backspace` | erase character, or recover previous word |
| `Tab` (hold) | peek at the full document |
| `Cmd`/`Ctrl` + `1` / `2` / `3` | heading 1 / 2 / 3 |
| `Cmd`/`Ctrl` + `B` | toggle **bold** |
| `Cmd`/`Ctrl` + `I` | toggle *italic* |
| `Cmd`/`Ctrl` + `S` | open save dialog |

## Saved file format

```yaml
---
created: 2026-05-17T09:42:11.000Z
location: 54.68916, 25.27975
tags: [morning-pages, train]
---

your words here…
```

Location is only included if you grant permission when saving. Tags are optional.
