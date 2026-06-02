# Contributing to MellowUI-Utilities

First off, thank you for considering contributing to MellowUI-Utilities! 🎉 It’s people like you who make the open-source community such an amazing place to learn, inspire, and create.

Please take a moment to review this document before making any contributions to ensure a smooth and efficient workflow.

---

## 🚀 How Can I Contribute?

### 1. Reporting Bugs
If you find a bug or something isn't rendering properly across browsers/devices:
- Check the Issues Tab (https://github.com/Shayan-0609/MellowUI-Utilities/issues) to make sure it hasn't already been reported.
- If it's a new bug, open a new issue. Clearly describe the problem, provide steps to reproduce it, and mention the browser/device you are using.

### 2. Suggesting Features & New Utilities
Want a new spacing utility, a different transition, or another responsive helper?
- Open an issue with the tag "enhancement".
- Describe why this utility is needed and provide an example of how the HTML class name should look.

### 3. Submitting Pull Requests (PR)
Ready to write some CSS? Follow these steps:

1. Fork the Repository: Click the "Fork" button at the top right of this page.
2. Clone Your Fork: Clone it to your local machine or Termux setup using command: git clone https://github.com/YOUR-USERNAME/MellowUI-Utilities.git
3. Create a Branch: Create a descriptive branch name: git checkout -b feature/add-new-utility
4. Make Your Changes: Follow our development guidelines below.
5. Commit & Push: Write clean commit messages and push:
   git commit -m "Feat: Add premium hover lift utilities"
   git push origin feature/add-new-utility
6. Open a PR: Go to the original repository and open a Pull Request against the main branch.

---

## 🛠️ Development Guidelines

To keep the framework lightweight, high-performance, and organized, please adhere to the following rules when editing the codebase:

### 1. File Modification Order
- Do NOT edit the minified file directly. All development changes must be made inside: dist/css/mellowui-utilities.css
- Once you add or modify a class, you must re-minify the file and update: dist/css/mellowui-utilities.min.css
- Use a standard CSS minifier tool (like Toptal CSS Minifier) ensuring that no advanced layout systems or calc blocks are broken.

### 2. Project Architecture
Ensure your changes reflect across the structured directory:

MellowUI-Utilities/
├── LICENSE
├── README.md
├── dist/
│   └── css/
│       ├── mellowui-utilities.css     <-- Edit here
│       └── mellowui-utilities.min.css <-- Update minified version here
└── examples/
    └── demo.html                      <-- Update demo if needed

### 3. Coding Standards
- Atomic & Utility-First: Do not create specific component styles (like .custom-navbar). Instead, create atomic utilities (like .d-flex, .gap-2) that allow developers to compose layouts dynamically.
- Naming Convention: Use clear, lowercase, dash-separated names consistent with Bootstrap/Tailwind practices (like .shadow-hover-md, .mellow-shadow).
- Responsive Classes: If adding responsive variations, ensure they use standard breakpoints (-sm-, -md-, -lg-, -xl-, -xxl-) and are safely wrapped inside the appropriate @media queries at the bottom of the stylesheet.
- Test Your Code: If you add a significant feature or utility, please update examples/demo.html to showcase your code so others can preview it instantly!

---

## 📄 License

By contributing to MellowUI-Utilities, you agree that your contributions will be licensed under the project's MIT License (LICENSE).

Thank you for making MellowUI-Utilities better! 🚀
