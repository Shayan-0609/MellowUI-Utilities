# MellowUI-Utilities Documentation

Welcome to the official documentation for **MellowUI-Utilities v1.3.1** — a lightweight, high-performance, utility-first CSS framework engineered for rapid component composition.

---

## Getting Started

### Installation

#### Option 1: NPM Package
```bash
npm install mellowui-utilities
```

Then import in your project:
```javascript
import 'mellowui-utilities';
```

#### Option 2: CDN (Recommended for HTML)
```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/mellowui-utilities@1.3.1/dist/css/mellowui-utilities.min.css">
```

#### Option 3: Direct Download
[Download the latest release](https://github.com/Shayan-0609/MellowUI-Utilities/releases) and include:
```html
<link rel="stylesheet" href="path/to/mellowui-utilities.min.css">
```

---

## Core Concepts

### Utility-First Architecture

MellowUI-Utilities follows a **utility-first CSS philosophy** inspired by Tailwind CSS, combined with the structural reliability of Bootstrap 5.3+ grid architecture. Instead of pre-built components, compose custom designs using atomic utility classes.

#### Example: Building a Card
```html
<div class="p-4 rounded shadow bg-white border">
  <h3 class="fs-5 fw-bold mb-2">Card Title</h3>
  <p class="text-gray-600 mb-3">Card description text</p>
  <button class="btn btn-primary">Action</button>
</div>
```

### Design Tokens & Variables

All design decisions are exposed as CSS variables, enabling:
- **Theme Customization** - Override any color, size, or effect globally
- **Consistency** - Maintain design system coherence across projects
- **Maintainability** - Update designs in one location
- **Performance** - Minimal CSS footprint with maximum flexibility

---

## Design System

### Color System

#### Primary Palette

MellowUI provides 11 carefully curated color families, each with 9 intensity levels (100-900):

| Color | Primary | Hex Value |
|-------|---------|----------|
| **Blue** | `--mu-blue` | `#339af0` |
| **Indigo** | `--mu-indigo` | `#5c7cfa` |
| **Purple** | `--mu-purple` | `#845ef7` |
| **Pink** | `--mu-pink` | `#e64980` |
| **Red** | `--mu-red` | `#ff7a5f` |
| **Orange** | `--mu-orange` | `#ff922b` |
| **Yellow** | `--mu-yellow` | `#ffd43b` |
| **Green** | `--mu-green` | `#51cf66` |
| **Teal** | `--mu-teal` | `#20c997` |
| **Cyan** | `--mu-cyan` | `#22b8cf` |
| **Gray** | `--mu-gray` | `#a8adb3` |

#### Semantic Colors

```css
--mu-primary: #339af0;      /* Primary actions */
--mu-secondary: #7d838a;    /* Secondary content */
--mu-success: #51cf66;      /* Success states */
--mu-warning: #ffd43b;      /* Warning alerts */
--mu-danger: #ff7a5f;       /* Destructive actions */
--mu-info: #22b8cf;         /* Information */
--mu-light: #f6f7f8;        /* Light backgrounds */
--mu-dark: #1f2328;         /* Dark content */
```

#### Color Variants

Each color provides **100 variants** (10 shades × 10 intensities):

```html
<!-- Usage Examples -->
<p class="text-blue-600">Primary blue text</p>
<div class="bg-green-100">Light green background</div>
<span class="border-red-500">Red border</span>
```

All color variants are automatically generated from the 11 base colors:
- **100** - Lightest (background use)
- **300** - Very light (hover states)
- **500** - Medium (primary use)
- **700** - Dark (emphasis)
- **900** - Darkest (strong contrast)

### Typography Scale

#### Font Sizes (Responsive)

Uses **CSS `clamp()`** for fluid, responsive typography:

```css
--mu-fs-1: clamp(1.375rem, 1.375rem + 1.5vw, 2.5rem);   /* h1 */
--mu-fs-2: clamp(1.325rem, 1.325rem + 0.9vw, 2rem);    /* h2 */
--mu-fs-3: clamp(1.3rem, 1.3rem + 0.6vw, 1.75rem);     /* h3 */
--mu-fs-4: clamp(1.275rem, 1.275rem + 0.3vw, 1.5rem);  /* h4 */
--mu-fs-5: 1.25rem;                                      /* h5 */
--mu-fs-6: 1rem;                                         /* h6 / body */
```

**Benefits:**
- 📱 Automatically scales between breakpoints
- 🎯 No media queries needed for font sizes
- ✨ Smooth, elegant scaling
- 🚀 Better performance

#### Font Families

```css
--mu-font-sans-serif: system-ui, -apple-system, "Segoe UI", "Helvetica Neue", Arial, sans-serif;
--mu-font-monospace: SFMono-Regular, Menlo, Monaco, Consolas, "Courier New";
```

### Spacing System

Follows a **4px baseline grid** for perfect alignment:

```css
--mu-base-spacer: 1rem;           /* 16px base unit */
--mu-spacer-1: 0.25rem;           /* 4px */
--mu-spacer-2: 0.5rem;            /* 8px */
--mu-spacer-3: 1rem;              /* 16px */
--mu-spacer-4: 1.5rem;            /* 24px */
--mu-spacer-5: 3rem;              /* 48px */
```

#### Spacing Utilities

```html
<!-- Margin -->
<div class="mt-2 mb-3 ms-4 me-5">Custom spacing</div>
<div class="m-0">Reset margins</div>
<div class="mx-auto">Center horizontally</div>

<!-- Padding -->
<div class="p-3 px-4 py-2">Custom padding</div>

<!-- Negative Margins -->
<div class="mt-n2">Negative top margin</div>
```

### Elevation & Shadows

Premium shadow system for depth:

#### Standard Shadows
```css
--mu-box-shadow-sm: 0 2px 4px rgba(0, 0, 0, 0.12);
--mu-box-shadow: 0 4px 10px rgba(0, 0, 0, 0.15);
--mu-box-shadow-lg: 0 8px 20px rgba(0, 0, 0, 0.2);
```

#### Mellow Premium Shadows ✨
```css
--mu-mellow-shadow: 0 0.25rem 0.5rem rgba(0, 0, 0, 0.12);
--mu-mellow-shadow-sm: 0 0.125rem 0.25rem rgba(0, 0, 0, 0.10);
--mu-mellow-shadow-lg: 0 0.5rem 1rem rgba(0, 0, 0, 0.16);
--mu-mellow-shadow-soft: 0 0.125rem 0.25rem rgba(0, 0, 0, 0.08), 
                         0 0.0625rem 0.125rem rgba(255, 255, 255, 0.4);
```

```html
<div class="mellow-shadow-soft">Soft, modern shadow with highlight</div>
```

### Border Radius

```css
--mu-border-radius: 0.375rem;     /* Default (6px) */
--mu-border-radius-sm: 0.25rem;   /* Small (4px) */
--mu-border-radius-lg: 0.5rem;    /* Large (8px) */
--mu-border-radius-xl: 1rem;      /* Extra large (16px) */
--mu-border-radius-2xl: 2rem;     /* 2x extra large (32px) */
--mu-border-radius-pill: 50rem;   /* Pill shape */
--mu-border-radius-circle: 50%;   /* Circle */
```

---

## Layout System

### Container

Responsive container with max-width constraints:

```html
<div class="container">
  <!-- Max-width: 540px (sm), 720px (md), 960px (lg), 1140px (xl), 1320px (xxl) -->
</div>

<div class="container-fluid">
  <!-- 100% width with side padding -->
</div>
```

### Grid System (12-Column)

Bootstrap-compatible 12-column grid:

#### Basic Grid

```html
<div class="row">
  <div class="col-6">Half width (50%)</div>
  <div class="col-6">Half width (50%)</div>
</div>

<div class="row">
  <div class="col-3">25%</div>
  <div class="col-3">25%</div>
  <div class="col-3">25%</div>
  <div class="col-3">25%</div>
</div>
```

#### Responsive Grid

```html
<div class="row">
  <!-- Full width on mobile, half on tablet, 33% on desktop -->
  <div class="col-12 col-md-6 col-lg-4">Column</div>
  <div class="col-12 col-md-6 col-lg-4">Column</div>
  <div class="col-12 col-lg-4">Column</div>
</div>
```

#### Column Utilities

| Class | Width |
|-------|-------|
| `.col-auto` | Auto based on content |
| `.col-1` to `.col-12` | 8.33% to 100% |

#### Row Columns (Automatic Wrapping)

```html
<!-- Automatically wrap into N columns -->
<div class="row row-cols-1">
  <div>Full width each</div>
  <div>Full width each</div>
</div>

<div class="row row-cols-3">
  <div>1/3 width</div>
  <div>1/3 width</div>
  <div>1/3 width</div>
</div>
```

#### Offsets

```html
<div class="col-6 offset-3">
  <!-- 6 columns wide, offset 3 columns from start -->
</div>
```

### Gutter Control

Premium **1.75rem** gutter spacing (customizable):

```html
<!-- Gutter Presets -->
<div class="row g-0">No gutter</div>
<div class="row g-1">0.25rem gutter</div>
<div class="row g-3">1rem gutter</div>
<div class="row g-5">3rem gutter</div>

<!-- Directional Gutters -->
<div class="row gx-2">Horizontal gutter only</div>
<div class="row gy-4">Vertical gutter only</div>
```

### Breakpoints

| Breakpoint | Class | Min-Width |
|-----------|-------|----------|
| Extra Small | None | 0px |
| Small | `sm` | 576px |
| Medium | `md` | 768px |
| Large | `lg` | 992px |
| Extra Large | `xl` | 1200px |
| Extra Extra Large | `xxl` | 1400px |

```html
<div class="d-none d-md-block">Hidden on mobile, visible on tablet+</div>
<div class="col-12 col-md-6 col-lg-4">Responsive columns</div>
<div class="fs-6 fs-md-5 fs-lg-4">Responsive font size</div>
```

---

## Utility Classes

### Display & Visibility

```html
<div class="d-none">Hidden</div>
<div class="d-block">Block (responsive: d-md-block)</div>
<div class="d-inline">Inline</div>
<div class="d-inline-block">Inline-block</div>
<div class="d-flex">Flexbox (responsive: d-md-flex)</div>
<div class="d-grid">CSS Grid</div>
<div class="d-table">Table display</div>

<!-- Visibility without removing from DOM -->
<div class="visually-hidden">Screen readers only</div>
```

### Flexbox Utilities

#### Direction

```html
<div class="d-flex flex-row">Horizontal (default)</div>
<div class="d-flex flex-column">Vertical stack</div>
<div class="d-flex flex-row-reverse">Reverse horizontal</div>
<div class="d-flex flex-column-reverse">Reverse vertical</div>
```

#### Justify Content

```html
<div class="d-flex justify-content-start">Start (default)</div>
<div class="d-flex justify-content-center">Center</div>
<div class="d-flex justify-content-end">End</div>
<div class="d-flex justify-content-between">Space between</div>
<div class="d-flex justify-content-around">Space around</div>
<div class="d-flex justify-content-evenly">Even spacing</div>
```

#### Align Items

```html
<div class="d-flex align-items-start">Align to top</div>
<div class="d-flex align-items-center">Center vertically</div>
<div class="d-flex align-items-end">Align to bottom</div>
<div class="d-flex align-items-stretch">Stretch (default)</div>
<div class="d-flex align-items-baseline">Baseline alignment</div>
```

#### Flex Wrapping

```html
<div class="d-flex flex-wrap">Wrap items</div>
<div class="d-flex flex-nowrap">No wrap (default)</div>
<div class="d-flex flex-wrap-reverse">Wrap in reverse</div>
```

#### Flex Growth & Shrink

```html
<div class="d-flex">
  <div class="flex-grow-1">Grows to fill available space</div>
  <div>Fixed width</div>
</div>

<div class="d-flex">
  <div>Fixed</div>
  <div class="flex-shrink-1">Can shrink</div>
</div>
```

#### Gap (Spacing Between Items)

```html
<div class="d-flex gap-1">0.25rem gap</div>
<div class="d-flex gap-3">1rem gap</div>
<div class="d-flex gap-5">3rem gap</div>
```

### Stack Components

Convenience classes for common flex patterns:

```html
<!-- Vertical Stack -->
<div class="vstack gap-3">
  <div>Item 1</div>
  <div>Item 2</div>
  <div>Item 3</div>
</div>

<!-- Horizontal Stack -->
<div class="hstack gap-2">
  <div>Left</div>
  <div class="ms-auto">Right (auto margin)</div>
</div>
```

### Text Utilities

#### Text Alignment

```html
<p class="text-start">Left aligned</p>
<p class="text-center">Center aligned</p>
<p class="text-end">Right aligned</p>
<p class="text-justify">Justified text</p>
```

#### Text Transformation

```html
<p class="text-lowercase">lowercase</p>
<p class="text-uppercase">UPPERCASE</p>
<p class="text-capitalize">Capitalized</p>
```

#### Font Weight & Style

```html
<p class="fw-light">Light (300)</p>
<p class="fw-normal">Normal (400)</p>
<p class="fw-bold">Bold (700)</p>

<p class="fst-italic">Italic</p>
<p class="fst-normal">Not italic</p>
```

#### Text Size & Color

```html
<p class="small">Small text (0.875em)</p>
<p class="lead">Lead text (1.25rem, weight 300)</p>

<p class="text-muted">Secondary/muted text</p>
<p class="text-primary">Primary blue</p>
<p class="text-danger">Danger red</p>
<p class="text-{color}-{shade}">Color variant</p>
```

#### Text Truncation

```html
<p class="text-truncate">This long text will be truncated with ellipsis...</p>

<div class="text-truncate">
  <span>Truncated in single line</span>
</div>
```

### Borders

#### Border Styles

```html
<div class="border">All sides</div>
<div class="border-0">No border</div>

<div class="border-top">Top border</div>
<div class="border-bottom">Bottom border</div>
<div class="border-start">Left border</div>
<div class="border-end">Right border</div>
```

#### Border Colors

```html
<div class="border border-primary">Primary color</div>
<div class="border border-danger">Danger color</div>
<div class="border border-{color}-{shade}">Color variant</div>
```

#### Border Radius

```html
<div class="rounded">Default radius</div>
<div class="rounded-1">Small (4px)</div>
<div class="rounded-2">Medium (8px)</div>
<div class="rounded-3">Large (16px)</div>
<div class="rounded-pill">Pill shape</div>
<div class="rounded-circle">Circle</div>

<!-- Corner-specific -->
<div class="rounded-top">Top corners only</div>
<div class="rounded-bottom">Bottom corners only</div>
```

### Shadows

```html
<div class="shadow-sm">Small shadow</div>
<div class="shadow">Standard shadow</div>
<div class="shadow-lg">Large shadow</div>

<!-- Premium Mellow Shadows -->
<div class="mellow-shadow">Modern soft shadow</div>
<div class="mellow-shadow-sm">Subtle shadow</div>
<div class="mellow-shadow-lg">Prominent shadow</div>
<div class="mellow-shadow-soft">Soft with highlight</div>

<div class="shadow-none">No shadow</div>
```

### Aspect Ratio

```html
<div class="ratio ratio-1x1">
  <img src="image.jpg" alt="">
</div>

<div class="ratio ratio-4x3">
  <img src="image.jpg" alt="">
</div>

<div class="ratio ratio-16x9">
  <iframe src="video.mp4"></iframe>
</div>

<div class="ratio ratio-21x9">
  <iframe src="embed.html"></iframe>
</div>
```

---

## Customization

### Override Design Tokens

Create a custom CSS file to override any design token:

```css
/* custom-theme.css */
:root {
  /* Override primary color */
  --mu-primary: #ff6b6b;
  --mu-primary-rgb: 255, 107, 107;
  
  /* Override spacing */
  --mu-base-spacer: 1.25rem;
  --mu-spacer-1: 0.3125rem;
  --mu-spacer-2: 0.625rem;
  --mu-spacer-3: 1.25rem;
  --mu-spacer-4: 1.875rem;
  --mu-spacer-5: 3.75rem;
  
  /* Override border radius */
  --mu-border-radius: 0.5rem;
  --mu-border-radius-lg: 0.75rem;
  
  /* Override shadows */
  --mu-box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
  --mu-box-shadow-lg: 0 8px 24px rgba(0, 0, 0, 0.15);
  
  /* Override font family */
  --mu-font-sans-serif: 'Inter', system-ui, sans-serif;
}
```

Load your custom theme **after** MellowUI:

```html
<link rel="stylesheet" href="mellowui-utilities.min.css">
<link rel="stylesheet" href="custom-theme.css">
```

### Dark Mode Theme

```css
/* dark-theme.css */
@media (prefers-color-scheme: dark) {
  :root {
    --mu-body-color: #e0e0e0;
    --mu-body-bg: #1a1a1a;
    --mu-secondary-bg: #2d2d2d;
    --mu-tertiary-bg: #242424;
    
    /* Adjust colors for dark mode */
    --mu-primary: #66b3ff;
    --mu-text-muted: #a0a0a0;
  }
}
```

---

## Best Practices

### 1. Use Semantic HTML
```html
<!-- Good -->
<header class="bg-dark text-white p-3">
  <h1>Site Title</h1>
</header>

<!-- Avoid -->
<div class="bg-dark text-white p-3">
  <h1>Site Title</h1>
</div>
```

### 2. Organize Utility Classes
```html
<!-- Group by category -->
<div class="d-flex justify-content-center align-items-center p-4 rounded shadow gap-2">
  <!-- Display → Positioning → Sizing → Spacing → Styling -->
</div>
```

### 3. Extract Repeated Patterns to CSS

```css
/* Instead of repeating utilities, create a custom class */
.card-elevated {
  padding: var(--mu-spacer-4);
  border-radius: var(--mu-border-radius-lg);
  box-shadow: var(--mu-box-shadow);
  background-color: var(--mu-body-bg);
}
```

### 4. Use CSS Variables for Consistency

```css
.my-component {
  color: var(--mu-primary);
  border: var(--mu-border-width) var(--mu-border-style) var(--mu-border-color);
  border-radius: var(--mu-border-radius);
  box-shadow: var(--mu-box-shadow);
}
```

### 5. Respect Accessibility
```html
<!-- Always include alt text -->
<img src="image.jpg" alt="Descriptive text">

<!-- Use semantic form elements -->
<label for="email">Email:</label>
<input id="email" type="email">

<!-- Screen reader only text -->
<span class="visually-hidden">Additional context</span>
```

### 6. Mobile-First Development
```html
<!-- Design for mobile first, then enhance -->
<div class="col-12 col-md-6 col-lg-4">
  Full width on mobile → 50% on tablet → 33% on desktop
</div>
```

---

## Resources

| Resource | Link |
|----------|------|
| **GitHub Repository** | [Shayan-0609/MellowUI-Utilities](https://github.com/Shayan-0609/MellowUI-Utilities) |
| **NPM Package** | [@mellowui-utilities](https://www.npmjs.com/package/mellowui-utilities) |
| **jsDelivr CDN** | [cdn.jsdelivr.net](https://cdn.jsdelivr.net/npm/mellowui-utilities@latest/) |
| **Issue Tracker** | [GitHub Issues](https://github.com/Shayan-0609/MellowUI-Utilities/issues) |
| **License** | [MIT License](https://github.com/Shayan-0609/MellowUI-Utilities/blob/main/LICENSE) |

---

**Maintained by:** [Shayan-0609](https://github.com/Shayan-0609)  
**Version:** 1.3.1  
**Last Updated:** June 14, 2026