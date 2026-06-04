# MellowUI-Utilities v1.1.0

A lightweight, high-performance, and Responsive Utility-First CSS Framework Engine built for fast component composition. It bridges the structural power of Bootstrap 5.3+ grid architecture with the atomic agility of Tailwind CSS, enhanced with soft premium Mellow Shadows.

## ✨ Features

- **Atomic Philosophy:** Pure utility-first utility classes (`d-flex, gap-*`, `border-*`, `rounded-*`) without bloated pre-made UI components.
- **Bootstrap 5.3+ Grid Layout:** Reliable, pixel-perfect responsive layout system (`row`, `col-1` to `col-12`, `col-md-6`, `g-*`).
- **Mellow Visual Identity:** Premium custom smooth shadows (`mellow-shadow`, `mellow-shadow-lg`) and custom `active/hover` state color tokens.
- **Advanced Core Layouts:** Includes layout engines like Vertical/Horizontal Stacks (`vstack`, `hstack`), Aspect Ratios (`ratio-*`), and Vertical Rules (`vr`).
- **Accessibility (A11y) First:** Built-in support for screen-readers and SEO via `.visually-hidden` and advanced keyboard navigation support.
- **Hover & Interaction Ready:** Out-of-the-box support for interactive transitions and hover utilities (`shadow-hover-*`, `transition-all`).

---

## 📂 Project Structure
````text
MellowUI-Utilities/
├── LICENSE
├── README.md
└── dist/
    └── css/
        ├── mellowui-utilities.css
        └── mellowui-utilities.min.css
````

---

## 🚀 Getting Started

### 1. Manual Installation
Simply download or clone this repository and copy the `dist/css/` folder containing the framework stylesheets into your project directory.

# Clone the repository
````bash
git clone https://github.com/Shayan-0609/MellowUI-Utilities.git
````

### 2. Include in HTML
Link the compressed production stylesheet inside your <head> tag before any custom project styles:
````html
<link rel="stylesheet" href="path/to/dist/css/mellowui-utilities.min.css">
````

### 3. Usage in React / Next.js
Import the production-ready minified CSS file directly into your global entry file (e.g., index.js, main.jsx, or _app.js):
````javascript
import 'mellowui-utilities';
````
(If you want to import the unminified version, you can use `import 'mellowui-utilities/css';`)

### 4. Include in Plain HTML

​If you are using npm, link the production stylesheet from node_modules inside your <head> tag:

````html
<link rel="stylesheet" href="./node_modules/mellowui-utilities/dist/css/mellowui-utilities.min.css">
````
Or if you installed it manually:
````html
<link rel="stylesheet" href="path/to/dist/css/mellowui-utilities.min.css">
````
---

## 📄 License

Distributed under the MIT License. See LICENSE for more information.

---

## 👨‍💻 Author

Created and maintained by Shayan-0609 — Feel free to connect or contribute!
- GitHub: https://github.com/Shayan-0609/