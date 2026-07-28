# phase_space_matcher

> **Non-Parametric Phase-Space Trajectory Matching & Verification Ledger**  
> *Local-First, Zero-Leakage Time-Series Falsification Engine*

---

## Overview

`phase_space_matcher` serves as the public, immutable proof ledger for empirical audits executed by our local-first geometric engine. 

Instead of relying on heavy parametric neural architectures or assuming signal stationarity, the engine reconstructs multi-dimensional phase-space manifolds from raw scalar time-series inputs. By evaluating structural trajectory geometry and orbital boundaries in real time, it identifies dynamic invariants without risk of distribution drift or model memorization.

---

## Empirical Audit Benchmark Summary

Every benchmark is evaluated against an exact **distribution-matched null model** (controlling for local variance and state persistence) under a strict zero-lookahead forward prediction harness.

| Domain Label | Audit File | Evaluated Steps | Geometry Accuracy | Matched-Null Accuracy | Predictive Edge ($\Delta$) | Receipt Link |
| :--- | :--- | :---: | :---: | :---: | :---: | :--- |
| `physical_systems/` | `hardware_ablation_run1`[cite: 2, 4] | 3,592[cite: 2, 4] | **83.96%**[cite: 2, 4] | **58.24%**[cite: 2, 4] | **+25.72%**[cite: 2, 4] | [Report](./physical_systems/) |
| `physical_systems/` | `hardware_ablation_run2`[cite: 3] | 3,592[cite: 3] | **86.02%**[cite: 3] | **56.38%**[cite: 3] | **+29.65%**[cite: 3] | [Report](./physical_systems/) |
| `physiological/` | `physionet_ecg_100` | 2,400 | **86.02%** | **56.74%** | **+29.29%** | [Report](./physiological/) |
| `industrial/` | `host_telemetry` | *Active Stream* | *In Progress* | *In Progress* | *Active Stream* | [Report](./industrial/) |

$$\Delta = \text{Accuracy}_{\text{Geometric}} - \text{Accuracy}_{\text{Matched Null}}$$

---

Repository Structure

```text
phase_space_matcher/
│
├── physical_systems/      # Hardware ablation & mechanical wear trajectory receipts
├── physiological/         # Biological & cardiac time-series audit receipts
├── industrial/            # Live computer telemetry & network metric receipts
│
└── README.md              # Public architecture, audit summary & research lineage


<img width="878" height="477" alt="image" src="https://github.com/user-attachments/assets/2d6a1f36-f190-4161-bcec-feb6f5d210de" />


Research Lineage
This public ledger represents the production output of a multi-year open/closed research lineage:

phase_space_matcher (This Repository) — Public attestation ledger, domain-tagged audit receipts, and verification reports.

phase_space_ — Initial phase-space mapping, delay-embedding primitives, and manifold feature extractors.

labrys & ibis-ledger — Telemetry streaming infrastructure, pipeline orchestration, and early state-tracking models.

Proprietary Core Engine — The un-tracked, local-first execution harness that processes raw streams, runs null-matched falsification tests, and generates signed receipt reports.

Security & Privacy Guarantee
100% Air-Gapped Execution: Audit harnesses run strictly on local hardware. Raw source telemetry or biological data never leaves the host environment.

Zero Code Exposure: Only verified text/markdown verdict receipts are published to this ledger. Core math algorithms and execution harnesses remain strictly private.
