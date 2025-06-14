# Decision-Trees
# 🎓 Student Performance Predictor

This project uses a Decision Tree Classifier to predict whether a student will **pass or fail** based on various demographic, academic, and behavioral factors from the UCI Student Performance dataset.

## 📂 Dataset

The dataset used is [`student-mat.csv`](https://archive.ics.uci.edu/ml/datasets/Student+Performance) from the UCI Machine Learning Repository. It contains attributes like:
- Age, gender, address type
- Parental education and job
- Study time, past failures, absences
- Alcohol consumption, health, internet access
- Grades (G1, G2, G3)

---

## 🧠 Objective

Predict whether a student will **pass** (final grade G3 ≥ 10) using a Decision Tree Classifier. This simplifies the regression task to a binary classification problem.

---

## 🛠️ Tech Stack

- Python 🐍
- Pandas & NumPy
- Scikit-learn
- Matplotlib (for tree visualization)

---

## 🚀 How It Works

1. **Load and Preprocess** the dataset
2. Convert final grade (G3) into binary target: `pass = 1 if G3 >= 10 else 0`
3. Encode categorical variables using one-hot encoding
4. Train a Decision Tree on the data
5. Evaluate the model using accuracy and classification report
6. Visualize the decision tree

---

## 📈 Example Output

```plaintext
✅ Accuracy: 0.9113924050632911
📋 Classification Report:
               precision    recall  f1-score   support

           0       0.86      0.89      0.87        27
           1       0.94      0.92      0.93        52

    accuracy                           0.91        79
   macro avg       0.90      0.91      0.90        79
weighted avg       0.91      0.91      0.91        79
