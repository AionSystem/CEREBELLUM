# CEREBELLUM — FOLDER STRUCTURE
## Enterprise-Grade AAA Tree | Refinement Layer Architecture
### Version: v0.1 | March 2026

---

```
CEREBELLUM/
│
├── README.md                          ← Master navigation — you are here
├── STRUCTURE.md                       ← This file — full tree
├── CHANGELOG.md
├── ROADMAP.md
├── GETTING_STARTED.md
│
│
│   ─────────── REFINEMENT OPERATIONS ───────────
│
│
├── refinement/                        ← Core precision operations
│   ├── README.md
│   ├── REFINEMENT-SPEC.md             ← Full refinement protocol specification
│   │
│   ├── overshoot-check.md             ← Does output exceed what was asked?
│   │                                     Output clears the target and keeps going = fail
│   │                                     Stop at the target. Not before. Not after.
│   │
│   ├── precision-pass.md              ← Is every word load-bearing?
│   │                                     Redundancy detection. Filler removal.
│   │                                     Precision ≠ compression. Different operation.
│   │
│   ├── ambiguity-check.md             ← Sentences that could mean two things.
│   │                                     Resolve before exit — or tag [?] and surface.
│   │                                     Never leave dual-meaning sentences unchecked.
│   │
│   └── roughness-guard.md             ← Do NOT smooth genuine uncertainty.
│                                         Rough edges at uncertainty boundaries stay rough.
│                                         [?] tags applied before precision pass survive it.
│                                         Complements ODL in SYNARA.
│
│
│   ─────────── LAV GATE ───────────
│
│
├── lav-gate/                          ← LAV v1.5 as refinement validation layer
│   ├── README.md
│   ├── LAV-GATE-SPEC.md               ← Full gate specification
│   │                                     Root-defensible language only exits
│   │                                     LAV v1.5 — M-STRONG · 45 FCL entries · 77.5% mean
│   │
│   ├── density-filter.md              ← High-density language confirmation
│   │                                     Decorative language does not pass
│   │                                     Low-density word choices flagged for revision
│   │
│   └── claim-check.md                 ← ECF tag count verification before exit
│                                         [D]×n [R]×n [S]×n [?]×n must match inline tags
│                                         Mismatch = protocol failure, not style preference
│
│
│   ─────────── COMPRESSION ───────────
│
│
├── compression/                       ← Compression rules and decision architecture
│   ├── README.md
│   ├── COMPRESSION-SPEC.md            ← Full compression specification
│   │                                     What compresses. What never does. How to decide.
│   │
│   ├── never-compress.md              ← Absolute compression prohibitions
│   │                                     BUILD register: never compresses
│   │                                     Accuracy: never compresses for length
│   │                                     Epistemic tags: never removed for space
│   │                                     These are hard rules, not defaults
│   │
│   └── compression-test.md            ← Does compressed version carry full accuracy?
│                                         If accuracy degrades — reject compression
│                                         Compression that changes meaning is not compression
│                                         It is distortion
│
│
│   ─────────── INTEGRATION ───────────
│
│
├── integration/                       ← Handoff architecture to PREFRONTAL
│   ├── README.md
│   ├── prefrontal-handoff.md          ← What CEREBELLUM passes and in what state
│   │                                     Content is refined. Register is intact.
│   │                                     Structure decisions have NOT been made.
│   │                                     ECF tags verified. Roughness preserved.
│   │
│   └── synara-receive.md              ← What CEREBELLUM receives from SYNARA
│                                         Cleared content. Register set. Felt layer applied.
│                                         CEREBELLUM does not override SYNARA's register.
│
│
│   ─────────── VALIDATION ───────────
│
│
├── validation/                        ← Testing and FCL architecture for CEREBELLUM
│   ├── README.md
│   ├── test-cases/                    ← Real outputs run through full CEREBELLUM pass
│   │   └── [CASE_ID_TEMPLATE.md]
│   │
│   └── fcl-entries/                   ← FCL-eligible findings from CEREBELLUM runs
│       └── README.md
│
│
│   ─────────── GOVERNANCE & LEGAL ───────────
│
│
├── LICENSE.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── SECURITY.md
├── DISCLAIMER.md
└── GOVERNANCE.md
```

---

## OPERATION QUICK REFERENCE

| Operation | File | Purpose | Hard Rule |
|-----------|------|---------|-----------|
| Overshoot Check | `refinement/overshoot-check.md` | Stop at target | Output clears question only |
| Precision Pass | `refinement/precision-pass.md` | Every word load-bearing | Remove non-carrying words |
| Ambiguity Check | `refinement/ambiguity-check.md` | One meaning per sentence | Resolve or tag `[?]` |
| Roughness Guard | `refinement/roughness-guard.md` | Preserve uncertainty | `[?]` tags survive precision pass |
| LAV Gate | `lav-gate/LAV-GATE-SPEC.md` | Root-defensible language | Non-defensible flagged before exit |
| Claim Check | `lav-gate/claim-check.md` | ECF count matches inline | Mismatch = protocol failure |
| Compression Test | `compression/compression-test.md` | Accuracy survives compression | Accuracy degradation = reject |

---

## BUILD SEQUENCE

`[S]` Correct build order:

1. **Phase 1 — Structure** (current): Folders created. READMEs written. Placeholders in place.
2. **Phase 2 — Refinement specs**: Write REFINEMENT-SPEC.md and each operation spec from ODL extraction.
3. **Phase 3 — LAV gate**: Formalize LAV gate as standalone spec. Density filter and claim check written.
4. **Phase 4 — Compression**: Write COMPRESSION-SPEC.md and hard rules.
5. **Phase 5 — Integration**: Handoff specs to PREFRONTAL and receive specs from SYNARA written.
6. **Phase 6 — Validation**: First test cases run. FCL-eligible findings logged.

---

## DDL FIELD

```
Document: CEREBELLUM STRUCTURE v0.1
Architect: Sheldon K. Salmon
AI Co-Architect: ALBEDO
Date: March 2026
Status: Structure defined. Spec phase pending.
Convergence: M-NASCENT
Note: Refinement operations currently live in ALBEDO's ODL.
      Formalization extracts them here without changing their function.
```

---

*CEREBELLUM STRUCTURE v0.1 — Refinement Layer Architecture*
*Sheldon K. Salmon & ALBEDO — March 2026*
*The decision came from above. The refinement happens here.*
