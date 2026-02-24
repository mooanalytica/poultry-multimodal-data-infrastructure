# Poultry Multimodal Data Infrastructure

## A Longitudinal Multimodal Big Data Infrastructure for Precision Poultry Monitoring

**Authors:** Daniel Edison Essien, Yashan Dhaliwal, Suresh Neethirajan  
**Institution:** Dalhousie University, Faculty of Agriculture & Faculty of Computer Science  
**Journal:** Frontiers in Big Data  
**Contact:** sneethir@gmail.com

---

## Overview

This repository contains the open-source preprocessing and analysis pipeline accompanying the manuscript. The study presents a longitudinal multimodal data acquisition framework collected over 22 consecutive weeks across five commercial-style poultry barns at the Atlantic Poultry Research Centre, Dalhousie University, Truro, Nova Scotia, Canada. 150 Lohmann LSL Lite laying hens were monitored from June 5, 2025 to October 31, 2025 across four complementary sensing modalities: RGB video, audio, radiometric thermal imaging, and environmental sensing.

---

## Repository Contents

| Notebook | Description |
|----------|-------------|
| `video_illumination_correction.ipynb` | Brightness, contrast and hue correction for barn video footage |
| `audio_denoising_pipeline.ipynb` | Spectral noise reduction for continuous barn audio recordings |
| `environmental_eda.ipynb` | Descriptive statistics for temperature and humidity data |
| `thermal_eda.ipynb` | Weekly surface temperature trends across developmental stages |

---

## Dataset Availability

A representative sample dataset is publicly available on Zenodo, including short video and audio clips, sample thermal images, and an environmental CSV file. The sample release is structured to reflect the full dataset organisation.

The full dataset (10.7 TB) is available under restricted access to comply with farm-level confidentiality agreements. Access to the full dataset is provided through a Data Access Agreement by contacting the corresponding author at sneethir@gmail.com.

**Sample Dataset DOI:** [to be updated upon publication]

---

## Sample Dataset Structure
```
Sample_Dataset/
├── Video/                → Short video clip samples (MP4, 1080p, 30fps)
├── Audio/                → Short audio clip samples (WAV, 48kHz, 24-bit)
├── Thermal/              → Sample thermal images (JPEG)
├── Environmental/        → Sample environmental log (CSV)
└── Metadata/
      ├── README.md
      ├── Data_Dictionary.pdf
      └── Folder_Structure_Diagram.png
```

---

## Modality Summary

| Modality      | Format       | Sampling Rate         | Coverage   |
|---------------|--------------|-----------------------|------------|
| Video         | MP4 (HEVC)   | 30 fps, 1080p         | 5 barns    |
| Audio         | WAV          | 48 kHz, 24-bit        | 4 barns    |
| Thermal       | JPEG         | Every 2 days          | 5 barns    |
| Environmental | CSV / XLSX   | Twice daily (AM & PM) | 5 barns    |

---

## File Naming Conventions

| Modality      | Convention                                             | Example                                               |
|---------------|--------------------------------------------------------|-------------------------------------------------------|
| Audio         | BarnX_SampleAudioClip_XX.wav                           | Barn1_SampleAudioClip_01.wav                          |
| Video         | BarnX_SampleClip_[Date].mp4                            | Barn1_SampleClip_5Sept.mp4                            |
| Thermal       | FLIR[ID]_[Date].jpg                                    | FLIR0714_16June.jpg                                   |
| Environmental | Environmental_Data_RoomX_YYYY-MM-DD_to_YYYY-MM-DD.csv | Environmental_Data_Room1_2025-06-05_to_2025-10-31.csv |

---

## Dependencies
```bash
pip install opencv-python tqdm numpy noisereduce librosa soundfile matplotlib
```

---

## Ethics

All animal procedures were reviewed and approved by the Dalhousie University Animal Care and Use Committee, Protocol No. 2025-012, in accordance with Canadian Council on Animal Care guidelines. The study was conducted as non-invasive observational research. All sensing devices were installed to avoid direct physical contact with the birds, and data collection procedures were designed to minimise disturbance to routine barn operations.

---

## Funding

This study was supported by the Natural Sciences and Engineering Research Council of Canada (NSERC), Nova Scotia Department of Agriculture, Mitacs Canada, and the New Brunswick Department of Agriculture, Aquaculture and Fisheries.

---

## Citation

If you use this repository or dataset, please cite:

Essien, D., Dhaliwal, Y., and Neethirajan, S. (2025). A Longitudinal Multimodal Big Data Infrastructure for Precision Poultry Monitoring. Frontiers in Big Data. [DOI to be updated upon publication]
