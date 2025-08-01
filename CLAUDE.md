# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a GitHub Pages static website for 6DoF Research, an immersive experience consultancy. The website is hosted at 6dof.io and serves as a simple landing page.

## Repository Structure

- **index.html** - Main landing page with inline CSS and minimal JavaScript
- **CNAME** - GitHub Pages custom domain configuration (6dof.io)
- **site.webmanifest** - Web app manifest for PWA features
- **Favicon files** - Various sizes and formats for browser/device compatibility
  - favicon.ico, favicon-16x16.png, favicon-32x32.png
  - apple-touch-icon.png, android-chrome-192x192.png, android-chrome-512x512.png
- **6DoF_Research_Logo_Black_Trim.png** - Company logo image

## Development Workflow

### Local Testing
Since this is a static HTML site, you can test changes by:
1. Opening index.html directly in a browser
2. Using a simple HTTP server: `python3 -m http.server 8000` or `npx http-server`

### Deployment
The site auto-deploys via GitHub Pages when changes are pushed to the master branch.

## Key Considerations

### Styling
- Uses PT Serif font from Google Fonts
- Inline CSS in index.html for simplicity
- Purple color theme (#b400b4) for links and accents
- Responsive design with max-width: 500px container

### Content Updates
When updating content:
- Maintain the minimalist design aesthetic
- Keep the purple (#b400b4) color scheme for brand consistency
- Ensure all links open in new tabs (target="_blank") for external URLs
- Logo image should remain non-clickable (pointer-events: none)

### Performance
- No build process or dependencies
- Minimal JavaScript (only console message on load)
- All assets served directly from repository

### Custom Domain
The site uses a custom domain (6dof.io) configured via CNAME file. Do not delete or modify the CNAME file unless changing the domain.