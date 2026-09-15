### 3.3 Factors that reduce detection effectiveness

SQ3 asks why passive detector effectiveness falls. The passive-detection evidence supports five main factor classes: compression and codecs, unseen generators or manipulation methods, deliberate evasion, dataset/acquisition shift, and evaluation-pipeline differences. The lecturer-requested watermarking evidence adds a separate provenance-specific boundary: watermark coverage and removal. These factors and boundaries are analytically separable, but several can occur together in actual media. A deepfake from a new generator may also be compressed, uploaded through an unknown platform, recorded or re-recorded, and intentionally modified to evade a detector.

#### 3.3.1 Compression, codecs, and ordinary post-processing

Compression changes the signal without changing the semantic content of the media. For deepfake detection this is important because many detectors rely on low-level artefacts that are weaker than the main visual or acoustic content. FaceForensics++ demonstrates that increasing visual compression reduces the quality of manipulation evidence and makes forensic analysis harder (Rössler et al., 2019). The decrease in the supplementary manipulation-classification figures from raw to strongly compressed video illustrates the magnitude with which processing can alter measurable cues, even before considering a new generator.

ASVspoof 5 treats the same issue explicitly for audio by incorporating conventional and neural codecs (Wang et al., 2024). Codec robustness is relevant because synthetic speech may be generated at high quality but later transmitted through telephony, messaging, streaming, or platform-specific compression. A detector trained on clean waveform artefacts may therefore receive a transformed signal at inference time. Across modalities, compression is a distribution shift created by normal media handling rather than by generation itself.

The evidence suggests two reliability consequences. First, a detector should not be described as robust merely because it tolerates mild compression inside its own benchmark; the strength and type of transformation matter. Second, the same preprocessing can affect detector families differently. A spatial detector, frequency detector, and temporal detector do not necessarily lose the same information when a video is recompressed. Robustness is therefore model- and transformation-specific.

#### 3.3.2 New or unseen generators and manipulation methods

Unseen generation methods are the most direct challenge to supervised deepfake detection. Training labels tell a model which examples are real and fake, but they do not force the model to learn the causal property that all future fakes will share. If a detector instead learns an artefact associated with one generator, that artefact may disappear when another generator is used. UCF's separation of method-specific and common forgery features is designed precisely around this problem (Yan, Zhang, Fan, et al., 2023).

SBI addresses the same weakness by removing the dependence on a fixed external forgery generator when creating part of the training data (Shiohara & Yamasaki, 2022). The reported cross-dataset improvements indicate that more generic training artefacts can increase transfer. Ramanaharan et al. (2025), however, show at review level that generalisation remains inconsistent across the field. The implication is that unseen-generator performance is not a solved extension of ordinary classification; it is a distinct evaluation target that requires specific training and testing choices.

This factor also reduces the useful lifetime of a detector. A model can be state of the art at publication time yet face new generation families later. Nguyen-Le et al. (2026) identify the continuing pace of generative development as a reason to favour invariant or transferable forensic representations over memorised artefacts. Reliability is therefore partly temporal: it depends on whether the detector remains valid as the generation ecosystem changes.

#### 3.3.3 Deliberate adversarial evasion

Deliberate evasion creates a stronger threat model because the media are modified specifically to reduce detector confidence. Hou et al. (2023) propose StatAttack and MStatAttack, which use exposure changes, blur, and noise in an adversarial optimisation process. Instead of adding visually conspicuous random perturbations, the attack selects natural-looking degradations that reduce statistical differences between fake and real images. The experiments cover four spatial-domain and two frequency-domain detectors across four datasets and demonstrate effectiveness in both white-box and black-box settings.

This result is significant for two reasons. First, it shows that an attacker does not need to reproduce the internal feature representation of every detector exactly; transfer can occur across models. Second, the attack manipulations resemble transformations that might already occur during ordinary media processing. This makes it harder to separate 'benign degradation' from 'malicious evasion' by visual inspection alone.

Nguyen-Le et al. (2026) extend the robustness concern across modalities and report white-box attack success rates above 80% against undefended models in the tested setting. ASVspoof 5 incorporates adversarial attacks into the speech-deepfake challenge for the first time and similarly reports that attacks significantly compromise baseline systems (Wang et al., 2024). Together, these sources show that adversarial robustness cannot be inferred from ordinary clean-test performance. A detector can be highly accurate on untouched benchmark samples and still be vulnerable when an attacker is allowed to optimise the input.

#### 3.3.4 Watermark removal and provenance limits

The watermarking evidence introduces a distinct reliability failure mode. Stable Signature shows that an embedded provenance signal can survive substantial ordinary modification (Fernandez et al., 2023), whereas Zhao et al. (2024) show that pixel-level invisible watermarks can be deliberately removed through regeneration attacks. Watermark reliability therefore has two separate dimensions: survival under benign processing and resistance to an adaptive remover.

Coverage is another limit. A passive detector can attempt to classify any supported input, whereas a watermark verifier only has evidence when a compatible mark was inserted. An absent or unreadable mark is ambiguous: the content may be authentic, unwatermarked synthetic media, or synthetic media from which the mark was degraded or removed. Watermarking should therefore provide positive provenance evidence when verification succeeds, not a universal negative test for authenticity.

#### 3.3.5 Dataset, identity, acquisition, and environment shift

Dataset shift is broader than unseen generation method. It includes differences in people, scenes, cameras, microphones, resolution, recording environments, background noise, editing, and other properties that may correlate with the label in a research dataset. WildDeepfake changes many of these variables simultaneously by using internet-sourced videos (Zi et al., 2020). The substantial reduction in baseline performance indicates that detectors can depend on dataset-specific regularities even when they were designed to learn manipulation artefacts.

In audio, ASVspoof 5 expands speaker and acoustic diversity through crowdsourcing (Wang et al., 2024). This is the acoustic equivalent of moving from curated face datasets toward less controlled real-world material. The shared lesson is that data diversity matters not merely because it increases training-set size, but because it reduces the chance that the model confuses environmental regularities with evidence of authenticity.

Dataset shift also complicates interpretation of model comparisons. If one method is evaluated on a clean, balanced dataset and another on a more heterogeneous internet dataset, their headline scores do not measure the same difficulty. DeepfakeBench's standardisation effort is therefore relevant not only for reproducibility but also for reliability claims: without a shared evaluation pipeline, performance differences can reflect the benchmark rather than the detector (Yan, Zhang, Yuan, et al., 2023).

#### 3.3.6 Non-standardised preprocessing and evaluation

DeepfakeBench identifies inconsistent data processing, experimental settings, metrics, and evaluation strategies as a major problem in the literature (Yan, Zhang, Yuan, et al., 2023). This factor differs from the others because it does not necessarily reduce the true technical capability of a detector. Instead, it can reduce the reliability of the *evidence used to judge* that capability. Two methods may appear to differ because they used different face crops, augmentation, train/test splits, backbone settings, or metrics.

For the present paper this finding justifies the decision not to pool reported percentages. A detector that reports 99% accuracy on one balanced in-domain dataset cannot be declared more reliable than a detector that reports a lower AUC on an unseen internet dataset. The evaluation questions are different. Reliability claims therefore require transparent reporting of training data, test data, metric, preprocessing, and whether the manipulation or generator was seen during training.

The systematic review by Ramanaharan et al. (2025) supports the same concern from a broader perspective: generalisation claims are difficult to compare when studies define cross-dataset or cross-manipulation evaluation differently. Standardised benchmarking is consequently part of the solution, but it must include difficult shifted conditions rather than standardise only easy in-domain tests.

#### 3.3.7 Interaction between failure factors

The five passive-detection factors are most dangerous when they interact. Consider a video generated by a method absent from the detector's training set, recompressed by a social platform, and intentionally blurred before upload. The detector then faces generator shift, codec shift, acquisition/post-processing shift, and potentially adversarial manipulation at the same time. Watermark coverage or removal can add a separate provenance uncertainty when an active marking system is involved. None of the reviewed benchmarks fully represents every such combination. This explains why 'real-world reliability' cannot be reduced to one extra test dataset.

Table 3 maps the supported factor classes and provenance boundary to the three media modalities. Each cell states whether the reviewed evidence is direct, indirect/relevant, or not evaluated for that modality. The table therefore represents evidence coverage rather than implying that all six rows are equivalent passive-detector failure mechanisms.

**Table 3. Reliability-reducing factors across modalities**

| Factor | Image | Video | Audio | Main evidence |
|---|---|---|---|---|
| Compression / codecs | Direct | Direct | Direct | Rössler et al. (2019); Wang et al. (2024) |
| Unseen generator / manipulation | Direct | Direct | Direct at challenge level | Shiohara & Yamasaki (2022); Yan, Zhang, Fan, et al. (2023); Wang et al. (2024) |
| Adversarial evasion | Direct | Relevant through frame/image attacks | Direct | Hou et al. (2023); Nguyen-Le et al. (2026); Wang et al. (2024) |
| Watermark absence / removal | Direct for generated images | Not evaluated in reviewed video evidence | Not evaluated in reviewed audio evidence | Fernandez et al. (2023); Zhao et al. (2024) |
| Dataset / acquisition shift | Direct | Direct | Direct | Zi et al. (2020); Wang et al. (2024) |
| Evaluation-pipeline variation | Direct | Direct | Direct in cross-study interpretation | Yan, Zhang, Yuan, et al. (2023); Nguyen-Le et al. (2026) |

SQ3 is therefore answered by a set of interacting boundary conditions rather than one isolated weakness. Compression can erase cues, unseen generators can invalidate learned shortcuts, adversarial attacks can exploit model sensitivity, watermark signals can be unavailable or deliberately removed, dataset shift can introduce unfamiliar content and environments, and non-standardised evaluation can make performance look more transferable than it is. These factors explain why detector reliability decreases as the evaluation moves away from the controlled conditions in which a model was developed.

### 3.4 Integrated reliability profile across the three subquestions

The three subquestions reveal one consistent structure. SQ1 shows that passive detectors learn spatial, frequency, temporal, fingerprint, and spectro-temporal signals; SQ2 shows that these signals can be highly discriminative when test conditions resemble training; SQ3 explains why passive performance falls when processing, generators, datasets, or attacker behaviour change. The watermarking evidence adds a complementary provenance layer with its own coverage and removal limits. Reliability is therefore not equivalent to one benchmark score but depends on discrimination, generalisation, robustness, and - where active provenance is available - the validity of the watermark signal.

This avoids two opposite overstatements. Deepfake detection is not simply unreliable, because FaceForensics++, AASIST, and other controlled benchmarks demonstrate strong capability. It is also not universally reliable, because WildDeepfake, cross-dataset studies, ASVspoof 5, and adversarial evaluations show material degradation outside familiar conditions. The most useful property is therefore evaluation breadth: evidence becomes stronger when validation includes the shifts expected in deployment.

Watermarking adds a complementary provenance channel rather than another passive classifier. When a participating generator embeds a mark and verification succeeds, attribution can be stronger because the signal is tied directly to the generation pipeline (Fernandez et al., 2023). However, removal attacks and unwatermarked generators mean that an absent mark cannot establish authenticity (Zhao et al., 2024). Passive detection and watermarking should therefore be interpreted as complementary layers.

Across image, video, and audio, the same reliability pattern remains visible despite different signals. Evidence is strongest for controlled discrimination, substantial but heterogeneous for cross-domain transfer, and narrower for robustness against processing, adaptive attacks, and watermark removal. Confidence in a result should therefore increase only when validation covers the media distribution, processing pipeline, provenance assumptions, and attacks expected in the intended use environment.