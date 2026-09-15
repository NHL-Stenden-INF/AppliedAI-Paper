### 3.2 Accuracy under real-world and cross-domain conditions

A direct answer to SQ2 requires separating three questions that are often collapsed into one accuracy number: how well a detector performs on a known benchmark, how well it transfers to a different dataset or manipulation process, and how well it survives media transformations or attacks that occur after generation. The reviewed studies use accuracy, AUC, EER, and challenge-specific metrics, so a pooled percentage would be misleading. DeepfakeBench specifically identifies non-standardised preprocessing, experimental settings, evaluation strategies, and metrics as causes of unfair or misleading comparison between detectors (Yan, Zhang, Yuan, et al., 2023). Consequently, the results below preserve the evaluation context instead of ranking all systems on one scale.

#### 3.2.1 Strong performance under controlled conditions

Controlled benchmarks establish that deepfake detection is technically feasible and can be highly effective. FaceForensics++ demonstrated that data-driven visual detectors could distinguish multiple manipulation types at high accuracy and outperform human observers, even when compression was introduced (Rössler et al., 2019). The importance of this result is that it demonstrates that specific classes of manipulated media are detectable under defined conditions; it does not establish that all forms of synthetic media are equally detectable. When the manipulation families are represented in training and the data pipeline is sufficiently controlled, discriminative artefacts exist and machine-learning models can exploit them.

The audio evidence is similarly strong within a defined benchmark. AASIST reports an EER of 0.83% on the ASVspoof 2019 Logical Access evaluation set (Jung et al., 2022). EER is the operating point at which false-accept and false-reject error rates are equal, so a lower value indicates better separation between bona fide and spoofed speech. The result demonstrates that a modern anti-spoofing architecture can separate known classes of synthetic and converted speech with very low error under the benchmark conditions.

These in-domain results are necessary evidence of detector capability, but they are not sufficient evidence of general reliability. A benchmark can only test the generators, data characteristics, preprocessing choices, and attack types represented in that benchmark. The central empirical question is therefore what happens when one or more of those conditions change.

#### 3.2.2 Cross-dataset generalisation gap

The clearest recurring pattern in the reviewed literature is a performance gap between in-domain and out-of-distribution evaluation. Nguyen-Le et al. (2026), in a recent cross-modality survey with empirical evaluation, report persistent double-digit degradation in out-of-distribution testing, with approximately 10-15% performance loss in the OOD scenarios summarised by the study. Their main contribution to the present paper is not a single detector ranking but the finding that generalisation remains a cross-modality problem affecting image, video, and audio systems.

The systematic review by Ramanaharan et al. (2025) independently reaches a similar conclusion for video detection. It identifies overfitting, limited dataset diversity, and insufficient evaluation on unseen manipulation types as recurring weaknesses in the field. The review reports that only 46.3% of the selected studies supported generalisation across different deepfake types. This does not mean that the remaining studies all failed under exactly the same protocol; rather, it shows that evidence for broad generalisation is substantially less common than evidence for good performance on the datasets used during development.

UCF provides a more granular example of this difficulty. In the cross-dataset table reported in the paper, the conventional Xception baseline reports an average cross-dataset AUC of 0.683, while the UCF model using the same Xception backbone reports 0.852 in the paper's Table 7 (Yan, Zhang, Fan, et al., 2023). The exact values depend on which manipulation types are held out and which target dataset is used, but the table illustrates a broader point: when the evaluation distribution changes, performance is no longer near the upper limit suggested by familiar in-domain benchmarks. The generalisation problem is therefore observable even before introducing adversarial attacks.

#### 3.2.3 Internet-sourced deepfakes as a real-world proxy

WildDeepfake makes the generalisation problem more concrete by changing where the fake videos come from. Instead of generating all manipulations inside one controlled research pipeline, the dataset contains 7,314 face sequences extracted from 707 deepfake videos collected from the internet (Zi et al., 2020). This changes several variables at once: identities, scenes, generation tools, video processing, editing history, resolution, and the unknown choices made by creators before uploading content.

Existing baseline detectors show substantial performance reductions on WildDeepfake compared with controlled datasets (Zi et al., 2020). The significance of this finding is methodological as well as technical. Internet-collected data are not a perfect model of every deployment environment, but they represent a stronger test of external validity because the detector cannot rely on a single research team's generation and preprocessing pipeline. WildDeepfake therefore supports the operational definition of real-world conditions used in this paper: a condition becomes more realistic when the detector faces sources and transformations that were not tightly controlled during model development.

This evidence also explains why high laboratory accuracy can coexist with practical uncertainty. A detector can genuinely be excellent at distinguishing the fake examples present in its benchmark while still being unreliable for content produced by different tools or processed through different online platforms. The two statements are not contradictory; they refer to different distributions.

#### 3.2.4 Improvements from generalisation-focused methods

The fact that cross-domain performance is weaker does not mean that progress is absent. SBI shows that altering training-data generation can improve performance on external datasets. It exceeds its baseline by 4.90 percentage points on DFDC and 11.78 percentage points on DFDCP in the reported cross-dataset evaluation (Shiohara & Yamasaki, 2022). These gains are important because they occur where existing methods suffer from domain gap rather than only on the dataset used to create the training examples.

UCF likewise reports superior generalisation to contemporary methods by isolating common forgery features (Yan, Zhang, Fan, et al., 2023). Taken together, SBI and UCF demonstrate that the generalisation gap is not fixed: detector design can reduce it. However, neither paper supports the stronger claim that the gap has been eliminated. Their methods are still evaluated on a finite set of datasets and manipulation families. A future generator may differ from all of them. The correct interpretation is therefore that generalisation can be improved through targeted design, while remaining a separate property that must be measured explicitly.

#### 3.2.5 Compression as evidence that accuracy is condition-dependent

FaceForensics++ directly illustrates how the same underlying content becomes harder to classify when media quality changes. The benchmark evaluates raw and compressed material and reports that stronger compression reduces the information available to the detector (Rössler et al., 2019). Its supplementary manipulation-classification results, for example, decrease from 99.03% on raw data to 95.42% under high-quality compression and 80.49% under low-quality compression. These values concern classification of the manipulation method rather than the binary deepfake-detection score, so they are not used here as a direct detector accuracy comparison. They nevertheless provide quantitative evidence that compression alters the forensic signal on which deepfake analysis depends.

This distinction matters for real-world use because media are routinely recompressed when uploaded, forwarded, edited, or stored. A detector validated only on high-quality source files may therefore face a different evidence distribution when analysing social-media video or messaging-app content. Compression is not an adversarial attack in the ordinary case; it is a normal part of media handling. Robustness to it is consequently part of baseline deployment reliability rather than an optional security feature.

#### 3.2.6 Audio performance under broader challenge conditions

The contrast between AASIST and ASVspoof 5 shows the same benchmark-to-deployment transition in audio. AASIST's 0.83% EER on ASVspoof 2019 LA demonstrates strong separation under a defined set of logical-access spoofing attacks (Jung et al., 2022). ASVspoof 5 deliberately increases the diversity of the problem by using crowdsourced speech from many more speakers and acoustic conditions, modern text-to-speech and voice-conversion systems, codecs, and adversarial attacks (Wang et al., 2024). The challenge paper reports that these attacks significantly compromise baseline systems, although submitted systems obtain substantial improvements.

The audio evidence is especially useful because it prevents the reliability analysis from becoming a purely face-manipulation argument. The underlying pattern is modality-independent: models can learn highly discriminative artefacts on known data, but performance must be reassessed when the generator, recording environment, speaker distribution, or transmission channel changes. For audio, codecs and acoustic conditions play a role analogous to image/video compression and acquisition shift.

#### 3.2.7 Why one accuracy percentage would be misleading

Table 2 summarises representative evidence used for SQ2. The metric column is intentionally included because a number has meaning only together with its metric and test condition. A low EER in audio is not numerically comparable with a visual AUC or accuracy value; even two visual AUC values can be misleading if they come from different train/test protocols.

**Table 2. Representative performance and generalisation evidence**

| Source | Modality | Evaluation condition | Metric / observation | Reliability implication |
|---|---|---|---|---|
| Rössler et al. (2019) | Image/video | Controlled benchmark with compression | Learned detectors remain strong; compression increases difficulty | High in-domain capability does not remove processing sensitivity |
| Jung et al. (2022) | Audio | ASVspoof 2019 LA | 0.83% EER | Very strong in-domain anti-spoofing performance |
| Zi et al. (2020) | Video | Internet-sourced WildDeepfake | Existing baselines decline substantially | External data distribution is materially harder |
| Shiohara & Yamasaki (2022) | Image/video | Cross-dataset DFDC / DFDCP | +4.90 pp / +11.78 pp over baseline | Generalisation can be improved by training-data design |
| Yan, Zhang, Fan, et al. (2023) | Image/video | Cross-dataset / held-out manipulation | Reported average AUC: Xception 0.683; UCF (Xception) 0.852 | Generalisation-focused representation learning improves transfer |
| Wang et al. (2024) | Audio | Crowdsourced, codec and adversarial conditions | Baselines significantly compromised | Broader attack and channel diversity changes performance |
| Nguyen-Le et al. (2026) | Image/video/audio | Unified OOD evaluation | Approx. 10-15% OOD degradation in summarised scenarios | Generalisation gap persists across modalities |

SQ2 is therefore answered conditionally. Current detectors can be extremely accurate under controlled and familiar conditions, but there is no defensible universal accuracy value for real-world media. The strongest pattern across the passive-detection evidence base is not that all systems fail, but that the variance between in-domain and shifted conditions is itself a defining property of current detector reliability.