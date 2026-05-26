# Ensemble Learning for Accommodation Affordability
This assignment focuses on applying and comparing different ensemble learning
techniques for predicting accommodation affordability using machine learning.

The project investigates how combining multiple models can improve prediction
accuracy and overall model performance compared to using a single classifier.

The following machine learning approaches were implemented:
- Logistic Regression
- Gaussian Naive Bayes
- Decision Tree Classifier
- Voting Classifier
- Stacking Classifier
- Bagging Classifier
- AdaBoost Classifier

---

# Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

# Dataset

Dataset used:
- `Accommodation2.csv`

Target variable:
- `Affordability`

The dataset was divided into:
- Training data
- Testing data

using `train_test_split()` with:
- `test_size = 0.25`
- `random_state = 5`

---

# Machine Learning Models and Results

| Model | Accuracy |
|------|------|
| GaussianNB | 75.32% |
| Logistic Regression | 79.28% |
| Decision Tree Classifier | 85.81% |
| Voting Classifier | 82.76% |
| Stacking Classifier | 85.82% |
| Bagging Classifier | 87.92% |
| AdaBoost Classifier | 83.56% |

---

# Ensemble Learning Techniques

## 1. Hard Voting
The VotingClassifier combined:
- GaussianNB
- LogisticRegression
- DecisionTreeClassifier

using majority voting (`voting='hard'`).

This method improved stability by combining predictions from multiple models.

---

## 2. Stacking
The StackingClassifier used:
- DecisionTreeClassifier
- SVC

as base learners, with:
- LogisticRegression

as the final estimator.

Stacking achieved one of the highest accuracy scores because it learns how to
best combine predictions from different models.

---

## 3. Bagging
BaggingClassifier used:
- DecisionTreeClassifier

as the base estimator.

Bagging achieved the highest accuracy score of 87.92%.
This method reduces overfitting by training multiple models on random subsets
of the dataset.

---

## 4. Boosting
AdaBoostClassifier used:
- DecisionTreeClassifier(max_depth=8, class_weight='balanced')

as the weak learner.

Boosting improved performance by focusing more on incorrectly classified samples
during training.

---

# Key Observations

- Ensemble learning methods generally performed better than single models.
- Decision tree-based methods produced the strongest results.
- Bagging achieved the best overall accuracy.
- GaussianNB produced the lowest accuracy because of its strong assumptions
  about feature independence.
- Stacking effectively combined multiple learning approaches.
- Voting improved model robustness but was influenced by weaker classifiers.
- Boosting performed well but was slightly more sensitive to difficult data.

---

# Conclusion

The assignment demonstrated the importance of ensemble learning in machine
learning problems. Combining multiple classifiers helped improve prediction
accuracy, reduce overfitting, and increase model stability.

Among all the models tested, BaggingClassifier achieved the best performance,
showing that ensemble methods based on decision trees are highly effective
for complex datasets.

---

# How to Run the Project

## Step 1: Clone the Repository

```bash
git clone <your-github-repository-link>
```

## Step 2: Open the Project Folder

```bash
cd Accommodation_Ensembe_Classification
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
Accommodation_Ensembe_Classification/
│
├── Accommodation2.csv
├── Assignment2.ipynb
├── README.md

```

---

# Author

Smiso Luyanda Nzama  
