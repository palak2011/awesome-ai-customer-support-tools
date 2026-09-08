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
| **Published** | **39** |

## Why candidates were dropped

- **It could only report a deflection rate.** The largest exclusion, and the
  reason several well-known chatbot products are absent.
- **No published pricing.** Support software is a multi-year decision; a price
  on request is not something a reader can act on.
- **It is a chat widget with no knowledge source.** A text box is not support
  software.
- **It is a feature sold as a product.** Standalone sentiment scoring is the
  clearest case.
- **It belongs to a sibling repository.** Sales tooling stayed in
  `awesome-ai-sales-tools` and store apps in `awesome-ai-tools-for-shopify`.

## Verification

Every published entry had its official URL resolved over HTTP before release, following
redirects to the canonical destination. 43 distinct external URLs were checked:
42 answered normally, 1 returned a bot-protection or rate-limit
response, and 0 were broken. Four entries were removed afterwards, when each link was compared with the address it actually resolves to and the destination turned out to describe a different product; `qa-report.md` names them.

A `401`, `403`, `405`, `429`, or `999` was never treated as evidence that a site is dead. Each
was re-probed by a second route and reasoned about rather than acted on automatically. No
entry was removed on the basis of a single failed request.

Time-sensitive facts — pricing tier, whether a free plan still exists, product availability,
renames, acquisitions, shutdowns, platform support — were re-checked against the vendor at
build time regardless of what the catalogue record said.
