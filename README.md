# Hotel Booking Cancellation Prediction

A machine learning project that predicts the likelihood of hotel booking cancellations
using customer, reservation, and behavioral features. The goal is to help hotels improve
forecasting, reduce revenue loss, and design more effective retention strategies.

This repository contains a cleaned and refactored version of a group project originally
developed for **Boston University – QST 576: Machine Learning for Business Analytics**, adapted
here as a standalone portfolio project. Note: for easiest use, follow the link to open the notebook in
colab and update the file path. 

---

## 📌 Problem Statement

Hotel cancellations lead to:
- Lost revenue
- Inefficient room utilization
- Overstaffing or understaffing risks

Using historical booking data, this project models **cancellation probability** and identifies
the most important drivers behind customer cancellations.

---

## 📊 Dataset

- **Source:** Hotel Booking Demand dataset (Kaggle)
- **Scope:** ~119,000 reservations (2015–2017)
- **Hotels:** City & Resort hotels in Portugal
- **Target Variable:** `is_canceled`

Features include:
- Lead time
- Length of stay
- Special requests
- Booking changes
- Customer and market segment attributes

---

## 🔍 Exploratory Insights

Key findings from EDA:
- Longer **lead times** are strongly associated with higher cancellation rates
- Guests with **special requests** are less likely to cancel
- Previous cancellations are a strong predictor of future behavior

(Selected figures and visualizations are included in `docs/figures/`.)

---

## 🤖 Models Implemented

The following models were trained and evaluated:

- Logistic Regression (Lasso & Ridge)
- Decision Tree
- Random Forest
- K-Nearest Neighbors (KNN)
- Gradient Boosting
- Neural Network (MLP)

### Best Performing Models
- **Random Forest**
  - Test Accuracy ≈ 79%
  - Strong performance across precision, recall, and F1
- **Neural Network**
  - Test Accuracy ≈ 80%
  - Captured non-linear relationships effectively

Feature importance analysis highlights **lead time**, **special requests**, and
**previous cancellations** as dominant predictors :contentReference[oaicite:0]{index=0}.

---

## 🧠 Business Takeaways

- Long lead times suggest opportunities for targeted re-engagement
- Encouraging special requests may increase customer commitment
- Historical customer behavior is critical for risk scoring

These insights can inform pricing strategy, overbooking policies, and customer communication.

---

