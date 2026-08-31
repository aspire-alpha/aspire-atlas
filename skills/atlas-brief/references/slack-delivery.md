# Sending the brief to Slack

**Slack is handled through the user's own connection.** This plugin declares no
Slack server and holds no credentials — it uses whatever Slack tool the session
already has. If none exists, say Slack isn't connected and offer the link instead.
Do not offer to set it up; that is not this skill's job.

## The three rules

### 1 · Confirm the destination and the text, every time

**A Slack post is visible to colleagues and cannot be recalled.** Show exactly what
will be posted and exactly where, then wait for a yes.

> I'd post this to **#creator-team**:
>
> *"Three things this week — the gap narrowed, Halo & Hearth signed two creators
> who've posted about us unpaid, and one partner tripped the standard. Brief:
> {link}"*
>
> Send it?

**No blanket permission.** "Yes, always post to #creator-team" still gets the text
shown each time, because the text is the part that can embarrass someone.

### 2 · Never guess the channel

Ask. A brand's competitive intelligence, a creator risk flag, or a partner's name
landing in the wrong channel is a real harm — reputational for them, and for
Aspire.

If they name a channel you can't verify exists, say so rather than posting
hopefully. If they say "the usual", ask which one; a remembered channel from a
previous session is still worth confirming, because channels get archived and
people change teams.

### 3 · Send the nudge, not the document

Three or four lines: the headline item, and the link. The page carries the detail.

**Why:** a wall of text in Slack gets scrolled past, and the brief's job is to pull
someone to the page where the evidence lives. Pasting the whole thing defeats both.

## Message shape

```
{One line: the most consequential thing, with the number}
{One line: the next two, compressed}
{The link}
```

> Gap narrowed — @mornings.with.dez's routine post saved 4,100, your best creator
> post yet.
> Also: Halo & Hearth signed two of your unpaid advocates, and @theshelfedit tripped
> the health-claims standard.
> Full brief → {link}

No emoji unless they use them first. No "Hi team". No engagement bait.

## A canvas instead?

A Slack canvas suits content meant to live in a channel and be edited — a standing
reference. **The brief is not that**: it changes every edition and already has a
permanent home at its own link.

Offer a canvas only if they ask for one, and if they do, put the *current* edition
in it and link the page for history. Never maintain both as separate sources of
truth.

## Never post in test or demo mode

Slack is externally visible, which makes posting a write in every sense that
matters — and unlike a config change, it reaches people. Say what would have gone
and where, then stop.

In a **demo**, this is a strength rather than a limitation: *"and this is where I'd
drop it in your team's channel — want to see the message?"* shows the workflow
without posting anything into a prospect's workspace.

## When Slack isn't connected

Say it once, plainly, and move:

> Slack isn't connected here, so the link is what I've got. Someone on your side
> can connect it whenever.

Do not treat it as an error, do not offer setup instructions, and do not raise it
again in later editions.
