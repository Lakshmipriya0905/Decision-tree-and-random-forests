
## Task 5 – Decision Tree & Random Forest Classifier (Heart Disease Prediction)
📌 Objective
The goal of this task is to:

Train a Decision Tree Classifier and visualize it.
Analyze overfitting and control the tree depth.
Train a Random Forest Classifier and compare it with Decision Tree.
Interpret feature importances.
Evaluate models using Cross-Validation.
📂 Dataset
Name: heart.csv
Description: Contains patient medical details (age, cholesterol, etc.) and whether they have heart disease (target column: 1 = yes, 0 = no).
🛠 Libraries Used
pandas → data handling
numpy → numerical operations
matplotlib → plotting graphs
scikit-learn → machine learning models & evaluation
🚀 Steps Performed
Step 0 – Load & Prepare Data
Loaded the CSV using pandas.
Split the data into:
X = features (all columns except target)
y = target (target column)
Train-test split (80% train, 20% test) using train_test_split.
Step 1 – Train & Visualize Decision Tree
Created a DecisionTreeClassifier.
Trained the model on X_train, y_train.
Printed Accuracy, Classification Report, and Confusion Matrix.
Used plot_tree() to visualize the trained tree.
Step 2 – Overfitting Analysis
