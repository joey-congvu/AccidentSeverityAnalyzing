🚗 Accident Severity Prediction

📌 Overview
This project focuses on predicting the severity of traffic accidents using machine learning techniques. The goal is to identify high-risk situations and improve decision-making for traffic safety and emergency response.
The model analyzes environmental and roadway-related factors (e.g., lighting conditions, weather, collision type) to classify accident severity.

🎯 Objectives
Predict accident severity using real-world crash data
Handle imbalanced datasets effectively
Compare baseline and advanced machine learning models
Improve detection of severe accidents (major injuries & fatalities)

📊 Dataset
Source: NHTSA Crash Report Sampling System (CRSS)
Includes features such as:
Time (hour, day of week, month)
Weather conditions
Lighting conditions
Type of collision
Roadway and intersection information
Note: Some features with excessive missing values (e.g., alcohol involvement) were removed to improve model reliability.

⚙️ Technologies Used
Python
Pandas, NumPy
Scikit-learn
Imbalanced-learn (SMOTE, RandomOverSampler, SMOTETomek)
XGBoost
CatBoost
Matplotlib / Seaborn

🧠 Models Implemented

1. Decision Tree (Baseline)
Easy to interpret
Fast to train
Limitation: biased toward majority classes

2. XGBoost
Gradient boosting algorithm
Handles complex relationships
Improved performance over baseline

4. CatBoost (Final Model)
Best performance overall
Handles categorical features effectively
More stable with imbalanced data

⚖️ Handling Imbalanced Data

To address class imbalance:
Random Oversampling
Random Undersampling
SMOTETomek (best performing method)
These techniques were integrated into pipelines to avoid data leakage during cross-validation.

📈 Evaluation Metrics
Accuracy
Precision (Macro)
Recall (Macro)
F1-score (Macro)
ROC-AUC (for binary classification)
Focus was placed on recall and F1-score to better detect severe accidents.

🔍 Key Insights

Important features:

Collision type
Harmful event
Lighting condition
Weather
Roadway relation
Severe accidents are harder to predict due to class imbalance
Binary classification (severe vs non-severe) improved model performance

How to run: demo.ipynb
Report: FinalReport.pdf
