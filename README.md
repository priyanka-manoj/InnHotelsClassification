# InnHotelsClassification
An end-to-end ML project that aims to explore factors that drive cancellation at INN hotels group and also build predictive models to identify bookings at high risk for cancellation.

# 🏨 Predicting Hotel Booking Cancellations

## 📌 Project Overview

Booking cancellations pose a significant challenge to the hospitality industry, leading to revenue loss from unsold rooms and inefficient resource planning. This project develops and compares multiple machine learning models to predict whether a hotel booking is likely to be cancelled, enabling **INN Hotels Group** to proactively identify high-risk reservations and implement targeted retention strategies.

---

## 🎯 Business Objective

The objective of this project is to build a predictive model that identifies bookings at risk of cancellation before the customer's arrival. The model can help hotels:

- Improve occupancy rates
- Reduce revenue loss due to cancellations
- Optimize customer retention strategies
- Support data-driven operational decisions

---

## 📊 Dataset

The dataset contains historical hotel booking information, including:

- Customer demographics
- Booking characteristics
- Room details
- Pricing information
- Stay duration
- Market segment
- Previous booking behaviour

**Target Variable**

| Variable | Description |
|----------|-------------|
| `booking_status` | 0 = Not Cancelled, 1 = Cancelled |

---

## 🛠️ Project Workflow

- Data Cleaning & Preprocessing
- Exploratory Data Analysis (EDA)
- Outlier Treatment
- Feature Engineering
- Logistic Regression
- Decision Tree Classification
- Hyperparameter Tuning
- Model Evaluation
- Business Recommendations

---

## 📈 Key Insights from EDA

- Longer lead times were associated with higher cancellation rates.
- Online bookings exhibited the highest cancellation behaviour.
- Higher room prices were linked to increased cancellation probability.
- Customers making special requests were less likely to cancel.
- Historical cancellation behaviour emerged as a strong predictor of future cancellations.

---

## 🤖 Models Developed

### Logistic Regression
- Addressed multicollinearity using Variance Inflation Factor (VIF)
- Performed backward feature elimination using p-values
- Optimized the classification threshold using the ROC Curve (Youden's J Statistic)

### Decision Tree Classifier
- Pre-pruning using GridSearchCV
- Post-pruning using Cost Complexity Pruning (`ccp_alpha`)

---

## 📊 Model Evaluation

Models were evaluated using:

- Accuracy
- Recall
- Precision
- F1 Score
- ROC-AUC

The **Optimized Logistic Regression** model was selected as the final model because it achieved the highest **Recall**, making it most suitable for identifying bookings at risk of cancellation while maintaining good overall performance.

---

## 💼 Business Recommendations

- Deploy the model to identify high-risk bookings at the time of reservation.
- Implement proactive retention strategies such as reminder emails, confirmation calls, flexible rescheduling options, or partial prepayment requirements.
- Review pricing strategies for high-priced bookings with elevated cancellation risk.
- Encourage guests to communicate special requests during booking, as these were associated with lower cancellation rates.
- Use predicted cancellation probabilities to prioritize customer intervention efforts.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels

---

## 📁 Repository Structure

```text
.
├── Data/
├── Notebook/
│   └── INN_Hotels_Booking_Cancellation.ipynb
├── Report/
│   └── Project_Report.pdf
├── Images/
└── README.md
```

---

## 🎯 Skills Demonstrated

- Exploratory Data Analysis (EDA)
- Data Cleaning & Feature Engineering
- Logistic Regression
- Decision Trees
- Hyperparameter Tuning
- Model Evaluation
- Threshold Optimization
- Statistical Interpretation
- Business Insight Generation
- Data Storytelling

---

## 🚀 Future Enhancements

- Evaluate ensemble models such as Random Forest and XGBoost.
- Perform cross-validated hyperparameter tuning for cost-complexity pruning.
- Deploy the model as a web application for real-time cancellation risk prediction.

---

## 👤 Author

**Priyanka Manoj**

*PGP in Data Science & GenAI | Aspiring Data Analyst | Passionate about solving business problems using data.*
