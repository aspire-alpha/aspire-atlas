# Publishing the snapshot as a visual artifact

Step 4b of `atlas-alignment-snapshot`. The written snapshot is the record; this page
is the thing a brand actually looks at, comes back to, and shows their team.

## Contents

- **What the page must do** — the bar it has to clear before you publish
- **One artifact per brand, updated in place** — why the URL must stay stable
- **Capabilities — what is worth declaring** — and what to leave off

---

**The aha is a visual moment. Markdown in a chat window undersells it.**

After writing the doc, publish the snapshot as a designed HTML page with the
Artifact tool. The markdown doc is the record; the artifact is the thing the brand
actually looks at, comes back to, and shows their team.

**Load `artifact-design` before writing the page — always.** Load `dataviz` too if
the page charts anything. Both are mandatory reads, not suggestions.

⚠️ **In demo mode, publishing is not optional.** The page *is* the demo — a link
they can open on their phone in the taxi is worth more than anything said out loud.
This is the **one** action demo mode permits: it is an outbound artifact carrying
the fixture brand's name, not a state write, so it does not contradict the block
below — see
`${CLAUDE_PLUGIN_ROOT}/skills/atlas-session-mode/references/write-boundaries.md`.
It never carries a real brand's name.
There is a worked example at
`${CLAUDE_PLUGIN_ROOT}/skills/atlas-session-mode/references/demo-snapshot-example.html`
built from the Northwind fixture: gap as an italic serif hero, the three panels
sharing one rule so they read as one instrument, the 4.1× as a hero number rather
than a chart, and the un-screened creator visibly flagged. Match that bar.

**A note on the numbers:** a ratio like 4.1× is a **single headline figure**, so it
belongs as a hero number, not a bar chart. If you do chart something, the three
panel colours are a validated categorical set — blue / amber / green, in that
order, each also directly labelled so identity is never carried by colour alone.

### What the page must do

- **The gap is the hero.** It opens the page, set large. The three panels sit
  beneath it as evidence. Never bury the gap below three tidy columns.
- **Three panels, visibly one system** — SAY, SHOW, RESPOND read as a single
  instrument, not three unrelated cards.
- **Every number links to its post.** The link is the product; a figure without
  one is what Atlas exists to replace.
- **Provenance is visible, not buried.** Web-sourced material is marked on the
  face of the page, with its platform named. Unanalyzed creators carry a flag.
- **Coverage stated honestly**, denominated against actual media count.
- **Three creators as a real table** — handle, why aligned, evidence, analyzed.

### One artifact per brand, updated in place

**Publish to the same URL each time.** Record the artifact URL in
`alignment-targets.md` so future sessions update rather than fork. This is the
retention mechanic: the second snapshot shows whether the named gap **widened or
closed**, and that delta is worth more than the first snapshot was. A new URL per
snapshot throws that away.

### Capabilities — what is worth declaring

Default to a **static page with no capabilities.** It is shareable, needs no
consent, and the aha does not depend on interactivity.

| Want | Declare | The catch |
|---|---|---|
| The brand ticks off creators they have contacted, and it persists for everyone | `{artifact: {}}` | Page must re-publish itself on each change; read-only viewers need a read-only render |
| A genuinely live page that re-queries the index | `{mcp: {...}}` | **A page declaring `mcp` cannot be shared publicly** — and most brands want to share this internally. Also requires a real observed request/response pair per tool before publishing. Do not guess argument shapes. |
| Viewer saves the snapshot as a file | `{downloads: true}` | Minor; the markdown doc already covers this |

Load `artifact-capabilities` before declaring anything. **Never declare `mcp` on a
snapshot the brand is expected to share** — losing shareability costs more than
live data buys, and the doc plus a republish already keep it current.
