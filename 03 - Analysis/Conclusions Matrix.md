# Conclusions Matrix

| Research question | Evidence threshold before conclusion | Current evidence | Analysis route | Conclusion status | Confidence | Remaining limitation |
| --- | --- | --- | --- | --- | --- | --- |
| SQ1 | Multiple relevant sources support a defensible current technique taxonomy across final scope | Passive visual/video/audio technique evidence from SRC-A001, A002, A003, A005, A006, A008, A009 plus active image-watermarking evidence from SRC-A011 | Taxonomic/thematic synthesis with active/passive distinction | Available | High for high-level taxonomy | Categories overlap; watermarking evidence is image-focused |
| SQ2 | Sufficient empirical results with metric/dataset/test context, including evidence beyond only in-domain benchmarks | In-domain + cross-dataset + internet-sourced + audio challenge evidence from SRC-A001, A003, A004, A005, A006, A008, A009, A010; watermark robustness reported separately in SRC-A011 | Contextual comparative synthesis; watermark metrics not pooled with passive metrics | Available | Moderate-High | Heterogeneous metrics/tasks prevent pooled accuracy |
| SQ3 | Direct evidence for key degradation/generalisation/evasion factors with context | Five passive factor classes supported by SRC-A001-A010, plus separate watermark coverage/removal evidence from SRC-A011/A012 | Thematic/effect synthesis with provenance boundary separated | Available | High for identified passive factor classes | Effect magnitude is detector/context specific; watermark evidence is image-specific |
| MRQ | SQ1-SQ3 answered with traceable evidence, source quality assessed, major contradictions addressed | Integrated twelve-source evidence base with explicit generalisation/robustness and watermark-provenance boundaries | Integrative synthesis | Available | Moderate-High | Focused rather than exhaustive review; rapidly changing field |

## Supported Conclusions

### SQ1

Deepfake detection currently uses multiple complementary passive technique families. Visual systems rely on learned spatial/frequency representations, forensic/statistical artefacts, temporal cues, fingerprints and hybrid combinations. Audio systems combine spectral-temporal evidence with increasingly end-to-end learned representations. Generalisation-oriented methods explicitly attempt to reduce dependence on one manipulation method or dataset. In addition, active invisible watermarking can embed an explicit provenance signal at generation time; this is analytically distinct from passive detection because it assumes generator participation.

### SQ2

Current passive systems can be highly accurate in controlled or in-domain tests, but no single accuracy percentage represents real-world reliability. Cross-domain, internet-sourced and more diverse challenge conditions produce materially weaker performance, while specialised generalisation methods improve but do not eliminate the gap. Watermark-origin detection can also be robust under some transformations, but its metrics answer a different provenance-verification question and are therefore not pooled with passive detector accuracy.

### SQ3

The five strongest passive-detection factor classes are compression/codecs, unseen generation or manipulation methods, deliberate adversarial evasion, dataset/acquisition shift and inconsistent preprocessing/evaluation conditions. Watermark coverage/removal is a separate provenance-specific boundary: a mark may be absent, degraded or deliberately removed. For watermarking specifically, survival under benign transformations and resistance to deliberate removal are separate properties.

### MRQ

AI-based deepfake detectors are **conditionally reliable**: strong when evaluated under familiar conditions, but substantially less dependable under distribution shift, post-processing and adaptive attack. Watermarking can add direct provenance evidence when a participating generator embeds a detectable signal, but it does not replace passive detection because marks may be absent, unsupported or deliberately removed. Detector output and watermark verification should therefore be interpreted within their validated operating conditions rather than as universal proof that media is authentic or manipulated.

## Rule Applied

Conclusions were only entered after the Evidence Matrix contained direct, contextualised evidence for the relevant question. Numerical evidence was not pooled when modalities, datasets, metrics, protocols or tasks were incompatible. Watermark-origin metrics were kept separate from passive deepfake-classification metrics, and absence of a watermark was not interpreted as evidence of authenticity.