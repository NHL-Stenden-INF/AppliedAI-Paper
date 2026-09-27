# Feedback Log

## Revision context

This log now records the feedback received on the submitted paper **De betrouwbaarheid van AI-gebaseerde deepfakedetectie** and the decisions taken during the post-review revision on 27 September 2026.

The revision rule is the one required by the Applied AI module: feedback must be **considered** and used **where appropriate**. Feedback is therefore not applied mechanically when doing so would conflict with the paper requirements, create unsupported evidence, or add structure that is not required.

## Actual feedback received

### Peer review — Lucas Lübbers

#### Positive feedback retained

The reviewer identified the following strengths:

- professional and logical paper structure;
- quantitative substantiation of the results, including AUC;
- visible author synthesis instead of merely summarising sources;
- clear answers to the subquestions and main research question;
- recommendations that follow from the findings;
- useful tables and figures that support the text.

These strengths were preserved during revision.

#### Actionable feedback and processing

| Feedback | Decision | Revision made | Rationale |
| --- | --- | --- | --- |
| Add short introductions to Chapter 2 (Method) and Chapter 4 (Conclusions and Discussion) | Accepted | Added a short orientation paragraph at the start of both chapters | Improves readability without changing the required structure |
| The introduction is information-dense and the research objective appears relatively late | Accepted | Moved the research gap and objective earlier and compressed background explanation | Strengthens B2 coherence and makes the purpose visible sooner |
| Consider moving technical AUC explanation to a theoretical framework | Partly accepted | AUC explanation was shortened, but it remains in the introduction | No separate theoretical-framework chapter is required by the available module documents; adding one would increase structure and length without a clear assessment need |
| Repeat the main research question verbatim when answering it | Accepted | Section 4.2 now states the complete main research question immediately before the answer | Makes the conclusion more independently readable |
| Make the key findings in Chapter 3 more visible | Accepted, minimally | Added concise synthesis sentences at the end of the 3.1, 3.2 and 3.3 result blocks | Highlights the answer to each subquestion without adding an unnecessary extra results section |
| Make the literature-study method more reproducible, for example with numbers found/excluded | Partly accepted | The method now explicitly states the search terms, time window, inclusion logic and extraction approach, and also states that exact search platforms, complete search strings and found/excluded counts were not systematically logged | Exact counts cannot be reconstructed reliably and were therefore not fabricated; the limitation is made explicit and carried into the reliability discussion |

### Rubric-based review — Mart Velema

The completed assessment form marks all form-aspect checks as met. The substantive marking is generally strong. The clearest relative improvement opportunity is **B3: argumentation of methodological choices**. Several B2 introduction rows and the first B4 substantiation row are also marked somewhat less strongly than the highest rows.

Actions taken:

- expanded the rationale for choosing a structured literature study instead of a small primary experiment or participant study;
- made the introduction more purpose-driven and compact;
- made the main results more explicit at the end of the relevant result sections;
- preserved the existing evidence base, references, tables and figures rather than changing claims that were already well supported.

No numeric grade was inferred from the colour marks because the submitted form does not provide a completed overall grade or written grading motivation.

## Feedback not implemented literally

Two points were deliberately bounded by the evidence and module requirements:

1. **No separate theoretical-framework chapter was added.** The assessment materials require an abstract, introduction, method, results, conclusions/discussion and literature list; a separate theoretical framework is not mandatory. The relevant AUC explanation was made more concise instead.
2. **No search-result or exclusion counts were invented.** The original research process did not preserve a fully reproducible search log. The revised method and reliability discussion now state this limitation explicitly.

## Revision traceability

The detailed post-review QA and document-level changes are recorded in:

- `04 - Paper/Peer Review Revision Record.md`
- `06 - Review/Post-Review QA.md`

The revised Word document generated from the submitted paper is identified by:

- filename: `Deepfake paper - Dave & Lucas - revised after peer review.docx`
- SHA-256: `6631abf57e15ae906c1552d2a519bdbd5eb80ec022e15d832ea29a3c0c7e41f4`


## Portfolio evidence package

The complete portfolio-facing explanation is now kept in `06 - Review/Peer Feedback Portfolio Evidence/`. That folder also records the separate module-book requirement that evidence of feedback **provided to another student** must be included elsewhere and must not be inferred from the two received reviews.
