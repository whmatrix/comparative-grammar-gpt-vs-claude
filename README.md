> **Author:** John Mitchell (@whmatrix)

# Comparative Grammar — GPT vs Claude

**Generated:** 2025-01-23
**Status:** Derived from validated corpora; meta-layer only

---

## Purpose

Structural comparison of two validated interaction grammars:

- **Research Corpus v1 (Old GPT):** 12-segment typology
- **Research Corpus v2 (Old Claude):** 8-segment typology

This comparison identifies structural alignments, invariants, and divergences between the two independently derived typologies.

---

## Input Sources

This repository contains derived analytical outputs (grammar crosswalk, structural invariants).

Source material (raw dialogue transcripts and segment typology maps) is private. Each corpus was independently validated before this comparative layer was constructed.

For reproducibility, the derived analysis is fully contained in this repo:
- `type_crosswalk_table.md` — type-by-type mapping between both grammars
- `comparative_grammar_matrix.md` — structural invariants, divergences, closure mechanics

For the downstream infrastructure built on these grammars, see:
- [interaction-mechanics-index](https://github.com/whmatrix/interaction-mechanics-index) — Queryable FAISS index of dialogue segments
- [structural-collaboration-primitives](https://github.com/whmatrix/structural-collaboration-primitives) — Interaction primitives derived from these grammars

---

## Output Files

| File | Content |
|------|---------|
| README.md | This document |
| type_crosswalk_table.md | Type-by-type mapping between corpora |
| comparative_grammar_matrix.md | Structural invariants, divergences, closure mechanics |

---

## Methodology

1. **Type extraction:** Segment types, markers, and frequency bands extracted verbatim from each corpus typology map
2. **Crosswalk construction:** Structural marker overlap used for mapping (no semantic interpretation)
3. **Invariant identification:** Types present in both grammars with similar structural function
4. **Divergence documentation:** Types or patterns unique to one grammar

---

## Non-Claims Statement

This comparative layer does NOT claim:

- Equivalence or superiority of either grammar
- Correctness or quality of segment content
- Representativeness of sampled sessions
- Cognitive or behavioral meaning of segment patterns
- Applicability to other AI systems or corpora
- Capability or alignment implications

**Structure-only analysis.** All statements traceable to validation documents.

---

## Limitations

| Limitation | Description |
|------------|-------------|
| Era constraint | GPT: May 2025 export; Claude: Jul-Oct 2025 export |
| Model family | GPT-4 vs Claude (Anthropic) — different architectures |
| Operator | Single operator (same user) for both corpora |
| Export format | Different JSON structures; extraction artifacts possible |
| Sample size | GPT: 6 sessions, 37 segments; Claude: 8 sessions, 80 segments |

---

## Related

- [structural-collaboration-primitives](https://github.com/whmatrix/structural-collaboration-primitives) — Interaction primitives derived from these grammars
- [interaction-mechanics-index](https://github.com/whmatrix/interaction-mechanics-index) — Queryable FAISS index over dialogue segments using these primitives
