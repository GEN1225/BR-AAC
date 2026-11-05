# Small research data

This directory provides small paper-related derived score tables. It contains no source images, depth maps, point clouds or large feature tensors. Existing compact role/calibration/transfer data remain in reproducibility/ to preserve working script paths; CATALOG.json indexes both locations and records hashes.

| File | Rows | Contents |
|---|---:|---|
| matched_external_scores.csv | 12,532 | 26 matched comparison endpoints on V350 and HOLD132 |
| pdreal_fixed_scores.csv | 17,424 | Three seed/ensemble recipes, four combinations and three branches on V164/HOLD320 |
| score_correlation_samples.csv | 132 | Normal-reference sample/group identities and four saved branch-score columns G0/G1/A0/A1 |
| evaluation_annotations.json | 514 | Real-IAD350 and PD-REAL164 public category, label and defect-type identities |
| paper_tables.json | 19 tables | Current English TeX table blocks, table identifiers and authoritative source hashes |
| paper_table_sources.json | 15 result tables | Designated source artifacts for numerical table transcription checks |

The two endpoint CSVs contain dataset, endpoint, role, sample_key, category, label and the saved logit. Values use a float64-safe decimal representation and were roundtrip-checked against every source NPZ element. Row counts count predictions, not independent observations. Endpoint names preserve experiment identities; lines across endpoints can refer to the same observation. These are custom development protocols described in the paper, not provider official leaderboard splits.

## Large external datasets

- Real-IAD D3: https://huggingface.co/datasets/Real-IAD/Real-IAD_D3 . Access conditions apply; exact raw members/hashes are listed in configs/realiad_*_assets.json.
- PD-REAL: https://github.com/Andy-cs008/PD-REAL . The provider links the dataset archive at https://drive.google.com/file/d/1EBapy9BGnwmZJ9Rxh0uTF-Xii9FU0YCG/view . Exact used members/hashes are in configs/pdreal_all2020_assets.json.
- Eyecandies: https://github.com/eyecan-ai/eyecandies . The small S9 prediction file is indexed in CATALOG.json.
- SiM3D: https://huggingface.co/datasets/arcanoXIII/SiM3D . Provider access conditions apply; the small S10 state-score file is indexed in CATALOG.json.

The provider repository's software license is not assumed to define redistribution rights for every dataset archive or derived asset. Source distribution conditions apply independently. No new dataset license is asserted here. Raw copies are obtained from providers; backbone access and hashes are documented in docs/BACKBONE.md. Public release permissions for derived metadata/scores still require final review.

The correlation CSV retains the G0/G1/A0/A1 field names from the archived branch-score diagnostic; see its original result under results/paper_evidence. The annotation file is a label/type lookup, not a defect-mask payload. The paper table snapshots are transcriptions; designated source records and replay commands provide the corresponding scientific evidence.

## Multi-dataset tables

multidataset/RESULT_TABLES.md presents the expanded detection and encoding tables. The collection includes 37 detection rows, four cost rows, 14 paired effects, observation identities, 180 timing measurements and DTD image/usage manifests. Protocols and provider links are in docs/MULTIDATASET_RESULTS.md.
