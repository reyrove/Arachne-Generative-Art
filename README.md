# Arachne — Generative Art

> A seed-based generative system for rotating ring compositions.  
> A reproducible catalogue of computational textile compositions.

---

## What is this?

**Arachne** is a generative design system that layers rotating bands of tiled pixels into concentric rings. Where the rings intersect, a moiré interference emerges — a woven surface that is neither fully planned nor fully random, but **emergent**.

Every artwork in this catalogue is defined by a single numeric seed. The same seed always produces the identical composition — making each piece **traceable, reproducible, and licensable** across textile, print, and apparel applications.

Named for the weaver of Greek myth — the mortal who rivalled a goddess and was transformed into a spider — **Arachne** translates that myth into code.

---

## Live

🌐 **[View the catalogue →](https://reyrove.github.io/Arachne-Generative-Art/)**

---

## The System

The generator combines two layers:

| Layer | Description |
|-------|-------------|
| **Ring bands** | Concentric discs of tiled pixel-patterns, each rotated at its own speed. |
| **Moiré interference** | Where rings overlap, an emergent pattern forms — the visual signature of the system. |

Both layers are driven by the same seed, ensuring deterministic output.

### Parameters

- **Ring count** — 5 to 15 concentric bands
- **Tile size** — derived from canvas scale
- **Rotation speeds** — from `-5` to `+5`, chosen per ring
- **Color palette** — randomized RGB per tile

---

## Structure

```
Arachne-Generative-Art/
├── index.html          ← Full catalogue (single-file)
├── images/
│   ├── fav.svg
│   ├── arachne-tote.png
│   ├── arachne-tee.png
│   └── arachne-cushion.png
└── README.md
```

The entire project is contained in a single `index.html` — no build step, no dependencies, no framework. Open it in any modern browser.

---

## Features

- **Seed-based generation** — every composition is deterministic and reproducible
- **Live catalogue** — cover, plate, surfaces, process, archive, commission sections
- **Multiple surfaces** — print, scarf, textile, wallpaper — all rendered from the same seed
- **Archive of 8 seeds** — click any plate to load it into the main view
- **PNG export** — download any composition directly from the browser
- **Keyboard shortcuts** — `R` for new seed, `S` to save
- **Legal modal** — licensing, terms, and credits built in
- **Responsive** — works on desktop, tablet, and mobile
- **Mobile-first navbar** — horizontally scrollable with fade hint

---

## Usage

### Generate a new composition

Click **New Seed** or press `R`.

### Download the current composition

Click **Download** or press `S`.

### Load a seed from the archive

Click any plate in the **Archive** section.

---

## Color System

Each ring is assigned a randomized tile palette drawn from:

- **Tile background** — RGB values with a bias toward deep tones
- **Tile stroke** — a matching line drawn inside each tile
- **Background gradient** — soft cool tones across the canvas

Each seed selects a unique combination — no two compositions share the same palette.

---

## Technical Notes

- Pure vanilla JavaScript — no libraries
- Canvas 2D rendering
- Custom xorshift random generator for deterministic seeds
- Device-pixel-ratio aware rendering
- Per-ring offscreen tile pre-rendering for performance

---

## About

**Arachne** is a project by [Reyhaneh Daneshdoost](https://reyrove.github.io/) — an Iranian-born artist working at the intersection of classical textile logic and generative systems.

The work begins with a simple observation: the woven surface — repetitive, mathematically structured, infinitely variable — has always been a form of computation, long before computers.

**Arachne** is an attempt to render that logic visible.

> *A spider spins without a plan — yet every web is structurally perfect.*

---

## Licensing

All compositions are seed-documented and available for licensing across textile, surface, and apparel applications.

For commercial use, custom editions, or exclusive rights:

📧 **reyhanehdaneshdoost@gmail.com**

See the **Licensing** section in the live catalogue for details.

---

## Links

- 🌐 [Website](https://reyrove.github.io/)
- 📷 [Instagram](https://www.instagram.com/rey._.rove/)
- 💼 [LinkedIn](https://www.linkedin.com/in/reyhaneh-daneshdoost-730481160/)
- 🐦 [X](https://x.com/reyrove)

---

## Credits

**Design & Generative System**  
Reyhaneh Daneshdoost

**Typefaces**  
Cormorant Garamond · DM Mono

**Edition**  
Arachne — Autumn 2026

---

<p align="center">
  <em>Computational Textile Design</em><br />
  <sub>© Reyrove Studio · All compositions reproducible by seed</sub>
</p>