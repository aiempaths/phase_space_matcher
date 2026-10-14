# State Shape: PREREG_12 sealed result

**Sealed:** 9 Oct 2026, 3:09 PM MT, before any held-out data was scored.
**Manifest SHA-256:** `cdfb47280069b86ad4714aec5cf042e1dcda620f014d87c3605b5c292fcfbd1b`

48 MIT-BIH ECG records, 480 held-out slices, scored against per-record skill.

| Result | Value |
|---|---|
| Closeness (d_rel) vs per-record skill, rank correlation ρ | **−0.75** |
| Agreement (purity) vs per-record skill, rank correlation ρ | **+0.72** |
| Held-out slices | **480** across 48 records |

All pre-registered outcomes are reported. Both trust signals passed. A third test failed: combining two leads was not better than the best single lead. A fourth, expected to show no gain in prediction, showed none. State Shape gives a trust signal, not a forecast. Validated on ECG only so far.

Data: [MIT-BIH Arrhythmia Database](https://physionet.org/content/mitdb/1.0.0/) (PhysioNet).
