# samuel-g-smith.github.io

Personal site — a single static page: name, role, and links out to GitHub,
LinkedIn and [needapc](https://needapc.vercel.app).

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole page — header, links, footer |
| `style.css` | Light theme, monospace type, framed panels, accent palette |
| `.nojekyll` | Tells GitHub Pages to serve the files as-is |

## Local preview

```sh
python3 -m http.server 8000
# then open http://localhost:8000
```

## Editing

- **Links** live in the `<ul class="links">` block in `index.html` — each row is
  a `<li>` with a `label` (shown in bold) and a `target` (the muted URL text).
- **Colours** are CSS custom properties at the top of `style.css`. `--paper`,
  `--panel` and `--ink` set the ground; `--rust`, `--blue` and `--violet` are
  the three accents, each paired with a `*-tint` used for panel shadows and
  link hover backgrounds. Each link row picks its accent via the `--c` /
  `--c-tint` pair set on its `li` (`.link--gh`, `.link--li`, `.link--pc`).
