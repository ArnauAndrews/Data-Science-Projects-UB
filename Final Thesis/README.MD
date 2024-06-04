### Treatwell Churn Prediction Project

![images](https://github.com/ArnauAndrews/Data-Science-Projects-UB/assets/132329252/e0a63c29-bafe-4038-bc17-106e49847d85)

#### Project Overview:

The **Treatwell Churn Prediction Project** aimed to develop a model to predict venue churn, providing Treatwell with actionable insights to retain venues on their platform. Through data analysis and machine learning techniques, the project sought to address the challenge of proactive churn management and enhance Treatwell's customer retention strategies.

#### Key Outcomes:

- **Churn Prediction Model Implementation:** Successfully implemented a Churn Prediction Model utilizing machine learning algorithms such as Random Forest, Logistic Regression, and XGBoost.
- **Proactive Churn Identification:** Enabled Treatwell to proactively identify venues with a higher probability of churn, facilitating early intervention and strategic retention efforts.
- **Financial and Operational Impact:** Anticipated positive impact on Treatwell's financial and operational performance through reduced venue losses and improved customer retention rates.

#### Evaluation Metrics:

- **Lift Index:** The Lift Index was used to measure the effectiveness of the model compared to a random classification baseline. It quantifies how much better the model is at identifying venues likely to churn compared to random chance. Higher Lift Index values indicate a better predictive performance of the model.
  
- **SHAP Values:** SHAP (SHapley Additive exPlanations) values were utilized to determine the relative contribution of each feature to the model's predictions. By analyzing SHAP values, we gained insights into which variables had the most significant impact on predicting churn, enabling us to prioritize retention strategies accordingly.

#### Model Performance Improvement:

- **Random Forest Model:**
  - Lift Index: Improved by 2.63 times compared to the baseline, indicating a significantly enhanced ability to identify venues at risk of churn.
  - SHAP Values: Identified "Antigüedad" (customer seniority), "appointments_l30d" (appointments in the last 30 days), and "n_channel" (number of channels) as the most influential variables in predicting churn, allowing for targeted retention efforts.

- **Logistic Regression Model:**
  - Lift Index: Achieved a lift of 2.43 times better than the baseline, demonstrating improved churn prediction capabilities.
  - SHAP Values: Highlighted "appointments_l30d," "net_orders," and "net_aov" as the most significant variables, providing insights into customer behavior patterns affecting churn likelihood.

- **XGBoost Model:**
  - Lift Index: Showed a lift of 2.78 times better than the baseline, indicating enhanced predictive power.
  - SHAP Values: Identified "Antigüedad," "appointments_l30d," and "n_channel" as key variables influencing churn prediction, guiding targeted retention strategies.

### Conclusion:

The **Treatwell Churn Prediction Project** successfully implemented predictive models leveraging Lift Index and SHAP values to enhance venue churn prediction. By improving model performance metrics and identifying influential variables, Treatwell gained actionable insights to proactively manage churn and optimize customer retention strategies. The project's outcomes demonstrate the potential for data-driven approaches to drive positive business outcomes and enhance customer satisfaction in the service industry.
