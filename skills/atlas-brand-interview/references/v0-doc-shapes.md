# The two v0 documents Step 3 writes

Step 3 seeds two living docs that sibling skills enrich later. **Match these
shapes exactly** — `atlas-brand-profile` and `atlas-user-profile` expect to fill
these files in, not to rewrite them.

Provenance tags on every claim: **(index)** · **(web)** · **(interview)** ·
**(inferred, unconfirmed)**. Delete sections you have nothing real for.

## Contents

- **1 · `profiles/{brand-slug}/brand-profile.md`**
- **Brand Summary**
- **Brand Context  *(web-sourced at onboarding; index-derived metrics land here on first refresh)***
- **Business Context**
- **Voice & Content Operations**
- **Commerce & channels**
- **Limits & gaps**
- **What this unlocks**
- **2 · `profiles/{brand-slug}/user-profile--{user-slug}.md`**
- **Who they are**
- **First ask**
- **Team & routing map**
- **Tools today & the friction**
- **Cadence policy**
- **Success, as they define it**
- **Config extracted**
- **Worked example**

---

---

## 1 · `profiles/{brand-slug}/brand-profile.md`

Owned long-term by `atlas-brand-profile`. Step 3 writes the research-only v0.

```markdown
# {Brand} — Brand Profile
*Atlas onboarding · {date} · handle: @{handle} · sources: web + interview · index: {present ({N} posts) / discovery started {date}}*

## Brand Summary
{One short prose paragraph: what the brand is, what it stands for, how it
differentiates, what it sells and where. From their own published words plus
anything learned during work. Strategic claims marked *(inferred)* until a
role-appropriate user confirms one in the natural course of work — never via a
dedicated question. NO framework labels — no golden circle, no why/how/what.}

## Brand Context  *(web-sourced at onboarding; index-derived metrics land here on first refresh)*
- Positioning & inferred category: …
- Content presence at a glance: platforms, apparent themes, rough cadence (with links)
- Notable moments: launches, press, viral moments — with sources
- Index status: {in the index (N posts, M analyzed) / discovery started — metrics will fill in}
- Coverage stamps: {N} indexed ({oldest}–{newest}) · {M} analyzed ({P}%) · snapshot {date}

## Business Context
- The 6–12 month outcome and its mechanics: …
- Scale & constraints: … | Seasonal calendar / upcoming moments: …
- Retail & channel relationships: … | Biggest threat: …

## Voice & Content Operations
- Tone of voice: … | Content pillars: …
- Production capacity & approval chain: …
- Owned channels: …

## Commerce & channels
- **Selling through this:** {product names they gave} *(interview)*
- **Creator content in paid:** {yes / no / not sure} *(interview)*
- **Store / commerce data:** not connected *(known-absent)*
- **Ad account:** not connected *(known-absent)*
- **Product catalog, margins, commission ranges, inventory, attribution:** not
  captured — nothing Atlas does today consumes them *(known-absent)*

## Limits & gaps
{Data gaps about the BRAND, framed neutrally: what is not yet measured, what is
web-sourced vs index-sourced, fields needing owner auth. Never framed as Atlas
product limitations or roadmap.}

## What this unlocks
{2–3 questions Atlas can now answer for this brand, each ending in an action}
```

**Channel note.** When Step 2 took the handle-only path, owned metrics (reach,
watch time, saves, audience demographics) are unavailable. Record that here as a
brand data gap — *"owned insights require Meta owner auth"* — not as a complaint
about the product, and do not raise it in conversation unless the user does.

**Known-absent is not the same as unknown.** A field marked *(known-absent)* records
a deliberate decision not to ask, so a future session reads a plan rather than a
gap and does not re-interview the brand for it. When commerce or ads data lands,
these rows are the checklist of what to ask for then.

---

## 2 · `profiles/{brand-slug}/user-profile--{user-slug}.md`

Owned long-term by `atlas-user-profile`. Step 3 writes the v0 stub — role, brand,
relationship, first ask. That is complete for v0; the rest enriches lazily.

```markdown
# {Name} — User Profile ({Brand})
*Atlas onboarding · {date} · role: {role} · relationship: {in-house / agency / owner}*

## Who they are
{Role, what they personally own day-to-day, register/tone to use with them —
a CMO asks different questions than a coordinator; note which this is.}

## First ask
{The job they named, close to verbatim, and what Atlas did about it this session}

## Team & routing map
{Not yet known — atlas-user-profile's P2 probe fills this}

## Tools today & the friction
{Not yet known — atlas-user-profile's P1 probe fills this}

## Cadence policy
{Not yet known}

## Success, as they define it
{If the first ask implied it, record it; otherwise leave for Step 4's 90-day target}

## Config extracted
- Relationship: {in-house | agency | owner} *(inferred from role)*
- {anything else structured that their answer actually held}
```

Leave the unfilled sections **present and labelled**, not deleted. They are the
enrichment skill's checklist, and an empty labelled section is honest where a
deleted one looks answered.

---

## Worked example

`profiles/yough/brand-profile.md` in this project is a real, matured Brand
Profile. It is richer than a Step 3 v0 — it carries index-derived themes, cadence,
top performers with links, and a confirmed positioning correction — but its
provenance tagging, coverage stamps and limits sections are the bar to hit.

The most valuable line in that file is a **correction**: Atlas guessed the brand
competed with Caulipower and Banza in the frozen-pizza aisle; the brand said no,
they compete with Quest and Legendary for the macro-tracking customer. Every
downstream search changed as a result.

That is what these files are for — not storing what Atlas already knew, but
capturing where it was wrong.
