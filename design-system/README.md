# Kroma Design System

Levende dokumentasjon av alle design tokens, typografi og UI-mønstre for Kroma Studio.

## Struktur

```
design-system/
├── kroma-design-tokens.json   ← Kilde til alle tokens
└── README.md
```

## Tokens-fil

`kroma-design-tokens.json` er kilden til alle tre plattformer:

| Plattform | Bruk |
|-----------|------|
| **Webflow** | CSS-variabler via `Kroma Design Tokens`-samlingen |
| **Figma** | Variables i `Kroma Design Tokens`-collection |
| **Kode** | Importer JSON direkte eller generer CSS med script |

## Synk-flyt

```
kroma-design-tokens.json  →  Git (her)
         ↕
      Claude
         ↕
   Figma ←→ Webflow
```

Endringer orkestreres via Claude-dialogen og committes her.

## Token-kategorier

- **color** — 10 fargetokens (ink, warm-white, linen, stone, warm-gray, accent, ++)
- **typography** — 2 skriftfamilier, 9 type-skalaer
- **spacing** — 6 spacing-tokens
- **layout** — max-width, grid, sidebar
- **components** — nav, artwork-card, buttons (4 typer × 6 states), form, footer
- **cms** — Webflow collection-IDer og felt-struktur

## Knappetyper

| Klasse | Beskrivelse |
|--------|-------------|
| `.kroma-btn-primary` | Primær — svart, 18px/36px |
| `.kroma-btn-secondary` | Outline — kantlinje, 16px/24px |
| `.g-nav-cta` | Nav CTA — liten, 10px/22px |
| `.kroma-btn-ghost` | Ghost — underline |

Alle har 6 states: Default, Hover, Pressed, Selected, Disabled, Focus.

## Versjon

**v1.0** — Mai 2026  
Synket: Webflow `joachims-exceptional-site-31862c.webflow.io` · Figma `JJ-RUN`

