A Machine Learning-Based Framework for Digital Addiction Risk Prediction with Integrated Health and Academic Performance Analysis among Teenagers

Overview

This project presents a data-driven machine learning framework to predict digital addiction risk among teenagers using behavioral, health, and academic indicators.

The system integrates a classification model with a health-risk assessment layer to provide both prediction and interpretability for real-world use in educational and counseling environments.

Objectives

* Predict digital addiction risk (Low, Moderate, High)
* Analyze relationships between screen usage, sleep, and academic performance
* Identify key behavioral indicators influencing addiction
* Estimate associated health risks (eye strain, depression, sleep disorders, anxiety)

 Dataset

* Sample Size: 125 teenagers (age 13–19)
* Data Source: Survey-based questionnaire
* Features Used:
  * Daily screen time
  * Social media usage
  * Pre-sleep phone usage
  * Phone checking frequency
  * Sleep duration
  * Academic concentration difficulty

 Methodology
 1. Data Preprocessing

* Removal of missing values
* Label encoding of categorical features
* Feature normalization
* Construction of composite addiction score

 2. Classification Models

* Random Forest (Best Performer)
* Logistic Regression
* Decision Tree
* Support Vector Machine (RBF Kernel)

 3. Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1 Score

Results

| Model               | Accuracy |
| ------------------- | -------- |
| Random Forest       | **75%**  |
| Logistic Regression | 62.5%    |
| SVM (RBF)           | 62.5%    |
| Decision Tree       | 37.5%    |

 Key Findings

* Random Forest achieved the highest performance
* Concentration difficulty is the most important feature
* Screen time and sleep duration strongly influence addiction risk
* Moderate-risk group shows overlap with both low and high-risk users

Health Risk Assessment Module

A weighted scoring system estimates:

*  Eye Health Risk
*  Depression Risk
*  Sleep Disorder Risk
*  Anxiety Risk

Formula:

Health Risk % = (w₁F₁ + w₂F₂ + w₃F₃ + w₄F₄) × 100

Insights:

* Depression risk ≈ 60% (highest)
* Sleep disorder risk ≈ 50%
* Anxiety risk ≈ 28%
* Eye health risk ≈ 20%

Visualizations

* Confusion Matrix
* Feature Importance Graph
* Correlation Heatmap
* Model Comparison Chart
* Health Risk Distribution

 How to Run

```bash
git clone https://github.com/Yogita5002/digital-addiction-risk-ml.git
cd digital-addiction-risk-ml
pip install -r requirements.txt
jupyter notebook
```

 Research Paper

Included in the `/reports` folder.


 Limitations

* Small dataset (125 samples)
* Self-reported data may introduce bias
* Moderate-risk classification boundary is less accurate

 Future Work

* Larger multi-institution dataset
* Integration of real device usage data
* Use of deep learning models (RNNs, Gradient Boosting)
* Explainability using SHAP

 Author

Yogita.Y.V
SRM Institute of Science and Technology
