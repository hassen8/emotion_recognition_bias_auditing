# Smile ≠ Happy  
## Auditing Emotion Recognition Bias Against Neurodiverse Individuals

Emotion recognition systems are increasingly used in hiring, education, and healthcare. However, most of these models are trained on **neurotypical facial expressions**, which can lead to systematic misclassification or exclusion of **neurodivergent individuals**, particularly those on the autism spectrum.

This project audits the **fairness, robustness, and ethical risks** of facial emotion recognition systems when applied to diverse expression styles and proposes a **lightweight auditing protocol** for more inclusive emotion AI.

---

## Project Objectives

- Evaluate how facial emotion recognition models generalize to neurodivergent expression patterns  
- Identify bias and failure modes using explainability and robustness analysis  
- Analyze whether model attention aligns with known neurodiverse expression traits  
- Propose a practical, ethics-driven auditing checklist for emotion AI systems  

---

## Models and Datasets

### Datasets
- RAF-DB  
- AffectNet  
- EmotioNet  

### Models Evaluated
- FER+  
- DeepFace  
- EmotiEffLib 

All evaluations are performed on **unaltered, real-world images** to reflect realistic deployment conditions.

---

## Evaluation Methodology

### Performance and Reliability
- Top-1 and Top-k accuracy  
- Per-class F1-score  
- Expected Calibration Error (ECE)  
- Reliability diagrams  

### Explainability and Robustness
- Grad-CAM for visual attention analysis  
- Occlusion sensitivity testing (eyes, mouth, nose regions)  
- Counterfactual explanations using LIME  

### Ethical Analysis
- Qualitative analysis of attention patterns and decision logic  
- Alignment with EU Trustworthy AI guidelines  
- Identification of risks related to exclusion, misrepresentation, and misuse  

---

## Repository_structure:
  - data/
  - models/
  - explainability/
  - evaluation/
  - notebooks/
  - audit_checklist/
  - report/
  - README.md


---

## Deliverables

- Final report (PDF)  
- Reproducible evaluation and explainability code  
- Fairness auditing checklist for emotion recognition systems  

---

## Team

- **Luwam Major Kefali** – Explainability (Grad-CAM, LIME), occlusion analysis, pipelines
- **Hassen Said Ali** – Model benchmarking, evaluation metrics, pipelines  
- **Hilina Fissha Woreta** – Ethical analysis and auditing checklist  

---

## Motivation

Emotion recognition models influence real decisions about people.  
If a system cannot handle expression diversity, it should not be trusted in high-stakes settings.

This project focuses on **auditing, explainability and accountability**, not on building new emotion classifiers.


