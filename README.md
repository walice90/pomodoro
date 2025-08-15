# Tomato Clock (Pomodoro) — Notion-ready widget

A minimal, self-contained Pomodoro timer you can embed in Notion using `/embed`.

## Quick start
1) Publish this folder with **GitHub Pages**, **Vercel**, or **Netlify**.
2) Copy the public URL (ending in `/` or `/index.html`).
3) In Notion, type `/embed`, paste the URL, and resize as you like.

## Customization via URL params
You can tweak behavior via query params appended to the URL:

- `focus` — focus minutes (default 25)
- `short` — short break minutes (default 5)
- `long`  — long break minutes (default 15)
- `rounds` — number of focus sessions before a long break (default 4)
- `auto` — `1` or `0` to auto-start next session (default 0)
- `theme` — `light`, `dark`, or `auto` (default `auto`)
- `accent` — hex color like `%23ff5a54` (URL-encoded `#`), or any valid CSS color
- `sound` — `ding` or `off` (default `ding`)
- `title` — sets the page title (shows in the browser/tab)

**Example:**

```
https://your-domain/tomato-clock/?focus=50&short=10&long=20&rounds=4&auto=1&theme=dark&accent=%23ff5a54&title=Deep%20Work
```

## Keyboard shortcuts
- **Space** — start/pause
- **R** — reset
- **S** — skip

## Notes
- Sound will play only after first user interaction (browser policy).
- State persists per browser via `localStorage`.
- The file is fully self-contained (no external assets or frameworks).
