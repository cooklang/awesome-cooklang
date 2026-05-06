# Contributing to Awesome Cooklang

Thanks for wanting to add to the list. The goal is to keep this *useful* — a short, curated set of tools people can trust — rather than exhaustive. Please read the rules below before opening a PR.

## What belongs here

Tools, libraries, applications, and integrations that **work with Cooklang**: parsers, CLIs, apps, editor plugins, build tooling, smart-home integrations, agent skills, format converters.

Recipe *collections* (cookbooks written in Cooklang) belong in [awesome-cooklang-recipes](https://github.com/cooklang/awesome-cooklang-recipes), not here.

## Quality bar

Every entry must meet **all** of the following:

1. **Functional.** It produces, parses, or integrates with Cooklang. Not a stale fork or empty placeholder.
2. **Documented.** A README that explains what it does and how to use it. One paragraph minimum.
3. **Maintained or stable.** Either commits in the last 18 months, or a tagged release that still works against the current Cooklang spec.
4. **Discoverable.** Public repository, public package, or public URL. No private or paid-only-to-see links.
5. **Distinct.** Doesn't duplicate an existing entry without a clear differentiator. "Another Go parser" needs a reason.

If your entry fits all five, open a PR.

## How to submit

1. Fork the repo and create a branch.
2. Add your entry to the appropriate section in `README.md`. If your project is an alternative parser that doesn't replace the canonical pick, add it to `parsers.md` instead.
3. Use this format:
   ```markdown
   - [Name](url) — One-line description. Optional language / platform note.
   ```
4. Keep descriptions to one sentence and start with a capital letter, end with a period.
5. Open a PR. Fill in the PR template — it confirms you've checked the criteria.

## How entries are reviewed

Maintainers will check that your entry meets all five criteria. Things that commonly cause requests for changes:

- Description is too long, marketing-speak, or missing.
- Project hasn't shipped or has no usable release.
- Adds a language that already has a canonical parser without explaining the differentiator.
- Belongs in `awesome-cooklang-recipes`, not here.

## Removing entries

If you spot an entry that no longer meets the bar — abandoned, broken, replaced — please open an issue or PR to remove it. Curation is ongoing.

## Code of conduct

Be kind. Treat the rest of the community the way you'd want to be treated. Anything else is grounds for the maintainers to take action.
