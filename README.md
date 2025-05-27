# 🧠 Childhood Obesity Risk Prediction Tutorial (ML Companion)

This repository provides the code and data accompanying the educational tutorial developed alongside the paper:

**“A Primer for Machine Learning Applications in Childhood Obesity”**

It walks through a complete machine learning (ML) pipeline using synthetic data modeled on real laboratory-based pediatric health assessments, with an emphasis on developmentally appropriate modeling, interpretability, and real-world constraints in childhood obesity research.

---

## 🎯 Who This Is For

- Childhood obesity researchers, stakeholders, and experts in pediatric eating behavior seeking a hands-on starting point for developing machine learning models

No prior experience with machine learning is required, though some familiarity with Python or structured data will be helpful. This tutorial is designed to accompany the manuscript **“A Primer for Machine Learning Applications in Childhood Obesity”**, which provides additional guidance on model development choices.

A [document](ML_childhood_obesity_tutorial.docx) for the tutorial is also available in the repository.


---

## 📚 What's in This Repository

| File/Folder | Description |
|-------------|-------------|
| [ML_modeling_child_obesity.ipynb](ML_modeling_child_obesity.ipynb) | Main Jupyter notebook tutorial: full end-to-end ML pipeline |
| [step1_merge_raw_sources.ipynb](step1_merge_raw_sources.ipynb) | Initial Dataset prep |
| [ML_child_obesity_syn_data.xlsx](ML_child_obesity_syn_data.xlsx) | Input dataset used in tutorial (synthetic pediatric data) |
| `xgb_model_with_bmi.pkl` | Trained model using baseline BMI |
| `xgb_model_without_bmi.pkl` | Trained model using only behavioral and caregiver-report features |
| `xgb_model_combined.pkl` | Final model using both baseline BMI and contextual features |
| `README.md` | This file |

---

## 🧠 Tutorial Objectives

By working through this tutorial, you will learn how to:

- Work with complex pediatric health data (including behavioral, psychological, and caregiver-report variables)
- Handle structured missing data and dropout
- Engineer developmentally meaningful features (e.g., portion response slopes)
- Use stratified splitting and recursive feature selection
- Train interpretable models using SHAP
- Evaluate model performance across scenarios (clinical vs modifiable predictors)

The tutorial demonstrates modeling under two use cases:
1. **BMI-Based Model** (high accuracy, low interpretability)
2. **Behavioral-Only Model** (low accuracy, high interpretability)


---

## 🚀 How to Use This Repo

### 1. Install Required Packages

Create a virtual environment and install dependencies:

```bash
pip install pandas numpy scikit-learn shap matplotlib seaborn openpyxl
```

### 2. Run the Notebooks

Start with [step1_merge_raw_sources.ipynb](step1_merge_raw_sources.ipynb) (optional – for those interested in how the dataset was constructed)

Use [ML_modeling_child_obesity.ipynb](ML_modeling_child_obesity.ipynb) to follow the full ML pipeline
(feature selection, model training and evaluation, post-hoc feature importance through SHAP plots)

### 3. Explore Outputs
Trained models (`.pkl`) can be loaded to skip training

SHAP plots and evaluation outputs are pre-generated for review (find in repo)

---
🔐 Synthetic Data and Raw Source Access
This repository begins from a fully merged synthetic dataset. If you are a researcher or educator who would like access to the original raw synthetic tables (e.g., intake_data, actigraph_raw, qs_cog_psych_soc), please contact:

📧 [ybr5070@psu.edu](mailto:ybr5070@psu.edu) or [klk37@psu.edu](mailto:klk37@psu.edu)

These files are available for non-commercial academic use upon request.

---

📄 License
This repository uses the MIT License for the code.

Note: While the code is openly licensed under MIT, the synthetic dataset and tutorial content are intended for academic, non-commercial use only. Contact the authors if you wish to adapt or redistribute beyond educational purposes.

---

⚠️ Disclaimer
This project uses synthetic, non-identifiable data.
It is provided for educational and training purposes only.
It is not validated for clinical use and should not be used to guide medical decisions.

---

📬 Contact
Yashaswini Rajendra Bhat
PhD Candidate in Nutritional Sciences, Pennsylvania State University
📧 [ybr5070@psu.edu](mailto:ybr5070@psu.edu) 


