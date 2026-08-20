<div align="center">

<img src="docs/logo.png" width="118" alt="MD Viewer" />

# MD Viewer

**A Windows Markdown reader for local technical documentation**

Long-form reading · Tabbed workspaces · 25+ diagram types · Chinese and English UI

[![Latest release](https://img.shields.io/github/v/release/zeronchen/md-viewer?style=flat-square&label=version)](https://github.com/zeronchen/md-viewer/releases/latest)
![Windows](https://img.shields.io/badge/Windows-10%20%7C%2011-0078d4?style=flat-square)
![License](https://img.shields.io/badge/license-commercial-orange?style=flat-square)
![Auto update](https://img.shields.io/badge/auto%20update-supported-2da44e?style=flat-square)

[Download](https://github.com/zeronchen/md-viewer/releases/latest) · [中文](README.md) · [Release notes](https://github.com/zeronchen/md-viewer/releases)

</div>

---

![MD Viewer main window](docs/screenshot-main.png)

## What MD Viewer does

MD Viewer is built for Windows users who regularly read API documentation, design notes, code analysis, and Mermaid-heavy documents. Files stay on the local machine. Tabs, the folder tree, and the outline make large document sets easier to navigate, while complex diagrams can be opened in a dedicated fullscreen viewer.

| Capability | Details |
|---|---|
| **Markdown reading** | GFM, footnotes, task lists, KaTeX math, code highlighting, in-document tables of contents, and find-in-page |
| **Tabbed workspace** | DOM caching reduces repeated rendering; session restore, tab switching, folder-tree following, and `Ctrl+P` quick open are included |
| **25+ diagram types** | 20 Mermaid types rendered locally, plus PlantUML, D2, Graphviz, Vega-Lite, and WaveDrom |
| **Stable fullscreen zoom** | The viewer keeps the same SVG while zooming. Mermaid does not re-layout after zoom settles, so text wrapping, node positions, and connections stay fixed |
| **Diagram controls** | Wheel and double-click zoom, drag to pan, fit, 100% view, text selection, ELK / dagre layout switching, and four flowchart directions |
| **Source viewing and conversion** | Switch the whole document to source mode, or edit Mermaid source in the preview and render it again with `Ctrl+Enter` |
| **Chinese and English UI** | Follow the system language or select 中文 / English; menus, dialogs, messages, dates, and license states update together |
| **Reading typography** | Adjustable width, font size, and code themes; the font menu shows only supported fonts installed on the machine |
| **Export** | Documents to PDF and self-contained HTML; diagrams to SVG, 2× PNG, and `.mmd` source |
| **Automatic updates** | Stable and beta channels, startup checks, automatic downloads, progress details, one retry after failure, and per-version skipping |

## Diagram support

| Type | Rendered by | Fence language |
|---|---|---|
| Flowchart, sequence, Gantt, class, state, ER, pie, mind map, timeline, Git, C4, Sankey, radar, and more | Local Mermaid | `mermaid` |
| PlantUML | plantuml.com | `plantuml` |
| D2 | kroki.io | `d2` |
| Graphviz / DOT | kroki.io | `dot` or `graphviz` |
| Vega-Lite | kroki.io | `vega-lite` |
| WaveDrom | kroki.io | `wavedrom` |

Mermaid is rendered locally. Other diagram types are controlled by the Online Lookup setting and ask before connecting by default. When allowed, only that diagram's source is sent; the rest of the document stays local. Returned SVG is sanitized before display.

## Install and update

1. Open the [latest release](https://github.com/zeronchen/md-viewer/releases/latest)
2. Download `MD-Viewer-Setup-1.6.0.exe`
3. Follow the installer

The current release channel provides the Windows installer only. After installation, MD Viewer is available in Open with for `.md`, `.markdown`, `.mdown`, and `.mkd` files.

The installed edition checks GitHub Releases according to your settings. When an update is available, you can review it, download it, and restart to install from inside the app.

## Privacy and security

- Markdown, images, code highlighting, KaTeX, and Mermaid are processed locally by default
- PlantUML and Kroki receive diagram source only after network access is allowed
- Update checks access GitHub Releases, and downloaded files are used only for software updates
- Markdown content and remote SVG are sanitized before entering the interface
- Electron sandboxing, sender validation, navigation restrictions, and asar integrity protection are enabled

## Trial and license

- A 14-day full-feature trial starts on first use
- License files use offline Ed25519 signatures and are machine-bound
- Open Help → License, copy the machine ID, and import the issued license file to activate
- Moving to another machine requires a re-issued license based on purchase information

## Keyboard shortcuts

| Shortcut | Action | Shortcut | Action |
|---|---|---|---|
| `Ctrl + O` | Open file | `Ctrl + Shift + O` | Open folder |
| `Ctrl + P` | Quick open | `Ctrl + F` | Find in page |
| `Ctrl + Tab` | Next tab | `Ctrl + Shift + Tab` | Previous tab |
| `Ctrl + W` | Close tab | `Ctrl + B` | Toggle sidebar |
| `Ctrl + /` | Source mode | `Ctrl + Shift + D` | Toggle light / dark |
| `Ctrl + Shift + P` | Export PDF | `Ctrl + E` | Export HTML |
| `Ctrl + Shift + L` | License | `Ctrl + Shift + U` | Check for updates |

## Requirements

- 64-bit Windows 10 or Windows 11
- 500 MB of available disk space recommended
- No separate Node.js, Java, or browser runtime required
- Offline reading works without a connection; online diagrams and updates require network access

---

<div align="center">

© 2026 MD Viewer · Commercially licensed software

</div>
