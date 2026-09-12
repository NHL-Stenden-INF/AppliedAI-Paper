# Evidence Matrix

## Status

Phase 2 evidence has been collected from ten academic publications. The matrix below records how the evidence supports the research questions and assessment criteria. Performance values are only used when the source provides sufficient metric/dataset/test context.

## Evidence Classes

- **Direct:** directly measures/describes the claim being made.
- **Supporting:** strengthens interpretation but does not independently establish the claim.
- **Contextual:** useful background only; must not be used as the sole basis for a technical conclusion.
- **QA / Method:** evidence about the research process rather than the deepfake-detection claim itself.

| ID | Question / criterion | Evidence obtained | Main sources | Evidence class | Status |
| --- | --- | --- | --- | --- | --- |
| EVD-001 | SQ1 | Visual detector families include forensic, learned/data-driven, fingerprint and hybrid approaches; video additionally uses temporal evidence | SRC-A001, SRC-A002, SRC-A003 | Direct + supporting | Sufficient |
| EVD-002 | SQ1 | Generalisation-focused visual methods include self-blended training and common-feature disentanglement; audio systems use spectro-temporal learned representations | SRC-A005, SRC-A006, SRC-A009 | Direct | Sufficient |
| EVD-003 | SQ1 | Current relevance is supported by a 2026 cross-modality survey/empirical evaluation and 2024 audio benchmark | SRC-A001, SRC-A008 | Supporting | Sufficient |
| EVD-004 | SQ2 | Strong in-domain performance is demonstrated in established visual and audio benchmarks | SRC-A003, SRC-A009 | Direct | Sufficient with scope limits |
| EVD-005 | SQ2 | Cross-domain/unseen-generator/internet-sourced evaluation produces materially weaker results than controlled evaluation | SRC-A001, SRC-A004, SRC-A005, SRC-A006, SRC-A010 | Direct | Sufficient |
| EVD-006 | SQ2 | Audio performance also degrades when attack diversity, acoustic conditions, codecs and adversarial conditions become more realistic | SRC-A008, SRC-A009 | Direct | Sufficient |
| EVD-007 | SQ2 | Metrics/conditions are heterogeneous across modalities; numerical pooling is not defensible | SRC-A001, SRC-A002, SRC-A008 | QA / Method | Sufficient |
| EVD-008 | SQ3 | Compression and post-processing reduce the visibility of subtle forensic artefacts | SRC-A003, SRC-A008 | Direct | Sufficient |
| EVD-009 | SQ3 | New or unseen generative/manipulation methods create generalisation failures; specialist methods improve but do not remove the problem | SRC-A005, SRC-A006, SRC-A010 | Direct | Sufficient |
| EVD-010 | SQ3 | Deliberate adversarial evasion can substantially reduce detector effectiveness in white-box and black-box conditions | SRC-A001, SRC-A007, SRC-A008 | Direct | Sufficient |
| EVD-011 | SQ3 | Dataset/acquisition shift and non-standardised preprocessing/evaluation can reduce or obscure measured performance | SRC-A002, SRC-A004, SRC-A008 | Direct + supporting | Sufficient |
| EVD-012 | MRQ | Reliability is conditional: strong in known/in-domain conditions, materially weaker under distribution shift, post-processing and adaptive attacks | Synthesis of SRC-A001-A010 | Synthesis of direct evidence | Sufficient |
| EVD-013 | B4 QA | Source set covers image, video and audio; includes 2019 foundational evidence and 2020-2026 current evidence; primary studies are used for major performance claims | SRC-A001-A010 | QA / Method | Sufficient for focused study |
| EVD-014 | B5 QA | Reliability, validity and usability can be evaluated from the executed literature protocol and evidence boundaries | Method records + SRC-A001-A010 | QA / Method | Sufficient |

## Representative Extracted Evidence

| Source | Modality | Condition | Extracted evidence used in the paper |
| --- | --- | --- | --- |
| SRC-A003 | Image/video | Controlled benchmark + compression | FaceForensics++ contains more than 1.8 million manipulated images; stronger compression makes detection more difficult even when learned detectors remain comparatively strong |
| SRC-A004 | Video | Internet-sourced data | WildDeepfake contains 7,314 face sequences from 707 internet-collected deepfake videos; existing baselines show substantial performance decline on this distribution |
| SRC-A005 | Image/video | Cross-dataset generalisation | Self-Blended Images improves its baseline by 4.90 percentage points on DFDC and 11.78 percentage points on DFDCP in the reported cross-dataset tests |
| SRC-A009 | Audio | In-domain anti-spoofing | AASIST reports 0.83% EER on the ASVspoof 2019 Logical Access benchmark |
| SRC-A007 | Image | Adversarial evasion | StatAttack/MStatAttack are effective against multiple spatial- and frequency-domain detectors in white-box and black-box settings |
| SRC-A008 | Audio | Diverse attacks/codecs/adversarial shift | ASVspoof 5 includes crowdsourced speech, modern TTS/voice conversion, codecs and adversarial attacks; baseline systems are significantly challenged |
| SRC-A001 | Image/video/audio | Unified OOD + robustness evaluation | The 2026 evaluation reports persistent double-digit out-of-distribution degradation and white-box attack success above 80% against undefended models in the tested setting |

## Evidence Acceptance Rules Applied

1. A source that merely mentions deepfakes is **contextual**, not evidence of detection reliability.
2. A reported percentage without metric/dataset/test context is not used for a major SQ2 claim.
3. Benchmark/in-domain accuracy is not treated as proof of real-world reliability.
4. Review papers support taxonomy and synthesis; major performance claims are linked to primary empirical evidence where feasible.
5. Contradictory/heterogeneous evidence is retained and represented as a boundary rather than forced into one pooled score.
6. Evidence quality and evidence directness remain separate judgements.

## Remaining Evidence Limits

- The ten-source sample is focused rather than exhaustive.
- Visual literature remains face-centric relative to the broader space of generated images.
- Audio and visual metrics are not directly comparable.
- New generators may emerge faster than peer-reviewed evaluation cycles.
- `Real-world` remains an operational category composed of cross-domain, internet-sourced, codec/post-processing and adversarial conditions rather than one universal benchmark.