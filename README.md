# AI Surrogate ERG in Cone Dystrophy / CORD — WOC 2026

This repository contains the Python/Google Colab analysis workflow for a feasibility study evaluating whether multimodal retinal imaging features can approximate 30-Hz flicker full-field electroretinography (ERG) amplitude in cone dystrophy and cone-rod dystrophy (CORD).

## Project details

**Title:** Artificial Intelligence as a Surrogate for Electroretinography in Cone Dystrophy Diagnosis: A Feasibility Framework  
**Conference:** World Ophthalmology Congress 2026  
**Poster ID:** PV-AI-033  
**Author:** Suneth Dayan Lindamulage  
**OSF DOI:** 10.17605/OSF.IO/NQSKD

## Methods

The workflow uses EfficientNetB0 transfer learning for CORD-versus-normal image classification and feature extraction from optical coherence tomography (OCT), fundus autofluorescence (FAF), and fundus photography (FF).

Ridge regression with leave-one-out cross-validation was used to predict 30-Hz flicker ERG amplitude from image-derived features. Multimodal fusion combined OCT, FAF, and FF features.

## Dataset note

A total of 665 retinal images were processed across training and test datasets. The ERG-linked disease dataset included 63 CORD cases curated from 17 publications, representing 9 gene-associated groups and clinically diagnosed cases.

Raw retinal images from published articles are not redistributed in this repository because of copyright restrictions. This repository includes code, derived statistical outputs, and generated summary figures only.

## Main result

Multimodal OCT + FAF + FF fusion predicted 30-Hz flicker ERG amplitude with:

- MAE: 11.68 µV
- RMSE: 15.05 µV
- R²: 0.695
- Pearson r: 0.842
- Spearman r: 0.844

## Reproducibility

The notebook documents the analysis workflow used for the WOC 2026 feasibility study. Code and derived outputs are provided to support transparent reporting and future extension of the project.

## License

Code is shared under the MIT License. Published retinal images are not included.
