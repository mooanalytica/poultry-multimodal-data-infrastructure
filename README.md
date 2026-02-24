# Longitudinal Multimodal Big Data Infrastructure for Precision Poultry Monitoring

**Authors:** Daniel Edison Essien, Yashan Dhaliwal, Suresh Neethirajan  
**Institution:** Dalhousie University  
**Journal:** Frontiers in Big Data  
**Contact:** sneethir@gmail.com

---

## Overview

This repository contains the preprocessing and analysis pipeline accompanying the manuscript. Data was collected over 22 consecutive weeks across five commercial-style poultry barns at the Atlantic Poultry Research Centre, Dalhousie University, Truro, Nova Scotia, Canada.

---

## Notebooks

| Notebook | Description |
|----------|-------------|
| `video_illumination_correction.ipynb` | Brightness, contrast and hue correction for barn video footage |
| `audio_denoising_pipeline.ipynb` | Spectral noise reduction for continuous barn audio recordings |
| `environmental_eda.ipynb` | Descriptive statistics for temperature and humidity data |

---

## Dataset

A representative sample dataset is publicly available on Zenodo. The full dataset (10.7 TB) is available under restricted access — contact sneethir@gmail.com to request access through a Data Access Agreement.

**Sample Dataset DOI:** https://doi.org/10.5281/zenodo.18735884

---

## Dependencies
```bash
pip install opencv-python tqdm numpy noisereduce librosa soundfile matplotlib
```

---

## Ethics

All animal procedures were reviewed and approved by the Dalhousie University Animal Care and Use Committee (Dalhousie ACUC), Protocol Approval No. 2025-012, in accordance with the Canadian Council on Animal Care guidelines. The study was conducted as non-invasive observational research. No experimental manipulations were introduced beyond standard husbandry practices. All sensing devices were installed to avoid direct physical contact with the birds, and data collection procedures were designed to minimise disturbance to routine barn operations.

---

## Funding

This study was supported by the Natural Sciences and Engineering Research Council of Canada (NSERC), the Nova Scotia Department of Agriculture, Mitacs Canada, and the New Brunswick Department of Agriculture, Aquaculture and Fisheries. The authors also thank the Atlantic Poultry Research Centre and Dalhousie University for providing facility access and operational support throughout the 22-week data collection period.

---

## Citation

Essien, D.E., Dhaliwal, Y., & Neethirajan, S.R.  
A Longitudinal Multimodal Big Data Infrastructure for Precision Poultry Monitoring.  
Frontiers in Big Data (submitted). DOI: [to be updated upon publication]
