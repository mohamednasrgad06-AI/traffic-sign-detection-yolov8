# 🚦 Traffic Sign Detection using YOLOv8

<p align="center">
  <b>Comparative Study of YOLOv8n and YOLOv8m for Traffic Sign Detection</b>
</p>

<p align="center">
  A computer vision project for traffic sign detection, training, evaluation, and model comparison using YOLOv8.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10%2B-blue?logo=python" alt="Python">
  <img src="https://img.shields.io/badge/YOLOv8-Ultralytics-orange" alt="YOLOv8">
  <img src="https://img.shields.io/badge/Computer%20Vision-Object%20Detection-green" alt="Computer Vision">
  <img src="https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter" alt="Jupyter">
</p>

---

## 📌 Overview

Traffic sign detection is an important computer vision task with applications in intelligent transportation systems, driver assistance, road monitoring, and autonomous driving.

This project investigates the performance of two YOLOv8 model variants for traffic sign detection:

- **YOLOv8n (Nano)** — a lightweight model designed for efficiency and lower computational requirements.
- **YOLOv8m (Medium)** — a larger model with higher model capacity and stronger detection performance.

The project focuses on comparing the two models using validation metrics and visual analysis to understand the trade-off between detection performance and model size.

---

## 🎯 Objectives

- Detect traffic signs using deep learning and object detection.
- Train YOLOv8 models on a traffic sign dataset.
- Compare **YOLOv8n** and **YOLOv8m**.
- Evaluate both models using standard detection metrics.
- Visualize model performance and detection outputs.
- Analyze the trade-off between accuracy and computational efficiency.

---

## 🔬 Methodology

```text
Traffic Sign Dataset
        │
        ▼
Data Preparation
        │
        ▼
Preprocessing / Annotation
        │
        ├───────────────┐
        ▼               ▼
   YOLOv8n          YOLOv8m
    Training         Training
        │               │
        └───────┬───────┘
                ▼
          Validation
                │
                ▼
       Performance Metrics
                │
                ▼
        Model Comparison
                │
                ▼
      Detection Visualization
```

---

## 📊 Performance Results

The following values are reported in the model comparison section of the project notebook.

| Metric | YOLOv8m | YOLOv8n |
|---|---:|---:|
| **Precision** | **94.6%** | **91.5%** |
| **Recall** | **92.8%** | **89.5%** |
| **F1-Score** | **93.7%** | **90.5%** |
| **mAP@50** | **97.0%** | **95.1%** |

### 🏆 Best Performing Model

**YOLOv8m achieved the highest value across all four reported metrics.**

| Metric | YOLOv8m Improvement |
|---|---:|
| Precision | **+3.1 percentage points** |
| Recall | **+3.3 percentage points** |
| F1-Score | **+3.2 percentage points** |
| mAP@50 | **+1.9 percentage points** |

> **Metric note:** The F1-Score reported in the notebook is an approximate value calculated from Precision and Recall.

---

## 📈 Evaluation Metrics

- **Precision:** Measures the proportion of detected objects that are correct.
- **Recall:** Measures the proportion of relevant objects successfully detected.
- **F1-Score:** Combines Precision and Recall into a single measure.
- **mAP@50:** Mean Average Precision at an IoU threshold of 0.50.

The notebook includes a dedicated **Performance Comparison** section with visual comparisons of Precision, Recall, F1-Score, and mAP@50.

---

## 🛠️ Tech Stack

| Technology | Role |
|---|---|
| **Python** | Main programming language |
| **YOLOv8** | Object detection models |
| **Ultralytics** | YOLOv8 implementation |
| **PyTorch** | Deep learning framework |
| **OpenCV** | Computer vision and image processing |
| **NumPy** | Numerical computation |
| **Matplotlib** | Visualization |
| **Jupyter / Google Colab** | Experimentation and training |

---

## 📂 Repository Structure

```text
traffic-sign-detection-yolov8/
│
├── notebooks/
│   ├── models/
│   │   ├── results/
│   │   └── README.md
│   └── README.md
│
├── Copy_of_Traffic_Sign_Detection_YOLOv8_ipynb_...ipynb
├── requirements.txt
├── .gitignore
└── README.md
```

---

## 🚀 Installation & Setup

### 1. Clone the repository

```bash
git clone https://github.com/mohamednasrgad06-AI/traffic-sign-detection-yolov8.git
cd traffic-sign-detection-yolov8
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Open the notebook

```bash
jupyter notebook
```

Then open the traffic sign detection notebook and run the cells in order.

---

## 📓 Main Notebook

The main notebook documents the experimental workflow, including:

- Project introduction
- Required library installation
- Dataset preparation
- YOLOv8 model setup
- Training
- Validation
- Performance evaluation
- Model comparison
- Visualization of results

---

## 🔍 Comparative Analysis

### YOLOv8m

**Strengths**
- Highest Precision
- Highest Recall
- Highest F1-Score
- Highest mAP@50
- Stronger overall detection performance

**Trade-off**
- Larger model compared with YOLOv8n.
- Requires more computational resources.

### YOLOv8n

**Strengths**
- Lightweight architecture
- Lower computational requirements
- Suitable when inference efficiency is a priority
- Still achieved strong detection results

**Trade-off**
- Lower reported performance than YOLOv8m across the evaluated metrics.

---

## 💡 Applications

Traffic sign detection can support:

- 🚗 Advanced Driver Assistance Systems (ADAS)
- 🚘 Autonomous driving systems
- 🛣️ Intelligent transportation systems
- 📷 Road and traffic monitoring
- 🚦 Traffic management systems
- 🧠 Computer vision applications

---

## 🔮 Future Work

- Real-time detection using live camera input.
- Deployment on edge devices.
- Model optimization for faster inference.
- Testing additional YOLOv8 variants.
- Expanding and improving the dataset.
- Improving detection of small traffic signs.
- Comparing YOLOv8 with other object detection architectures.
- Evaluating inference speed and resource consumption alongside accuracy.

---

## 📌 Key Takeaway

**YOLOv8m achieved the best reported detection performance:**

> **97.0% mAP@50 · 94.6% Precision · 92.8% Recall · 93.7% F1-Score**

**YOLOv8n achieved:**

> **95.1% mAP@50 · 91.5% Precision · 89.5% Recall · 90.5% F1-Score**

Therefore, **YOLOv8m is the stronger choice when detection performance is the main priority**, while **YOLOv8n offers a lighter alternative when computational efficiency is more important**.

---

## 👨‍💻 Author

**Mohamed Nasr Gad**

Artificial Intelligence / Machine Learning

GitHub: https://github.com/mohamednasrgad06-AI

---

## 📜 License

This project is intended for educational and research purposes.
