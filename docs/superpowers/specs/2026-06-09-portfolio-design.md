# Portfolio Website — Design Spec
**Date:** 2026-06-09  
**Status:** Approved

---

## Overview

A single-page personal portfolio website for Mustafa Kavçın. Aesthetic inspired by Aeternia Core — dark, cyberpunk/HUD style with purple accents. Built with pure HTML + CSS + JS, hosted on GitHub Pages.

---

## Aesthetic

- **Background:** `#0a0a0f`
- **Accent:** `#7c3aed` → `#a855f7` (purple gradient)
- **Text:** `#e2e8f0`
- **Border/glow:** `#7c3aed` semi-transparent
- **Style:** Terminal/HUD — scan-line overlay, glowing borders, typing animation, fade-in on scroll

---

## Page Structure (one-page, scroll)

### 1. HERO
- Large heading: `MUSTAFA KAVÇIN`
- Typing animation cycling: `"AI Developer"` → `"Automation Engineer"` → `"Node.js Developer"`
- Tagline (single line): `AI • Automation • APIs • Real-World Solutions`
- Two CTA buttons: `View Projects` and `Download CV`
- Right side: `aeternia-banner.jpg` hero image
- Subtle scan-line background effect

### 2. ABOUT
- **Left:** 2–3 sentence bio:
  > "Computer Programming student focused on AI applications, automation systems, and API integrations. I build things that connect intelligence to real-world workflows."
- **Right:** Tech stack badges in a grid:
  `Node.js` `JavaScript` `Python` `SQL` `n8n` `OpenAI API` `REST APIs` `Git`
- Badges fade in on scroll

### 3. PROJECTS
Two cards side by side:

**Card 1 — Aeternia Core**
- Description: Twitch AI avatar bot with mood engine, TTS, rank system, and OSC avatar control
- Tags: `Node.js` `OpenAI` `ElevenLabs` `Twitch`
- Link: GitHub repo

**Card 2 — n8n AI Automation**
- Description: AI-powered product data automation using n8n, OpenAI, and Google Sheets
- Tags: `n8n` `OpenAI` `Google Sheets`
- Link: GitHub repo (optional)

Cards have purple glow border on hover.

### 4. CONTACT
- Three buttons: `LinkedIn` · `GitHub` · `mustafakavcin43@gmail.com`
- Below: prominent `Download CV` button

---

## Animations
- Typing effect in hero (loops)
- Elements enter from below on scroll (IntersectionObserver)
- Card hover: purple glow border
- Tech badges: staggered fade-in

---

## Tech Stack
- Pure HTML + CSS + JS (no framework, no build step)
- Hosted on GitHub Pages
- Single `index.html` + `style.css` + `script.js`

---

## Assets
- `assets/aeternia-banner.jpg` — hero image (already compressed to 0.16 MB)
- `assets/cv.pdf` — CV file (to be added by user)
