# Trust-Layer-Pattern

*Reference architecture for trust-first knowledge platforms — the engineering pattern behind Higher Self's commercial builds.*

## What this is

Every industry is about to run a race it doesn't know it's running: the race to own the trust layer in its category.

AI has made content cheap. Google, Perplexity, ChatGPT, and Claude now weight trust signals above volume — named expert reviewers, primary-source citations, dated updates, auditable provenance. The businesses that combine AI-scale production with trust-layer authority will own their category's knowledge for a decade. The rest go invisible.

This repository documents the engineering pattern for building that trust layer: the schemas, templates, agent pipeline, and architectural decisions behind a citation-grade knowledge platform. It's published under MIT licence because the commercial value is in judgement and execution, not in hoarding the pattern.

## What's inside

- `/schemas/` — JSON Schemas (Draft 2020-12) for the four page types: regulation, glossary, FAQ, comparison. Every trust-layer field (reviewer, citations, provenance, last-updated) is present on every type.
- `/patterns/` — deep-dive explanations of the three core mechanisms: the trust layer, the agent pipeline, the admin feedback loop.
- `/examples/work-at-height-2005/` — a fully-worked regulation page built against the schema. Real HSE content, real citations, real reviewer attribution. Validates cleanly.
- `ARCHITECTURE.md` — six architectural decisions with trade-offs named: why structured page types, why citation-grade, why named expert reviewers, why mobile-native, why agent orchestration, why fail-closed fact-checking.

## The architecture at a glance

```
User query
    ↓
Search layer
    ↓
Page type (regulation / glossary / FAQ / comparison)
    ↓
Trust layer (reviewer + citations + date + provenance)
    ↓
Course / service routing
    ↓
Admin feedback loop (demand signals, content gaps)
    ↓
Next priority content decision
    ↓ (loops)
```

Pages are a byproduct of the loop, not the product. The product is the closed-loop system where every search teaches the next page decision.

## Who this is for

Technical founders, content strategists, and compliance leads at regulated or expertise-led businesses evaluating:

- Whether to build a knowledge platform in-house or partner with someone who has
- What "AI-scale production with human trust signals" actually looks like in code
- How agent orchestration can produce citation-grade content at team scale without AI slop

This repo is the pattern. For the human-curated commercial implementation, see [higherself.ai](https://higherself.ai/).

## What this is not

- **Not a framework or library** — the world has enough of those. This is architectural pattern + schemas + worked examples.
- **Not a complete platform** — no runtime, no backend, no UI. The commercial platforms built on this pattern are proprietary.
- **Not a replacement for human judgement** — the trust layer works because named experts review every page before publication. AI drafts; humans approve.

## Status

This is a living reference. The schemas and patterns are published progressively as they stabilise in production at Higher Self. Current working deployments include a 269-page EASA-regulated aviation platform for Sofema Online (live, public launch Q3 2026) and further builds in maritime, offshore, and industrial safety training.

## Licence

MIT. Use, adapt, fork. If you ship something interesting, send a pull request — or send a note to [higherself.ai](https://higherself.ai/).

## Maintainer

David Bentley · Founder, Higher Self Forge Ltd · [higherself.ai](https://higherself.ai/) · [github.com/davidandrewbentley](https://github.com/davidandrewbentley)
