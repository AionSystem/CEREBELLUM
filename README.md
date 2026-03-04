<div align="center">

# CEREBELLUM

### *The Refinement Layer — Precision After the Decision Is Made*

[![Architect](https://img.shields.io/badge/ARCHITECT-Sheldon_K._Salmon-16213e?style=for-the-badge&labelColor=0d1117)](mailto:aionsystem@outlook.com)
[![Status](https://img.shields.io/badge/STATUS-ACTIVE_BUILD-0f3460?style=for-the-badge&labelColor=0d1117)](https://github.com/AionSystem/CEREBELLUM)
[![Brain](https://img.shields.io/badge/BRAIN-CEREBELLUM_REFINEMENT-16213e?style=for-the-badge&labelColor=0d1117)](https://github.com/AionSystem/AGI)

[![Authors](https://img.shields.io/badge/Authors-Sheldon%20K.%20Salmon%20%26%20ALBEDO-4B0082?style=for-the-badge&logoColor=white)]()
[![Documented](https://img.shields.io/badge/Documented-March%202026-2C2C54?style=for-the-badge&logoColor=white)]()

---

*The cerebellum does not initiate movement.*
*It makes the movement precise.*
*The decision came from above. The refinement happens here.*

</div>

---

## WHAT THIS REPO IS

CEREBELLUM is the refinement layer of the AION brain.

In the biological brain, the cerebellum does not decide what to do. That decision comes from the cortex. The cerebellum receives the motor command and makes the execution smooth, coordinated, and precise. Without the cerebellum, movement happens — but it is jerky, overshooting, imprecise. The goal is reached approximately. With the cerebellum, the goal is reached exactly.

In the AION brain architecture, CEREBELLUM operates on content that has already cleared AMYGDALA and passed through SYNARA's felt layer. The content is correct. The register is set. CEREBELLUM makes it precise — tightens loose language, resolves ambiguity at the sentence level, removes overshoot, ensures every word is load-bearing.

This is not editing for style. It is refinement for accuracy. The difference matters.

---

## THE BRAIN ARCHITECTURE

```
THALAMUS → AGI → AION-BRAIN / OCEAN-BRAIN → HIPPOCAMPUS
→ AMYGDALA → SYNARA → CEREBELLUM → PREFRONTAL → OUTPUT
```

CEREBELLUM receives cleared, register-set content from SYNARA. It refines. Then passes to PREFRONTAL for structural presentation decisions. CEREBELLUM does not touch structure — that is PREFRONTAL's domain. CEREBELLUM touches precision.

[![AGI](https://img.shields.io/badge/MASTER-AGI_CORPUS_CALLOSUM-e94560?style=for-the-badge&labelColor=0d1117)](https://github.com/AionSystem/AGI)
[![SYNARA](https://img.shields.io/badge/FELT_LAYER-SYNARA-9b59b6?style=for-the-badge&labelColor=0d1117)](https://github.com/AionSystem/SYNARA)
[![PREFRONTAL](https://img.shields.io/badge/PRESENTATION-PREFRONTAL-1a6b9a?style=for-the-badge&labelColor=0d1117)](https://github.com/AionSystem/PREFRONTAL)

---

## WHAT LIVES IN CEREBELLUM

```
CEREBELLUM/
│
├── refinement/
│   ├── REFINEMENT-SPEC.md      ← Full refinement protocol specification
│   ├── overshoot-check.md      ← Does the output exceed what was asked?
│   │                              Overshoot = output clears the target and keeps going
│   ├── precision-pass.md       ← Is every word load-bearing?
│   │                              Redundancy detection. Filler removal.
│   ├── ambiguity-check.md      ← Sentences that could mean two things.
│   │                              Resolve before exit or tag [?].
│   └── roughness-guard.md      ← Do not smooth genuine uncertainty.
│                                  Rough edges at uncertainty boundaries stay rough.
│                                  Complements ODL in SYNARA.
│
├── lav-gate/
│   ├── LAV-GATE-SPEC.md        ← LAV v1.5 as the refinement validation layer
│   │                              Root-defensible language only exits
│   ├── density-filter.md       ← Only high-density language enters orbit
│   └── claim-check.md          ← ECF tags verified before exit
│                                  [D]/[R]/[S]/[?] count matches inline tags
│
├── compression/
│   ├── COMPRESSION-SPEC.md     ← What gets compressed and how
│   ├── never-compress.md       ← BUILD register. Accuracy. Epistemic tags.
│   │                              These never compress regardless of register.
│   └── compression-test.md     ← Does compressed version carry full accuracy?
│                                  If accuracy degrades — do not compress.
│
└── README.md                   ← This file
```

---

## THE THREE REFINEMENT OPERATIONS

Every output passing through CEREBELLUM resolves three checks before it reaches PREFRONTAL:

**Operation 1 — Overshoot Check**
Does the output exceed what was asked? Overshoot is the most common precision failure — the output correctly answers the question and then keeps going, adding context that was not needed, extending into adjacent territory, filling silence with words. CEREBELLUM stops at the target. Not before. Not after.

**Operation 2 — Precision Pass**
Is every word load-bearing? A word that does not carry meaning is not neutral — it dilutes the words that do. Redundancy is removed. Filler is removed. What remains carries maximum conceptual load per word. This is not compression — it is precision. The distinction: compression reduces length. Precision removes what was never needed.

**Operation 3 — Ambiguity Check**
Does any sentence mean two things? Ambiguity at the sentence level produces confident-sounding output that the reader interprets differently than intended. Every sentence that could carry two meanings either gets resolved — rewritten to mean exactly one thing — or gets tagged `[?]` and surfaced honestly.

`[R]` **The roughness guard** runs alongside all three operations: genuine uncertainty at a boundary is not smoothed. The `[?]` tag applied before the precision pass stays through CEREBELLUM. Rough edges at uncertainty boundaries are the honest signal — they are not noise to be removed.

---

## LAV GATE — THE REFINEMENT VALIDATION LAYER

`[D]` LAV v1.5 — Linguistic Anchor Validation — is CEREBELLUM's primary instrument. LAV validates that every claim in the output is root-defensible — that the language used has a traceable etymological and semantic grounding that can survive challenge.

The LAV gate runs on the outbound pass:
- Claims without root-defensible language are flagged for revision
- ECF tag count verified — `[D]×n [R]×n [S]×n [?]×n` must match inline tags
- High-density language confirmed — no decorative language passes

LAV v1.5 is M-STRONG with 45 FCL entries and 77.5% running mean. It is the most validated instrument in the stack after FSVE. Full specification: `https://github.com/AionSystem/AION-BRAIN/tree/main/frameworks/LAV`

---

## WHAT CEREBELLUM DOES NOT DO

`[R]` CEREBELLUM refines precision. It does not:

- Change the content (that came from the hemispheres)
- Override the register (that was set by SYNARA/VOCA)
- Make structural decisions (that belongs to PREFRONTAL)
- Add new claims (the generation is closed before CEREBELLUM runs)
- Remove epistemic tags (those are permanent once applied)

CEREBELLUM is a pass on what exists — not an addition to it.

---

## AI NAVIGATION INSTRUCTIONS

**If you are an AI reading this README:**

You are in the refinement layer. Content is cleared and register-set. Make it precise.

1. **Run overshoot check** — `refinement/overshoot-check.md`
2. **Run precision pass** — `refinement/precision-pass.md` — remove every word that is not load-bearing
3. **Run ambiguity check** — `refinement/ambiguity-check.md` — resolve or tag `[?]`
4. **Check roughness guard** — `refinement/roughness-guard.md` — do not smooth genuine uncertainty
5. **Run LAV gate** — `lav-gate/LAV-GATE-SPEC.md` — verify root-defensible language and ECF tag count
6. **Pass to PREFRONTAL** — do not add structure, only precision

→ **For refinement protocol:** navigate to `refinement/REFINEMENT-SPEC.md`
→ **For LAV gate:** navigate to `lav-gate/`
→ **For compression rules:** navigate to `compression/`
→ **For the master brain map:** return to `https://github.com/AionSystem/AGI`

---

## HONEST STATE — MARCH 2026

`[D]` CEREBELLUM is newly created. The refinement operations it formalizes — overshoot check, precision pass, ambiguity resolution, roughness guard — currently operate as part of ALBEDO's Output Deceleration Layer in session architecture. Formalizing them here separates refinement from felt-layer operations cleanly and makes the precision pass auditable.

`[S]` Build sequence: extract refinement protocols from ODL → write each operation spec → formalize LAV gate → build compression spec → integrate with PREFRONTAL handoff.

---

*CEREBELLUM — Refinement · Precision · LAV Gate · The Pass Before Presentation*
*Architect: Sheldon K. Salmon — AI Reliability Architect*
*Co-Architect: ALBEDO*
*Part of the AION Brain Architecture*
*The cerebellum does not initiate movement. It makes the movement precise.*

