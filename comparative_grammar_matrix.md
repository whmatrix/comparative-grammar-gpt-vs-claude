# Comparative Grammar Matrix — GPT ↔ Claude

**Generated:** 2025-01-23
**Status:** Structure-only comparison of validated interaction grammars

---

## A. Grammar Summary

### A.1 GPT Grammar (Research Corpus v1)

| Metric | Value | Source |
|--------|-------|--------|
| Type count | 12 | segment_typology_map.md |
| Validation status | VALIDATED (LIMITED) / STABLE WITH NOTES | phase_4b_typology_validation.md |
| Sessions | 6 | phase_4a_ingestion_summary.md |
| Segments | 37 | phase_4b_typology_validation.md |
| Turns | ~108 | phase_4a_ingestion_summary.md |
| Hybrid rate | 16.2% (6/37) | phase_4b_typology_validation.md |
| Forced classifications | 0 | phase_4b_typology_validation.md |
| Export era | May 2025 | segment_typology_map.md |

### A.2 Claude Grammar (Research Corpus v2)

| Metric | Value | Source |
|--------|-------|--------|
| Type count | 8 | segment_typology_map.md |
| Validation status | VALIDATED WITH NOTES / STABLE | phase_4b_typology_validation.md |
| Sessions | 8 | phase_4a_ingestion_summary.md (Phase 4A′) |
| Segments | 80 | phase_4a_ingestion_summary.md (Phase 4A′) |
| Messages | 464 | phase_4a_ingestion_summary.md (Phase 4A′) |
| Hybrid rate | 10.2% (5/49 at Phase 4B) | phase_4b_typology_validation.md |
| Forced classifications | 0 | phase_4b_typology_validation.md |
| Export era | July-October 2025 | phase_4a_ingestion_summary.md |

### A.3 Grammar Size Comparison

| Dimension | GPT | Claude | Ratio |
|-----------|-----|--------|-------|
| Type count | 12 | 8 | 1.5:1 |
| Sessions | 6 | 8 | 1:1.3 |
| Segments | 37 | 80 | 1:2.2 |
| Segments/session | 6.2 | 10.0 | 1:1.6 |

---

## B. Structural Invariants

Types or patterns observed in both grammars with similar structural function.

### B.1 Session Initiation

| Invariant | GPT Type | Claude Type | Shared Markers |
|-----------|----------|-------------|----------------|
| Opening task specification | Task Framing | Task Initiation | Request language, session start, explicit constraints |

**Evidence:**
- GPT: "Appears at or near session start" (segment_typology_map.md L38)
- Claude: "Typically occurs at session start" (segment_typology_map.md L40)
- Both: Single exchange pair as typical size

### B.2 Correction Mechanism

| Invariant | GPT Types | Claude Type | Shared Markers |
|-----------|-----------|-------------|----------------|
| Error-triggered refinement | Constraint Clarification, Correction Retry | Correction Cycle | Correction language, modified output |

**Evidence:**
- GPT Constraint Clarification: "Correction phrases" (L54)
- GPT Correction Retry: "Near-duplicate message content" (L150)
- Claude Correction Cycle: "Failure indication in HUMAN input" (L61)
- Both involve re-processing of prior exchange

### B.3 Procedural Content

| Invariant | GPT Type | Claude Types | Shared Markers |
|-----------|----------|--------------|----------------|
| Step-based exchange | Procedural Execution | Procedural Evidence, Configuration Sequence | Structured content, sequential flow |

**Evidence:**
- GPT: "Sequential step-by-step work" (L67)
- Claude Procedural Evidence: "execution output, terminal logs" (L74)
- Claude Configuration Sequence: "sequential configuration decisions" (L110)
- Both involve structured, ordered content

### B.4 Cross-Source Reference

| Invariant | GPT Type | Claude Type | Shared Markers |
|-----------|----------|-------------|----------------|
| External content integration | Memory/Context Recall | External Reference | Reference to content outside current session |

**Evidence:**
- GPT: "Reference to past discussions" (L166)
- Claude: "content or analysis from source outside the current session" (L92)
- Both trigger distinct processing of external material

---

## C. Structural Divergences

Types or patterns unique to one grammar or with opposite structural behavior.

### C.1 Claude-Only Types

| Claude Type | Primary Marker | GPT Equivalent | Divergence Reason |
|-------------|----------------|----------------|-------------------|
| Synthesis Trigger | Minimal input → extended output | NONE | GPT lacks input/output asymmetry type |
| Critical Instruction | Urgency/security markers, imperative output | NONE | GPT lacks urgency-differentiated type |
| Terminal Block | Session-ending multi-turn continuation | NONE | GPT termination is truncation (opposite) |

**Synthesis Trigger Detail:**
- Marker: "Empty, single-character, or minimal HUMAN message" + "Extended ASSISTANT response" (Claude L151-153)
- Pattern: Structural asymmetry where minimal input produces substantial output
- No GPT type captures this input/output ratio pattern

**Critical Instruction Detail:**
- Marker: "Security, permissions, or critical system content" + "Imperative language in ASSISTANT output" (Claude L134-135)
- Pattern: Urgency-differentiated exchange
- GPT Procedural Execution lacks urgency markers

**Terminal Block Detail:**
- Marker: "Extended multi-turn segment occurring at session end" + "High message count (5+ messages)" (Claude L165-172)
- Pattern: Session continues with multiple exchanges before closure
- Opposite of GPT Truncation/Abandonment (abrupt termination)

### C.2 GPT-Only Types

| GPT Type | Primary Marker | Claude Equivalent | Divergence Reason |
|----------|----------------|-------------------|-------------------|
| Exploratory Questioning | Topic shifts, "what if", no resolution | NONE | Claude technical corpus lacks open-ended exploration |
| Derailment | Sudden discontinuity, context loss | NONE | Claude sessions maintain topic continuity |
| Resynchronization | Re-orientation after tangent | NONE | Dependent on Derailment; not present |
| Expressive Overflow | Non-task content, philosophical | NONE | Claude corpus technical-only |
| Precision Drilling | Narrow question, exact specification | NONE | May be absorbed into Correction Cycle |
| Greeting/Pleasantry | Salutations | NONE | Not observed in Claude corpus |

**Exploratory Questioning Detail:**
- Marker: "Topic shifts between turns without explicit transition" (GPT L86)
- Pattern: Open-ended questioning without task frame
- Claude corpus exhibits task-oriented structure throughout

**Derailment/Resynchronization Detail:**
- GPT: "Sudden topic discontinuity" (L101) followed by "explicit re-orientation" (L117)
- Pattern: Deviation-recovery pair
- Claude sessions lack topic deviation markers

**Expressive Overflow Detail:**
- Marker: "Extended segment dominated by non-task content" (GPT L130)
- Pattern: High token density without task progression
- Claude corpus contains no non-task extended content

### C.3 Opposite Termination Patterns

| Dimension | GPT | Claude |
|-----------|-----|--------|
| Type | Truncation/Abandonment | Terminal Block |
| Marker | "Sentence ends mid-phrase" (L198) | "High message count (5+ messages)" (L172) |
| Pattern | Abrupt, incomplete | Extended, multi-turn |
| Closure | No closing acknowledgment | "Closure or summary language" (L168) |

**Structural Observation:**
- GPT sessions terminate via truncation (incomplete)
- Claude sessions terminate via extended continuation (complete)
- This represents opposite terminal mechanics in the two grammars

---

## D. Closure Mechanics

### D.1 GPT Termination Structure

| Pattern | Type | Marker |
|---------|------|--------|
| Abrupt termination | Truncation/Abandonment | Mid-phrase cutoff, no closure |
| No multi-turn closure type | (absent) | N/A |

**Source:** segment_typology_map.md L193-207

**Observed in:** 3/6 sessions (phase_4b_typology_validation.md L186)

### D.2 Claude Termination Structure

| Pattern | Type | Marker |
|---------|------|--------|
| Extended continuation | Terminal Block | 5+ messages, closure language |
| Synthesis at resolution | Synthesis Trigger | Minimal input → extended summary |

**Source:** segment_typology_map.md L162-178, L144-159

**Observed in:**
- Terminal Block: 5/5 sessions at Phase 4B (phase_4b_typology_validation.md L157)
- Synthesis Trigger: Often follows procedural exchanges (segment_typology_map.md L154)

### D.3 Continuation Behavior Comparison

| Behavior | GPT | Claude |
|----------|-----|--------|
| Empty ASSISTANT responses | Not documented | Documented: "Occur when HUMAN continues without pause" (L231) |
| Minimal HUMAN inputs | Correction Retry pattern | Synthesis Trigger pattern |
| Session extension | Absent | Terminal Block (3+ pairs) |

### D.4 Resolution Mechanics

| Phase | GPT Pattern | Claude Pattern |
|-------|-------------|----------------|
| Task completion | No dedicated type | Synthesis Trigger (minimal input → summary) |
| Session closure | Truncation/Abandonment | Terminal Block (extended multi-turn) |
| Recovery from deviation | Resynchronization | Not required (no Derailment) |

---

## E. Residual Uncertainty

### E.1 Mapping Ambiguities

| Mapping | Ambiguity | Source |
|---------|-----------|--------|
| Constraint Clarification ↔ Correction Cycle | GPT clarification vs Claude failure-retry distinction | Both typology maps |
| Procedural Execution ↔ Configuration Sequence | Multi-turn boundary unclear | Claude segment_typology_map.md L225 |
| Memory/Context Recall ↔ External Reference | Cross-session vs cross-platform distinction | Both typology maps |

### E.2 Edge Cases from Validation

| Corpus | Edge Case | Source |
|--------|-----------|--------|
| GPT | "Procedural execution (conceptual)" — qualified classification | phase_4b_typology_validation.md L121-125 |
| Claude | Multi-turn Synthesis Trigger — definitional gap | phase_4b_typology_validation.md L227-233 |
| Claude | Handoff as Task Initiation — hybrid with External Reference | phase_4b_typology_validation.md L235-241 |

### E.3 Corpus Limitations

| Limitation | GPT | Claude |
|------------|-----|--------|
| Sample size | 6 sessions, 37 segments | 8 sessions, 80 segments |
| Era | May 2025 | July-October 2025 |
| Model family | GPT-4 (OpenAI) | Claude (Anthropic) |
| Operator | Single user | Same single user |
| Task domain | Mixed (practice exams, personal, analysis) | Technical (debugging, configuration, security) |
| Export format | ChatGPT conversations.json | Claude conversations.json |

### E.4 Comparability Constraints

| Constraint | Impact |
|------------|--------|
| Different task domains | Some types may be domain-specific (Expressive Overflow, Critical Instruction) |
| Same operator | Interaction patterns may reflect operator style, not model behavior |
| Different export structures | Extraction artifacts may differ between corpora |
| Non-overlapping timeframes | Model behavior may have changed between eras |

---

## F. Non-Claims Boundary

This comparative grammar matrix does NOT claim:

### F.1 Equivalence Claims
- Types with STRONG mapping are NOT semantically equivalent
- Structural similarity does NOT imply functional equivalence
- Grammar size difference does NOT indicate completeness

### F.2 Quality Claims
- Neither grammar is "better" or "more complete"
- Type count does NOT indicate grammar sophistication
- Validation status does NOT indicate correctness

### F.3 Behavioral Claims
- Divergences do NOT indicate model capabilities
- GPT-only types do NOT mean Claude cannot exhibit those patterns
- Claude-only types do NOT mean GPT cannot exhibit those patterns

### F.4 Scope Claims
- Comparison limited to validated corpus material
- No extrapolation to unsampled sessions
- No extrapolation to other operators or timeframes

### F.5 Cognitive Claims
- No claims about reasoning, understanding, or intelligence
- No claims about alignment or safety properties
- No claims about "relationship" or interaction quality

---

## G. Summary Table

| Dimension | GPT Grammar | Claude Grammar |
|-----------|-------------|----------------|
| Types | 12 | 8 |
| Validation | VALIDATED (LIMITED) | VALIDATED WITH NOTES |
| Strong mappings | 1 | 1 |
| Partial mappings | 5 | 5 |
| Unique types | 7 | 3 |
| Termination pattern | Truncation (abrupt) | Terminal Block (extended) |
| Continuation types | 0 | 2 (Synthesis Trigger, Terminal Block) |
| Deviation-recovery types | 2 (Derailment, Resync) | 0 |
| Non-task types | 2 (Expressive, Greeting) | 0 |

---

**END OF COMPARATIVE GRAMMAR MATRIX**
