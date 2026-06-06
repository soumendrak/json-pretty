# {JSON} Pretty

![Format](https://img.shields.io/badge/json-formatter-%23f0883e?style=flat-square)
![Validate](https://img.shields.io/badge/json-validator-%233fb950?style=flat-square)
![Tree View](https://img.shields.io/badge/tree-view-%23d2a8ff?style=flat-square)
![Zero Deps](https://img.shields.io/badge/zero-dependencies-%230d1117?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-%2330363d?style=flat-square)

<p align="center">
  <img src="https://img.shields.io/badge/%7B%7D-json--pretty-%23f0883e?style=for-the-badge&logo=json&logoColor=white" alt="JSON Pretty logo">
</p>

A **polished, single-file** JSON formatter, validator, and tree-view explorer — all in one HTML page. No build step, no dependencies, deploy anywhere.

**[→ Live Demo](https://soumendrak.github.io/json-pretty)**

---

## ✨ Features

- **Format** — Pretty-prints JSON with full syntax highlighting (keys, strings, numbers, booleans, null)
- **Minify** — Compresses JSON to a single line
- **Validate** — Validates JSON syntax with detailed error messages including line & column numbers
- **Tree View** — Interactive expandable/collapsible JSON tree with clickable keys
- **Drag & Drop** — Drop `.json` files directly onto the page
- **Copy** — One-click copy of formatted output to clipboard
- **Stats** — Real-time character and line counts
- **Dark Theme** — Eye-friendly dark UI with orange accent
- **Responsive** — Works on desktop and mobile
- **Zero Dependencies** — Everything in one HTML file, no CDN, no build tools

## 🚀 Usage

Open `index.html` in any modern browser, or deploy to GitHub Pages / Netlify / any static host.

1. Paste JSON into the input textarea (or drag-and-drop a `.json` file)
2. Click **Format**, **Minify**, **Validate**, or **Tree**
3. Use **Copy** to grab the formatted output

Keyboard shortcut: <kbd>Ctrl+Enter</kbd> / <kbd>Cmd+Enter</kbd> to format.

## 🔧 Pipeline

```mermaid
flowchart LR
    A["`Raw JSON Input`"] --> B{"Parse"}
    B -- "✅ Valid" --> C["Format / Minify"]
    B -- "✅ Valid" --> D["Tree View"]
    B -- "❌ Error" --> E["Error Display<br>line + column"]
    C --> F["Syntax Highlighted Output"]
    F --> G["Copy to Clipboard"]
    D --> H["Expand / Collapse<br>Interactive Tree"]
```

## 📁 Files

```
json-pretty/
├── index.html          # Single-file application (~29 KB)
└── README.md           # This file
```

## 🎨 Syntax Highlighting

| Token    | Color    | Example            |
|----------|----------|--------------------|
| Keys     | Orange   | `"name"`           |
| Strings  | Blue     | `"hello"`          |
| Numbers  | Cyan     | `42`, `3.14`       |
| Booleans | Purple   | `true`, `false`    |
| Null     | Purple   | `null`             |

## 📄 License

Licensed under the [MIT License](LICENSE).
