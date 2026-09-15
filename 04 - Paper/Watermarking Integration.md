# Watermarking Integration

## Status

**Integrated into the current DOCX/PDF paper version on 15 September 2026.**

Lecturer feedback on the approved topic was: `OK, also look into watermarking please`.

The approved MRQ and three SQs were not changed. Watermarking is treated as a complementary active provenance mechanism within the existing reliability argument rather than as a new fourth research question.

## Why It Fits the Existing Paper

The primary paper studies passive AI-based detection: systems infer synthetic/manipulated media from visual or acoustic evidence. Watermarking addresses the same authenticity problem from a different direction. A participating generator deliberately embeds a signal that can later be detected. This makes watermarking relevant to SQ1 as a complementary detection mechanism and to SQ3/MRQ because watermark reliability can fail when marks are absent, degraded or deliberately removed.

The paper explicitly avoids the incorrect inference that absence of a watermark proves authenticity.

## Added Academic Evidence

### SRC-A011 - Stable Signature

Fernandez, P., Couairon, G., Jégou, H., Douze, M., & Furon, T. (2023). *The Stable Signature: Rooting watermarks in latent diffusion models*. Proceedings of the IEEE/CVF International Conference on Computer Vision, 22466-22477. https://doi.org/10.1109/ICCV51070.2023.02053

Evidence used:

- active invisible binary signature embedded through the latent-diffusion decoder;
- dedicated extraction/statistical verification;
- reported robustness to multiple image modifications;
- example: >90% origin-detection accuracy after cropping to retain only 10% of content, at false-positive rate <10^-6.

### SRC-A012 - Watermark removal

Zhao, X., Zhang, K., Su, Z., Vasan, S., Grishchenko, I., Kruegel, C., Vigna, G., Wang, Y.-X., & Li, L. (2024). *Invisible image watermarks are provably removable using generative AI*. Advances in Neural Information Processing Systems, 37, 8643-8672. https://doi.org/10.52202/079017-0276

Evidence used:

- regeneration attacks add noise and reconstruct images using denoising/generative models;
- pixel-level invisible watermark detection can be reduced while image quality remains high;
- watermark robustness to ordinary transformations is therefore distinct from robustness to deliberate removal.

## Paper Integration Points

### Abstract

Adds the bounded conclusion that invisible watermarking can provide explicit provenance when a participating generator embeds a mark, but removal research shows that this evidence is not inherently tamper-proof.

### Introduction / Scope

Passive image/video/audio detection remains the primary scope. Invisible watermarking for AI-generated images is included because the lecturer explicitly requested it. Legal analysis and development of a new detector/watermarking method remain outside scope.

### Method

The literature sample changes from 10 to 12 publications. Search concepts now also include `invisible watermarking`, `provenance`, and `watermark removal`. The two watermark studies were selected deliberately to represent both capability and limitation.

### Results 3.1

New subsection: `3.1.6 Active watermarking as a complementary detection mechanism`.

The subsection distinguishes active watermark provenance from passive forensic inference and explains why a positive verified mark can strengthen attribution without making watermark absence evidence of authenticity.

The existing technique-taxonomy subsection becomes `3.1.7` and Table 1 receives a row for active invisible watermarking.

### Results 3.3

New subsection: `3.3.4 Watermark removal and provenance limits`.

It separates:

1. survival under benign transformations; and
2. resistance to adaptive removal.

Existing subsections are renumbered, and Table 3 adds watermark absence/removal as a reliability factor for generated images.

### Results 3.4

The integrated reliability profile now treats watermarking as an additional provenance channel. Passive detection and watermarking are described as complementary layers rather than competing replacements.

### Conclusions and Discussion

The main conclusion remains `conditionally reliable`. A fifth recommendation is added: where a generation system supports robust watermarking, successful verification can be used as additional provenance evidence, but absence of a mark must not be treated as proof of authenticity.

## Consistency Controls

- Approved MRQ/SQs unchanged.
- Main passive-detection conclusion unchanged.
- Watermark metrics are not pooled with passive deepfake-classification metrics.
- Image-watermark evidence is not silently generalised to all audio/video watermark systems.
- Sources Index updated with SRC-A011 and SRC-A012.
- Evidence Matrix updated with EVD-020 to EVD-022.
- Findings and Conclusions Matrix updated before final QA.
- Rubric Check rerun after integration.

## Page-Count Control

The first watermarking edit pushed `Conclusions and Discussion` to physical page 14, which would have made the counted Results body exceed the safe 8-10-page interpretation.

The integration was therefore tightened by removing redundant synthesis while keeping all new watermark evidence.

Final rendered state:

- complete document: **15 pages**;
- Results begins: **page 4**;
- Conclusions begins: **page 13**;
- pages 4-12 are full Results pages and page 13 contains the final Results material before Conclusions;
- counted body: safely **between 9 and 10 pages**.

All 15 pages were visually inspected after the final DOCX render.