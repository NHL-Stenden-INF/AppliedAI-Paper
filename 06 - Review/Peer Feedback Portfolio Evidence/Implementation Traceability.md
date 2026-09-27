# Implementation Traceability

## Baseline and final file

| Version | File | SHA-256 |
| --- | --- | --- |
| Original submitted version | `Deepfake paper - Dave & Lucas(1).docx` | `b92179182fc5f14e1168bef6807c5c7da76cad161ec65db9f7ef51f236eddf31` |
| Revised + final checked | `Deepfake paper - Dave & Lucas - revised after peer review.docx` | `6631abf57e15ae906c1552d2a519bdbd5eb80ec022e15d832ea29a3c0c7e41f4` |

## Feedback-to-paper mapping

| Change | Revised paper location | Evidence/reason |
| --- | --- | --- |
| Research objective moved earlier | 1. Inleiding, opening paragraph | Implements review concern that the objective appeared too late |
| AUC explanation shortened | 1. Inleiding, second paragraph | Partly implements suggestion to reduce technical density without adding a non-required theoretical framework |
| Short method orientation added | Start of 2. Methode | Implements chapter-introduction feedback |
| Method choice justified | 2. Methode — Aanpak en onderbouwing | Addresses B3 methodological-choice argumentation; explains literature study vs. limited experiment/interviews/surveys |
| Search-process limitation stated | 2. Methode — Dataverzameling | Implements reproducibility feedback without inventing historical counts |
| Key finding made explicit for technique overview | End of 3.1.4 | Implements request to make main results easier to find |
| Key finding made explicit for performance | End of 3.2.6 | Same reason |
| Key finding made explicit for degradation factors | End of 3.3.7 | Same reason |
| Short conclusion/discussion orientation added | Start of 4. Conclusies en discussie | Implements chapter-introduction feedback |
| Main research question repeated verbatim | 4.2 Antwoord op de hoofdonderzoeksvraag | Implements explicit reviewer request and strengthens standalone readability |
| Search-log limitation aligned with discussion | 4.4 Betrouwbaarheid | Keeps Method and Discussion internally consistent |

## Final-check corrections made after feedback integration

These edits were not new reviewer requests. They were made during the requested final spelling/grammar/logical-consistency check.

| Final-check issue | Correction | Why |
| --- | --- | --- |
| English phrase `generation-only studies` inside Dutch prose | Replaced with `studies die uitsluitend deepfakes genereren` | Language consistency |
| `evaluatie pipelines` | Replaced with `evaluatiepijplijnen` | Dutch compound/spelling consistency |
| Conclusion stated that published accuracy **systematically** overestimates practice performance | Softened to: published accuracy figures **can give an overly optimistic picture** | The evidence supports a strong context effect, but the original wording was broader than the reviewed evidence warrants |
| `Interpreteerbaarheid is de zwakste van de drie dimensies` | Changed to `Interpreteerbaarheid is in de gebruikte literatuur het minst uitgebreid onderbouwd` | Distinguishes lack of evidence from proof that the dimension itself is objectively weakest |
| `nep data` | Corrected to `nepdata` | Spelling/compound consistency |

## What was deliberately left unchanged

- main research question and all three subquestions;
- 15-source evidence base;
- numerical results;
- dataset sizes;
- AUC/AUROC/EER values;
- figure data;
- three tables and two figures;
- legal date/context already cited;
- recommendation set, except for language cleanup;
- scope across image, video and audio.

Reason: the reviews did not identify factual errors in these elements, and changing them without new source evidence would be unnecessary.

## Integrity rule

No change in this revision introduces a new empirical result, source, search count, approval claim or research action that was not supported by the original research record.
