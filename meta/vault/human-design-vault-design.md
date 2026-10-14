# Human Design Knowledge Vault Design

## Purpose

This repository can evolve from a collection of explanatory Markdown files into a small, navigable knowledge vault for Human Design and related contemplative systems.

The aim is dual-use:

- **Human-readable:** a newcomer can enter through a clear overview and follow a natural learning path.
- **Machine-readable:** recurring concepts, fields, links, provenance, and validation states are predictable enough for search, graph navigation, and future tooling.

The Gemstones repository is a useful reference because it treats knowledge engineering as a bounded, incremental experiment. It combines one-note-per-entity pages with a reusable specification, a dictionary interface, a repeatable process, source attribution, and proof-run audits. [Gemstones README](https://github.com/fountain-of-love/gemstones/blob/main/README.md)

## Lessons to carry over

### 1. Define the interface before expanding the ontology

The most important lesson is to create a shared vocabulary before writing hundreds of notes. Gemstones uses a dictionary as an interface layer: concepts receive a short, consistent definition first, then can later grow into deeper notes or link outward.

For Human Design, the first dictionary should define terms such as:

- Type
- Strategy
- Authority
- Signature
- Not-Self Theme
- Center
- Gate
- Line
- Channel
- Definition
- Profile
- Incarnation Cross
- Design
- Personality
- Activation
- Source
- Interpretation

This prevents the same term from quietly changing meaning across pages.

### 2. Keep domain boundaries visible

Human Design touches astrology, the I Ching, Gene Keys, psychology, spirituality, genetics, coaching, and health claims. The vault should connect these domains without pretending to own all of them.

Recommended boundary:

> This vault documents Human Design as a symbolic and esoteric knowledge system, its internal vocabulary, its source traditions, and its contemplative applications. It does not present Human Design as scientific diagnosis or medical advice.

Gene Keys, astrology, the I Ching, and psychology should be treated as connected domains with their own source notes—not collapsed into one undifferentiated ontology.

### 3. Use links as controlled expansion

Do not place every possible explanation into every page. A Type note should link to Authority, Centers, and Strategy rather than re-explaining the entire system each time.

Obsidian-style links such as `[[Strategy]]` and `[[Sacral Center]]` can provide graph navigation. Normal Markdown links should remain available where portability outside Obsidian matters.

The principle is:

> Keep the local page coherent; let the graph carry depth.

### 4. Separate overview, structured facts, interpretation, and sources

Gemstones distinguishes narrative orientation from tables, linked concepts, and validation notes. Human Design pages should do the same.

Each concept page should distinguish:

1. **Overview** — an approachable explanation.
2. **Structured identity** — stable fields that can be compared across notes.
3. **System relationships** — links to related concepts.
4. **Interpretive layer** — how practitioners commonly contemplate the concept.
5. **Source context** — where each claim comes from.
6. **Cautions and boundaries** — what should not be inferred.

This prevents poetic interpretation from being mistaken for canonical system mechanics or empirical evidence.

### 5. Preserve absence and uncertainty

The Gemstones process explicitly keeps missing fields visible rather than silently filling them with invented completeness. The Human Design vault should use the same discipline.

Useful states include:

- `Not yet researched`
- `Not specified by source`
- `Interpretation varies by school`
- `Source disagreement`
- `Contemplative claim; not empirically validated`

Empty or uncertain knowledge is more trustworthy than confident fabrication.

### 6. Create a repeatable page contract

One-page guides are useful, but a vault needs predictable structure. A reusable specification makes it possible to compare five Types, nine Centers, 64 Gates, 36 Channels, 13 planetary elements, and Profiles without flattening their differences.

The contract should be a guide, not a rigid writing cage. Shared fields provide comparability; the overview and interpretation should retain a natural voice.

### 7. Work incrementally through proof runs

Do not generate the entire Human Design ontology in one pass. Start with a small proof run:

- the five Types;
- the main Strategy and Authority concepts;
- the nine Centers;
- one or two example case studies;
- a small set of linked Gates or Channels.

Audit the proof run for consistency, source quality, link integrity, and usefulness before scaling toward all 64 Gates and 36 Channels.

### 8. Make provenance first-class

The source model should distinguish among:

- original Human Design system material;
- official or lineage-specific explanations;
- Richard Rudd’s Gene Keys interpretation;
- independent practitioner interpretations;
- psychological or scientific commentary;
- this vault’s own synthesis.

Claims should not be presented as if all sources have equal authority or belong to the same tradition. A source table and claim-level attribution are more valuable than a long undifferentiated bibliography.

### 9. Keep personal charts in a separate layer

Yves’s chart is useful as a real-world case study, but it should not pollute the theory layer. Personal charts belong under `human-design-content/case-studies/` and should link back to general concepts.

This separation supports both privacy and context efficiency:

- theory can be acquired without personal data;
- case studies can demonstrate application;
- new anonymized or consented examples can be added later;
- no individual chart becomes the hidden definition of a concept.

### 10. Treat health and therapeutic claims carefully

The Gemstones repository keeps therapeutic traditions source-attributed and avoids presenting them as medical advice. Human Design needs an even clearer boundary because its language can sound psychological or biological.

The vault should label claims as one of:

- **System description** — how Human Design defines a concept internally.
- **Practitioner interpretation** — a reading used by a school or teacher.
- **Contemplative prompt** — a question for self-observation.
- **Empirical claim** — a claim requiring external scientific evidence.
- **Unsupported or disputed claim** — retained only with explicit caution.

## Proposed vault structure

```text
README.md
human-design-content/
  HUMAN-DESIGN-BASICS.md
  HUMAN-DESIGN-13-ELEMENTS.md
  README.md

  types/
  concepts/
  case-studies/

meta/
  vault/
    human-design-vault-design.md
    meta-dictionary-best-practice.md
  human-design/
    human-design-spec.md
    human-design-process.md
    human-design-dictionary.md
    human-design-proof-run.md
    sources/
      source-index.md

human-design-content/
  centers/
    head.md
    ajna.md
    throat.md
    g-center.md
    heart-ego.md
    solar-plexus.md
    sacral.md
    spleen.md
    root.md
  gates/
    gate-01.md
    ...
    gate-64.md
  channels/
    channel-index.md
    ...
  planets/
    sun.md
    earth.md
    lunar-nodes.md
    moon.md
    mercury.md
    venus.md
    mars.md
    jupiter.md
    saturn.md
    uranus.md
    neptune.md
    pluto.md
  profiles/
    profile-index.md
    ...
```

The current content now lives under `human-design-content/`. The existing type one-pagers are under `human-design-content/types/`, and the Yves case study is under `human-design-content/case-studies/`.

## Proposed page contract

Each concept page should use only the fields that make sense for its entity, while preserving a stable core:

```yaml
---
entity_type: "type | center | gate | channel | planet | profile | concept | case-study"
name: ""
slug: ""
domain: "human-design"
status: "draft | reviewed | stable"
source_scope: "system | practitioner | synthesis"
last_reviewed: "YYYY-MM-DD"
---
```

Suggested body structure:

```markdown
# {Name}

## Overview

## Structured identity

## Core mechanics

## Relationships

## Contemplative interpretation

## Example

## Boundaries and uncertainty

## Sources

## Review notes
```

Not every page needs every heading in equal depth. The contract exists to make omission visible and comparison possible.

## Proposed dictionary role

`meta/human-design/human-design-dictionary.md` should be the stable interface for repeated field labels and terms. It should remain short at first. A dictionary entry can be one paragraph and link to a deeper page later.

Example:

```markdown
## Authority

The Human Design mechanism used to describe how a person may make decisions according to their chart. In this vault, Authority is documented as a system concept and not presented as a scientifically established decision-making process.

Related: [[Strategy]], [[Type]], [[Solar Plexus]], [[Sacral Center]], [[Spleen]]
```

The dictionary should be an interface layer, not an encyclopedia.

## Proposed creation process

For each new note:

1. Select the concept from an index or backlog.
2. Read the page specification.
3. Identify the concept’s source scope.
4. Capture source claims and terminology before rewriting.
5. Write the overview in original language.
6. Fill structured fields and preserve unknowns explicitly.
7. Add links to existing concepts.
8. Separate system description from interpretation.
9. Add source notes and any necessary caution.
10. Check headings, links, metadata, and terminology against the dictionary.
11. Add the page to a small proof run.
12. Review the proof run before expanding the ontology.

This is deliberately lightweight. The vault should grow through small, auditable increments rather than a large speculative taxonomy.

## What to avoid

- Generating all 64 Gates before the page contract is tested.
- Treating one teacher’s interpretation as the universal Human Design meaning.
- Mixing Human Design, Gene Keys, astrology, and psychology without labeling the boundaries.
- Repeating the same definition in every note instead of linking to a canonical concept.
- Presenting esoteric interpretations as medical, genetic, or psychological facts.
- Hiding missing research behind polished prose.
- Making Yves’s chart the implicit example for every concept.
- Building automation before the vocabulary and source model are stable.

## Recommended first milestone

The first vault milestone should be a small, coherent foundation:

1. Add `README.md` as the vault map.
2. Add `meta/human-design/human-design-spec.md`.
3. Add `meta/human-design/human-design-process.md`.
4. Add `meta/human-design/human-design-dictionary.md`.
5. Keep the five type one-pagers under `human-design-content/types/`.
6. Keep personal charts under `human-design-content/case-studies/`.
7. Add concept pages for Strategy, Authority, Design, Personality, Signature, and Not-Self Theme.
8. Create a proof-run audit covering those pages.

Only after that should the vault expand systematically into Centers, Planets, Gates, Channels, and Profiles.

## Design principles

The resulting vault should follow these principles:

- **Smallest useful structure:** introduce a page or abstraction when it improves navigation or consistency.
- **Source-aware writing:** preserve distinctions among tradition, interpretation, synthesis, and evidence.
- **Explicit uncertainty:** absence and disagreement remain visible.
- **Graph over duplication:** links carry depth; pages retain local coherence.
- **Theory before biography:** personal charts illustrate the model but do not define it.
- **Incremental proof:** every expansion is tested on a small set before being generalized.
- **Human and machine readability:** prose, tables, metadata, and links serve different reading modes.

## Reference

The main reference repository is [fountain-of-love/gemstones](https://github.com/fountain-of-love/gemstones). Its most relevant design artifacts are:

- [README and project principles](https://github.com/fountain-of-love/gemstones/blob/main/README.md)
- [Page specification](https://github.com/fountain-of-love/gemstones/blob/main/gemstone-spec.md)
- [Dictionary interface](https://github.com/fountain-of-love/gemstones/blob/main/gemstone-dictionary.md)
- [Creation process](https://github.com/fountain-of-love/gemstones/blob/main/gemstone-process.md)
