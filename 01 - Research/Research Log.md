# Research Log

## 2026-09-10 - Foundation and Research Setup

### Phase

Foundation and Research Setup

### Documents Reviewed

- `APPENDIX 9 ASSESSMENT RESEARCH PAPER.pdf` - all six pages.
- `APPLIED AI MODULE BOOK V1.pdf` - all 63 pages with paper-relevant sections mapped.
- `Research paper Subject.xlsx` - current proposal record.
- Initial GitHub repository structure.

### Main Findings and Decisions

- The paper is written in pairs during weeks 1-4 and is mandatory for the period-1 Go/no-go.
- The assessment form contains a mandatory form-aspects gate before substantive assessment.
- The direct rubric covers A and B1-B5, including reliability, validity and usability in the discussion.
- The research questions were retained exactly as registered rather than silently changed.
- The methodology was framed as a **structured literature study / desk research with document analysis**, not as a full systematic literature review.
- Assessment form and module book were treated as authoritative for school requirements; the subject spreadsheet was treated as project/proposal evidence.

### Initial Unknowns

Lecturer approval status, exact Teams submission details, official APA edition, page-count interpretation, and exact rubric aggregation.

---

## 2026-09-10 - Foundation Audit and Improvement

### Problems Found

- Rubric rows were not yet traced individually enough.
- Printed and PDF page locators needed clearer distinction.
- `structured literature review` risked overstating methodological completeness.
- The page-budget interpretation was uncertain.
- Findings and argument-map files needed stricter evidence-status labels.

### Corrections

- Decomposed B1-B5 into traceable requirements.
- Strengthened the Evidence Matrix, Analysis Framework, method operationalisation and research-gap controls.
- Preserved explicit unknowns rather than filling them with assumptions.
- Established evidence-first drafting: Sources Index -> Evidence Matrix -> Findings -> Conclusions Matrix -> Paper Draft -> Rubric Check.

---

## 2026-09-12 - Phase 2 Research Execution

### Lecturer Approval

The authors confirmed that the title, main research question and three subquestions were approved by the lecturer.

### Academic Source Set

Ten academic publications were selected for direct relevance:

- Nguyen-Le et al. (2026) - cross-modality survey plus empirical generalisation/robustness evaluation.
- Yan, Zhang, Yuan, et al. (2023) - DeepfakeBench.
- Rössler et al. (2019) - FaceForensics++.
- Zi et al. (2020) - WildDeepfake.
- Shiohara and Yamasaki (2022) - Self-Blended Images.
- Yan, Zhang, Fan, et al. (2023) - UCF.
- Hou et al. (2023) - adversarial statistical-consistency evasion.
- Wang et al. (2024) - ASVspoof 5.
- Jung et al. (2022) - AASIST.
- Ramanaharan et al. (2025) - systematic review of video-detector generalisation.

### Operational Definitions

- **Reliability:** discriminatory performance + generalisation outside training distribution + robustness to transformations/attacks.
- **Real-world conditions:** internet-sourced/cross-dataset data, unseen generators/manipulations, compression/codecs, diverse acquisition conditions and deliberate evasion.
- **Current:** primarily 2020-2026, with 2019 FaceForensics++ retained as foundational evidence.
- **Scope:** passive AI/ML deepfake detection for image, video and audio.

### Initial Analysis

- SQ1: bounded taxonomy of detector techniques.
- SQ2: contextual comparison of in-domain and cross-domain performance without unsupported metric pooling.
- SQ3: synthesis of compression/codecs, unseen generators, adversarial evasion, dataset/acquisition shift and evaluation-pipeline effects.
- MRQ: integrated judgement weighted toward generalisation and robustness evidence.

### Initial Conclusion

Current AI-based deepfake detection is **conditionally reliable**: strong under familiar/validated conditions but materially less dependable under distribution shift, media processing and adaptive attack.

---

## 2026-09-12 - Final QA Before Body Expansion

### Corrections

- Rechecked source metadata and selected numerical claims against publisher/conference sources where available.
- Corrected author diacritics (`Rössler`, `Rieß`, `Nießner`).
- Replaced an overly broad OOD range with the more conservative `10-15%` wording used in the relevant 2026 source discussion.
- Strengthened scope and method wording.
- Improved APA-style reference presentation.
- Confirmed that the mandatory peer-review step is still scheduled for the following week and is therefore not yet available.

### Problem Discovered After QA

The rendered draft contained eight pages **in total**. The assessment footnote states that the required 8-10 pages apply to the **body**, excluding Introduction, Method, Conclusions, Discussion and the source list. Therefore the eight-page-total draft did not safely satisfy the volume requirement.

---

## 2026-09-12 - Body-Page Correction and Evidence Expansion

### Requirement Interpretation Applied

The assessment form is now followed literally:

> the 8-10-page requirement applies to the body, excluding Introduction, Method, Conclusions, Discussion and References.

For this paper structure, the counted body is Section `3. Results`, including its evidence-bearing figure and tables.

### Workflow Followed

The paper was **not** expanded first and justified afterwards. The repository's evidence-first sequence was followed:

1. rechecked the official page rule;
2. expanded the Evidence Matrix with additional bounded evidence and metric cautions;
3. expanded `Findings by Research Question.md`;
4. preserved the existing Conclusions Matrix conclusion;
5. expanded the Results/body around SQ1, SQ2, SQ3 and an integrated MRQ synthesis;
6. updated the Word/Page Budget;
7. updated the Rubric Check;
8. rendered the DOCX and visually inspected every page.

### Body Expansion Performed

The Results section was expanded from approximately **1,806 words** to approximately **5,541 words**. The expansion adds analysis rather than filler:

- spatial and forensic visual cues;
- frequency-domain and generator-related cues;
- generalisation-oriented techniques (SBI and UCF);
- temporal video evidence;
- audio anti-spoofing techniques;
- detector-family reliability dependencies;
- controlled versus cross-domain performance;
- internet-sourced WildDeepfake evidence;
- compression as a condition-dependent reliability factor;
- broader ASVspoof 5 challenge conditions;
- why accuracy/AUC/EER cannot be pooled into one reliability percentage;
- compression/codecs, unseen generators, adversarial evasion, dataset/environment shift and evaluation-pipeline variation;
- interaction between failure factors;
- integrated reliability profile and evidence-strength gradient.

### New Evidence-Bearing Visuals

- Figure 1 - reliability chain.
- Table 1 - detector technique families and reliability implications.
- Table 2 - representative performance/generalisation evidence with metric context.
- Table 3 - reliability-reducing factors across image, video and audio.

### Metric Safeguards

- UCF's reported Xception baseline average AUC of 0.702 is used only in its stated cross-dataset context.
- FaceForensics++ values 99.03%, 95.42% and 80.49% are explicitly described as **manipulation-method classification** under raw/HQ/LQ compression, not re-labelled as binary deepfake-detection accuracy.
- Visual accuracy/AUC and audio EER remain unpooled.

### Rendered Page Result

- Complete rendered paper: **14 pages**.
- Results starts on physical page **4**.
- Conclusions and Discussion starts on physical page **13**.
- Therefore the counted Results/body occupies physical pages **4-13**, exactly **10 pages**.
- The excluded sections remain outside the page-count justification.

### Visual QA

All 14 rendered pages were inspected. No clipping, overlapping text, broken tables, missing glyphs, or unreadable page-flow problems were found. Tables are allowed to break only between rows; rows are not split across pages.

### Consistency Check

The expansion does **not** change the approved MRQ/SQs or the main conclusion. It deepens the reasoning supporting the same bounded finding: current detectors are conditionally reliable, with confidence depending on validation coverage, generalisation and robustness.

### Current Status

**Ready for the mandatory peer review next week.**

Remaining before submission:

1. receive and provide the required peer feedback;
2. process relevant peer feedback;
3. keep the Results/body at no more than 10 pages after revisions;
4. repeat APA/citation/grammar/layout QA after peer-review edits;
5. follow the final Teams submission instructions.