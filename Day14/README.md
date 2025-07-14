# Logistic Regression

## Overview

Logistic Regression is a supervised machine learning algorithm used for classification problems.  
Unlike Linear Regression, which predicts continuous values, Logistic Regression predicts the probability that an input belongs to a specific class.  
It is primarily used for **binary classification**, but it can also handle multiple classes.

Logistic Regression uses the **sigmoid function** (for binary) or **softmax function** (for multinomial) to convert inputs into probability values.

---

## Types of Logistic Regression

1. **Binomial Logistic Regression**
   - The dependent variable has only two categories (e.g., Yes/No, 0/1).
   - Example use cases: Spam detection, pass/fail prediction.

2. **Multinomial Logistic Regression**
   - The dependent variable has three or more **unordered** categories (e.g., classifying animals into cat, dog, sheep).
   - Uses the softmax function.

3. **Ordinal Logistic Regression**
   - The dependent variable has three or more **ordered** categories (e.g., low, medium, high).
   - Takes the natural order into account.

---

## Binomial Logistic Regression Example

```python
from sklearn.datasets import load_breast_cancer
from sklearn.linear_model import LogisticRegression
from sklearn.model_selection import train_test_split
from sklearn.metrics import accuracy_score

# Load dataset
X, y = load_breast_cancer(return_X_y=True)

# Split dataset
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.20, random_state=23)

# Train model
clf = LogisticRegression(max_iter=10000, random_state=0)
clf.fit(X_train, y_train)

# Evaluate
acc = accuracy_score(y_test, clf.predict(X_test)) * 100
print(f"Logistic Regression model accuracy: {acc:.2f}%")
```

## References

- `Day14.pdf` — Full notes & examples  
- [scikit-learn Documentation](https://scikit-learn.org/stable/modules/linear_model.html#logistic-regression)

---

> "Logistic Regression: A simple yet powerful way to classify the world in 0s and 1s."
