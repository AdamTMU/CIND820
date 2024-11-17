# Predicting Heart Disease Risk: A Classification Approach Using Demographic and Biomarker Data
Predicting Heart Disease Risk: A Classification Approach Using Demographic and Biomarker Data

This project leverages the Cleveland database from the UCI Heart Disease dataset to develop and evaluate predictive models for diagnosing heart disease based on a range of patient features.
The dataset includes features such as age, sex, chest pain type, resting blood pressure, serum cholesterol levels, fasting blood sugar, electrocardiographic results, maximum heart rate achieved, and the presence of major vessels colored by fluoroscopy. 

The problem is approached by framing it as a binary classification task, where the goal is to predict the presence (coded as 1) or absence (coded as 0) of heart disease. Key research questions include: What are the most significant predictors of heart disease within this dataset? How do various classification algorithms perform in terms of accuracy and reliability? What is the impact of different data preprocessing techniques on model performance?

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

# Key Takeaways
The Naive Bayes model is performing well overall, with an accuracy of 85%, and it’s especially strong at predicting the "no heart disease" class (class 0). The slightly lower recall for class 1 (heart disease) compared to class 0 indicates that the model might miss some cases of heart disease. The results are fairly consistent, as evidenced by the relatively small standard deviation in cross-validation scores.


