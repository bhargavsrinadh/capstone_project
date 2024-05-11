### README: Predicting Mortality in Heart Failure Patients Using Machine Learning

This project involves developing predictive models to estimate the survival outcomes of patients suffering from heart failure based on clinical features. This README provides an overview of the dataset, methods used, findings, and how to utilize the prediction tool developed as part of this analysis.

#### Project Title
Analyzing Clinical Parameters Influencing Mortality in Heart Failure Patients: A Machine Learning Approach

#### Data Sources
The primary data source for this project is a heart failure clinical records dataset available on Kaggle. It contains several clinical parameters such as age, anaemia, creatinine phosphokinase, diabetes, ejection fraction, high blood pressure, platelets, serum creatinine, serum sodium, sex, smoking status, and follow-up time.

#### Analytical Techniques
The analysis utilizes various statistical and machine learning methods, including:
- **Descriptive Statistics**: Summarize data to understand the distribution of key variables.
- **Exploratory Data Analysis (EDA)**: Visualize relationships between variables and survival outcomes.
- **Machine Learning Models**:
  - **Logistic Regression**
  - **Random Forest** with hyperparameter tuning using Grid Search and Cross-Validation.

#### Key Findings
- **Important Predictors**: Age, serum creatinine, and ejection fraction were identified as significant predictors of mortality.
- **Model Performance**: The optimized Random Forest model demonstrated superior predictive capabilities with an accuracy of approximately 87.11%.

#### Usage
The project includes a Python function `predict_heart_failure_survival(features)` that can predict mortality based on input clinical features. Example usage is provided below.


##### Predicting Survival
Here's how to use the function in your Python environment:
```python
# Example features: [Age, Anaemia, CPK, Diabetes, Ejection Fraction, High BP, Platelets, Serum Creatinine, Serum Sodium, Sex, Smoking, Time]
features = [60, 0, 582, 0, 38, 1, 250000, 1.3, 137, 1, 0, 4]
prediction = predict_heart_failure_survival(features)
print(prediction)
```

#### Conclusions
The project illustrates the potential of machine learning in improving the predictive accuracy of patient outcomes in medical settings. The findings can help clinicians develop more tailored treatment strategies for heart failure patients.

#### Future Work
Further research could expand the dataset size, incorporate more diverse clinical parameters, and explore advanced modeling techniques to enhance predictive accuracy. The deployment of these models in real-time clinical settings could also be explored to aid in immediate decision-making.
