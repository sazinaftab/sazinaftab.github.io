---
title: "Project 1: Waveguide Dispersion Analysis: TE0 Mode using FDE Solver"
collection: portfolio
permalink: /portfolio/project-1
date: 2026-06-29
---

## Executive Summary
An optical waveguide structure was modeled and analyzed using the Ansys Lumerical FDE (Finite-Difference Eigenmode) solver. The primary objective was to characterize the mode confinement and determine key modal parameters of the fundamental Transverse Electric (TE0) mode. A frequency sweep was performed across the C-band (1.55 um to 1.56 um), validating the design's suitability for low-loss, wideband integrated photonic applications.

## Simulation Setup & Optimization
* **Solver:** Ansys Lumerical FDE Solver
* **Boundary Conditions:** Perfectly Matched Layers (PML) to minimize reflections and ensure accurate mode profile simulation.
* **Mesh Settings:** Fine mesh override across the core region (0.01 um x 0.01 um) for high accuracy.
* **Convergence Optimization:** Resolved initial non-convergence by systematically expanding the simulation domain, allowing the evanescent field to decay properly and ensuring stable calculation baselines.

## Key Results (C-Band Analysis)
* **Effective Index (n_eff):** Characterized at an operating wavelength of 1.55 um, yielding an effective index of **2.44359**, confirming strong optical confinement within the waveguide core.
* **Dispersion Parameter (D):** Exhibits a positive dispersion parameter ranging from approximately 530.5 to 551.2 ps/nm/km ** across the C-band.
* **Modal Response:** Demonstrates a stable, predictable linear response for both group index (n_g) and group velocity (v_g) across the 1.55um to 1.56 um range (10 discrete points).

## Conclusion
The broadband sweep successfully validates strong light-matter interaction and confirms the design's suitability for wideband optical modulators or sensors. Future focus will be on the influence of geometric variations on mode stability.
