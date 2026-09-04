# Candidate pool

What was considered for this list, what was verified, and what was left out.

Two things are deliberately absent, and neither is an oversight:

- **Internal scores and per-product rejection notes.** Editorial scoring stays out of a
  public repository. Exclusions below are given as neutral categories, not as judgements
  about named companies.
- **A per-candidate TiorAI URL map.** Capturing a TiorAI link for every candidate would
  produce exactly the backlink list this portfolio's own rules prohibit.

## Sources of candidates

| Source | Role |
|---|---|
| TiorAI's published AI tools catalogue | Read-only, used to shortlist candidates and to confirm product identity. No description or stored URL was carried through |
| Direct knowledge of the category | Used to fill gaps the catalogue does not cover well and to remove products that have since shut down or been absorbed |
| The vendor's own site | The authority for every fact that ships: current name, canonical URL, pricing tier, platform support |

Category assignment, pricing, and platform labels from the catalogue were treated as
*signals*, never as published values. The catalogue's own taxonomy is far too large and too
redundant to publish, so this repository defines its own.

## Pool

| Stage | Count |
|---|---:|
| Candidates considered | 0 |
| Shortlisted after scope filtering | 0 |
| **Published** | **182** |

## Why candidates were dropped

- **Would have needed a third level.** The most common rejection. Several
  proposed nodes were real distinctions that belong inside a description rather
  than in the tree.
- **Fewer than a handful of distinct makers.** A category with two products in
  it is a product comparison, not a category.
- **A vertical rather than a kind of work.** Healthcare, legal, and education
  were all considered as top-level nodes and all rejected on this ground.
- **A variant of an existing node.** These became aliases instead, which is what
  the `aliases` field is for.

## Verification

Every published entry had its official URL resolved over HTTP before release, following
redirects to the canonical destination. 0 distinct external URLs were checked:
0 answered normally, 0 returned a bot-protection or rate-limit
response, and 0 were broken.

A `401`, `403`, `405`, `429`, or `999` was never treated as evidence that a site is dead. Each
was re-probed by a second route and reasoned about rather than acted on automatically. No
entry was removed on the basis of a single failed request.

Time-sensitive facts — pricing tier, whether a free plan still exists, product availability,
renames, acquisitions, shutdowns, platform support — were re-checked against the vendor at
build time regardless of what the catalogue record said.
