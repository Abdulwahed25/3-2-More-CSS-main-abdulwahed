[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](#)
# SocialBook - CSS Layout & Typography (Easy)

## Overview

In this assignment you’ll **reuse the same HTML** and practice new CSS concepts: **Common Properties (colors, backgrounds, display, floats/clear, CSS variables), Font & Text, Box Model, Flexbox, and Positioning (relative/absolute/fixed with z-index)**. Your goal is to style the SocialBook UI with clean layout and readable typography — keeping the tasks simple and focused.

## What You'll Learn

* **CSS Variables** for theme colors
* **Typography basics** (font, size units, text-transform)
* **Box Model** (padding, border, margin, box-sizing)
* **Flexbox** for navigation and tag rows
* **Common Properties** (backgrounds, display, float & clear)
* **Positioning** (fixed nav, absolute badges, z-index)
* **Responsive units** with `clamp()`

## Prerequisites

* Basic understanding of HTML structure
* Any modern web browser
* A text editor (VS Code, Sublime, Notepad++)

## Files

* `index.html`: Same structure as before (link your CSS in the head)
* `styles.css`: Starter CSS with TODOs for the new concepts
* `README.md`: This instruction file

## Instructions

### Step 1: Set Up the Project

1. Open `index.html` in your editor.
2. **TODO 0**: Link the external CSS file in the `<head>` (see comment).

### Step 2: Complete the CSS TODOs

Open `styles.css` and complete each TODO section to style your app:

#### TODO 1: CSS Variables
Define theme colors on `:root` and use them with `var(--color-name)`.

#### TODO 2: Base Typography
Set base font, line-height, and page background on `body`.

#### TODO 3: Box Model & Sizing
Enable `box-sizing: border-box` globally; center `#app` with a card look.

#### TODO 4: Display & Flexbox
Turn `.navigation` into a flex row and make `.trending-tags` wrap with gaps.

#### TODO 5: Font & Text
Make `.username` bolder/larger; adjust heading sizes with `rem`; try a text transform.

#### TODO 6: Backgrounds & Borders
Give `.post` and `.profile-card` nice surfaces, borders, padding, and spacing.

#### TODO 7: Float & Clear
Float `.timestamp` to the right inside `.post` and clear as needed.

#### TODO 8: Positioning + z-index
Fix the top nav with `position: fixed` and `z-index`; add a **Pinned** ribbon to `.post.highlight` using `::before` with `position: absolute`; absolutely position `.follower-count` in `.profile-card`.

#### TODO 9: Buttons & Links (states)
Style `button` and `.chat-link:hover` for simple interactivity.

#### TODO 10: Responsive Units
Use `clamp()` so paragraph text scales a little on wide screens.

### Step 3: Test Your App

1. Save both files
2. Open `index.html` in your browser
3. Verify:
   - Top navigation stays visible while scrolling (fixed + z-index)
   - Posts and profile cards have clean spacing and borders
   - Timestamps float to the right in posts
   - Trending tags wrap nicely on small screens (flex-wrap)
   - Usernames are bold and transformed
   - Buttons/links have hover states
   - Paragraphs scale subtly with `clamp()`

## Understanding the Concepts (Cheat Sheet)

* **Common Properties & Variables**: Colors (hex, rgb, hsl), backgrounds, `display`, `float/clear`, and reusable `--variables`.
* **Font & Text**: `font-family`, `font-size` (use `rem`), `font-weight`, `text-transform`, `letter-spacing`.
* **Box Model**: `padding`, `border`, `margin`, `border-radius`, and universal `box-sizing`.
* **Flexbox**: `display: flex`, `justify-content`, `gap`, `flex-wrap`.
* **Positioning**: `position: fixed/relative/absolute`, anchoring, and `z-index` for stacking.

## Troubleshooting

* **Nav overlaps content?** Increase `body { padding-top: ... }` to match nav height.
* **Float looks odd?** Ensure the container uses a clearfix or add `::after` clear.
* **Badge misplaced?** Make the parent `position: relative` first.
* **Fonts too big/small?** Tweak the base font size or the `clamp()` range.

## Project Structure

```
css-layout-typography/
├── index.html
├── styles.css
└── README.md
```

## Next Steps

* Try `position: sticky` on headers.
* Explore `flex` shorthand on items.
* Experiment with `background-image: linear-gradient(...)` for surfaces.

## CSS Resources

* **MDN CSS Variables**: https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties
* **MDN Box Model**: https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model
* **MDN Flexbox**: https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox
* **MDN Positioning**: https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Positioning
