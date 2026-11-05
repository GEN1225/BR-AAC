# BR-AAC research data

This repository provides data supporting the paper Background-relative surface learning with anchored appearance correction for industrial anomaly detection, together with its core training traces.

## Contents

- research_data/: manuscript table snapshots, source mappings, evaluation annotations and readable score tables.
- reproducibility/: saved prediction, role, calibration and transfer data in CSV, JSON and NPZ formats.
- results/training_records/: two Real-IAD surface traces, two Real-IAD appearance continuation traces and two PD-REAL training traces, for seeds 20261017 and 20261018.
- results/core_records/ and results/paper_evidence/: source records for the reported tables, controls, effects and example diagnostics.
- docs/DATA.md: dataset providers and role definitions.

The paper and supplement define supervision, statistical units and metric aggregation. Results include the reported comparisons and their measured effects. NPZ files can be read with NumPy using allow_pickle=False. JSON and CSV files retain recorded precision and identifiers. FILE_MANIFEST.json lists file sizes and SHA-256 hashes.

Large source datasets are obtained from their providers. The current branch distributes data and core training logs. Implementation code, model weights and configuration snapshots are retained separately by the authors.
