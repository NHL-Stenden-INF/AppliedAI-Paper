# Analysis Framework

## Status

**Planned. No final analysis or findings have been produced.**

## Analysis Logic

Every research question has a defined route from evidence type to analysis output.

| Question | Evidence type | Planned analysis | Decision rule / caution | Planned output |
| --- | --- | --- | --- | --- |
| SQ1 | Technique descriptions from current primary/review literature | Taxonomic/thematic classification by modality and detector approach | Include only categories relevant to the final scope and reliability discussion | Technique taxonomy + concise synthesis |
| SQ2 | Empirical metrics with dataset/test/generalisation context | Contextual comparative synthesis | Compare only genuinely comparable metrics/conditions; separate in-domain from broader generalisation | Performance comparison with explicit boundaries |
| SQ3 | Robustness/generalisation/evasion evidence | Thematic synthesis of factors plus effect direction/magnitude/context where reported | Do not treat hypothesised limitations as measured effects | Degradation/failure-factor matrix |
| MRQ | Completed SQ1–SQ3 evidence plus source-quality/directness assessments | Integrative synthesis | Weight conclusions by evidence quality, directness and generalisability; preserve contradictions | Bounded reliability judgement |

## Operational Definitions Dependency

No evidence should be coded as `current`, `reliable` or `real-world` until those terms have been explicitly operationalised in Phase 2.

## Comparison / Extraction Fields

- source/evidence ID;
- media modality;
- manipulation/deepfake type;
- detector technique/model family;
- training dataset/context;
- test dataset/context;
- seen vs unseen generator/manipulation;
- compression/quality transformation;
- metric type and value;
- false-positive / false-negative information where available;
- evaluation setting;
- evidence directness;
- source quality and limitations.

## Validation Approach

- preserve metric context rather than isolated percentages;
- corroborate important claims across multiple independent studies where feasible;
- use review-level evidence for field mapping and primary empirical evidence for major performance claims where feasible;
- record contradictory evidence explicitly;
- cross-check high-impact extraction decisions between both authors;
- document protocol changes and scope changes in the Research Log.

## Potential Analytical Structures

No theory/model is mandated by the school documents. Possible **Proposed** analytical structures include:

- modality-based detector taxonomy;
- robustness versus generalisation distinction;
- standard classification-performance measures;
- evaluation-context categories developed from the actual evidence set.

These should be adopted only when they improve analysis rather than added for formality.

## Output Constraints

- Results should present source evidence and authors' synthesis without collapsing the distinction between them.
- Figures/tables should carry evidence, not decoration.
- No conclusion should be entered into the final paper until the relevant Conclusions Matrix row has sufficient traceable evidence.

## Dependencies / Unknowns

- lecturer-approved/stable question set;
- final modality scope;
- operational definitions;
- completed search/screening protocol;
- sufficient empirical evidence;
- final decision on which metrics are comparable.