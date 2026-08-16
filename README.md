# 🧠 ML-Fundamentals

A structured collection of Machine Learning practice notebooks — covering the
full workflow from raw data to trained models: preprocessing, regression,
classification, ensemble learning, and unsupervised learning.

![Python](https://img.shields.io/badge/Python-3.13-blue)
![scikit--learn](https://img.shields.io/badge/scikit--learn-ML-orange)
![Status](https://img.shields.io/badge/Status-Learning%20%2F%20Practice-yellow)

---

## 📁 Folder Structure

```
ML-Projects/
├── 01_Data_Preprocessing/       # Imputation, Outliers, Encoding, Scaling, Imbalanced Data, Train-Test Split
│   ├── 01_Imputation.ipynb
│   ├── 02_Outlier_Detection.ipynb
│   ├── 03_Encoding.ipynb
│   ├── 04_Scaling.ipynb
│   ├── 05_Imbalanced_Data_Handling.ipynb
│   ├── 06_Training_Testing_Split.ipynb
│   └── README.md
├── 02_Regression/                # Linear & Polynomial Regression
│   ├── 01_Linear_Regression.ipynb
│   ├── 02_Polynomial_Regression.ipynb
│   └── README.md
├── 03_Classification/            # KNN, Decision Tree, Random Forest, Logistic Regression
│   ├── 01_KNN_Classifier.ipynb
│   ├── 02_Decision_Tree.ipynb
│   ├── 03_Random_Forest_vs_Decision_Tree.ipynb
│   ├── 04_Logistic_Regression_Task.ipynb
│   └── README.md
├── 04_Ensemble_Learning/         # Boosting Algorithms
│   ├── 01_Boosting_Algorithms.ipynb
│   └── README.md
├── 05_Unsupervised_Learning/     # Clustering / Unsupervised ML
│   ├── 01_Unsupervised_ML.ipynb
│   └── README.md
├── 06_Practice_and_Misc/         # Practice notebooks & draft tasks
│   ├── 01_KNN_Visualization_Practice.ipynb
│   ├── 02_Read_File_Task.ipynb
│   └── README.md
├── datasets/                     # Shared CSV datasets used across notebooks
│   ├── Social_Network_Ads.csv
│   └── README.md
└── README.md                     # You are here
```

Each subfolder has its own `README.md` explaining exactly what every notebook does.

---

## 🚀 Getting Started

**1. Clone the repo**
```bash
git clone <your-repo-url>
cd ML-Projects
```

**2. Install dependencies**
```bash
pip install pandas numpy scikit-learn matplotlib jupyter
```

**3. Launch Jupyter**
```bash
jupyter notebook
```

**4. Dataset paths**
Notebooks that read a CSV (e.g. `Social_Network_Ads.csv`) look for it relative to
their own folder by default. Update the `pd.read_csv(...)` path to point to
`../datasets/<filename>.csv` if a notebook can't find the file.

---

## 📚 Topics Covered

| Category | Concepts |
|---|---|
| **Data Preprocessing** | Missing value imputation, outlier detection, Label/One-Hot/Ordinal encoding, MinMax/Standard/Robust scaling, imbalanced data handling, train-test splitting |
| **Regression** | Linear Regression, Polynomial Regression |
| **Classification** | K-Nearest Neighbors, Decision Tree, Random Forest, Logistic Regression |
| **Ensemble Learning** | Boosting |
| **Unsupervised Learning** | Clustering |

---

## 🛠️ Tech Stack

- **Language:** Python 3.13
- **Libraries:** pandas, numpy, scikit-learn, matplotlib

---

## ⚠️ Known Issues

- `06_Practice_and_Misc/01_KNN_Visualization_Practice.ipynb` — the scatter plot cell throws a `NameError: name 'X' is not defined`; needs a fix before it runs end-to-end.
- `03_Classification/04_Logistic_Regression_Task.ipynb` — expects a `ChurnData.csv` file that isn't included in `datasets/`; add it before running.

---

## 🗺️ Roadmap

- [ ] Fix the KNN visualization NameError
- [ ] Add the missing ChurnData dataset
- [ ] Add model comparison summary notebook
- [ ] Add cross-validation examples

---

## 👤 Author

**Naveen** — AI/ML enthusiast, building this repo as a hands-on ML practice log.
