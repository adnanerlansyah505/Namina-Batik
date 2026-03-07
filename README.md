# Namina Batik

A modern, responsive website for **Namina Batik** — an MSME (UMKM) brand selling adult men's and women's Batik clothing.

## Tech Stack

- **Framework:** Astro.js
- **Styling:** Tailwind CSS
- **CMS:** Markdown (Astro Content Collections)
- **Interactivity:** Vanilla JS & HTML5 dialogs

## Project Structure

```
src/
├── components/     # Reusable components (Navbar, Footer, ProductGallery)
├── content/
│   └── articles/   # Markdown articles for the blog
├── layouts/        # BaseLayout
├── pages/          # Routes
│   ├── index.astro
│   └── articles/
│       ├── index.astro
│       └── [slug].astro
└── styles/         # Global CSS
```

## Getting Started

```bash
npm install
npm run dev      # Start dev server at http://localhost:4321
npm run build    # Production build
npm run preview  # Preview production build
```

## Adding Articles

Create a new `.md` file in `src/content/articles/` with frontmatter:

```yaml
---
title: Your Article Title
description: Brief excerpt for the article list
pubDate: 2024-01-15
---
```

## Customization

- **Colors:** Edit `tailwind.config.mjs` under the `batik` color palette
- **Products:** Update `ProductGallery.astro` with your product data
- **Location:** Replace the Google Maps embed URL in `index.astro` with your actual location
