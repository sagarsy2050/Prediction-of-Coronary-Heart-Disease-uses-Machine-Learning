# Coronary Heart Disease Prediction Using Machine Learning Technique
PREPROCESSED DATA FROM FRAMINGHAM CARDIOVASCULAR DISEASE DATASET

Introduction
As a beginner, cleaning, preprocessing, and preparing the data is one of the most time-consuming steps. So, I preprocessed the data from 'https://www.kaggle.com/dileep070/heart-disease-prediction-using-logistic-regression?select=framingham.csv' and ready to go (I hope) for the further steps.

Source
The dataset is publically available on the Kaggle website, and it is from an ongoing cardiovascular study on residents of the town of Framingham, Massachusetts. The classification goal is to predict whether the patient has a 10-year risk of future coronary heart disease (CHD). The dataset provides the patients’ information. It includes over 4,000 records and 15 attributes.
Variables
Each attribute is a potential risk factor. There are both demographic, behavioral, and medical risk factors.
# working point
# Heart Disease Prediction
### Will a patient have a 10 year risk of developing a cardio vascular diseases?

### Table of contents
1. [Introduction](#introduction)
2. [Exploratory Data Analysis](#paragraph1)
3. [Feature Selection](#paragraph2)
4. [Feature Scaling](#paragraph3)
5. [Test - Train Split](#paragraph4)
6. [Resampling](#paragraph5)
7. [Model Pipeline](#paragraph6)
8. [Modelling & Evaluation](#paragraph7)
9. [Apply model](#paragraph8)

## Introduction <a name="introduction"></a>

**Problem:**
The World Health Organization has estimated 12 million deaths occur worldwide, every year due to Heart diseases. Half the deaths in the United States and other developed countries are due to cardio vascular diseases. The early prognosis of cardiovascular diseases can aid in making decisions on lifestyle changes in high risk patients and in turn reduce the complications. This research intends to pinpoint the most relevant/risk factors of heart disease as well as predict the overall risk using logistic regression Data Preparation

**Source:**
The dataset is publically available on the Kaggle website, and it is from an ongoing cardiovascular study on residents of the town of Framingham, Massachusetts. The classification goal is to predict whether the patient has 10-year risk of future coronary heart disease (CHD).The dataset provides the patients’ information. It includes over 4,000 records and 15 attributes. Variables Each attribute is a potential risk factor. There are both demographic, behavioral and medical risk factors.

**Attributes:**

#### Demographic: 
* Sex: male or female(Nominal) 
* Age: Age of the patient;(Continuous - Although the recorded ages have been truncated to whole numbers, the concept of age is continuous) 
* Education: no further information provided

#### Behavioral: 
* Current Smoker: whether or not the patient is a current smoker (Nominal) 
* Cigs Per Day: the number of cigarettes that the person smoked on average in one day.(can be considered continuous as one can have any number of cigarettes, even half a cigarette.) 

#### Information on medical history: 
* BP Meds: whether or not the patient was on blood pressure medication (Nominal) 
* Prevalent Stroke: whether or not the patient had previously had a stroke (Nominal) 
* Prevalent Hyp: whether or not the patient was hypertensive (Nominal) 
* Diabetes: whether or not the patient had diabetes (Nominal) 

#### Information on current medical condition: 
* Tot Chol: total cholesterol level (Continuous) 
* Sys BP: systolic blood pressure (Continuous) 
* Dia BP: diastolic blood pressure (Continuous) 
* BMI: Body Mass Index (Continuous) 
* Heart Rate: heart rate (Continuous - In medical research, variables such as heart rate though in fact discrete, yet are considered continuous because of large number of possible values.) 
* Glucose: glucose level (Continuous) 

# Result Analyzed

The dataset is provided based on study on residents of the town of Framingham, Massachusetts. The
classification goal is to predict whether the patient has 10-year risk of future coronary heart disease
(CHD).The dataset provides the patients’ information.

It is seen that Random Forest and Logistic Regression performs better than the other classifiers during
training and that Logistic Regression is better than Random Forest during testing.

The LR classifier outperforms the other classifiers in terms of accuracy and memory utilization.

For class imbalance issue though we used XG Boost and feature selection in Random Forest it did not help
much

Another important point is the over-fitting suffered by classifiers other than XGBoost despite regularization
or introduction of randomness, as the case maybe.

XGBoost overcomes this problem due to its excellent inherent regularization and hence works perfectly for
the noisy data from the HRIS.

However LR worked better as compared to other models, the AUC score was also 91%.
