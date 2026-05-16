# After Expiry Developer Notes

This is a static prototype for the band website. It is intentionally small: HTML, CSS, images, and no runtime JavaScript.

## What This Site Is

- `index.html` is the main one-page band site.
- `about.html` is a simple secondary page from the original scaffold. It is not the main prototype surface.
- `assets/css/style.css` owns the visual design.
- `assets/img/original/` preserves source assets.
- `assets/img/brand/` contains human-readable copies for design use.
- `assets/img/working/` contains derived working assets, currently transparent alien PNGs made from the checkerboard exports.

## Current Design Direction

The prototype uses the original IA:

1. Header
2. Hero
3. After Expiry?
4. Music
5. Social
6. Merch
7. Footer

The visual language comes from the supplied artwork: aqua sky, sand, burnt orange, black sigil, and alien band members. The header keeps the real AE sigil. The hero title is real text styled with a blackletter web font, not the black logo image.

## JavaScript Policy

There is no runtime JavaScript in the site. The previous inline copyright-year script was removed.

The only iframe is the YouTube embed in the Music section. Console messages from browser extensions or Codex browser tooling may mention iframe observation; that is not site JavaScript.

## Local Development

Install tooling once:

```bash
npm install
```

Run the local static server:

```bash
npm run serve
```

Open:

```text
http://localhost:8080
```

## Quality Checks

Run all checks:

```bash
npm run lint
```

That runs:

- `htmlhint` on the HTML files
- `stylelint` on CSS
- `prettier --check` on text files

Format files:

```bash
npm run format
```

## Responsive And Accessibility Notes

- Phone support is a priority. The nav wraps instead of disappearing.
- Buttons meet a 44px minimum tap target.
- The YouTube iframe has a descriptive title and lazy loading.
- Keyboard users get visible focus states.
- A skip link is present for keyboard/screen-reader users.
- The page avoids runtime animation, and reduced-motion safeguards are in CSS.

## Prototype Guardrails

- Preserve original assets; do not overwrite them.
- Use derived assets in `assets/img/working/` when needed.
- Avoid image generation or image manipulation unless explicitly agreed.
- Keep changes small and preview them locally before committing.
- Commit coherent checkpoints to `dev`.
