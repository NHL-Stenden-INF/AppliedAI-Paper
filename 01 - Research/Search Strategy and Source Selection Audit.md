> **Historische audit van de eerdere 15-bronnenversie.** De bijlage gecontroleerd op 27 september 2026 heeft 14 bronnen en bevat zoekqueries met aantallen. Deze oudere tekst bewijst niet hoe die zoekacties zijn uitgevoerd. De actuele status en de open bewijsbehoefte staan in [het controleverslag](../06%20-%20Review/Peer%20Feedback%20Portfolio%20Evidence/Controleverslag-2026-09-27.md). Uitspraken hieronder zoals “current”, “final” en “the paper states” gelden uitsluitend voor de destijds beschreven versie.

# Search Strategy and Source Selection Audit

## Purpose

This audit was added after peer feedback raised a valid reproducibility question: the original literature search was not logged in enough detail to reconstruct every historical search platform, exact query and result count.

The purpose of this audit is therefore **not** to rewrite the history of the literature study. It documents what can still be stated truthfully, performs a dated supplementary search-method check, and explains the criteria used to judge whether the existing sources are suitable.

**Audit date:** 27 September 2026  
**Paper:** `De betrouwbaarheid van AI-gebaseerde deepfakedetectie`  
**Final source set:** unchanged at 15 sources.

## Integrity rule

No original search platform, query, hit count, screening count or exclusion count is reconstructed when it was not recorded at the time.

The final paper therefore states explicitly that the original search route was not fully logged. The supplementary checks below are labelled as **post-hoc validation**, not as part of the original source-selection process.

## Search terms documented from the original research

The paper records the following search-term families:

- `deepfake detection`
- `generalisation`
- `cross-dataset`
- `robustness`
- `audio spoofing`
- `adversarial evasion`
- `evaluation protocol`
- `watermarking`

Publication window used in the final paper: **2019-2026**.

References from relevant review papers were also followed.

## Supplementary search-engine validation

### IEEE Xplore

**Status:** used for a supplementary content check, not for changing the source set.

IEEE Xplore is directly relevant to this topic because it indexes technical computer-science and engineering publications, including IEEE/CVF conference papers and IEEE journal/conference material. Several sources already present in the paper are IEEE/CVF or IEEE publications.

The interactive IEEE Xplore search interface could not be queried directly in the automated audit environment. Instead, IEEE Xplore publication pages were checked through domain-restricted searches.

Queries used on 27 September 2026:

1. `deepfake detection AND (generalization OR generalisation OR robustness OR cross-dataset)`
2. `deepfake detection AND (image OR video OR audio) AND (survey OR review)`

The check returned current IEEE publications in the same subject area, including work on deepfake-detection reviews, generalisation and adversarial robustness.

**Why these results were not added to the paper:** the check was performed after the 15-source evidence base and analysis had already been completed. Adding sources at that point would change the evidence base after the analysis. The user also explicitly required the current sources to remain unchanged. IEEE Xplore was therefore used as a **validation channel**, not as a new inclusion channel.

This is not a negative judgement about IEEE Xplore. It is a strong and appropriate technical literature source; it simply was not used to retroactively alter the completed source set.

### Consensus

**Status:** evaluated as a possible academic discovery tool; not used as a formal selection channel.

A direct Consensus search was **not executed** in this audit. The Consensus connector was not connected, and its interactive search URL was not accessible through the available web interface. No Consensus hit count or result list is therefore claimed.

Official Consensus documentation was reviewed instead. It states that Consensus aggregates a very large academic corpus from sources including Semantic Scholar, OpenAlex and its own scholarly-web crawl, combines semantic and keyword search, and then uses research-quality signals and AI re-ranking to prioritise results.

**Why Consensus was not chosen as the formal selection channel:**

- it is an aggregation/discovery layer rather than the original publisher or venue database;
- it adds an AI-based ranking/synthesis layer between the researcher and the source list;
- its own documentation states that its coverage is broad but not complete;
- direct publisher, conference and journal pages provide more direct provenance for final verification;
- no direct Consensus query was executed in this audit, so claiming it as an executed search route would be inaccurate.

Consensus can still be useful for discovering papers or checking whether important themes are missing. For this completed paper, it was kept as a **supplementary discovery option**, not as evidence for changing the 15 selected sources.

## Source acceptance criteria

Before a source is considered suitable for a claim, the following points are checked.

| Criterion | What is checked | Why it matters |
| --- | --- | --- |
| Relevance | Does the source directly support SQ1, SQ2, SQ3, the method, or required legal context? | Prevents sources that only mention deepfakes from being treated as evidence |
| Publication date | Is it within the 2019-2026 study window, or otherwise clearly justified? | Deepfake generation and detection change quickly |
| Publication type | Journal article, conference paper, systematic review, benchmark/dataset paper, preprint or official government source | Different source types support different kinds of claims |
| Peer review / authority | Peer-reviewed venue where applicable; official institution for legal claims | Helps distinguish research evidence from commentary |
| Publisher / venue / institution | IEEE/CVF, ACM, Springer Nature, Elsevier, NeurIPS, European Commission, etc. | Provides provenance and accountability |
| Method transparency | Are method, experiment, sample/dataset and evaluation setup clear enough to interpret the result? | A percentage without method context is weak evidence |
| Dataset and conditions | Training/test dataset, seen/unseen setting, compression/attack context where relevant | Core requirement for interpreting detector performance |
| Metric clarity | AUC/AUROC, EER, accuracy or another metric is clearly identified | Prevents invalid comparisons |
| Traceability | DOI, official publisher page or stable official URL is available | Allows the claim to be checked again |
| Directness | Is the source primary evidence, a review, contextual background or method/legal evidence? | Source quality and claim relevance are separate decisions |
| Limitations | Does the paper disclose limits, and are those limits respected in the research paper? | Reduces overgeneralisation |
| Role restriction | Non-peer-reviewed or official-policy sources are used only for the role they can support | Prevents a preprint or policy page from becoming technical proof |

## Selection policy applied to the final 15 sources

- Peer-reviewed empirical papers and benchmarks are preferred for technical performance claims.
- Review papers are used to map technique families and compare broader patterns.
- The European Commission source is used only for legal/regulatory context.
- The DFDC arXiv preprint is used only for dataset/challenge information and is labelled as a preprint.
- Results measured with different metrics or under different test conditions are not pooled as if they were directly comparable.
- No supplementary IEEE/Consensus result from this audit was inserted into the reference list.

## What remains unrecoverable

The following cannot be supplied truthfully for the original search:

- the complete list of original search engines/platforms;
- every exact original query string;
- exact original search dates per query;
- the number of hits returned by each historical query;
- exact duplicate-removal counts;
- exact title/abstract exclusion counts;
- exact full-text exclusion counts.

These are limitations of the original research log. The paper now states this directly instead of reconstructing numbers after the fact.

## Conclusion

The current 15-source set was left unchanged. The added audit strengthens transparency by separating:

1. what was actually recorded during the original literature study;
2. what was checked on 27 September 2026;
3. what cannot be reconstructed;
4. why IEEE Xplore and Consensus did not become new formal source-selection routes after the analysis had already been completed.

