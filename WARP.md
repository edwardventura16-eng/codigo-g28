# WARP.md

This file provides guidance to WARP (warp.dev) when working with code in this repository.

## Project Overview

This is a frontend learning repository (Codigo G28) focused on HTML and CSS fundamentals. The codebase contains educational examples and challenges for learning web development basics.

## Repository Structure

```
codigo-g28/
├── index.html              # Main HTML practice file with various HTML elements
├── sobre-mi.html           # Personal profile page (About Me)
├── sobre-mi.css            # Styles for personal profile
├── reto-1/                 # Challenge 1: HTML & CSS foundations
│   ├── reto-1.html         # Blog preview card component
│   ├── reto-1.css          # Styles with CSS reset and flexbox layout
│   ├── style-guide.md      # Design specifications (colors, typography, layout)
│   └── assets/
│       ├── images/         # SVG and WebP images for challenge
│       └── fonts/          # Figtree font files
└── *.jpeg                  # Profile and course images
```

## Development Approach

### Styling Methods
The project demonstrates three CSS approaches:
1. **Inline CSS**: Direct styling on HTML elements (e.g., `sobre-mi.html` h1 tag)
2. **Internal CSS**: `<style>` tags within HTML files
3. **External CSS**: Linked `.css` files (preferred for reto-1)

### CSS Patterns
- **CSS Reset**: `reto-1.css` uses universal selector (`*`) to reset browser defaults
- **Selectors**: Uses element, ID (`#image-profile`), and class (`.container`) selectors
- **Layout**: Flexbox for centering and component layout (main container uses `display: flex` with `justify-content` and `align-items`)
- **Design tokens**: Color values use HSL format (e.g., `hsl(47, 88%, 63%)` for yellow)

## Design System (Reto-1)

From `reto-1/style-guide.md`:
- **Layouts**: Mobile (375px), Desktop (1440px)
- **Colors**: 
  - Yellow: `hsl(47, 88%, 63%)`
  - White: `hsl(0, 0%, 100%)`
  - Gray 500: `hsl(0, 0%, 42%)`
  - Gray 950: `hsl(0, 0%, 7%)`
- **Typography**: 
  - Font: Figtree (Google Fonts)
  - Weights: 500, 800
  - Body text: 16px

## Common Tasks

### Viewing HTML Files
Open any `.html` file directly in a browser:
```powershell
# From repository root
Start-Process index.html
Start-Process sobre-mi.html
Start-Process reto-1/reto-1.html
```

### Making Changes
- Edit HTML/CSS files directly in a text editor
- Refresh browser to see changes (no build step required)
- For CSS changes in external files, ensure proper linking in HTML

### Working with Reto-1
The challenge implements a blog preview card component following the style guide specifications. When modifying:
- Maintain the HSL color palette
- Keep Figtree font family
- Use flexbox for layout adjustments
- Ensure responsive design for 375px-1440px range

## Git Status
The repository is initialized but has no commits yet. All files are currently untracked.
