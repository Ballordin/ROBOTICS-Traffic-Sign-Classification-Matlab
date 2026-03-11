# Source Code & Application Data

This folder contains the core logic for the traffic sign detection and classification system.

## Components:
* **`app_TP1_25547_15526.mlapp`**: A MATLAB App Designer file that integrates the vision pipeline with a functional GUI. It handles real-time frame acquisition, color thresholding, and geometric classification.
* **`History.mat`**: A data file containing the detection history used for statistical analysis, including accuracy, precision, and recall calculations.

### Key Logic:
1. **Color Segmentation:** Dynamic HSV filtering to isolate Blue (Mandatory) and Red (Prohibitory) signs.
2. **Morphological Operations:** Noise reduction using opening/closing operations to refine the binary mask.
3. **Blob Analysis:** Feature extraction (Area, Eccentricity, Euler Number) to identify sign shapes (Circles vs Octagons).
