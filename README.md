# Halcourt Search Website

Executive search website for Halcourt Search Ltd — specialist recruiters for senior Data, Analytics and AI professionals.

## Live Site

[https://halcourtsearch.com](https://halcourtsearch.com) (once deployed)

## Tech Stack

- **HTML5** — Semantic markup
- **CSS3** — Custom properties, Flexbox, Grid
- **Vanilla JavaScript** — No frameworks
- **Vercel** — Hosting and deployment
- **Supabase Storage** — Image hosting (optional)

## Local Development

No build step required. Simply open `index.html` in a browser or use a local server:

```bash
# Using Python
python -m http.server 8000

# Using Node.js (npx)
npx serve

# Using VS Code
# Install "Live Server" extension, right-click index.html → Open with Live Server
```

## Deployment

This site auto-deploys to Vercel when changes are pushed to the `main` branch.

1. Connect this repo to Vercel
2. Framework Preset: Other
3. Root Directory: `./`
4. No build command needed
5. Push to `main` → site deploys automatically

## File Structure

```
halcourt-search/
├── index.html          # Home page
├── expertise.html      # Expertise page
├── services.html       # Services page
├── about.html          # About page
├── contact.html        # Contact page
├── privacy.html        # Privacy Policy
├── terms.html          # Terms & Conditions
├── 404.html            # Error page
│
├── css/
│   ├── variables.css   # Design tokens (colours, typography, spacing)
│   └── styles.css      # Main stylesheet
│
├── js/
│   └── main.js         # Navigation, forms, animations
│
├── images/
│   ├── logo.png        # Halcourt Search logo
│   ├── favicon.ico     # Favicon
│   └── og-image.jpg    # Social sharing image
│
├── docs/               # Documentation
│   ├── STYLE-GUIDE.md
│   ├── CONTENT.md
│   └── IMAGES.md
│
├── vercel.json         # Vercel configuration (optional)
├── .gitignore          # Git ignore rules
└── README.md           # This file
```

## Colour Palette

| Name | Hex | Usage |
|------|-----|-------|
| Deep Navy | `#0F172A` | Primary backgrounds, footer |
| Navy Blue | `#1E2A5E` | Brand colour (matches logo) |
| Slate | `#64748B` | Secondary text |
| Cream | `#FAF9F6` | Warm backgrounds |
| White | `#FFFFFF` | Main backgrounds |
| Black | `#0A0A0A` | Body text |

## Typography

**Font Family:** Plus Jakarta Sans (Google Fonts)

## Updating Content

### Text Content
Edit the HTML files directly. Look for `[PLACEHOLDER]` comments for content that needs to be provided by the client.

### Images
1. Add images to `/images/` folder OR upload to Supabase Storage
2. Update the `src` attribute in HTML files
3. Ensure images are optimised (compressed, correct dimensions)

### Forms
Contact form requires a form submission service (Formspree, Web3Forms, or custom API endpoint). Update the `action` attribute in `contact.html` with your form endpoint URL.

## SEO Checklist

Each page has:
- Unique `<title>` tag
- Meta description
- Canonical URL
- Open Graph tags
- Proper heading hierarchy (single H1)
- Alt text on images

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome for Android)

## Contact

For questions about this website, contact [info@halcourtsearch.com](mailto:info@halcourtsearch.com).
