---
# Mantl deck defaults — applied to every deck built from this repo.
theme: seriph
title: The Instrumental Method
info: A mechanistic approach to setting goals, defining success criteria, and cutting activity that doesn't earn its place.
class: text-center
transition: slide-left
mdc: true
colorSchema: dark
---

# The Instrumental Method

<div v-click class="text-lg opacity-80 max-w-3xl mt-4">
Why activity isn't achievement — and a mechanistic way to tell the difference, on purpose, every time.
</div>

<!--
FACILITATOR NOTE — the logic underneath this deck, stated once here so it doesn't need
re-explaining slide by slide:

Any institution built to pursue a stated goal has two kinds of activity operating inside it.
CONSTITUTIVE activity is logically entailed by the goal — remove it and the goal becomes
unreachable. DISCRETIONARY activity is imported from habit, culture, prestige, or someone's
previous job — it is not entailed by the goal, which doesn't make it worthless, but it does
mean the burden of proof shifts onto a demonstrated benefit rather than a hoped-for one.

The method is recursive: state the goal in checkable terms, sort every activity by whether
it's logically required to reach it, and for everything discretionary, demand the same three
answers — what benefit, to whom, evidenced how. Two failure modes follow from skipping this:
discretionary activity gets promoted to necessity (sacred cows, cargo-cult process), or
constitutive activity gets demoted to "nice to have" and cut under pressure. This deck is the
teaching template; slides 3–9 get re-populated with each client's own goals, activity audit,
and evidence.
-->

---
layout: default
---

# What this deck covers

<div class="grid grid-cols-2 gap-x-12 gap-y-4 mt-8 text-lg">
  <div class="flex items-center gap-3"><span class="agenda-num">1</span> The symptom: motion vs. progress</div>
  <div class="flex items-center gap-3"><span class="agenda-num">4</span> The discipline: evidence over hope</div>
  <div class="flex items-center gap-3"><span class="agenda-num">2</span> The core distinction</div>
  <div class="flex items-center gap-3"><span class="agenda-num">5</span> Why bad activity survives its own evidence</div>
  <div class="flex items-center gap-3"><span class="agenda-num">3</span> The test, applied</div>
  <div class="flex items-center gap-3"><span class="agenda-num">6</span> Building the goal tree</div>
</div>

<Callout v-click class="mt-8">
This is a template. Everything from slide 3 onward gets re-populated with your goals, your activity, your evidence.
</Callout>

---
layout: default
---

# Motion is not progress

<CardGrid :cols="3">
  <Card v-click accent="stop" title="Full calendars, flat pipeline">Activity has never been higher. The number that matters hasn't moved.</Card>
  <Card v-click accent="stop" title="More dashboards, same conversion">Reporting on the work has scaled faster than the work's effect.</Card>
  <Card v-click accent="stop" title="Headcount up, output flat">Capacity was added. Nobody can say to what it was instrumental.</Card>
</CardGrid>

<Callout v-click accent="warn" class="mt-6">
Activity is not evidence of progress toward a goal. Past a point, it's evidence of the opposite —
an organisation substituting motion for a theory of how the goal gets reached.
</Callout>

---
layout: default
---

# Two kinds of activity

<CardGrid :cols="2">
  <Card v-click accent="go" title="Constitutive">Logically entailed by the stated goal. Remove it and the goal becomes unreachable — not harder, unreachable.</Card>
  <Card v-click accent="warn" title="Discretionary">Not entailed by the goal. Imported from habit, culture, prestige, or someone's previous job. Might still be worth doing — that's a separate, evidenced case.</Card>
</CardGrid>

<Callout v-click class="mt-6">
Every activity in the business is one or the other. Almost no organisation has ever actually sorted them —
which is why "we're busy" and "we're on track" get treated as the same sentence.
</Callout>

---
layout: default
class: dense
---

# The test, applied to any activity

<CardGrid :cols="3">
  <NumberedCard v-click accent="neutral" :n="1" title="State the goal in checkable terms">Not "grow the business" — a number, a date, a way to check it against reality.</NumberedCard>
  <NumberedCard v-click accent="neutral" :n="2" title="Run the entailment test">Would the goal become unreachable without this activity? Not "harder" — unreachable.</NumberedCard>
  <NumberedCard v-click accent="neutral" :n="3" title="Branch on the answer">Yes → constitutive: protect it, resource it, don't cut it under pressure. No → discretionary: it now owes you evidence.</NumberedCard>
</CardGrid>

<Callout v-click accent="go" class="mt-6">
"Not entailed" is not a verdict of "stop." It's a change of burden — from habit to demonstrated benefit.
</Callout>

---
layout: default
---

# The discipline: evidence over hope

<div v-click class="text-lg mt-4 mb-4">For every discretionary activity, demand three answers — not one of them optional:</div>

<CardGrid :cols="3">
  <Card v-click accent="neutral" title="What benefit?">Stated as a checkable outcome, not a feeling.</Card>
  <Card v-click accent="neutral" title="To whom?">Named — the goal, the customer, the team. Not "the business" in the abstract.</Card>
  <Card v-click accent="neutral" title="Evidenced how?">A number that existed before you asked the question, not one invented to answer it.</Card>
</CardGrid>

<Callout v-click accent="stop" class="mt-6">
"It feels important" and "we've always done it" are not answers. A hoped-for benefit is not a benefit.
</Callout>

<Callout v-click accent="warn" class="mt-4">
Watch for the tell: when a metric stops moving, the first move is often to redefine the metric —
not the reality. Renaming what "engagement" means after missing a target isn't progress. It's language
standing in for evidence.
</Callout>

---
layout: default
---

# Why bad activity survives its own evidence

<div v-click class="text-lg mt-4 max-w-4xl">
The pattern repeats everywhere, not just here: an initiative launches on a <strong>hoped-for</strong>
benefit. It gets budget, headcount, a constituency whose role now depends on it existing. When the
evidence comes back mixed or negative, the initiative doesn't stop — the finding gets reframed as
support, and the programme keeps spreading on momentum: constituencies, budgets, sunk cost.
</div>

<Callout v-click accent="warn" class="mt-6">
Sincerity is not a safeguard. Nobody running the initiative needs to be wrong-intentioned for the harm
to be real. The only safeguard is a constitutive requirement: a claim survives on evidence, not belief.
</Callout>

---
layout: default
---

# Two ways this goes wrong

<CardGrid :cols="2">
  <Card v-click accent="stop" title="Doctrine promoted to necessity">A discretionary activity gets treated as sacred — nobody questions the standing all-hands, the weekly status deck, the certification programme — purely because it has always been there.</Card>
  <Card v-click accent="stop" title="Muscle demoted to optional">A genuinely constitutive activity gets cut as "nice to have" under cost pressure — direct customer contact, root-cause QA, the one metric that was actually predictive — because on the org chart it looked like overhead.</Card>
</CardGrid>

<Callout v-click class="mt-6">
Both failures look identical from an org chart. Only the entailment test — run activity by activity — tells them apart.
</Callout>

---
layout: default
class: dense
---

# Building the goal tree

<div v-click class="text-lg mt-2 mb-4">The method applied recursively, top to bottom, until every branch grounds out in something checkable:</div>

<div class="text-base leading-relaxed mt-4">
<div v-click class="mb-2"><Pill accent="go">Level 0</Pill> &nbsp; The market goal, stated in checkable terms (a number, a date)</div>
<div v-click class="mb-2 ml-6">↳ <Pill accent="warn">Level 1</Pill> &nbsp; Sub-goals logically required to reach it — ask the entailment test of each</div>
<div v-click class="mb-2 ml-12">↳ <Pill accent="neutral">Level 2</Pill> &nbsp; Constitutive activities required for each sub-goal — everything else is discretionary by default</div>
<div v-click class="mb-2 ml-16">↳ <Pill accent="go">Level 3</Pill> &nbsp; Success criteria: checkable, evidenced, owned by one name</div>
</div>

<Callout v-click accent="go" class="mt-6">
The recursion stops when a claim grounds out in something you can check against reality — not before.
Anything still floating above that line is an assumption wearing the costume of a plan.
</Callout>

---
layout: center
class: text-center
---

# This is the template. Now make it theirs.

<div v-click class="text-lg opacity-80 max-w-3xl mt-4 mx-auto">
Slides 3–9 get re-populated for every client: their symptom (their actual dashboards), their goal
tree (their actual market goal, decomposed), their evidence audit (their three biggest discretionary
activities, tested live).
</div>

<div v-click class="text-2xl font-bold text-teal-400 mt-8">
A goal only counts as attained when you can point to the evidence — not the effort.
</div>

<MantlFooter />

<!--
============================================================
WORKSHOP MODULE — an add-on, not part of the 10-slide core.
Insert after the closing slide when the session includes a
working exercise. Run after slides 1–10; needs one thing in
advance from the client: their own list of 15–20 recurring
activities/initiatives (standing meetings, programmes,
reports, roles) to bring into the room.
============================================================
-->

---
layout: section
---

# Workshop: stress-test your own activity

---
layout: default
---

# Format

<CardGrid :cols="3">
  <NumberedCard v-click accent="neutral" :n="1" title="90–120 minutes">Small groups of 4–6, one facilitator per group.</NumberedCard>
  <NumberedCard v-click accent="neutral" :n="2" title="Bring your own list">Each team arrives with 15–20 of their real recurring activities — no hypotheticals.</NumberedCard>
  <NumberedCard v-click accent="neutral" :n="3" title="One real goal">Each team picks one actual market goal they're currently accountable for.</NumberedCard>
</CardGrid>

<Callout v-click class="mt-6">
The exercise only works on real activity. A workshop run on hypothetical examples teaches the method
and changes nothing — the whole point is that it's uncomfortable to apply to your own calendar.
</Callout>

---
layout: default
class: dense
---

# Exercise 1 — The entailment sort

<div v-click class="text-lg mt-2 mb-4">20 minutes. Working from their own list of 15–20 activities:</div>

<CardGrid :cols="2">
  <Card v-click accent="go" title="Sort left">Would the stated goal become unreachable without this? → Constitutive.</Card>
  <Card v-click accent="warn" title="Sort right">Everything else. → Discretionary — no verdict yet, just a different pile.</Card>
</CardGrid>

<Callout v-click class="mt-6">
Expect disagreement inside the team. That's the exercise working — the sort forces people to state,
out loud, what they actually believe the goal requires.
</Callout>

---
layout: default
class: dense
---

# Exercise 2 — The evidence audit

<div v-click class="text-lg mt-2 mb-4">30 minutes. For every item in the "discretionary" pile, the team must produce all three answers or flag the item:</div>

<CardGrid :cols="3">
  <Card v-click accent="neutral" title="What benefit?">Stated as a checkable outcome.</Card>
  <Card v-click accent="neutral" title="To whom?">Named, not abstract.</Card>
  <Card v-click accent="neutral" title="Evidenced how?">A number that predates the question.</Card>
</CardGrid>

<Callout v-click accent="stop" class="mt-6">
Anything that can't produce all three in the time box gets flagged "unproven" — not cancelled on the
spot, but moved to someone's desk with a deadline to produce the evidence or lose the activity.
</Callout>

---
layout: default
class: dense
---

# Exercise 3 — Build one goal tree, live

<div v-click class="text-lg mt-2 mb-4">30–40 minutes. Using the one real goal the team picked:</div>

<NumberedCard v-click accent="neutral" :n="1" title="State it in checkable terms">If the team can't, that's the first finding.</NumberedCard>
<NumberedCard v-click accent="neutral" :n="2" title="Decompose to constitutive sub-goals and activities" compact>Level 1 and Level 2 of the tree, built from the actual sort above.</NumberedCard>
<NumberedCard v-click accent="neutral" :n="3" title="Compare to what's currently resourced" compact>Where is headcount and budget actually going, versus where the tree says it must go?</NumberedCard>

---
layout: center
class: text-center
---

# Output: keep / defend / cut

<div v-click class="text-lg opacity-80 max-w-3xl mt-4 mx-auto">
Each team leaves with one page: activities to <strong>keep</strong> (constitutive, protected),
activities to <strong>defend</strong> (discretionary, evidence due by a named date), and activities
to <strong>cut</strong> (discretionary, no case made).
</div>

<Callout v-click accent="go" class="mt-6">
The test isn't finished in the room. It's finished when the "defend" list either produces evidence
or gets cut on schedule.
</Callout>

<MantlFooter />
