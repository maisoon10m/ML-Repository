# SVM Classification on the Iris Dataset

A machine learning assignment that applies **Support Vector Machines (SVM)** to classify iris flower species using the classic Iris dataset. It covers the full ML workflow: data loading, exploratory data analysis, model training, evaluation, and hyperparameter tuning with GridSearchCV.

---

## Dataset

This assignment uses the famous **Iris flower dataset**, originally introduced by Sir Ronald Fisher in 1936. It is one of the most well-known datasets in pattern recognition and machine learning.

### Source

The dataset is **built-in** and loaded directly from the `seaborn` library — no external download required:

​```python
import seaborn as sns
iris = sns.load_dataset('iris')
​```

> **Note:** The same dataset is also available via `sklearn.datasets.load_iris()`. The seaborn version is used here because it returns a clean pandas DataFrame with named columns, which is convenient for the visualization steps.

### Description

The dataset contains **150 samples** of iris flowers, evenly distributed across **3 species** (50 samples each):

| Class | Samples |
|---|---|
| Iris-setosa | 50 |
| Iris-versicolor | 50 |
| Iris-virginica | 50 |

### Features

Each sample has **4 numerical features** measured in centimeters:

| Feature | Description |
|---|---|
| `sepal_length` | Length of the sepal (cm) |
| `sepal_width` | Width of the sepal (cm) |
| `petal_length` | Length of the petal (cm) |
| `petal_width` | Width of the petal (cm) |

### Target

- `species` — The flower species (categorical: `setosa`, `versicolor`, `virginica`)

---

## Project Workflow

1. **Load the data** using seaborn's built-in dataset.
2. **Exploratory Data Analysis (EDA)**
   - Pairplot of all features colored by species
   - 2D KDE plot of sepal dimensions for the *setosa* species
3. **Train/Test Split** — 70% training, 30% testing (`random_state=101`)
4. **Train SVM Model** — Default `SVC()` from scikit-learn
5. **Evaluate** — Confusion matrix and classification report
6. **Hyperparameter Tuning** — `GridSearchCV` over `C` and `gamma`
7. **Compare Results** — Default model vs. tuned model

---

## 🛠️ Requirements

- Python 3.7+
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- jupyter

Install all dependencies with:

​```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
​```

---

## How to Run

1. Clone the repository:
   ​```bash
   git clone <your-repo-url>
   cd <your-repo-name>
   ​```
2. Launch Jupyter:
   ​```bash
   jupyter notebook
   ​```
3. Open `02-SVM_Assignment.ipynb` and run the cells in order.

---

## Results

The SVM classifier achieved **~98% accuracy** on the test set, correctly classifying 44 out of 45 test samples. GridSearchCV explored 16 combinations of `C` and `gamma` but did not improve on the default model — the Iris dataset is small and well-separated, leaving little room for tuning gains.

| Model | Accuracy |
|---|---|
| Default `SVC()` | ~98% |
| GridSearch-tuned SVC | ~98% |

The most separable class is **Iris-setosa**, which forms a clearly distinct cluster in the pairplot. The remaining misclassifications occur between *versicolor* and *virginica*, which overlap slightly in feature space.

---
