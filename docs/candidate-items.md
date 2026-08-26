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
| Candidates considered | 282 |
| Shortlisted after scope filtering | 131 |
| **Published** | **94** |

## Why candidates were dropped

- **Wrong repository.** Developer, marketing, and SEO tools were moved to the repositories that exist for them rather than padding this one.
- **Requires a new habit to pay off.** The most common quiet failure: a tool that works only if you remember to open it. Several well-regarded products were dropped on this alone.
- **A chat box in a familiar wrapper.** Adding an assistant panel to an existing product is not by itself a productivity feature.
- **Enterprise-only rollouts.** Excluded where nobody can evaluate the product without a procurement process, unless it is significant enough that a reader should know it exists.
- **Shut down during this build.** Height closed its project management product in September 2025. It was shortlisted, verified, and dropped rather than shipped as a dead link.
- **Pivoted away.** Several presentation and notes products moved into sales or enterprise search during the past two years and no longer serve this audience.
- **Category already well covered.** Meeting transcription in particular could have filled thirty slots with barely distinguishable products.

## Verification

Every published entry had its official URL resolved over HTTP before release, following
redirects to the canonical destination. 94 distinct external URLs were checked:
86 answered normally, 8 returned a bot-protection or rate-limit
response, and 0 were broken.

A `401`, `403`, `405`, `429`, or `999` was never treated as evidence that a site is dead. Each
was re-probed by a second route and reasoned about rather than acted on automatically. No
entry was removed on the basis of a single failed request.

Time-sensitive facts — pricing tier, whether a free plan still exists, product availability,
renames, acquisitions, shutdowns, platform support — were re-checked against the vendor at
build time regardless of what the catalogue record said.
