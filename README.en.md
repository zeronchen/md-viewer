<div align="center">

<img src="docs/logo.png" width="118" alt="MD Viewer" />

# MD Viewer

**A Windows Markdown reader for local technical documentation**

Long-form reading · Tabbed workspaces · 25+ diagram types · Account licensing · Chinese and English UI

[![Latest release](https://img.shields.io/github/v/release/zeronchen/md-viewer?style=flat-square&label=version)](https://github.com/zeronchen/md-viewer/releases/latest)
![Windows](https://img.shields.io/badge/Windows-10%20%7C%2011-0078d4?style=flat-square)
![License](https://img.shields.io/badge/license-commercial-orange?style=flat-square)
![Auto update](https://img.shields.io/badge/auto%20update-supported-2da44e?style=flat-square)

[Download](https://github.com/zeronchen/md-viewer/releases/latest) · [中文](README.md) · [Release notes](https://github.com/zeronchen/md-viewer/releases)

</div>

---

![MD Viewer main window](docs/screenshot-main.png)

## What MD Viewer does

MD Viewer is built for Windows users who read API docs, design specs, code analyses and Mermaid diagram collections. Files stay on your machine; move fast between tabs, the file tree and the outline, and take complex diagrams fullscreen.

| Capability | Details |
|---|---|
| **Account licensing** | Sign in with email to unlock: 3 devices per account, 14-day offline grace; manage devices, change and recover passwords in-app |
| **Markdown reading** | GFM, footnotes, task lists, KaTeX math, syntax highlighting, in-document TOC and search |
| **Cross-file search** | `Ctrl+Shift+F` searches every Markdown file in the folder — results grouped by file with line numbers and context; case-sensitive / whole-word / regex modes; click to jump and highlight |
| **Tabbed workspace** | DOM caching avoids re-rendering; session restore, tab switching, tree follow and `Ctrl+P` quick open |
| **Zen mode** | `F11` for immersive reading: adaptive measure, focus dimming, progress bar and outline overlay |
| **25+ diagram types** | 20 Mermaid types rendered locally, plus PlantUML, D2, Graphviz, Vega-Lite and WaveDrom |
| **Stable fullscreen zoom** | The fullscreen preview always zooms one single SVG — continuous zoom never re-layouts Mermaid, so line wrapping, node positions and edges stay put |
| **Diagram interaction** | Wheel and double-click zoom, drag pan, fit-to-window, 100%, text selection, ELK / dagre layout toggle, four-way direction switch |
| **Source view & convert** | Toggle the whole document to source; edit Mermaid source in the preview layer and regenerate with `Ctrl+Enter` |
| **Bilingual UI** | Follow-system, Chinese or English — menus, dialogs, toasts, dates and license states switch together |
| **Reading typography** | Adjustable measure, font size and code theme; the font menu only lists fonts actually installed |
| **Export** | PDF and single-file HTML for documents; SVG, 2× PNG and `.mmd` source for diagrams |
| **Auto update** | Stable and beta channels, startup check, auto download, progress, retry and skip-version |

## Licensing (since v2.0)

**Trial**: 14 days of full functionality on first use — no sign-up needed.

**Account license (recommended)**: purchased accounts sign in with email and a password you set.

- Up to **3 devices** per account; a 4th sign-in shows a device-list guide
- Self-service in the app: unbind old devices (password confirm, once per 30 days), change password
- Password recovery via email link — without revealing whether an account exists
- **Works offline**: two weeks of full functionality without network; multi-anchor state makes tampering with config useless at extending the grace period

**Certificate license (legacy-compatible)**: existing `license.key` files remain valid. You can also tap **"Convert to account license"** in Help → License to migrate your certificate into an account (online, one click), then just sign in anywhere.

> Purchase & provisioning: [TBD: contact / channel]

## Diagram support

| Type | Rendered by | Code fence |
|---|---|---|
| Flowchart, sequence, gantt, class, state, ER, pie, mindmap, timeline, git graph, C4, sankey, radar, etc. | Local Mermaid | `mermaid` |
| PlantUML | plantuml.com | `plantuml` |
| D2 | kroki.io | `d2` |
| Graphviz / DOT | kroki.io | `dot` or `graphviz` |
| Vega-Lite | kroki.io | `vega-lite` |
| WaveDrom | kroki.io | `wavedrom` |

Mermaid renders on your machine. Online diagrams are gated by the "online diagrams" setting — asked first by default; when allowed, only the diagram source is sent, never the rest of the document. Returned SVGs are sanitized before display.

## Install & update

1. Open [Releases](https://github.com/zeronchen/md-viewer/releases/latest)
2. Download `MD-Viewer-Setup-2.0.0.exe` (installer) or `MD-Viewer-Folder-2.0.0.zip` (portable, unzip and run)
3. Follow the installer; SHA256 checksums are in the release notes

After installing, use "Open with" to open `.md`, `.markdown`, `.mdown` and `.mkd` files with MD Viewer.

The installer checks GitHub Releases per your settings: see what's new in-app, download, and restart to install — any older version upgrades to the latest in one step.

## Privacy & security

- Markdown, images, syntax highlighting, KaTeX and Mermaid are processed locally by default
- Account licensing only exchanges credentials, heartbeats and device identifiers with the license server — **document content never leaves your machine**
- PlantUML and Kroki diagrams send their source only after you grant network permission
- Update checks reach GitHub Releases only, and downloads are used solely for the update
- Markdown content and remote SVGs are sanitized before entering the UI
- Electron sandbox, origin validation, navigation restrictions and asar integrity protection are enabled

## Keyboard shortcuts

| Key | Action | Key | Action |
|---|---|---|---|
| `Ctrl + O` | Open file | `Ctrl + Shift + O` | Open folder |
| `Ctrl + P` | Quick open | `Ctrl + F` | Find in document |
| `Ctrl + Shift + F` | Cross-file search | `F3` / `Shift + F3` | Next / previous match |
| `Ctrl + Tab` | Next tab | `Ctrl + Shift + Tab` | Previous tab |
| `Ctrl + W` | Close tab | `Ctrl + B` | Toggle sidebar |
| `Ctrl + /` | Source mode | `Ctrl + Shift + D` | Toggle theme |
| `F11` | Zen mode | `Ctrl + Shift + L` | License / account |
| `Ctrl + Shift + P` | Export PDF | `Ctrl + E` | Export HTML |
| `Ctrl + Shift + U` | Check updates | | |

> The cross-file search panel can also be summoned by scrolling up at the top of the file tree / outline; dismiss with a downward scroll or `Esc` when the query is empty.

## System requirements

- Windows 10 or 11, 64-bit
- ~500 MB of free disk space recommended
- No Node.js, Java or browser runtime required
- Offline reading works out of the box (account licensing keeps a 14-day offline grace); online diagrams and auto update need network

---

<div align="center">

© 2026 MD Viewer · Commercially licensed software

</div>
