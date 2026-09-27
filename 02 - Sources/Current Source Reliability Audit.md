# Current Source Reliability Audit

## Scope

This file evaluates the **existing 15 references only**. No source was added, removed or replaced.

The audit uses the criteria documented in `01 - Research/Search Strategy and Source Selection Audit.md`: relevance, date, publication type, peer review/authority, publisher or institution, method transparency, dataset/metric context, traceability, directness and limitations.

## Overall source-base profile

- **15 total sources**
- Publication years: **2019-2026**
- Strong representation from established research venues/publishers: IEEE/CVF, IEEE, ACM, Springer Nature, Elsevier and NeurIPS
- **1 official European Commission source**, used only for legal context
- **1 arXiv preprint (DFDC)**, explicitly labelled and used only for dataset/challenge information
- Mix of primary empirical studies, benchmark/dataset papers and review/systematic-review work
- All 15 entries have an official/stable URL or DOI in the reference list

The mix is appropriate for the paper because no single source type can answer all three subquestions: technique mapping benefits from reviews, performance claims need empirical/benchmark evidence, and Article 50 requires an official institutional source.

## Source-by-source audit

| ID | Source | Year | Type / venue / institution | Role in paper | Why acceptable | Main limitation / boundary |
| --- | --- | ---: | --- | --- | --- | --- |
| SRC-A001 | Chandra et al., *Deepfake-Eval-2024* | 2026 | IEEE/CVF CVPR Workshops; benchmark study | Real-world/in-the-wild performance | Recent multimodal empirical benchmark with explicit data and test conditions; official CVF proceedings page | One benchmark and 2024-circulated content; not automatically representative of future generators |
| SRC-A002 | Dolhansky et al., *DFDC Dataset* | 2020 | arXiv preprint / dataset paper | DFDC size, composition and challenge context | Primary description of the dataset/challenge and stable arXiv identifier | Preprint; therefore not used as the main basis for broad reliability claims |
| SRC-A003 | European Commission, Article 50 transparency information | 2026 | Official EU institution | Legal/regulatory context | Primary institutional source for EU AI Act implementation context | Not a technical deepfake-detection study; used only for legal context |
| SRC-A004 | Hou et al., adversarial statistical consistency | 2023 | IEEE/CVF CVPR | Deliberate evasion/adversarial attack evidence | Peer-reviewed empirical conference research; attack setup and multiple detectors/datasets are described | Specific attack design and evaluated models; cannot represent every adversarial threat |
| SRC-A005 | Jung et al., AASIST | 2022 | IEEE ICASSP | Audio detection method and baseline performance | Peer-reviewed technical conference paper with explicit model/evaluation setup and DOI | Strong benchmark result does not by itself prove wider deployment performance |
| SRC-A006 | Li et al., Celeb-DF | 2020 | IEEE/CVF CVPR | Cross-dataset/challenging dataset evidence | Peer-reviewed dataset/forensics paper; official CVF proceedings | Focused on visual face deepfakes; does not cover audio |
| SRC-A007 | Nguyen-Le et al. | 2026 | *Artificial Intelligence Review*, Springer Nature | Cross-modality technique map, generalisation and robustness evidence | Recent peer-reviewed survey plus substantial empirical evaluation across image/video/audio | Review and experiments still depend on selected datasets/methods; not all real-world conditions are covered |
| SRC-A008 | Ramanaharan et al. | 2025 | *Data and Information Management*, Elsevier/ScienceDirect | Systematic-review evidence on generalisation | Recent systematic review directly focused on model generalisation | Review conclusions depend on the included-study set and mainly concern video |
| SRC-A009 | Rössler et al., FaceForensics++ | 2019 | IEEE/CVF ICCV | Benchmark/compression background | Foundational peer-reviewed benchmark with explicit manipulation/compression setup | Older benchmark; useful as baseline/foundation, not proof of 2026 practical performance |
| SRC-A010 | T. Wang et al. | 2024 | *ACM Computing Surveys* | Reliability framework, technique families and robustness | Peer-reviewed ACM survey focused specifically on transferability, interpretability and robustness | Survey synthesis; important performance claims still need primary empirical context |
| SRC-A011 | X. Wang et al., ASVspoof 5 | 2026 | *Computer Speech & Language*, Elsevier | Current audio robustness/generalisation context | Peer-reviewed research article; diverse speakers, codecs, synthesis algorithms and adversarial attacks | Audio-specific and challenge-oriented |
| SRC-A012 | Yan et al., DeepfakeBench | 2023 | NeurIPS Datasets & Benchmarks | Evaluation-pipeline comparability | Peer-reviewed benchmark work explicitly addressing standardised data processing, protocols and metrics | Benchmark framework; does not itself establish all real-world deployment performance |
| SRC-A013 | Yermakov et al. | 2026 | IEEE/CVF WACV | Cross-benchmark generalisation | Recent peer-reviewed empirical evaluation across many benchmarks with official proceedings/DOI | Academic benchmark coverage is broad, but differs from randomly circulating online content |
| SRC-A014 | Zhao et al. | 2024 | NeurIPS | Watermark-removal robustness | Peer-reviewed theoretical + empirical research in a major ML venue; official proceedings/DOI | Concerns specific pixel-level watermark settings; not all provenance methods |
| SRC-A015 | Zi et al., WildDeepfake | 2020 | ACM Multimedia | In-the-wild video evidence | Peer-reviewed ACM conference dataset based on internet-collected deepfakes | Older and video-specific; sample reflects the web content available at that time |

## Claim-role controls

The source audit does **not** treat every accepted source as equally suitable for every statement.

Examples:

- The European Commission is authoritative for Article 50 context but is not used to claim detector accuracy.
- The DFDC preprint is acceptable for DFDC dataset/challenge facts but is not treated as equivalent to a peer-reviewed current reliability benchmark.
- FaceForensics++ is important foundational benchmark evidence, but its age and controlled setup are explicitly part of the reason the paper compares it with newer in-the-wild datasets.
- Review papers support the taxonomy and broader pattern, while direct performance values remain tied to their original dataset, metric and test condition.

## Date and currency check

The included sources span 2019-2026. Older sources were retained only where they provide foundational datasets/benchmarks or historically important baselines. Current sources from 2025-2026 are included for generalisation, multimodal detection, audio attacks and in-the-wild performance.

This combination is preferable to using only the newest papers: the research question specifically compares how performance changes between older controlled benchmarks and newer/less controlled conditions.

## Publisher / institution coverage

The selected set includes material from:

- IEEE/CVF and IEEE;
- ACM;
- Springer Nature;
- Elsevier;
- NeurIPS proceedings;
- European Commission;
- arXiv for the explicitly labelled DFDC preprint.

No vendor blog or general news article is used as the primary basis for a technical performance claim.

## Reliability conclusion

The current 15-source set is **defensible for the roles assigned to the sources**. Its strongest feature is that technical conclusions are supported by established academic venues and are interpreted together with dataset, metric and test-condition context.

The main methodological weakness remains the incomplete original search log, not the traceability of the final 15 references. That limitation is now stated openly in the paper and documented in the search audit.
