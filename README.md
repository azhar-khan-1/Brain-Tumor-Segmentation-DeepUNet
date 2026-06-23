# 🧠 Brain Tumor Segmentation using Deep U-Net

## 📌 Project Overview

Brain tumor segmentation is a critical task in medical image analysis that assists radiologists in identifying and quantifying tumor regions from MRI scans. This project implements a **Deep U-Net architecture** for automatic multi-class brain tumor segmentation using the **BraTS 2020 dataset**.

The model learns to identify different tumor subregions from multi-modal MRI images and generates pixel-wise segmentation masks for accurate tumor localization.

---

## 🎯 Objectives

* Perform automatic brain tumor segmentation from MRI scans.
* Segment multiple tumor subregions.
* Evaluate model performance using Dice Similarity Coefficient (DSC) and Intersection over Union (IoU).
* Analyze segmentation performance across different tumor sizes.
* Visualize best-case and worst-case predictions.

---

## 🗂 Dataset

**Dataset:** BraTS 2020 (Brain Tumor Segmentation Challenge)

### MRI Modalities Used

* T1
* T1CE (T1 Contrast Enhanced)
* T2
* FLAIR

### Segmentation Classes

| Class | Description                    |
| ----- | ------------------------------ |
| 0     | Background                     |
| 1     | Necrotic / Non-Enhancing Tumor |
| 2     | Edema                          |
| 3     | Enhancing Tumor                |

---

## 🏗 Model Architecture
![Model Architecture](images/Model_Architecture.png)

This project utilizes a **Deep U-Net** architecture consisting of:

* Encoder-Decoder structure
* Skip Connections
* Multi-class Segmentation Output
* Convolution + Batch Normalization Blocks
* Upsampling Layers

The architecture enables precise localization while preserving contextual information from MRI scans.

---

## 📊 Results

### Performance Metrics

| Metric             | Value |
| ------------------ | ----- |
| Average Dice Score | 0.67+ |
| Average IoU        | 0.57+ |
| Best Dice Score    | 0.96  |

---

## 🖼 Visualizations

### MRI Modalities

![MRI Modalities](images/mri_modalities_best_case.png)

### Multi-Class Tumor Labels

![Tumor Labels](images/brats_multiclass_labels.png)

### Tumor Subregions

![Tumor Subregions](images/brats_tumor_subregions.png)

### Best Case Segmentation

![Best Case](images/best_case_segmentation.png)

### Worst Case Segmentation

![Worst Case](images/worst_case_segmentation.png)

### Tumor Size Distribution

![Tumor Distribution](images/tumor_size_distribution.png)

### Tumor Size vs Dice Score

![Tumor Size vs Dice](images/tumor_size_vs_dice.png)

---

## 📁 Project Structure

```text
Brain-Tumor-Segmentation-DeepUNet
│
├── notebooks/
│   └── Brain_Tumor_Segmentation.ipynb
│
├── images/
│
├── results/
│   └── metrics_summary.csv
│
├── README.md
├── requirements.txt
└── LICENSE
```

---

## ⚙️ Installation

```bash
git clone https://github.com/your-username/Brain-Tumor-Segmentation-DeepUNet.git

cd Brain-Tumor-Segmentation-DeepUNet

pip install -r requirements.txt
```

---

## 🚀 Future Improvements

* Attention U-Net Implementation
* Residual U-Net Architecture
* 3D Brain Tumor Segmentation
* Streamlit Deployment
* FastAPI Deployment
* Clinical Decision Support Integration

---

## 👨‍💻 Author

**Azhar Khan**

M.Tech (Biomedical Engineering)
Indian Institute of Technology Indore (IIT Indore)

---

## 📜 License

This project is released under the MIT License.
