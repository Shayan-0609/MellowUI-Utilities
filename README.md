# MellowUI-Utilities v1.3.1

[![npm version](https://img.shields.io/npm/v/mellowui-utilities?style=flat&color=007bec)](https://www.npmjs.com/package/mellowui-utilities)
[![npm downloads](https://img.shields.io/npm/dw/mellowui-utilities?style=flat&color=28a745)](https://www.npmjs.com/package/mellowui-utilities)
[![minified size](https://img.shields.io/bundlephobia/min/mellowui-utilities?style=flat&color=4154f1)](https://bundlephobia.com/package/mellowui-utilities)
[![bundle size](https://img.shields.io/bundlephobia/minzip/mellowui-utilities?style=flat&color=6f42c1)](https://bundlephobia.com/package/mellowui-utilities)
[![GitHub license](https://img.shields.io/github/license/Shayan-0609/MellowUI-Utilities?style=flat&color=orange)](LICENSE)

A lightweight, high-performance, and Responsive Utility-First CSS Framework Engine built for fast component composition. It bridges the structural power of Bootstrap 5.3+ grid architecture with the atomic agility of Tailwind CSS, enhanced with soft premium Mellow Shadows.

## ✨ Features

- **Atomic Philosophy:** Pure utility-first utility classes (`d-flex`, `gap-*`, `border-*`, `rounded-*`) without bloated pre-made UI components.
- **Premium Grid Layout (Upgraded ✨):** Reliable, pixel-perfect Bootstrap 5.3+ architecture (`row`, `col-1` to `col-12`, `g-*`) now upgraded with a premium **`1.75rem` gutter spacing** for more spacious and breathy professional layouts.
- **Tailwind-style Atomic Color Classes (New 🚀):** Direct styling power with native utility classes for all 11 core colors across 100-900 shading scales. Use them instantly without configuration:
  - `text-{color}-{shade}` (e.g., `.text-blue-600`, `.text-slate-900`)
  - `bg-{color}-{shade}` (e.g., `.bg-emerald-500`, `.bg-zinc-100`)
  - `border-{color}-{shade}` (e.g., `.border-indigo-300`, `.border-red-500`)
- **Flexible CSS Variables:** All 11-color palette tokens are also exposed as standard CSS variables (`var(--mu-*)`) for absolute custom overrides.
- **Semantic Body & BG Utilities:** Contextual modern classes for themes, including `text-body`, `text-body-secondary`, `bg-body`, `bg-body-secondary`, `bg-transparent`, and `bg-gradient`.
- **Advanced Core Layouts:** Includes layout engines like Vertical/Horizontal Stacks (`vstack`, `hstack`), Aspect Ratios (`ratio-*`), and Vertical Rules (`vr`).
- **Accessibility (A11y) First:** Built-in support for screen-readers and SEO via `.visually-hidden` with standard keyboard focus ring support.
- **Advanced Transitions & Hover:** Enhanced smart interaction utilities (`.transition-colors`, `.transition-border`, `.transition-size`) for butter-smooth hover and focus effects.

---

## 📂 Project Structure

```text
MellowUI-Utilities/
├── CONTRIBUTING.md
├── LICENSE
├── README.md
├── examples/
│    └── demo.html
└── dist/
      └── css/
           ├── mellowui-utilities.css
           └── mellowui-utilities.min.css
```

---

## 🚀 Getting Started

### 1. Manual Installation

Simply download or clone this repository and copy the `dist/css/` folder containing the framework stylesheets into your project directory.

# Clone the repository

```bash
git clone https://github.com/Shayan-0609/MellowUI-Utilities.git
```

### 2. Include in HTML

Link the compressed production stylesheet inside your <head> tag before any custom project styles:

```html
<link rel="stylesheet" href="path/to/dist/css/mellowui-utilities.min.css">
```

### 3. Usage in React / Next.js

Import the production-ready minified CSS file directly into your global entry file (e.g., index.js, main.jsx, or \_app.js):

```javascript
import 'mellowui-utilities';
```

(If you want to import the unminified version, you can use `import 'mellowui-utilities/css';`)

### 4. Include via CDN (Recommended for Plain HTML)

If you are using plain HTML without npm, you can link the production-ready minified stylesheet directly from the CDN inside your `<head>` tag.

#### Option A: jsDelivr

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/mellowui-utilities@1.3.1/dist/css/mellowui-utilities.min.css">

```

#### Option B: unpkg (Alternate CDN)

```html
<link rel="stylesheet" href="https://unpkg.com/mellowui-utilities@1.3.1/dist/css/mellowui-utilities.min.css">

```

---

## 📄 License

Distributed under the MIT License. See LICENSE for more information.

---

## 👨‍💻 Author

Created and maintained by Shayan-0609 — Feel free to connect or contribute!

- GitHub: https://github.com/Shayan-0609/
