# Charme e Flores 🐰🌸

> A premium handmade flower boutique website with an AI-powered assistant.

This project is part of **[TrendCode](https://trendcode.ie)** — a software and cloud engineering service focused on delivering modern, high-quality digital products.

> ⚠️ This website is entirely in **Brazilian Portuguese**, as it serves a Brazilian audience.

---

## About the Project

**Charme e Flores** is a Brazilian handmade flower brand specializing in crochet and chenille artisan pieces. This website serves as a premium digital storefront — not an e-commerce platform, but a curated portfolio that showcases the products and directs customers to WhatsApp or Instagram to place orders.

The site features a kawaii-inspired aesthetic with a signature bunny mascot, soft pink and gold tones, and subtle animations — designed to feel warm, charming, and premium at the same time.

---

## Features

- **Responsive portfolio** — mobile-first design optimized for the brand's audience
- **Product categories** — expandable sections showcasing decorative vases, keychains, and lamp/photo frame pieces
- **AI Assistant (Lua 🐰)** — a floating bunny assistant powered by the Anthropic API that answers product questions and directs customers to order via WhatsApp or Instagram
- **Micro-animations** — falling petals, hover transitions, and subtle motion effects for a premium feel
- **Single HTML file** — no build tools, no frameworks, deployable anywhere

---

## Tech Stack

|
 Layer 
|
 Technology 
|
|
---
|
---
|
|
 Frontend 
|
 HTML5, CSS3, Vanilla JS 
|
|
 AI Assistant 
|
 Anthropic API (
`claude-sonnet-4-20250514`
) 
|
|
 Hosting 
|
 Static (Vercel / Netlify / GitHub Pages) 
|
|
 Dependencies 
|
 None (CDN only if needed) 
|

---

## Project Structure

```
charme-e-flores/
├── index.html        # Full site — single file
├── CLAUDE.md         # Claude Code development guide
├── EDITS.md          # Pending and completed edits log
├── README.md         # This file
└── assets/
    ├── logo.png
    ├── logo-bunny.png
    └── products/
        ├── vasinho-1.jpg
        ├── chaveiro-1.jpg
        └── luminaria-1.jpg
```

---

## Getting Started

No build step required. Just open `index.html` in a browser — or deploy the folder to any static hosting provider.

To enable the AI assistant, set your Anthropic API key where indicated in `index.html`:

```js
// index.html
const ANTHROPIC_API_KEY = "your-api-key-here";
```

---

## Part of TrendCode

This project was designed and developed by **TrendCode** — a self-employed software and cloud engineering venture building modern digital products.

🌐 [trendcode.ie](https://trendcode.ie)

---

*Made with 🌸 for Charme e Flores*
