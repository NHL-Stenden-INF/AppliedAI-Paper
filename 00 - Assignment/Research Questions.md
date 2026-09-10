# Research Questions

Source for the current wording: `Research paper Subject.xlsx` (`Blad1`, row 3).

## Problem Statement

**Inferred from the registered topic/questions:** AI-based deepfake detectors are intended to distinguish manipulated/AI-generated media from authentic content, but the current proposal specifically questions how dependable that distinction remains across techniques, evaluation conditions and degrading factors.

This is not a school-provided or lecturer-approved problem statement.

## Research Objective

**Proposed:** determine the extent to which current AI-based deepfake detection can be considered reliable within a clearly defined scope by synthesising evidence on detection techniques, reported performance and conditions that reduce effectiveness.

The objective deliberately avoids promising a universal accuracy value.

## Main Research Question

**Status: Proposed / lecturer approval To Verify**

> To what extent can AI-based deepfake detection systems reliably distinguish AI-generated or manipulated media from authentic content?

## Main-Question Audit

| Check | Audit result |
| --- | --- |
| Relevant to Applied AI | Yes |
| Neutral / non-leading | Yes |
| Researchable | Yes, with existing empirical literature |
| Analytic rather than purely descriptive | Yes — `to what extent` requires evaluation |
| Feasible | **Conditional** — image, video and audio together may be broad for the time/page constraint |
| Key concept operationalised | No — `reliably` still needs explicit dimensions/criteria |
| Approval evidence | Missing |

No silent replacement is recommended before lecturer approval. The wording is coherent; the main risk is breadth and undefined evaluation terms rather than basic question quality.

## Subquestions

### SQ1

> Which AI and machine learning techniques are currently used to detect deepfake images, videos, and audio?

- **Function:** establish the detector landscape needed to interpret performance evidence.
- **MRQ contribution:** identifies what types of systems the reliability judgement concerns.
- **Evidence needed:** current primary and/or high-quality review evidence on detector approaches by modality.
- **Planned analysis:** taxonomy/thematic classification.
- **Risk:** can become a broad catalogue if not limited to technique families relevant to SQ2/SQ3.
- **Status:** Proposed / approval To Verify.

### SQ2

> How accurately can current deepfake detection systems identify manipulated content under real world conditions?

- **Function:** provide the core empirical evidence for reliability.
- **MRQ contribution:** evaluates performance rather than merely describing methods.
- **Evidence needed:** empirical results with metric, dataset, modality, detector/generator context and test conditions preserved.
- **Planned analysis:** contextual comparative synthesis; numerical pooling only when conditions are genuinely comparable.
- **Risk:** `real world conditions` is undefined and cannot be used as an evidence label until operationalised.
- **Status:** Proposed / approval To Verify.

### SQ3

> What factors, such as video compression, new generative models, or deliberate attempts to avoid detection, reduce the effectiveness of deepfake detection systems?

- **Function:** establish boundary conditions and failure modes.
- **MRQ contribution:** explains when reported performance does not generalise.
- **Evidence needed:** robustness/generalisation/evasion studies and any additional degradation factors discovered through the review.
- **Planned analysis:** thematic synthesis with direction/magnitude/context of effects where reported.
- **Risk:** the examples are not an exhaustive list and should not predetermine the only factors considered.
- **Status:** Proposed / approval To Verify.

## Subquestion Coverage

The sequence is logically complementary:

1. **What detection approaches are in scope?**
2. **How well do they perform under defined conditions?**
3. **What causes performance to degrade?**

No substantial overlap or missing question is currently evident. SQ1 should remain subordinate to the reliability purpose so it does not consume disproportionate space.

## Operational Definitions Required Before Evidence Extraction

Phase 2 must define, at minimum:

- `deepfake` / `AI-generated or manipulated media` for inclusion purposes;
- `current` as a publication/evidence window plus treatment of foundational older work;
- `reliably` using dimensions such as discriminatory performance, error behaviour, generalisation and robustness;
- `real-world conditions` as explicit test conditions rather than a rhetorical label;
- final modality coverage (image, video, audio or an approved narrower subset).

## Scope-Control Options — Proposed, Not Adopted

If early source mapping shows the three-modality scope is infeasible, discuss one of these with the lecturer rather than silently changing the approved proposal:

- retain all three modalities but compare only high-level technique/performance categories;
- narrow the empirical reliability comparison to one or two modalities while using the others only as context;
- narrow the time window or degradation-factor set.

Any change to the question wording remains subject to lecturer approval.