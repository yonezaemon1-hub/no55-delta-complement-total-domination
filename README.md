# No.55 — Exact Total-Domination Embeddings and Computational Hardness in δ-Complement Graphs

**Ryutaro Yonezu — Independent Researcher**  
Version **v1.0** · Published **5 November 2026** · **Preprint**

**All rights reserved. Not human peer-reviewed. Novelty: INCONCLUSIVE. Independent AI audit: PASS within the audited scope (user-provided audit reports).**

## Paper and reproducibility files

- [Paper PDF — GitHub Release v1.0](https://github.com/yonezaemon1-hub/no55-delta-complement-total-domination/releases/download/v1.0/No55_v1.0_PREPRINT_20261105.pdf)
- [Reproducibility ZIP — GitHub Release v1.0](https://github.com/yonezaemon1-hub/no55-delta-complement-total-domination/releases/download/v1.0/No55_v1.0_REPRODUCIBILITY_20261105.zip)
- [Zenodo preprint record](https://zenodo.org/records/23971752)
- **DOI:** [10.5281/zenodo.23971752](https://doi.org/10.5281/zenodo.23971752)

The manuscript sources, frozen code and evidence, original audit-stage archives, original Windows transcript, editorial diff and current publication-status notes are **inside the reproducibility ZIP**. Extract it to access those materials.

## Scope

For every isolate-free finite simple graph Q with m >= 2 vertices, the paper gives a polynomial-time construction F satisfying:

- gamma_t(F(Q)) = 3m;
- gamma_t(F(Q)_delta) = 2m + gamma_t(Q);
- k(F(Q)) = m + 1, where k counts distinct original vertex degrees.

The construction preserves bipartiteness and trees. A direct Set Cover reduction proves NP-completeness for total domination in the δ-complement of a **bipartite input** graph. The resulting δ-complement need not be bipartite.

A tree family has unbounded excess over the separate auxiliary bound 2k. **Chen's original total-domination sum conjecture is neither proved nor refuted in this work.**

## Reproduction

Extract the reproducibility ZIP and make a disposable copy of its `frozen_v0.2/` directory. Run the following from that copy, using Python 3.10+ with locally available NumPy, SciPy (including `scipy.optimize.milp`) and NetworkX:

```text
python -B code/verify_no55.py --milp --output sample_recheck.json
python -B code/audit_atlas.py
```

The Atlas script writes its evidence file, which is why a disposable working copy is required.

## Audit and Windows provenance

The independent mathematical audit and the v0.2 documentation-only differential-audit PASS are **user-provided results**, limited to the audited scope. This publication does not constitute a new independent mathematical audit or human peer review. References remain PARTIAL; unavailable original full texts are not claimed to have been inspected.

The user-supplied original `windows/No55_WINDOWS_LOG.txt` records a **v0.1 source-package** run on 5 November 2026 at 14:11 JST with the separate `No55_Run_Windows_v012.ps1` hotfix:

- Windows 10 / PowerShell 5.1 / Python 3.10.11;
- NumPy 2.2.6 / SciPy 1.15.3 / NetworkX 3.4.2;
- 16 sample MILP, 33 Atlas, 40 Set Cover and 11 composed F(B) cases PASS;
- the original v0.1 ZIP SHA256 identical before and after execution.

**This is not Windows execution of v0.2 or v1.0.** The hotfix is distinct from the frozen `run_windows.ps1`. Separately generated Windows result JSON files were not supplied and are not claimed to be included.

Historical HOLD and NOT DONE labels in `frozen_v0.2/` remain archival snapshots. The public manuscript is the primary public proof; `PUBLICATION_STATUS_20261105.md` inside the ZIP explains current authorization and attribution. The seven frozen proof/code/evidence/script files remain byte-identical to the audited source.

## SHA256 of the fixed public files

```text
7a455ac2dccc74fc9c6ae00a893834eabeb9fc256b016910ca75f344b6775dee  No55_v1.0_PREPRINT_20261105.pdf
4216c450f60c768f3d8ff6b0b10a17364493d3e2a1d7625edcf788943153ad20  No55_v1.0_REPRODUCIBILITY_20261105.zip
```

All four public downloads (PDF and ZIP from GitHub Release and Zenodo) were directly compared with the fixed originals on 5 November 2026: SHA256, sizes and bytes matched in all four cases.

## Rights

Copyright (c) 2026 Ryutaro Yonezu. **All rights reserved.** See [LICENSE](LICENSE). Public availability does not grant an additional reuse license. Third-party works retain their respective rights.

This repository-level README and LICENSE were added after the v1.0 release as publication metadata. The released PDF, reproducibility ZIP, v1.0 tag and Zenodo deposit are unchanged.
