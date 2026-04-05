# Samaan-Ensemble
Adaptive routing-based ensemble model for per-sample ML model selection

# SAMAAN Ensemble (Sample-Adaptive Artificial Network Ensemble)

This repository presents the implementation of the **SAMAAN Ensemble**, a novel adaptive machine learning framework designed to improve classification performance by dynamically selecting the most suitable model for each input sample.

## 📌 Overview

Traditional machine learning approaches rely on a single model or static ensemble techniques such as averaging or majority voting. These methods assume that a single decision boundary can generalize across all data instances.

The proposed **SAMAAN Ensemble** addresses this limitation by introducing a **routing-based architecture**, where a meta-level decision tree selects the most appropriate base classifier for each input instance. This enables **per-sample model selection**, allowing the system to adapt to heterogeneous data patterns.

---

## ⚙️ Methodology

The framework consists of two main components:

### 1. Base Models
The following machine learning models are trained independently:
- Logistic Regression  
- Random Forest  
- K-Nearest Neighbors (KNN)  
- XGBoost  

Each model captures different characteristics of the data.

### 2. Adaptive Routing Mechanism
A Decision Tree is used as a **router** to:
- Analyze input features  
- Predict the best-performing model  
- Route the input to the selected classifier  

---

## 🔁 Workflow
Input Data → Router (Decision Tree) → Selected Model → Prediction


---

## 📊 Results

The proposed SAMAAN Ensemble achieves:

- **Accuracy:** 84.26%  
- **Precision:** 0.841  
- **Recall:** 0.834  
- **F1-Score:** 0.842  
- **ROC-AUC:** 0.914  

These results outperform baseline models, demonstrating the effectiveness of adaptive model selection.

---

## 📁 Dataset

The model is trained on a student depression dataset containing:
- Demographic features (Age, Gender, City)
- Academic indicators (CGPA, Academic Pressure)
- Lifestyle factors (Sleep Duration, Work/Study Hours, Diet)
- Psychological indicators (Suicidal Thoughts, Family History)

---

## 💡 Key Contribution

Unlike traditional ensemble methods, the SAMAAN Ensemble:
- Performs **dynamic per-sample model selection**
- Adapts to **heterogeneous datasets**
- Provides **interpretable routing decisions**
- Combines strengths of multiple ML models without averaging

---

## 🚀 Future Improvements

- Integration with deep learning models  
- Multi-class classification support  
- Deployment as a real-time prediction system  

---

## 👩‍💻 Author

**Sampoorna Chakraborti**  
KIIT Deemed to be University  
