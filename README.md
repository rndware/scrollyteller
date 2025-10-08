# 🖼️ CSS-Only Scrollyteller Gallery

A simple **scrollytelling gallery** component built using **HTML, CSS, and Vue 3**.  
Each image sticks as you scroll, while titles and descriptions fade in and out, powered entirely by modern CSS scroll-linked animations.

## 📷 Images

<img src="https://github.com/rndware/scrollyteller/raw/master/main/screenshot.png" width="75%">

---

## ✨ Features

- Pure CSS scroll animations using no JavaScript or intersection observer
- Sticky image transitions using `position: sticky`
- Lightweight Vue 3 instance for templating (no build tools)
- Works directly from a single `index.html` file

---

## ⚙️ How It Works

Each gallery item stays fixed with `position: sticky` while the user scrolls.  
Text overlays animate with:

```css
animation-timeline: view();
animation-range: entry 0% exit 100%;
```

This ties the animation to the scroll position, creating a smooth scrollytelling effect.  
The last hidden item keeps the final image visible at the end.

---

## 🧱 Tech

- **HTML5 + CSS3**
- **Vue 3 (CDN)**
- Modern CSS features:
  - `position: sticky`
  - `animation-timeline: view()`
  - `backdrop-filter`
  - CSS custom properties

---

## 🚀 Run It Locally

1. Download or clone the project  
2. Open `index.html` in your browser  

No setup or build step needed.

---

## 🧩 Customization

Adjust scroll duration or image size via CSS variables:

```css
--gallery-scroll-height: 300vh;
--gallery-item-width: 600px;
```

Add or edit images inside the Vue app data section.

---

## 🌐 Browser Support

CSS scroll-linked animations are supported in:
- Chrome / Edge 115+
- Safari 17+

Older browsers will still show the sticky layout, but without animations.

---

## 🧠 Summary

A minimal experiment showing how scrollytelling effects can be done **entirely with CSS**,  
using `position: sticky` and `animation-timeline` for smooth, declarative scroll interactions.
