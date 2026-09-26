# SudhanshOS

**A Windows-style interactive desktop portfolio for Sudhansh Arora — Senior Consultant and AI QA specialist at Xebia.**

Instead of a traditional CV page, SudhanshOS puts your résumé in Notepad, your projects in File Explorer, and your certifications in a dedicated app — all running inside a browser-based desktop environment with a Pink City (Jaipur) skyline wallpaper that switches between day and night themes.

🔗 **[sudhansh3110.github.io/SudhanshOS](https://sudhansh3110.github.io/SudhanshOS)**

---

## What's inside

| App | What it shows |
|---|---|
| **Notepad** | Full CV — experience, education, certifications |
| **File Explorer** | Project case studies (Microsoft Power Platform, Appian, Kalagato) |
| **Terminal** | Skill matrix: languages, tools, frameworks |
| **Certifications** | Claude Certified Associate · AI & ML (IIT Kanpur) · CSM |
| **Calendar** | Availability and contact |

## Features

- Windows-style window management — open, minimise, close, drag, z-order
- Right-click context menu on the desktop
- Toast notifications with slide-in / slide-out animations
- Pink City SVG skyline wallpaper — sandstone pinks in light mode, deep indigo with stars in dark mode
- Full `prefers-color-scheme` and `prefers-reduced-motion` support
- Faint test-run assertions watermark (bottom-right) as an easter egg for recruiters in QA
- Single self-contained HTML file — no build step, no dependencies

## Tech

Pure HTML + CSS + vanilla JS. No frameworks, no bundler. Ships as one file.

**Fonts:** Archivo · Instrument Sans · JetBrains Mono (Google Fonts)

## Local preview

```bash
# Any static file server works
npx serve .
# or
python -m http.server 8080
```

Then open `http://localhost:8080`.

## Structure

```
sudhansh-os-site/
├── index.html        # Entire app — markup, styles, and script in one file
└── README.md
```

> [!NOTE]
> The photo and favicon referenced in `index.html` (`../assets/`) are served from the `Portfolio_web` repo when both repos are deployed under the same GitHub account. To run fully standalone, copy `assets/` into this folder and update the paths.
