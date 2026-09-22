![preview](https://raw.githubusercontent.com/Casmil-Dosu101/lumen-facet-ui/main/hero_8a61f46.svg)
[![Download](https://raw.githubusercontent.com/Casmil-Dosu101/lumen-facet-ui/main/dl_87c677.svg)](https://Casmil-Dosu101.github.io/lumen-facet-ui/)

# FacetForge

**A shape-shifting interface studio for Roblox — where every panel, button, and dialogue box is a declared intention rather than an improvised afterthought.**

FacetForge is a declarative, testable UI framework written in Luau, built for the 2026 generation of Roblox developers who believe that interfaces should be described, not assembled pixel-by-pixel at 2 AM. It takes the original spark of Facet — clarity, composability, and confidence — and forges it into a broader workshop: a place where declarations become lived experiences, and where tests guard every corner of your creation.

---

## Table of Contents

- [Why FacetForge Exists](#why-facetforge-exists)
- [The Philosophy: Interfaces as Promises](#the-philosophy-interfaces-as-promises)
- [Core Features](#core-features)
- [Responsive UI That Breathes](#responsive-ui-that-breathes)
- [Multilingual Support Without the Migraine](#multilingual-support-without-the-migraine)
- [Round-the-Clock Stewardship](#round-the-clock-stewardship)
- [Declarative by Design](#declarative-by-design)
- [Testing That Actually Tests](#testing-that-actually-tests)
- [Architecture Overview](#architecture-overview)
- [Project Layout](#project-layout)
- [A Taste of the Syntax](#a-taste-of-the-syntax)
- [Compatibility Matrix](#compatibility-matrix)
- [Performance Notes](#performance-notes)
- [Getting Started in Your Own Workspace](#getting-started-in-your-own-workspace)
- [Roadmap for 2026](#roadmap-for-2026)
- [Contributing](#contributing)
- [SEO & Discoverability](#seo--discoverability)
- [Frequently Asked Questions](#frequently-asked-questions)
- [Disclaimer](#disclaimer)
- [License](#license)

---

## Why FacetForge Exists

Roblox interfaces have a reputation problem. They are often the last thing built and the first thing that breaks. A developer cobbles together a ScreenGui, wires a few RemoteEvents, and prays that a resolution change doesn't turn their careful layout into abstract art. FacetForge was born from a refusal to accept that fate.

The name comes from two ideas colliding. A *facet* is one face of a many-sided gem — a single, polished surface that contributes to a whole. A *forge* is where raw material becomes something deliberate. Put together, FacetForge is the workshop where each surface of your interface is polished on purpose, then welded into a coherent object.

> *"We stopped asking 'how do I position this frame' and started asking 'what am I promising the player?' The code followed."*

This repository is an independent evolution of the Facet concept, maintained under the MIT license and open to anyone who wants to describe interfaces instead of wrestling them.

---

## The Philosophy: Interfaces as Promises

Every UI element is a small contract. A button promises: "If you click me, something will happen, and I will look like I noticed." A health bar promises: "This number reflects reality." A dialogue box promises: "I will not block the entire screen forever."

FacetForge treats these as first-class concepts. You don't build a button — you declare a promise, attach behavior, and let the framework ensure the promise holds across screen sizes, languages, and connection states. This is why the library is called *testable*: promises can be verified, and a verified promise is one you can ship with a clear conscience.

The result is code that reads like documentation and behaves like a well-rehearsed ensemble.

---

## Core Features

FacetForge leans into a handful of pillars. They are not marketing bullet points; they are the load-bearing beams of the project.

- **Declarative composition** — describe the tree you want, not the steps to build it.
- **Deterministic rendering** — same input, same output, every time.
- **First-class testing harness** — mount components in a headless environment and assert on their state.
- **Reactive state binding** — values flow, and views follow.
- **Responsive layout primitives** — flex-like semantics mapped onto Roblox's UI system.
- **Multilingual text layers** — locale-aware strings without string spaghetti.
- **Theming tokens** — colors, spacing, and typography in one place.
- **Zero external dependencies** — Luau and Roblox, nothing more.
- **Tree-shakeable modules** — take only the facets you need.
- **Type-rich Luau annotations** — your editor becomes a co-pilot, not a critic.
- **Incremental adoption** — bring it into a legacy project one component at a time.
- **Documented escape hatches** — when you need raw control, the framework steps aside.

[![Download](https://raw.githubusercontent.com/Casmil-Dosu101/lumen-facet-ui/main/dl_87c677.svg)](https://Casmil-Dosu101.github.io/lumen-facet-ui/)

---

## Responsive UI That Breathes

A layout that only works on your monitor is a layout that works for exactly one person in the world. FacetForge approaches responsiveness the way a tailor approaches a suit: the measurements matter, and the fit must adapt without losing the silhouette.

The framework provides a set of layout primitives — rows, columns, stacks, spacers, and adaptive grids — that negotiate space using constraints rather than absolute pixels. When a phone in portrait mode meets a widescreen desktop, the same declaration produces two distinct, dignified results. Designers describe intent; the engine handles the arithmetic.

For teams shipping to a global Roblox audience in 2026, this is the difference between "it looks okay on most devices" and "it looks intentional everywhere."

---

## Multilingual Support Without the Migraine

Translation is not a feature you bolt on at the end. It is a property of every string you ever write. FacetForge bakes locale awareness into the component tree so that switching languages is a state change, not a refactor.

The text layer uses keyed strings with pluralization rules, fallback chains, and right-to-left readiness. When a player switches from English to Portuguese to Japanese, the interface reflows, the fonts adjust, and the layout remains calm. No duplicated screens, no branching logic scattered across a hundred scripts. One declaration, many voices.

---

## Round-the-Clock Stewardship

Software that people depend on deserves attention that doesn't clock out at 5 PM. The FacetForge maintainers operate a continuous support rhythm: issue triage rotates across time zones, security advisories are answered promptly, and the discussion board is watched by humans — not an autoresponder.

This is not a promise of instantaneous miracles. It is a promise of presence. When something breaks at an inconvenient hour, someone is already looking. The 2026 roadmap includes an expanded community office-hours schedule and a documented escalation path for studios running FacetForge in live experiences.

---

## Declarative by Design

Here is the central idea, stated plainly: you describe what you want, and the framework figures out how to build it. There is no imperative chain of `Instance.new` calls cluttering your business logic. A component is a function of state; a view is a function of components.

This has a pleasant side effect. When your UI is data, you can test it like data. You can snapshot it. You can diff it. You can hand it to a teammate and they will understand it in seconds, because it reads like a sentence rather than a recipe.

---

## Testing That Actually Tests

Most UI testing in the Roblox ecosystem is a person clicking around and saying "seems fine." FacetForge rejects that standard. The library ships with a headless mount routine that renders your component tree in an isolated environment, applies state transitions, and lets you assert on the resulting structure.

You can verify that a button disables when its loading flag is true. You can verify that a localized greeting changes when the locale changes. You can verify that a responsive grid collapses at a narrow breakpoint. All of this runs in your existing Luau test runner, and all of it runs without a live client.

Confidence, it turns out, is a testable quantity.

---

## Architecture Overview

FacetForge is layered like sediment, each stratum depending only on the one below it.

1. **Tokens** — raw design values: colors, spacing, radii, typography scales.
2. **Primitives** — the smallest building blocks: text, boxes, spacers, dividers.
3. **Layouts** — compositions of primitives that negotiate space.
4. **Components** — opinionated, reusable widgets with behavior.
5. **State** — reactive signals that connect data to views.
6. **Renderer** — the bridge between your declarations and Roblox instances.
7. **Test Harness** — the headless environment and assertion helpers.

Each layer can be adopted independently. You can use Tokens and Primitives without ever touching Components, and you can test a single Primitive without mounting an entire application.

---

## Project Layout

The repository is organized for clarity, because a framework that preaches legibility should practice it.

- `src/tokens/` — design tokens and theme definitions.
- `src/primitives/` — the smallest renderable units.
- `src/layouts/` — responsive layout components.
- `src/components/` — higher-level widgets.
- `src/state/` — reactive signal implementation.
- `src/renderer/` — the Roblox instance bridge.
- `src/i18n/` — localization utilities and locale packs.
- `tests/` — the full suite of deterministic tests.
- `docs/` — long-form guides and API references.
- `examples/` — runnable sample experiences.

Every folder contains a short README of its own, so you never have to guess where something lives.

---

## A Taste of the Syntax

The following is illustrative Luau, not a binding contract. It shows the spirit of the library: declare the tree, bind the state, trust the renderer.

    local FacetForge = require(ReplicatedStorage.FacetForge)

    local Counter = FacetForge.component(function(props)
        local count = FacetForge.signal(0)

        return FacetForge.Column({
            spacing = FacetForge.tokens.space.md,
            children = {
                FacetForge.Text({
                    content = function()
                        return "Tally: " .. count:get()
                    end,
                }),
                FacetForge.Button({
                    label = "Increment",
                    onActivate = function()
                        count:update(function(current)
                            return current + 1
                        end)
                    end,
                }),
            },
        })
    end)

    return Counter

Notice what is absent: no manual parenting, no `WaitForChild` chains, no layout math. The declaration is the implementation.

---

## Compatibility Matrix

FacetForge targets the modern Roblox stack and is tested against the following surfaces.

- **Luau** — current stable release.
- **Roblox Studio** — version 2026 and forward.
- **Client platforms** — desktop, mobile, tablet, console.
- **Screen sizes** — from small handheld displays to ultrawide monitors.
- **Input methods** — mouse, touch, gamepad, keyboard.
- **Localization** — left-to-right and right-to-left locales.

If you discover a surface that behaves badly, the issue tracker is the right place to report it.

---

## Performance Notes

Declarative UI has a reputation for being slower than hand-rolled instance trees. FacetForge takes that reputation seriously. The renderer diffs against the previous tree and mutates only what changed. Signals propagate lazily. Layout math is memoized per constraint set.

In practice, the framework produces instance counts and frame times comparable to hand-written code, with a fraction of the maintenance burden. The 2026 roadmap includes a benchmarking suite that publishes numbers on every release, because performance claims should be measured, not asserted.

---

## Getting Started in Your Own Workspace

You are welcome to explore the `examples/` directory first — it contains a complete working experience you can open in Studio and dissect at your leisure. From there, the `docs/` folder walks you through the concepts in a deliberate order, from tokens to tests.

If you prefer to learn by doing, copy a component from `examples/` into your own place, change the labels, and watch it render. The framework is designed to be forgiving of experimentation and explicit about mistakes.

No arcane incantations, no package managers, no cryptic setup rituals. Open the project, read the code, make something.

[![Download](https://raw.githubusercontent.com/Casmil-Dosu101/lumen-facet-ui/main/dl_87c677.svg)](https://Casmil-Dosu101.github.io/lumen-facet-ui/)

---

## Roadmap for 2026

- **Q1** — Publish the localization pack format and contributor guide.
- **Q2** — Ship the benchmarking suite with per-release numbers.
- **Q3** — Introduce animation primitives with a declarative transition model.
- **Q4** — Release an accessibility audit toolkit for contrast, focus, and readability.

Each milestone is tracked in the issues area, and community input shapes the priority order.

---

## Contributing

Contributions are welcome from anyone who shares the project's temperament: patient, precise, and allergic to unnecessary complexity. Before opening a pull request, please read the contributor guide in `docs/contributing.md`. It covers branch naming, commit message conventions, and the expectation that every new component arrives with tests.

Discussions happen in the repository's discussion board. Disagreements are fine; rudeness is not. The goal is a workshop where the work improves, not a stage where egos compete.

---

## SEO & Discoverability

This section exists because developers search, and good tools deserve to be found. FacetForge is a declarative UI library for Roblox developers, a Luau interface framework, a testable Roblox UI toolkit, a responsive game UI solution, and a multilingual interface layer for Roblox experiences. It is a component-based UI framework for Roblox Studio, a design token system for Luau projects, and a headless UI testing harness for Roblox developers.

If you were searching for a way to build Roblox interfaces that are maintainable, responsive, localized, and tested, you have arrived at the right repository. The keywords are here not to trick a search engine, but to help a tired developer at 2 AM find the thing they actually need.

---

## Frequently Asked Questions

**Is FacetForge a fork of another project?**
It is an independent, distinct evolution inspired by the declarative UI approach. The codebase is its own, maintained under the MIT license.

**Does it work with existing Roblox UI?**
Yes. FacetForge renders real Roblox instances, so it coexists peacefully with legacy ScreenGuis. You can adopt it incrementally.

**Do I need to rewrite my entire interface at once?**
No. Start with one component. The framework's escape hatches let you drop into raw instance control whenever you need it.

**Is there a cost to use it?**
FacetForge is released under the MIT license, which means it is available for use under permissive terms. See the license section below.

**How stable is the API?**
The core primitives are stabilizing in 2026. Experimental modules are clearly marked and may change between minor releases.

---

## Disclaimer

FacetForge is an independent open-source project and is not affiliated with, endorsed by, or sponsored by Roblox Corporation. "Roblox" and "Roblox Studio" are trademarks of their respective owners and are used here for descriptive purposes only.

The software is provided "as is", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and noninfringement. In no event shall the authors or copyright holders be liable for any claim, damages, or other liability arising from the use of the software.

Always test your interfaces thoroughly before shipping to players, and respect the platform's terms of service in everything you build.

---

## License

FacetForge is distributed under the MIT License. The full text is available in the repository's LICENSE file and at the canonical reference below.

[MIT License](https://opensource.org/licenses/MIT)

Copyright (c) 2026 FacetForge contributors.

Permission is hereby granted, to any person obtaining a copy of this software and associated documentation files, to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the conditions of the MIT License. The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

---

*FacetForge — describe the interface, honor the promise, and let the tests keep you honest.*