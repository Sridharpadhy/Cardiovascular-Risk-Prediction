# Cardiovascular-Risk-Prediction
Cardiovascular Risk Prediction

![68747470733a2f2f737465616d75736572696d616765732d612e616b616d616968642e6e65742f7567632f313937333136393932323934313239393939392f413442354644343537354530464339353133413139343241463842333835333146434337343937412f3f696d](https://github.com/Sridharpadhy/Cardiovascular-Risk-Prediction/assets/120051156/79739db6-d386-417b-b4dc-7ac37ea29e63)


Explainatory Video : https://drive.google.com/drive/folders/1JClKXiEyCLBS5BkVej_e2OkQy55OvwnW?usp=sharing 

1. PowerBi dashboard - This File contains the pdf and the powerBI file of the dashboard prepared from the provided data after doing EDA.
2. Collab file - This is the whole project file from EDA , data cleaning , data preprocessing , Model implementation and hyperameter with detail conculsion
3. CSV File - This csv File contain the raw data provided to us.



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



The following machine learning models were built and evaluated in this project:

* Logistic Regression
* Naive Bayes 
* Decision Tree
* Random forest 
* XGboost
* KNN
* SVM

  
Results:

Our data set has 17 features & 3390 rows. We studied all these features and have drawn following conclusions:

The very first graphs gives us the distribution of dependent variable and whch shows that very less no of peoples are prone to cardiovascular risk.

Any value outiside the given normal range determines higher risk of cardiovascular risk. Thus, various companies like insurance, healthcare, fitness-nutrition and medical can target this population for better revenue generation.
-We have observed that people wether or not smoking are at equal risk of cardio vascular diseases, which suggests companies to target them equally.

-Our data shows that people having hypertension are more prone to cardio vascular diseases, very less no. of paitents are on BpMeds, but 50 % of then are at cardiovascular risk, which is significant. Thus, this information can be leveraged by various companies.

-Distribution of cardiovascular Risk and Age shows that with increase in age chances of having cardiovascular diseases increases.

-Diabetic patients are high risk of getting cardio vascular disease as our data shows; ~ 61% of the diabetic population is at high risk.

-Gender distribution shows that males are more prone to cardio vascular risk as compared to females because the frequency of males having smoking habits is more.

-Another bivariate plot between Systolic and diastolic BP shows that they are positivly correalted and with increase in any of this values increses the ridk of cardiovascular diseases.

-Orderwise correlation shows that age and systolic pressure highly affect our dependent variable.

Machine Learning :

Following Machine Learning models are used in this project with their corresponding performance metrics on the test data -


![final final](https://github.com/Sridharpadhy/Cardiovascular-Risk-Prediction/assets/120051156/74e9e97a-35c1-4891-acd2-c014d76a8179)


From all this ML Models - Xgboost with hyperparameter is been selected as the Prediction Model because it is giving the result with high accuracy of 0.84 and rou-auc value of 0.84 and precision of 0.86 which is great and also it doesnt seems like overfitting .

Orther then that shap is used to justify the importance xgboost is giving to the features.

The above plot shows the feature importances of the dataset.

Gender is the most influencing factor in prediction.

age, cigsPerDay, pulsePressure,totChol & heartRate also shows good contribution in prediction.

Other features are having less contribution in prediction. Least being BPMeds,diabetes & prevalentStroke.
