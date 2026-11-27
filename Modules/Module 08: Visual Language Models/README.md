# Lab 08: Vision Transformers and VLMs — Talking to Your Images

**Course:** ITAI 1378 – Computer Vision  
**Platform:** Google Colab (Free T4 GPU recommended; CPU fallback supported)  
**Model:** `SmolVLM-500M-Instruct`  
**Estimated Duration:** ~3–4 hours  
**Points:** 100 points total (up to 20 optional bonus points)

## Overview

In this lab, you explore how Vision Transformers (ViTs) divide images into fixed-size patches and how a compact open-weight Vision-Language Model (`SmolVLM-500M-Instruct`) handles visual question answering, accessibility alt text, chart reading, hallucination testing, and workplace reliability auditing through prompting. Unlike single-task specialist models, a VLM can switch tasks by changing the prompt.

## Learning Objectives

By completing this lab, you will be able to:

1. Explain how a Vision Transformer processes an image as a sequence of patches.
2. Visualize an image using different ViT patch sizes.
3. Use a VLM for image captioning and visual question answering.
4. Use prompting to make one model classify, count, read, and describe image content.
5. Write effective prompts for accessibility alt text.
6. Test a VLM's ability to read charts and numerical information.
7. Identify and document VLM hallucinations.
8. Evaluate a VLM using known ground-truth information.
9. Test the consistency of a VLM across differently worded prompts.
10. Write a professional recommendation about whether a VLM should be deployed for a workplace task.

## File Naming Convention & Submission

* **Required File:** `L08_LastName_FirstName_ITAI1378.ipynb` (example: `L08_Smith_John_ITAI1378.ipynb`)
* **Submission Format:** Only the completed `.ipynb` notebook is submitted to Canvas (do not submit a PDF instead of the notebook).
* **Before Submitting:**
  * Run **Runtime → Run all** and confirm there are no unresolved errors.
  * Ensure all required code, outputs, and `YOUR ANSWER` / `YOUR TURN` sections are complete and visible.
  * Check for leftover `TODO` or `replace` placeholders.
  * Do not clear notebook outputs before downloading and submitting.

## Getting Started

1. Download the Lab 08 notebook from Canvas, upload it to Google Colab, and rename it to `L08_LastName_FirstName_ITAI1378.ipynb`.
2. Go to **Runtime → Change runtime type** and select **T4 GPU** when available (CPU fallback works, though responses take longer). The model download is ~1 GB and uses ~1 GB of GPU memory; try to finish in one session so it stays cached.
3. Run the setup cells to install Hugging Face libraries and verify hardware (`GPU ready: [GPU name]` or `CPU fallback active...`) and model loading (`VLM loaded. Say hello:`).
4. Follow notebook markers carefully:
   * `RUN AS IS`: Run and study the existing cell.
   * `YOUR CODE HERE`: Complete code where marked by `TODO`.
   * `YOUR ANSWER`: Replace placeholder markdown with your written response.
   * `YOUR TURN`: Complete graded checkpoints with code, prompts, outputs, and analysis.
   * `Try It Yourself`: Mini-project with minimal starter code.

## Lab Structure & Deliverables

### Implementation (60 Points)

* **Section 1 – Environment Setup:** Install libraries, verify GPU/CPU detection, and run setup cells with visible output.
* **Section 2 – Seeing Like a Vision Transformer (10 pts):** Choose a non-sample image, resize it to `384 × 384` pixels, display patch grids at `48px` and `96px`, and explain how patch size affects detail and compute using an image or sentence analogy.
* **Section 3 – Load the VLM and Interview an Image (10 pts):** Use `ask(image, question)` on one image with three questions of increasing difficulty (1. easy factual; 2. detail such as color, position, count, or background; 3. reasoning about mood, unusual features, or what might happen next). Print each question with its answer and write a 2–3 sentence analysis of the weakest answer and why it was harder.
* **Section 4 – One Model, Many Jobs (10 pts):** Use constrained prompts on the same VLM for classification, counting, and reading/describing (e.g., *"Answer with one word only."*, *"Answer with just a number."*, *"List one object per line."*). Include a written comparison highlighting one advantage of a specialist model (such as YOLO) and one advantage of a VLM.
* **Section 5 – Workforce Task A: Accessibility Alt Text (10 pts):** Generate alt text for the sample cat image and one additional image using both a weak prompt (`Describe this image.`) and a custom professional prompt (concise, specific, screen-reader friendly, 1–2 sentences, not starting with *"an image of"*). Label all four outputs, add a 2–3 sentence comparison, and note what still requires human review before publishing.
* **Section 6 – Workforce Task B: Reading Documents and Charts (10 pts):** Ask at least three questions about the generated sales bar chart—including a specific value, a max/min, and a comparison between at least two bars/months. Display model answers alongside ground-truth values, report accuracy/score, and write a 2–3 sentence recommendation on unsupervised trust.
* **Section 7 – Hallucination Hunt (10 pts):** Create two original trap questions (not copied from notebook examples) containing false assumptions (e.g., non-existent objects, text, or trends). Run both on the cat image and the sales chart (four exchanges total), then write a 3–4 sentence hallucination report explaining why hallucinations can be riskier in the workplace than a simple counting error.
* **Section 8 – Preview: The Agent's Eyes:** Execute the preview cell moving from perception to action recommendation (bridge to Module 09; not separately graded).

### Analysis (40 Points)

* **Section 9 – Try It Yourself: VLM Deployment Audit (20 pts):** Act as a junior CV technician evaluating a VLM for a chosen workplace scenario (Retail, Safety, Accessibility, Education, or a clearly explained custom scenario):
  * **Part 1 – Scenario & Test Set (5 pts):** Define the scenario and gather 2–3 fitting test images (following privacy/safety rules—no identifiable people or confidential workplace data).
  * **Part 2 – Reliability Test (5 pts):** Ask the same task question in three different phrasings, print each prompt next to its response, and compare consistency.
  * **Part 3 – Audit Memo (10 pts):** Write a 5–8 sentence memo covering what you tested, what worked, what failed or was inconsistent, one scenario-specific hallucination risk, and an evidence-backed recommendation (*Deployment with human review*, *Unsupervised deployment*, or *No deployment*).
* **Section 10 – Final Reflection Questions (20 pts, 2 pts each):** Answer all 10 reflection questions in complete sentences in your own words with specific references to your lab experiments (no short bullet-point answers):
  1. Image patches and Vision Transformers
  2. Vision encoder, projector, and language model
  3. Prompt-based task selection
  4. Constrained model outputs
  5. Small local models versus frontier models
  6. Accessibility and alt-text ethics
  7. Ground-truth evaluation
  8. Errors versus hallucinations
  9. Evidence-based auditing
  10. How the lab changed your understanding of image AI

## Grading Rubric

| Category | Component | Points |
| :--- | :--- | :---: |
| **Implementation** | ViT patch-grid experiment and explanation | 10 |
| | Interview an image | 10 |
| | One model, many jobs | 10 |
| | Accessibility alt text | 10 |
| | Chart reading and accuracy evaluation | 10 |
| | Hallucination hunt | 10 |
| **Analysis** | Independent deployment audit | 20 |
| | Ten reflection questions (2 pts each) | 20 |
| **Total** | | **100** |

* **Grading Notes:** Working code earns full credit regardless of minor structural differences from scaffolding. Model errors or messy outputs do not lose points when honestly documented and analyzed. There is no deduction for late submission.

## Optional Bonus Challenges (Up to 20 Bonus Points Max)

* **Bonus A – The Tiny Sibling (+5):** Load `HuggingFaceTB/SmolVLM-256M-Instruct`, repeat the three image-interview questions, and explain in 1–2 sentences what quality/performance was lost.
* **Bonus B – Receipt Reader (+5):** Use `PIL` and `ImageDraw.text` to generate a synthetic receipt (store name, 3 items, 3 prices, total) and compare extracted values against ground truth.
* **Bonus C – Patch-Size Probe (+5):** Test an image with a small detail (such as text or a small object) at `96px` patches, ask about the detail, and relate the patch grid to the model's answer.
* **Bonus D – Your Own Photo Set (+5):** Complete the deployment audit using your own original photos (no identifiable people) and identify the relevant cells.

*(If running bonus models causes memory issues, finish required sections first, delete/clear the previous model from memory, and then load the bonus model.)*

## Troubleshooting

* **GPU unavailable:** Continue on CPU fallback or retry selecting a T4 GPU in Colab runtime settings.
* **Slow responses:** Run one question at a time and avoid unnecessary repeated calls.
* **Setup/model load errors or runtime disconnects:** Restart the runtime, reselect T4 GPU if available, and run cells sequentially from the top.
* **Image open errors:** Verify the file is uploaded to Colab and check the path/filename; resize images to `384 × 384` if patch grid dimensions do not divide evenly.
* **Verbose responses:** Add output constraints such as *"one sentence,"* *"one word,"* or *"just the number."*

## Academic Integrity & Responsible Image Use

* Write reflections, analyses, and audit memos in your own words based on your own prompts and observations.
* AI tools may be used to help debug technical code errors, not to generate your reflections or audit judgments.
* Only use images you created, photographed, or have permission to use; do not upload photos of identifiable people or private/confidential workplace information.
