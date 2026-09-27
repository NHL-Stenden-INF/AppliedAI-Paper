# Peer Review Revision Record

## Document

**Paper:** De betrouwbaarheid van AI-gebaseerde deepfakedetectie  
**Authors:** Lucas Wanink & Dave van den Berg  
**Revision date:** 27 September 2026  
**Basis:** submitted DOCX plus two received reviews and the Applied AI module-book / research-paper assessment requirements.

## Revision principles

The submitted paper was not rewritten from scratch. The revision preserves claims, figures, tables and references that were already supported, and only changes material where review feedback identified a meaningful improvement.

The Applied AI module requires authors to consider received peer feedback and use it where appropriate. It does not require every suggestion to be implemented literally. No evidence, search counts, approvals or research activities were invented during revision.

## Implemented document changes

### 1. Introduction

Changes:

- moved the research gap and research objective into the opening paragraph;
- compressed background material about deepfakes, AUC and the EU AI Act;
- retained the main research question, three subquestions, scope and reading guide;
- kept the reliability dimensions and operational definition of practice conditions visible before the questions.

Reason:

The peer review noted that the introduction contained relevant information but that the research objective appeared relatively late. The change improves the logical route from context -> gap -> objective -> questions without adding a new theoretical-framework chapter.

### 2. Method

Changes:

- added a short chapter introduction describing what the method chapter covers;
- strengthened the methodological justification for a structured literature study;
- explicitly explained why a small primary detector experiment or participant study would not answer the three research questions as broadly;
- retained population/sample, data collection, instruments and analysis;
- added an explicit reproducibility limitation: exact search platforms, complete search strings, and counts of found/excluded publications were not systematically logged.

Reason:

This directly addresses the peer-review request for a more reproducible method and the relatively weaker rubric indication for methodological-choice argumentation. Missing historical search counts were not reconstructed because doing so would create unsupported evidence.

### 3. Results

Changes:

- preserved the existing 3.1 / 3.2 / 3.3 structure and quantitative evidence;
- added one concise synthesis statement at the end of each major results block:
  - 3.1: technique family alone does not predict generalisation;
  - 3.2: performance decreases as test material moves further from the training environment;
  - 3.3: multiple degradation factors can act simultaneously.

Reason:

The peer review stated that important findings could disappear among the detail. The revision therefore highlights the main result of each subquestion without introducing repetitive summaries or a new chapter.

### 4. Conclusions and discussion

Changes:

- added a short chapter introduction;
- repeated the main research question verbatim in section 4.2 before answering it;
- retained the direct answers to all three subquestions;
- retained the five recommendations;
- aligned the reliability discussion with the newly explicit method limitation concerning the search log.

Reason:

The peer reviewer specifically requested that the main research question be repeated word-for-word so the conclusion can function more independently.

## Feedback deliberately not implemented literally

### Separate theoretical framework

Not added.

The assessment requirements list a concise abstract, introduction, method, results, conclusions/discussion and literature list. A separate theoretical-framework chapter is not mandatory. The relevant technical explanation was shortened instead of moving it into a new chapter.

### Exact numbers of found and excluded publications

Not added.

Those numbers were not preserved during the original search process. The revision states the limitation explicitly rather than fabricating a reproducibility trail after the fact.

## Unchanged strengths

The following parts were intentionally retained:

- the same main research question and three subquestions;
- the same evidence-supported conclusions;
- the three existing tables;
- the two synthesis figures;
- the 15-source reference base;
- the distinction between same-dataset, unseen-research-dataset and online-circulating content;
- the conclusion that detector accuracy is context-dependent and should not be represented by one universal score.

## Revised file

Generated revised DOCX:

`Deepfake paper - Dave & Lucas - revised after peer review.docx`

SHA-256:

`162f7224b29717845a2cd4aa21d743bdc39c01a2e9c63b80bdb322e809f70c42`

The original submitted DOCX was retained unchanged outside this revision:

`Deepfake paper - Dave & Lucas(1).docx`

Original SHA-256:

`b92179182fc5f14e1168bef6807c5c7da76cad161ec65db9f7ef51f236eddf31`
