# Lab 04: Neural Networks Fundamentals — "Chihuahua or Muffin" Workshop

**Course:** ITAI 1378  
**Topic:** Image Classification, Convolutional Neural Networks (CNNs), & Transfer Learning  
**Repository:** [patitimoner/workshop-chihuahua-vs-muffin](https://github.com/patitimoner/workshop-chihuahua-vs-muffin)

---

## 📋 Overview

In this workshop lab, you will explore the classic computer vision classification challenge: distinguishing between images of **Chihuahuas** and **Muffins**. The lab focuses on setting up a cloud environment (Google Colab or AWS SageMaker Studio Lab), cloning the workshop repository, training/evaluating image classification models, and writing a comprehensive reflective journal supported by academic citations.

---

## 🚀 Environment Setup Instructions

### Option A: Google Colab
1. Go to [Google Colab](https://colab.research.google.com/) and sign in.
2. Select **File** > **Open notebook** > **GitHub** tab.
3. Search for the repository: `patitimoner/workshop-chihuahua-vs-muffin`.
4. Open `workshop_1.ipynb`.
5. Run the setup cell at the top of the notebook:
   ```python
   !git clone https://github.com/patitimoner/workshop-chihuahua-vs-muffin.git
   %cd workshop-chihuahua-vs-muffin
   !ls
   ```
6. *(Optional)* Mount Google Drive to preserve work:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```

### Option B: AWS SageMaker Studio Lab
1. Sign in to [AWS SageMaker Studio Lab](https://studiolab.sagemaker.aws/).
2. Start the runtime and click **Open project**.
3. Open a **Terminal** from the launcher and execute:
   ```bash
   git clone https://github.com/patitimoner/workshop-chihuahua-vs-muffin
   cd workshop-chihuahua-vs-muffin
   ```
4. Open `Workshop_1.ipynb` from the left file navigator.

---

## 📦 Deliverables & File Naming Conventions

All submitted files must strictly adhere to the following naming rules:

| Deliverable | Format Options | Required Naming Structure | Description |
| :--- | :--- | :--- | :--- |
| **Reflective Journal** | PDF (`.pdf`) | `L04_FirstName_LastName_ITAI_1378.pdf` | 1–2 page single-spaced synthesis with citations |
| **Completed Notebook** | `.ipynb` or `.html` | `Workshop_1.ipynb` (or custom per instructions) | Executed notebook showing all code outputs |

---

## 📝 Reflective Journal Requirements

The reflective journal must be **1–2 pages (single-spaced, 12pt font, standard margins)** covering:

1. **Workshop Objectives & Methods:** Summary of the primary goals and techniques implemented.
2. **Key Concepts Learned:** Explanations of Convolutional Neural Networks (CNNs), feature extraction, and Transfer Learning.
3. **Challenges & Solutions:** Specific obstacles faced during data prep or model execution and how they were resolved.
4. **Insights & Real-World Applications:** Broad takeaways on vision model behavior and practical deployment scenarios.
5. **Citations & References:** Formal academic/technical citations (APA/IEEE style) supporting technical concepts.

---

## 📊 Grading Criteria

* **Notebook Completeness (Execution & Correctness):** All code cells executed sequentially with output clear and visible.
* **Reflection Depth:** Demonstrates genuine technical understanding beyond surface summary.
* **Academic Citations:** Correct usage of in-text citations and a matching reference section.
* **Compliance:** Strict adherence to submission formatting, page limits, and file naming rules.