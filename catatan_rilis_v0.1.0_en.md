Accompanies manuscript version 6, *Improved Hour-Ahead Solar Irradiance Forecasts in Indonesia Based on Himawari-8/9 Cloud Retrievals*. Every number in that manuscript and its Online Resource 1 was recomputed from database version 6.10 and can be traced to a script and a result file in this repository.

**This is a pre-submission release (v0.1.0).** The manuscript has not yet been submitted; the version of record will be issued as v1.0.0 after acceptance.

- **Layout:**
  - `paper_v2_clpbanten/`: helpers, reused stage scripts, database stages 93–113, supporting analyses in stage 114;
  - `Manuskrip_versi6/`: training protocol, analysis, results;
  - `training mirip/`, `data_versions/`, `figures/`.
- **Data:** database 6.10. Clear-sky irradiance averaged per slot. Himawari-8/9 CLP re-extracted in station-centred boxes, with the box retrieval coverage. AWS meteorology checked against SYNOP and rebuilt causally. SYNOP reports kept for 50 min.
- **Methods:**
  - 44 predictors;
  - eight architectures × five seeds under one protocol;
  - box statistics rebuilt and verified against Himawari chips;
  - supporting analyses recomputed on version 6.10;
  - a checker that recomputes every number quoted in the manuscript.
- **Not distributed:** station observations, database and model frames, prediction archives, trained models, extraction archives, manuscript files.

See `CHANGELOG.md` for details.
