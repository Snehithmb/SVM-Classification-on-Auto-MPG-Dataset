# SVM Classification on Auto MPG Dataset

Google colab link -- https://colab.research.google.com/drive/1iucAgtz0YJKPW_sphxfYWAdGJZv3a_3v

This project demonstrates how to apply **Support Vector Machines (SVM)** using scikit-learn to classify cars based on fuel efficiency (MPG). The dataset used is a modified version of the **Auto MPG dataset**, where we classify vehicles into **high-MPG** and **low-MPG** classes.

---

## What You'll Learn

- How to prepare real-world data for SVMs
- Margin maximization using linear and non-linear (RBF) kernels
- The Kernel Trick for non-linear decision boundaries
- Hyperparameter tuning (`C`, `gamma`) using `GridSearchCV`
- Cross-validation to evaluate model performance
- PCA for 2D decision boundary visualization

---

## Tools & Libraries

- Python 3.x
- [Pandas](https://pandas.pydata.org/)
- [NumPy](https://numpy.org/)
- [Scikit-learn](https://scikit-learn.org/)
- [Matplotlib](https://matplotlib.org/)

---

## Dataset Description

| Feature        | Description                       |
|----------------|-----------------------------------|
| `horsepower`   | Engine horsepower                 |
| `weight`       | Vehicle weight (lbs)              |
| `mpg`          | Miles per gallon (target variable)|

The dataset is cleaned (missing values removed), and MPG is converted into a **binary label**:
- `1`: High MPG (above median)
- `0`: Low MPG (below or equal to median)

---

## Tasks Performed

1. Data loading and cleaning
2. Feature selection: `horsepower`, `weight`
3. Target encoding: Binary classification of `mpg`
4. Scaling features using `StandardScaler`
5. Training two SVMs:
   - Linear kernel
   - RBF kernel
6. Model evaluation using `classification_report`
7. Visualizing the decision boundary using PCA
8. Hyperparameter tuning using `GridSearchCV`
9. Cross-validation to check model robustness

---

## Example Output

- **Classification Accuracy** using Linear and RBF Kernels
- **Best Parameters** from GridSearchCV
- **Decision boundary** plotted using PCA

![SVM Decision Boundary](https://via.placeholder.com/400x300.png?text=Decision+Boundary+Plot)

---

## ▶How to Run

1. Clone this repo:
   ```bash
   git clone https://github.com/your-username/svm-auto-mpg.git
   cd svm-auto-mpg
