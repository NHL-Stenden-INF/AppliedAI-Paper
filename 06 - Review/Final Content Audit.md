# Final Content Audit — 21 September 2026

## Scope

This is the final pre-peer-review audit of the Dutch paper `Deepfake_paper_Nederlands_SUPERCHECK.docx`. The audit was performed against the official Applied AI assessment form and the module-book research-paper assignment.

Checks performed:

- mandatory form aspects and 8–10 page body rule;
- all A and B1–B5 assessment criteria;
- factual accuracy of the main quantitative claims against primary/authoritative sources;
- citation/reference reconciliation and APA metadata;
- consistency between Introduction, Method, Results, Conclusions and recommendations;
- passive detection versus watermarking boundaries;
- language/natural Dutch and metric terminology;
- rendered Word layout on all pages;
- watermark, comments, tracked changes, hidden text, custom XML and accessibility checks.

## Assessment-form status

The current version contains all mandatory parts: abstract, introduction, method, results, conclusions/discussion and reference list. The rendered document has 21 physical pages. Results starts on page 8 and Conclusions/Discussion starts on page 17, so the counted body is exactly **9 pages (pages 8–16)** and satisfies the official 8–10 page body rule.

The current version covers every substantive criterion:

- **A:** appropriate title, audience-appropriate academic language, reference list, design, spelling/grammar, paragraph structure and component consistency;
- **B1:** concise summary containing problem/method, results and conclusion;
- **B2:** reason, subject explanation, importance, MRQ/SQs/objective, scope, reading guide and logical connection;
- **B3:** population/sample, data collection, instruments, analysis and methodological justification;
- **B4:** contextualised/argued claims, visible author synthesis, informative depth and relevant/current source base;
- **B5:** answers to MRQ/SQs, internally consistent conclusions, identifiable recommendations and explicit reliability/validity/usability discussion.

The known B3 limitation remains explicit: exact historical database query strings and result counts were not retained. The study therefore remains correctly described as a **structured literature study**, not as a systematic literature review.

## Final factual verification

### Deepfake-Eval-2024
Confirmed against the CVPRW 2026 publication:

- 45 hours video, 56.5 hours audio, 1,975 images;
- material from 88 websites and 52 languages;
- average AUC decrease relative to previous academic benchmarks: 50% video, 48% audio, 45% image;
- best commercial AUCs: 0.79 video, 0.93 audio, 0.90 image;
- no evaluated commercial model reaches 90% classification accuracy;
- the authors use approximately 90% as a lower-bound estimate for human deepfake analyst accuracy based on inter-labeler agreement.

### Yermakov et al. (WACV 2026)
Confirmed:

- evaluation across 14 cross-dataset benchmarks;
- best GenD variant mean AUROC: **91.6% / 0.916**;
- paired training mean: **90.0% AUROC** versus **85.3%** unpaired, i.e. **+4.7 percentage points**;
- paired training reduces shortcut learning/overfitting;
- the paper supports the claim that dataset composition can matter more than simple recency.

The Dutch paper was tightened further so it no longer implies that the same GenD models were directly tested on Deepfake-Eval-2024. Figure 2 is now explicitly labelled as an **illustrative cross-study synthesis, not a direct same-detector comparison**.

### DFDC
Confirmed against Dolhansky et al. (2020):

- more than 100,000 clips;
- 3,426 paid actors;
- the 0.734 ROC-AUC statement is correctly described as a post-competition analysis on a real-video subset of the private test set, not as the official competition score.

### Nguyen-Le et al. (2026)
Confirmed:

- 13 within-domain detector verifications;
- 33 generalisation methods;
- 6 robustness methods;
- abstract-level summary of 10–15% OOD degradation;
- white-box adversarial attack success above 80% against undefended models in the tested setting.

Claims in the conclusion are explicitly bounded to that tested setting.

### ASVspoof 5
Confirmed against the final Computer Speech & Language record:

- final journal publication: **January 2026**, volume 95, article 101825;
- crowdsourced speech under diverse acoustic conditions;
- attacks produced with 32 algorithms, including contemporary TTS/voice-conversion and adversarial attacks;
- the in-text year and reference entry are consistently **2026**.

### Watermarking
Confirmed against Zhao et al. (NeurIPS 2024):

- four pixel-level invisible watermark schemes evaluated;
- regeneration attacks add noise and reconstruct the image;
- RivaGAN: 98% watermark removal while maintaining PSNR above 30;
- theoretical vulnerability for pixel-level invisible watermarks is not generalised beyond the study’s assumptions.

Watermarking remains a complementary provenance mechanism, not a replacement for passive detection. Absence of a watermark is not interpreted as proof of authenticity.

### EU AI Act Article 50
Rechecked against current European Commission guidance:

- Article 50 transparency obligations apply from 2 August 2026;
- providers must support machine-readable marking/detection of AI-generated/manipulated content;
- deployers must disclose deepfakes to natural persons by first exposure at the latest and cannot rely only on the machine-readable mark;
- there is a limited transition/grace arrangement for the Article 50(2) marking/detection obligation for systems placed on the market before 2 August 2026.

The Introduction now includes this transition nuance without expanding the paper into a legal/policy study.

## Final wording/logic tightening

The supercheck made five final precision changes without changing the argument:

1. the abstract now describes the 15-source sample more accurately (technical literature plus relevant regulation);
2. AUC is no longer presented as though it were the only performance metric; EER is explicitly acknowledged for audio;
3. Yermakov is described as using pre-trained vision encoders (CLIP, Perception Encoder and DINO), not generically as “language models”;
4. Figure 2 and the SQ2 conclusion no longer imply a same-model comparison between generalisation benchmarks and online-circulating content;
5. the usability paragraph now uses more natural Dutch (“praktijkcijfers zijn gebaseerd op content…”).

## Reference and document integrity checks

- 15 reference entries; all cited source families used in the paper have a matching reference entry.
- Reference order is alphabetical.
- Key DOI/year/page metadata rechecked.
- Hanging indents and italics are present in the reference list.
- No comments.
- No tracked insertions/deletions.
- No hidden `w:vanish` text.
- No custom XML or custom document properties.
- No zero-width hidden Unicode characters.
- No OpenAI/ChatGPT/SynthID/C2PA strings embedded in the OOXML.
- Watermark audit: **0 watermark-like objects**.
- Accessibility audit after the supercheck: **0 high, 0 medium, 0 low findings**; both figures now contain alt text.

## Rendered-layout QA

The final supercheck DOCX was rendered again after the last precision changes.

- total physical pages: **21**;
- Introduction: pages 4–5;
- Method: pages 6–7;
- Results/body: pages **8–16 (9 pages)**;
- Conclusions/Discussion: pages 17–19;
- References: pages 20–21;
- TOC page numbers remain correct;
- all tables and figures remain readable;
- no clipping, overlap, broken rows, missing glyphs or page-flow defects were found.

## Remaining external/process items

No known material factual contradiction remains after this audit.

Two items remain outside the document audit:

1. the title page still contains student-number placeholders and must be completed by the students;
2. the mandatory week-3 peer review still has to be completed, considered and evidenced in the portfolio.

After peer-review edits, run one final targeted citation/language/page-count/layout check before submission.
