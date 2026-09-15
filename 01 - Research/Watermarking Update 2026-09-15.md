# Research Log - Watermarking Update

**Date:** 2026-09-15  
**Phase:** Final evidence expansion / pre-peer-review QA

## Trigger

Lecturer feedback on the approved subject: `OK, also look into watermarking please`.

## Decision

The approved title, MRQ and three SQs remain unchanged. Watermarking is incorporated as a bounded complementary active provenance mechanism because it directly relates to the identification of AI-generated media, but it is technically different from passive deepfake detection.

## Evidence Added

- `SRC-A011` - Fernandez et al. (2023), *The Stable Signature: Rooting Watermarks in Latent Diffusion Models*, ICCV.
- `SRC-A012` - Zhao et al. (2024), *Invisible Image Watermarks Are Provably Removable Using Generative AI*, NeurIPS.

The source pair was deliberately chosen to avoid a one-sided treatment:

- SRC-A011 supports capability and robustness of active watermark provenance under ordinary image modifications.
- SRC-A012 supports the limitation that invisible pixel-level watermarks can be targeted by regeneration/removal attacks.

## Method Update

- Candidate population extended to include scholarly watermarking literature for generative images.
- Final focused sample expanded from 10 to 12 publications.
- Search concepts extended with `invisible watermarking`, `provenance`, and `watermark removal`.
- Watermark metrics are not pooled with passive detection metrics because the task and assumptions differ.

## Evidence / Analysis Update

- Added EVD-020: active watermark capability/provenance.
- Added EVD-021: watermark-removal vulnerability.
- Added EVD-022: passive detection + active watermarking complementarity.
- Findings updated for SQ1 context, SQ3 failure modes and MRQ synthesis.
- Conclusions Matrix updated while preserving the main `conditionally reliable` conclusion.

## Paper Update

- Abstract: watermark capability/removal boundary mentioned.
- Introduction: scope changed from excluding watermarking to bounded inclusion following lecturer feedback.
- Method: sample/search protocol updated.
- Results: new 3.1.6 active-watermarking subsection and new 3.3.4 watermark-removal/provenance-limits subsection.
- Tables 1 and 3 updated.
- Integrated reliability synthesis updated.
- Conclusion: fifth recommendation added for watermark use as supplementary provenance evidence.
- Two APA references added.

## Page-Count Control

The first edit pushed Conclusions to page 14, creating a body-length risk. Redundant synthesis text was compressed while preserving the new watermark evidence.

Final rendered result:

- 15 pages total;
- Results begins page 4;
- Conclusions begins page 13;
- counted Results body = pages 4-12 plus the opening part of page 13, safely between 9 and 10 pages.

## QA

- Final DOCX rendered to 15 page images.
- All pages visually inspected.
- No clipping, overlap, broken tables, missing text or obvious page-flow defects observed.
- Watermark references and core quantitative claim from Stable Signature verified against ICCV source.
- Watermark removal claim verified against NeurIPS 2024 source.

## Remaining

Mandatory peer review next week, followed by one final APA/citation/grammar/layout pass.