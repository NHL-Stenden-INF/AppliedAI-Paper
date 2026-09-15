# Research Questions

Source for the current wording: `Research paper Subject.xlsx` (`Blad1`, row 3).

## Approval Status

**Lecturer approval: Confirmed by the authors on 12 September 2026.**

The title, main research question and all three subquestions below are treated as the approved question set for the current paper.

## Problem Statement

AI-based deepfake detectors are intended to distinguish manipulated or AI-generated media from authentic content, but their dependability may change across detector techniques, evaluation conditions, media modalities and degradation factors.

## Research Objective

Determine the extent to which current AI-based deepfake detection can be considered reliable within the approved scope by synthesising evidence on detection techniques, reported performance and conditions that reduce effectiveness. The objective deliberately avoids promising a universal accuracy value.

## Main Research Question

> To what extent can AI-based deepfake detection systems reliably distinguish AI-generated or manipulated media from authentic content?

## Main-Question Audit

| Check | Audit result |
| --- | --- |
| Relevant to Applied AI | Yes |
| Neutral / non-leading | Yes |
| Researchable | Yes, with existing empirical literature |
| Analytic rather than purely descriptive | Yes - `to what extent` requires evaluation |
| Feasible | Yes, when the three modalities are compared at technique/reliability level rather than exhaustively catalogued |
| Key concept operationalised | Yes in the executed paper - reliability is treated through performance, generalisation and robustness |
| Approval | Confirmed by authors |

## Subquestions

### SQ1

> Which AI and machine learning techniques are currently used to detect deepfake images, videos, and audio?

- **Function:** establish the detector landscape needed to interpret performance evidence.
- **MRQ contribution:** identifies what types of systems the reliability judgement concerns.
- **Executed analysis:** bounded taxonomy/thematic classification by modality and technique family.
- **Status:** Approved and answered in Results 3.1.

### SQ2

> How accurately can current deepfake detection systems identify manipulated content under real world conditions?

- **Function:** provide the core empirical evidence for reliability.
- **MRQ contribution:** evaluates performance rather than merely describing methods.
- **Executed analysis:** contextual comparison preserving metric, dataset, modality and test/generalisation conditions; incompatible metrics were not pooled.
- **Status:** Approved and answered in Results 3.2.

### SQ3

> What factors, such as video compression, new generative models, or deliberate attempts to avoid detection, reduce the effectiveness of deepfake detection systems?

- **Function:** establish boundary conditions and failure modes.
- **MRQ contribution:** explains when reported performance does not generalise.
- **Executed analysis:** thematic synthesis of compression/codecs, unseen generators, adversarial evasion, dataset/acquisition shift and evaluation-pipeline effects.
- **Status:** Approved and answered in Results 3.3.

## Subquestion Coverage

The sequence is complementary:

1. What detection approaches are in scope?
2. How well do they perform under defined conditions?
3. What causes performance to degrade?

The final paper keeps SQ1 subordinate to the reliability purpose so technique description does not replace analysis.

## Operational Definitions Used in the Paper

- `deepfake` / `AI-generated or manipulated media`: synthetic or manipulated image, video or audio content within the selected passive-detection literature.
- `current`: primarily 2020-2026 evidence, with FaceForensics++ (2019) retained as a directly relevant foundational benchmark.
- `reliably`: discriminatory performance combined with generalisation outside the training distribution and robustness to transformations or attacks.
- `real-world conditions`: conditions meaningfully different from controlled training benchmarks, including internet-sourced media, cross-dataset tests, unseen manipulation methods, compression/codecs, diverse recording conditions and adversarial evasion.
- modality scope: image, video and audio, compared at a level appropriate to the 8-10-page paper constraint.