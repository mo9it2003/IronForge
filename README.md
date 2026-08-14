# 🏋️ IRONFORGE — Gym Equipment Store

A full-stack e-commerce web app for gym equipment, built as a single HTML file with a real cloud database. Customers can browse products and place orders from any device. Owners manage everything through a PIN-protected admin panel.

**Live demo:** https://mo9it2003.github.io/IronForge

---

## Features

**Customer side**
- Mobile-first design with bottom navigation bar
- Product grid with images and prices in DZD
- Slide-up cart drawer (swipe to close)
- Order form — name, phone, wilaya, address

**Admin panel** (PIN protected)
- Real-time dashboard — total orders, revenue, pending/confirmed count
- Confirm, cancel, or delete orders
- Add products with image upload or emoji
- All data syncs instantly across every device

---

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | HTML, CSS, Vanilla JavaScript |
| Database | JSONBin.io REST API |
| Hosting | GitHub Pages |
| Fonts | Bebas Neue + DM Sans (Google Fonts) |
| Images | Compressed client-side via Canvas API |

---

## Architecture

Everything runs from a single `index.html` file — no frameworks, no build tools, no server required.

- Product and order data is stored in **JSONBin.io** (cloud key-value store)
- All API calls use `fetch()` with a Master Key in the request headers
- Images are resized and compressed to base64 before saving to stay under the 1MB bin limit
- GitHub Pages serves the static file — any commit to `main` auto-deploys

---

## What I learned building this

- Why `localStorage` fails in multi-device apps and how to replace it with a real API
- How to authenticate REST API calls with headers
- Client-side image compression using the Canvas API
- Debugging CORS issues, file size limits, and silent API failures
- Deploying static sites with GitHub Pages

---

*Built by [Abdelmokit](https://github.com/mo9it2003) — Algeria 🇩🇿*
