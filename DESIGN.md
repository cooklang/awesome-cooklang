# Design Notes

Brief record of the decisions behind this repo, kept so future maintainers don't have to re-litigate them.

## Goals

- A single curated, audience-organised entry point for **tools** that work with Cooklang.
- Complement, not duplicate, [`awesome-cooklang-recipes`](https://github.com/cooklang/awesome-cooklang-recipes), which covers recipe *collections*.

## Non-goals

- Be exhaustive. We deliberately apply a quality filter (see `CONTRIBUTING.md`) and keep one canonical pick per parser language; alternatives live in `parsers.md`.
- Replace [`cooklang.org/docs/for-developers`](https://cooklang.org/docs/for-developers/). The site stays the entry point for newcomers; this repo is the maintained list of links.

## Scope decisions

- **Curation level: strict.** Only actively maintained or tagged-stable projects make the README. Failures or stale projects either get noted in `parsers.md` or omitted.
- **Categories: audience-first.** Top-level sections are *For Cooks*, *For Developers*, *For Tinkerers*, and *Resources*. Subsections are conventional within each.
- **Officials included.** Both first-party (`cooklang/`, `cook-md/`) and community projects appear, distinguished by description rather than separate sections — readers tend to want what works, not who built it.
- **No "Related" section.** Comparable non-Cooklang tools (Mealie, Tandoor, Paprika) are out of scope; the [blog](https://cooklang.org/blog) handles comparisons.
- **One canonical parser per language** in the README, with a `parsers.md` long-tail. Avoids the README drowning in 6 Go parsers, while still acknowledging community work.

## File layout

```
README.md                          — the awesome list
parsers.md                         — alternative parser implementations
CONTRIBUTING.md                    — submission rules + quality bar
LICENSE                            — CC0 1.0
.github/PULL_REQUEST_TEMPLATE.md   — checkbox-driven PR template
DESIGN.md                          — this file
```

## Quality bar (used by CONTRIBUTING.md)

1. Functional — produces, parses, or integrates with Cooklang.
2. Documented — README explaining what and how.
3. Maintained or stable — commits in last 18 months, or tagged release that still works.
4. Discoverable — public repo / package / URL.
5. Distinct — clear differentiator if duplicating a category.

## Open follow-ups

- `cooklang/cooked` (GPUI desktop app) is in active development but has no released build at the time of this seeding. Add to *Desktop & Editors* once it ships a release.
- VS Code extension marketplace publisher ID was confirmed as `dubadub.cook`; if a future release moves it under a different publisher, update the link.
- Self-hosting docker images for CookCLI exist on Docker Hub (community-maintained); not seeded because none had clear ownership / maintenance signals at seed time.
