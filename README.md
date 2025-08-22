🚢 Titanic Survival Prediction using Logistic Regression

This project applies Logistic Regression to the famous Titanic dataset
, predicting whether a passenger survived based on features such as age, class, sex, and fare.

📌 Project Overview

Perform exploratory data analysis (EDA) to understand survival patterns.

Clean the dataset (handle missing values, drop irrelevant features, encode categorical variables).

Train and evaluate a logistic regression classifier using scikit-learn.

Achieve ~83% accuracy in predicting passenger survival.

🛠️ Tools & Libraries

Python

Pandas, NumPy → Data handling & cleaning

Matplotlib, Seaborn, Plotly (Cufflinks) → Visualization

scikit-learn → Logistic Regression, model evaluation

📊 Exploratory Data Analysis

Inspected missing values using heatmaps.

Visualized survival distributions by passenger class, sex, siblings/spouses, and age.

Observed:

Higher survival rates among 1st-class and female passengers.

Strong influence of fare and family members on survival chances.

🧹 Data Cleaning

Imputed missing ages using median values based on passenger class.

Dropped the Cabin column (too many missing values).

Removed remaining nulls from Embarked.

Converted categorical features (Sex, Embarked, Pclass) into dummy variables.

Dropped unnecessary columns (PassengerId, Name, Ticket).

🤖 Model Training

Split dataset into train/test (70/30).

Trained Logistic Regression on preprocessed features.

Addressed convergence warnings (increasing iterations).

Performance

Accuracy: ~83%

Confusion Matrix:

[[150,  13],
 [ 33,  71]]


Classification Report:

Precision: 0.82 (class 0), 0.85 (class 1)

Recall: 0.92 (class 0), 0.68 (class 1)

F1-score: 0.87 (class 0), 0.76 (class 1)

📈 Key Insights

Sex and Pclass are the strongest predictors of survival.

Fare also correlates with survival (wealthier passengers tended to survive more).

Logistic Regression, despite being a simple model, captures meaningful survival patterns.

🚀 How to Run

Clone this repository

git clone https://github.com/yourusername/titanic-logistic-regression.git
cd titanic-logistic-regression


Install dependencies

pip install -r requirements.txt


Run the Jupyter Notebook

jupyter notebook Titanic_Logistic_Regression.ipynb

📌 Future Improvements

Try more advanced models (Random Forest, Gradient Boosting).

Apply feature scaling for faster convergence.

Hyperparameter tuning for Logistic Regression.

Compare results with modern Kaggle solutions.

✨ Built with curiosity & data science fundamentals.
