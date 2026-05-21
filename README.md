# 🚗 Linear Regression on Automobile Dataset

This project demonstrates how to perform **Data Preprocessing, Encoding Techniques, and Linear Regression** using Python and Machine Learning libraries on an Automobile Dataset.

The notebook covers:
- Data Loading
- Data Exploration
- Handling Categorical Data
- Label Encoding
- One Hot Encoding
- Building a Linear Regression Model
- Model Evaluation


# 📂 Project Structure

├── Auto Data Set.csv  
├── Day 30_Linear Regression_Auto Data Set.ipynb  
└── README.md  



# 📌 Problem Statement

The objective of this project is:

> To predict the price of vehicles using various independent features from the automobile dataset.



# 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Seaborn
- Scikit-Learn



# 📚 Libraries Used

```python
import pandas as pd
import numpy as np
import seaborn as sns

from sklearn.linear_model import LinearRegression
from sklearn.model_selection import train_test_split
from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score
from sklearn.preprocessing import LabelEncoder, OneHotEncoder
📊 Dataset Information

The dataset contains automobile specifications such as:

Make
Fuel Type
Engine Type
Horsepower
Wheel Base
Height
Width
MPG
Price
and many more...
Dataset Shape
Rows: 205
Columns: 26
🔍 Steps Performed
1. Data Gathering

Loaded the dataset using Pandas.

df = pd.read_csv("Auto Data Set.csv")
2. Data Exploration

Performed:

df.head()
df.shape
df.info()
value_counts()

to understand the dataset structure and feature types.

🔐 Encoding Techniques

This project explains different encoding methods used in Machine Learning.

✅ Label Encoding

Converted categorical labels into numerical values.

Example:

Category	Encoded Value
Low	0
Medium	1
High	2

Example code:

labelEnc = LabelEncoder()
labelEnc.fit_transform(df['num-of-cylinders'])
✅ Manual Encoding
df['num-of-cylinders'].replace({
    'four':4,
    'six':6,
    'five':5,
    'three':3,
    'twelve':12,
    'two':2,
    'eight':8
}, inplace=True)
✅ One Hot Encoding

Used to convert categorical values into binary columns.

Example:

Gender	Male	Female
Male	1	0
Female	0	1
🤖 Machine Learning Model

Used Linear Regression model from Scikit-Learn.

model = LinearRegression()
📈 Model Evaluation Metrics

The following evaluation metrics were used:

Mean Absolute Error (MAE)
Mean Squared Error (MSE)
R² Score
mean_absolute_error()
mean_squared_error()
r2_score()
🚀 How to Run the Project
Step 1: Clone Repository
git clone https://github.com/your-username/your-repo-name.git
Step 2: Install Dependencies
pip install pandas numpy seaborn scikit-learn
Step 3: Run Jupyter Notebook
jupyter notebook

Open the notebook file and run all cells.

📷 Output

The notebook demonstrates:

Data preprocessing
Encoding categorical variables
Building a regression model
Predicting automobile prices
🎯 Learning Outcomes

By completing this project, you will learn:

Data preprocessing
Handling categorical data
Encoding techniques
Linear Regression basics
Model evaluation
Machine Learning workflow
📌 Future Improvements
Feature Engineering
Missing Value Handling
Hyperparameter Tuning
Advanced Regression Models
Visualization Dashboard

👨‍💻 Author
Neha Pingale
