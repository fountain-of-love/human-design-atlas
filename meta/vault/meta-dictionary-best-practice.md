# Meta-Dictionary: Compact Vocabulary as an Interface

## Purpose

A meta-dictionary describes how a knowledge dictionary should work. It defines the writing and information-architecture pattern, rather than defining the domain’s concepts themselves.

The dictionary is not an encyclopedia. Its primary function is to give people and tools a compact, shared vocabulary that keeps the rest of the vault consistent.

## Core pattern

Use a short grouped list:

```markdown
- **Concept:** concise definition in one or two sentences.
```

For example:

```markdown
- **Strategy:** the Type-specific way Human Design proposes that a person engage with life.
```

This format keeps the concept visually prominent, makes scanning easy, and allows definitions to be compared without forcing the reader through many headings.

## What a dictionary entry should do

Each entry should:

- establish one shared meaning;
- use consistent vocabulary;
- distinguish the domain’s internal definition from external evidence;
- point toward a deeper note when necessary;
- remain short enough to function as a lookup reference.

The dictionary should answer “What does this term mean here?” It should not attempt to answer every question about the term.

## What belongs in a deeper note

Create a dedicated concept note when a term needs:

- detailed mechanics;
- historical background;
- competing interpretations;
- examples or case studies;
- diagrams or tables;
- multiple sources;
- validation notes;
- uncertainty or disagreement analysis.

The dictionary can then retain the compact definition and link to the deeper note.

## Recommended entry shape

```markdown
- **Term:** shared definition. Optional boundary or qualification.
  - Related: [[Canonical Note]]
  - Scope: `system | practitioner | synthesis | evidence`
```

The related-note and scope lines are optional. Use them when they improve navigation or prevent ambiguity; do not add metadata mechanically to every entry.

## Organize by use, not alphabetically

Group terms according to how readers ask questions:

- system vocabulary;
- structural or data vocabulary;
- process vocabulary;
- source and evidence vocabulary;
- operational vocabulary.

Grouping gives the dictionary a map-like function. Alphabetical ordering can be added later if the collection becomes large enough to require it.

## Keep headings purposeful

Use headings only when they create a meaningful category or navigation boundary. Avoid creating a heading for every term.

Prefer:

```markdown
## System vocabulary

- **Type:** ...
- **Strategy:** ...
- **Authority:** ...
```

Avoid:

```markdown
## Type

Definition...

## Strategy

Definition...
```

The second form makes a compact dictionary behave like a collection of miniature articles and increases visual and context overhead.

## Definition rules

### Be concise

Aim for one sentence. Use a second sentence only for an important boundary, qualification, or distinction.

### Be stable

Define the term in a way that can remain valid as the vault grows. Avoid embedding temporary examples or personal interpretations in the canonical definition.

### Be explicit about scope

Terms from an esoteric system, a practitioner tradition, and empirical research should not sound interchangeable.

Useful qualifiers include:

- “Within Human Design…”
- “In this vault…”
- “Some practitioners interpret…”
- “This claim requires evidence outside the system…”

### Avoid false completeness

If a meaning varies by school or remains unresolved, say so briefly rather than selecting one interpretation silently.

## Dictionary versus index versus glossary

These functions are related but distinct:

- **Dictionary:** defines shared terms and stabilizes language.
- **Index:** points to the available notes or entities.
- **Glossary:** provides quick reader orientation, often for a specific document.
- **Ontology:** models relationships, categories, and constraints between entities.

A compact dictionary may link to an index and gradually become an ontology interface, but it should not be forced to perform all four functions at once.

## Quality checks

Before adding or revising an entry, ask:

- Is this term used in more than one note?
- Does the entry establish a shared meaning?
- Is it short enough to scan?
- Is the source scope clear?
- Does it duplicate a deeper note unnecessarily?
- Would a link be more useful than another paragraph?
- Have uncertainty and disagreement been preserved?

## Anti-patterns

Avoid:

- turning every entry into a full essay;
- repeating the same definition across many pages;
- hiding interpretation inside an apparently factual definition;
- mixing source traditions without attribution;
- adding headings solely because a term exists;
- filling unknown fields with plausible-sounding prose;
- creating a large ontology before the vocabulary has stabilized.

## Design principle

> The dictionary is a stable interface between human understanding, machine navigation, and deeper knowledge—not the place where all knowledge must live.

This practice supports clarity, modularity, incremental growth, and lower context overhead while preserving links to richer material.
