# Predicting Heart Disease Risk: A Classification Approach Using Demographic and Biomarker Data
Predicting Heart Disease Risk: A Classification Approach Using Demographic and Biomarker Data

This project leverages the Cleveland database from the UCI Heart Disease dataset to develop and evaluate predictive models for diagnosing heart disease based on a range of patient features.
The dataset includes features such as age, sex, chest pain type, resting blood pressure, serum cholesterol levels, fasting blood sugar, electrocardiographic results, maximum heart rate achieved, and the presence of major vessels colored by fluoroscopy. 

The problem is approached by framing it as a binary classification task, where the goal is to predict the presence (coded as 1) or absence (coded as 0) of heart disease. Key research questions include: What are the most significant predictors of heart disease within this dataset? How do various classification algorithms perform in terms of accuracy and reliability? What is the impact of different data preprocessing techniques on model performance?

# Project Organization



![image](https://github.com/user-attachments/assets/b6736f9f-8918-414b-a424-2c98b03c8a50)







# Modelling
The modeling process began with partitioning the dataset into training (80%) and testing (20%) subsets. Six different classification algorithms were evaluated: Logistic Regression, Decision Tree, Random Forest, Naive Bayes, Support Vector Machine (SVM), and k-Nearest Neighbors (KNN). Model performance was assessed using multiple evaluation metrics, including accuracy, precision, recall, and F1-score. 
                                                                                                                                                                  

To ensure robust evaluation, a 10-fold cross-validation approach was employed. The results were visualized through graphical representations to facilitate comparison. Among the models tested, Naive Bayes achieved the highest performance in terms of the selected evaluation metrics.
