# Lab 06: Object Detection and Image Segmentation

**Course:** ITAI 1378 – Computer Vision  
**Estimated Time:** 2–3 hours  
**Platform:** Google Colab  
**Total Points:** 100 points (60 pts Implementation + 40 pts Reflection; up to +10 bonus points)

## 📋 Overview

This lab covers modern object detection and instance segmentation using **YOLO11**, **YOLO11-seg**, and **SAM 2** (Segment Anything Model 2). You will compare specialist detectors with foundation segmentation models, explore confidence thresholds and evaluation metrics (IoU, precision, recall, mAP), and outline a midterm project idea.

## 🚀 Setup & Workflow

1. Upload the lab `.ipynb` notebook to [Google Colab](https://colab.research.google.com/) and run cells sequentially (`Shift + Enter`).
2. Complete Sections 1–7, including custom-image tests (**Your Turn 1 & 2**), confidence threshold comparisons, YOLO11-seg masks, a YOLO + SAM 2 detect-then-segment pipeline, and IoU visualization.
3. Review midterm project options (Section 8) and answer all 10 reflection questions (Section 9), including a midterm project pitch in Question 10 (2–4 sentences per question).

## 📦 Deliverables & Grading

* **Completed Notebook (`.ipynb`):** Executed top-to-bottom with all outputs visible, using a custom image in Your Turn 1 & 2.
* **Reflection Answers (40 pts):** Written in notebook markdown cells (preferred) or a separate `.pdf` file.
* **Bonus Opportunities (up to +10 pts max):**
  * Larger YOLO11 variant comparison (`+3`)
  * YOLO-World open-vocabulary detection (`+3`)
  * SAM 2 vs. SAM 3 comparison (`+2`)
  * Fine-tuning YOLO11 on a small custom dataset (`+5`)