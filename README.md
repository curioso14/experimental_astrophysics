# Experimental Astrophysics Projects

A collection of observational and data analysis projects developed for the course AST0421 – Experimental Astrophysics at Pontificia Universidad Católica de Chile. Each project applies state-of-the-art astronomical tools and datasets to real scientific problems, from galaxy spectroscopy to protoplanetary disk interferometry.

Each PDF report includes the full analysis code alongside the written results.

**Course:** AST0421 – Astrofísica Experimental · Pontificia Universidad Católica de Chile  
**Instructor:** Prof. Ezequiel Treister  
**Stack:** Python · Astropy · MPDAF · SExtractor · CIGALE · CASA · Numpy · Matplotlib

---

## Projects

| # | Project | Topic | Instrument / Survey |
|---|---------|-------|-------------------|
| 1 | [Integral Field Spectroscopy of NGC 2992](#project-1--integral-field-spectroscopy-of-ngc-2992) | AGN ionization, emission line fitting, kinematics | VLT-MUSE |
| 2 | [Photometry of the Next Generation Fornax Survey](#project-2--photometry-of-the-next-generation-fornax-survey-ngfs) | Data reduction, source detection, globular clusters | VISTA/VIRCam |
| 3 | [SED Modeling of AGNs with CIGALE](#project-3--sed-modeling-of-agns-with-cigale) | Multi-wavelength fitting, stellar populations, AGN parameters | AHA Survey |
| 4 | [Interferometric Analysis of HD 163296 with MAPS](#project-4--interferometric-analysis-of-hd-163296-maps) | Protoplanetary disk structure, HCO+ emission, baseline analysis | ALMA/MAPS |

---

## Project 1 — Integral Field Spectroscopy of NGC 2992

**Tools:** VLT-MUSE · MPDAF · Gaussian fitting · BPT diagrams

Integral field spectroscopic observations of NGC 2992 (z ~ 0.00771) obtained with VLT-MUSE. Continuum subtraction and Gaussian fitting were performed for emission lines Hβ, [OIII], Hα, [NII], and [SII]. BPT diagrams revealed that the dominant ionization mechanism is AGN activity, while three small regions show star-formation-dominated ionization. Moment maps were constructed, showing rotation velocities of ±300 km/s, evidence of gravitational interaction with the Arp 245 system, and a maximum velocity dispersion of ~400 km/s — likely due to an outflow from the central region observed in the emission maps.

---

## Project 2 — Photometry of the Next Generation Fornax Survey (NGFS)

**Tools:** VISTA/VIRCam · THELI · SExtractor · 2MASS · SSP models

Data reduction, photometry, and analysis of imaging from the Next Generation Fornax Survey using VISTA/VIRCam. The pipeline included processing of darks and flats, global and individual weight maps, astrometric calibration using 2MASS as reference catalog, and sky subtraction with a zero-point of ZP=23.75. Source detection was performed with SExtractor and cross-matched against the K-band and ugi catalogs. A completeness parameter was defined to distinguish globular cluster populations in the color-color diagram. SSP models were overlaid to compare with the observed populations, concluding that globular clusters with metallicities of 0.004, 0.008, and 0.02 best match the data — indicating the presence of multiple stellar populations within the globular clusters.

---

## Project 3 — SED Modeling of AGNs with CIGALE

**Tools:** CIGALE · Pearson & Kendall correlation · AHA Survey

SED modeling for 19 AGNs using multi-wavelength data from the AHA Survey. CIGALE was used to fit spectral energy distributions, incorporating modules for star formation history, stellar population contributions, nebular emission, dust attenuation and emission, and AGN contribution. Models were iterated until the majority achieved χ²_red < 2.5. Recovered parameters include instantaneous SFR, age of the dominant stellar population, total stellar mass, color excess E(B-V), AGN X-ray and bolometric luminosity, and accretion power. Pearson and Kendall τ correlation indices were computed across all parameters, finding 5 correlations with |r| > 0.3. Key results: stellar population age shows a negative correlation with SFR and E(B-V); total stellar mass correlates positively with SFR and AGN X-ray luminosity; and a positive correlation between total AGN luminosity and accretion disk luminosity was identified.

---

## Project 4 — Interferometric Analysis of HD 163296 (MAPS)

**Tools:** ALMA · CASA · Moment maps · Baseline configuration analysis

Radio interferometric analysis of the protoplanetary disk HD 163296 using data from the MAPS project, comprising 80 observations across six antenna configurations to observe HCO+ emission. The effect of baseline configuration on the spatial representation of disk structure was characterized. Data were analyzed using CASA, with robust weighting values of -2.0, 0.5, and 2.0 tested; robust=2.0 was selected to prioritize resolution. Short and long baseline images revealed distinct interference patterns. Moment 0 and velocity maps provided quantitative spatial information, and the radial profile highlighted the near-absence of material near the nucleus and variations in the distribution toward the disk edge. Results underscore the importance of baseline configuration and robust parameter selection in interferometric data interpretation.

---

## Repository Structure

```
experimental-astrophysics/
├── README.md
├── project1_IFS_NGC2992.pdf
├── project2_photometry_NGFS.pdf
├── project3_SED_AGN_CIGALE.pdf
└── project4_interferometry_HD163296_MAPS.pdf
```

> Each PDF contains the full written report together with the analysis code used to produce the results.
