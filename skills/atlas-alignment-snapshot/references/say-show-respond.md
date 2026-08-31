# Building the three panels from real fields

Targeted reads only — the narrowest queries that answer today's question. Every
claim links to the post behind it.

## Contents

- **SAY — what the brand claims**
- **SHOW — what the market shows**
- **RESPOND — what people react to**
- **Sequencing so it lands**

---

---

## SAY — what the brand claims

**Sources:** their own account (`fetch_account`), their own posts
(`search_posts` filtered to `author.username`), the site and press already
captured in `brand-profile.md`.

| Read | How |
|---|---|
| Content themes & aesthetics | Aggregate over own posts — **normalize casing first** |
| Cadence | Posts per week since the last meaningful moment |
| Own hashtags | Ranked; an empty result is a finding, not a failure |
| Stated positioning | From `brand-profile.md` — flag if `(inferred, unconfirmed)` |

⚠️ **Normalize aesthetic-tag casing before counting.** `Modern` and `modern` are
one theme, and a known case-split defect will otherwise split it in two and rank
both halves too low to appear.

⚠️ **Positioning may be wrong on file.** Yough's profile guessed the frozen-pizza
aisle; the brand competed with Quest and Legendary for the macro-tracking
customer. If SAY rests on an unconfirmed inference, the whole gap may be
mis-aimed — mark it and let the mirror invite the correction.

---

## SHOW — what the market shows

**Sources:** `search_posts` for mentions and tags of the brand handle,
`search_accounts` / `fetch_account` on the creators found,
`search_creator_marketplace` for category whitespace.

| Read | How |
|---|---|
| Who posts about them | Repeat mentions are signal; a single tag is noise |
| What that content shows | Themes in creator content **vs** the brand's own themes — the divergence is usually the gap |
| Whether it's analyzed | `analyzedAt` per post. Unanalyzed ≠ clean |
| Category whitespace | Creators making content the buyer watches, without mentioning the brand |

**Exclude the brand's own posts** when searching its name in text — their own
marketing mentions themselves and will pollute the panel. Filter `author.username`.

**Exact-match fields return a silent zero on casing mismatch.** A zero on
`pastBrandPartnershipPartners` means *check the casing variants* before it means
"none".

### The web-research bridge (empty or thin SHOW)

Search the open web for creator activity on platforms not yet live in the index.
**Label every web-sourced claim with its platform and mark it web-sourced.**

Rules:
- Name the platform explicitly — *"TikTok, web-sourced"*, never a bare number.
- Never present web-sourced reach beside index-measured engagement as if they were
  the same instrument.
- Frame the limit as a **brand data gap**, not as Atlas roadmap: *"this activity is
  TikTok-native and web-sourced here"* — never *"we don't support TikTok yet."*
- Check what platform coverage is actually live before describing any as missing.
  Coverage is expanding.

If web research also finds nothing, the absence becomes the finding — and the
panel fills with category whitespace instead.

---

## RESPOND — what people react to

⚠️ **State the panel's scope on its face.** This measures **attention, not
conversion.** Say so in the panel itself — one clause is enough:

> RESPOND · what people react to *(attention — I can't see your store)*

Without that, "responds 4× more" reads as a sales claim, and the brand will make a
revenue decision on an engagement number. If Step 2 recorded what they sell, use
the product names here so the panel is specific about what it *is* measuring
attention toward.

**Sources:** engagement on their own and partner content, relative to their own
baseline.

| Read | How |
|---|---|
| What over-performs | Ratio to the brand's own median, not raw counts |
| What the winners share | Retail news? Community prompts? Product shots? Name the pattern |
| Trend line | Comment volume where likes are withheld — Yough had likes hidden on 45 of 101 posts |
| Creator-side response | Post performance vs **that creator's** baseline, never vs the brand's |

**Not available — do not imply otherwise:**

- **Comment text mining / purchase intent** — comments are not persisted. Check
  what sentiment fields actually exist before citing any; never infer intent.
- **Audience demographics** — **conditional.** Null for many accounts, fully
  populated for others (Minted: age, gender, city, country). Read the field
  before saying it is unavailable.
- **Audience authenticity / pod detection** — no signal exists.
  ⚠️ `vibeAnalysis.authenticityScore` scores **content** authenticity. Never
  present it as an audience or follower-quality signal.
- **Revenue, conversion, ROI** — the store and ad account are not connected. RESPOND is reaction, not sales. Say it that way to the brand, never as an empty field.

---

## Sequencing so it lands

1. **SAY first** — familiar ground, establishes Atlas read their work properly.
2. **SHOW second** — the first thing they cannot see themselves.
3. **RESPOND third** — where the surprise usually is.
4. **Then the gap.** It should feel earned by the three panels above it.

Do not open with the gap. It reads as a claim before it reads as a finding.
