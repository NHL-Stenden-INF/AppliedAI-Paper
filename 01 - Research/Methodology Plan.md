# Methodology Plan

## Status

**Proposed / Planned — audited for feasibility. No research has been executed.**

The school does not prescribe one named research method for the period-1 paper. The assessment form does require B3 to describe population/sample, data collection, instruments, analysis and argumentation of methodological choices.

## Proposed Research Approach

**Structured literature study / desk research using document analysis, comparative evidence extraction and thematic synthesis.**

This repository does **not** claim a full systematic literature review unless a later protocol actually meets that standard. The purpose is a transparent, reproducible literature-based investigation that is feasible within the four-week paper period.

## Why This Method Fits the Questions

- SQ1 asks which detection techniques are used: literature/document evidence can establish a technique taxonomy.
- SQ2 asks how accurately systems perform under defined conditions: empirical studies can provide metrics and evaluation context.
- SQ3 asks which factors reduce effectiveness: robustness/generalisation/evasion studies can provide direct evidence.
- No available school source mandates interviews, surveys, participant research, detector implementation or primary empirical testing for this paper.

## B3 Operationalisation for Document Research

The interpretation below is **Proposed project methodology**, because the rubric does not explain how B3 should be applied to literature-only studies.

| B3 rubric item | Proposed operationalisation |
| --- | --- |
| Population and sample | Population = potentially eligible publications/evidence records within defined search scope; sample = included publications after documented screening |
| Data collection | Documented database/search-system queries and screening procedure |
| Instruments | Search protocol, eligibility checklist, source-assessment fields and evidence-extraction matrix |
| Analysis | Taxonomic, comparative and thematic synthesis by research question |
| Argumentation of choices | Justify scope, search strategy, source types, eligibility rules, metric handling and synthesis limits |

**To Verify:** lecturer/assessor acceptance of this B3 operationalisation.

## Selection Strategy

### Candidate Evidence Population

Potentially relevant scholarly/technical publications concerning AI-based deepfake detection within the final operational scope.

### Planned Sample

Publications that pass documented title/abstract and, where needed, full-text eligibility screening.

### Inclusion Criteria — To Finalise Before Extraction

Planned criteria should cover:

- direct relevance to SQ1, SQ2 and/or SQ3;
- modality within final scope;
- clear method/evidence basis;
- sufficient detail to interpret the claimed result;
- identifiable publication date/source context;
- for performance claims, explicit evaluation data/metrics/conditions where possible.

### Exclusion Criteria — To Finalise Before Extraction

Planned exclusions should cover:

- generation-only work without detection relevance;
- unsupported commentary used as evidence for technical performance;
- duplicates;
- material outside final scope;
- sources whose result cannot be interpreted or traced well enough for the intended claim.

Publication-year, language, preprint/grey-literature and access rules are not yet fixed and must be recorded before final screening.

## Planned Procedure

1. Record each search system, exact query, date and result count.
2. Deduplicate records.
3. Screen titles/abstracts using the final eligibility rules.
4. Check full text for sources supporting important claims.
5. Record important exclusion decisions where they affect coverage.
6. Assess source authority, currency, method/evidence basis, directness and limitations.
7. Extract evidence into standard fields.
8. Cross-check high-impact sources/values between both authors.
9. Analyse by research question.
10. Reassess gaps and contradictory evidence before conclusions.

## Extraction Instrument

For relevant empirical evidence, record where available:

- source ID and publication year;
- media modality;
- manipulation/deepfake type;
- detector technique/model family;
- training dataset/context;
- test dataset/context;
- seen vs unseen generator/manipulation;
- transformations such as compression/quality changes;
- performance metric and value;
- false-positive/false-negative or equivalent error information;
- evaluation setting;
- limitations stated by authors;
- evidence directness and source-quality assessment.

## Planned Analysis

### SQ1

Create a bounded taxonomy of detector approaches relevant to the final scope. Avoid an exhaustive catalogue when a technique does not contribute to the reliability analysis.

### SQ2

Compare reported performance with metric, dataset and test context preserved. Do not pool or rank values across incompatible conditions. Separate controlled/in-domain performance from cross-dataset, unseen-generator or otherwise operationalised real-world evidence.

### SQ3

Group degradation/generalisation factors and synthesise the direction, magnitude and consistency of effects where evidence allows.

### MRQ

Integrate SQ1–SQ3 into a bounded judgement of reliability, explicitly stating where evidence is strong, inconsistent or non-generalizable.

## Reliability Controls

- documented search/screening rules;
- stable source/evidence IDs;
- exact metric/context capture;
- duplicate handling;
- cross-check of important extraction decisions by both authors;
- research log of changes to criteria and scope.

## Validity Controls

- operational definitions before evidence extraction;
- direct evidence for technical performance claims;
- clear distinction between in-domain accuracy and generalisation/robustness;
- coverage across the modalities actually retained in scope;
- avoidance of conclusions beyond the evaluated conditions;
- explicit treatment of source limitations and contradictory findings.

## Usability / Applicability Considerations

The later discussion should distinguish whether evidence supports conclusions for controlled research settings, particular media types/datasets, or broader practical use. `Usability` must not be interpreted as deployment usefulness without evidence.

## Triangulation Decision

No participant-method triangulation is currently justified by the research questions. Appropriate triangulation here means comparing **multiple independent studies/evidence types** for important claims and using both review-level mapping and primary empirical evidence where useful.

An additional technical replication is **not part of the active plan**. It should only be proposed later if a specific evidence gap cannot be answered responsibly from literature and if the lecturer agrees that it is feasible and relevant.

## Expected Limitations

- publication and reporting bias;
- heterogeneous datasets/metrics/protocols;
- rapid evolution of generative models;
- incomplete comparability across image/video/audio;
- practical time constraints;
- potential overrepresentation of benchmark conditions compared with true deployment settings.

## Readiness

**Mostly Prepared / Ready with protocol conditions.** Finalise operational definitions, eligibility rules, search strategy and lecturer acceptance of the question set before treating evidence extraction as final.