# 🚀 Spaceship Titanic — Machine Learning Classification

End-to-end Machine Learning solution for the  
[Kaggle Spaceship Titanic competition](https://www.kaggle.com/competitions/spaceship-titanic).

---

## 📌 Project Overview

The objective is to predict whether a passenger was **transported to an alternate dimension** following the Spaceship Titanic’s collision with a spacetime anomaly.

**Best Model Performance**  
- **Model:** `HistGradientBoostingClassifier`  
- **Accuracy:** ~81.3%

---

## 📁 Project Structure

```text
├── Data/                    # Dataset files (ignored by git)
│   ├── train.csv
│   └── test.csv
├── spaceship_titanic.ipynb  # Main Jupyter Notebook (full ML pipeline)
├── .gitignore               # Ignored files (CSV, configs, etc.)
└── README.md                # Project documentation
```

## ⚙️ Methodology

1. **Feature Engineering:**
   * Extracted `Deck` and `Side` from the `Cabin` column.
   * Created a `TotalSpend` feature by aggregating luxury amenities.

2. **Preprocessing Pipeline:**
   * **Numerical Data:** Median imputation + Standard Scaling.
   * **Categorical Data:** Most frequent imputation + One-Hot Encoding.

3. **Model Selection:**
   * Tested multiple classifiers: Logistic Regression, KNN, SVM, Random Forest, Gradient Boosting, Naive Bayes.
   * Used `GridSearchCV` for hyperparameter tuning.

4. **Final Model:**
   * Selected **HistGradientBoostingClassifier** as the top performer.

## 🚀 How to Run

1. **Clone the repository:**
  ```
   git clone [https://github.com/RaoufKessouar/spaceship-titanic-classifier.git](https://github.com/RaoufKessouar/spaceship-titanic-classifier.git)
   cd spaceship-titanic-classifier
  ```

2. **Download the Data:**
   * Download `train.csv` and `test.csv` from the [Kaggle Competition Page](https://www.kaggle.com/competitions/spaceship-titanic/data).
   * Create a folder named `Data` in the root directory.
   * Place the CSV files inside the `Data/` folder so the structure looks like this:
     * `Data/train.csv`
     * `Data/test.csv`

3. **Run the Notebook:**
   * Open `spaceship_titanic.ipynb` in Jupyter Notebook, VS Code, or Google Colab.
   * Run all cells to train the model and generate predictions.

## 👤 Author
[RaoufKessouar](https://github.com/RaoufKessouar)
