## Auditing Emotion Recognition Bias Against Neurodiverse Individuals
> A fairness audit of commercial and open-source emotion recognition systems, examining systematic bias against neurodiverse individuals — grounded in EU Trustworthy AI guidelines.
---
## Motivation

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
| Dataset | Description |
|---------|-------------|
| RAF-DB | Real-world affective faces, 7 basic emotions |
| AffectNet | Large-scale annotated facial affect |
| FER-2013 | Benchmark facial expression recognition |
| FER-Autism | Facial expressions from autistic individuals |

### Models Evaluated
| Model | Type |
|-------|------|
| DeepFace | Deep CNN ensemble |
| EmotiEffLib | EfficientNet-based |

---

## Evaluation Methodology

### Performance and Reliability
- Top-1 and Top-3 accuracy  
- Per-class F1-score  
- Expected Calibration Error (ECE)  
- Reliability diagrams  
- Confusion Matrices
  
### Explainability and Robustness
- Grad-CAM for visual attention analysis  
- Occlusion sensitivity testing (eyes, mouth, nose regions)  
- Counterfactual explanations using LIME  

### Ethical Analysis
- Qualitative analysis of attention patterns and decision logic  
- Alignment with EU Trustworthy AI guidelines  
- Identification of risks related to exclusion, misrepresentation, and misuse  

---
## Key Findings

- Both models show measurable accuracy drops on the FER-Autism dataset compared to neurotypical benchmarks
- Grad-CAM analysis reveals that models frequently attend to mouth and eye regions — features that are expressed atypically in many neurodiverse individuals
- Calibration error increases significantly on neurodiverse samples, indicating overconfident misclassifications
- A systematic bias risk was identified for deployment in hiring and education contexts

---

## Repository_structure:
  - notebooks/
    - qualitative_analysis/      # Grad-CAM, occlusion, LIME notebooks
    - quantitative_analysis/     # Accuracy, F1, ECE evaluation notebooks
  - report                       # Full technical report
  - README.md


---

## Output

- Final report (PDF)  
- Reproducible evaluation and explainability code  
- Fairness auditing checklist for emotion recognition systems  

---

## Team

- **Luwam Major Kefali** – Explainability (Grad-CAM, LIME), occlusion analysis, pipelines
- **Hassen Said Ali** – Model benchmarking, evaluation metrics, pipelines  
- **Hilina Fissha Woreta** – Ethical analysis and auditing checklist  

---
