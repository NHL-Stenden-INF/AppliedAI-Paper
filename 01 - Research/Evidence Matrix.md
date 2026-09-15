# Evidence Matrix

## Status

Phase 2 evidence has been collected from twelve academic publications. The matrix below records how the evidence supports the research questions and assessment criteria. Ten sources address passive image/video/audio detection; two additional peer-reviewed sources were added to address lecturer-requested watermarking from both capability and removal-risk perspectives. The body expansion and watermarking addition were performed from this matrix and the source records; no filler claims were added merely to reach the page requirement.

## Evidence Classes

- **Direct:** directly measures/describes the claim being made.
- **Supporting:** strengthens interpretation but does not independently establish the claim.
- **Contextual:** useful background only; must not be used as the sole basis for a technical conclusion.
- **QA / Method:** evidence about the research process rather than the deepfake-detection claim itself.

| ID | Question / criterion | Evidence obtained | Main sources | Evidence class | Status |
| --- | --- | --- | --- | --- | --- |
| EVD-001 | SQ1 | Visual detector families include spatial/forensic, learned/data-driven, frequency, fingerprint, temporal and hybrid approaches | SRC-A001, SRC-A002, SRC-A003, SRC-A007 | Direct + supporting | Sufficient |
| EVD-002 | SQ1 | Generalisation-focused visual methods include self-blended training and common-feature disentanglement; audio systems use learned spectro-temporal representations | SRC-A005, SRC-A006, SRC-A009 | Direct | Sufficient |
| EVD-003 | SQ1 | Technique choice is inseparable from the evidence signal and its dependency on generator, dataset, processing and modality | SRC-A001, SRC-A002, SRC-A006, SRC-A009 | Synthesis of direct evidence | Sufficient |
| EVD-004 | SQ2 | Strong in-domain performance is demonstrated in established visual and audio benchmarks | SRC-A003, SRC-A009 | Direct | Sufficient with scope limits |
| EVD-005 | SQ2 | Cross-domain/unseen-generator/internet-sourced evaluation produces materially weaker results than controlled evaluation | SRC-A001, SRC-A004, SRC-A005, SRC-A006, SRC-A010 | Direct | Sufficient |
| EVD-006 | SQ2 | Audio performance is challenged when speaker/acoustic diversity, codecs, newer attacks and adversarial conditions increase | SRC-A008, SRC-A009 | Direct | Sufficient |
| EVD-007 | SQ2 | Metrics and protocols are heterogeneous; numerical pooling across modality/dataset/protocol is not defensible | SRC-A001, SRC-A002, SRC-A008, SRC-A010 | QA / Method | Sufficient |
| EVD-008 | SQ2/SQ3 | FaceForensics++ supplementary manipulation-classification results decline from 99.03% raw to 95.42% HQ compression and 80.49% LQ compression; these are not treated as binary deepfake-detection accuracy | SRC-A003 | Direct, bounded use | Sufficient |
| EVD-009 | SQ2 | UCF reports a conventional Xception baseline average AUC of 0.702 in its reported cross-dataset table, illustrating the margin lost under distribution shift | SRC-A006 | Direct, context-specific | Sufficient |
| EVD-010 | SQ3 | Compression and codecs suppress or alter subtle forensic/acoustic evidence | SRC-A003, SRC-A008 | Direct | Sufficient |
| EVD-011 | SQ3 | New or unseen generative/manipulation methods expose overfitting to method-specific artefacts; SBI/UCF improve but do not eliminate this problem | SRC-A005, SRC-A006, SRC-A010 | Direct | Sufficient |
| EVD-012 | SQ3 | Deliberate adversarial evasion can substantially reduce detector effectiveness in white-box and black-box settings | SRC-A001, SRC-A007, SRC-A008 | Direct | Sufficient |
| EVD-013 | SQ3 | Dataset, identity, acquisition and environment shift make external/internet/crowdsourced data harder than curated benchmarks | SRC-A004, SRC-A008 | Direct | Sufficient |
| EVD-014 | SQ3 | Non-standardised preprocessing, training settings, metrics and evaluation pipelines can make detector comparisons misleading | SRC-A002, SRC-A010 | Direct + QA | Sufficient |
| EVD-015 | SQ3/MRQ | Reliability-reducing factors can interact; no reviewed benchmark covers every combination of generator shift, processing, acquisition shift and adaptive attack | Synthesis of SRC-A001-A010 | Synthesis | Sufficient with explicit limitation |
| EVD-016 | MRQ | Reliability is conditional: strongest under validated/known conditions and progressively less certain as distribution, processing and threat conditions diverge from validation | Synthesis of SRC-A001-A010 | Synthesis of direct evidence | Sufficient |
| EVD-017 | MRQ | Evidence strength itself forms a gradient: mature for in-domain discrimination, substantial but heterogeneous for cross-domain transfer, narrower for robustness/adaptive attack | SRC-A001, SRC-A002, SRC-A004, SRC-A007, SRC-A008, SRC-A010 | Synthesis + QA | Sufficient |
| EVD-018 | B4 QA | Source set covers image, video and audio, includes primary empirical studies, benchmarks, a systematic review and a recent peer-reviewed cross-modality empirical survey | SRC-A001-A010 | QA / Method | Sufficient for focused study |
| EVD-019 | B5 QA | Reliability, validity and usability can be evaluated from the executed method, contextual evidence and explicitly bounded conclusions | Method records + SRC-A001-A010 | QA / Method | Sufficient |
| EVD-020 | Lecturer feedback / SQ1 context | Active invisible watermarking can embed a recoverable provenance signal during image generation; Stable Signature reports robust detection under image modifications | SRC-A011 | Direct | Sufficient for bounded image-watermarking analysis |
| EVD-021 | Lecturer feedback / SQ3 context | Invisible pixel-level watermarks are not inherently tamper-proof; regeneration attacks can reduce watermark detectability while preserving image quality | SRC-A012 | Direct + theoretical | Sufficient |
| EVD-022 | MRQ | Watermarking and passive detection have complementary evidence models: a verified watermark can strengthen provenance, but absence of a watermark cannot prove authenticity because marks may never have been embedded or may have been removed | SRC-A011, SRC-A012 | Synthesis of direct evidence | Sufficient with modality limitation |

## Representative Extracted Evidence

| Source | Modality | Condition | Extracted evidence used in the paper |
| --- | --- | --- | --- |
| SRC-A003 | Image/video | Controlled benchmark + compression | >1.8 million manipulated images; stronger compression makes forensic analysis harder; supplementary manipulation-method classification: 99.03% raw, 95.42% HQ, 80.49% LQ |
| SRC-A004 | Video | Internet-sourced data | 7,314 face sequences from 707 internet-collected deepfake videos; existing baselines show substantial performance decline |
| SRC-A005 | Image/video | Cross-dataset generalisation | SBI improves its baseline by 4.90 percentage points on DFDC and 11.78 percentage points on DFDCP |
| SRC-A006 | Image/video | Cross-dataset/held-out manipulation | UCF separates common from method-specific forgery information; reported Xception baseline average AUC 0.702 in the cited cross-dataset table |
| SRC-A009 | Audio | In-domain anti-spoofing | AASIST reports 0.83% EER on ASVspoof 2019 Logical Access |
| SRC-A007 | Image | Adversarial evasion | StatAttack/MStatAttack evaluated against four spatial- and two frequency-domain detectors across four datasets in white-box and black-box settings |
| SRC-A008 | Audio | Diverse attacks/codecs/adversarial shift | ASVspoof 5 includes crowdsourced speech, modern TTS/voice conversion, codecs and adversarial attacks; baseline systems are significantly challenged |
| SRC-A001 | Image/video/audio | Unified OOD + robustness evaluation | Approximately 10-15% OOD degradation in summarised scenarios and white-box attack success above 80% against undefended models in the tested setting |
| SRC-A002 | Image/video | Benchmark methodology | Fifteen detection methods across nine datasets under standardised preprocessing/evaluation; demonstrates why protocol context is required for fair comparison |
| SRC-A010 | Video | Systematic generalisation review | Overfitting and dataset diversity remain recurring limitations; only 46.3% of selected studies supported generalisation across different deepfake types as characterised by the review |
| SRC-A011 | Generated images | Active invisible watermarking | Stable Signature embeds a binary signature into latent-diffusion outputs; after cropping to retain 10% of image content, the paper reports >90% origin-detection accuracy at false-positive rate <10^-6 |
| SRC-A012 | Generated images | Deliberate watermark removal | Regeneration attacks using noise plus reconstruction reduce detection of four pixel-level invisible watermarking schemes while preserving image quality |

## Evidence Acceptance Rules Applied

1. A source that merely mentions deepfakes is contextual, not evidence of detection reliability.
2. A percentage without metric/dataset/test context is not used for a major SQ2 claim.
3. Benchmark/in-domain accuracy is not treated as proof of real-world reliability.
4. Values measuring a different task, such as FaceForensics++ manipulation-method classification, are explicitly labelled and not silently reinterpreted as binary detector accuracy.
5. Review papers support taxonomy and synthesis; primary empirical evidence is used for major performance claims where feasible.
6. Contradictory/heterogeneous evidence is retained and represented as a boundary rather than forced into one pooled score.
7. Evidence quality and evidence directness remain separate judgements.
8. Body expansion is permitted only when the added text maps back to an Evidence Matrix row or a clearly identified authors' synthesis of such rows.
9. Watermarking is not silently grouped with passive classification. Claims must state whether the evidence assumes generator participation.
10. Absence of a watermark is never used as evidence of authenticity.

## Remaining Evidence Limits

- The twelve-source sample is focused rather than exhaustive.
- Visual literature remains face-centric relative to the broader space of generated images.
- Audio and visual metrics are not directly comparable.
- New generators may emerge faster than peer-reviewed evaluation cycles.
- `Real-world` remains an operational category composed of cross-domain, internet-sourced, codec/post-processing and adversarial conditions rather than one universal benchmark.
- Robustness evidence cannot cover every possible transformation or adaptive threat.
- The added watermarking evidence is image-focused; it is not generalised to all audio/video watermarking systems.