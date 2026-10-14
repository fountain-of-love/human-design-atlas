# Human Design Content

This directory contains the Human Design content layer. It is intentionally separate from:

- `meta/vault/` — general knowledge-engineering practices;
- `meta/human-design/` — Human Design-specific dictionaries, specifications, indexes, source models, and audits.

The governing boundary is defined in [human-design-boundaries.md](../meta/human-design/human-design-boundaries.md), while the more formal roadmap is maintained in [human-design-fishbone.md](../meta/human-design/human-design-fishbone.md).

The content layer is organized as a fishbone spine: a central learning path with expandable branches. The branches are not a demand to write everything immediately; they are a visible map for incremental growth.

## Fishbone spine

```text
Human Design
│
├── Orientation
│   ├── What Human Design is
│   ├── BodyGraph
│   ├── Design and Personality
│   └── How to approach it experimentally
│
├── Chart Mechanics
│   ├── Birth data
│   ├── Design date
│   ├── 13 planetary elements
│   ├── Gates and Lines
│   └── Activations
│
├── Energy Mechanics
│   ├── Five Types
│   ├── Strategy
│   ├── Authority
│   ├── Signature
│   └── Not-Self Theme
│
├── BodyGraph Structure
│   ├── Nine Centers
│   ├── Channels
│   ├── Definition
│   ├── Split types
│   └── Circuitry
│
├── Archetypal Layer
│   ├── 64 Gates
│   ├── Six Lines
│   ├── 36 Channels
│   ├── Profiles
│   └── Incarnation Crosses
│
├── Interpretive Interfaces
│   ├── I Ching interface
│   ├── Astrology interface
│   ├── Gene Keys interface
│   ├── Chakra interface
│   └── Scientific commentary interface
│
└── Application
    ├── Reading method
    ├── Contemplative practice
    ├── Case studies
    └── Questions and experiments
```

## Current content

### Orientation

- [Human Design basics](HUMAN-DESIGN-BASICS.md)
- [The 13 elements](HUMAN-DESIGN-13-ELEMENTS.md)

### Energy Mechanics

- [Generator](types/generator.md)
- [Manifesting Generator](types/manifesting-generator.md)
- [Projector](types/projector.md)
- [Manifestor](types/manifestor.md)
- [Reflector](types/reflector.md)
- [Type](concepts/type.md)
- [Strategy](concepts/strategy.md)
- [Authority](concepts/authority.md)
- [Signature](concepts/signature.md)
- [Not-Self Theme](concepts/not-self-theme.md)

### Chart Mechanics

- [Design and Personality](concepts/design-and-personality.md)
- [Activation](concepts/activation.md)

### Application

- [Yves’s chart case study](case-studies/yves-chart.md)

## Growth order

The next content slices should be developed vertically rather than as isolated lists:

1. Complete the decision-mechanics slice: Type → Strategy → Authority → Signature → Not-Self Theme.
2. Build the nine Centers as the first BodyGraph structure branch.
3. Add the planetary elements and activations as a chart-mechanics branch.
4. Add a small, representative set of Gates and Channels before expanding toward all 64 and 36.
5. Add Profiles and Incarnation Crosses after the chart mechanics are stable.

Each new branch should use the [Human Design page specification](../meta/human-design/human-design-spec.md) and remain inside the boundaries defined by the [Human Design dictionary](../meta/human-design/human-design-dictionary.md).
