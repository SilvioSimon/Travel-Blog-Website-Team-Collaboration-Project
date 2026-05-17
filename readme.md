# 🌍 Travel Blog

A responsive, multi-page travel blog built with HTML and CSS project.

---

## 📋 Project Overview

Travel Blog is a static website featuring travel articles about destinations around the world. The blog includes animated hero sections, interactive UI components, and a fully responsive layout for all screen sizes.

**Authors:** Regina Metzler, Silvio Simon, Stefan Friggemann  
**Year:** 2026  

---

## 🗂️ Project Structure

```
travel-blog/
│
├── index.html          # Home page – Hero (Cappadocia), Highlights slider, FAQ, Contact form
├── carousel.html       # Article – World's Most Breathtaking Beaches (image carousel)
├── video.html          # Article – Copenhagen in 3 Days (embedded video)
├── graph.html          # Article – Pattaya Pulse (data charts/graphs)
├── imprint.html        # Imprint, Copyright & Cookie Preferences
│
├── css/
│   ├── variables.css   # CSS custom properties (colors, fonts)
│   ├── standard.css    # Global base styles, typography, shared components
│   ├── style.css       # Main layout styles (header, footer, hero, author card, share section)
│   ├── animation.css   # Keyframe animations (hero entrance, wave effects, mobile transitions)
│   ├── carousel.css    # Styles for the beach image carousel / slider
│   ├── video.css       # Styles for the Copenhagen video article page
│   └── graph.css       # Styles for the Pattaya charts page
│
├── assets/
│   ├── fonts/
│   │   ├── Arima/                    # Variable font (headings)
│   │   └── font-Palanquin/palanquin/ # Palanquin font weights (body text)
│   ├── icons/                        # SVG icons (logo, nav, social media, UI elements)
│   └── img/                          # Photos and decorative images
```

---

## 📄 Pages

### `index.html` – Home
- Animated hero section with Cappadocia imagery, floating waves and a rotating location badge
- **Highlights** slider: radio-input–driven CSS-only carousel linking to all three articles
- **FAQ** section using native `<details>` / `<summary>` elements
- **Contact form** with name, email, message and privacy policy checkbox
- Sticky desktop header + mobile bottom navigation bar

### `carousel.html` – Beaches Article
- 3D perspective card carousel (CSS-only, hover-driven on desktop)
- On mobile (≤ 1100 px): switches to a radio-button–controlled sliding carousel with dot indicators
- Pro Tips box and Share button with LinkedIn / WhatsApp options

### `video.html` – Copenhagen Article
- Article layout with author card sidebar
- Clickable video thumbnail linking to YouTube
- Pro Tips section and Share button

### `graph.html` – Pattaya Article
- Article layout with embedded SVG data visualisations:
  - Rain periods bar chart
  - Popular beach activities pie chart
  - Accommodation expenses bar chart
- Share button

### `imprint.html` – Legal
- Impressum (DE) with anchor links from the footer
- Copyright notice
- Cookie policy information

---

## ✨ Features

- **CSS-only sliders** – no JavaScript required for the Highlights slider or the beach carousel
- **3D card effects** – `perspective` + `rotateY` transforms on the carousel cards
- **Entrance animations** – hero text, waves, and location badge animate in on page load (`animation.css`)
- **Custom fonts** – Arima (variable, for headings) and Palanquin (multi-weight, for body)
- **Share button** – expands on focus to reveal LinkedIn and WhatsApp links
- **Responsive design** – breakpoints at 479 px, 500 px, 544 px, 694 px, 700 px, 767 px, 875 px, 932 px, 1100 px, 1280 px, 1440 px
- **Mobile bottom navbar** – fixed navigation bar replaces the desktop header nav on small screens

---

## 🎨 Design System

| Token | Value |
|---|---|
| Primary green | `#4EA487` |
| Accent yellow | `#F1C953` / `#F1C983` |
| Dark brown | `#54370D` |
| Body text | `#3D3D3D` |
| Nav / Footer bg | CSS variable `--nav-footer-bg-color` |
| Heading font | Arima (700) |
| Body font | Palanquin (400 – 700) |

---

## 🚀 Getting Started

No build tools or dependencies required. Open directly in a browser:

```bash
# Clone the repository
git clone <repository-url>

# Open the project
open index.html
```

Or use the **Live Server** extension in VS Code for hot reload during development.

---

## 📱 Responsive Breakpoints

| Range | Layout |
|---|---|
| ≥ 1280 px | Full desktop – side-by-side hero + author card |
| 875 px – 1279 px | Tablet – stacked hero, horizontal author card |
| 480 px – 874 px | Mobile-landscape – adjusted padding, smaller type |
| ≤ 479 px | Mobile – single-column, 16 px gutters, bottom navbar |

---
