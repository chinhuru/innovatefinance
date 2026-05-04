# &lt;Innovative Finance&gt; — Website

A static, multi-page marketing site. No build step. No frameworks. Just HTML, CSS, and a tiny bit of JavaScript.

## Pages

| File | Purpose |
| --- | --- |
| `index.html` | Home — positioning, two pillars, who we serve |
| `philosophy.html` | Philosophy & offering — four dimensions, methodology, both pillars in detail, landscape |
| `about.html` | About — founders, board of advisors, team intent |
| `thinking.html` | Thought leadership — articles list (placeholder) |
| `resources.html` | Public tools — models, frameworks, external reading (placeholder) |
| `404.html` | Not-found page |

## Editing content

- **Founder bios:** `about.html`, search for `[Bio placeholder`
- **Advisor cards:** `about.html`, search for `[Advisor name]`
- **Articles:** `thinking.html`, search for `[Article title placeholder`
- **Resources:** `resources.html`, search for `placeholder`
- **Contact email:** every page uses `hello@example.com` — find/replace globally

## Brand tokens

All colors, fonts, and spacing rules are CSS variables defined at the top of `styles.css`. To adjust the palette, edit the `:root` block.

## Hosting on GitHub Pages

Push the repo to GitHub, enable Pages on the `main` branch root. Site goes live at `https://<username>.github.io/` (or `/<repo-name>/` if not using the special username repo naming).

## License

Private / not licensed for redistribution.
