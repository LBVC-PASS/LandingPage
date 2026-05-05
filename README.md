# LB — Tools & Links

Personal landing page hosted on GitHub Pages. A lightweight, single-file homepage that centralizes links to internal tools, work bookmarks, and personal sites.

**Live site:** `https://lbvc-pass.github.io`

---

## What's on it

| Section | Contents |
|---|---|
| GitHub Tools | Procurement tool, Capital Dashboard, Personal Dashboard (placeholder) |
| Work | IACLEA, IACP, ASIS, PMI, SEAO, PowerDMS, Agency360, ControlPerfect, Omnivox, Alarm.com |
| Personal | Facebook, Reddit, LinkedIn, YouTube |

---

## How to edit

Everything lives in a single file: `index.html`. No build step, no dependencies, no framework.

### Add a card

Copy any existing card block and paste it inside the relevant `<div class="grid">`:

```html
<a class="card a-purple" href="https://your-url.com" target="_blank">
  <div class="card-stripe"></div>
  <div class="card-top">
    <div class="card-icon">🔧</div>
    <span class="badge">GitHub</span>
  </div>
  <div class="card-name">Tool Name</div>
  <div class="card-desc">Short description of what this does</div>
</a>
```

### Change a card's colour

Swap the accent class on the `<a>` tag:

| Class | Colour |
|---|---|
| `a-purple` | Purple |
| `a-teal` | Teal |
| `a-amber` | Amber |
| `a-blue` | Blue |
| `a-coral` | Coral / Orange |
| `a-red` | Red |
| `a-pink` | Pink |
| `a-plum` | Plum |
| `a-sky` | Sky blue |
| `a-green` | Green |

### Add a new section

```html
<div class="section-label">Section Name</div>
<div class="grid">
  <!-- cards go here -->
</div>
```

### Change the badge label

The badge (top-right of each card) is just text — change it to anything: `GitHub`, `App`, `Web`, `Personal`, `Tool`, etc.

---

## Deployment

This repo is published via **GitHub Pages**.

Settings → Pages → Source: `main` branch, `/ (root)` folder.

Any push to `main` updates the live site within ~30 seconds.

---

## Stack

- Plain HTML + CSS — no build tools, no JavaScript frameworks
- Fonts loaded from Google Fonts (Syne, DM Mono, DM Sans)
- Works offline once fonts are cached
