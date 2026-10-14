# Human Design Page Specification

This specification defines the reusable structure for concept pages in the Human Design Atlas.

## Scope

Use this contract for Types, Centers, Gates, Channels, Planets, Profiles, and core concepts. Case studies may use a modified version because they contain chart-specific data.

## Frontmatter

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

## Page contract

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

Not every page needs every section in equal depth. The headings make omissions visible and provide a stable navigation contract.

## Writing rules

- Start with an accessible explanation before specialist detail.
- Separate system description from practitioner interpretation.
- Use tables for stable, comparable facts and prose for nuance.
- Link recurring terms to the dictionary or canonical concept pages.
- Mark missing, disputed, or unverified information explicitly.
- Keep adjacent systems—Gene Keys, astrology, psychology, and science—clearly attributed.
- Avoid presenting contemplative interpretations as medical or psychological facts.
