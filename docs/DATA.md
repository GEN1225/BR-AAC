# Dataset sources and allocations

| Source | FIT | Normal reference | Supervision E | Calibration C | Evaluation V |
|---|---:|---:|---:|---:|---:|
| Real-IAD D3 | 468 | 132 | 90 | 63 | 350 |
| PD-REAL | 1279 | 320 | 147 | 110 | 164 |

reproducibility/role_sample_manifest.csv identifies the main allocations. Eye500, Source456 and SiM3D metadata accompany their respective saved-score NPZ files. Source456 is a separate three-category Real-IAD cohort. Eye results average three seed-specific category-macro metrics. SiM3D uses 35 states with 12 views each and identity-weighted category metrics.

Provider links:

- Real-IAD D3: https://huggingface.co/datasets/Real-IAD/Real-IAD_D3
- PD-REAL: https://github.com/Andy-cs008/PD-REAL
- Eyecandies: https://github.com/eyecan-ai/eyecandies
- SiM3D: https://huggingface.co/datasets/arcanoXIII/SiM3D

Provider distribution terms apply. Source records identify the reported method configurations and preserve their numerical outputs. Main and supplementary table blocks are in research_data/paper_tables.json.
