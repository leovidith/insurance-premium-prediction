
# Insurance Premium Prediction using Machine & Deep 

This project investigates the impact of demographic and lifestyle features on health insurance premiums. A diverse suite of regression models—including traditional ML regressors and deep neural networks—was employed to predict charges and evaluate the relative influence of each feature. The study identifies **smoking status** as the most dominant factor, contributing approximately **62.04%** to the prediction performance.

---

## Objective

To build accurate and interpretable models for predicting individual insurance costs based on features such as age, BMI, number of children, region, and smoking behavior.

---

## Experimental Setup

- **Dataset:** 1338 samples, 7 features (sourced from Kaggle)
- **Preprocessing:** Encoding, outlier handling (IQR & Z-score), standard scaling
- **Modeling:** 13 classical ML models + 2 deep learning architectures (base & tuned)
- **Tuning Methodology:** Keras Tuner (Hyperband) for deep learning model optimization

---

## Results
| Model                          | RMSE      | MAE      | R² Score            |
|-------------------------------|-----------|----------|---------------------|
| Linear Regression             | 0.5342    | 0.3567   | 0.6049              |
| Ridge Regression              | 0.5342    | 0.3568   | 0.6042              |
| ElasticNet                    | 0.8517    | 0.6036   | -19.3423            |
| Bayesian Ridge                | 0.5341    | 0.3568   | 0.6036              |
| Huber Regressor               | 0.5960    | 0.2972   | 0.6807              |
| Gradient Boosting             | 0.4143    | 0.2226   | 0.7705              |
| HistGradient Boosting         | 0.4125    | 0.2301   | 0.7844              |
| SVR                           | 0.4260    | 0.2250   | 0.7600              |
| Decision Tree                 | 0.5057    | 0.2334   | 0.7202              |
| K-Nearest Neighbors           | 0.4868    | 0.3050   | 0.6736              |
| Gaussian Process Regressor    | 53.9763   | 19.7436  | -0.0005             |
| ARD Regression                | 0.5362    | 0.3572   | 0.6027              |
| Deep Learning (Base)          | -         | 0.2394   | 0.7363              |
| Deep Learning (Tuned)         | -         | 0.2426   | 0.7818              |

---

## Key Findings

- **Smoking** is the most significant predictor of insurance premiums.
- Ensemble models and tuned DNNs exhibit superior predictive capabilities.
- Outlier removal and feature scaling substantially improve model robustness.
