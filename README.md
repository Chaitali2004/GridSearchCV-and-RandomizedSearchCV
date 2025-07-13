# GridSearchCV-and-RandomizedSearchCV
hyperparameter tuning techniques like GridSearchCV and RandomizedSearchCV to optimize model parameters

ML Model Comparison with Hyperparameter Tuning
Project Overview
This project compares multiple machine learning models—Logistic Regression and Random Forest—on a classification task using hyperparameter tuning techniques. The objective was to identify the best-performing model based on evaluation metrics such as Accuracy, Precision, Recall, and F1 Score (weighted).

Dataset
Features: 784 numerical features

Target: 1 categorical class column

Preprocessing: Removed constant features, selected top 50 features using SelectKBest(f_classif)

Evaluation Metrics
Model	Accuracy	Precision	Recall	F1 Score
Tuned Logistic Regression	0.7410	0.7370	0.7410	0.7379 
Tuned Random Forest	0.6983	0.6980	0.6983	0.6888 

Final Decision: Logistic Regression chosen for its higher F1 score and faster runtime.

Techniques Used
Feature Selection: SelectKBest (k=50)

GridSearchCV: for Logistic Regression (C, solver)

RandomizedSearchCV: for Random Forest (n_estimators, max_depth, min_samples_split)

Cross-validation: 3-fold and 2-fold for efficiency

Model Evaluation: Accuracy, Precision, Recall, F1 Score
Output
Final model: LogisticRegression(C=1, solver='saga')
<img width="385" height="242" alt="image" src="https://github.com/user-attachments/assets/2b40efbd-ea35-43e1-b456-47e4f1ea316f" />


Saved as: best_model.pkl
link -> https://colab.research.google.com/drive/1m_gZyImLDyq-zN2g4urqtOU6IZuAPs6S?usp=sharing

All code available in notebook
