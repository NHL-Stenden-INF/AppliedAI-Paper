# Conclusions Matrix

| Research question | Evidence threshold before conclusion | Current evidence | Analysis route | Conclusion status | Confidence | Remaining limitation |
| --- | --- | --- | --- | --- | --- | --- |
| SQ1 | Multiple relevant sources support a defensible current technique taxonomy across final scope | Visual, video and audio technique evidence from SRC-A001, A002, A003, A005, A006, A008, A009 | Taxonomic/thematic synthesis | Available | High for high-level taxonomy | Categories overlap; not exhaustive |
| SQ2 | Sufficient empirical results with metric/dataset/test context, including evidence beyond only in-domain benchmarks | In-domain + cross-dataset + internet-sourced + audio challenge evidence from SRC-A001, A003, A004, A005, A006, A008, A009, A010 | Contextual comparative synthesis | Available | Moderate-High | Heterogeneous metrics prevent pooled accuracy |
| SQ3 | Direct evidence for key degradation/generalisation/evasion factors with context | Compression, unseen manipulation, dataset shift and adversarial evidence from SRC-A001, A002, A003, A004, A005, A006, A007, A008, A010 | Thematic/effect synthesis | Available | High for identified factor classes | Effect magnitude is detector/context specific |
| MRQ | SQ1-SQ3 answered with traceable evidence, source quality assessed, major contradictions addressed | Integrated ten-source evidence base with explicit generalisation/robustness boundaries | Integrative synthesis | Available | Moderate-High | Focused rather than exhaustive review; rapidly changing field |

## Supported Conclusions

### SQ1

Deepfake detection currently uses multiple complementary technique families. Visual systems rely on learned spatial/frequency representations, forensic/statistical artefacts, temporal cues, fingerprints and hybrid combinations. Audio systems combine spectral-temporal evidence with increasingly end-to-end learned representations. Generalisation-oriented methods explicitly attempt to reduce dependence on one manipulation method or dataset.

### SQ2

Current systems can be highly accurate in controlled or in-domain tests, but no single accuracy percentage represents real-world reliability. Cross-domain, internet-sourced and more diverse challenge conditions produce materially weaker performance, while specialised generalisation methods improve but do not eliminate the gap.

### SQ3

The strongest evidence-based causes of reduced effectiveness are compression/codecs, unseen generation or manipulation methods, deliberate adversarial evasion, dataset/acquisition shift and inconsistent preprocessing/evaluation conditions.

### MRQ

AI-based deepfake detectors are **conditionally reliable**: strong when evaluated under familiar conditions, but substantially less dependable under distribution shift, post-processing and adaptive attack. Detector output should therefore be interpreted within its validated operating conditions rather than as universal proof that media is authentic or manipulated.

## Rule Applied

Conclusions were only entered after the Evidence Matrix contained direct, contextualised evidence for the relevant question. Numerical evidence was not pooled when modalities, datasets, metrics or protocols were incompatible.