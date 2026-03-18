🌧️ Rainfall Prediction using Machine Learning

📌 Overview

This project is focusing on predicting rainfall using historical weather data. A complete machine learning pipeline is being implemented, including data preprocessing, feature engineering, model training, and evaluation.

---

📂 Dataset

* Source: `weatherHistory.csv`
* The dataset is containing weather-related attributes such as:

  * Temperature
  * Humidity
  * Wind Speed
  * Wind Bearing
  * Pressure
  * Other environmental factors

---

⚙️ Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn

---
 🔄 Workflow

1. Data Loading

* Reading dataset using Pandas
* Inspecting structure using `.head()` and `.info()`

2. Data Preprocessing

* Handling missing values (if any)
* Converting features into usable format

3. Feature Engineering

* Transforming wind direction into:

  * `wind_x = cos(theta)`
  * `wind_y = sin(theta)`
* Dropping original wind bearing column

### 4. Data Splitting

* Splitting dataset into training and testing sets
* Maintaining proper ratio for evaluation

5. Model Training

* Implementing:

  * Linear Regression
  * Random Forest

6. Model Evaluation

Classification Metrics:

* Accuracy
* Precision
* Recall
* F1-score

Regression Metrics:

* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)
* R² Score

---

📊 Results

🔹 Initial Model Performance

* Accuracy: 99.33%
* Precision: 99.73%
* Recall: 99.52%
* F1-score: 99.62%

🔹 Regression Performance

* R² Score: 0.38
* RMSE: 0.247

### 🔹 Random Forest Performance

* Accuracy: 91.94%
* RMSE: 0.284

---

🚀 Future Improvements

* Handling class imbalance using techniques like:

  * SMOTE
  * Class weighting
* Hyperparameter tuning for Random Forest
* Feature selection using importance scores
* Cross-validation for better evaluation
* Trying advanced models (XGBoost, LightGBM)

---

▶️ How to Run

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

```bash
jupyter notebook finalrainfallpredictor.ipynb
```

---

📁 Project Structure

```
.
├── weatherHistory.csv
├── finalrainfallpredictor.ipynb
└── README.md
```

---
📌 Conclusion

This project is demonstrating a complete machine learning workflow for rainfall prediction and is highlighting the importance of preprocessing, feature engineering, and model selection in achieving good performance.
