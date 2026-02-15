# Face Clustering Using Distance-Based Learning

## Project Overview

This project implements a distance-based learning approach for face clustering and classification using computer vision techniques. Faces are detected from an image, color-based features are extracted, and K-Means clustering is applied to group similar faces. A template image is then classified based on learned clusters.

The project demonstrates the practical application of similarity-based learning in image analysis.
## Aim

To detect faces from an image, extract meaningful color features, cluster them using a distance-based algorithm, and classify a new template image based on similarity.
## Methodology

The project follows these major steps:

### 1️⃣ Image Acquisition
- The input image is loaded using OpenCV.
- The image is converted from BGR to grayscale for face detection.

### 2️⃣ Face Detection
- Haar Cascade Classifier is used to detect faces.
- Bounding boxes are drawn around detected faces.

### 3️⃣ Feature Extraction
- The original image is converted to HSV color space.
- For each detected face:
  - Mean Hue value is calculated
  - Mean Saturation value is calculated
- These values form a 2D feature vector (Hue, Saturation).

### 4️⃣ Clustering Using K-Means
- K-Means clustering is applied to group faces based on similarity.
- Faces with similar color characteristics are grouped into the same cluster.
- Scatter plots are generated for visualization.

### 5️⃣ Template Image Classification
- A separate template image is loaded.
- Face detection and feature extraction are performed.
- The trained K-Means model predicts the cluster of the template image.

### 6️⃣ Visualization and Analysis
- Scatter plots show cluster distribution.
- Template image cluster prediction is visualized.
- Theoretical analysis of distance-based learning concepts is included in the report.
## Model Evaluation

- Clustering performance is analyzed visually.
- Similarity between faces is determined using Euclidean distance within K-Means.
- Cross-validation and theoretical concepts related to distance-based learning are discussed in the report.
## Key Findings

- HSV color features can effectively represent facial characteristics for clustering.
- Distance-based clustering works well for grouping visually similar data.
- Proper feature extraction significantly impacts clustering performance.
- Visualization helps interpret clustering behavior.

## Conclusion

This project demonstrates how distance-based learning techniques can be applied to real-world image data. By combining computer vision with clustering algorithms, meaningful grouping of faces can be achieved. Feature selection plays a critical role in improving similarity-based classification performance.

## Repository Contents

- `Yasa_Swaminath_Reddy_lab5.ipynb` – Complete Jupyter Notebook with code, outputs, and visualizations
- 📄 Report – Answers to theoretical and analytical questions
- README.md – Project documentation

## How to Run the Project

1. Clone or download the repository
2. Open the Jupyter Notebook file
3. Ensure required libraries are installed:
   - OpenCV
   - NumPy
   - Matplotlib
   - scikit-learn
4. Run all cells to reproduce the results

## Technologies Used

- Python
- OpenCV
- NumPy
- Matplotlib
- scikit-learn (K-Means)
