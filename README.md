# Predicting Heart Disease Risk: A Classification Approach Using Demographic and Biomarker Data
Predicting Heart Disease Risk: A Classification Approach Using Demographic and Biomarker Data

This project leverages the Cleveland database from the UCI Heart Disease dataset to develop and evaluate predictive models for diagnosing heart disease based on a range of patient features.
The dataset includes features such as age, sex, chest pain type, resting blood pressure, serum cholesterol levels, fasting blood sugar, electrocardiographic results, maximum heart rate achieved, and the presence of major vessels colored by fluoroscopy. 

The problem is approached by framing it as a binary classification task, where the goal is to predict the presence (coded as 1) or absence (coded as 0) of heart disease. Key research questions include: What are the most significant predictors of heart disease within this dataset? How do various classification algorithms perform in terms of accuracy and reliability? What is the impact of different data preprocessing techniques on model performance?

# Exploratory Data Analysis (EDA)

![image](https://github.com/user-attachments/assets/8b065e25-a816-49d5-9a63-bc50c47ada7d)






# Project Organization



![image](https://github.com/user-attachments/assets/b6736f9f-8918-414b-a424-2c98b03c8a50)







# Modelling
The modeling process began with partitioning the dataset into training (80%) and testing (20%) subsets. Six different classification algorithms were evaluated: Logistic Regression, Decision Tree, Random Forest, Naive Bayes, Support Vector Machine (SVM), and k-Nearest Neighbors (KNN). Model performance was assessed using multiple evaluation metrics, including accuracy, precision, recall, and F1-score. 
                                                                                                                                                                  

To ensure robust evaluation, a 10-fold cross-validation approach was employed. The results were visualized through graphical representations to facilitate comparison.

# Interpretation
Naive Bayes classification model was the best performer out of the six methods.

Observations:

Overall Performance Accuracy: 0.85 The model's overall accuracy is 85%, meaning it correctly predicts the presence or absence of heart disease 85% of the time across all instances.

Macro Average: Precision: 0.85, Recall: 0.84, F1-score: 0.84 The macro average treats both classes equally, giving us an overall view of the model's performance across both classes. The high macro average precision, recall, and F1-score indicate the model is doing a good job at predicting both classes.

Weighted Average Precision: 0.85, Recall: 0.85, F1-score: 0.84 The weighted average accounts for the imbalanced dataset (more instances of class 0 than class 1). Since the number of instances in each class is weighted, the weighted averages are very similar to the macro averages, which is a good sign. It suggests the model is not heavily biased toward the larger class (class 0) and is performing fairly well for both classes.

# Suggestions for Improvement
Improving Recall for Class 1: The model could potentially be improved in detecting heart disease cases by exploring techniques like oversampling (e.g., SMOTE), to make it more sensitive to class 1. In addition hyperparameter tuning such as treshold adjustment could also further improve performance.

# Improved Results
The precision and recall for both classes are now more balanced, and the recall for class 1 (heart disease) has improved significantly to 92%. This suggests that the adjustments (SMOTE and threshold tuning) helped the model become much better at detecting heart disease cases without sacrificing too much precision. Our applied strategies were effective in improving the model's ability to detect heart disease cases while maintaining a good performance on the "no heart disease" class.

# Key Takeways
Based on the analysis and model evaluation, Naive Bayes emerged as the best-performing machine learning model for predicting heart disease. It demonstrated strong performance with a weighted average precision of 92%, indicating its ability to accurately identify heart disease cases across different classes. Feature selection using the ANOVA F-test revealed the five most important predictors of heart disease, which were: Thalassemia, the number of major vessels colored by fluoroscopy (ca), ST depression induced by exercise (oldpeak), maximum heart rate achieved (thalach), and the presence of exercise-induced angina (exang). These features were found to have the highest statistical significance in distinguishing between individuals with and without heart disease. This analysis highlights the effectiveness of both Naive Bayes and the selected features in providing meaningful insights for heart disease prediction.
