# KlineCraft.com - Astro Project

## Theme  
Minecraft memories, family chronicles, seasonal celebrations, holiday traditions, birthday magic, halloween spirits, easter joy, valentine sweetness, festive gatherings, social moments

## Framework: Astro
Ideal for content-heavy family blog with excellent static site generation and Markdown support.

## Local Development

### Prerequisites
- Node.js 18+
- npm or yarn

### Setup
```bash
# Install dependencies
npm install

# Start development server
npm run dev
```

Visit `http://localhost:4321`

### Available Scripts
- `npm run dev` - Development server with hot reload
- `npm run build` - Production build
- `npm run preview` - Preview production build
- `npm run astro add [integration]` - Add integrations (React, Vue, etc.)

## Content Management

### Blog Posts
Create `.md` or `.mdx` files in `src/content/blog/`:
```markdown
---
title: "Halloween 2024 Photos"
date: 2024-10-31
tags: ["halloween", "family", "photos"]
---

# Our spooky Halloween adventure...
```

### Holiday Collections
Organize content by holidays in `src/content/holidays/`:
- `halloween/`
- `christmas/` 
- `birthday/`
- `easter/`

## Deployment to Cloudflare Pages

### Git Integration (Recommended)
1. Push to GitHub repository
2. Connect to Cloudflare Pages  
3. Configure build:
   - **Build command**: `npm run build`
   - **Build output**: `dist`
   - **Node.js version**: 18

### Direct Deployment
```bash
# Build the site
npm run build

# Deploy via Wrangler
npx wrangler pages publish dist --project-name klinecraft
```

### Domain Setup
- Primary domain: `klinecraft.com`
- Additional domains: `benkline.com`, `boisebenkline.com`
- Configure DNS in Cloudflare dashboard

## Family Blog Features
- Markdown blog support
- Image galleries for family photos
- Holiday-themed layouts
- SEO optimization for family content
- Comments system (via integration)
- Photo optimization and lazy loading

## Recommended Integrations
```bash
# Add React for interactive components
npm run astro add react

# Add image optimization
npm run astro add image

# Add sitemap for SEO
npm run astro add sitemap
```