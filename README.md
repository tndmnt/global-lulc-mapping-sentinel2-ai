# Global Land Cover Mapping with Sentinel-2 and AI

## Overview
This project explores land use and land cover (LULC) change detection by leveraging Sentinel-2 satellite imagery, deep learning (UNet), and cloud computing. It generates global, high-resolution annual LULC maps and visualizes land dynamics across space and time — particularly focusing on Mato Grosso, Brazil.

## Objectives
- Build and apply a UNet segmentation model trained on >5 billion manually labelled pixels across 10 land cover categories.
- Access and visualize satellite-derived LULC data from the Microsoft Planetary Computer.
- Perform multi-scale land cover change analysis: aggregate, pixel-by-pixel (confusion matrix + Sankey diagram), and zonal (municipality-level).

## Key Features
- **High Resolution (10m)**: Based on Sentinel-2 imagery.
- **Global & Annual**: LULC maps from 2017 to 2022.
- **Deep Learning-Based**: Trained with class imbalance handling, dropout, and data augmentation.
- **Rich Visualizations**: Static and interactive maps, bar plots, Sankey diagrams.
- **Real-World Use Case**: Mato Grosso (Brazil) — agricultural expansion and deforestation.

## Technologies Used
- Python (xarray, geopandas, matplotlib, hvplot, odc.stac)
- Microsoft Planetary Computer
- UNet architecture (Keras/TensorFlow)
- Sentinel-2 Satellite Data

## Land Cover Classes
- Water, Trees, Grass, Flooded Vegetation, Crops, Scrub/Shrub, Built Area, Bare Ground, Snow/Ice, Cloud

## Repository Structure
- `C3.ipynb/`: Jupyter Notebooks for data access, preprocessing, and analysis
- `geodata.yml/`: The environment needed to run the code
- `Presentation.pdf/`: Presentation content

## Acknowledgements
- Sentinel-2 data via [Microsoft Planetary Computer](https://planetarycomputer.microsoft.com/)
- LULC classification methodology based on [Dynamic World](https://www.dynamicworld.app/)
- UNet: Ronneberger et al., 2015
