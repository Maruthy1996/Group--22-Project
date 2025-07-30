
Titanic - Machine Learning from Disaster
========================================

This project is a solution to the Kaggle competition "Titanic - Machine Learning from Disaster", where the goal is to predict whether a passenger survived the Titanic shipwreck based on features such as age, sex, class, etc.

📌 Objective
------------
To build and evaluate multiple machine learning models that classify passengers as Survived or Not Survived using the Titanic dataset.

📁 Dataset
----------
The dataset includes:
- train.csv — contains features and labels (Survived)
- test.csv — contains features without labels
- gender_submission.csv — a sample submission file

Features include:
- Pclass, Sex, Age, SibSp, Parch, Fare, Embarked, etc.

🧰 Technologies Used
---------------------
- Python 3
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- XGBoost, LightGBM

⚙️ Workflow
-----------
1. Data Loading
   - Load the training and test datasets using pandas.
   - Display dataset structure and check for missing values.

2. Data Preprocessing
   - Impute missing values for Age, Embarked, and Fare.
   - Encode categorical variables using LabelEncoder.
   - Feature engineering:
     - Create a new feature Family_Size.
     - Bin ages into categorical ranges.

3. Exploratory Data Analysis (EDA)
   - Visualize survival rates by gender, class, age bins, etc.
   - Correlation heatmap.

4. Model Building
   Trained and evaluated the following models:
   - Logistic Regression
   - K-Nearest Neighbors
   - Random Forest Classifier
   - XGBoost Classifier
   - LightGBM Classifier
   - Voting Classifier (ensemble)

   Used train_test_split and performance metrics like accuracy, confusion matrix, and classification report.

5. Submission
   - Selected the best-performing model.
   - Predicted survival on test data.
   - Prepared a submission.csv file for Kaggle.


📁 Output
---------
The final output is a CSV file:
submission.csv with two columns:
- PassengerId
- Survived (0 or 1)

🚀 How to Run
-------------
1. Clone the repository or download the notebook.
2. Upload to Google Colab or run in Jupyter Notebook.
3. Ensure required libraries are installed.
4. Run all cells to preprocess data, train models, and generate submission.

✍️ Author
---------
Developed by [Your Name] as part of Kaggle Titanic competition practice.
