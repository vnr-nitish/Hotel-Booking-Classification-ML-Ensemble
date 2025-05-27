# 🏨 Hotel Booking Outcome Classification using Machine Learning  
**Author:** Nitish Raj Vinnakota | 🔗 [LinkedIn](https://linkedin.com/in/vnr-nitish)  
---

## 🔍 Project Overview

This repository contains two machine learning pipelines built on the **Hotel Booking Dataset**, each focused on predicting customer reservation outcomes. These predictions are crucial for hotels to manage cancellations, no-shows, and successful check-outs effectively.

- ✅ **Project 1:** Predict whether a booking will be canceled (Binary Classification)
- ✅ **Project 2:** Predict final reservation status (Multi-Class Classification: Canceled, No-Show, Check-Out)

---

## 🎯 Objective

> To build classification models using both base learners and ensemble methods that accurately predict hotel booking outcomes, enabling data-driven decision-making for the hospitality industry.

---

## 📁 Dataset Summary

- **Source**: hotel_bookings.csv  
- **Records**: ~119,000  
- **Key Features**: Lead time, arrival date, deposit type, customer type, previous cancellations, agent, meal, etc.  
- **Target**:  
  - Project 1: `is_canceled` (0 = Not Canceled, 1 = Canceled)  
  - Project 2: `reservation_status` (Check-Out, Canceled, No-Show)

---

## 🧠 Project 1: Hotel Booking Cancellation Prediction (Binary Classification)

### 🔧 Techniques Used
- Data cleaning, feature engineering
- One-hot encoding & standard scaling
- `train_test_split` and model comparison

### 🧪 Models Applied & Accuracy

| Model               | Accuracy (%) |
|--------------------|--------------|
| Logistic Regression | 79.6         |
| Decision Tree       | 81.2         |
| Random Forest       | 84.1         |
| SVM                 | 82.7         |
| **Bagging**         | 85.4 ✅ (Best Ensemble) |
| AdaBoost            | 84.3         |
| Gradient Boosting   | 85.1         |
| Stacking            | 84.2         |

📌 **Conclusion:**  
Bagging delivered the **highest accuracy** (85.4%) in this binary classification task, slightly outperforming Gradient Boosting.

---

## 🔁 Project 2: Hotel Reservation Status Classification (Multi-Class Classification)

### 🔧 Techniques Used
- Multi-class target: `reservation_status` (Canceled, No-Show, Check-Out)  
- Added `KNN` model  
- Compared ensemble approaches using macro-averaged metrics

### 🧪 Models Applied & Accuracy

| Model               | Accuracy (%) |
|--------------------|--------------|
| Logistic Regression | 76.4         |
| KNN Classifier       | 73.2         |
| Decision Tree       | 78.1         |
| SVM                 | 80.6         |
| Random Forest       | 81.4         |
| AdaBoost            | 82.2         |
| Gradient Boosting   | 84.0         |
| Bagging             | 82.5         |
| **Stacking**        | 86.1 ✅ (Best Ensemble) |

📌 **Conclusion:**  
Stacking produced the **highest accuracy** at 86.1%, showing excellent performance in multi-class classification and outperforming all base and ensemble models.

---

## 📊 Key Takeaways

- Feature engineering and consistent preprocessing significantly impact model performance  
- Ensemble methods like **Bagging (Project 1)** and **Stacking (Project 2)** outperform individual models  
- Evaluation using precision, recall, and F1-score provides deeper insight beyond accuracy  
- Custom pipeline structure ensures reproducibility and scalability

---

## 🚀 Future Improvements

- 🧠 Extend Project 2 with deep learning (ANN or LSTM for sequential bookings)  
- 📈 Add model explainability (e.g., SHAP, LIME)  
- 🧪 Use hyperparameter tuning (`GridSearchCV`, `Optuna`)  
- 🌐 Deploy models using Streamlit or Flask  
- 📊 Integrate dashboards using Power BI or Tableau

---

## 📫 Contact

Feel free to connect or collaborate:

- 📧 **Email:** nvinnako2@gitam.in  
- 🔗 **LinkedIn:** [linkedin.com/in/vnr-nitish](https://linkedin.com/in/vnr-nitish)

---

> *"Empowering decisions with data — one prediction at a time."*
