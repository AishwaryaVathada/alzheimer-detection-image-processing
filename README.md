# alzheimer-detection-image-processing
Developed a Computer-Aided Diagnosis (CAD) system for early-stage Alzheimer’s detection, leveraging multimodal neuroimaging fusion to integrate structural and anatomical insights for accurate disease staging.

---

## contents

| File                            | Description |
|---------------------------------|-------------|
| `stripping-mri-image.ipynb` | Preprocessing, enhancement, and segmentation of MRI brain scans |
| `white-gray-matter-ratio.ipynb`| Extended version with feature extraction and fusion strategy |
| `sample_data`      | Example MRI images (T1-weighted Axial, Coronal, Sagittal) |

---

## key Techniques Used

- ✅ Intensity Adjustment (α and β tuning)
- ✅ Histogram Equalization
- ✅ High-pass Filtering (edge enhancement)
- ✅ Skull Stripping and Masking
- ✅ Otsu’s Thresholding and Random Walker Segmentation
- ✅ Gray Matter / White Matter Volume Ratio
- ✅ Brain scan Fusion (MRI + PET) using PCA & Wavelet Transforms

---

## outcome

Classification of MRI scans into:
- Normal Brain
- Alzheimer’s Brain (based on GM/WM volume ratio)

| Ratio (GM/WM) | Diagnosis           |
|---------------|---------------------|
| > 0.6         | Normal Brain        |
| 0.5 – 0.6     | Early Stage AD      |
| < 0.5         | Advanced Stage AD   |

---

## how to Use

1. Open notebooks in [Google Colab](https://colab.research.google.com)
2. Upload MRI slices (T1-weighted or FLAIR preferred)
3. Run each step: pre-processing → segmentation → ratio calculation
4. Review plots and ratio to determine AD presence and stage

---

## authors

- Lakshmi Aishwarya Vathada  
- Nikitha Prasanth Nambiar  
- Noopura Parvathi A  

> *Submitted as part of final year B.Tech project in ECE, Amrita School of Engineering, 2020*

---
