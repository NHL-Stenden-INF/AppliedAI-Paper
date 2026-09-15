# Sources Index

This is the central source register. School/project sources define the assignment and assessment requirements; the academic sources below form the evidence base for the deepfake-detection study.

| ID | Source | Type | Author / Organisation | Year | Purpose | Reliability | Used for | Status |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SRC-S01 | `APPENDIX 9 ASSESSMENT RESEARCH PAPER.pdf` | School / Assessment | NHL Stenden University of Applied Sciences, Tech & Design | 2026 | Direct research-paper assessment form and form-aspects gate | **Authoritative for direct paper assessment** | Requirements, rubric, structure, QA | Available / Rechecked |
| SRC-S02 | `APPLIED AI MODULE BOOK V1.pdf` | School / Module book | Development team / NHL Stenden Applied AI module | 2026 | Assignment process, Go/no-go role, learning outcomes, portfolio evidence and schedule | **Authoritative for assignment/module context** | Assignment, process, learning outcomes, assessment context | Available / Rechecked |
| SRC-P01 | `Research paper Subject.xlsx` | Project / Proposal record | Unknown | Unknown | Current pair, topic, title, MRQ and three SQs | Supporting only | Research-question and scope planning | Available / Rechecked |
| SRC-A001 | *Deepfake detection across image, video, and audio: a comprehensive survey with empirical evaluation of generalization and robustness* | Academic / Peer-reviewed survey + empirical evaluation | Nguyen-Le, Tran, Nguyen, & Le-Khac | 2026 | Current cross-modality taxonomy; empirical generalisation and robustness evidence | **High** — peer-reviewed, recent, broad empirical comparison; survey-level limitations remain | SQ1, SQ2, SQ3, MRQ | Included |
| SRC-A002 | *DeepfakeBench: A Comprehensive Benchmark of Deepfake Detection* | Academic / Benchmark | Yan, Zhang, Yuan, Lyu, & Wu | 2023 | Standardised comparison of visual deepfake detectors, datasets, metrics and protocols | **High** — peer-reviewed benchmark with reproducible evaluation framework | SQ1, SQ2, methodology context | Included |
| SRC-A003 | *FaceForensics++: Learning to Detect Manipulated Facial Images* | Academic / Primary empirical | Rössler, Cozzolino, Verdoliva, Rieß, Thies, & Nießner | 2019 | Foundational visual benchmark; compression and manipulation evidence | **High / foundational** — peer-reviewed, large benchmark; older but directly relevant to compression | SQ1, SQ2, SQ3 | Included |
| SRC-A004 | *WildDeepfake: A Challenging Real-World Dataset for Deepfake Detection* | Academic / Dataset + empirical evaluation | Zi, Chang, Chen, Ma, & Jiang | 2020 | Internet-sourced real-world visual dataset and performance degradation evidence | **High** — peer-reviewed and directly aligned with real-world generalisation | SQ2, SQ3 | Included |
| SRC-A005 | *Detecting Deepfakes with Self-Blended Images* | Academic / Primary empirical | Shiohara & Yamasaki | 2022 | Cross-dataset/generalisation method and comparative evidence | **High** — peer-reviewed CVPR study with cross-dataset evaluation | SQ1, SQ2, SQ3 | Included |
| SRC-A006 | *UCF: Uncovering Common Features for Generalizable Deepfake Detection* | Academic / Primary empirical | Yan, Zhang, Fan, & Wu | 2023 | Generalisable feature learning for unseen manipulations | **High** — peer-reviewed ICCV study focused directly on generalisation | SQ1, SQ2, SQ3 | Included |
| SRC-A007 | *Evading DeepFake Detectors via Adversarial Statistical Consistency* | Academic / Primary empirical | Hou, Guo, Huang, Xie, Ma, & Zhao | 2023 | Deliberate evasion against multiple deepfake detectors | **High** — peer-reviewed CVPR robustness study with white-box/black-box evaluation | SQ3, MRQ | Included |
| SRC-A008 | *ASVspoof 5: Crowdsourced Speech Data, Deepfakes, and Adversarial Attacks at Scale* | Academic / Benchmark + empirical | Wang et al. | 2024 | Audio deepfake evaluation under diverse conditions, codecs and adversarial attacks | **High** — current community benchmark with direct audio robustness evidence | SQ1, SQ2, SQ3 | Included |
| SRC-A009 | *AASIST: Audio Anti-Spoofing Using Integrated Spectro-Temporal Graph Attention Networks* | Academic / Primary empirical | Jung et al. | 2022 | Representative learned audio anti-spoofing architecture and benchmark performance | **High** — peer-reviewed ICASSP study; strong in-domain evidence but limited deployment generalisation claim | SQ1, SQ2 | Included |
| SRC-A010 | *DeepFake video detection: Insights into model generalisation — A systematic review* | Academic / Systematic review | Ramanaharan, Guruge, & Agbinya | 2025 | Synthesis of video detector generalisation limitations and research patterns | **High for synthesis** — recent systematic review; performance claims treated as review-level evidence | SQ2, SQ3, MRQ | Included |
| SRC-A011 | *The Stable Signature: Rooting Watermarks in Latent Diffusion Models* | Academic / Primary empirical | Fernandez, Couairon, Jégou, Douze, & Furon | 2023 | Active invisible watermarking for diffusion-generated images; robustness and provenance detection | **High** — peer-reviewed ICCV study with empirical robustness testing and explicit false-positive control | Watermarking, SQ1 context, MRQ | Included |
| SRC-A012 | *Invisible Image Watermarks Are Provably Removable Using Generative AI* | Academic / Primary empirical + theoretical | Zhao et al. | 2024 | Limits of invisible pixel-level watermarking under regeneration attacks | **High** — peer-reviewed NeurIPS study with formal analysis and multi-scheme empirical evaluation | Watermarking limitations, SQ3 context, MRQ | Included |

## Source-Use Rules

- Every important claim is linked to one or more source IDs and Evidence Matrix rows.
- Evidence directness and source quality are assessed separately.
- Review papers establish field structure and synthesis; major performance claims are preferably supported by primary empirical evidence.
- Metrics are not compared as isolated percentages when datasets, modalities, test conditions or protocols differ.
- Foundational older work is retained only when it directly supports a current reliability factor that remains relevant.
- Watermarking evidence is analysed separately from passive forensic detection because it assumes participation by the generator or content pipeline.
- Absence of a watermark is not treated as evidence that content is authentic.
- Missing metadata is recorded as `Unknown`; author, year, DOI, publisher or URL must never be invented.

## Source Categories

School, Academic, Professional, Project, Internal, Government, Standard, Dataset, Interview, Observation, Technical Documentation, Other.

## Reliability Principle

A source is not `strong` merely because it is relevant. Authority/publication context, currency, method/evidence basis, transparency, directness, limitations and generalisation risk are considered independently. For watermarking specifically, robustness to benign transformations and resistance to deliberate removal are treated as separate properties.