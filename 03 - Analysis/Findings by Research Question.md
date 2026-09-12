# Findings by Research Question

## Main Research Question

> To what extent can AI-based deepfake detection systems reliably distinguish AI-generated or manipulated media from authentic content?

### Status

**Answered for the current focused literature sample.**

### Integrated Finding

Current AI-based deepfake detectors are **conditionally reliable**. They can achieve very strong discrimination when test data resemble the training distribution and when the manipulation type is represented in the benchmark. Reliability falls materially when the detector is exposed to internet-sourced content, unseen generators or manipulation methods, stronger compression/codecs, acoustic variation, acquisition shift, or deliberate adversarial evasion. The reviewed evidence therefore does not support treating one benchmark accuracy value as a universal measure of authenticity-detection reliability.

The expanded analysis adds an important qualification: confidence in a detector result should increase only when its validation coverage resembles the intended use environment. Benchmark capability is the best-characterised part of the evidence base; cross-domain transfer is substantial but heterogeneous; robustness against processing and adaptive attacks is narrower and more threat-specific. Reliability should therefore be treated as a chain from discrimination to generalisation to robustness rather than as a single score.

### Evidence

- SRC-A001: recent cross-modality empirical evaluation reports approximately 10-15% OOD degradation in summarised scenarios and strong adversarial vulnerability in the tested setting.
- SRC-A003 and SRC-A009: strong controlled visual/audio benchmark performance demonstrates high in-domain capability.
- SRC-A004, SRC-A005, SRC-A006 and SRC-A010: internet-sourced, cross-dataset and unseen-manipulation evidence demonstrates a generalisation gap.
- SRC-A007 and SRC-A008: deliberate attacks and broader deployment conditions reduce effectiveness.
- SRC-A002: standardised benchmarking demonstrates that preprocessing, datasets, metrics and protocols must be preserved when reliability claims are compared.

### Limitations

The conclusion is bounded to passive AI-based detection represented by the reviewed literature. It does not establish a universal reliability percentage, cover every image-generation family or adaptive attack, or provide a permanent judgement about future detectors and generators.

## Subquestion 1

> Which AI and machine learning techniques are currently used to detect deepfake images, videos, and audio?

### Finding

Current methods form a layered taxonomy rather than one dominant architecture. Visual techniques include spatial/forensic cues, CNN/transformer-based learned representations, frequency-domain analysis, generator/fingerprint signals and hybrid combinations. Video systems can additionally exploit temporal consistency. Generalisation-oriented techniques include data-generation strategies such as Self-Blended Images and representation-disentanglement approaches such as UCF. Audio detection combines spectral/cepstral evidence with increasingly end-to-end learned spectro-temporal representations, illustrated by AASIST.

The expanded synthesis links each family to a reliability dependency. Spatial and frequency methods can learn powerful but dataset-sensitive artefacts; fingerprints may depend strongly on generator identity; temporal techniques gain an additional evidence dimension but depend on frame quality and processing; audio systems can be sensitive to speakers, acoustic environments and codecs. SBI and UCF are especially relevant because they explicitly attempt to reduce dependence on one known manipulation process.

### Evidence

SRC-A001, SRC-A002, SRC-A003, SRC-A005, SRC-A006, SRC-A007, SRC-A008 and SRC-A009.

### Limitations

Technique categories overlap and differ by modality. The taxonomy is intentionally bounded to categories that contribute to the reliability analysis rather than attempting to catalogue every published detector.

## Subquestion 2

> How accurately can current deepfake detection systems identify manipulated content under real world conditions?

### Finding

No single defensible accuracy percentage exists across real-world conditions. Within-domain benchmarks can produce near-perfect visual results or very low audio error rates, but cross-domain testing is consistently harder. AASIST reports 0.83% EER on ASVspoof 2019 LA, while internet-sourced WildDeepfake causes substantial degradation for existing visual baselines. The 2026 cross-modality evaluation reports persistent double-digit OOD loss, summarised at approximately 10-15% for the relevant scenarios. Generalisation-specific approaches such as SBI and UCF improve cross-dataset performance but do not remove dependence on evaluation conditions.

The expanded analysis makes the context problem explicit. UCF's reported cross-dataset table contains an average AUC of 0.702 for a conventional Xception baseline, showing how much margin can be lost when the test distribution changes. FaceForensics++ also demonstrates that processing changes measurable evidence: its supplementary manipulation-method classification falls from 99.03% on raw data to 95.42% under high-quality compression and 80.49% under low-quality compression. These FaceForensics++ values are used only as evidence of processing sensitivity, not as binary deepfake-detection accuracy. DeepfakeBench reinforces why such distinctions matter: detector comparisons are unreliable when preprocessing, metrics and protocols are not standardised.

### Evidence

SRC-A001, SRC-A002, SRC-A003, SRC-A004, SRC-A005, SRC-A006, SRC-A008, SRC-A009 and SRC-A010.

### Limitations

Accuracy, AUC, EER and other metrics are not directly comparable across datasets and modalities. Results are therefore synthesised contextually rather than pooled. Internet-sourced and cross-domain datasets are useful real-world proxies but do not reproduce every deployment condition.

## Subquestion 3

> What factors, such as video compression, new generative models, or deliberate attempts to avoid detection, reduce the effectiveness of deepfake detection systems?

### Finding

Five interacting factors are most strongly supported by the reviewed evidence:

1. **Compression and codecs** can suppress or transform subtle forensic and acoustic traces.
2. **Unseen generators/manipulation methods** expose overfitting to method-specific artefacts.
3. **Adversarial evasion** can deliberately move fake media toward detector decision regions associated with authentic content.
4. **Dataset/acquisition/environment shift** changes identities, scenes, devices, speakers, acoustic conditions and internet-processing pipelines.
5. **Non-standardised preprocessing and evaluation** can produce misleading comparisons and obscure actual robustness.

The expanded synthesis emphasises interaction. A new-generator video can also be recompressed, edited and intentionally blurred, which means several shifts may occur simultaneously. No reviewed benchmark covers every such combination. This is why reliability must be validated against the intended operating conditions rather than inferred from one robustness test.

### Evidence

SRC-A001, SRC-A002, SRC-A003, SRC-A004, SRC-A005, SRC-A006, SRC-A007, SRC-A008 and SRC-A010.

### Limitations

The factors are not exhaustive. Their magnitude depends on modality, detector architecture, training data, attack assumptions and the exact transformation applied. Robustness evidence is necessarily narrower than the full space of possible processing and adaptive attacks.

## Cross-Question Synthesis Used for the Expanded Body

The body expansion follows the sequence already defined in the Analysis Framework rather than introducing a new narrative:

1. identify which signals current detectors learn (SQ1);
2. determine how those systems perform when evaluation conditions change (SQ2);
3. explain the mechanisms and boundary conditions behind performance degradation (SQ3);
4. integrate these findings into a bounded reliability judgement (MRQ).

This preserves consistency between the Evidence Matrix, Results and Conclusions Matrix while providing the depth required by B4 and the 8-10-page body requirement.