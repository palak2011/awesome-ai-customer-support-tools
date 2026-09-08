# QA report

Result of the release checks for version 1.0.0, run on 2026-08-22.

## Summary

| Check | Result |
|---|---|
| Entries | 43 across 7 categories |
| Required files | Present |
| Issue forms parse against GitHub's schema | Pass |
| README section order and canonical names | Pass |
| Contents block — every section listed, every anchor resolves | Pass |
| Entry format on every entry | Pass |
| Alphabetical ordering within every category | Pass |
| Duplicate names | None |
| Duplicate URLs | None |
| Pricing and platform labels within the vocabularies | Pass |
| Description length and quality rules | Pass |
| TiorAI link budget | 0 deep links, 0.0% of entries (cap 25%) |
| External links checked | 43 |
| **Broken links** | **0** |
| Secret and credential scan | Clean |
| Internal URL and local path scan | Clean |

## Categories

| Category | Entries |
|---|---:|
| Help desks | 8 |
| Resolution agents | 6 |
| Voice and phone support | 6 |
| Knowledge bases | 4 |
| Quality and coaching | 5 |
| Workforce and operations | 7 |
| Support for small teams | 7 |

Every category holds at least 4 entries, and none exceeds the ceiling of roughly 15.

## Link checking

Method: browser user agent, redirects followed to a depth of 8, 12-second connect and
30-second total timeout, at least 400ms between requests to the same host, single flight per
host, `HEAD` first with a `GET` fallback.

- **Answered normally:** 42
- **Bot protection or rate limit:** 1
- **Broken:** 0

Hosts that challenged the checker: `www.ada.cx`.

None is treated as dead. A challenged host was re-probed by a second route, normally the bare
origin and then `robots.txt`. A challenge response says the host declines automated requests;
it says nothing about whether the site works.

Answering is not the finish line, and this report used to treat it as one. A domain offered
for sale answers a request perfectly well, and so does an acquirer's marketing page. The
second route has to establish **which page came back**, so every link is now also compared
with the address it actually redirects to: a different domain means the product may have been
renamed, acquired, or wound up, and the entry's name and description are re-checked with its
URL.



**Broken links:** None.

TiorAI links were verified separately: 2 checked, 2 resolved with a
`200`, 0 broken.

## What QA does not cover

Automated checks confirm that a URL resolves, that the format is right, and that ordering and
vocabularies hold. They cannot confirm that a description is accurate or that a product still
does what it claims. Those were checked by reading each category back as a block against the
vendor's current site, which is also the only way the "could these two descriptions swap
places unnoticed" test can be applied.

Pricing is the fastest-moving fact here and the most likely to be wrong first. It was correct
on 2026-08-22; it is not guaranteed to be correct now, which is what the review date is for.

## Changes since this run

**2026-08-22.** Every link was compared with the address it actually redirects to, which is a check this run did not make.

- 3 entries now ship the address their link resolves to rather than one that redirects.

- Removed, because the destination is a page about somebody else's product with no trace of the name the entry carried: **Calabrio** (folded into Verint workforce engagement), **Surfboard** (folded into Dialpad workforce management), **Tymeshift** (folded into Zendesk workforce management), **Ultimate** (folded into Zendesk AI agents).
