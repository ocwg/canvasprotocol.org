# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the static website for the **Open Canvas Working Group (OCWG)** at https://canvasprotocol.org. It serves as the landing page for the OCIF (Open Canvas Interchange Format) specification effort.

The OCIF specification itself lives in a sibling repository (`../spec`), hosted at https://spec.canvasprotocol.org.

## Architecture

Pure static site — no build system, no package manager, no JavaScript framework.

- `index.html` — single-page site with all content
- `style.css` — all styling, uses modern CSS nesting, responsive design, light/dark mode
- `meetings/` — ICS calendar files

## Development

Open `index.html` in a browser, or:

```
python3 -m http.server
```

No build step, no dependencies to install.

## Deployment

Deployed via GitHub Pages from the `main` branch. Commits to `main` trigger deployment automatically.

## Key External Services

- **Buttondown.email** — newsletter signup form (ocwg list)
- **Luma** — meeting scheduling links
- **Discord** — community chat (https://discord.gg/32CWVJkUts)
- **GitHub org** — https://github.com/ocwg

## Common Updates

The most frequent changes are updating meeting dates/links in `index.html` — the meetings section near the bottom of the file contains a chronological list of all past and upcoming meetings.
