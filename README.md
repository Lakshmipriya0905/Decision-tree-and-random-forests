
 ## Task 5 – Decision Tree & Random Forest Classifier (Heart Disease Prediction)
# 📌 Objective
The goal of this task is to:

Train a Decision Tree Classifier and visualize it.
Analyze overfitting and control the tree depth.
Train a Random Forest Classifier and compare it with Decision Tree.
Interpret feature importances.
Evaluate models using Cross-Validation.

 # 📂 Dataset
Name: heart.csv
Description: Contains patient medical details (age, cholesterol, etc.) and whether they have heart disease (target column: 1 = yes, 0 = no).

 # 🛠 Libraries Used
pandas → data handling
numpy → numerical operations
matplotlib → plotting graphs
scikit-learn → machine learning models & evaluation

# 🚀 Steps Performed
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
Trained multiple Decision Trees with different max_depth values (1–20).
Plotted Train Accuracy vs Test Accuracy to detect overfitting.
Selected the max_depth with the highest test accuracy.
Step 3 – Random Forest
Created a RandomForestClassifier with 100 trees.
Trained it and compared accuracy with Decision Tree.
Calculated ROC-AUC to measure classification quality.
Step 4 – Feature Importances
Extracted and sorted feature_importances_ from Random Forest.
Displayed top 10 features and plotted them as a bar chart.
Step 5 – Cross-Validation
Used Stratified 5-Fold Cross-Validation to evaluate both models.
Printed mean accuracy and standard deviation for:
Random Forest
Pruned Decision Tree (best max_depth from Step 2)

# 📌 Key Insights
Decision Tree can overfit if max_depth is too high.
Random Forest usually performs better due to averaging multiple trees.
Feature importance shows which health metrics are most useful for prediction.

# 📷 Outputs
Include screenshots of:
Decision Tree visualization
Overfitting plot
Feature importance bar chart
