# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a single-page portfolio website for a Shopify developer. The entire application is self-contained within `index.html` with no external dependencies, build process, or frameworks.

## Architecture

- **Single-file application**: All HTML, CSS, and JavaScript are embedded in `index.html`
- **No build process**: Direct deployment of the HTML file to any static hosting service
- **No dependencies**: Pure HTML5, CSS3, and vanilla JavaScript
- **Responsive design**: Mobile breakpoint at 768px

## Key Sections and Features

1. **Navigation** (lines ~140-160): Fixed header with smooth scroll links
2. **Hero Section** (lines ~165-185): Animated title with glitch and typing effects
3. **Skills Section** (lines ~190-220): Shopify-specific skills with progress bars
4. **Portfolio Section** (lines ~225-265): Project showcase grid
5. **Services Section** (lines ~270-310): Service cards with hover effects
6. **Contact Section** (lines ~315-340): Contact method links

## JavaScript Functionality (lines ~530-670)

- Scroll-triggered navbar style changes
- Smooth scrolling navigation
- Typing animation for hero text
- Intersection Observer for scroll animations
- Skill bar animations
- Portfolio item click handlers (placeholder)

## CSS Architecture (lines ~35-525)

- CSS custom properties for theme colors
- Shopify brand colors: green (#96bf48) and purple (#5c6ac4)
- Animated gradient background
- Glassmorphism effects with backdrop-filter
- Grid and flexbox layouts
- Transition and animation utilities

## Development Commands

Since this is a static site with no build process:

```bash
# View the site locally
# Option 1: Open directly in browser
start index.html  # Windows
open index.html   # macOS
xdg-open index.html  # Linux

# Option 2: Use a simple HTTP server
python -m http.server 8000  # Python 3
# Then navigate to http://localhost:8000
```

## Common Tasks

- **Modify content**: Edit directly in `index.html`
- **Update styles**: Modify CSS within the `<style>` tags
- **Add functionality**: Edit JavaScript within the `<script>` tags
- **Deploy**: Upload `index.html` to any static hosting service

## Important Considerations

- All assets (images) are currently placeholder URLs
- Contact links use placeholder URLs (mailto:, linkedin.com, github.com)
- Portfolio items have placeholder click handlers
- No form submission functionality implemented
- No analytics or tracking code present