# 📝 Project Summary: Alzheimer's Detection via Image Processing & Fusion

## 🎯 Problem Statement

Alzheimer’s Disease (AD) is a chronic neurodegenerative condition that often goes undetected in early stages. Current clinical diagnosis is often delayed or inaccurate. The goal of our project is to create a **Computer-Aided Diagnosis System (CADS)** that uses **MRI and PET scans** for early detection of AD by segmenting brain tissue and analyzing neurodegeneration markers.

---

## 🎯 Objective

To implement an image processing-based solution that:
1. Preprocesses and enhances MRI brain scans
2. Segments gray and white matter from multiple brain cross-sections
3. Calculates volume ratios to identify AD severity
4. Fuses MRI and PET images for comprehensive structural + functional information

---

## 🧠 Why This Matters

- Early AD diagnosis enables better treatment outcomes and planning
- Reduces dependency on expensive or subjective clinical evaluations
- Bridges the gap between biomedical imaging and practical software tools
- Offers explainable and visual output for physicians and researchers

---

## ⚙️ Methodology Overview

1. **Image Preprocessing**  
   - Resize, enhance contrast, adjust intensity (α & β), filter noise
2. **Segmentation**
   - Otsu’s thresholding & Random Walker to extract GM/WM regions
3. **Skull Stripping & Masking**
   - Remove non-brain tissues and background
4. **Volume Ratio Calculation**
   - Compare gray-to-white matter volume across slices
5. **Image Fusion (MRI + PET)**
   - PCA & wavelet-based fusion for better visualization
6. **Diagnosis**
   - Use predefined GM/WM ratio thresholds to detect AD stage

---

## 📊 Results

- High accuracy in differentiating Normal vs AD brain
- Segmentation and enhancement steps successful across axial, sagittal, coronal planes
- Volume ratio-based classification worked consistently for our dataset

---

## 🔍 Findings

| Gray/White Matter Ratio | Conclusion      |
|-------------------------|------------------|
| > 0.6                   | Healthy Brain     |
| 0.5 – 0.6               | Early-Stage AD    |
| < 0.5                   | Advanced AD       |

MRI + PET fusion further improved visual diagnostics and interpretability.

---

## 📌 Future Enhancements

- Deep learning classification (e.g., CNN)
- Real-time scanner integration
- Larger dataset testing for statistical validation
- Clinical usability evaluation with professionals

---

## 📚 References

- ISBB 2014: PET-MRI Wavelet Fusion  
- IEEE BioMed, 2019: Feature Extraction + KNN  
- Harvard Brain Atlas Dataset

---
