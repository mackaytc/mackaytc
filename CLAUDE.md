# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build Commands

This is a Jekyll static site. To build and serve locally:

```bash
bundle exec jekyll serve
```

The site will be available at `http://localhost:4000`.

## Architecture

This is a personal academic website built with Jekyll using the Minima theme with extensive customizations.

### Theme & Styling

- **Theme**: Minima (default Jekyll theme)
- **Color scheme**: Solarized palette throughout
- **Typography**: Libre Baskerville (body), Source Sans Pro (headings/navigation)
- **Primary CSS**: `assets/css/custom.css` - contains all custom styling with `!important` overrides
- **SCSS override**: `_sass/minima/custom-styles.scss` - alternative/backup styles

### Key Design Patterns

- All custom CSS uses `!important` to override Minima defaults
- Solarized colors: `#fdf6e3` (background), `#586e75` (text), `#2aa198` (accent cyan), `#268bd2` (links)
- Images should include `display: block; margin: 0 auto;` for consistent centering
- Two-column layouts use `.two-col-section`, `.two-col-title`, `.two-col-content` classes

### Content Structure

- Pages use `layout: page` frontmatter
- Research detail pages (`drivers-licenses.md`, `nitrate-contamination.md`) follow a Q&A format with subsections
- Navigation order controlled by `header_pages` in `_config.yml`
- PDFs stored in `assets/pdfs/`, images in `assets/images/`

### Custom Includes

- `_includes/head.html` - Custom head with favicon and CSS imports
- `_includes/footer.html` - Currently commented out
