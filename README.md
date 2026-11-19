# 🌐 LearnSphere — Landing Page

A premium, fully responsive landing page for **LearnSphere**, a next-generation online educational platform. Built with pure HTML5, CSS3, and Vanilla JavaScript — no frameworks or dependencies required.

---

## 📁 Project Structure

```
landing page/
├── index.html      ← Main HTML file (all page content)
├── style.css       ← All styles (layout, colours, animations, responsive)
├── logo.png        ← Platform logo (AI-generated)
├── hero.png        ← Hero section illustration (AI-generated)
└── README.md       ← This file
```

---

## 🚀 How to View the Page

### Option 1 — Open Directly (Quickest)
Double-click **`index.html`** in File Explorer. It will open in your default browser.

### Option 2 — Use VS Code Live Server
1. Install the **Live Server** extension in VS Code.
2. Open the `landing page` folder in VS Code.
3. Right-click `index.html` → **Open with Live Server**.
4. The page auto-refreshes on every save.

### Option 3 — Use Python Local Server
```bash
# Navigate to the project folder, then run:
python -m http.server 8080
# Open: http://localhost:8080
```

### Option 4 — Use Node.js `http-server`
```bash
npx http-server . -p 8080
# Open: http://localhost:8080
```

---

## 🎨 Design System

| Token | Value |
|---|---|
| **Primary Font** | Outfit (headings) |
| **Body Font** | Inter (body text) |
| **Background** | `#05061a` (deep navy) |
| **Accent Purple** | `#8b5cf6` |
| **Accent Cyan** | `#22d3ee` |
| **Accent Pink** | `#ec4899` |

### Colour Palette
- **Background**: Deep navy `#05061a` / `#0a0d2e`
- **Cards**: Glassmorphism with `rgba(255,255,255,0.04)`
- **Gradient**: Purple → Indigo → Cyan
- **Text Primary**: `#f1f5f9` | Secondary: `#94a3b8` | Muted: `#64748b`

---

## 📐 Page Sections

| # | Section | Description |
|---|---|---|
| 1 | **Navbar** | Fixed header with logo, nav links, CTA buttons, mobile drawer |
| 2 | **Hero** | Full-viewport hero with animated orbs, stats bar, and dual CTAs |
| 3 | **Trusted By** | Logos of well-known organizations |
| 4 | **Features** | 6-card grid highlighting platform capabilities |
| 5 | **How It Works** | 4-step numbered process with connecting timeline |
| 6 | **Testimonials** | 3 customer review cards with star ratings |
| 7 | **Pricing** | 3-tier pricing table (Free / Pro / Team) |
| 8 | **CTA** | Full-width conversion section |
| 9 | **Footer** | Multi-column footer with links and social icons |

---

## 📱 Responsive Breakpoints

| Breakpoint | Layout |
|---|---|
| **Desktop** (`>1023px`) | Full multi-column layouts |
| **Tablet** (`768–1023px`) | 2-column grids, mobile nav |
| **Mobile** (`<768px`) | Single column, stacked CTAs |
| **Small Mobile** (`<480px`) | Fully stacked, optimised padding |

---

## ✨ Features & Techniques

### CSS
- CSS Custom Properties (design tokens)
- CSS Grid & Flexbox layouts
- Glassmorphism effects (`backdrop-filter: blur`)
- Animated gradient backgrounds with radial orbs
- `clamp()` for fluid typography
- CSS `@keyframes` animations
- Scroll-driven entrance animations via Intersection Observer
- Mobile-first responsive design

### JavaScript
- **Navbar**: Transparent → frosted glass on scroll
- **Mobile Navigation**: Smooth side-drawer with overlay
- **Scroll Animations**: `IntersectionObserver` for staggered fade-in effects
- **Active Nav Highlight**: Highlights current section's nav link
- **Ripple Effect**: Material-style button click ripples
- **Smooth Scrolling**: Native smooth scroll for all anchor links
- **Accessibility**: ARIA labels, keyboard navigation (Escape to close menu)

---

## 🌐 Browser Support

| Browser | Support |
|---|---|
| Chrome 90+ | ✅ Full |
| Firefox 88+ | ✅ Full |
| Edge 90+ | ✅ Full |
| Safari 14+ | ✅ Full |
| Opera 76+ | ✅ Full |

> **Note**: `backdrop-filter` (blur glassmorphism) requires a browser that supports it. All listed browsers above support this feature.

---

## ♿ Accessibility

- Semantic HTML5 elements (`<header>`, `<main>`, `<section>`, `<article>`, `<nav>`, `<footer>`)
- ARIA roles and labels on all interactive and landmark elements
- Keyboard navigable mobile menu (Escape to close)
- `aria-expanded` state on hamburger button
- `aria-hidden="true"` on decorative elements
- `role="list"` and `role="listitem"` on content collections
- `<blockquote>` for testimonial quotes
- Descriptive `alt` text on all images

---

## 🔧 Customisation Guide

### Changing Colours
Edit the CSS variables at the top of `style.css`:
```css
:root {
  --clr-accent-purple: #8b5cf6;  /* Change primary accent */
  --clr-accent-cyan:   #22d3ee;  /* Change secondary accent */
  --clr-bg-primary:    #05061a;  /* Change background */
}
```

### Changing Brand Name
Search and replace `LearnSphere` in `index.html`.

### Changing Fonts
Update the Google Fonts import at the top of `style.css`:
```css
@import url('https://fonts.googleapis.com/css2?family=YourFont...');
```
Then update `--font-heading` and `--font-body` variables.

### Adding/Removing Sections
Each section is clearly commented in `index.html` with a matching ID. Add or remove as needed.

---

## 📸 Screenshots

The page can be viewed live by opening `index.html` in a browser.

---

## 📄 License

This project is for educational and demonstration purposes.

---

*Built with HTML5, CSS3, and Vanilla JavaScript — no frameworks, no dependencies.*
