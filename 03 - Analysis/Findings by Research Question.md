# Findings by Research Question

## Main Research Question

> To what extent can AI-based deepfake detection systems reliably distinguish AI-generated or manipulated media from authentic content?

### Status

**Answered for the current focused literature sample.**

### Integrated Finding

Current AI-based deepfake detectors are **conditionally reliable**. They can achieve very strong results when test data resemble the training distribution and when the manipulation type is represented in the benchmark. Reliability falls materially when the detector is exposed to internet-sourced content, unseen generators or manipulation methods, stronger compression/codecs, acoustic variation, or deliberate adversarial evasion. The reviewed evidence therefore does not support treating one benchmark accuracy value as a universal measure of authenticity-detection reliability.

### Evidence

- SRC-A001: current cross-modality evaluation reports persistent double-digit out-of-distribution degradation and strong adversarial vulnerability in the tested setting.
- SRC-A003 and SRC-A009: strong controlled visual/audio benchmark performance demonstrates that detection can work very well in-domain.
- SRC-A004, SRC-A005, SRC-A006 and SRC-A010: cross-dataset and unseen-manipulation evidence demonstrates a generalisation gap.
- SRC-A007 and SRC-A008: deliberate attacks and more diverse deployment conditions reduce effectiveness.

### Limitations

The conclusion is bounded to passive AI-based detection represented by the reviewed literature. It does not establish a universal reliability percentage or a permanent judgement about future detectors and generators.

## Subquestion 1

> Which AI and machine learning techniques are currently used to detect deepfake images, videos, and audio?

### Finding

Current methods form a layered taxonomy rather than one dominant architecture. Visual techniques include forensic/statistical cues, CNN/transformer-based learned representations, frequency-domain analysis, generator/fingerprint signals and hybrid combinations. Video systems can additionally exploit temporal consistency. Generalisation-oriented techniques include data-generation strategies such as Self-Blended Images and feature-disentanglement approaches such as UCF. Audio detection combines spectral/cepstral evidence with increasingly end-to-end learned spectro-temporal representations, illustrated by AASIST.

### Evidence

SRC-A001, SRC-A002, SRC-A003, SRC-A005, SRC-A006, SRC-A008 and SRC-A009.

### Limitations

Technique categories overlap and differ by modality. The taxonomy is intentionally bounded to categories that contribute to the reliability analysis rather than attempting to catalogue every published detector.

## Subquestion 2

> How accurately can current deepfake detection systems identify manipulated content under real world conditions?

### Finding

No single defensible accuracy percentage exists across real-world conditions. Within-domain benchmarks can produce near-perfect visual results or very low audio error rates, but cross-domain testing is consistently harder. AASIST reports 0.83% EER on ASVspoof 2019 LA, while internet-sourced WildDeepfake causes substantial degradation for existing visual baselines. The 2026 cross-modality evaluation reports persistent double-digit out-of-distribution losses. Generalisation-specific approaches such as SBI and UCF improve cross-dataset performance but do not remove the underlying dependence on evaluation conditions.

### Evidence

SRC-A001, SRC-A003, SRC-A004, SRC-A005, SRC-A006, SRC-A008, SRC-A009 and SRC-A010.

### Limitations

Accuracy, AUC, EER and other metrics are not directly comparable across datasets and modalities. Results are therefore synthesised contextually rather than pooled.

## Subquestion 3

> What factors, such as video compression, new generative models, or deliberate attempts to avoid detection, reduce the effectiveness of deepfake detection systems?

### Finding

Five interacting factors are most strongly supported by the reviewed evidence:

1. **Compression and codecs** can suppress subtle forensic traces.
2. **Unseen generators/manipulation methods** expose overfitting to method-specific artefacts.
3. **Adversarial evasion** can deliberately move fake media toward detector decision regions associated with authentic content.
4. **Dataset/acquisition shift** changes identities, scenes, devices, speech conditions and internet-processing pipelines.
5. **Non-standardised preprocessing and evaluation** can produce misleading comparisons and obscure actual robustness.

### Evidence

SRC-A002, SRC-A003, SRC-A004, SRC-A005, SRC-A006, SRC-A007, SRC-A008, SRC-A010 and SRC-A001.

### Limitations

The factors are not exhaustive. Their magnitude depends on modality, detector architecture, training data, attack assumptions and the exact transformation applied.