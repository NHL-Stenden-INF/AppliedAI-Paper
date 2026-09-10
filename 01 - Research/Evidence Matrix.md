# Evidence Matrix

## Status

No substantive academic deepfake-detection evidence has been collected. This matrix defines the evidence that Phase 2 must obtain and how it should be judged.

## Evidence Classes

- **Direct:** directly measures/describes the claim being made.
- **Supporting:** strengthens interpretation but does not independently establish the claim.
- **Contextual:** useful background only; must not be used as the sole basis for a technical conclusion.
- **QA / Method:** evidence about the research process rather than the deepfake-detection claim itself.

| ID | Question / criterion | Required evidence | Preferred evidence class | Minimum context to capture | Existing evidence | Status |
| --- | --- | --- | --- | --- | --- | --- |
| EVD-001 | SQ1 | Defensible classification of current deepfake-detection technique families | Direct + supporting | Modality, detector family/features, source year | None | Missing |
| EVD-002 | SQ1 | Modality-specific signals/features/representations used by detectors | Direct | Modality, approach, evidence basis | None | Missing |
| EVD-003 | SQ1 | Evidence that included technique categories are current/relevant | Supporting | Publication date, field coverage, limitations | None | Missing |
| EVD-004 | SQ2 | Reported detector performance | Direct | Metric, value, dataset, modality, detector, test condition | None | Missing |
| EVD-005 | SQ2 | Controlled/in-domain versus generalised or operationally real-world performance | Direct | Training/test relation, seen/unseen generator, transformations, metric | None | Missing |
| EVD-006 | SQ2 | Error behaviour where available | Direct | False positives/false negatives or equivalent metric/context | None | Missing |
| EVD-007 | SQ2 | Modality-specific evidence when metrics/conditions are not comparable | Direct | Modality + comparison boundaries | None | Missing |
| EVD-008 | SQ3 | Effect of compression/quality degradation | Direct | Transformation level, detector, metric before/after or comparative effect | None | Missing |
| EVD-009 | SQ3 | Generalisation to new/unseen generative models/manipulations | Direct | Seen/unseen condition, dataset/generator, metric | None | Missing |
| EVD-010 | SQ3 | Deliberate evasion/adversarial robustness | Direct | Attack/evasion condition, threat assumptions, metric/effect | None | Missing |
| EVD-011 | SQ3 | Other evidence-based degradation factors | Direct | Factor, test condition, effect, limitations | None | Planned discovery |
| EVD-012 | MRQ | Integrated reliability judgement | Synthesis of direct evidence | Evidence quality, modality, conditions, conflicting results | None | Missing |
| EVD-013 | B4 QA | Source base is adequate in amount/completeness/timeliness/quality/relevance | QA / Method | Coverage by SQ/modality/year/source quality | Assessment criterion only | Planned |
| EVD-014 | B5 QA | Research reliability/validity/usability can be evaluated | QA / Method | Executed protocol, deviations, limitations, applicability | Method plan only | Planned |

## Evidence Acceptance Rules

1. A source that merely mentions deepfakes is **contextual**, not evidence of detection reliability.
2. A reported percentage without metric/dataset/test context is insufficient for a major SQ2 claim.
3. Benchmark/in-domain accuracy is not automatically evidence of `real-world` reliability.
4. Review papers may support taxonomy/coverage, but important performance claims should be traceable to primary empirical evidence where feasible.
5. Contradictory evidence remains in the matrix and must be analysed.
6. Evidence quality and evidence directness are separate judgments: a high-quality source can still be only contextual for a specific claim.

## Phase-2 Source Quality Fields

For each important source assess:

- authority/publication context;
- relevance to the specific question/claim;
- currency;
- method/evidence basis;
- evaluation transparency;
- independence/potential bias where relevant;
- directness;
- limitations/generalisation risk;
- primary empirical vs review/synthesis vs commentary status.