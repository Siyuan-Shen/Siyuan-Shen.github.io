---
title: "Global Satellite-derived Monthly PM₂.₅ Total Mass (0.01x0.01) - V6.02.04"
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
    URL: "https://sites.wustl.edu/acag/datasets/surface-pm2-5/#V6.GL.02.04"
    Text: "ACAG Datasets"
showToc: true
disableAnchoredHeadings: false

---

## Overview

We estimate annual and monthly ground-level fine particulate matter ($\rm{PM_{2.5}}$) for 2000-2019 by combining Aerosol Optical Depth (AOD) retrievals (Dark Target, Deep Blue, MAIAC) that make use of observations from numerous satellite-based NASA instruments (MODIS/Terra, MODIS/Aqua, MISR/Terra, SeaWiFS/SeaStar, VIIRS/SNPP, and VIIRS/NOAA20) with the GEOS-Chem chemical transport model, and subsequently calibrating to global ground-based observations using a residual Convolutional Neural Network (CNN), as detailed in the below reference for V6.GL.01. V6.GL.02.04 follows the methodology of V6.GL.01 but updates the ground-based observations used to calibrate the geophysical $\rm{PM_{2.5}}$ estimates for the entire time series, extends temporal coverage through 1998 – 2023, and includes retrievals from the SNPP VIIRS instrument. Also, previous versions were reported to contain abnormally low values in certain, rare circumstances. This limitation has been addressed in V6.GL.02.04 using a modified padding strategy and stronger geophysical constraints.

---

## View dataset

+ Annual and monthly mean $\rm{PM_{2.5}}$ [ug/m3] at 0.01° × 0.01°:
[https://wustl.box.com/v/ACAG-V6GL0204-CNNPM25](https://wustl.box.com/v/ACAG-V6GL0204-CNNPM25)
+ Annual and monthly mean $\rm{PM_{2.5}}$ [ug/m3] at 0.1° × 0.1°: 
[https://wustl.box.com/v/ACAG-V6GL0204-CNNPM25c0p10](https://wustl.box.com/v/ACAG-V6GL0204-CNNPM25c0p10)
+ Sat$\rm{PM_{2.5}}$ data is alternatively available via the Registry of Open Data on AWS:
[https://registry.opendata.aws/surface-pm2-5-v6gl/](https://registry.opendata.aws/surface-pm2-5-v6gl/)
+ Processed Datasets: 
  + [Annual Global country-level mean $\rm{PM_{2.5}}$](https://wustl.app.box.com/s/e673hbmsl75gechxnrjotenel6k4hdfc)
  + [Annual Canada provincial-level mean $\rm{PM_{2.5}}$](https://wustl.app.box.com/s/186m7jepygxyie217fxmhp39azzg6ehc)
  + [Annual China regional-level mean $\rm{PM_{2.5}}$.](https://wustl.app.box.com/s/i06fhiyh664ig5ukm5hg498d8ez50egg)
  + [Annual India regional-level mean $\rm{PM_{2.5}}$](https://wustl.app.box.com/s/ju2gka9hgicvmg8mh87fg5ueao2tvkr0)
  + [Annual United States state-level mean $\rm{PM_{2.5}}$](https://wustl.app.box.com/s/z7kwgojr4ty3gimn55wso5iw2eh4jk6b)

+ Sat$\rm{PM_{2.5}}$ data V6.GL.02.04 are licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/?ref=chooser-v1)


---

## Using data with Python


### Start Python:

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
tempor incididunt ut labore et dolore magna aliqua.

```python
import numpy as np
import pandas as pd
```

### Open the file:

Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat `data.csv`.

```python
file_path = 'data.csv'
with open(file_path, 'r') as file:
```

### Read data:

Duis aute irure dolor in reprehenderit in voluptate velit esse
cillum dolore eu fugiat nulla pariatur.

```python
    lines = file.readlines()
```

### Parse and process data:

Duis aute `line_data` irure dolor in reprehenderit in voluptate velit esse
cillum dolore eu fugiat nulla pariatur `data.extend`.

```python
data = []
for line in lines:
    line_data = line.strip().split(',')  # Split the line into a list of values
    line_data = [float(value) for value in line_data]  # Convert values to floats
    data.extend(line_data)  # Extend the main list with values from the line
```

#### Compute summary statistics using NumPy:

Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum: `data_array`. 

```python
data_array = np.array(data)  # Convert the list to a NumPy array
mean = np.mean(data_array)
median = np.median(data_array)
std_dev = np.std(data_array)
min_value = np.min(data_array)
max_value = np.max(data_array)
```

#### Display summary statistics:

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
consequat `print`.

```python
print(f"Mean: {mean}")
print(f"Median: {median}")
print(f"Standard Deviation: {std_dev}")
print(f"Minimum Value: {min_value}")
print(f"Maximum Value: {max_value}")
```

---

## Description of simulation parameters

| Parameter |   Value   |  Language  | Time period |           Description            |
| :-------: | :-------: | ---------- | :---------: | :------------------------------: |
|  $\alpha$ |   $1/2$   | French     |  1930–1954  |         Tempor dolor in          |
| $\lambda$ |   $e/2$   | French     |  1930–1954  |       Fugiat sint occaecat       |
|  $\gamma$ |  $\ln(3)$ | Spanish    |  1833–1954  |      Duis officia deserunt       |
|  $\omega$ | $10^{-4}$ | Italian    |  1930–1994  | Excepteur et dolore magna aliqua |
|  $\sigma$ |   $1.5$   | Portuguese |  1990–2023  |         Lorem culpa qui          |
|  $\chi^2$ |  $\pi^2$  | Portuguese |  1990–2023  |         Labore et dolore         |


## Reference and citation

Shen, S. Li, C. van Donkelaar, A. Jacobs, N. Wang, C. Martin, R. V.: Enhancing Global Estimation of Fine Particulate Matter Concentrations by Including Geophysical a Priori Information in Deep Learning. (2024) ACS ES&T Air. DOI: 10.1021/acsestair.3c00054. [Link](https://pubs.acs.org/doi/full/10.1021/acsestair.3c00054)

