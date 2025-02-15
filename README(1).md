# Heart Disease Prediction Using Machine Learning.

**Problem Statement**

Heart disease is one of the leading causes of mortality worldwide, and early diagnosis is crucial for effective treatment and prevention. Traditional diagnostic methods are often time-consuming, costly, and require expert medical knowledge. With the increasing availability of medical data, machine learning techniques offer a promising approach to predicting heart disease with higher accuracy and efficiency. This research aims to develop a machine learning-based predictive model that can analyze patient data and identify individuals at risk of heart disease. By leveraging various classification algorithms and feature selection techniques, the model seeks to improve early detection and assist healthcare professionals in making informed decisions, ultimately reducing the burden of heart-related illnesses.

**Dataset**
The dataset is from an ongoing cardiovascular study on residents of the town of Framingham, Massachusetts. The classification goal is to predict whether the patient has 10-year risk of future coronary heart disease (CHD). The dataset provides the patients’ information. It includes over 4,000 records and 15 attributes.Total Records: 4,240
Total Features: 16 (including the target variable)
Target Variable: TenYearCHD (binary: 1 = At risk, 0 = Not at risk)
Missing Values: Present in some columns (e.g., education, glucose, BMI)
Feature Types: Mix of categorical (e.g., gender, smoker status) and numerical (e.g., age, cholesterol, blood pressure)
Use Case: Predicting heart disease risk based on health and lifestyle factors

![Histogram](https://github.com/user-attachments/assets/1d66f71c-88a9-407d-86c2-807d1ab99cee)

Counting number of patients affected by CHD where (0= Not Affected; 1= Affected)

**Sample of dataset**


![Dataset](https://github.com/user-attachments/assets/781d138d-36b3-4f5a-a4ef-f419c94cda80)

**Approach**

We implement machine learning To predict heart disease using machine learning, the approach begins with data preprocessing, including handling missing values, encoding categorical variables, feature scaling, and selecting the most relevant features. Exploratory Data Analysis (EDA) follows, where data distributions, correlations, and class imbalance are analyzed. Next, various classification models such as Logistic Regression, Decision Tree, Random Forest, SVM, and XGBoost are trained, with hyperparameter tuning to optimize performance. Model evaluation is conducted using metrics like accuracy, precision, recall, F1-score, and ROC-AUC. If needed, the final model can be deployed using Flask or Django as an API and integrated into a cloud platform for real-world use.

[modelstrategy_flowchart]

![flowchart](https://github.com/user-attachments/assets/fb1f2f41-5989-4507-8b68-837bb1a15416)

**For classifying the contents according to their information we used the following steps:**

Step 1: Collect the various data from online .

Step 2: Removed special characters, punctuation, stop words, and frequent terms from the content. For collecting the actual feature from the content, we removed the special characters, punctuation, stop words, and frequent terms from the content. 

Step 3: We utilized tokenizer to tokenize the data .In this step we use tokenization to separate the individual word from content.

Step 4: We now have a list of terms and the frequency with which they appeared in each piece of content. The feature was then extracted from the material using tf-idf. Full form of if-idf is Term Frequency Inverse Document Frequency. 

Step 5: We then divided the dataset into 80% for training and 20% for testing. 

Step 6: We then trained a variety of machine learning models to categorize the contents. 
*Machine Leaning Models used:*
•	Logistic Regression
•	Decision Tree
•	Random Forest
•	K-Nearest Neighbor
•	Linear Regression
•	SVC

Step 7: We used a test dataset to assess the machine learning models. We plot confusion matrix for each model. Then we calculate precision, recall, accuracy, F1-score for each model. We evaluated our machine learning approaches using different test contents from our created dataset. In this case, machine learning models performed well for Random Forest feature. 

Step 8: Using the evaluated findings, we selected the best machine learning model is Random Forest. We achieved 95% accuracy using the Random Forest.

![modeltable](https://github.com/user-attachments/assets/bc587548-6235-4372-ba86-3b0fc38549a5)

[performance table of machine learning models]

Step 9: We then used the Random Forest model to forecast the unlabeled content.

**Input Content:**

1. 

male : 1
age : 48
education : 1
currentSmoker :1
cigsPerDay : 20
BPMeds : 0
prevalentStroke : 0
prevalentHyp : 0 
diabetes : 0
totChol : 245
sysBP :127.5
diaBP : 80
BMI :25.34
heartRate :75
glucose :70
TenYearCHD :  0

2.

male : 0
age : 61
education : 3
currentSmoker :1
cigsPerDay : 30
BPMeds : 0
prevalentStroke : 0
prevalentHyp : 1
diabetes : 0
totChol : 225
sysBP :150
diaBP : 95
BMI :28.58
heartRate :65
glucose :103
TenYearCHD :  1

**Output Content:**


![output](https://github.com/user-attachments/assets/3c4de235-e55c-441b-9636-1d41226dc5a8)

**Conclusion**
This project has been conducted to offer an approach for classifying Heart disease remains a leading cause of mortality worldwide, making early prediction crucial for effective prevention and treatment. This project demonstrates how machine learning can be leveraged to develop a predictive model for assessing heart disease risk based on medical and lifestyle factors. By preprocessing the dataset, performing exploratory data analysis, selecting the best machine learning models, and evaluating their performance, we aim to build an accurate and reliable system for heart disease prediction. The results from this study can assist healthcare professionals in early diagnosis, reducing the burden of heart-related illnesses. Future improvements could include incorporating deep learning techniques, real-time patient data, or wearable device integration to enhance prediction accuracy and practical usability. With all of the conclusions of this experiment, it is possible to infer that the approach is an efficient and accurate method for classifying the Heart Disease. 

