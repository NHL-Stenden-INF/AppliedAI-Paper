# Final Content Audit — 21 September 2026

## Scope

This is the final pre-peer-review audit of the Dutch paper, now including the simplified Method section and corrected figure-caption formatting in `Deepfake_paper_Nederlands_METHODE_KORT_EN_DUIDELIJK_CAPTIONS.docx`. The audit was performed against the official Applied AI assessment form and the module-book research-paper assignment.

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

The current version contains all mandatory parts: abstract, introduction, method, results, conclusions/discussion and reference list. After simplifying the Method, the rendered document has **20 physical pages**. Results starts on page **7** and Conclusions/Discussion starts on page **16**, so the counted body remains exactly **9 pages (pages 7–15)** and satisfies the official 8–10 page body rule.

The current version covers every substantive criterion:

- **A:** appropriate title, audience-appropriate academic language, reference list, design, spelling/grammar, paragraph structure and component consistency;
- **B1:** concise summary containing problem/method, results and conclusion;
- **B2:** reason, subject explanation, importance, MRQ/SQs/objective, scope, reading guide and logical connection;
- **B3:** population/sample, data collection, instruments, analysis and methodological justification;
- **B4:** contextualised/argued claims, visible author synthesis, informative depth and relevant/current source base;
- **B5:** answers to MRQ/SQs, internally consistent conclusions, identifiable recommendations and explicit reliability/validity/usability discussion.

The known B3 limitation remains explicit: exact historical database query strings and result counts were not retained. The study therefore remains correctly described as a **structured literature study**, not as a systematic literature review.

## Method simplification

The Method was deliberately shortened and rewritten in more natural Dutch after review feedback that the earlier version was too technical and too long.

Changes:

- removed jargon such as `documentanalyse`, `vergelijkende extractie van resultaten` and `thematische synthese`;
- reduced the Method from roughly **818 words to 391 words**;
- reduced the Method from two physical pages to **one page (page 6)**;
- retained all B3 requirements: methodological justification, population/sample, data collection, source/result registration and analysis;
- merged the separate definitions/analysis explanation into one concise `Analyse` subsection;
- renamed `Onderzoeksinstrumenten` to the clearer `Vastlegging van bronnen en resultaten`;
- updated the reading guide and cached TOC page numbers after the page shift.

The shorter wording changes presentation only; it does not alter the research design, source sample, evidence or conclusions.

## Figure/table caption consistency

The table captions already used a compact, italic 9 pt grey style. The two figure captions had reverted to normal body-text formatting. This has been corrected:

- `Figuur 1` and `Figuur 2` captions now use the same 9 pt, italic, grey formatting as the table captions;
- caption text itself was not changed;
- the edit did not change the total page count or the 9-page body count;
- both figures and all three tables remain readable and properly referenced in the surrounding text.

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

The Dutch paper no longer implies that the same GenD models were directly tested on Deepfake-Eval-2024. Figure 2 is explicitly labelled as an **illustrative cross-study synthesis, not a direct same-detector comparison**.

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

The Introduction includes this transition nuance without expanding the paper into a legal/policy study.

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
- Both figures contain alt text.

## Rendered-layout QA

The caption-corrected DOCX was rendered again and visually reviewed page by page.

- total physical pages: **20**;
- Introduction: pages 4–5;
- Method: **page 6**;
- Results/body: pages **7–15 (9 pages)**;
- Conclusions/Discussion: pages 16–18;
- References: pages 19–20;
- TOC page numbers remain correct;
- all tables and figures remain readable;
- figure captions now visually match the table-caption style;
- no clipping, overlap, broken rows, missing glyphs or page-flow defects were found.

## Remaining external/process items

No known material factual contradiction remains after this audit.

Two items remain outside the document audit:

1. the title page still contains student-number placeholders and must be completed by the students;
2. the mandatory week-3 peer review still has to be completed, considered and evidenced in the portfolio.

After peer-review edits, run one final targeted citation/language/page-count/layout check before submission.
