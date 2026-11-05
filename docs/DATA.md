# Dataset sources and allocations

| Source | FIT | Normal reference | Supervision E | Calibration C | Evaluation V |
|---|---:|---:|---:|---:|---:|
| Real-IAD D3 | 468 | 132 | 90 | 63 | 350 |
| PD-REAL | 1279 | 320 | 147 | 110 | 164 |

reproducibility/role_sample_manifest.csv identifies the main allocations. Eye500, Source456 and SiM3D metadata accompany their respective saved-score NPZ files. Source456 is a separate three-category Real-IAD cohort. Eye results average three seed-specific category-macro metrics. SiM3D uses 35 states with 12 views each and identity-weighted category metrics.

## Data sources

| Dataset | Provider / access | Inputs and use |
|---|---|---|
| Real-IAD D³ | [Dataset](https://huggingface.co/datasets/Real-IAD/Real-IAD_D3) | Paired RGB and XYZ-derived surface information for detection and fusion experiments. |
| PD-REAL | [Project and data access](https://github.com/Andy-cs008/PD-REAL) | RGB and depth/XYZ observations of Play-Doh objects for detection and fusion comparisons. |
| Eyecandies | [Project and data access](https://github.com/eyecan-ai/eyecandies) | Synthetic RGB and geometric observations for transfer and appearance/geometry comparisons. |
| MVTec 3D-AD | [Dataset](https://www.mvtec.com/research-teaching/datasets/mvtec-3d-ad) | Paired RGB and 3D surface observations for context and normal-reference comparisons. |
| SiM3D | [Dataset](https://huggingface.co/datasets/arcanoXIII/SiM3D) | Multiview RGB and geometry for state-level transfer and probability-mapping comparisons. |
| 3D-ADAM | [Prepared subset](https://huggingface.co/datasets/pmchard/3D-ADAM_anomalib) · [Full dataset](https://huggingface.co/datasets/pmchard/3D-ADAM) | Additive-manufacturing observations for frozen surface transfer and input-adaptation analysis. |
| MulSen-AD | [Project](https://github.com/MapleBoat/MulSen-AD) · [Data](https://huggingface.co/datasets/orgjy314159/MulSen_AD) | RGB, infrared and point clouds for sensor-encoding measurements. |
| Describable Textures Dataset (DTD) | [Dataset](https://www.robots.ox.ac.uk/~vgg/data/dtd/) | Auxiliary texture images for local synthetic anomaly generation. |

These sources cover the datasets used across the study. The paper and supplement specify the configurations and results reported for each analysis. The repository contains the selected paper data and core training logs; source images, depth maps and point clouds are obtained from their providers under the corresponding distribution terms. DTD is an auxiliary training-texture source. Source456 and Real-IAD350 are evaluation cohorts within Real-IAD D³.

Provider distribution terms apply. Source records identify the reported method configurations and preserve their numerical outputs. Main and supplementary table blocks are in research_data/paper_tables.json.
