# Heart Disease Classification
Using various machine learning and data science techniques &amp; libraries to attempt to predict heart disease based on medical attributes. Dataset from UCI Machine Learning Repository.

View notebook at GitHub or at NBViewer via this link: https://nbviewer.org/github/rasyadanfz/heart-disease-classification/blob/main/Heart%20Disease%20Classification.ipynb

## Exploratory Data Analysis (EDA) Insights
- Heart disease target classes are quite balanced
- No missing values in data
- Based on data, ~75% female has heart disease
- Based on data, female has a bigger ratio of heart disease to no heart disease than male
- Features that looks correlated to target based on correlation matrix:
  - Positive correlation : cp, thalach, slope
  - Negative corrletion : age, sex, exang, oldpeak, ca, thal

## Modelling
### Models and Hyperparameter tuning
Models :
- Logistic Regression
- K-Nearest Neighbors Classifier
- Random Forest Classifier
- Gradient Boosting Classifier

Best 2 models after hyperparameter tuning with RandomizedSearchCV and GridSearchCV:
- LogisticRegression
- Random Forest Classifier

### Classification Report using 5-fold Cross Validation
Evaluation Results:
- Accuracy : 84.46 %
- Precision : 82.07 %
- Recall : 92.12 %
- F1-Score : 86.73 %
  
Based on classification reports (Accuracy, Precision, Recall, and F1-Score), Logistic Regression performs better than Random Forest Classifier. So, it is chosen.

## Feature Importance
Important features :
- sex
- cp
- restecg
- exang
- oldpeak
- slope
- ca
- thal

## Evaluation
Few things that could be done to reach evaluation target:
- Try other models (such as XGBoost)
- Increase the number of data in dataset
- Improve current models


