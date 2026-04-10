# Multi-Plant Disease Perception System

## Overview
This project explores a perception-driven approach to multi-plant disease classification using deep learning models. The system is designed to operate under realistic conditions, where variability in lighting, background, and data quality affects model performance.

The work focuses on comparing a baseline Artificial Neural Network (ANN) with a Convolutional Neural Network (CNN) to understand performance differences in visual disease recognition tasks.

---

## Problem
Plant diseases significantly impact agricultural productivity, and early detection is critical for reducing losses and improving crop management.

However, most models perform well only on clean, curated datasets and struggle when exposed to real-world variability such as:
- inconsistent lighting
- background noise
- varying image quality

This project investigates how different model architectures handle these challenges.

---

## Dataset
The project is based on publicly available multi-plant disease datasets containing images of healthy and diseased leaves across multiple crop types.

Typical datasets in this domain include tens of thousands of images across multiple disease classes and plant species, often organized into structured train/validation splits :contentReference[oaicite:1]{index=1}.

Due to size limitations, the full dataset is not included in this repository.

👉 You can use datasets like:
- PlantVillage / New Plant Diseases Dataset (Kaggle)
- Multi-class crop disease datasets

---

## Approach

### Models Used
- **ANN (Baseline)**  
  - Used for comparison  
  - Limited spatial feature extraction  
<img width="1542" height="1166" alt="image" src="https://github.com/user-attachments/assets/f41f2e67-ef90-45dc-9b0b-d37e3e0bf689" />

- **CNN (Primary Model)**  
  - Captures spatial patterns in leaf images  
  - More suitable for visual perception tasks  
<img width="1556" height="1190" alt="image" src="https://github.com/user-attachments/assets/7d24f790-0638-42b0-814f-245bed62a6fc" />

---

### Pipeline
- Image preprocessing and normalization  
- Model training (ANN vs CNN)  
- Evaluation using classification metrics  
- Visualization of results (confusion matrix, predictions)

---

## Challenges
- High variability in real-world image conditions  
- Overfitting on structured datasets  
- Generalization across plant species and disease types  

---

## Results & Insights
- CNN significantly outperforms ANN in visual classification tasks  
- Model accuracy alone is not sufficient — robustness is critical  
- Performance degrades when conditions deviate from training data  

👉 Key takeaway:  
Real-world deployment requires systems that handle noise, variability, and unseen conditions—not just high benchmark accuracy.

---

## Tech Stack
- Python  
- TensorFlow / Keras  
- NumPy, Pandas  
- OpenCV  
- Matplotlib  

---
## Note
Model files and full datasets are not included to keep the repository lightweight and focused on implementation.

---

## Future Work
- Improve robustness under real-world conditions  
- Explore multi-modal sensing (beyond RGB images)  
- Integrate with real-time monitoring systems  

---
