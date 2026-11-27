# Module 3: Machine Learning Foundations for Computer Vision

## Lab 03b: Image Classification with Support Vector Machines (SVM)

### 📋 Overview
This lab introduces classical machine learning algorithms applied to visual recognition tasks. Using the CIFAR-10 dataset, the project covers the full machine learning pipeline—from data preprocessing (grayscale conversion and vector flattening) to training a Support Vector Machine (SVM) classifier and evaluating its predictive accuracy.

---

### 🎯 Learning Objectives
* Understand how Support Vector Machines (SVM) classify visual data.
* Preprocess image datasets for classical machine learning algorithms.
* Evaluate classification performance using accuracy metrics and confusion visualizations.
* Critically analyze the limitations of classical ML compared to deep learning methods for visual recognition.

---

### 🛠️ Tech Stack & Tools
* **Language:** Python
* **Environment:** Jupyter Notebook / Google Colab / Studio Lab
* **Libraries:** `scikit-learn`, `numpy`, `matplotlib`, `tensorflow` (for dataset loading)

---

### 📊 Dataset: CIFAR-10
* **Classes (10):** Airplane, Automobile, Bird, Cat, Deer, Dog, Frog, Horse, Ship, Truck.
* **Format:** $32 \times 32$ color images.
* **Preprocessing Pipeline:**
  1. Load CIFAR-10 visual samples.
  2. Convert 3-channel RGB images to 1-channel Grayscale.
  3. Flatten $32 \times 32$ matrices into 1D feature vectors ($1024$ features).
  4. Train/Test split and feature scaling.

---

### 📁 Required Deliverables & Naming Convention

| Deliverable | File Format | Naming Format |
| :--- | :--- | :--- |
| **Lab Notebook** | Jupyter Notebook (`.ipynb`) | `L03b_LastName_FirstName_ITAI1378.ipynb` |
| **Reflective Journal** | PDF (`.pdf`) | `L03_StudentName_ITAI_1378.pdf` |

#### Reflective Journal Structure:
1. **Reflection on Learning:** Understanding of SVM principles, data prep steps, and performance insights.
2. **Lab Questions:** Detailed answers to all inline notebook questions.
3. **Visual Evidence:** Embedded code outputs, loss curves, and prediction grids.
4. **Critical Analysis & Citations:** Discussion on classical ML tradeoffs with proper APA/IEEE in-text citations and references.