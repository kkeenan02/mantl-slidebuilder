---
# Mantl deck defaults — applied to every deck built from this repo.
theme: seriph
title: Your deck title
info: A Mantl-branded presentation. Edit this file; the brand is applied automatically.
class: text-center
transition: slide-left
mdc: true
colorSchema: dark
---

# Your Deck Title

<div v-click class="text-lg opacity-80 max-w-3xl mt-4">
A one-line description of what this deck is about.
</div>

<!--
Speaker notes go here. Everything on this slide is Mantl-branded by default:
the radar watermark, the corner tagline, the dark scheme, and the fonts.
-->

---
layout: default
---

# Agenda

<div class="grid grid-cols-2 gap-x-12 gap-y-4 mt-8 text-lg">
  <div class="flex items-center gap-3"><span class="agenda-num">1</span> First topic</div>
  <div class="flex items-center gap-3"><span class="agenda-num">4</span> Fourth topic</div>
  <div class="flex items-center gap-3"><span class="agenda-num">2</span> Second topic</div>
  <div class="flex items-center gap-3"><span class="agenda-num">5</span> Fifth topic</div>
  <div class="flex items-center gap-3"><span class="agenda-num">3</span> Third topic</div>
  <div class="flex items-center gap-3"><span class="agenda-num">6</span> Takeaway</div>
</div>

---
layout: section
---

# A section divider

---
layout: default
---

# Colour-coded cards

Use `<Card>` with an accent, and `<CardGrid>` to lay them out. They reveal one at a time.

<CardGrid :cols="3">
  <Card v-click accent="go" title="Green — do this">The recommended, low-risk option.</Card>
  <Card v-click accent="warn" title="Amber — with care">Fine in the right, narrow cases.</Card>
  <Card v-click accent="stop" title="Red — avoid">The costly or unreliable path.</Card>
</CardGrid>

<Callout v-click class="mt-6">
Use <code>&lt;Callout&gt;</code> for a highlighted line. It defaults to the Mantl teal.
</Callout>

---
layout: default
class: dense
---

# Numbered cards, pills, and a footer

<CardGrid :cols="3">
  <NumberedCard v-click accent="neutral" :n="1" title="Point one">A short line, with an example beneath.</NumberedCard>
  <NumberedCard v-click accent="warn" :n="2" title="Point two">A short line, with an example beneath.</NumberedCard>
  <NumberedCard v-click accent="go" :n="3" title="Point three">A short line, with an example beneath.</NumberedCard>
</CardGrid>

<div v-click class="flex gap-2 mt-5">
  <Pill accent="go">High</Pill>
  <Pill accent="warn">Medium</Pill>
  <Pill accent="stop">Low</Pill>
</div>

<MantlFooter />

---
layout: center
class: text-center
---

# Closing

<div v-click class="text-2xl font-bold text-teal-400 mt-6">
Your one-line takeaway.
</div>

<MantlFooter />
