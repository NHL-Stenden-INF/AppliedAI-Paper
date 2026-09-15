# Final Content Audit — 15 September 2026

## Scope of this audit

This pass rechecked the watermarking-integrated paper for:

- factual accuracy of quantitative and technical claims;
- correct interpretation of source metrics/tasks;
- consistency between Scope, Sources Index, Evidence Matrix, Findings, Results and Conclusions;
- passive detection versus active watermarking boundaries;
- reference metadata and ordering;
- the assessment-form body-page requirement;
- rendered DOCX/PDF layout and page flow.

The authoritative paper source after this audit is `04 - Paper/Final Draft/`.

## Material correction found

### UCF cross-dataset AUC

The previous draft stated that the conventional Xception baseline had an average cross-dataset AUC of `0.702`. Rechecking UCF Table 7 showed that this was incorrect.

Correct values:

- Xception baseline average cross-dataset AUC: **0.683**;
- UCF using the same Xception backbone: **0.852**.

The correction is now reflected in the Final Draft, Evidence Matrix and Findings. The old monolithic draft has been replaced with a pointer so the incorrect value cannot be reused accidentally.

## Quantitative/technical claims rechecked

| Claim in final paper | Audit result | Source |
| --- | --- | --- |
| FaceForensics++ contains >1.8 million manipulated images | Confirmed | SRC-A003 |
| FaceForensics++ supplementary manipulation classification: 99.03% raw, 95.42% HQ, 80.49% LQ | Confirmed; correctly labelled as manipulation-method classification, not binary fake/real accuracy | SRC-A003 |
| AASIST reports 0.83% EER on ASVspoof 2019 LA | Confirmed | SRC-A009 |
| WildDeepfake contains 7,314 face sequences from 707 internet-collected deepfake videos | Confirmed | SRC-A004 |
| SBI improves its baseline by 4.90 pp on DFDC and 11.78 pp on DFDCP in the reported cross-dataset evaluation | Confirmed | SRC-A005 |
| UCF Table 7: Xception avg. AUC 0.683; UCF (Xception) 0.852 | Confirmed after correction | SRC-A006 |
| Hou et al. evaluate four spatial and two frequency detectors over four datasets in white-/black-box settings | Confirmed | SRC-A007 |
| ASVspoof 5 uses crowdsourced/diverse speech, adversarial attacks and codec conditions; attacks significantly compromise baselines | Confirmed | SRC-A008 |
| Nguyen-Le et al. report approximately 10–15% OOD degradation in the summarised scenarios and >80% white-box attack success against undefended models in the tested setting | Confirmed and kept context-bounded | SRC-A001 |
| DeepfakeBench contains 15 detection methods and 9 datasets and addresses non-standardised evaluation | Confirmed | SRC-A002 |
| Ramanaharan et al. report 46.3% of selected studies supporting generalisation across different deepfake types | Confirmed and interpreted cautiously | SRC-A010 |
| Stable Signature: >90% origin detection after crop retaining 10% content at FPR <10^-6 | Confirmed; correctly treated as provenance verification, not open-world fake classification | SRC-A011 |
| Zhao et al. demonstrate regeneration-based removal vulnerability for four pixel-level invisible watermarking schemes | Confirmed | SRC-A012 |

## Interpretation corrections/controls

- Removed the overbroad implication that controlled benchmark performance proves synthetic media in general are detectable.
- Replaced `highly reliable` wording in the main conclusion with `very strong measured performance` for familiar/validated conditions, avoiding circular use of the term reliability.
- Preserved the distinction between passive detection and active watermark provenance.
- SQ3 now identifies **five passive-detection factor classes** plus a **separate watermark provenance/removal boundary** rather than treating watermark absence as an ordinary passive-detector failure mode.
- Absence of a watermark is explicitly not evidence of authenticity.
- Image-specific watermark evidence is not generalised to audio/video watermark systems.
- Incompatible metrics (accuracy, AUC, EER, watermark-origin detection) are not pooled.

## Reference/APA reconciliation

- Twelve cited scholarly sources are present in the reference list.
- In-text citations map to reference entries.
- Rössler/Rieß/Nießner and Jégou diacritics are preserved.
- DOI/page metadata was rechecked for the two watermark papers and key benchmark sources.
- Reference order corrected so `Zhao` precedes `Zi` alphabetically.
- The school does not explicitly name an APA edition; APA 7 remains the project working standard.

## Page-volume and visual QA

Final checked DOCX/PDF render:

- **15 total pages**;
- Results/body starts on **page 4**;
- Conclusions/Discussion starts on **page 13**;
- therefore the counted body remains safely within the required **8–10 pages**, without using Introduction, Method, Conclusions/Discussion or References to satisfy the volume rule.

All 15 pages were inspected after the final factual correction. No clipping, overlap, broken table rows, missing text or unreadable page-flow defects were found. Page 3 intentionally contains white space because Results begins on a new physical page, making the body-volume boundary explicit.

## Remaining limitation / open process item

No material factual contradiction is known in the final checked version after this audit. The main methodological weakness remains **B3 reproducibility depth**: the study records search systems, concepts, date window, inclusion/exclusion logic and extraction fields, but exact historical query strings/result counts were not retained. It must therefore continue to be described as a **structured literature study**, not a full systematic literature review.

The only mandatory process item still open is the scheduled week-3 peer review. After peer-review edits, citation/reference, language, page-volume and rendered-layout QA must be run once more.