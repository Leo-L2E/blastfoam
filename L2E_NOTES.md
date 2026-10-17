# L2E notes: blastFoam in the XFE.rs project

This is a fork of [synthetik-technologies/blastfoam](https://github.com/synthetik-technologies/blastfoam), kept by Leo Laine (LL Engineering AB / L2E).

## Purpose
- **Theory reference** for the XFE.rs Phase 5b structured blast solver: flux schemes (HLLC, AUSM+, AUSM+up, Kurganov–Tadmor), MUSCL reconstruction, Runge–Kutta time integration, JWL and other EOS, afterburn models, and AMR.
- **Open oracle:** the Phase 5b gate cases are run here as an independent reference, next to the Autodyn 2019 SHIELD results:
  - Sod and Sedov
  - free-air TNT against Kingery–Bulmash
  - the Chalmers 1:5 urban case
  - SHIELD in 2D
- XFE.rs implements the methods from the published papers. If code is ever ported, it keeps its GPL-3.0-or-later notices. GPL-3.0 code may be combined with the AGPL-3.0 XFE.rs (GPLv3/AGPLv3 §13); this is to be confirmed by Jose.

## State when forked
| Branch | Upstream commit | Note |
|---|---|---|
| `master` | 4e6ee07a (2023-03-27, release 6.2.0) | OpenFOAM-9 |
| `develop` | 21cf05d1 (2026-03-17) | active development; `l2e-main` starts here |
| `v12` | 3f915a36 (2025-07-29) | port to a newer OpenFOAM |

## Changes in this fork
- `l2e-main`: this file only. The solver is unchanged.

Licence: GPL-3.0-or-later (see `COPYING`).
