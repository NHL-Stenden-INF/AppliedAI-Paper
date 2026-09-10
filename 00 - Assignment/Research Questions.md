# Research Questions

Source for current wording: `Research paper Subject.xlsx`.

## Problem Statement

**Inferred:** Deepfake detection systems are intended to distinguish manipulated or AI-generated media from authentic content, but their practical reliability may vary across media types and conditions. The current proposal focuses on understanding the detection techniques, reported performance and conditions that reduce effectiveness.

This is an interpretation of the current topic/questions, not an approved school-provided problem statement.

## Research Objective

**Proposed:** Evaluate how reliably current AI-based deepfake detection systems distinguish manipulated media from authentic content by synthesising evidence about detection techniques, reported real-world performance and known performance-degrading factors.

## Main Research Question

**Status: Proposed / lecturer approval To Verify**

> To what extent can AI-based deepfake detection systems reliably distinguish AI-generated or manipulated media from authentic content?

## Subquestions

### SQ1

> Which AI and machine learning techniques are currently used to detect deepfake images, videos, and audio?

- **Purpose:** establish and classify the current detection approaches across the three modalities.
- **Contribution to MRQ:** defines what technical approaches are being evaluated before judging reliability.
- **Required evidence:** recent, relevant sources describing detection approaches, inputs/features, model classes and modalities.
- **Likely method:** structured literature review and taxonomy/thematic synthesis.
- **Status:** Proposed / approval To Verify.

### SQ2

> How accurately can current deepfake detection systems identify manipulated content under real world conditions?

- **Purpose:** evaluate reported performance beyond idealised laboratory results.
- **Contribution to MRQ:** provides the main evidence for the degree of reliability.
- **Required evidence:** empirical evaluations, benchmark/cross-dataset results, realistic transformations or deployment-like conditions, reported metrics and test context.
- **Likely method:** comparative evidence synthesis; quantitative comparison only where metrics/conditions are sufficiently comparable.
- **Status:** Proposed / approval To Verify.

### SQ3

> What factors, such as video compression, new generative models, or deliberate attempts to avoid detection, reduce the effectiveness of deepfake detection systems?

- **Purpose:** identify the conditions under which reliability degrades.
- **Contribution to MRQ:** explains limitations and boundaries of reported performance.
- **Required evidence:** studies on compression/quality changes, cross-generator generalisation, unseen manipulations, adversarial/evasion techniques and modality-specific degradation.
- **Likely method:** thematic synthesis supported by comparative empirical evidence.
- **Status:** Proposed / approval To Verify.

## Research Question Coverage

The three subquestions form a logical sequence:

1. **What techniques exist?**
2. **How well do they perform?**
3. **Under what conditions does performance fall?**

Together they can support an evidence-based answer to `to what extent` the systems are reliable, provided reliability is operationalised before data extraction.

## Open Issues

- **Approval:** the module requires lecturer approval of the title, main question and subquestions before writing; no approval evidence is available.
- **Breadth:** images, video and audio together may be too broad for the assignment's volume constraint. This should be tested during initial source mapping and narrowed if necessary.
- **`Reliably`:** needs measurable criteria, potentially including discrimination metrics, generalisation, robustness and false-positive/false-negative behaviour.
- **`Real world conditions`:** needs an explicit operational definition rather than being used as a vague label.
- **`Current`:** needs a defined evidence time window.
- **Metric comparability:** image/video and audio detection may use different metrics, datasets and protocols. Direct numerical ranking may be invalid without normalisation/context.

## Proposed Improvements — Do Not Replace Without Approval

The current questions are coherent and aligned. Any narrowing should preserve the approved wording unless a lecturer agrees to a revision. Possible scope controls for discussion with the lecturer include limiting the comparison to a defined date range, specifying the operational meaning of real-world conditions, or reducing the number of media modalities if evidence volume becomes unmanageable.