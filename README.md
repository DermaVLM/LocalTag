# 🏷️ LocalTag

**A lightweight, privacy-first bounding box annotation tool.**

Zero-install, runs entirely in your browser. All data stays on your device — nothing is sent to any server.

![LocalTag Screenshot](https://img.shields.io/badge/version-v5.0-blue) ![License](https://img.shields.io/badge/license-MIT-green) ![Platform](https://img.shields.io/badge/platform-browser-orange)

## ✨ Features

- **Zero Installation** — Just open `index.html` in any modern browser
- **Privacy-First** — All data stays local, no server, no cloud
- **Multi-Format Export** — YOLO, COCO JSON, Pascal VOC XML, CSV, raw JSON
- **Session Persistence** — Auto-saves to localStorage; resume anytime
- **EXIF Correction** — Handles rotated images from medical cameras
- **Keyboard Shortcuts** — `1-9` class select, `A/D` navigation, `⌘Z` undo, `Del` delete
- **Smart Append** — Add more images without resetting your session
- **Gallery View** — Left panel with thumbnails, filters (All/Labeled/Unlabeled)
- **Bounding Box Resize** — Drag handles to adjust annotations
- **Cross-Browser** — Chrome, Firefox, Safari, Edge

## 🚀 Quick Start

1. Download or clone this repository
2. Open `index.html` in your browser
3. Click **Open Images** or drag & drop your images
4. Draw bounding boxes, assign classes, export

```bash
# Clone
git clone https://github.com/DermaVLM/LocalTag.git

# Open
open LocalTag/index.html
```

## 📦 Export Formats

| Format | Description | Use Case |
|--------|-------------|----------|
| **YOLO** | `.txt` per image + `classes.txt` + `data.yaml` | YOLOv5/v8 training |
| **COCO** | Single JSON file, COCO detection format | COCO-compatible frameworks |
| **VOC** | XML per image, Pascal VOC format | Faster R-CNN, SSD |
| **CSV** | Spreadsheet-friendly tabular format | Data analysis, review |
| **JSON** | Structured JSON with metadata | Custom pipelines |

## ⌨️ Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `1-9` | Select class |
| `A` / `D` | Previous / Next image |
| `Del` / `Backspace` | Delete selected annotation |
| `⌘Z` / `Ctrl+Z` | Undo |
| `+` / `-` | Zoom in / out |

## 🏗️ Architecture

- **Single-file HTML/JS/CSS** — No build tools, no dependencies (except JSZip for ZIP export)
- **State Management** — Central `state` object with `localStorage` persistence
- **Export Engine** — Client-side Blob generation with JSZip for YOLO ZIP bundles

## 📄 License

MIT License — free for academic and commercial use.

## 🤝 Contributing

Built and maintained by the [DermaVLM](https://github.com/DermaVLM) research group.

Contributions, issues, and feature requests are welcome.
