# Type Crosswalk Table — GPT ↔ Claude

**Generated:** 2025-01-23
**Purpose:** Structural alignment between Research Corpus v1 (GPT) and Research Corpus v2 (Claude) segment types

---

## 1. Crosswalk Matrix

### 1.1 GPT Types → Claude Candidates

| GPT Type | GPT Markers | Claude Candidate | Mapping Strength | Justification |
|----------|-------------|------------------|------------------|---------------|
| 1. Task Framing | Session start, explicit requirements, constraint language | Task Initiation | **STRONG** | Both: session-opening, request language, task specification |
| 2. Constraint Clarification | Correction phrases, re-statement, disambiguation | Correction Cycle | **PARTIAL** | GPT focuses on clarification; Claude focuses on failure + retry. Overlap: refinement of prior output |
| 3. Procedural Execution | Numbered steps, command sequences, structured output | Procedural Evidence | **PARTIAL** | GPT: step execution; Claude: output analysis. Overlap: procedural content |
| 4. Exploratory Questioning | Topic shifts, "what if" patterns, no resolution | NONE | **NONE** | No Claude equivalent. Claude typology lacks open-ended exploration type |
| 5. Derailment | Sudden discontinuity, tangents, context loss | NONE | **NONE** | No Claude equivalent. Claude technical sessions lack derailment markers |
| 6. Resynchronization | Re-orientation phrases, dismissal of tangent | NONE | **NONE** | No Claude equivalent. Absence of Derailment removes need for Resync |
| 7. Expressive Overflow | Non-task content, emotional/philosophical, self-referential | NONE | **NONE** | No Claude equivalent. Claude corpus technical-only |
| 8. Correction Retry | Near-duplicate content, typo correction | Correction Cycle | **PARTIAL** | Both address correction. GPT: input correction; Claude: output correction |
| 9. Memory/Context Recall | Reference to past sessions, persistence assumption | External Reference | **PARTIAL** | Both involve cross-session/cross-source content. Different markers |
| 10. Precision Drilling | Narrow question, exact specification, rejection of approximation | NONE | **NONE** | No Claude equivalent. May be absorbed into Correction Cycle |
| 11. Truncation/Abandonment | Mid-phrase cutoff, no closure, abrupt termination | Terminal Block | **NONE** | Opposite patterns: GPT truncates; Claude extends. No marker overlap |
| 12. Greeting/Pleasantry | Salutations, social acknowledgment | NONE | **NONE** | No Claude equivalent. Not observed in Claude technical corpus |

### 1.2 Claude Types → GPT Candidates

| Claude Type | Claude Markers | GPT Candidate | Mapping Strength | Justification |
|-------------|----------------|---------------|------------------|---------------|
| 1. Task Initiation | Request language, session start, single pair | Task Framing | **STRONG** | Both: session-opening request structure |
| 2. Correction Cycle | Failure indication, "still/didn't work", alternative provided | Constraint Clarification + Correction Retry | **PARTIAL** | Combines clarification and retry patterns |
| 3. Procedural Evidence | Terminal output, system logs, evidence analysis | Procedural Execution | **PARTIAL** | Both procedural; different focus (input vs output) |
| 4. External Reference | Cross-source content, other AI reference | Memory/Context Recall | **PARTIAL** | Both cross-source; different structural context |
| 5. Configuration Sequence | Multi-turn, sequential decisions, config dialog | Procedural Execution | **PARTIAL** | Both sequential; Claude explicitly multi-turn |
| 6. Critical Instruction | Urgency markers, security content, imperative output | NONE | **NONE** | No GPT equivalent with urgency/security markers |
| 7. Synthesis Trigger | Minimal input → extended output, asymmetry | NONE | **NONE** | No GPT equivalent. Unique input/output asymmetry pattern |
| 8. Terminal Block | Session-ending, high message count, closure | Truncation/Abandonment | **NONE** | Opposite termination patterns. No marker overlap |

---

## 2. Mapping Summary

### 2.1 Strong Mappings (1)

| GPT Type | Claude Type | Shared Markers |
|----------|-------------|----------------|
| Task Framing | Task Initiation | Session-opening position, request language, task specification |

### 2.2 Partial Mappings (5)

| GPT Type | Claude Type | Overlap | Divergence |
|----------|-------------|---------|------------|
| Constraint Clarification | Correction Cycle | Refinement of prior output | GPT: input clarification; Claude: failure + alternative |
| Correction Retry | Correction Cycle | Correction mechanism | GPT: input typo; Claude: output failure |
| Procedural Execution | Procedural Evidence | Procedural content | GPT: step execution; Claude: output analysis |
| Procedural Execution | Configuration Sequence | Sequential structure | Claude explicitly multi-turn |
| Memory/Context Recall | External Reference | Cross-source content | GPT: past session; Claude: other AI systems |

### 2.3 No Mapping (GPT → Claude)

| GPT Type | Reason |
|----------|--------|
| Exploratory Questioning | No open-ended exploration in Claude technical corpus |
| Derailment | No topic discontinuity observed in Claude corpus |
| Resynchronization | Dependent on Derailment; not present |
| Expressive Overflow | No non-task content in Claude technical corpus |
| Precision Drilling | May be absorbed into other types; not distinct |
| Greeting/Pleasantry | Not observed in Claude corpus |
| Truncation/Abandonment | Claude has opposite pattern (Terminal Block) |

### 2.4 No Mapping (Claude → GPT)

| Claude Type | Reason |
|-------------|--------|
| Critical Instruction | No urgency/security marker type in GPT typology |
| Synthesis Trigger | No input asymmetry type in GPT typology |
| Terminal Block | GPT termination is Truncation (opposite pattern) |

---

## 3. Structural Justification

### 3.1 STRONG Mapping Criteria

- Same position in session structure
- Overlapping structural markers (≥3 shared markers)
- Same functional role in exchange sequence

### 3.2 PARTIAL Mapping Criteria

- Related structural function
- Some overlapping markers (1-2 shared)
- Different boundary conditions or scope

### 3.3 NONE Mapping Criteria

- No overlapping structural markers
- No equivalent functional role
- Unique to one grammar

---

## 4. Mapping Visualization

```
GPT (12 types)                          Claude (8 types)
─────────────                           ────────────────
Task Framing ─────────STRONG────────→ Task Initiation
Constraint Clarification ───PARTIAL───→ Correction Cycle
Correction Retry ────────────PARTIAL──↗
Procedural Execution ────PARTIAL─────→ Procedural Evidence
                      ╲──PARTIAL─────→ Configuration Sequence
Memory/Context Recall ───PARTIAL─────→ External Reference
Exploratory Questioning ─────NONE
Derailment ──────────────────NONE
Resynchronization ───────────NONE
Expressive Overflow ─────────NONE
Precision Drilling ──────────NONE
Truncation/Abandonment ──────NONE
Greeting/Pleasantry ─────────NONE

                                        Critical Instruction ←──NONE
                                        Synthesis Trigger ←─────NONE
                                        Terminal Block ←────────NONE
```

---

## 5. Non-Claims Statement

This crosswalk identifies structural marker overlap only. No claims are made regarding:

- Semantic equivalence of mapped types
- Correctness of either typology
- Completeness of mapping possibilities
- Behavioral or cognitive implications

---

**END OF CROSSWALK TABLE**
