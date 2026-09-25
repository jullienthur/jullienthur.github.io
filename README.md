# Portfolio

My personal portfolio website showcasing interests and projects.

Inspired by [astro-theme-cactus](https://astro-cactus.chriswilliams.dev/) :)

## Development branch

The `development` branch is the design workspace. The site is plain HTML, CSS, JavaScript, and Markdown served from `docs/`; no build tool is required. `docs/development.css` contains the current visual exploration, leaving the original stylesheet available for comparison.

To preview locally from the repository root:

```powershell
python -m http.server 8765 --directory docs
```

Open <http://localhost:8765/>. A local server is needed because the page loads its Markdown sections with `fetch()`.

## Cloudflare Pages setup

This repository can be connected to Cloudflare Pages with these settings:

| Setting | Value |
| --- | --- |
| Production branch | `master` until the new design is ready |
| Preview branch | `development` |
| Root directory | repository root |
| Build command | `exit 0` |
| Build output directory | `docs` |

Cloudflare Pages can create preview deployments for branch changes. If the site later needs server-side features, add Pages Functions under a root-level `functions/` directory; a specific function should be designed around the feature it serves.
