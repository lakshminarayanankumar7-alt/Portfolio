# TOPICS.md — Required HTML & CSS Topics Reference

**Portfolio: Lakshmi Narayana Kumar**
*B.Tech CSE · SRMIST, Kattankulathur · 3rd Year*

This file maps each of the 14 required topics to the exact file(s) and
sections that implement it. Use this during your viva to explain what you built
and why.

---

## Topic 1 — HTML Structure

| Requirement | File | Location / Comment |
|---|---|---|
| `<!DOCTYPE html>` | All 5 HTML files | Line 1 of every file |
| `<html lang="en">` | All 5 HTML files | Opening `<html>` tag |
| `<meta charset="UTF-8">` | All 5 HTML files | Inside `<head>` |
| `<meta name="viewport">` | All 5 HTML files | Inside `<head>` |
| Descriptive `<title>` | All 5 HTML files | Inside `<head>` |
| `<header>`, `<nav>` | All 5 HTML files | Before `<main>` |
| `<main>`, `<section>`, `<article>` | All 5 HTML files | Body content |
| `<footer>` | All 5 HTML files | End of each page |

---

## Topic 2 — Headings, Paragraphs, Text Formatting

| Element | File | Usage |
|---|---|---|
| `<h1>` | All pages | Page / hero headings |
| `<h2>` | All pages | Section headings |
| `<h3>` | `index.html`, `projects.html`, `skills.html` | Card titles |
| `<h4>` | `about.html`, `contact.html`, `skills.html` | Sub-headings |
| `<h5>` | `about.html`, `projects.html`, `skills.html` | Minor labels |
| `<h6>` | `about.html`, `skills.html`, `contact.html` | Footnote labels |
| `<p>` | All pages | Body paragraphs |
| `<strong>` | All pages | Bold emphasis |
| `<em>` | All pages | Italic emphasis |
| `<mark>` | All pages | Highlighted text |
| `<small>` | All pages | Fine-print text |
| `<sub>` | `about.html`, `contact.html` | CO₂ subscript demo |
| `<sup>` | `index.html`, `about.html`, `contact.html` | mc² superscript, 3rd year |
| `<blockquote>` | All pages | Inspirational quotes |

---

## Topic 3 — Lists and Tables

| Element | File | Usage |
|---|---|---|
| `<ul>` unordered list | `skills.html`, `about.html`, `contact.html` | Skill categories, tech stack per card |
| `<ol>` ordered list | `about.html` | Education history (3 steps) |
| `<table>` with `<thead>` / `<tbody>` | `about.html` | Certifications table |
| `<th>` / `<td>` | `about.html` | Table header & data cells |
| `colspan="2"` | `about.html` | "Certifications Earned" merged header |
| `rowspan="2"` | `about.html` | NPTEL row spans 2 certifications; same for Cisco |

---

## Topic 4 — Links

| Link type | File | Detail |
|---|---|---|
| Internal navigation links | All pages | `<nav>` bar links between all 5 pages |
| External — GitHub | All pages | `href="https://github.com/lakshminarayanankumar7-alt"` |
| External — LinkedIn | All pages | `href="https://www.linkedin.com/in/lakshmi-narayanan-kumar-5279a4340/"` |
| External — LeetCode | All pages | `href="https://leetcode.com/u/Lakshmi_Narayana_Kumar/"` |
| All external links | All pages | `target="_blank" rel="noopener noreferrer"` |
| Mailto link | `index.html` footer, `contact.html` | `href="mailto:lakshmi.narayana@example.com"` marked `<!-- EDIT EMAIL -->` |
| In-page anchor (Back to top) | All pages | `href="#top"` → `id="top"` on `<body>` |

> **To update your email:** search for `<!-- EDIT EMAIL -->` in the HTML files.
> It appears in `index.html` and `contact.html`. Replace `lakshmi.narayana@example.com` with your real address.

---

## Topic 5 — Images and Multimedia

| Element | File | Detail |
|---|---|---|
| Profile photo (round, framed) | `index.html` hero | `images/profile.jpg` · class `profile-img` · border-radius 50% |
| Profile photo (float demo) | `about.html` | `images/profile.jpg` · floated left beside bio text |
| Project images with `alt` text | `projects.html`, `index.html` | CSS gradient `<div>` with `role="img"` and `aria-label` (placeholder) |
| `<video controls>` | `about.html` | `media/intro.mp4` · poster set to `profile.jpg` |
| `<audio controls>` | `about.html` | `media/intro.mp3` |
| `<source>` elements | `about.html` | Inside both `<video>` and `<audio>` |

> **To add your own media:** place your video at `media/intro.mp4` and audio at `media/intro.mp3`.
> To add real project screenshots, replace the gradient `<div>` blocks in `projects.html` with `<img>` tags pointing to `images/project1.jpg` etc.

---

## Topic 6 — Colors, Fonts, Backgrounds

| Feature | File | Detail |
|---|---|---|
| CSS custom properties (palette) | `css/style.css` → `:root` block | `--accent`, `--bg-primary`, `--text-primary`, etc. |
| Google Fonts `@import` | `css/style.css` line 1 | Poppins (heading) + Inter (body) with Arial/sans-serif fallbacks |
| Gradient hero background | `css/style.css` → `.hero` | `radial-gradient` + `linear-gradient` combined |
| Gradient page-hero banner | `css/style.css` → `.page-hero` | `linear-gradient` on inner pages |
| Background gradients on project cards | `css/style.css` → `.grad-1` to `.grad-4` | Unique gradient per project category |

---

## Topic 7 — Margins, Padding and the Box Model

| Feature | File | Detail |
|---|---|---|
| `box-sizing: border-box` | `css/style.css` → global `*` reset | Applied to every element |
| `margin:` | `css/style.css` → `.card`, `.form-group`, `.section` | Vertical rhythm between components |
| `padding:` | `css/style.css` → `.card`, `.contact-form`, `thead th`, `tbody td` | Inner spacing |
| `border:` | `css/style.css` → `.card`, `.contact-form`, inputs | 1px solid border on all cards |
| Box Model explanation card | `about.html` → `#boxmodel-heading` section | Visual nested diagram: Margin → Border → Padding → Content |

---

## Topic 8 — Alignment, Floating and Positioning

| Feature | File | Detail |
|---|---|---|
| `text-align: center` | `css/style.css` → `.section-title`, `.page-hero`, `.text-center` | Multiple sections |
| `float: left` | `css/style.css` → `.float-section .float-img` | Profile photo floats beside bio text on `about.html` |
| `position: sticky` | `css/style.css` → `.navbar` | Navbar sticks to top while scrolling |
| `position: fixed` | `css/style.css` → `.back-to-top` | "↑" button fixed to bottom-right corner |
| `position: absolute` | `css/style.css` → `.badge`, `.profile-ring::before`, `.profile-ring::after`, `.page-hero::before`, `.boxmodel-card .bm-label` | Badges on cards, decorative rings |
| `position: relative` | `css/style.css` → `.profile-ring`, `.card`, `.project-card`, `.navbar` | Positioning contexts |

---

## Topic 9 — Navigation Bar

| Feature | File | Detail |
|---|---|---|
| Horizontal sticky navbar | `css/style.css` → `.navbar` | `position: sticky; top: 0` |
| Flexbox layout in navbar | `css/style.css` → `.navbar`, `.nav-links` | `display: flex` with `gap` |
| Hover effect | `css/style.css` → `.nav-links a:hover` | Background tint + underline slide-in |
| Active-page highlight | All HTML files | `class="active"` on current page link + `::after` underline |
| Underline animation | `css/style.css` → `.nav-links a::after` | `width: 0 → 65%` on hover/active |

---

## Topic 10 — CSS Layouts (Flexbox, Grid, Media Queries)

| Feature | File / Section | Detail |
|---|---|---|
| **Flexbox** — navbar | `css/style.css` → `.navbar` | `display: flex; justify-content: space-between` |
| **Flexbox** — hero | `css/style.css` → `.hero` | Side-by-side text + photo |
| **Flexbox** — buttons | `css/style.css` → `.hero-buttons`, `.btn` | Inline button row |
| **Flexbox** — chips & stats | `css/style.css` → `.chips-wrap`, `.stats-row`, `.footer-links` | Wrapping flex rows |
| **CSS Grid** — project cards | `css/style.css` → `.projects-grid` | `repeat(auto-fit, minmax(290px, 1fr))` |
| **CSS Grid** — skill categories | `css/style.css` → `.skills-grid` | `repeat(auto-fit, minmax(240px, 1fr))` |
| **CSS Grid** — social links | `css/style.css` → `.social-links` | `repeat(auto-fit, minmax(200px, 1fr))` |
| **CSS Grid** — contact layout | `contact.html` local `<style>` | 2-column form + social at ≥ 800px |
| **Media queries** — tablet | `css/style.css` → `@media (max-width: 900px)` | Hero stacks, float clears, reduced padding |
| **Media queries** — mobile | `css/style.css` → `@media (max-width: 600px)` | Single-column grids, smaller nav/buttons |

---

## Topic 11 — Borders and Backgrounds

| Feature | File | Detail |
|---|---|---|
| Rounded borders | `css/style.css` → `.card`, `.project-card`, `.btn`, `.profile-img` | `border-radius` from `--r-sm` to `--r-full` |
| Border styles demo | `css/style.css` → `.b-solid`, `.b-dashed`, `.b-dotted`, `.b-double`, `.b-groove` | 5 styles shown on `skills.html` |
| `box-shadow` | `css/style.css` → `.card:hover`, `.back-to-top`, `.profile-ring::after` | Shadow + accent glow |
| Gradient backgrounds | `css/style.css` → `.hero`, `.page-hero`, `.grad-1` to `.grad-4`, `thead` | `linear-gradient` + `radial-gradient` throughout |
| Conic-gradient ring | `css/style.css` → `.profile-ring::before` | Spinning rainbow ring on profile photo |

---

## Topic 12 — Transformations and Transitions

| Feature | File | CSS Property |
|---|---|---|
| Cards lift on hover | `css/style.css` → `.card:hover`, `.project-card:hover` | `transform: translateY(-6px) scale(1.015)` |
| Cards rotate on hover | `css/style.css` → `.project-card:hover` | `rotate(-0.4deg)` |
| Skill cards rotate | `css/style.css` → `.skill-card:hover` | `rotate(-0.6deg)` |
| Buttons lift + shadow | `css/style.css` → `.btn-primary:hover`, `.btn-outline:hover` | `translateY(-3px)` |
| Back-to-top scale | `css/style.css` → `.back-to-top:hover` | `translateY(-5px) scale(1.1)` |
| Social links slide | `css/style.css` → `.social-link:hover` | `translateX(5px)` |
| Smooth transitions | `css/style.css` | `transition: all var(--tr-med)` on cards, buttons, links |
| Transform demo cards | `projects.html` | Inline `onmouseover` demo for translateY / scale / rotate |

---

## Topic 13 — CSS Animations (`@keyframes`)

| Animation name | CSS file | Effect | Used on |
|---|---|---|---|
| `fade-in-up` | `css/style.css` | Elements slide up and fade in | Hero text, role, buttons, page-hero h1/p |
| `float` | `css/style.css` | Gentle up-down bob | Profile photo (`.profile-img`) |
| `spin-ring` | `css/style.css` | Full 360° rotation | Conic-gradient ring (`.profile-ring::before`) |
| `glow-pulse` | `css/style.css` | Opacity + slight scale pulse | Glow layer (`.profile-ring::after`) |
| `pulse-orb` | `css/style.css` | Scale + opacity pulse | Hero decorative orb (`::before`) |
| `bar-grow` | `css/style.css` | Width grows from 0 | CSS skill bars on `skills.html` |
| `bounce-in` | `css/style.css` | Scale bounce entrance | Card badges |
| `submit-pulse` | `contact.html` local `<style>` | Box-shadow pulses | Submit button on contact form |

---

## Topic 14 — HTML Canvas

| Feature | File | Detail |
|---|---|---|
| `<canvas>` element | `skills.html` | `id="skillChart"`, width 800 × height 380, with fallback text |
| JavaScript drawing | `skills.html` | Vanilla JS inside `<script>` tag (the ONLY JS in the project) |
| Animated bar chart | `skills.html` | `requestAnimationFrame` loop, ease-out cubic, `1500ms` duration |
| Editable data array | `skills.html` | `var SKILL_DATA = [...]` — clearly commented, one array to edit |
| Skill values | `skills.html` | HTML 85, CSS 80, JavaScript 70, Java 75, React 65, SQL 70 |
| Responsive canvas | `skills.html` | `sizeCanvas()` recalculates on window resize |
| Canvas glow effect | `skills.html` | `ctx.shadowColor` + `ctx.shadowBlur` per bar |

---

## File Summary

| File | Size | Purpose |
|---|---|---|
| `index.html` | ~190 lines | Home — hero, career interests, stats, featured projects |
| `about.html` | ~240 lines | Bio, float demo, video/audio, education list, certifications table, box model card, leadership |
| `skills.html` | ~270 lines | Skill grid, border demo, Canvas chart, CSS bars, certifications overview |
| `projects.html` | ~200 lines | All 4 project cards, transform hover demo |
| `contact.html` | ~210 lines | Contact form + social links, 2-column layout |
| `css/style.css` | ~580 lines | Shared stylesheet — 15 labelled sections covering all 14 topics |

---

## How to Open the Site

1. Place your photo at `portfolio/images/profile.jpg` (already referenced).
2. Optionally replace `portfolio/media/intro.mp4` and `portfolio/media/intro.mp3`.
3. **Double-click `index.html`** — it opens in your browser with no server required.
4. To update your email, search for `<!-- EDIT EMAIL -->` in `index.html` and `contact.html`.

> **Viva tip:** Every requirement is marked with an HTML comment like
> `<!-- Topic 4: Links -->` or a CSS comment like `/* Topic 7: Box Model */`
> so you can point an examiner to the exact line.

