# Sample Dataset — README
## A Longitudinal Multimodal Big Data Infrastructure for Precision Poultry Monitoring

**Authors:** Daniel Edison Essien, Yashan Dhaliwal, Suresh Neethirajan  
**Institution:** Dalhousie University, Faculty of Agriculture & Faculty of Computer Science  
**Journal:** Frontiers in Big Data  
**Contact:** sneethir@gmail.com & sureshraja@dal.ca
 
---

## Dataset Overview

This sample dataset accompanies the manuscript and provides representative files 
across all four modalities collected during the 22-week longitudinal study conducted 
at the Atlantic Poultry Research Centre, Truro, Nova Scotia, Canada.

150 Lohmann LSL Lite laying hens were monitored across five commercial-style barns 
from June 5, 2025 to October 31, 2025.

---

## Folder Structure
```
Sample_Dataset/
├── Audio/                  → Raw .wav audio clips (48 kHz, 24-bit, WAV format)
├── Environmental/          → Temperature and relative humidity logs (.csv and .xlsx)
├── Thermal/                → Radiometric thermal images (.jpg)
├── Video/                  → Raw video clips (1080p, 30fps, MP4 format)
└── Metadata/
      ├── README.md         
      ├── Data_Dictionary.pdf → Definitions for all variables and file naming conventions
      └── Folder_Structure_Diagram.png → Visual overview of dataset organisation
```

---

## Modality Summary

| Modality      | Format       | Sampling Rate         |
|---------------|--------------|-----------------------|
| Video         | MP4 (HEVC)   | 30 fps, 1080p         |
| Audio         | WAV          | 48 kHz, 24-bit        |
| Thermal       | JPEG (rJPEG) | Every 2 days          |
| Environmental | CSV / XLSX   | Twice daily (AM & PM) |

---

## File Naming Conventions

| Modality      | Convention                                              | Example                                          |
|---------------|---------------------------------------------------------|--------------------------------------------------|
| Audio         | BarnX_SampleAudioClip_XX.wav                           | Barn1_SampleAudioClip_01.wav                     |
| Video         | BarnX_SampleClip_[Date].mp4                            | Barn1_SampleClip_5Sept.mp4                       |
| Thermal       | FLIR[ID]_[Date].jpg                                    | FLIR0714_16June.jpg                              |
| Environmental | Environmental_Data_RoomX_YYYY-MM-DD_to_YYYY-MM-DD.csv  | Environmental_Data_Room1_2025-06-05_to_2025-10-31.csv |

---

## Data Access

The full dataset is deposited on Zenodo under restricted access to comply with 
farm-level confidentiality agreements. Access is granted through a Data Access Agreement.

**Full Dataset DOI:** [to be updated upon publication]  
**Code Repository:** https://github.com/mooanalytica/poultry-multimodal-data-infrastructure

---

## Ethics

All animal procedures were reviewed and approved by the Dalhousie University Animal Care and Use Committee (Dalhousie ACUC), Protocol Approval No. 2025-012, 
in accordance withthe Canadian Council on Animal Care guidelines. The study was conducted as non-invasiveobservational research. 
No experimental manipulations were introduced beyond standardhusbandry practices. 
All sensing devices were installed to avoid direct physical contact with the birds, 
and data collection procedures were designed to minimize disturbance to routine barn operations.

---

## Funding

This study was supported by the Natural Sciences and Engineering Research Council 
of Canada (NSERC), Nova Scotia Department of Agriculture, Mitacs Canada, and the 
New Brunswick Department of Agriculture, Aquaculture and Fisheries.
