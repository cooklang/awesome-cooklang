# Awesome Cooklang [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

<img src="https://cooklang.org/images/logo.svg" align="right" width="100" alt="Cooklang logo"/>

> Curated list of apps, CLIs, libraries, and integrations for [Cooklang](https://cooklang.org) — a plain-text markup language for recipes.

Cooklang lets you write recipes as `.cook` files that any tool can read: scale them, generate shopping lists, build cookbooks, sync between devices. This list points to the best tooling, official and community-built.

For curated recipe collections written *in* Cooklang, see [awesome-cooklang-recipes](https://github.com/cooklang/awesome-cooklang-recipes).

## Contents

- [For Cooks](#for-cooks)
  - [Mobile Apps](#mobile-apps)
  - [Desktop & Editors](#desktop--editors)
  - [Web Apps](#web-apps)
  - [Recipe Discovery](#recipe-discovery)
- [For Developers](#for-developers)
  - [Official Libraries](#official-libraries)
  - [Parsers by Language](#parsers-by-language)
  - [CLI Tools](#cli-tools)
  - [Build & Site Plugins](#build--site-plugins)
  - [Format Converters](#format-converters)
  - [AI & Agent Tooling](#ai--agent-tooling)
- [For Tinkerers](#for-tinkerers)
  - [Editor Integrations](#editor-integrations)
  - [Smart Home & Hardware](#smart-home--hardware)
  - [Self-Hosting](#self-hosting)
- [Resources](#resources)
  - [Specification & Tests](#specification--tests)
  - [Talks](#talks)
  - [Articles](#articles)
  - [Community](#community)
- [Contributing](#contributing)

## For Cooks

### Mobile Apps

- [Cook for iOS](https://apps.apple.com/us/app/cooklangapp/id1598799259) — Native iOS app. Sync your `.cook` files via iCloud Drive.
- [Cook for Android](https://play.google.com/store/apps/details?id=md.cook.android) — Native Android app, with optional desktop sync agent.

### Desktop & Editors

- [Cook Editor](https://github.com/cook-md/editor) — Free desktop app for macOS, Windows, and Linux. Syntax highlighting, recipe preview, multi-day meal plans, optional Cookbot AI sidebar.

### Web Apps

- [cook.md](https://cook.md) — AI-powered recipe converter. Paste a URL, image, or text and get back Cooklang.
- [Cooklang Playground](https://cooklang.github.io/cooklang-rs/) — In-browser editor with raw parser output, powered by `cooklang-rs` compiled to WebAssembly.

### Recipe Discovery

- [Cooklang Federation](https://recipes.cooklang.org) — Federated search across community recipe repositories via RSS / Atom feeds and a crawler.
- [awesome-cooklang-recipes](https://github.com/cooklang/awesome-cooklang-recipes) — Curated list of public cookbooks written in Cooklang.

## For Developers

### Official Libraries

- [cooklang-rs](https://github.com/cooklang/cooklang-rs) — Canonical parser. Optional extensions, unit conversion, recipe scaling, rich error reporting. Rust.
- [cooklang-bindings](https://crates.io/crates/cooklang-bindings) — UniFFI bindings exposing `cooklang-rs` to Kotlin, Swift, Ruby, and Python.
- [cooklang-import](https://github.com/cooklang/cooklang-import) — Import recipes from URLs into Cooklang via LLM. Rust.
- [cooklang-reports](https://github.com/cooklang/cooklang-reports) — Generate reports from recipes using Jinja2-style templates with scaling, metadata, and YAML datastore. Rust.
- [cooklang-find](https://github.com/cooklang/cooklang-find) — Filesystem search and tree-building for recipe collections. Rust.
- [cooklang-sync](https://github.com/cooklang/cooklang-sync) — File-sync library optimised for plain-text recipes. Rust.

### Parsers by Language

One canonical pick per language. See [`parsers.md`](parsers.md) for alternative implementations and historical projects.

- **C** — [cook-in-c](https://github.com/cooklang/cook-in-c)
- **Clojure** — [cooklang-clj](https://github.com/kiranshila/cooklang-clj)
- **Dart** — [cooklang-dart](https://github.com/aquilax/cooklang-dart) ([pub.dev](https://pub.dev/packages/cooklang))
- **Elixir** — [cooklang-ex](https://github.com/cooklang/cooklang-ex) ([hex.pm](https://hex.pm/packages/cooklang_ex)) — official bindings.
- **Go** — [cooklang-go](https://github.com/aquilax/cooklang-go)
- **Haskell** — [cooklang-hs](https://github.com/isaacvando/cooklang-hs) ([Hackage](https://hackage.haskell.org/package/cooklang-hs))
- **JavaScript / TypeScript** — [@cooklang/cooklang](https://www.npmjs.com/package/@cooklang/cooklang) — official WASM build of `cooklang-rs`.
- **Lua** — [cooklang-lua](https://github.com/michal-h21/cooklang-lua)
- **.NET / C#** — [cooklangnet](https://github.com/heytherewill/cooklangnet) ([NuGet](https://www.nuget.org/packages/CookLangNet))
- **Perl** — [CookLang](https://metacpan.org/pod/CookLang) on CPAN.
- **Python** — [cooklang-py](https://github.com/brass75/cooklang-py) ([PyPI](https://pypi.org/project/cooklang-py/))
- **Ruby** — [cooklang_rb](https://github.com/drbragg/cooklang_rb) ([RubyGems](https://rubygems.org/gems/cooklang_rb))
- **Rust** — [cooklang-rs](https://github.com/cooklang/cooklang-rs) — see *Official Libraries* above.
- **Swift** — [CookInSwift](https://github.com/cooklang/CookInSwift) — used by the iOS app.

### CLI Tools

- [CookCLI](https://github.com/cooklang/cookcli) — Official CLI. Parse, validate, scale, generate shopping lists, run a web server, import recipes from the web, manage a pantry, expose an LSP. Available via [Homebrew](https://formulae.brew.sh/formula/cookcli) and [AUR](https://aur.archlinux.org/packages/cookcli). Rust.
- [cooklang-chef](https://github.com/Zheoni/cooklang-chef) — Alternative CLI with a built-in web UI for scaling and conversion. Rust.

### Build & Site Plugins

For generating recipe websites from `.cook` files.

- [eleventy-plugin-cooklang](https://github.com/matt-auckland/eleventy-plugin-cooklang) — Eleventy.
- [jekyll-cooklang-converter](https://rubygems.org/gems/jekyll-cooklang-converter) — Jekyll.
- [astro-cooklang](https://www.npmjs.com/package/astro-cooklang) — Astro.
- [vite-plugin-cooklang](https://www.npmjs.com/package/vite-plugin-cooklang) — Vite.
- [vitepress-plugin-cooklang](https://www.npmjs.com/package/vitepress-plugin-cooklang) — VitePress.
- [markdown-it-cooklang](https://github.com/ulfschneider/markdown-it-cooklang) — markdown-it.
- [n8n-nodes-cooklang](https://www.npmjs.com/package/n8n-nodes-cooklang) — Custom nodes for n8n workflows.
- [cookhub](https://www.npmjs.com/package/cookhub) — Pull and parse recipes from GitHub repositories.

### Format Converters

- [cooklang-to-md](https://crates.io/crates/cooklang-to-md) — Cooklang → Markdown. Rust.
- [cooklang-epub](https://github.com/pakohan/cooklang-epub) — Cooklang → EPUB. Go.
- [cooklang-sankey](https://www.npmjs.com/package/@4kk11/cooklang-sankey) — Build Sankey diagram data from a recipe.

### AI & Agent Tooling

- [cooklang-skills](https://github.com/cooklang/cooklang-skills) — Skills for Claude and Codex agents: create, import, validate, scale, meal-plan, manage a pantry, and export Cooklang recipes from inside an agent session.

## For Tinkerers

### Editor Integrations

- [VS Code extension](https://marketplace.visualstudio.com/items?itemName=dubadub.cook) — Syntax highlighting, validation, autocomplete.
- [Cooklang for Obsidian](https://github.com/cooklang/cooklang-obsidian) — Recipe preview, interactive timers, shopping checklists inside Obsidian.
- [tree-sitter-cooklang](https://github.com/addcninblue/tree-sitter-cooklang) — Tree-sitter grammar. Wire it into Neovim, Helix, Zed, or Emacs.
- [cooklang-language-server](https://github.com/cooklang/cooklang-language-server) — LSP server. Works in any LSP-aware editor.

### Smart Home & Hardware

- [homeassistant-cookcli](https://github.com/cooklang/homeassistant-cookcli) — Home Assistant custom component. Meal-plan calendar, shopping list as a Todo entity, pantry sensors, recipe stats. HACS-compatible.
- [Raspberry Pi kitchen display guide](https://cooklang.org/blog/17-raspberry-pi-kitchen-display/) — Build a touchscreen kitchen display backed by CookCLI.
- [Sync Agent](https://cook.md/download) — Lightweight desktop sync service that keeps a recipe folder in sync with the iOS and Android apps.

### Self-Hosting

- [Federation](https://github.com/cooklang/federation) — Run your own federated recipe search node.
- [CookCLI server](https://cooklang.org/cli/commands/server/) — Self-host a private recipe web UI with `cook server ./recipes`.

## Resources

### Specification & Tests

- [Cooklang Specification](https://cooklang.org/docs/spec/) — Reference grammar and conventions.
- [EBNF definition](https://github.com/cooklang/spec/blob/main/EBNF.md) — Formal grammar.
- [Canonical test suite](https://github.com/cooklang/spec/tree/main/tests) — Conformance tests every parser should pass.

### Talks

- [Cooklang at FOSDEM](https://youtu.be/3uYmduWuhNk)
- [Cooklang at OggCamp](https://youtu.be/lZUqhxX9-w8)

### Articles

- [Designing a Recipe Markup Language](https://cooklang.org/blog/37-designing-a-recipe-markup-language/) — How and why Cooklang exists.
- [Cooking for Programmers](https://cooklang.org/blog/22-cooking-for-programmers/) — Why developers like plain-text recipes.
- [Why Plain Text Recipes](https://cooklang.org/blog/12-why-plain-text-recipes/) — Long-form rationale.
- [Building a Recipe API with Cooklang](https://cooklang.org/blog/29-building-recipe-api-with-cooklang/) — End-to-end developer walkthrough.
- [Parser Integration Guide](https://cooklang.org/blog/44-cooklang-parser-integration-guide/) — Embedding a Cooklang parser in your app.
- [Editor Setup](https://cooklang.org/blog/39-cooklang-editor-setup/) — Configuring VS Code, Obsidian, Vim, and others.

### Community

- [Discord](https://discord.gg/fUVVvUzEEK) — Community chat.
- [Cooklang on GitHub](https://github.com/cooklang) — Official organisation.

## Contributing

Submissions welcome — please read [CONTRIBUTING.md](CONTRIBUTING.md) first.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, contributors have waived all copyright and related rights to this work.
