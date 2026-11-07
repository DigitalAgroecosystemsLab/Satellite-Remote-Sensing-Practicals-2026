# Satellite Remote Sensing — Practical Classes (2026)

**University of Manitoba · Digital AgroEcosystems Lab (DALab)**  
**Instructor:** Dr. Nasem Badreldin

Interactive practicals in satellite remote sensing, Earth observation and agricultural landscape analysis. Each practical runs in **Google Colab** using Python. No local Python installation is required.

> **Students:** Select **Open in Colab** below, then use **File → Save a copy in Drive** before editing or running the notebook. **Each student uses their own Google Earth Engine-enabled Cloud project and Google Drive account.** Class input datasets, where needed, are accessed as specified by the notebook; analytical outputs go to the student’s own Drive.

## Practical notebooks

| Practical | Topics and activities | Launch |
|---|---|---|
| **01. Satellite Remote Sensing Fundamentals & Multispectral Imagery** | Sentinel-2, Landsat and MODIS; NDVI, EVI, SAVI; June–August seasonal means and time series | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DigitalAgroecosystemsLab/Satellite-Remote-Sensing-Practicals-2026/blob/main/Practical_01_Multisensor_Vegetation_Indices.ipynb) |
| **02. Vegetation Indices & Multitemporal Dynamics** | Sentinel-2 field-level growth curves, 10-day composites and crop phenology metrics | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DigitalAgroecosystemsLab/Satellite-Remote-Sensing-Practicals-2026/blob/main/Practical_02_Crop_Growth_Phenology.ipynb) |
| **03. Land Use/Land Cover Dynamics** | AAFC Annual Crop Inventory, land-cover transitions, area statistics and Sankey diagrams | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DigitalAgroecosystemsLab/Satellite-Remote-Sensing-Practicals-2026/blob/main/Practical_03_AAFC_LULC_Dynamics.ipynb) |
| **04. Digital Elevation Models & Hydrological Processes** | LiDAR 1 m, LiDAR 30 m and SRTM 30 m; terrain and hydrology analyses | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DigitalAgroecosystemsLab/Satellite-Remote-Sensing-Practicals-2026/blob/main/Practical_04_DEM_Hydrology.ipynb) |
| **05. Hyperspectral Satellite Imaging & Spectroscopy** | Soil and vegetation spectral signatures | *Coming soon* |
| **06. Synthetic Aperture Radar (SAR)** | Sentinel-1 and agricultural monitoring | *Coming soon* |
| **07. Multisensor Image Fusion & Data Integration** | Integrating optical, SAR and terrain data | *Coming soon* |
| **08. Satellite Applications & Research Case Studies** | Agricultural decision-making and research applications | *Coming soon* |

## Getting started

1. Click **Open in Colab** next to the practical assigned for class.
2. Sign into your own Google account, and select **File → Save a copy in Drive** so your notebook and edits are preserved.
3. In the student configuration cell, enter **your own Google Earth Engine project ID** and **student identifier**. The account/project must have Earth Engine access.
4. Run cells **from top to bottom**. Follow the instructions when prompted to authenticate Earth Engine and mount your Google Drive.
5. Review maps, data quality and scientific interpretation as you proceed. Save/export required figures and tables to **your** Google Drive, and check that asynchronous GeoTIFF exports have completed.
6. Follow the instructor’s instructions in UM Learn for what to submit. The exported files and saved notebook copy are separate artifacts.

**Important:** Never upload your credentials, account tokens, private field locations, individual student outputs or full research datasets to this public course repository.

## Notebook-specific guidance

| Practical | Student-defined study area | External inputs and outputs |
|---|---|---|
| 01 | Draw **one ROI** on the interactive map (bbox/GeoJSON alternatives) | Landsat/Sentinel-2/MODIS from Earth Engine; exports indices and figures to your own Drive |
| 02 | Draw **three field polygons** (with alternate input options) | Sentinel-2 from Earth Engine; exports field time series, phenology and rasters to your own Drive |
| 03 | Draw **one agricultural landscape ROI** | AAFC Annual Crop Inventory from Earth Engine; exports area statistics, maps and transitions to your own Drive |
| 04 | **No student-uploaded ROI required**; the supplied Elm Creek regional ROI and zoom boundary are loaded automatically | LiDAR archives are in instructor-shared Drive; SRTM from Earth Engine; outputs go to your own Drive |

### Practical 4 instructor-provided datasets

- [Regional ROI shapefile folder (`ROI_1.shp`, `.shx`, `.dbf`, `.prj`, `.cpg`)](https://drive.google.com/drive/folders/1Na-g_HROPwbgsYLJ3Cj9u3xCFJmFUz-s)
- [LiDAR archives (`Elm_Creek_LiDAR_DEM1.zip` and `Elm_Creek_LiDAR_DEM2.zip`) plus `Zoom_roi.kmz`](https://drive.google.com/drive/folders/1i3Ovt3cPGgTaw5rgfruavjWBoqSBFDAb)

These inputs are **not stored in GitHub**. Practical 4 attempts to download required data automatically from the instructor’s shared folders. If access fails, contact the instructor; do not substitute a different elevation dataset.

## Scientific and technical notes

- The notebooks are educational exercises; vegetation phenology is a satellite-derived proxy and not a direct observation of field management or crop developmental stages.
- Different satellite products, resolutions and acquisition dates can affect comparisons. Interpret class changes and DEM-derived flow pathways with care.
- Cloud masking, Earth Engine quotas, shared-folder access and Google Colab availability can change. If a cell fails, preserve the error message and contact the instructor.
- Notebook metadata and Python syntax are checked prior to publication; **live Earth Engine computations, interactive widgets, full LiDAR downloads and all exports must be tested in a student-equivalent Colab account before classroom release**.

## Repository contents

```text
Satellite-Remote-Sensing-Practicals-2026/
├── README.md
├── Practical_01_Multisensor_Vegetation_Indices.ipynb
├── Practical_02_Crop_Growth_Phenology.ipynb
├── Practical_03_AAFC_LULC_Dynamics.ipynb
├── Practical_04_DEM_Hydrology.ipynb
└── .gitignore
```

## Acknowledgment

Course materials prepared for teaching at the University of Manitoba, Digital AgroEcosystems Lab.
