# Applied AI Research Paper

## Research Project

**Title:** The reliability of AI-based deepfake detection  
**Topic:** AI-generated deepfakes and the technology used to detect them  
**Authors:** Lucas Wanink & Dave van den Berg

## Current Phase

**Final content audit completed — ready for mandatory peer review**

The research phase has been executed, the lecturer-requested watermarking analysis is integrated, the paper satisfies the 8-10-page body rule, and a complete factual/consistency/layout audit was completed on 15 September 2026.

## Approval / Feedback Status

**Lecturer approval: Confirmed by the authors.**

Approved main research question:

> To what extent can AI-based deepfake detection systems reliably distinguish AI-generated or manipulated media from authentic content?

The three approved subquestions remain unchanged.

Additional lecturer feedback:

> OK, also look into watermarking please

This is implemented as a bounded complementary analysis of active invisible watermarking for AI-generated images. It is not treated as a replacement for passive deepfake detection.

## Research Status

- Structured literature study completed.
- Twelve selected scholarly sources registered and quality-labelled.
- Ten sources cover passive image/video/audio detection; two peer-reviewed sources cover watermark capability and watermark removal.
- Evidence Matrix, Findings and Conclusions Matrix aligned with the final paper.
- Lecturer-requested watermarking integrated into technique, provenance/failure-boundary and deployment analysis.
- One synthesis figure and three evidence-bearing tables included.
- Quantitative claims rechecked against source material.
- References and in-text citations reconciled.
- Final DOCX/PDF rendered to 15 pages and visually inspected page by page.

## Final factual audit

The audit found one material numerical transcription error in the earlier draft: UCF's conventional Xception baseline was previously written as average AUC `0.702`. UCF Table 7 actually reports:

- **Xception average cross-dataset AUC: 0.683**;
- **UCF (Xception) average cross-dataset AUC: 0.852**.

This is corrected in the authoritative Final Draft, Evidence Matrix and Findings. The previous monolithic paper file is now a pointer so the old value cannot be reused accidentally.

Other audit changes tightened the passive-detection/watermarking distinction, removed an overbroad statement about synthetic media being inherently detectable, clarified task-specific FaceForensics++ metrics, and corrected final reference ordering.

See [Final Content Audit](06%20-%20Review/Final%20Content%20Audit.md).

## Authoritative paper source

The authoritative checked Markdown source is under [Final Draft](04%20-%20Paper/Final%20Draft/README.md), split into five ordered files for traceable review. The corresponding `FINAL_CHECKED` DOCX/PDF is the version to use for peer review.

## Watermarking interpretation

The paper distinguishes:

- **Passive detection:** infer manipulation/synthetic origin from media features.
- **Active watermarking:** a participating generator embeds a recoverable provenance signal.

A successfully verified watermark can strengthen provenance. An absent watermark does **not** prove authenticity because the generator may never have embedded one or the mark may have been degraded/removed.

## Page-requirement status

The assessment form states that the required **8-10 pages apply to the body**, excluding Introduction, Method, Conclusions, Discussion and the source list.

Final checked render:

- complete document: **15 pages**;
- Results/body starts on page **4**;
- Conclusions and Discussion starts on page **13**;
- the counted Results/body therefore remains safely within **8-10 pages**.

## Repository Navigation

- [Assignment Overview](00%20-%20Assignment/Assignment%20Overview.md)
- [Requirements Checklist](00%20-%20Assignment/Requirements%20Checklist.md)
- [Assessment Criteria](00%20-%20Assignment/Assessment%20Criteria.md)
- [Research Questions](00%20-%20Assignment/Research%20Questions.md)
- [Scope](00%20-%20Assignment/Scope.md)
- [Research Plan](01%20-%20Research/Research%20Plan.md)
- [Methodology Plan](01%20-%20Research/Methodology%20Plan.md)
- [Evidence Matrix](01%20-%20Research/Evidence%20Matrix.md)
- [Sources Index](02%20-%20Sources/Sources%20Index.md)
- [Analysis Framework](03%20-%20Analysis/Analysis%20Framework.md)
- [Findings](03%20-%20Analysis/Findings%20by%20Research%20Question.md)
- [Conclusions Matrix](03%20-%20Analysis/Conclusions%20Matrix.md)
- [Final Draft](04%20-%20Paper/Final%20Draft/README.md)
- [Watermarking Integration](04%20-%20Paper/Watermarking%20Integration.md)
- [Word / Page Budget](04%20-%20Paper/Word%20Budget.md)
- [Rubric Check](06%20-%20Review/Rubric%20Check.md)
- [Final Content Audit](06%20-%20Review/Final%20Content%20Audit.md)

## Remaining Before Submission

1. Complete the mandatory week-3 peer review next week and retain evidence of feedback received and feedback given.
2. Process relevant peer-review feedback into the final paper.
3. Keep the counted body within the 8-10-page range after peer-review changes.
4. Re-run citation/reference, spelling/grammar, consistency and rendered-layout QA after those changes.
5. Follow the final Teams submission instructions.

## Current Readiness

**Ready for peer review.** No material factual contradiction is known in the final checked version after the audit. The main remaining academic weakness is B3 reproducibility depth: exact historical query strings/result counts were not retained, so the method remains correctly described as a structured literature study rather than a systematic literature review.