# Lab 05: Convolutional Neural Networks (CNNs) — "Chihuahua or Muffin" Workshop

**Course:** ITAI 1378  
**Topic:** Convolutional Neural Networks, Hyperparameter Tuning, & Model Comparison  
**Repository:** [patitimoner/workshop-chihuahua-vs-muffin](https://github.com/patitimoner/workshop-chihuahua-vs-muffin)

## 📋 Overview

This lab builds on the Chihuahua vs. Muffin classification task using **Convolutional Neural Networks (CNNs)** (`CNN_1 Chihuahua or Muffin.ipynb`). You will complete missing code placeholders, run experiments adjusting epochs, learning rate, and architecture, compare CNN performance against the traditional neural network from Lab 04, and document your findings in a reflective journal.

## 🚀 Environment Setup

### Option A: Google Colab
1. Open [Google Colab](https://colab.research.google.com/) and sign in.
2. Go to **File > Open notebook > GitHub**, search for `patitimoner/workshop-chihuahua-vs-muffin`, and select `CNN_1 Chihuahua or Muffin.ipynb`.
3. Run the setup cell at the top:
   ```python
   !git clone https://github.com/patitimoner/workshop-chihuahua-vs-muffin.git
   %cd workshop-chihuahua-vs-muffin
   !ls
   ```

### Option B: Amazon SageMaker Studio Lab
1. Sign in to [Amazon SageMaker Studio Lab](https://studiolab.sagemaker.aws/) and start a runtime.
2. Open a terminal and clone the repository:
   ```bash
   git clone https://github.com/patitimoner/workshop-chihuahua-vs-muffin.git
   cd workshop-chihuahua-vs-muffin
   ```
3. Open `CNN_1 Chihuahua or Muffin.ipynb` from the file browser.

## 🧪 Workflow & Experiments

1. **Complete & Run Code:** Fill in missing imports and replace `?` placeholders, then run cells sequentially and comment any changes.
2. **Hyperparameter & Architecture Experiments:** Test variations in:
   * Number of epochs
   * Learning rate
   * Model layers/architecture
3. **Analyze & Compare:** Record accuracy, misclassification patterns, and training time compared to the traditional neural network from Lab 04.

## 📦 Deliverables

| Deliverable | Format | Naming / File |
| :--- | :--- | :--- |
| **Completed Notebook** | `.ipynb` or `.html` | `Lab05_CNN_Chihuahua_Muffin.ipynb` (all outputs visible) |
| **Reflective Journal** | `.pdf` or Word | `L05_YourName_ITAI_1378` (1–2 pages with citations) |

### Reflective Journal Topics
* **CNN Architecture:** How it works and how it differs from Lab 04's traditional neural network.
* **Model Performance:** Accuracy results and notable misclassification patterns.
* **Comparison:** Performance and training time vs. the traditional neural network.
* **Challenges & Solutions:** Issues encountered and how you solved them.
* **Real-World Applications & Ethics:** Practical use cases, ethical considerations, and supporting references.