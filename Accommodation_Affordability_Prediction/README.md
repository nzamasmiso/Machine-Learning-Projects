# Accommodation Affordability Classification
This project focuses on solving a supervised machine learning classification problem using accommodation data. 
The goal is to predict the **Affordability** of accommodation listings based on different features such as city, 
accommodation type, safety rating, and distance from the city centre.

The project includes:
- Data loading and inspection
- Exploratory Data Analysis (EDA)
- Data preprocessing
- Feature engineering
- Model training
- Model evaluation
- Comparison of machine learning algorithms

---

# Technologies Used
- Python
- Pandas
- NumPy
- Seaborn
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

# Dataset
Dataset used:
- `Accomodation.csv`

The dataset contains:
- Numerical features
- Categorical features
- Missing values
- A target variable called `Affordability`

---

# Project Workflow

## 1. Data Loading and Inspection
The dataset was loaded into a pandas DataFrame and explored using:
- `head()`
- `tail()`
- `describe()`
- `info()`

This helped identify:
- Data types
- Missing values
- Feature distributions
- Potential outliers

---

## 2. Data Preprocessing

### Missing Value Handling
- Numerical features were filled using the **mean**
- Categorical features were filled using the **mode**

### Encoding
- Label Encoding was applied to:
  - `Day`
  - `Type`

- One-Hot Encoding was applied to:
  - `City`

### Log Transformation
Log transformation was applied to:
- `Safety Rating`
- `City Centre Distance (km)`

This helped reduce skewness and improve feature distributions.

---

# Exploratory Data Analysis (EDA)

Visualisations created:
- Countplots
- Distribution plots
- Correlation heatmap

EDA helped identify:
- Class imbalance
- Feature distributions
- Correlations
- Potential outliers
- Relationships between variables

---

# Machine Learning Models Used

## Logistic Regression
A linear classification algorithm used as a baseline model.

### Evaluation Metrics:
- Confusion Matrix
- Classification Report
- Accuracy Score

---

## Random Forest Classifier
An ensemble learning algorithm capable of capturing nonlinear relationships.

### Evaluation Metrics:
- Confusion Matrix
- Classification Report
- Accuracy Score

---

# Model Evaluation

The models were evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

The comparison showed differences in performance between linear and nonlinear models.

---

# No Free Lunch Theorem

The project also discusses the No Free Lunch theorem, which states that:
> No single machine learning algorithm performs best on every dataset.

This explains why one model may outperform another depending on the structure and characteristics of the data.

---

# Key Observations
- Data preprocessing significantly improves model readiness
- Encoding categorical variables is essential for machine learning
- Log transformation helps reduce skewness
- Random Forest can capture complex patterns better than Logistic Regression
- Accuracy alone is not always sufficient for evaluating classification performance

---

# How to Run the Project

## Step 1: Clone the Repository
```bash
git clone <your-github-repo-link>
```

## Step 2: Open the Project Folder
```bash
cd Accommodation_Affordablity_Prediction
```

## Step 3: Launch Jupyter Notebook
```bash
jupyter notebook
```

## Step 4: Open the Notebook
Open the `.ipynb` notebook file and run all cells.

---

# Repository Structure

```text
MALE402_Assignment1_Accommodation_Classification/
│
├── Accomodation.csv
├── Accomodation_Affordability_Classification.ipynb
├── README.md
└── requirements.txt
```

---

# Author
Smiso Luyanda Nzama  
