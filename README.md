# Titanic-Survival-Prediction 🚢

## Project Description
The **Titanic Survival Prediction** project focuses on predicting the survival outcomes of passengers aboard the Titanic using machine learning techniques. This project leverages passenger data, such as age, gender, class, and other attributes, to build classification models capable of identifying survival probabilities. By employing systematic data preprocessing, exploratory data analysis (EDA), and robust machine learning pipelines, the project aims to provide a comprehensive approach to understanding survival factors and enhancing predictive accuracy.

This project serves as an academic exploration of predictive modeling, with detailed documentation, reproducible workflows, and insights that bridge theoretical concepts and practical applications in the field of data science.

---

## Project Structure

```
Titanic-Survival-Prediction/
├── data/               
├── notebooks/          
├── docs/               
├── README.md           
└── requirements.txt    
```

---

## Workflow

### **1. Data Exploration**
- Perform exploratory data analysis (EDA) to identify key trends and distributions in the dataset.
- Visualize survival distributions across different categories such as passenger class, age, and gender.
- Analyze correlations between features to determine their potential impact on survival outcomes.

### **2. Preprocessing**
- **Handle Missing Data:**
  - Impute missing ages using median values or predictive modeling.
  - Fill missing embarked values with the mode.
- **Feature Engineering:**
  - Encode categorical variables (e.g., Gender, Embarked) using one-hot encoding.
  - Create new features such as family size, title extraction from names, or ticket grouping.
- **Normalize Data:**
  - Scale numerical features (e.g., Age, Fare) to improve model performance.

### **3. Modeling**
- Train predictive models using:
  - **Logistic Regression**: A baseline model for binary classification.
  - **Random Forest**: To capture non-linear relationships and feature importance.
  - **XGBoost**: For advanced gradient boosting and handling imbalanced data.

### **4. Model Evaluation**
- Evaluate models using metrics such as:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - ROC-AUC
- Perform cross-validation to ensure the robustness of model performance.

### **5. Results Interpretation**
- Visualize model performance using confusion matrices, precision-recall curves, and feature importance plots.
- Document insights on significant predictors of survival, such as passenger class, gender, and age.

---

## How to Run the Project

1. Clone this repository:
   ```bash
   git clone https://github.com/2AM-Labs/Titanic-Survival-Prediction.git
   ```
2. Navigate to the project folder:
   ```bash
   cd Titanic-Survival-Prediction
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the notebook for exploration and modeling:
   ```bash
   jupyter notebook notebooks/titanic_analysis.ipynb
   ```

---

## Technologies Used

- **Programming Language:** Python 3.9+
- **Libraries and Tools:**
  - **Pandas:** For data cleaning and manipulation.
  - **NumPy:** For numerical operations.
  - **Scikit-learn:** For machine learning models and evaluation metrics.
  - **XGBoost:** For advanced gradient boosting.
  - **Matplotlib & Seaborn:** For data visualization.
  - **Jupyter Notebook:** For interactive experimentation and documentation.

---

## Dataset Information
- **Source:** [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic)
- **Files:**
  - `train.csv`: Training dataset containing features and survival labels.
  - `test.csv`: Test dataset for making predictions.
  - `gender_submission.csv`: Baseline predictions for comparison.

---

## Results and Analysis
- **Key Model Performance Metrics:**
  - Logistic Regression: Accuracy = ...
  - Random Forest: Accuracy = ...
  - XGBoost: Accuracy = ...
- **Insights:**
  - Gender (female) and higher class (1st class) significantly increased survival probabilities.
  - Age played a crucial role, with younger passengers having higher survival rates.

---

## Documentation and Resources
- **Presentation Deck:** [Canva Titanic Presentation](https://www.canva.com/design/DAFwAGR05Do/jUbQsT2sqDrDY_2KkexYtw/view?utm_content=DAFwAGR05Do&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=h08133543cb)
- **Notebooks:** Jupyter notebooks with detailed steps for data analysis and modeling are available in the `notebooks/` folder.
- **Technical Reports:** Additional findings and documentation can be found in the `docs/` folder.

---

## Contribution Guidelines

1. Fork this repository.
2. Create a new branch for features or fixes:
   ```bash
   git checkout -b feature-branch-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Description of changes"
   ```
4. Push to your branch:
   ```bash
   git push origin feature-branch-name
   ```
5. Create a pull request on GitHub.

---

# requirements.txt

```
pandas
numpy
scikit-learn
xgboost
matplotlib
seaborn
jupyter