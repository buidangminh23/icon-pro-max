# Icon Pro Max

**The single source of truth for every icon on [example.com](https://example.com).**

A Claude Code / Codex / Gemini skill that catalogs every icon the Personal Web
ships — with the exact asset path, React component, canonical size, brand color,
render recipe, and accessibility rule for each — plus an anti-slop checklist so an
agent never redraws a logo, recolors a brand mark, distorts an aspect ratio, or
re-inlines a duplicated icon.

## What's inside

| Group | Count | Render style |
|-------|:---:|--------------|
| **Payment methods** | 6 (+2 variants) | white badge wrapper, per-logo height (`PaymentLogos.tsx`) |
| **QR codes** | 2 static + VietQR dynamic | raster image / `qrUrl()` |
| **Social & app brand** | 6 (GitHub, LinkedIn, Facebook, Telegram, Zalo, Gmail) | `currentColor` inline SVG + brand SVG (`SocialIcons.tsx`) |
| **UI icons (lucide-react)** | ~70 in use | `lucide-react`, `currentColor`, sized by class |
| **Tech-stack logos** | 50 | brand-colored SVG files |
| **Site & brand** | 9 | favicons, app icons, OG, avatar, BIMI |

All brand assets are mirrored, self-contained, under
[`skills/icon-pro-max/assets/`](skills/icon-pro-max/assets/) so the catalog is
usable outside the web repo.

## Install

Add to a project's skill lockfile (source `buidangminh23/icon-pro-max`,
skill path `skills/icon-pro-max/SKILL.md`), or drop the folder into a
Claude Code / Codex / Gemini plugin marketplace.

## The one rule

> An icon carries a brand's identity. **Reproduce it exactly — never redraw,
> recolor, or restretch a logo.** Generic UI glyphs (lucide) are the only icons
> you may freely restyle.

See [`SKILL.md`](skills/icon-pro-max/SKILL.md) for the full catalog, render
recipes, the anti-slop checklist, and the add-an-icon procedure.

## License

MIT for the skill text and structure. Bundled third-party brand marks under
`assets/` remain the property of their respective owners and must not be
modified — see [`LICENSE`](LICENSE).
