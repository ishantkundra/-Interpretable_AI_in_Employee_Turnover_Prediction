🧠 Project Overview
	•	Course: CSCE 689 – Special Topics in Human-AI Interaction
	•	Title: Interpretable AI in Employee Turnover Prediction
	•	Focus: Using LIME and SHAP to explain model predictions and assess fairness
	•	Model: Random Forest Classifier
	•	Dataset: Employee attrition dataset
	•	XAI Techniques: LIME (local), SHAP (global)
	•	Insights: Feature influence, calibration, bias by age/gender, compute time comparison

⸻

📦 Suggested Repository Name

You can go with:
	•	lime-shap-employee-explainability
	•	interpretable-ai-turnover
	•	xai-employee-attrition
	•	✅ Recommended: employee-attrition-xai-lime-shap

⸻

📝 GitHub-Ready README.md with <pre> Structure

# Explainable AI for Employee Turnover Prediction: LIME vs SHAP

This project explores **interpretable AI techniques** to explain the predictions of a Random Forest model trained on employee attrition data. Using **LIME** (Local Interpretable Model-agnostic Explanations) and **SHAP** (SHapley Additive exPlanations), the study compares local and global feature attributions and analyzes model fairness with respect to **age** and **gender**.

Developed as part of **CSCE 689: Human-AI Interaction** at **Texas A&M University**.

---

## 📁 Repository Structure

<pre>
employee-attrition-xai-lime-shap/
│
├── Code/                      # Jupyter Notebook with full implementation
│   └── CSCE 689 Human AI - Interaction HW- 02 ISHANT KUNDRA.ipynb
│
├── Report/                    # Final PDF report with visualizations and analysis
│   └── CSCE 689- Ishant Kundra.pdf
│
├── Dataset/                   # Employee attrition dataset
│   └── Employee.csv
│
├── Problem_Questtion/                # Original assignment brief for reference
│   └── Assignment 2.pdf
│
└── README.md                  # You’re here!
</pre>

---

## 📌 Project Goals

- Train a machine learning model (Random Forest) to predict employee attrition
- Apply LIME and SHAP for model interpretation
- Visualize feature influences and compare explanations
- Evaluate fairness of predictions across **age** and **gender**
- Compare **execution time** and effectiveness of LIME vs SHAP

---

## 🧪 Methodology

- Data preprocessing & encoding of categorical features
- Split: 70% train / 30% test
- RandomForestClassifier from `sklearn`
- Feature importance measured via:
  - LIME (individual predictions)
  - SHAP (global impact)

---

## 📊 Key Results

- **LIME**: Explained individual predictions (e.g., influence of `City`, `Education`, `JoiningYear`)
- **SHAP**: Global feature importance showed `JoiningYear` and `PaymentTier` as key predictors
- **Bias Analysis**:
  - Higher attrition prediction for <30 age group and females
  - Calibration curve issues for older employees and females
- **Time Comparison**:
  - LIME: ~0.23 seconds (fast, instance-level)
  - SHAP: ~13.8 seconds (slower, global-level)

---

## 🧠 Insights

| Technique | Type       | Speed      | Best For                    |
|-----------|------------|------------|-----------------------------|
| LIME      | Local      | Very Fast  | Real-time decisions         |
| SHAP      | Global     | Slower     | Audits, fairness evaluation |

Both are **model-agnostic**, powerful tools for explainability.

---

## 📈 Visuals Included

- LIME bar charts for instance-level interpretation
- SHAP summary plots for global feature impact
- Calibration curves for fairness across groups

---

## ⚙️ Tools & Libraries

- Python
- Scikit-learn
- LIME
- SHAP
- Pandas, Matplotlib

---

## 👨‍💻 Author

**Ishant Kundra**  
M.S. Computer Science, Texas A&M University  
📬 [ishantkundra9@gmail.com]

