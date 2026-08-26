# samuel-g-smith.github.io

Personal site — a single static page: name, role, and links out to GitHub,
LinkedIn and [needapc](https://needapc.vercel.app).

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole page — header, links, footer |
| `style.css` | Light theme, monospace type, box-drawing frames |
| `.nojekyll` | Tells GitHub Pages to serve the files as-is |

## Local preview

```sh
python3 -m http.server 8000
# then open http://localhost:8000
```

## Editing

- **Links** live in the `<ul class="links">` block in `index.html` — each row is
  a `<li>` with a `label` (shown in bold) and a `target` (the muted URL text).
- **Colours** are CSS custom properties at the top of `style.css` (`--bg`,
  `--ink`, `--accent`, …); changing those restyles the whole page.
