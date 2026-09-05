# Mantl SlideBuilder

A Mantl-branded [Slidev](https://sli.dev) starter. Write your slides in Markdown and the Mantl
design system — colours, cards, callouts, the radar watermark, the corner tagline, dark theme and
fonts — is applied automatically. No styling to copy, no design decisions to make.

> Private to Mantl Decision Intelligence. See `LICENSE`.

## Start a new deck

```bash
npm install     # once (downloads Slidev + Chromium for PDF export)
npm run dev     # opens the deck at http://localhost:3030
```

Then edit **`slides.md`**. That's the whole workflow — everything in it is already on-brand.

## Authoring cheatsheet

Slides are separated by `---`. A block of `---` with keys between them sets that slide's layout.
The brand components are available in any slide, no import needed:

```md
# A slide title

<CardGrid :cols="3">
  <Card v-click accent="go"   title="Do this">Recommended, low risk.</Card>
  <Card v-click accent="warn" title="With care">Right, narrow cases only.</Card>
  <Card v-click accent="stop" title="Avoid">The costly path.</Card>
</CardGrid>

<Callout v-click>A highlighted line, in Mantl teal by default.</Callout>
```

| Component | What it is | Key props |
|---|---|---|
| `<Card>` | Coloured container box | `accent` (go/warn/stop/neutral), `title`, `compact` |
| `<NumberedCard>` | Card with a coloured number badge | `accent`, `n`, `title`, `compact` |
| `<CardGrid>` | Lays cards out in a row | `cols` (2 or 3) |
| `<Callout>` | Highlighted strip | `accent` (teal default, or go/warn/stop/neutral) |
| `<Pill>` | Small tag | `accent` (go/warn/stop) |
| `<MantlFooter>` | Mantl lockup pinned to the slide bottom | `right` (email/role), `name`, `tagline`, `fixed` |
| `<Publication>` | Image plate + caption | `img`, `alt`, `caption`, `plate`, `height` |

Add `v-click` to any element to reveal it on the next click; wrap several in
`<v-clicks> … </v-clicks>` to reveal them one at a time.

**Colour language:** green = go / recommended, amber = with care, red = avoid, blue = neutral
framing, teal = emphasis. Keep to it and decks stay consistent.

**Layouts:** `layout: default`, `layout: center` (vertically centred), `layout: section` (divider).
Add `class: dense` to a slide to shrink type so a wide table or busy grid clears the bottom margin.

**Images:** drop the file in this folder and reference it with a leading slash, e.g.
`<Publication img="/cover.png" caption="…" plate />`.

## Export

```bash
npm run build          # static site into dist/
npm run export         # slides.md -> PDF (one page per slide)
npm run export:clicks  # PDF with each click step as its own page
```

The route `http://localhost:3030/?print` also prints to PDF with no extra tooling — in the browser
print dialog, turn **Background graphics on** and set **Margins: None**.

## Customising the brand

All brand values live in `style.css`:

- **Accent colours** — the `.accent-*` rules and the teal used by `.callout`.
- **Watermark** — the `.slidev-layout` background rule (position/size) and `radar.svg` (opacity).
- **Corner tagline** — the `.slidev-layout::after` rule (text, colour, position).

The Mantl footer lockup and its default email live in `components/MantlFooter.vue`.

## Contents

```
slides.md      the deck you edit
components/     Mantl components (Card, NumberedCard, Callout, CardGrid, Pill, MantlFooter, Publication)
style.css       the Mantl design system + watermark + tagline
radar.svg       the watermark mark
```
