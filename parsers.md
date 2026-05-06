# Alternative Parser Implementations

The main [README](README.md) lists one canonical parser per language. This file collects the long tail: alternative implementations, ports, and historical projects.

Many of these are still useful — pick whichever fits your dependency story or licence preferences. Inclusion here is not an endorsement of maintenance status; verify before depending on one.

## Go

Multiple Go parsers exist. The canonical pick is [`aquilax/cooklang-go`](https://github.com/aquilax/cooklang-go). Alternatives:

- [hilli/cooklang](https://github.com/hilli/cooklang) — Parser plus pantry, renderers, shopping list helpers. Active.
- [justintout/cooklang-go](https://github.com/justintout/cooklang-go) — Lexer-based parser.
- [hugoShaka/cooklang-go](https://codeberg.org/hugoShaka/cooklang-go) — Lexical-scanning parser. Hosted on Codeberg.
- [ediblesimpl/cooklang-go](https://github.com/ediblesimpl/cooklang-go)
- [daverik/cooklang-go](https://github.com/daverik/cooklang-go)
- [rottenfishbone/cooklang-go](https://git.sr.ht/~rottenfishbone/cooklang-go) — Hosted on Sourcehut.

## TypeScript / JavaScript

Canonical pick: [`@cooklang/cooklang`](https://www.npmjs.com/package/@cooklang/cooklang) — official WASM build of `cooklang-rs`. Pure-JS or alternative TS implementations:

- [tmlmt/cooklang-parser](https://github.com/tmlmt/cooklang-parser) — TypeScript, no native dependencies.
- [deathau/cooklang-js](https://github.com/deathau/cooklang-js) — Plain JavaScript, used by older projects (notably the Obsidian plugin's older versions).
- [cadpnq/cooklangjs](https://github.com/cadpnq/cooklangjs) — Earlier JavaScript implementation.
- [cooklang-parse](https://www.npmjs.com/package/cooklang-parse) — Type-safe parser built with Ohm.js.
- [@alexanderson1993/cooklang-ts](https://www.npmjs.com/package/@alexanderson1993/cooklang-ts) — Fork of the deprecated `@cooklang/cooklang-ts`.
- [@devapeu/cooklang-parser](https://www.npmjs.com/package/@devapeu/cooklang-parser)

## Rust

Canonical pick: [`cooklang-rs`](https://github.com/cooklang/cooklang-rs). Alternatives are rare since `cooklang-rs` is the reference implementation, but worth noting:

- [umgefahren/cook-with-rust](https://github.com/umgefahren/cook-with-rust) — Independent Rust parser.

## .NET

Canonical pick: [`heytherewill/cooklangnet`](https://github.com/heytherewill/cooklangnet). Alternatives:

- [CooklangSharp](https://www.nuget.org/packages/CooklangSharp) — Alternative .NET parser with full ingredient / cookware / timer support.

## Tree-sitter Bindings & Ports

The canonical Tree-sitter grammar is [`addcninblue/tree-sitter-cooklang`](https://github.com/addcninblue/tree-sitter-cooklang). It has been re-exported in some bundles:

- [`go-sitter-forest/cooklang`](https://github.com/alexaandru/go-sitter-forest/cooklang) — Pre-built Go binding.

## Deprecated or archived

These are listed for completeness; they are no longer recommended for new projects.

- [`@cooklang/cooklang-ts`](https://github.com/cooklang/cooklang-ts) — Superseded by `@cooklang/cooklang` (WASM). The npm package is marked deprecated.
- [luizribeiro/py-cooklang](https://github.com/luizribeiro/py-cooklang) — Earlier Python parser. The canonical pick is now [`brass75/cooklang-py`](https://github.com/brass75/cooklang-py); use that for new projects.
- [`cook-markdown`](https://crates.io/crates/cook-markdown) — Earlier Cooklang-to-Markdown crate, last published in 2021.
