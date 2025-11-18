# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a minimal single-page academic personal website template designed for GitHub Pages hosting. It's a pure HTML/CSS static site with no build process, dependencies, or JavaScript.

## Development

### Local Preview
Open `index.html` directly in a browser - no build step or local server required.

### Deployment
```bash
git add --all
git commit -m "Update website"
git push
```
Site becomes live at `https://<username>.github.io` within a few minutes after push.

## Architecture

**Single-page centered layout:**
- `index.html` - Main HTML with content structure
- `main.css` - All styling (centered layout using absolute positioning + transform)
- `image.jpg` - Avatar/profile photo
- `favicon.png` - Browser favicon

**External dependencies (loaded via CDN):**
- Google Fonts (Source Sans Pro)
- FontAwesome 6.1.1 (general icons)
- Academicons 1.9.2 (academic icons: Google Scholar, ORCiD, NASA/ADS, etc.)

**Layout structure:**
- Content container (`#content`) is vertically and horizontally centered
- Max-width: 520px, padding: 32px
- Avatar: 150px circular image
- Icons: Flexbox horizontal distribution, max 6 icons displayed

## Customization Points

When editing for personalization:
1. **index.html**: Name in `<title>` and `<h1>`, bio paragraphs, icon hrefs, image alt text
2. **main.css**: Color scheme (primary: #1565c0, hover: #217ee7), fonts, spacing
3. **Images**: Replace `image.jpg` and `favicon.png`

**Adding icons** (see README.md for examples):
- FontAwesome: `<i class="fas fa-icon-name"></i>` or `<i class="fab fa-icon-name"></i>`
- Academicons: `<i class="ai ai-icon-name"></i>`

## Repository Constraints

- Must be named exactly `<username>.github.io` for GitHub Pages
- Must be a public repository
- No build tools, package managers, or local dependencies
