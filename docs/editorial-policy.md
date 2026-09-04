# Editorial policy

The rules this repository is built and maintained by. The README's
"How categories are selected" section is the short version; this is the full one.

## Scope

A two-level tree of the kinds of work AI tools are bought to do, with the top
level matching the twenty categories used by the TiorAI AI tools dataset so the
two remain compatible.

## What qualifies

- It answers a question people actually arrive with, in the words they use.
- At least a handful of distinct products would sit in it, from different makers.
- It is a kind of work, not a kind of customer and not a kind of technology.
- There is enough public information to describe it accurately.
- It covers something the entries already in that category do not.

## What does not

- A third level. Two is the whole design; a third produces nodes with one
  member and a judgement call on every new tool.
- Categories named after a single product or vendor.
- Industry verticals. A tool sold to hospitals is still a transcription tool.
- Marketing phrases with no settled meaning, however often they appear on
  homepages.
- Spelling and abbreviation variants of a node that already exists. Those are
  aliases, and adding one to the right node is a genuinely useful contribution.
- Broken, parked, or login-walled sites with no public information.
- Products that have shut down or been folded into something else.
- Affiliate landing pages, coupon sites, and lead-capture funnels.
- Near-identical clones with no meaningful difference from something already listed.
- Anything whose main activity is clearly illegal, and NSFW-focused products.
- Anything submitted purely as a promotional exercise.

## Descriptions

One sentence, 8 to 25 words, 35 at the absolute maximum, ending in a full stop. Written for
this repository rather than adapted from a vendor's homepage, and rewritten if a neighbouring
entry could swap places with it unnoticed.

Banned outright: superlatives (*best*, *leading*, *revolutionary*, *cutting-edge*,
*game-changing*, *world-class*, *ultimate*, *powerful*, *seamless*, *unleash*), `AI-powered`
as an opening, unverifiable claims about users, funding, or awards, and the em dash inside a
description, which is reserved as the entry separator so the format stays machine-parseable.

## Metadata vocabularies

Closed sets. A term outside them is a defect, not a judgement call.

**Pricing** — at least one, at most two, in this order:
`Free` · `Freemium` · `Paid` · `Open Source` · `Free Trial`

`Open Source` means an OSI-approved licence. Source-available products do not get the label;
the description says "source-available" instead. `Free Trial` never appears alone.

**Platform** — zero to six, in this order:
`Web` · `Windows` · `macOS` · `Linux` · `iOS` · `Android` · `API` · `CLI` ·
`Browser Extension` · `VS Code` · `JetBrains` · `Discord`

Applied only where verified. A wrong label is worse than a missing one.



## Ordering

Alphabetical within a category, ignoring punctuation and a leading "The". Position carries no
meaning and there is no paid placement.

Between categories, the order is editorial, by expected reader interest. That ranks topics,
never products.

## Categories

Minimum 4 entries, 8 is the working target, roughly 15 is the ceiling. A category that cannot
reach 8 strong entries is merged or dropped rather than padded. No subcategories.

The taxonomy is revisited when a category drops below 6 entries, passes 15, or starts
receiving the same submissions as its neighbour.

## Links

The primary link is the resource's own official site: canonical, HTTPS, no tracking
parameters, no affiliate parameters, no shortener, no directory listing, no review page.

TiorAI links are capped: at most 25% of entries carry one, all distinct, at most three per
category, maintainer-placed only. Contributors are asked not to add them.

## Removal

An entry is removed when the product shuts down, the domain is taken over or starts serving
something harmful, the listing turns out to be misleading, or the entry no longer meets the
scope above. Removals are recorded in [CHANGELOG.md](../CHANGELOG.md). An entry removed for
a safety reason goes through review again rather than being quietly restored.
