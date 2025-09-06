# CSS Fundamentals

## What is CSS?
CSS (Cascading Style Sheets) styles your HTML—controlling colors, fonts, spacing, sizes, and layout.

## Why CSS?
- Makes pages clear and attractive  
- Separates content (HTML) from design (CSS)  
- Adapts layouts to phones, tablets, and desktops

## How to Add CSS
1. **External (recommended):**
   ```html
   <link rel="stylesheet" href="styles.css">
   ```
2. **Internal (in `<head>`):**
   ```html
   <style> h1 { color: teal; } </style>
   ```
3. **Inline (avoid for most cases):**
   ```html
   <h1 style="color: teal;">Title</h1>
   ```

## CSS Fundamentals (Cheat Sheet)
**Selectors** — tell the browser what to style:
```css
/* Element */     p { line-height: 1.6; }
/* Class */       .card { background: #fff; padding: 1rem; border-radius: 8px; }
/* ID (unique) */ #site-title { font-weight: 800; }
/* Descendant */  .nav a { text-decoration: none; }
```

**Properties & values** — `color`, `background`, `font-size`, `margin`, `padding`, `border`, `width`, `height`.

**Box model** — content → padding → border → margin.
```
+-----------------------------+
|         margin              |
|  +-----------------------+  |
|  |        border         |  |
|  |  +-----------------+  |  |
|  |  |     padding     |  |  |
|  |  |  +-----------+  |  |  |
|  |  |  |  content  |  |  |  |
|  |  |  +-----------+  |  |  |
|  |  +-----------------+  |  |
|  +-----------------------+  |
+-----------------------------+
```

**Cascade & specificity** — later/more specific wins: `#id` > `.class` > `element` (many styles like `color` inherit).

**States (pseudo-classes)** — simple interactivity:
```css
.nav a:hover { background: #e5e7eb; }
```

## TODO Tasks Overview
Style a small page using **an external stylesheet**. You’ll practice:
- linking CSS in HTML  
- **element** selectors (`h1`, `p`, `a`)  
- **class** selectors (`.card`, `.btn`)  
- **id** selector (`#site-title`)  
- **descendant** selector (`.nav a`)  
- **grouping** selectors (`h2, h3`)  
- simple **box model** (margin, padding, border)  
- basic **hover** effect (`:hover`)

> Work mostly in `styles.css`. No JavaScript, no frameworks.

## Repo structure
```
/ (repo root)
├─ README.md
├─ index.html       # starter markup
├─ styles.css       # students edit this (TODOs inside)
└─ .gitignore
```

## Getting started
1. Open `index.html` in your editor and browser.
2. Complete the TODOs in `styles.css` (keep changes small and simple).
3. Refresh the browser after each step to see changes.

---

## Tasks (step-by-step)

### 1) Link the stylesheet
- Confirm `<link rel="stylesheet" href="styles.css">` is present in `<head>`.
- ✅ *Verify:* Changing `body { background: ... }` updates the page.

### 2) Global base
- In `styles.css`, set a readable font for the whole page and a comfy line-height.
- Remove default page margins (set `body { margin: 0; }`).
- ✅ *Verify:* Text looks cleaner and touches no screen edge.

### 3) Element selectors
- Style `h1`, `h2`, `p` (font-size, color). Keep it simple.
- ✅ *Verify:* All headings share a consistent look; paragraphs have spacing below.

### 4) ID selector
- Make `#site-title` (the big page title) larger/bolder than other headings.
- ✅ *Verify:* Only the top title is affected.

### 5) Class selectors (cards + buttons)
- Style `.card` with a light background, padding, rounded corners, and margin.
- Style `.btn` with background color, white text, padding, and rounded corners.
- ✅ *Verify:* Articles look like simple cards; the button looks clickable.

### 6) Descendant selector (nav links)
- Target `.nav a` to remove underline and add spacing.
- Add `:hover` for `.nav a` to change color or background slightly.
- ✅ *Verify:* Only links inside the nav change; hover feedback is visible.

### 7) Grouping selector
- Give `h2, h3` a shared color or font-size tweak.
- ✅ *Verify:* Both `h2` and `h3` change together.

### 8) Box model touch-up (recommended)
- Add `max-width` and centered layout to the main content (e.g., `main { max-width: 800px; margin: 0 auto; padding: 1rem; }`).
- ✅ *Verify:* Content is centered with comfortable side padding.

---

## Submission checklist
- [ ] External stylesheet is linked (no inline styles for required tasks).
- [ ] Element selectors used for `h1/h2/p`.
- [ ] `#site-title` styled differently with an **id** selector.
- [ ] `.card` and `.btn` styled using **class** selectors.
- [ ] `.nav a` styled using a **descendant** selector, with a working `:hover`.
- [ ] `h2, h3` grouped in one rule.
- [ ] Basic spacing added with margin/padding.
- [ ] Code is tidy and commented where you made changes.

# Congratulations! You've mastered the CSS fundamentals! 🎉
