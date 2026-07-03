# Portfolio Website Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Build a single-page dark/cyberpunk portfolio website for Mustafa Kavçın showcasing Aeternia Core and n8n AI Automation projects.

**Architecture:** Pure HTML + CSS + JS, no build step, no dependencies. Three files: `index.html` (structure), `style.css` (Aeternia-inspired dark theme), `script.js` (typing animation + scroll fade-in). Hosted on GitHub Pages.

**Tech Stack:** HTML5, CSS3 (custom properties, grid, flexbox), Vanilla JS (IntersectionObserver, setInterval)

---

## File Structure

```
portfolio/
├── index.html               ← Full page structure, all sections
├── style.css                ← All styles, CSS variables, animations
├── script.js                ← Typing effect, scroll animations
└── assets/
    ├── aeternia-banner.jpg  ← Hero image (copy from Downloads)
    └── cv.pdf               ← CV file (user adds manually)
```

---

### Task 1: Project Setup & Assets

- [ ] **Step 1: Copy hero image**

```bash
cp "C:/Users/ikkiz/Downloads/aeternia-banner.jpg" "C:/Users/ikkiz/portfolio/assets/aeternia-banner.jpg"
```

- [ ] **Step 2: Create index.html**

Create `C:\Users\ikkiz\portfolio\index.html` with full one-page structure: nav, hero, about, projects, contact, footer.

- [ ] **Step 3: Verify file opens in browser**

Open `portfolio/index.html` in browser. Should show unstyled HTML with all sections visible.

- [ ] **Step 4: Init git and commit**

```bash
cd C:/Users/ikkiz/portfolio
git init
git add index.html assets/aeternia-banner.jpg
git commit -m "feat: initial HTML structure"
```

---

### Task 2: CSS — Base, Nav, Hero

- [ ] **Step 1: Write style.css** with CSS variables, reset, scanlines, nav, hero
- [ ] **Step 2: Verify** — background `#0a0a0f`, hero two-column layout, image visible

---

### Task 3: CSS — About, Projects, Contact, Footer

- [ ] **Step 1: Append** about grid, badges, project cards with hover glow, contact buttons, footer
- [ ] **Step 2: Verify** — all sections styled, card hover glows purple
- [ ] **Step 3: Commit**

```bash
git add style.css
git commit -m "feat: complete CSS styling"
```

---

### Task 4: CSS — Animations & Responsive

- [ ] **Step 1: Append** `.fade-in` / `.visible` classes and `@media (max-width: 768px)` breakpoints
- [ ] **Step 2: Verify** — mobile view collapses to single column

---

### Task 5: JavaScript

- [ ] **Step 1: Create script.js** with typing effect (cycles 4 titles) and IntersectionObserver scroll fade-in
- [ ] **Step 2: Verify typing** — hero shows cycling animated text
- [ ] **Step 3: Verify scroll** — sections fade in from below on scroll
- [ ] **Step 4: Commit**

```bash
git add script.js style.css
git commit -m "feat: typing animation and scroll fade-in"
```

---

### Task 6: GitHub Pages Deployment

- [ ] **Step 1: Create .gitignore** (`.DS_Store`, `Thumbs.db`, `*.log`)
- [ ] **Step 2: Create GitHub repo** at https://github.com/new — name: `portfolio`, Public
- [ ] **Step 3: Push**

```bash
cd C:/Users/ikkiz/portfolio
git add .gitignore
git commit -m "chore: add gitignore"
git remote add origin https://github.com/Vortexalpha123/portfolio.git
git branch -M main
git push -u origin main
```

- [ ] **Step 4: Enable GitHub Pages** — Settings → Pages → Branch: main / root → Save
- [ ] **Step 5: Verify** — visit `https://vortexalpha123.github.io/portfolio/` after ~60 seconds
- [ ] **Step 6: Add CV later** — copy `cv.pdf` to `assets/`, commit and push
