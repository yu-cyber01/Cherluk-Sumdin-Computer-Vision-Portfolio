# Lab 08: Vision Transformers and VLMs — Talking to Your Images

**Course:** ITAI 1378 – Computer Vision | **Model:** `SmolVLM-500M-Instruct` | **Platform:** Google Colab

## Overview

This lab explores how Vision Transformers (ViTs) process images as patch sequences and how a compact Vision-Language Model (`SmolVLM-500M-Instruct`) handles visual question answering, accessibility alt text, chart reading, hallucination testing, and workplace reliability auditing through prompting.

## Key Topics & Activities

* **Vision Transformer Patches:** Resized images to `384 × 384` and compared `48px` vs. `96px` patch grids to examine detail vs. computational trade-offs.
* **Image Interview & Multi-Task Prompting:** Tested progressive difficulty questions and used constrained prompts for classification, counting, and object/text extraction.
* **Accessibility Alt Text:** Compared generic prompts against structured alt-text prompts for screen-reader usability and identified details requiring human review.
* **Chart Reading & Hallucination Audit:** Evaluated accuracy against ground-truth chart values, tested false-assumption trap questions, and audited consistency across prompt phrasings for a workplace deployment recommendation.

## Deliverable

* **Notebook:** `L08_LastName_FirstName_ITAI1378.ipynb` (executed with all outputs visible)
