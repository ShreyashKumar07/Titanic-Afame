# Titanic-Afame
This project was developed as part of an internship at Afame Technologies to predict the survivability of passengers aboard the Titanic.

Dataset
The dataset used for this project is named Titanic-Dataset.csv. It contains the following columns:

PassengerId: Unique identifier for each passenger
Survived: Binary indicator (0 = No, 1 = Yes) for whether the passenger survived
Pclass: Ticket class (1 = Upper, 2 = Middle, 3 = Lower)
Name: Passenger's name
Sex: Passenger's gender
Age: Passenger's age
SibSp: Number of siblings/spouses aboard the Titanic
Parch: Number of parents/children aboard the Titanic
Ticket: Ticket number
Fare: Passenger fare
Cabin: Cabin number
Embarked: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)
Files
Titanic Prediction Final.ipynb: Jupyter Notebook containing the code for data preprocessing, model training, and prediction.
Titanic-Predictions.csv: Final prediction file containing PassengerId and Survived columns.
README.md: This file, providing an overview of the project.
Workflow
Data Handling: Missing age values are filled using an AgeImputer. Categorical variables (Embarked) are converted to numerical values using OneHotEncoder. Unnecessary columns (Name, Ticket, Cabin, Sex) are dropped using FeatureDropper. All these steps are encapsulated in a pipeline from sklearn.

Data Scaling: StandardScaler is used to scale the data before training the model.

Model Training: RandomForestClassifier is used as the predictive model. GridSearchCV is employed to tune hyperparameters for optimal performance.

Prediction: The trained model is used to make predictions on the test dataset.

Usage
To replicate the analysis and predictions:

Clone the repository to your local machine.
Ensure you have the necessary dependencies installed (Pandas, NumPy, Matplotlib, Seaborn, scikit-learn).
Open and run the Titanic Prediction Final.ipynb notebook in Jupyter environment.
Review the predictions in Titanic-Predictions.csv.
