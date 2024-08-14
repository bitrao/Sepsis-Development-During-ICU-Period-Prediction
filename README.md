# Sepsis Development During ICU Period Prediction
## Introduction:

Sepsis is a life-threatening infection that can develop from staying in Intensive Care Units (ICU), occurring when the infection-fighting processes damage the body's own organs. During the COVID-19 pandemic, ICUs need to focus on this problem more than ever, increasing the need to monitor patients' status regarding their infection risk. Therefore, the goal of this notebook is to build a machine learning model that can predict the probability of a patient developing an infection based on a provided dataset.

This notebook utilizes various libraries, including analytical and visualization tools like numpy, pandas, matplotlib, and seaborn, as well as machine learning models and data processor from scikit-learn. Since our objective is to predict the outcome of Sepsis, the models employed are binary classifiers, specifically Logistic Regression and K-Nearest Neighbor


## Conclusion:

| Models      | MCC | f1-score(%) | AUC_ROC (%) | Accuracy (%) |
|-------------|--------------------------|----------------------|-----|----|
| 1. Hyperparameter-tuned Logistic Regression** | 0.4568 | 65.12 | 73.08 | 75|
| 2. Hyperparameter-tuned K-Nearest Neighbor with transformed data and Oversampling** | 0.4790 | 68 | 75.09 | 73.33 |

The Hyperparameter-tuned K-Nearest Neighbor with transformed data and
Oversampling performs the best overall and achieve greater score. Despite the prediction
of negative case is not adequate to the Logistic Regression, it has the superior capability
to predict positive case which make the model is more precise regarding both classes,
hence more practical in real-life.


*Assignment 1 of COSC3013-Computational Machine Learning RMIT 2024*
