# Real-World Examples

Practical, production-ready examples using MellowUI-Utilities.

---

## Complete Examples

### Example 1: Landing Page

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>MellowUI Landing Page</title>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/mellowui-utilities@1.3.2/dist/css/mellowui-utilities.min.css">
</head>
<body>
  <!-- Navigation -->
  <nav class="d-flex justify-content-between align-items-center p-3 border-bottom sticky-top bg-white">
    <div class="fs-5 fw-bold text-primary">MellowUI</div>
    <div class="d-none d-md-flex gap-4">
      <a href="#" class="text-decoration-none text-dark">Features</a>
      <a href="#" class="text-decoration-none text-dark">Pricing</a>
      <a href="#" class="text-decoration-none text-dark">Docs</a>
      <a href="#" class="text-decoration-none text-dark">About</a>
    </div>
    <button class="btn btn-primary">Get Started</button>
  </nav>

  <!-- Hero Section -->
  <section class="py-5" style="background: linear-gradient(135deg, rgba(51, 154, 240, 0.1) 0%, rgba(92, 124, 250, 0.1) 100%);">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-12 col-lg-6 mb-4 mb-lg-0">
          <h1 class="display-3 fw-bold mb-4">Build Faster with MellowUI</h1>
          <p class="fs-5 text-muted mb-4">A lightweight, utility-first CSS framework for rapid component composition. Combine Bootstrap's reliability with Tailwind's agility.</p>
          <div class="d-flex gap-2 flex-wrap">
            <button class="btn btn-primary btn-lg px-4">Start Building</button>
            <button class="btn btn-outline-primary btn-lg px-4">View Docs</button>
          </div>
        </div>
        <div class="col-12 col-lg-6">
          <div class="bg-light rounded-3 p-5 text-center" style="min-height: 400px; display: flex; align-items: center; justify-content: center;">
            <div class="text-muted">Visual mockup or screenshot here</div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Features Section -->
  <section class="py-5 border-top">
    <div class="container">
      <h2 class="text-center fw-bold mb-5">Why Choose MellowUI?</h2>
      <div class="row row-cols-1 row-cols-md-2 row-cols-lg-3 g-4">
        <div class="col">
          <div class="p-4 rounded-3 border h-100">
            <div class="fs-3 mb-3">⚡</div>
            <h4 class="fw-bold mb-2">Lightweight</h4>
            <p class="text-muted">Only 25KB minified. Zero JavaScript dependencies. Pure CSS performance.</p>
          </div>
        </div>
        <div class="col">
          <div class="p-4 rounded-3 border h-100">
            <div class="fs-3 mb-3">🎨</div>
            <h4 class="fw-bold mb-2">Highly Customizable</h4>
            <p class="text-muted">All design tokens exposed as CSS variables. Override anything globally.</p>
          </div>
        </div>
        <div class="col">
          <div class="p-4 rounded-3 border h-100">
            <div class="fs-3 mb-3">📱</div>
            <h4 class="fw-bold mb-2">Responsive First</h4>
            <p class="text-muted">Mobile-first approach with 6 breakpoints. Built-in responsive utilities.</p>
          </div>
        </div>
        <div class="col">
          <div class="p-4 rounded-3 border h-100">
            <div class="fs-3 mb-3">🌈</div>
            <h4 class="fw-bold mb-2">11 Color Palettes</h4>
            <p class="text-muted">100+ color variants. Semantic colors for quick theme implementation.</p>
          </div>
        </div>
        <div class="col">
          <div class="p-4 rounded-3 border h-100">
            <div class="fs-3 mb-3">✨</div>
            <h4 class="fw-bold mb-2">Premium Shadows</h4>
            <p class="text-muted">Beautiful elevation system with mellow soft shadows for modern UX.</p>
          </div>
        </div>
        <div class="col">
          <div class="p-4 rounded-3 border h-100">
            <div class="fs-3 mb-3">♿</div>
            <h4 class="fw-bold mb-2">Accessible</h4>
            <p class="text-muted">A11y-first design. Keyboard support. Screen reader optimized.</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Pricing Section -->
  <section class="py-5 bg-light">
    <div class="container">
      <h2 class="text-center fw-bold mb-5">Simple Pricing</h2>
      <div class="row row-cols-1 row-cols-md-3 g-4">
        <div class="col">
          <div class="card h-100 border-0 shadow">
            <div class="card-body p-4">
              <h5 class="card-title fw-bold mb-2">Starter</h5>
              <p class="text-muted small mb-4">For beginners</p>
              <div class="fs-4 fw-bold text-primary mb-3">Free</div>
              <ul class="list-unstyled small mb-4">
                <li class="mb-2">✓ Core utilities</li>
                <li class="mb-2">✓ 12-column grid</li>
                <li class="mb-2">✓ Basic colors</li>
              </ul>
              <button class="btn btn-outline-primary w-100">Get Started</button>
            </div>
          </div>
        </div>
        <div class="col">
          <div class="card h-100 border-0 shadow border-3" style="border-color: var(--mu-primary) !important;">
            <div class="card-body p-4">
              <h5 class="card-title fw-bold mb-2">Pro</h5>
              <p class="text-muted small mb-4">For professionals</p>
              <div class="fs-4 fw-bold text-primary mb-3">$29<span class="fs-6 text-muted">/year</span></div>
              <ul class="list-unstyled small mb-4">
                <li class="mb-2">✓ All Starter features</li>
                <li class="mb-2">✓ Premium shadows</li>
                <li class="mb-2">✓ Dark mode theme</li>
                <li class="mb-2">✓ Priority support</li>
              </ul>
              <button class="btn btn-primary w-100">Subscribe Now</button>
            </div>
          </div>
        </div>
        <div class="col">
          <div class="card h-100 border-0 shadow">
            <div class="card-body p-4">
              <h5 class="card-title fw-bold mb-2">Enterprise</h5>
              <p class="text-muted small mb-4">For large teams</p>
              <div class="fs-4 fw-bold text-primary mb-3">Custom</div>
              <ul class="list-unstyled small mb-4">
                <li class="mb-2">✓ All Pro features</li>
                <li class="mb-2">✓ Custom branding</li>
                <li class="mb-2">✓ Dedicated support</li>
                <li class="mb-2">✓ SLA guarantee</li>
              </ul>
              <button class="btn btn-outline-primary w-100">Contact Sales</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- CTA Section -->
  <section class="py-5 text-white" style="background: linear-gradient(135deg, #339af0 0%, #5c7cfa 100%);">
    <div class="container text-center">
      <h2 class="fw-bold mb-3">Ready to Build Something Amazing?</h2>
      <p class="fs-5 mb-4 opacity-75">Join thousands of developers using MellowUI-Utilities</p>
      <button class="btn btn-light btn-lg px-5">Get Started Free</button>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-dark text-white py-5">
    <div class="container">
      <div class="row row-cols-1 row-cols-md-4 g-4 mb-4">
        <div class="col">
          <h6 class="fw-bold mb-3">Product</h6>
          <ul class="list-unstyled small">
            <li class="mb-2"><a href="#" class="text-white text-decoration-none">Features</a></li>
            <li class="mb-2"><a href="#" class="text-white text-decoration-none">Pricing</a></li>
            <li class="mb-2"><a href="#" class="text-white text-decoration-none">Updates</a></li>
          </ul>
        </div>
        <div class="col">
          <h6 class="fw-bold mb-3">Resources</h6>
          <ul class="list-unstyled small">
            <li class="mb-2"><a href="#" class="text-white text-decoration-none">Documentation</a></li>
            <li class="mb-2"><a href="#" class="text-white text-decoration-none">Examples</a></li>
            <li class="mb-2"><a href="#" class="text-white text-decoration-none">Blog</a></li>
          </ul>
        </div>
        <div class="col">
          <h6 class="fw-bold mb-3">Company</h6>
          <ul class="list-unstyled small">
            <li class="mb-2"><a href="#" class="text-white text-decoration-none">About</a></li>
            <li class="mb-2"><a href="#" class="text-white text-decoration-none">Contact</a></li>
            <li class="mb-2"><a href="#" class="text-white text-decoration-none">GitHub</a></li>
          </ul>
        </div>
        <div class="col">
          <h6 class="fw-bold mb-3">Legal</h6>
          <ul class="list-unstyled small">
            <li class="mb-2"><a href="#" class="text-white text-decoration-none">Privacy</a></li>
            <li class="mb-2"><a href="#" class="text-white text-decoration-none">Terms</a></li>
            <li class="mb-2"><a href="#" class="text-white text-decoration-none">License</a></li>
          </ul>
        </div>
      </div>
      <hr class="bg-white opacity-25 my-4">
      <div class="text-center text-muted small">
        <p>&copy; 2026 MellowUI. MIT Licensed. Made with ❤️ by Shayan-0609</p>
      </div>
    </div>
  </footer>
</body>
</html>
```

---

### Example 2: Dashboard Layout

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dashboard</title>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/mellowui-utilities@1.3.2/dist/css/mellowui-utilities.min.css">
</head>
<body>
  <div class="d-flex h-100">
    <!-- Sidebar -->
    <aside class="bg-dark text-white p-4" style="width: 250px; height: 100vh; overflow-y: auto;">
      <h5 class="fw-bold mb-4">Dashboard</h5>
      <nav class="vstack gap-2">
        <a href="#" class="text-white text-decoration-none p-2 rounded bg-primary">📊 Overview</a>
        <a href="#" class="text-white text-decoration-none p-2 rounded">👥 Users</a>
        <a href="#" class="text-white text-decoration-none p-2 rounded">📈 Analytics</a>
        <a href="#" class="text-white text-decoration-none p-2 rounded">⚙️ Settings</a>
      </nav>
    </aside>

    <!-- Main Content -->
    <main class="flex-grow-1 p-4 bg-light">
      <!-- Header -->
      <div class="d-flex justify-content-between align-items-center mb-4">
        <h1 class="fw-bold">Dashboard</h1>
        <div class="d-flex gap-3 align-items-center">
          <input type="search" class="form-control" placeholder="Search..." style="width: 200px;">
          <button class="btn btn-primary">+ New</button>
        </div>
      </div>

      <!-- Stats Cards -->
      <div class="row row-cols-1 row-cols-md-4 g-3 mb-4">
        <div class="col">
          <div class="bg-white p-4 rounded shadow">
            <p class="text-muted small mb-2">Total Users</p>
            <h3 class="fw-bold text-primary mb-0">1,234</h3>
            <p class="text-success small mt-2">+5.2% from last month</p>
          </div>
        </div>
        <div class="col">
          <div class="bg-white p-4 rounded shadow">
            <p class="text-muted small mb-2">Revenue</p>
            <h3 class="fw-bold text-success mb-0">$45.2K</h3>
            <p class="text-success small mt-2">+12.5% from last month</p>
          </div>
        </div>
        <div class="col">
          <div class="bg-white p-4 rounded shadow">
            <p class="text-muted small mb-2">Orders</p>
            <h3 class="fw-bold text-info mb-0">856</h3>
            <p class="text-danger small mt-2">-2.1% from last month</p>
          </div>
        </div>
        <div class="col">
          <div class="bg-white p-4 rounded shadow">
            <p class="text-muted small mb-2">Conversion</p>
            <h3 class="fw-bold text-warning mb-0">3.24%</h3>
            <p class="text-success small mt-2">+0.3% from last month</p>
          </div>
        </div>
      </div>

      <!-- Data Table -->
      <div class="bg-white rounded shadow p-4">
        <h5 class="fw-bold mb-3">Recent Transactions</h5>
        <div class="table-responsive">
          <table class="table table-hover mb-0">
            <thead class="table-light">
              <tr>
                <th class="text-muted">ID</th>
                <th class="text-muted">Customer</th>
                <th class="text-muted">Amount</th>
                <th class="text-muted">Status</th>
                <th class="text-muted">Date</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>#1001</td>
                <td>John Doe</td>
                <td>$245.00</td>
                <td><span class="badge bg-success">Completed</span></td>
                <td>2026-06-14</td>
              </tr>
              <tr>
                <td>#1002</td>
                <td>Jane Smith</td>
                <td>$456.00</td>
                <td><span class="badge bg-warning">Pending</span></td>
                <td>2026-06-13</td>
              </tr>
              <tr>
                <td>#1003</td>
                <td>Bob Wilson</td>
                <td>$123.00</td>
                <td><span class="badge bg-danger">Failed</span></td>
                <td>2026-06-12</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </main>
  </div>
</body>
</html>
```

---

### Example 3: Blog Post Layout

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Blog Post</title>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/mellowui-utilities@1.3.2/dist/css/mellowui-utilities.min.css">
</head>
<body>
  <!-- Header -->
  <header class="border-bottom py-3">
    <div class="container d-flex justify-content-between align-items-center">
      <h1 class="fw-bold">Our Blog</h1>
      <nav class="d-flex gap-3">
        <a href="#" class="text-decoration-none text-dark">Home</a>
        <a href="#" class="text-decoration-none text-dark">Posts</a>
        <a href="#" class="text-decoration-none text-dark">About</a>
      </nav>
    </div>
  </header>

  <!-- Main Content -->
  <main class="py-5">
    <div class="container">
      <div class="row g-4">
        <!-- Blog Post -->
        <div class="col-12 col-lg-8">
          <article>
            <img src="featured-image.jpg" class="img-fluid rounded mb-4" alt="Featured image">
            
            <header class="mb-4">
              <h1 class="fw-bold mb-2">Getting Started with MellowUI-Utilities</h1>
              <div class="d-flex gap-3 text-muted small">
                <span>By Sarah Johnson</span>
                <span>June 14, 2026</span>
                <span>5 min read</span>
              </div>
            </header>

            <div class="prose">
              <p>MellowUI-Utilities is a revolutionary CSS framework that combines the best of Bootstrap and Tailwind CSS. In this guide, we'll explore how to get started and build your first project.</p>
              
              <h2 class="fw-bold mt-4 mb-3">Why MellowUI?</h2>
              <p>There are several reasons why developers love MellowUI-Utilities:</p>
              <ul class="ps-4">
                <li>Lightweight and performant</li>
                <li>Highly customizable with CSS variables</li>
                <li>Responsive out of the box</li>
                <li>Beautiful shadow system</li>
              </ul>

              <h2 class="fw-bold mt-4 mb-3">Getting Started</h2>
              <p>Installation is simple. Just include the CSS file in your HTML:</p>
              <pre><code>&lt;link rel="stylesheet" href="mellowui-utilities.min.css"&gt;</code></pre>
              
              <p>Then start using utility classes right away!</p>
            </div>

            <!-- Author Info -->
            <div class="bg-light p-4 rounded mt-5 mb-4">
              <div class="d-flex gap-3">
                <img src="author-avatar.jpg" class="rounded-circle" width="60" height="60" alt="Author">
                <div>
                  <h6 class="fw-bold mb-1">Sarah Johnson</h6>
                  <p class="text-muted small mb-0">Full-stack developer and CSS enthusiast. Passionate about building beautiful web experiences.</p>
                </div>
              </div>
            </div>

            <!-- Comments Section -->
            <section>
              <h3 class="fw-bold mb-4">Comments</h3>
              
              <div class="mb-4 pb-4 border-bottom">
                <div class="d-flex gap-3 mb-3">
                  <img src="comment-avatar-1.jpg" class="rounded-circle" width="40" height="40" alt="Commenter">
                  <div>
                    <h6 class="fw-bold mb-1">Mike Chen</h6>
                    <p class="text-muted small mb-2">2 days ago</p>
                    <p>Great introduction! I've been using MellowUI for a month now and love it.</p>
                  </div>
                </div>
              </div>

              <!-- Comment Form -->
              <div class="vstack gap-3" style="max-width: 600px;">
                <h5 class="fw-bold">Leave a Comment</h5>
                <textarea class="form-control" placeholder="Your comment here..." rows="4"></textarea>
                <button class="btn btn-primary align-self-start">Post Comment</button>
              </div>
            </section>
          </article>
        </div>

        <!-- Sidebar -->
        <aside class="col-12 col-lg-4">
          <!-- Recent Posts -->
          <div class="bg-light p-4 rounded mb-4">
            <h5 class="fw-bold mb-3">Recent Posts</h5>
            <div class="vstack gap-3">
              <div class="pb-3 border-bottom">
                <h6 class="fw-bold mb-1"><a href="#" class="text-decoration-none text-dark">Advanced CSS Techniques</a></h6>
                <p class="text-muted small mb-0">June 12, 2026</p>
              </div>
              <div class="pb-3 border-bottom">
                <h6 class="fw-bold mb-1"><a href="#" class="text-decoration-none text-dark">Web Performance Tips</a></h6>
                <p class="text-muted small mb-0">June 10, 2026</p>
              </div>
              <div>
                <h6 class="fw-bold mb-1"><a href="#" class="text-decoration-none text-dark">Design Systems 101</a></h6>
                <p class="text-muted small mb-0">June 8, 2026</p>
              </div>
            </div>
          </div>

          <!-- Categories -->
          <div class="bg-light p-4 rounded">
            <h5 class="fw-bold mb-3">Categories</h5>
            <div class="d-flex flex-wrap gap-2">
              <span class="badge bg-primary">CSS</span>
              <span class="badge bg-info">Web Design</span>
              <span class="badge bg-success">Performance</span>
              <span class="badge bg-warning">Tutorials</span>
            </div>
          </div>
        </aside>
      </div>
    </div>
  </main>
</body>
</html>
```

---

## Component Snippets

### Alert Component

```html
<!-- Success Alert -->
<div class="alert alert-success alert-dismissible fade show" role="alert">
  <strong>Success!</strong> Your action was completed successfully.
  <button type="button" class="btn-close" data-bs-dismiss="alert"></button>
</div>

<!-- Error Alert -->
<div class="alert alert-danger alert-dismissible fade show" role="alert">
  <strong>Error!</strong> Something went wrong. Please try again.
  <button type="button" class="btn-close" data-bs-dismiss="alert"></button>
</div>
```

### Modal Dialog

```html
<!-- Modal Trigger Button -->
<button class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#exampleModal">
  Open Modal
</button>

<!-- Modal -->
<div class="modal fade" id="exampleModal" tabindex="-1">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header border-bottom">
        <h5 class="modal-title fw-bold">Modal Title</h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
      </div>
      <div class="modal-body">
        <p>Modal content goes here.</p>
      </div>
      <div class="modal-footer border-top">
        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
        <button type="button" class="btn btn-primary">Save Changes</button>
      </div>
    </div>
  </div>
</div>
```

### Badge

```html
<span class="badge bg-primary">Primary</span>
<span class="badge bg-success">Success</span>
<span class="badge bg-danger">Danger</span>
<span class="badge bg-warning">Warning</span>
<span class="badge bg-info">Info</span>
```

### Breadcrumb

```html
<nav aria-label="breadcrumb">
  <ol class="breadcrumb">
    <li class="breadcrumb-item"><a href="#">Home</a></li>
    <li class="breadcrumb-item"><a href="#">Library</a></li>
    <li class="breadcrumb-item active" aria-current="page">Data</li>
  </ol>
</nav>
```

### Pagination

```html
<nav aria-label="Page navigation">
  <ul class="pagination">
    <li class="page-item disabled">
      <a class="page-link" href="#">Previous</a>
    </li>
    <li class="page-item"><a class="page-link" href="#">1</a></li>
    <li class="page-item active">
      <a class="page-link" href="#">2</a>
    </li>
    <li class="page-item"><a class="page-link" href="#">3</a></li>
    <li class="page-item">
      <a class="page-link" href="#">Next</a>
    </li>
  </ul>
</nav>
```

---

## Tips for Using Examples

1. **Customize Colors** - Change `bg-primary` to `bg-success`, `bg-danger`, etc.
2. **Adjust Spacing** - Modify `p-4`, `m-3`, `gap-2` values as needed
3. **Responsive Adjustments** - Add responsive classes like `col-md-6`, `d-md-none`
4. **Dark Mode** - Add dark mode CSS variables for dark theme support
5. **Combine Utilities** - Mix and match utilities to create unique designs

---

**Happy building! 🚀**