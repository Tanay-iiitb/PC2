# PC2 – Medical Image Enhancement and Feature Evaluation

## Overview
This project focuses on analyzing **medical image enhancement techniques** using a set of handcrafted statistical and texture features.  
We applied multiple filters and evaluated their performance using various distance and similarity metrics to determine the most effective enhancement methods.

---
## How to run
Clone the repository: git clone https://github.com/Tanay-iiitb/PC2
Open the notebook in Jupyter/Colab/Vs-code then run all cells sequentially to get results.

---
## What We Did
We used several image enhancement techniques such as:
- Low-pass filtering (noise reduction)
- High-pass filtering (edge sharpening)
- Gaussian smoothing
- Histogram Equalization (HE)
- CLAHE (Adaptive contrast)
- Sobel and Prewitt edge enhancement
- Frequency Domain Sharpening
- Laplacian Filtering
We simulated and removed these noises:
- Gaussian Noise 
- Salt and pepper noise
- Mixture of S&P + gaussian noise
- Band Pattern noise
- Pattern/sinusoidal noise
- Motion blurred noise


For evaluation, we compared **handcrafted features** (Mean, Std, Entropy, Contrast, Energy, Homogeneity, LBP, Hu Moments, etc.) between **original and enhanced** images.

---

## Evaluation Metrics
We used a **multi-metric weighted scoring system** combining:
- **Distance metrics:** Euclidean, Manhattan, Cosine, Canberra, Minkowski  
- **Similarity metrics:** Pearson, Spearman, Mutual Information  
- **Preservation metric:** Feature Preservation Ratio  

These were normalized and combined with weights to compute an overall enhancement score for each technique.

---

## Notebook Contents
The Jupyter Notebook includes:
1. Image loading and preprocessing  
2. Application of multiple enhancement filters  
3. Feature extraction (statistical + texture)  
4. Computation of multi-metric comparison  
5. Weighted ranking of techniques  
6. Visualization of top-performing methods (radar chart, bar chart)

---

## References
- Gonzalez & Woods – Digital Image Processing (4th Ed.)  
- Haralick et al. – Textural Features for Image Classification (IEEE, 1973)  
- Ojala et al. – Texture Measures and LBP Patterns (1996)  
- Gonzalez, Woods & Eddins – Digital Image Processing Using MATLAB  


---

