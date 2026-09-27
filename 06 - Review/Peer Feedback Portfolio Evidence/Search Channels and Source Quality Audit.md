# Search Channels and Source Quality Audit

## Purpose

This note documents an additional final check of the literature-search approach after peer feedback. It is evidence for the portfolio and must not be read as a reconstruction of the original search process.

The existing 15-source paper base was deliberately kept unchanged. No source was added, removed or replaced during this check.

## What was known from the original research

The original literature study used academic search engines, publisher databases and references from review papers. Search terms included:

- `deepfake detection`
- `generalisation`
- `cross-dataset`
- `robustness`
- `audio spoofing`
- `adversarial evasion`
- `evaluation protocol`
- `watermarking`

The publication window was 2019-2026.

The exact original search platforms, complete query strings and numbers of found/excluded records were not systematically logged. These details are therefore not reconstructed after the fact.

## Additional control search

**Date:** 27 September 2026.

Two additional search channels were checked to see whether the existing topic coverage was still reflected in recent academic search results.

### IEEE Xplore

Control queries:

1. `deepfake detection generalization robustness cross-dataset`
2. `deepfake detection audio spoofing ASVspoof robustness`

The search returned current IEEE records on cross-dataset generalisation, adversarial robustness, video detection and audio deepfake detection. This confirmed that the existing paper themes — generalisation, dataset shift, robustness and audio spoofing — are still active research topics.

### Consensus

Control queries:

1. `deepfake detection generalization robustness cross-dataset real-world`, filtered to 2019-2026 and computer science;
2. `deepfake detection adversarial evasion compression watermarking robustness`, filtered to 2019-2026 and computer science.

Consensus returned recent work on cross-dataset generalisation, robust audio detection, adversarial robustness and watermarking. It also surfaced a paper already present in the paper's source base: Yermakov et al., *Deepfake Detection that Generalizes Across Benchmarks*.

## Why these channels were not used to change the final source set

### IEEE Xplore

IEEE Xplore is a strong source for IEEE journals and conference proceedings. It was not used to rebuild the final source set because:

- the paper already used material from multiple publishers and venues;
- IEEE Xplore is publisher-specific and therefore does not give complete coverage of ACM, Springer, Elsevier, CVPR open-access and other relevant sources;
- replacing or adding sources after the analysis would break the traceability between the existing evidence tables, figures, conclusions and reference list;
- the purpose of this late search was coverage control, not a new literature-selection round.

### Consensus

Consensus is useful for quickly discovering academic papers and checking whether a topic is represented in recent literature. It was not used as a primary evidence source because:

- it is a search and synthesis layer, not the original publisher of the papers;
- bibliographic and methodological decisions should be checked against the original paper or publisher record;
- the existing paper already has a fixed, traceable 15-source set;
- the late check was used only to see whether relevant themes and overlapping literature could still be found.

## Source-quality criteria used in the paper

A source was judged on several features together. A well-known publisher or institution alone was not enough.

For each included source, the authors considered where possible:

1. **Origin / publisher** — scientific journal, conference, recognised academic publisher or official government institution.
2. **Date** — normally within the 2019-2026 research window.
3. **Direct relevance** — the source must contribute to at least one research question.
4. **Method clarity** — it must be clear how the study reached its result.
5. **Dataset / test context** — for performance claims, the training/test setting and media type must be understandable.
6. **Metric clarity** — AUC, AUROC, EER, accuracy or another reported measure must be named and interpretable.
7. **Traceability** — preferably a DOI, official publisher page or conference record.
8. **Limitations** — the paper's own limitations and generalisation boundaries are considered.
9. **Evidence type** — direct empirical evidence is weighted more strongly for technical performance claims than general commentary.
10. **Role in this paper** — the European Commission source is used only for legal context, not to support technical detector-performance claims.

## Result of the control search

The control search did not change the paper's evidence base. It showed that the final source set covers the main themes still returned by IEEE Xplore and Consensus: cross-dataset generalisation, robustness, audio spoofing, adversarial evasion and watermarking.

The control search improves transparency, but it does **not** make the original search fully reproducible. The original search-log limitation remains explicitly reported in the Method and in section 4.4.
