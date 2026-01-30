# Jamnagar Agro Industries Ltd. (JAI) - Corporate Website

A editorial style corporate website for Jamnagar Agro Industries Ltd., designed to reflect their 11+ years of excellence in the agricultural commodities sector. This project emphasizes a distinct brand identity through bold typography and earthy color palettes.

![Design Preview](assets/images/logo.png)

## Design Philosophy: Earthy Editorial

The design language moves away from traditional cluttered industrial websites to a modern narrative-driven experience. It combines the raw and organic nature of agriculture with the precision of modern manufacturing.

### Key Visual Concepts
1.  **Vertical Stacking**: Content is organized into distinct "cards" or sections that stack vertically. Each section has deeply rounded top corners (`border-radius: 5rem`), creating a smooth, tactile feeling of layering as the user scrolls.
2.  **High-Contrast Typography**:Dramatic contrast between massive and condensed display text for impact.
3.  **Organic Palette**: The color story is strictly derived from nature—deep forest greens, soft sage, warm cream, and earthy moss—avoiding harsh pure blacks or whites.
4.  **Texture & Depth**: A subtle fractal noise overlay is applied globally to soften digital edges, mimicking the texture of paper or organic material. Deep, colored shadows (`shadow-float`) lift elements off the page.

## Design Tokens

The project uses a CSS Variable system to ensure consistency.

### Color Palette
| Token | Hex | Usage |
| :--- | :--- | :--- |
| `--color-forest` | `#01472e` | Primary brand color, text, footers |
| `--color-sage` | `#ccd5ae` | Secondary backgrounds, accents |
| `--color-olive` | `#e9edc9` | Highlights, card backgrounds |
| `--color-cream` | `#fefae0` | Main background, light text |
| `--color-moss` | `#a3b18a` | Subtle text, tertiary backgrounds |

### Typography
*   **Display Font**: `Anton` (Google Fonts). Used for Hero sections and major headings. Uppercase, tight leading (`0.85`), and negative letter spacing.
*   **Body/Utility**: `Inter` (Google Fonts). Used for paragraphs, navigation, and labels. Labels are uppercase with wide tracking (`0.25em`).

### Layout & Spacing
*   **Fluid Typography**: Font sizes use `clamp()` functions to scale seamlessly from mobile to wide screens (e.g., Hero text scales from `3.5rem` to `18rem`).
*   **Border Radius**: 
    *   `--radius-section`: `5rem` (Desktop) / `2rem` (Mobile) - For main section dividers.
    *   `--radius-card`: `2.5rem` - For editorial cards and images.
    *   `--radius-pill`: `9999px` - For navigation and buttons.

## Project Structure

```
/
├── index.html              # Landing Page (Hero, Profile, Clients, Reach)
├── 404.html                # Custom Error Page
│
├── pages/                  # Inner Pages
│   ├── about.html          # History, Timeline, Mission, Vision
│   ├── contact.html        # Contact Form, Map, FAQ
│   ├── products.html       # Retail Brands, Wholesale List, Process
│   └── services.html       # Capabilities, Workflow, Technology
│
├── components/             # Reusable HTML snippets (Reference)
│   ├── navbar.html
│   ├── footer.html
│   └── ...
│
└── assets/
    ├── css/
    │   ├── base/           # Typography, Resets, Variables
    │   ├── components/     # Cards, Buttons, Timeline, Marquee
    │   ├── layout/         # Header, Footer
    │   ├── utilities/      # Helper classes, Stacking logic
    │   ├── vendor/         # Bootstrap, FontAwesome
    │   └── main.css        # Main import file
    │
    ├── images/             # Optimized assets (WebP/PNG/SVG)
    └── js/                 # Vendor scripts & main.js
```
