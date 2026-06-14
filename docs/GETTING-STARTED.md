# Getting Started with MellowUI-Utilities

Quick reference guide to get up and running with MellowUI-Utilities in minutes.

---

## 5-Minute Setup

### Step 1: Install

#### For NPM Projects
```bash
npm install mellowui-utilities
```

#### For HTML Projects
Simply link the CDN in your `<head>`:
```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/mellowui-utilities@1.3.1/dist/css/mellowui-utilities.min.css">
```

### Step 2: Use in Your HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>MellowUI Demo</title>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/mellowui-utilities@1.3.1/dist/css/mellowui-utilities.min.css">
</head>
<body>
  <div class="container mt-5">
    <h1 class="mb-4">Welcome to MellowUI</h1>
    <p class="lead">Build beautiful layouts with utility-first CSS</p>
  </div>
</body>
</html>
```

### Step 3: Start Using Utilities!

```html
<!-- Create a simple card -->
<div class="bg-white rounded shadow p-4 mb-3">
  <h3 class="fw-bold mb-2">Card Title</h3>
  <p class="text-muted">Card description goes here</p>
</div>
```

---

## Common Patterns

### 1. Centered Card

```html
<div class="d-flex justify-content-center align-items-center" style="min-height: 100vh;">
  <div class="bg-white rounded shadow p-5" style="max-width: 400px;">
    <h2 class="mb-4">Card Title</h2>
    <p class="text-muted mb-4">Some descriptive text here</p>
    <button class="btn btn-primary w-100">Action Button</button>
  </div>
</div>
```

### 2. Responsive Grid

```html
<div class="container mt-5">
  <div class="row g-4">
    <div class="col-12 col-md-6 col-lg-4">
      <div class="bg-light p-3 rounded">Column 1</div>
    </div>
    <div class="col-12 col-md-6 col-lg-4">
      <div class="bg-light p-3 rounded">Column 2</div>
    </div>
    <div class="col-12 col-lg-4">
      <div class="bg-light p-3 rounded">Column 3</div>
    </div>
  </div>
</div>
```

### 3. Navigation Bar

```html
<nav class="d-flex justify-content-between align-items-center p-3 bg-primary rounded mb-4">
  <span class="text-white fw-bold fs-5">Brand</span>
  <div class="d-flex gap-3">
    <a href="#" class="text-white text-decoration-none">Home</a>
    <a href="#" class="text-white text-decoration-none">About</a>
    <a href="#" class="text-white text-decoration-none">Contact</a>
  </div>
</nav>
```

### 4. Feature Section

```html
<section class="py-5">
  <div class="container">
    <h2 class="text-center mb-5">Our Features</h2>
    <div class="row row-cols-1 row-cols-md-3 g-4">
      <div class="col">
        <div class="text-center">
          <div class="bg-primary text-white rounded-circle d-flex justify-content-center align-items-center" style="width: 60px; height: 60px; margin: 0 auto 1rem;">
            ✨
          </div>
          <h4 class="fw-bold">Feature One</h4>
          <p class="text-muted">Description of the first feature</p>
        </div>
      </div>
      <div class="col">
        <div class="text-center">
          <div class="bg-success text-white rounded-circle d-flex justify-content-center align-items-center" style="width: 60px; height: 60px; margin: 0 auto 1rem;">
            🚀
          </div>
          <h4 class="fw-bold">Feature Two</h4>
          <p class="text-muted">Description of the second feature</p>
        </div>
      </div>
      <div class="col">
        <div class="text-center">
          <div class="bg-info text-white rounded-circle d-flex justify-content-center align-items-center" style="width: 60px; height: 60px; margin: 0 auto 1rem;">
            💎
          </div>
          <h4 class="fw-bold">Feature Three</h4>
          <p class="text-muted">Description of the third feature</p>
        </div>
      </div>
    </div>
  </div>
</section>
```

### 5. Image Gallery

```html
<section class="py-5">
  <div class="container">
    <h2 class="mb-4">Gallery</h2>
    <div class="row row-cols-1 row-cols-md-2 row-cols-lg-3 g-3">
      <div class="col">
        <img src="image1.jpg" class="img-fluid rounded shadow" alt="Gallery item 1">
      </div>
      <div class="col">
        <img src="image2.jpg" class="img-fluid rounded shadow" alt="Gallery item 2">
      </div>
      <div class="col">
        <img src="image3.jpg" class="img-fluid rounded shadow" alt="Gallery item 3">
      </div>
    </div>
  </div>
</section>
```

### 6. Form Layout

```html
<form class="vstack gap-3" style="max-width: 500px;">
  <div>
    <label class="form-label fw-bold">Email Address</label>
    <input type="email" class="form-control" placeholder="you@example.com">
  </div>
  <div>
    <label class="form-label fw-bold">Password</label>
    <input type="password" class="form-control" placeholder="Enter password">
  </div>
  <div class="d-flex align-items-center">
    <input type="checkbox" class="form-check-input" id="remember">
    <label class="form-check-label ms-2" for="remember">
      Remember me
    </label>
  </div>
  <button type="submit" class="btn btn-primary btn-lg">Sign In</button>
</form>
```

### 7. Hero Section with CTA

```html
<section class="bg-gradient p-5 text-center text-white" style="background: linear-gradient(135deg, #339af0 0%, #5c7cfa 100%);">
  <div class="container">
    <h1 class="fs-1 fw-bold mb-3">Build Amazing Websites</h1>
    <p class="fs-5 mb-4 opacity-75">With MellowUI-Utilities, create stunning designs faster than ever</p>
    <div class="d-flex gap-2 justify-content-center flex-wrap">
      <button class="btn btn-light btn-lg px-4">Get Started</button>
      <button class="btn btn-outline-light btn-lg px-4">Learn More</button>
    </div>
  </div>
</section>
```

### 8. Footer

```html
<footer class="bg-dark text-white py-5 mt-5">
  <div class="container">
    <div class="row row-cols-1 row-cols-md-4 g-4 mb-4">
      <div class="col">
        <h6 class="fw-bold mb-3">Product</h6>
        <ul class="list-unstyled">
          <li><a href="#" class="text-white text-decoration-none">Features</a></li>
          <li><a href="#" class="text-white text-decoration-none">Pricing</a></li>
          <li><a href="#" class="text-white text-decoration-none">Security</a></li>
        </ul>
      </div>
      <div class="col">
        <h6 class="fw-bold mb-3">Company</h6>
        <ul class="list-unstyled">
          <li><a href="#" class="text-white text-decoration-none">About</a></li>
          <li><a href="#" class="text-white text-decoration-none">Blog</a></li>
          <li><a href="#" class="text-white text-decoration-none">Careers</a></li>
        </ul>
      </div>
      <div class="col">
        <h6 class="fw-bold mb-3">Resources</h6>
        <ul class="list-unstyled">
          <li><a href="#" class="text-white text-decoration-none">Documentation</a></li>
          <li><a href="#" class="text-white text-decoration-none">Guides</a></li>
          <li><a href="#" class="text-white text-decoration-none">API</a></li>
        </ul>
      </div>
      <div class="col">
        <h6 class="fw-bold mb-3">Legal</h6>
        <ul class="list-unstyled">
          <li><a href="#" class="text-white text-decoration-none">Privacy</a></li>
          <li><a href="#" class="text-white text-decoration-none">Terms</a></li>
          <li><a href="#" class="text-white text-decoration-none">Contact</a></li>
        </ul>
      </div>
    </div>
    <hr class="bg-light opacity-25">
    <div class="text-center text-muted">
      <p>&copy; 2026 MellowUI. All rights reserved.</p>
    </div>
  </div>
</footer>
```

---

## Utility Quick Reference

### Display
```html
<div class="d-none">Hidden</div>
<div class="d-block">Block</div>
<div class="d-flex">Flexbox</div>
<div class="d-grid">Grid</div>
```

### Spacing (Margin & Padding)
```html
<div class="m-1">Margin all sides</div>
<div class="mt-2">Margin top</div>
<div class="p-3">Padding all sides</div>
<div class="px-2">Padding horizontal</div>
```

### Text
```html
<p class="text-start">Left aligned</p>
<p class="text-center">Centered</p>
<p class="fw-bold">Bold</p>
<p class="text-muted">Muted/gray</p>
```

### Colors
```html
<div class="text-primary">Primary blue</div>
<div class="bg-success">Green background</div>
<div class="border-danger">Red border</div>
```

### Grid
```html
<div class="row">
  <div class="col-6">Half width</div>
  <div class="col-6">Half width</div>
</div>
```

### Responsive
```html
<div class="d-none d-md-block">Hidden on mobile</div>
<div class="col-12 col-md-6 col-lg-4">Responsive column</div>
```

---

## Tips & Tricks

### 1. Use `ms-auto` to Push Elements Right
```html
<div class="d-flex">
  <span>Left</span>
  <span class="ms-auto">Right</span>
</div>
```

### 2. Stack Multiple Utilities
```html
<!-- Combine utilities for complex layouts -->
<div class="d-flex justify-content-center align-items-center p-4 rounded shadow">
  Content
</div>
```

### 3. Use Responsive Classes
```html
<!-- Adapts to screen size -->
<div class="col-12 col-md-6 col-lg-4">Responsive</div>
```

### 4. Create Custom Classes with CSS Variables
```css
.my-card {
  padding: var(--mu-spacer-4);
  border-radius: var(--mu-border-radius-lg);
  box-shadow: var(--mu-box-shadow);
}
```

---

## Next Steps

- 📖 Read the [full documentation](./index.md)
- 🎨 Explore [real-world examples](./EXAMPLES.md)
- 🔗 Check out the [GitHub repository](https://github.com/Shayan-0609/MellowUI-Utilities)
- 📦 Visit [NPM package](https://www.npmjs.com/package/mellowui-utilities)

---

**Happy coding! 🚀**