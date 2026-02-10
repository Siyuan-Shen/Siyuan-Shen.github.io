---
title: "North America Satellite-derived Monthly PM₂.₅ Total and Compositional Mass (0.01x0.01) - V6.NA.01"
date: 2026-02-08
tags: ["Remote Sensing","Air Quality","Gloabl Datasets","Deep Learning","Geophysical Constraints","Simulations"]
author: ["Siyuan Shen","Chi Li","Aaron van Donkelaar","Nathan A. Jacobs","Randall V. Martin"]
description: "This dataset contains North America annual and monthly ground-level fine particulate matter ($\rm{PM_{2.5}}$) total and compositional mass for 2000-2023 at around 1 km resolution."
summary: "This version is recommended for users with a North American-only focus and includes total and compositional PM₂.₅, as well as the as well as the uncertainty estimation for 2000-2023. This version uses deep learning based structures."
cover:
    image: "image.png"
    alt: "Figure title (preferably 1280x720 pixels)"
    relative: true
editPost:
    URL: "https://www.satpm.org/v6-na-01"
    Text: "SatPM (ACAG Datasets)"
showToc: true
disableAnchoredHeadings: false

---

## Overview

We estimate annual and monthly ground-level fine particulate matter (PM₂.₅)  total and compositional mass concentrations over North America for 1998-2023 by combining Aerosol Optical Depth (AOD) retrievals (Dark Target, Deep Blue, MAIAC, and SNPP VIIRS) that make use of observations from numerous satellite-based NASA instruments (MODIS/Terra, MODIS/Aqua, MISR/Terra, SeaWiFS/SeaStar, VIIRS/SNPP, and VIIRS/NOAA20) with the GEOS-Chem chemical transport model, and subsequently calibrating ground-based observations using a residual Convolutional Neural Network (CNN), as detailed in the below reference for V6.NA.01. 

---

## View dataset

Annual and monthly datasets are provided in NetCDF [.nc] format. Gridded files use the WGS84 projection. Latitude centers on the 0.01°×0.01° grid range from 10.005 °N to 69.995 °N and longitude centers range from 169.995 °W to 40.005 °W. Please contact our Support Team (support@satpm.org) for further information.
 
Note that these estimates are primarily intended to aid in large-scale studies. Annual and coarse-resolution averages correspond to a simple mean of within-grid values. Gridded datasets are provided to allow users to agglomerate data as best meets their particular needs. High-resolution (0.01° × 0.01°) datasets are gridded at the finest resolution of the information sources that were incorporated but are unlikely to fully resolve PM₂.₅ gradients at the gridded resolution due to influence by information sources at coarser resolution.

Note that a VPN may be necessary  to access the Box data repositories, depending on local web traffic restrictions.

+ Annual and monthly mean total and compositional $\rm{PM_{2.5}}$ [ug/m3] at 0.01° × 0.01°:
[https://wustl.box.com/v/ACAG-V6NA01-CNNPM25](https://wustl.box.com/s/qwvj00cvghiebo7wdf1voip42mcdvk89)
+ Annual and monthly mean $\rm{PM_{2.5}}$ [ug/m3] at 0.1° × 0.1°: 
[https://wustl.box.com/v/ACAG-V6NA01-CNNPM25-Uncertainty](https://wustl.box.com/s/njjw6nbgx8zeac9z4hv2ijxyu9ib8ckg)
+ Sat$\rm{PM_{2.5}}$ data V6.NA.01 are licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/?ref=chooser-v1)


---

## Reference and citation

**Shen, S. Li, C. van Donkelaar, A. Jacobs, N. Martin, R. V.: Enhancing Estimation of Fine Particulate Matter Chemical Composition across North America by Including Geophysical A Priori Information in Deep Learning with Uncertainty Quantification. (2026) ACS ES&T Air Article ASAP. DOI: 10.1021/acsestair.5c00251. [Link](https://pubs.acs.org/doi/10.1021/acsestair.5c00251)**

