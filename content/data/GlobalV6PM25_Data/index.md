---
title: "Global Satellite-derived Monthly PM₂.₅ Total Mass (0.01x0.01) - V6.GL.02.04 (Selected as AGU Impactful Datasets)"
date: 2025-05-07
tags: ["Remote Sensing","Air Quality","Gloabl Daatsets","Deep Learning","Geophysical Constrains","Simulations"]
author: ["Siyuan Shen","Chi Li","Aaron van Donkelaar","Nathan A. Jacobs", "Chenguang Wang","Randall V. Martin"]
description: "This dataset contains global annual and monthly ground-level fine particulate matter ($\rm{PM_{2.5}}$) for 2000-2023 at around 1 km resolution."
summary: "This dataset contains global annual and monthly ground-level fine particulate matter ($\rm{PM_{2.5}}$) for 2000-2023 at around 1 km resolution."
cover:
    image: "data1.png"
    alt: "Figure title (preferably 1280x720 pixels)"
    relative: true
editPost:
    URL: "https://www.satpm.org/v6-gl-02-04"
    Text: "SatPM (ACAG Datasets)"
showToc: true
disableAnchoredHeadings: false

---

## Overview

We estimate annual and monthly ground-level fine particulate matter ($\rm{PM_{2.5}}$) for 2000-2019 by combining Aerosol Optical Depth (AOD) retrievals (Dark Target, Deep Blue, MAIAC) that make use of observations from numerous satellite-based NASA instruments (MODIS/Terra, MODIS/Aqua, MISR/Terra, SeaWiFS/SeaStar, VIIRS/SNPP, and VIIRS/NOAA20) with the GEOS-Chem chemical transport model, and subsequently calibrating to global ground-based observations using a residual Convolutional Neural Network (CNN), as detailed in the below reference for V6.GL.01. V6.GL.02.04 follows the methodology of V6.GL.01 but updates the ground-based observations used to calibrate the geophysical $\rm{PM_{2.5}}$ estimates for the entire time series, extends temporal coverage through 1998 – 2023, and includes retrievals from the SNPP VIIRS instrument. Also, previous versions were reported to contain abnormally low values in certain, rare circumstances. This limitation has been addressed in V6.GL.02.04 using a modified padding strategy and stronger geophysical constraints.

---

## View dataset

+ Annual and monthly mean $\rm{PM_{2.5}}$ [ug/m3] at 0.01° × 0.01°:
[https://wustl.box.com/v/ACAG-V6GL0204-CNNPM25](https://wustl.app.box.com/folder/327754511205?s=y143mciw7jz7ft2qe3hccjw65m3xe8f2)
+ Annual and monthly mean $\rm{PM_{2.5}}$ [ug/m3] at 0.1° × 0.1°: 
[https://wustl.box.com/v/ACAG-V6GL0204-CNNPM25c0p10](https://wustl.app.box.com/folder/327765750841)
+ Sat$\rm{PM_{2.5}}$ data is alternatively available via the Registry of Open Data on AWS:
[https://registry.opendata.aws/surface-pm2-5-v6gl/](https://registry.opendata.aws/surface-pm2-5-v6gl/)
+ Processed Datasets: 
  + [Annual Global country-level mean $\rm{PM_{2.5}}$](https://wustl.app.box.com/s/e673hbmsl75gechxnrjotenel6k4hdfc)
  + [Annual Canada provincial-level mean $\rm{PM_{2.5}}$](https://wustl.app.box.com/s/186m7jepygxyie217fxmhp39azzg6ehc)
  + [Annual China regional-level mean $\rm{PM_{2.5}}$.](https://wustl.app.box.com/s/i06fhiyh664ig5ukm5hg498d8ez50egg)
  + [Annual India regional-level mean $\rm{PM_{2.5}}$](https://wustl.app.box.com/s/ju2gka9hgicvmg8mh87fg5ueao2tvkr0)
  + [Annual United States state-level mean $\rm{PM_{2.5}}$](https://wustl.app.box.com/s/z7kwgojr4ty3gimn55wso5iw2eh4jk6b)

+ Sat$\rm{PM_{2.5}}$ data V6.GL.02.04 are licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/?ref=chooser-v1)


## Reference and citation

**Shen, S. Li, C. van Donkelaar, A. Jacobs, N. Wang, C. Martin, R. V.: Enhancing Global Estimation of Fine Particulate Matter Concentrations by Including Geophysical a Priori Information in Deep Learning. (2024) ACS ES&T Air. DOI: 10.1021/acsestair.3c00054. [Link](https://pubs.acs.org/doi/full/10.1021/acsestair.3c00054)**

