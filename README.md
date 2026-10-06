# Terrain Classification for Small Legged Robots Using Deep Learning on Tactile Data

## Overview

This project investigates terrain classification for small legged robots using tactile sensor data and machine learning.

The objective is to classify different terrain surfaces based on tactile measurements collected from a robot's foot. The project compares traditional machine learning using engineered tactile features with a deep learning approach that learns directly from raw temporal tactile data.

Three final models are evaluated:

1. SVM using 33 engineered features
2. SVM using the complete 447-dimensional representation
3. 1D CNN using raw tactile data

The experiments show that the SVM using the complete tactile and engineered feature representation achieves the highest test accuracy of **76.08%**.

---

## Problem Statement

Legged robots need to understand the terrain beneath their feet to move safely and effectively.

Vision-based terrain classification can be affected by lighting, occlusion, viewpoint, and environmental conditions. Tactile sensing provides another source of information by directly measuring the interaction between the robot's foot and the ground.

This project explores whether tactile sensor measurements can be used to reliably distinguish different terrain types.

---

## Objectives

- Analyze tactile sensor data collected from different terrain surfaces.
- Preprocess and normalize the tactile measurements.
- Compare engineered features with raw tactile measurements.
- Develop traditional machine learning and deep learning models.
- Evaluate classification performance across different terrain types.
- Analyze common classification errors and terrain confusions.
- Identify the best-performing representation and model for the dataset.

---

## Dataset

The dataset contains **5,990 samples** collected from eight terrain classes.

### Terrain Classes

| Label | Terrain |
|---:|---|
| 0 | Asphalt |
| 1 | Cork |
| 2 | Grass |
| 3 | Gravel |
| 4 | Lab |
| 5 | Laminate Wood |
| 6 | Pebble |
| 7 | Sand |

Each sample contains:

- **414 raw tactile measurements**
- **33 engineered features**
- **447 total input features**

The 414 tactile measurements correspond to:

- 6 tactile channels
- 69 temporal readings per channel

Therefore:

```text
6 × 69 = 414 tactile values
414 tactile values + 33 engineered features = 447 features