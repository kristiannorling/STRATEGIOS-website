# strategios-website

Public-facing Quarto website for STRATEGIOS research program. Hosted at strategios.se.

## Purpose

Curated analyses and tools from STRATEGIOS made accessible to practitioners and the public. Bilingual Swedish/English.

## Structure

```
website/
├── _quarto.yml          # Site config
├── index.qmd            # Landing page (bilingual)
├── about.qmd            # About STRATEGIOS
├── analyses/            # Published analyses from subprojects
│   └── blai/            # Language complexity analysis
├── tools/               # Practitioner tools
│   └── strategitavlan.qmd
└── _site/               # Generated output (gitignored)
```

## Workflow

1. Write/update `.qmd` files
2. `quarto preview` for local development
3. `quarto render` to build
4. `git push` to GitHub
5. Pull from cPanel at Oderland

## Design

Uses STRATEGIOS brand identity:

- Inter typeface
- Black/white high contrast
- Generous whitespace
- Clean tables and figures

See `custom.scss` for theme customization.

## Adding analyses

1. Create folder in `analyses/` (e.g., `analyses/dna-i/`)
2. Add `index.qmd` with content
3. Update navbar menu in `_quarto.yml`
4. Render and push

## Content sources

Analyses are adapted from STRATEGIOS subprojects:

- BLAI → `../../CORPUS/BLAI/`
- Strategitavlan → `../../STRATEGITAVLAN/`

Keep website content self-contained (copy, don't symlink).

## Git Remote

```bash
git remote -v
# origin https://github.com/kristiannorling/STRATEGIOS-website.git
```
