# Predictive Analysis for Heart Disease
## Lavanya Kandhari
### Introduction

The selected dataset for the report is the Heart Diseases Dataset from Kaggle and it can be found [HERE](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset/data)

One of the leading causes of death in Hungary are cardiovascular diseases (CVDs) (OECD and WHO, 2017). It constitutes approximately 52.4% of the main diagnoses underlying cause of death and 47.6% of the secondary diagnoses prior to death. Heart failure is a common result of CVDs. Several risk factors are known to be associated with CVDs; the most prominent among them are high blood pressure, high cholesterol levels, and smoking (CDC, 2022). Moreover, susceptibility to heart disease increases with age and other uncontrollable factors such as sex (McLaren, 2023).in this data set, It contains various clinical and demographic attributes of patients, for example, age, gender, cholesterol levels, and resting blood pressure results along with the “target” variable indicating the presence or absence of heart disease.Our research question is about about how will the quantitative variable(age, cholesterol levels, tres tbsp, restecg ,,slope,cp) helps us to determine regarding to whether there is heart disease.Previous research has been showing us that adults with age 65 and older are more likely to suffer from the disease , than young people, so we thought that there should be a positive correlation between the age and the chances of getting diseases(CDC, 2018),regarding to the relationship between the diseases and the cholesterol level it becomes a little bit bit ambiguous, the article from the medical news today shows that even though it is previously being showed that people with high cholesterol are more tending to get the disease, the recent research has been showing that the relationship is not as clearly as we thought before.(MedicalNewsToday,2023)

![Heart](https://c8y.doxcdn.com/image/upload/c_fill,fl_progressive,h_800,q_auto,w_1600/gau2taystiugaa2br7zs.webp)
### Data:
Heart disease is a leading cause of mortality worldwide, and early diagnosis and risk assessment are important for effective management and prevention. This dataset contains information related to heart disease diagnosis from 1988 and consists of Cleveland databases. It contains various clinical and demographic attributes of patients, for example, age, gender, cholesterol levels, and resting blood pressure results along with the “target” variable indicating the presence or absence of heart disease.
We will now explore the key objectives of the data to know more about it :


- We have a total number of 1025 observations, out of which 302 are unique
- We have 14 variables, out of which "target" is the response varibale and the rest are predictors
- The dataset that we will be using features 14 attributes of patients that will be examined to determine which are possible indicators of heart disease: 
    - age: age (continuous)
    - sex: binary , 1 = male; 0 = female (will be used as a categorical variable)
    - cp: chest pain type, 4 values 0 = typical angina; 1 = atypical angina; 2 = non-anginal pain; 3 = asymptomatic (will be used as a categorical variable)
    - trestbps: resting blood pressure (in mm Hg on admission to the hospital)(continuous, double)
    - chol: serum cholesterol in mg/dl (continuous)
    - fbs: fasting blood sugar > 120 mg/dl binary 1 = true; 0 = false (will be used as a categorical variable)
    - restecg: resting electrocardiographic results 0: normal; 1: having ST-T wave abnormality ; 2: showing probable or definite left ventricular hypertrophy by Estes' criteria (will be used as a categorical variable)
    - thalach: maximum heart rate achieved (continuous)
    - exang: exercise induced angina, 1 = yes; 0 = no (will be used as a categorical variable)
    - oldpeak: ST depression induced by exercise relative to rest (continuous, double)
    - slope: the slope of the peak exercise ST segment 0: upsloping; 1: flat; 2: downsloping (will be used as a categorical variable)
    - ca: number of major vessels (0-3) colored by flourosopy (continuous)
    - thal: 0 = normal; 1 = fixed defect; 2 = reversable defect (will be used as a categorical variable)
    - target: resting electrocardiographic results (values 0,1) (response variable)

This dataset has been collected by the cleveland clinical foundation, little is known about the origin but it is known that this research has been used by ML researchers to date for modelling related to heart diseases. 

### Question
Research Question: **Determine the possible numeric indicators of heart disease which will then be used to predict the presence of heart disease in patients**
    
Response Variable: Taget (1=no disease, 0 = disease)  
Explanatory Variables: age, cholesterol levels, trestbps,restecg,slope,cp

Since the data set contains all those explanatory variables, we need to first do inference, which is exploring which variable is significant to the response variable. Secondly, we need to build a model to do prediction, and those explantory variables that are significant must considered into model to get higher accuacy.
