# Cardiovascular-Risk-Prediction
Cardiovascular Risk Prediction

![image](https://github.com/Sridharpadhy/Cardiovascular-Risk-Prediction/assets/120051156/9b376225-ef69-4c20-9954-d6a309af66d8)


Overview
This project aims to develop a predictive model for cardiovascular disease (CVD) risk based on demographic and lifestyle factors. The ultimate goal is to provide a personalized risk score for each individual, which will enable healthcare providers to take necessary preventive measures and improve disease outcomes.


Data
Demographic:
* Sex: male or female("M" or "F")
* Age: Age of the patient;(Continuous - Although the recorded ages have been truncated to whole numbers, the concept of age is continuous)
Behavioral:
* is_smoking: whether or not the patient is a current smoker ("YES" or "NO")
* Cigs Per Day: the number of cigarettes that the person smoked on average in one day.(can be considered continuous as one can have any number of cigarettes, even half a cigarette.)
Medical( history):
* BP Meds: whether or not the patient was on blood pressure medication (Nominal)
* Prevalent Stroke: whether or not the patient had previously had a stroke (Nominal)
* Prevalent Hyp: whether or not the patient was hypertensive (Nominal)
* Diabetes: whether or not the patient had diabetes (Nominal)
Medical( current):
* Tot Chol: total cholesterol level (Continuous)
* Sys BP: systolic blood pressure (Continuous)
* Dia BP: diastolic blood pressure (Continuous)
* BMI: Body Mass Index (Continuous)
* Heart Rate: heart rate (Continuous - In medical research, variables such as heart rate though infact discrete, yet are considered continuous because of large number of possible values.)
* Glucose: glucose level (Continuous)
Predict variable (desired target):
* 10-year risk of coronary heart disease CHD(binary: “1”, means “Yes”, “0” means “No”)
Models
The following machine learning models were built and evaluated in this project:

* Logistic Regression
* Naive Bayes 
* Decision Tree
* Random forest 
* Adaboost
* KNN
* SVM
Results
The end result of this project will be a predictive model that healthcare providers can use to prioritize their interventions and improve the outcomes for individuals at high risk of CVD. The model has the potential to significantly impact public health by reducing the incidence of CVD and improving the lives of those affected by the disease.

Implementation
The model will be developed using appropriate machine learning techniques and tools, and its performance will be evaluated using confusion matrix. The solution will be easily interpretable, scalable, and capable of handling missing data.

Evaluation
The performance of each model was evaluated using these metrics which provide a comprehensive view of the model's performance:

* Accuracy
* Precison 
* Recall
* F1 Score
Conclusion
Based on the analysis of the data, the following conclusions were be drawn:

* The comparison of the performance of two models, Logistic Regression and Adaboost, was performed before and after hyperparameter tuning.
* Logistic Regression model showed the best performance overall, both before and after tuning the hyperparameters.
* Adaboost model showed significant improvement in performance after hyperparameter tuning, but it still didn't outperform the Logistic Regression model in all metrics used for comparison.
* Hence, the Logistic Regression model is selected as the best model for predicting heart risk.
In conclusion, the Logistic Regression model was determined to be the most accurate and efficient model for predicting heart risk. Its performance was consistent and stable, both before and after tuning the hyperparameters. This model can serve as a reliable tool for healthcare professionals to use in their assessments of a patient's heart risk.


