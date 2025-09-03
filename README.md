# Feature Selection and Transformations

This repository contains code for **Feature Selection** and **Feature Transformation (Scaling & Normalization)** using Python libraries like Pandas, Matplotlib, Seaborn, and Scikit-learn.

---

## 📂 Dataset

The dataset used is `mobile.csv`, which contains mobile specifications with features such as battery power, RAM, pixel resolution, etc.

---

## 🧾 Steps Performed

### 1. Feature Selection

Feature selection helps in identifying the most relevant features for building models.

* **Correlation Analysis**: Identify correlation between numerical features.
* **Heatmap Visualization**: Plot correlation heatmap for better visualization.
* **Dropping Unnecessary Features**: Remove highly correlated/redundant features.
* **Univariate Feature Selection**: Using statistical tests to select the best features.
* **Recursive Feature Elimination (RFE)**: Select features by recursively considering smaller feature sets.

### 2. Feature Transformation

Feature transformation ensures that the dataset is scaled, normalized, and suitable for machine learning models.

#### 🔹 Normalization

* Scales features to a fixed range **\[0,1]**.
* Formula: $X' = \frac{X - X_{min}}{X_{max} - X_{min}}$
* Useful when features have varying ranges.

#### 🔹 Standardization

* Scales features to have **zero mean** and **unit variance**.
* Formula: $X' = \frac{X - \mu}{\sigma}$
* Suitable for algorithms assuming normally distributed data (e.g., Logistic Regression, SVM).

#### 🔹 Min-Max Scaling

* Alternative form of normalization.
* Compresses all values between 0 and 1.
* Preserves relationships but can be sensitive to outliers.

#### 🔹 Robust Scaling

* Uses **median** and **interquartile range (IQR)** instead of mean and variance.
* Formula: $X' = \frac{X - Median}{IQR}$
* Works well when the dataset has outliers.

#### 🔹 Log Transformation

* Reduces **skewness** of features.
* Applies natural log: $X' = log(X+1)$
* Helps when data has a long tail distribution.

#### 🔹 Gaussian Transformation

* Transforms features to follow a Gaussian-like (normal) distribution.
* Useful for models sensitive to non-Gaussian features.

---

## 📊 Visualization

* Heatmaps for correlation.
* Distribution plots before & after transformation.
* Boxplots to visualize scaling effects.

---

## ⚙️ Libraries Used

* **pandas** → Data handling
* **matplotlib** → Plotting
* **seaborn** → Statistical visualization
* **sklearn** → Feature selection and transformation

---

## 🚀 How to Run

```bash
pip install pandas matplotlib seaborn scikit-learn
python feature_selection.py
```

---

## ✅ Summary

* Performed **Feature Selection** to reduce irrelevant features.
* Applied multiple **Feature Transformation methods**: Normalization, Standardization, Min-Max Scaling, Robust Scaler, Log Transform, and Gaussian Transformation.
* Ensured the dataset is ready for **Machine Learning Models**.



## 📬 Contact

Maintained by **Balaji Kudumu**  
If you use this project in your research, please give appropriate credit.

---

## 📄 License

MIT License - see `LICENSE` file for details.
