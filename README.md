# Wine Quality Prediction using Supervised Learning

![image](https://github.com/user-attachments/assets/25236665-600e-4527-8234-0e69d6968d01)

---

### Objective
This project was completed as part of CU Boulder's Introduction to Machine Learning: Supervised Learning course. The project aims to utilize and compare various supervised machine learning approaches on predicting the quality of red variants of the Portuguese "Vinho Verde" wine based upon 11 physicochemical characteristics. This project is a binary classification task, where the models will work to predict whether a wine is 'good' or 'bad' based upon its features. The performance of the models will be compared to determine the most effective machine learning strategy. The dataset is publicly available on UCI's machine learning repository and is licensed for public use under the CC BY 4.0 license. The following models will be used: logistic regression, random forest, k-nearest neighbors (KNN), support vector classifier (SVC). Furthermore, the performance of the models will be optimized by either GridSearchCV or cross validation.

---

### Methods
Libraries Used
- pandas
- numpy
- seaborn
- matplotlib
- sklearn (LogisticRegression, RandomForestClassifier, KNeighborsClassifier, SVC)
- sklearn.metrics (accuracy_score, precision_score, recall_score, classification_report)
- sklearn.preprocessing (LabelEncoder, StandardScaler)
- sklearn.model_selection (train_test_split, GridSearchCV, cross_val_score)

Exploratory Data Analysis (EDA)
- Histograms visualizing the distributions of each feature
- Correlation matrix (heatmap) visualizing the potential correlations between features and target variable
- Bar plots visualizing the compared distributions of certain features vs the target

Data Preprocessing
- Dividing the target variable 'quality' into two groups: 'good' and 'bad'
- 'good' = 'quality' score above 5.5
- 'bad' = 'quality' score below 5.5
- Encoded 'good' and 'bad' to 1 and 0, respectively

Models
- Logistic regression
- Random forest
- KNN
- SVC
- Metrics: acccuracy, precision

Model Improvements
- Random forest w/ GridSearchCV
- KNN w/ Cross Validation
- SVC w/ GridSearchCV

---

### General Results
Accuracy
- SVC w/ GridSearchCV --> 77.2%
- KNN w/ Cross Validation ---> 76.9%
- Random Forest --> 76.9%
- SVC --> 76.6%
- Logistic Regression --> 73.75%
- KNN --> 73.1%
- Random Forest w/ GridSearchCV --> 72.5%

Precision
- SVC w/ GridSearchCV --> 81.5%
- Random Forest --> 81.4%
- SVC --> 81%
- Logistic Regression --> 79.5%
- Random Forest w/ GridSearchCV --> 78.6%
- KNN w/ Cross Validation --> 78.1%
- KNN --> 74.1%

Overall, SVC with GridSearchCV yielded the best performance metrics. 
