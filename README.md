# &lt;Innovative Finance&gt; — Website

A static, multi-page marketing site. No build step. No frameworks. Pure HTML/CSS plus a small JavaScript file for the mobile nav.

## File structure

| File | Purpose |
| --- | --- |
| `index.html` | Home page |
| `what-we-do.html` | What we do (philosophy, methodology, two pillars, landscape) |
| `team.html` | Team (founders, advisors, team philosophy) |
| `insights.html` | Insights & perspectives (articles list) |
| `resources.html` | Resources (models, frameworks, external reading) |
| `404.html` | Not found page |
| `styles.css` | All styles |
| `script.js` | Mobile nav toggle |
| `mark.svg` | Brand mark (for light backgrounds, has navy outline on cream tile) |
| `mark-dark.svg` | Brand mark (for dark backgrounds, no outline) |
| `favicon.svg` | Browser tab icon |

## Editing content via Word docs

The five Word documents in `website-content/` correspond to the five main pages:

1. `01-Home.docx` → `index.html`
2. `02-What-We-Do.docx` → `what-we-do.html`
3. `03-Insights-Perspectives.docx` → `insights.html`
4. `04-Resources.docx` → `resources.html`
5. `05-Team.docx` → `team.html`

Each document contains every editable string on the corresponding page, organized by section. To update the site, edit the docx, send it back, and the HTML will be patched accordingly. **Do not edit the SECTION labels in red** — they are used to find the right place in the HTML.

## Image slots

The site has placeholder image slots throughout. The `image-slot` divs render as gradient placeholders with a label until real images are added. Image briefs:

### Slot 1 — Home page (after "Who we serve" section)
- Type: 16:9 wide editorial photograph
- Theme: Architectural infrastructure
- Prompt for Gemini: *"Editorial architectural photograph of a layered modernist concrete and glass facade, viewed from a low angle, soft overcast diffused light, warm neutral tones with subtle cream and gray, generous negative space at top, professional financial publication aesthetic, no people, no text"*

### Slot 2 — Insights & perspectives page (between header and articles)
- Type: 16:9 wide editorial photograph
- Theme: Bridge cable system or scaffolding lattice
- Prompt: *"Detailed black and white architectural photograph of a suspension bridge cable system, geometric pattern of taut cables converging, soft warm undertones, editorial finance journal style, high resolution"*

### Slot 3 — Resources page (between header and models section)
- Type: 16:9 wide editorial photograph
- Theme: Practitioner desk with notebook
- Prompt: *"Top-down photograph of a financial practitioner's desk: open notebook with hand-drawn capital stack diagrams in navy ink, brass ruler, magnifying loupe, ceramic mug in deep teal, on warm cream surface, soft natural light, editorial finance aesthetic"*

### To swap a placeholder for a real image
Once you have an image, save it to the website folder (e.g., `image-home-1.jpg`) and replace this:
```html
<div class="image-slot aspect-wide" style="min-height: 320px;">
  <span class="slot-label">[Image slot · ...]</span>
</div>
```
with this:
```html
<div class="image-slot aspect-wide" style="min-height: 320px;">
  <img src="image-home-1.jpg" alt="Description of image">
</div>
```

## Hosting on GitHub Pages

Push the repo to GitHub, enable Pages on the `main` branch root.

## Updating the logo

The brand mark lives in two SVG files (`mark.svg` for light backgrounds, `mark-dark.svg` for dark). To change the logo, edit just those two files. Every page references them, so any change propagates everywhere automatically.

## License

Private. Not licensed for redistribution.
