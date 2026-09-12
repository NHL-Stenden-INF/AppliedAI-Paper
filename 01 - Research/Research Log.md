# Research Log

## 2026-09-10 — Foundation and Research Setup

### Phase

Foundation and Research Setup

### Documents Reviewed

- `APPENDIX 9 ASSESSMENT RESEARCH PAPER.pdf` — all 6 pages.
- `APPLIED AI MODULE BOOK V1.pdf` — all 63 pages with paper-relevant sections mapped.
- `Research paper Subject.xlsx` — current proposal record.
- Initial GitHub repository — only a minimal README existed before setup.

### Main Findings

- Pair paper during weeks 1–4; mandatory for period-1 Go/no-go.
- Current questions exist but lecturer approval is not evidenced.
- Mandatory form-aspects gate precedes substantive assessment.
- Direct rubric covers A and B1–B5, including method and methodological reliability/validity/usability.
- 8–10-page requirement exists with an unusual counting footnote.

### Decisions

- Assessment form and module book treated as authoritative within their specific scopes.
- Subject spreadsheet treated as project proposal evidence only.
- Initial proposed method: literature-based comparative investigation.
- No substantive research findings or paper prose generated.

### Unknowns

Lecturer approval, APA edition, Teams submission details, page-count interpretation and `sub-digit` aggregation.

### Next Actions

Confirm question/title approval, operationalise terms, finalise the research protocol and begin Phase 2 only after readiness review.

---

## 2026-09-10 — Complete Foundation Audit and Improvement

### Phase

Foundation Audit and Improvement

### Documents Rechecked

- `APPENDIX 9 ASSESSMENT RESEARCH PAPER.pdf` — form gate, page-count footnote, colour/grade explanation and every A/B1–B5 row revalidated.
- `APPLIED AI MODULE BOOK V1.pdf` — learning outcomes/alignment, Appendix 1 period-1 portfolio evidence, Appendix 3 research-paper assignment and Appendix 8 grade calculation revalidated.
- `Research paper Subject.xlsx` — `Blad1` A1:H3 rechecked; proposal wording unchanged.
- Entire current GitHub foundation structure and all active Markdown files audited.

### Problems Found

- B1–B5 rubric rows had been collapsed into broad checklist requirements, weakening one-by-one traceability.
- Module-book printed page numbers and PDF page numbers were not distinguished, making source locators less precise.
- The methodology label `structured literature review` could imply a full systematic-review standard not actually planned.
- The page-budget file overinterpreted the unusual 8–10-page footnote as mainly a `results/body` allocation.
- Findings structure lacked explicit limitations fields.
- Unsupported intended claims in the Argument Map were marked `Planned` instead of `Evidence Needed`.
- Rubric preparation statuses were too optimistic for criteria whose evidence does not yet exist.
- Planned future peer-review obligations were mixed into the same table as actual feedback.

### Corrections Made

- Decomposed all B1–B5 assessment rows into stable child requirements while preserving REQ-001–043.
- Added explicit A-design/consistency and peer-review feedback-content requirements.
- Added dual printed/PDF page locators for module-book traceability.
- Reframed the method as a structured literature study / desk research with document analysis, without claiming a full SLR.
- Expanded end-to-end assessment traceability and evidence directness rules.
- Strengthened operational-definition, comparability, source-quality and feasibility controls.
- Corrected page-budget interpretation to preserve the source wording without unsupported allocation assumptions.
- Added explicit limitations/gaps structures and stricter rubric-readiness statuses.
- Separated actual feedback from future feedback obligations.

### Decisions

- Current MRQ/SQs remain unchanged and Proposed; no unauthorized academic change was made.
- No interviews/surveys/experiment were added because the current questions do not require them and school sources do not mandate them.
- APA 7 remains a project working fallback, not a school-confirmed edition.
- Research readiness is `Ready with Conditions`, not unconditional Ready.

### New Unknowns

No material new source-derived unknowns were introduced. One methodological confirmation was elevated explicitly: whether the assessor accepts publication population/sample as the B3 interpretation for literature-based research.

### Resolved Unknowns

- Confirmed there are exactly three Project source files currently available.
- Confirmed the module book does not provide a paper-specific named methodology or APA edition in the available material.
- Confirmed no separate feedback/template/APA document is present in the Project.

### Research Readiness

**Ready with Conditions.**

### Next Actions

1. Verify lecturer approval of the title/MRQ/SQs.
2. Finalise operational definitions and the literature-study protocol.
3. Begin Phase 2 evidence collection without drafting final-paper prose.
4. Verify Teams/page-count/APA details before final drafting and submission.

---

## 2026-09-12 — Phase 2 Research Execution and Paper Draft

### Phase

Phase 2 — Research Execution, Evidence Synthesis and Drafting

### Academic Sources Added

Ten academic sources were selected for direct relevance to the three research questions and the main reliability judgement:

- Nguyen-Le et al. (2026) — cross-modality survey with empirical generalisation/robustness evaluation.
- Yan, Zhang, Yuan, et al. (2023) — DeepfakeBench benchmark.
- Rossler et al. (2019) — FaceForensics++ foundational benchmark and compression evidence.
- Zi et al. (2020) — WildDeepfake real-world internet dataset.
- Shiohara and Yamasaki (2022) — Self-Blended Images generalisation method.
- Yan, Zhang, Fan, et al. (2023) — UCF generalisable common-feature method.
- Hou et al. (2023) — adversarial statistical-consistency evasion attacks.
- Wang et al. (2024) — ASVspoof 5 crowdsourced/deepfake/adversarial audio benchmark.
- Jung et al. (2022) — AASIST audio anti-spoofing architecture.
- Ramanaharan et al. (2025) — systematic review of deepfake-video generalisation.

### Operational Definitions Used

- **Reliability:** combined discriminatory performance, generalisation outside the training distribution and robustness to transformations/attacks.
- **Real-world conditions:** conditions meaningfully different from a controlled training benchmark, including internet-sourced/cross-dataset data, unseen generators/manipulations, compression/codecs, diverse acquisition conditions and deliberate evasion.
- **Current:** primarily 2020-2026 evidence, with 2019 FaceForensics++ retained as a justified foundational source.
- **Modality scope:** image, video and audio retained at high-level comparative depth.

### Analysis Performed

- SQ1: bounded taxonomy of visual/video/audio detection techniques.
- SQ2: contextual comparison of in-domain versus cross-domain performance without pooling incompatible metrics.
- SQ3: synthesis of compression/codecs, unseen generators, adversarial evasion, dataset/acquisition shift and evaluation-pipeline effects.
- MRQ: integrated reliability judgement weighted toward evidence that tests generalisation and robustness rather than benchmark accuracy alone.

### Main Findings

- Strong controlled benchmark performance is common and does not by itself establish deployment reliability.
- Out-of-distribution and internet-sourced evaluation reveals a persistent generalisation gap.
- Generalisation-oriented methods such as SBI and UCF improve cross-dataset performance but do not eliminate dependence on training/evaluation conditions.
- Compression/codecs can suppress subtle forensic traces.
- Deliberate adversarial attacks can substantially reduce effectiveness; recent cross-modality evaluation reports white-box attack success above 80% against undefended models in its tested robustness setting.
- Audio evidence shows the same pattern: strong benchmark anti-spoofing results are challenged by newer attacks, diverse speakers/acoustics, codecs and adversarial conditions.

### Conclusion Entered

Current AI-based deepfake detection is **conditionally reliable**: effective in known or well-represented conditions, but materially less dependable under distribution shift, post-processing and adaptive attack. No universal accuracy percentage is supported across image, video and audio.

### Paper Draft Produced

- Complete English paper created under `04 - Paper/Research Paper Draft.md`.
- Required sections present: abstract, introduction, method, results, conclusions/discussion and references.
- Results include an evidence-bearing synthesis figure in the rendered version and a representative evidence table.
- APA-style citations/reference list applied using APA 7 as the project working default.
- DOCX and PDF render created separately for final document delivery.
- Final rendered document visually checked page by page; current version is 8 pages total.

### QA / Rubric Actions

- Sources Index populated with stable academic source IDs.
- Evidence Matrix populated and acceptance rules applied.
- Findings by Research Question and Conclusions Matrix completed.
- Rubric Check updated against every form/A/B1-B5 area.
- Metrics were not pooled where datasets, modalities or protocols were incompatible.

### Unresolved External Dependencies

- Lecturer approval evidence for the current title/MRQ/SQs is still not present in the repository.
- Teams-only submission/template/file-type requirements remain unverified.
- Official APA edition remains unnamed by the school sources.
- The exact intended interpretation of the assessment form's unusual 8-10-page counting footnote remains unverified.
- Required week-3 peer review has not yet been completed/recorded.

### Current Status

**Complete draft ready for lecturer and peer review, not yet final-submission cleared.**