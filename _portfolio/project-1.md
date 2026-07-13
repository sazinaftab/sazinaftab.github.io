---
title: "Project 1: Waveguide Dispersion Analysis TE0 Mode using FDE Solver"
collection: portfolio
permalink: /portfolio/project-1
date: 2026-06-29
---

## Executive Summary
In this study, an optical waveguide structure was modeled and analyzed using the Ansys Lumerical FDE (Finite-Difference Eigenmode) solver. The primary objective was to characterize the mode confinement and determine the effective index, group index, group velocity, and dispersion parameter of the fundamental TE mode. A frequency sweep was performed across the C-band (1.55 µm to 1.56 µm), validating the design's suitability for low-loss, wideband integrated photonic applications.

## Simulation Setup
* **Solver Used:** FDE (Finite-Difference Eigenmode) Solver.
* **Boundary Conditions:** Perfectly Matched Layers (PML) were applied at the boundaries to minimize reflections and ensure accurate simulation of the mode profile.
* **Mesh Settings:** To ensure high accuracy and convergence of the mode profile, a fine mesh override was applied across the core region with a cell size of 0.01um x 0.01um.
* **Challenges & Optimization:** Initially, the simulation failed to converge due to an undersized simulation domain. This was resolved by systematically expanding the simulation area to allow the evanescent field to decay properly, achieving a stable calculation.

![Fig 1](/images/project-1/Fig1_Large_Area.PNG)
*Fig 1 : Computational region is sufficiently large to prevent artificial confinement effects.*

![Fig 2](/images/project-1/Fig2_Small_Area.PNG)
*Fig 2 : Computational region is small results in confinement problem.*

## Broad-band Analysis (Frequency Sweep)
To understand the wideband characteristics, a frequency sweep was performed between **1.55 um - 1.56 um**, collecting data at **10 discrete points**.

![Fig 3](/images/project-1/neff_VS%20wavelength.png)
*Fig 3 : neff vs Wavelength*

![Fig 5](/images/project-1/Group_index_VS%20wavelength.png)
*Fig 5 : Group index vs Wavelength*

![Fig 4](/images/project-1/Group_Velocity_VS%20wavelength.png)
*Fig 4 : Group Velocity vs Wavelength*

![Fig 6](/images/project-1/dispersion_vs_wavelength.png)
*Fig 6 : Dispersion vs Wavelength*

## Key Results
* **Effective Index (n_eff) :** The fundamental TE0 mode was characterized at an operating wavelength of 1.55 um, yielding an effective index of **2.44359**. This high refractive index value confirms **strong optical confinement** within the waveguide core.
* **Dispersion Characteristics:** As shown in Fig 6, the waveguide exhibits a positive dispersion parameter (D) ranging from approximately **530.5 to 551.2 ps/nm/km** across the C-band. This significant dispersion profile is a critical design metric for characterizing signal pulse broadening and dispersion-engineered photonic applications.
* **Analysis:** As illustrated in Fig 4 and Fig 5, the waveguide exhibits a stable and predictable **linear response** for both group index and group velocity across the 1.55 um to 1.56 um range. The gradual change in these parameters confirms the waveguide's suitability for wideband light management, maintaining consistent signal propagation characteristics across the entire C-band.

## Analysis & Conclusion
The simulation successfully characterizes the waveguide properties. The optimized setup resolved initial convergence issues, and the broadband analysis validates strong light-matter interaction. The dispersion profile confirms the design's suitability for applications such as wideband optical modulators or sensors. Future work will focus on investigating the influence of geometric variations on mode stability.

> 📁 **Download Lumerical File:** [Waveguide_Dispersion_Analysis_TE0_Mode_28_June_2026.lms](/files/project-1/Waveguide_Dispersion_Analysis_TE0_Mode_28_June_2026.lms)
