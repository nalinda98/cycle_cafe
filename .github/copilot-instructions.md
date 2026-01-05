# Copilot Instructions for cycle_cafe

## Project Overview
- This project is a static HTML/CSS/JS personal portfolio site, based on the "ProMan" template from HTML Codex.
- Main entry point: `index.html`.
- Custom styles: `css/style.css`.
- Custom scripts: `js/main.js`.
- Third-party libraries are in `lib/` (e.g., Bootstrap, Owl Carousel, Lightbox, Animate.css, etc.).
- Images are in `img/`.
- SCSS sources for Bootstrap are in `scss/` but are not directly referenced in the HTML (likely for manual or external compilation).

## Key Patterns & Conventions
- **No build system**: There are no build scripts, package.json, or task runners. All files are edited directly.
- **Direct HTML linking**: All CSS and JS are linked directly in `index.html`.
- **jQuery-based scripting**: All custom JS uses jQuery and is wrapped in an IIFE for isolation.
- **Class/ID conventions**: Uses Bootstrap and template-specific classes (e.g., `.back-to-top`, `#spinner`).
- **No module system**: All JS is global or IIFE-scoped; no ES modules or imports.
- **No backend**: This is a purely frontend/static site.

## Editing & Extending
- To add new sections, edit `index.html` and add corresponding CSS/JS if needed.
- For new styles, use `css/style.css`.
- For new scripts, use `js/main.js` or add new files and link them in `index.html`.
- To update libraries, replace files in `lib/` and update links in `index.html`.

## External Dependencies
- All third-party libraries are vendored in `lib/` and referenced locally.
- No CDN dependencies except for Google Fonts and icon fonts (Font Awesome, Bootstrap Icons).

## Example: Adding a Feature
- To add a new animated section:
  1. Add HTML markup in `index.html`.
  2. Add styles to `css/style.css`.
  3. Add JS logic to `js/main.js` (use jQuery, wrap in the existing IIFE).
  4. Use classes from `lib/animate/animate.css` or `lib/wow/wow.js` for animation.

## Testing & Debugging
- Open `index.html` in a browser to view changes.
- No automated tests or build steps are present.

## References
- Template: https://htmlcodex.com/personal-portfolio-html-template
- License: https://htmlcodex.com/license

---
If you need to automate, lint, or add a build process, you must introduce those tools from scratch.
