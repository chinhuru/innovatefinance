# [Firm Name] — Website

A static, multi-page marketing site built from the brand guide. No build step. No frameworks. Just HTML, CSS, and a tiny bit of JavaScript.

## Pages

| File | Purpose |
| --- | --- |
| `index.html` | Home — positioning, headline stats, two offerings, who we serve |
| `philosophy.html` | Philosophy & offering — methodology, framework, advisory & platform detail, competitive landscape |
| `about.html` | About — founders, board of advisors, future team |
| `thinking.html` | Thought leadership — articles list (placeholder) |
| `resources.html` | Public tools — models, frameworks, external reading (placeholder) |
| `404.html` | Not-found page |

## Editing the firm name

Every page uses `[Firm Name]` as the placeholder. To replace globally, run a find-and-replace across all `.html` files. On macOS / Linux:

```bash
# Replace [Firm Name] with your real firm name in every HTML file
find . -name "*.html" -exec sed -i '' 's/\[Firm Name\]/Your Firm Name/g' {} +
```

(On GNU sed / Linux, drop the `''` after `-i`.)

## Editing content

- **Founder bios:** `about.html`, search for `[Bio placeholder`
- **Advisor cards:** `about.html`, search for `[Advisor name]`
- **Articles:** `thinking.html`, search for `[Article title placeholder`
- **Resources:** `resources.html`, search for `placeholder`
- **Contact email:** every page uses `hello@example.com` — find/replace globally
- **External links:** Update `LinkedIn` and any external resource URLs in the footer and resources page

## Brand tokens

All colors, fonts, and spacing rules are CSS variables defined at the top of `styles.css`. To adjust the palette, edit the `:root` block.

## Hosting on GitHub Pages

Push the repo to GitHub, enable Pages on the `main` branch root. Site goes live at `https://<username>.github.io/<repo-name>/`. See the launch instructions you were sent with this site.

## License

Private / not licensed for redistribution.
