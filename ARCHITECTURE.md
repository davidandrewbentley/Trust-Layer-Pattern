# ARCHITECTURE

## Decision 1: Structured page types over freeform publishing

Freeform blog posts are expressive, but they are a poor substrate for authority capture. They blur intent, mix definitions with persuasion, and make it hard for search systems, AI retrieval layers, and human reviewers to understand what a page is supposed to do. Structured page types force editorial discipline. A regulation page explains a rule. A glossary page defines a term. A comparison page resolves a distinction. The trade-off is less creative freedom and more schema work. The decision is that structured always wins for authority capture because legibility compounds better than flair.

## Decision 2: Citation-grade over persuasive writing

Persuasive writing is fast, emotionally effective, and often useless for consequential decisions. Citation-grade writing takes longer because sources must be gathered, checked, and anchored before the prose can stand. It is also less likely to go viral, because it is designed to reduce ambiguity rather than maximise novelty. That is the trade-off: slower production and lower virality in exchange for verifiability. The decision is that regulated buyers and AI discovery systems both reward citation, while persuasive blog content neither ranks nor converts reliably for expertise-led businesses.

## Decision 3: Named expert reviewers over anonymous publication

Anonymous content is cheap to scale and impossible to trust at the point of consequence. A named reviewer introduces friction, coordination, and real dependency on qualified people. It means you need access to domain experts, calendar time, and a clear review standard. That is the trade-off: higher operating cost in exchange for visible accountability. The decision is to require bylined review because anonymous expertise is commoditised. A reader deciding whether to rely on a compliance answer should see who signed it and why that person is allowed to do so.

## Decision 4: Mobile-native surfaces over layout richness

Regulated-industry buyers do not only research from desks. SHEQ leads, maintenance teams, site supervisors, and compliance managers often read in the field, between tasks, or on a phone during a decision window. Designing for mobile first constrains layout richness, table density, and decorative complexity. That is the trade-off: less visual flourish in exchange for usability where intent actually happens. The decision is to optimise for mobile-native reading because a page that looks elegant on a widescreen and fails in the hand is not an authority asset.

## Decision 5: Agent orchestration over single-LLM prompting

A single prompt can produce plausible content quickly, but it cannot be trusted to maintain a hard boundary between sourced claims and invented connective tissue. A staged agent pipeline is more complex to design, costs more per page, and forces explicit interfaces between research, outlining, writing, checking, and publishing. That is the trade-off: more moving parts in exchange for stronger control. The decision is that orchestration beats one-shot prompting because citation-grade pages need evidence before prose, and that ordering cannot be left to model instinct.

## Decision 6: Fail-closed fact-checking over permissive publishing

Most content systems fail open. If the draft mostly looks right, it ships. That logic is catastrophic for trust-first knowledge platforms because one unsupported claim weakens belief in every other page. A fail-closed checker rejects more drafts, slows throughput, and can frustrate teams that are used to publishing first and tidying later. That is the trade-off: lower short-term output in exchange for long-term integrity. The decision is to reject any page whose claims cannot be supported, because publishing a bad citation is worse than publishing nothing at all.

## What this is not

- Not a framework.
- Not a full platform.
- Not a replacement for human judgement about which queries matter and which experts should sign.
