# Trust layer

The trust layer is the point of difference between a knowledge platform and a content farm. Many systems can generate an answer-shaped page. Far fewer can show why that page deserves to be believed. In trust-first platforms, credibility is not implied by tone. It is made visible through repeatable signals that appear on every page type, not just the most important ones.

## 1. Named expert reviewer

A named reviewer is the human being willing to stand behind the page. This is not decoration. It tells the reader that a qualified person has inspected the answer, accepted the framing, and is accountable for the current version. The pattern implements this as a required object across every schema: name, title, credentials, and organisation. If you skip it, the page immediately looks interchangeable with anonymous AI output. Authority collapses the moment nobody is willing to sign.

## 2. Primary-source citation with working link

A citation is the bridge between explanation and evidence. The page should not merely mention a regulation, framework, or policy in vague terms. It should point to the exact source and let the reader inspect it. The pattern implements this with structured citation objects, retrievable URLs, and section-level references back to the source list. If you skip it, every strong sentence becomes suspect. The reader cannot distinguish expertise from assertion.

## 3. Last-reviewed date

Knowledge decays. Some domains decay quickly. A last-reviewed date tells the reader whether the page belongs to the present tense or to a forgotten editorial moment. The pattern implements this as a required top-level field so the date survives design changes, CMS migrations, and page rewrites. If you skip it, the page may still be correct, but it cannot prove that anybody checked. In compliance-facing content, undated truth is operationally weak.

## 4. Change tracking against previous versions

Authority is not strengthened by pretending pages were always perfect. It is strengthened by responsible revision. A page that records meaningful changes shows editorial seriousness and reduces the fear that updates are happening silently. The pattern references change tracking as a required operational behaviour even where the schemas stay implementation-agnostic. If you skip it, trust becomes brittle. Users notice when the answer moves, but they cannot see why.

## 5. Auditable content provenance

Provenance is the chain of custody for the page itself: who authored it, whether the author was human or agentic, when review happened, and whether fact-checking passed. This is the infrastructure behind the front-end trust signals. The pattern implements provenance as a required object across page types because publishing discipline should be queryable, not folkloric. If you skip it, you lose the ability to audit your own corpus. The page exists, but the editorial process disappears.

These five signals work together. A reviewer without sources is weak. Sources without dates go stale. Dates without provenance can be fabricated. Provenance without accountability is invisible to the reader. The trust layer makes the page legible to sceptical humans and to retrieval systems looking for durable signals of authority.

The trust layer is not optional. It is the moat.
