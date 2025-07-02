# Task-5
🚢 Titanic Survival Prediction using Decision Trees & Random Forest
📌 Project Overview
This project is part of the AI & ML Internship Task 5. The objective is to understand and apply tree-based machine learning models, specifically Decision Tree and Random Forest, to classify survival outcomes on the Titanic dataset.

🔍 Task Objectives
Train a Decision Tree Classifier and visualize it.

Analyze overfitting and use max_depth to control it.

Train a Random Forest Classifier and compare performance.

Interpret and visualize feature importance.

Perform cross-validation for model evaluation.

📁 Dataset
Source: Kaggle Titanic Dataset (uploaded as titanic dataset.csv)

Target Variable: Survived

Features: Pclass, Sex, Age, SibSp, Parch, Fare, Embarked, etc.

🛠 Tools & Libraries Used
Python

Google Colab

pandas, numpy, matplotlib, seaborn

scikit-learn (for training models)

plot_tree for visualization

📊 Steps and Explanation
1. Data Cleaning
Removed irrelevant columns like PassengerId, Name, Ticket, Cabin.

Handled missing values in Age (filled with median) and Embarked (filled with mode).

Encoded categorical features: Sex (binary map), Embarked (one-hot encoded).

2. Decision Tree Classifier
Trained on 80% of the data, tested on 20%.

Achieved 100% accuracy on the test set due to dataset bias or simplicity.

Visualized using plot_tree (see image below):


3. Overfitting Analysis
Plotted train vs. test accuracy against varying max_depth.

Both remained 100%, suggesting the model perfectly fits the data.


4. Random Forest Classifier
Trained using 100 estimators.

Achieved 100% accuracy as well.

Extracted and plotted feature importances:


5. Cross-Validation
Used 5-fold cross-validation.

Both models yielded a CV Score of 1.0, indicating perfect consistency across folds.

