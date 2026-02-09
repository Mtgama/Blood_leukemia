# Five-Year Survival Analysis in Pediatric Leukemia Using Machine Learning

## Project Overview
This project analyzes clinical and laboratory factors associated with survival outcomes in pediatric leukemia patients using supervised machine learning models.  

The primary objective is to predict treatment outcomes (survival vs. death) and identify key prognostic variables.

---

## Dataset Description
- Total samples: 259 pediatric patients  
- Features: Demographic, clinical, laboratory, metastasis indicators, organ involvement, and blood group  
- Target variable: **Treatment Outcome** (0 = Death, 1 = Survival)

### Key Variables
- Gender
- Age
- Brain metastasis (binary)
- Testicular metastasis (binary)
- Splenomegaly
- Hepatomegaly
- Leukemia type (ALL / AML)
- Blood group (One-Hot Encoded)

---

## Data Preprocessing
- Encoding categorical variables
- Binary transformation of metastasis and clinical indicators
- One-hot encoding for blood groups
- Removal of irrelevant features (IDs, dates, descriptive text)
- Missing value handling
- Feature scaling using `StandardScaler`
- Train-test split (85% train / 15% test)

---

## Exploratory Data Analysis
- Diagnosis distribution by gender
- Mean age comparison between genders
- Mortality comparison by gender
- Survival comparison across age groups
- Metastasis distribution analysis

Visualization tools:
- Matplotlib
- Seaborn

---

## Machine Learning Models

### 1. Decision Tree (Entropy)
Accuracy: **0.718**

### 2. Random Forest (Entropy)
Accuracy: **0.795**

### 3. CatBoost Classifier
- Iterations: 1000
- Learning rate: 0.1
- Depth: 6  
(Performance evaluated using LogLoss and validation set monitoring)

---

## Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-score
- Classification Report

---

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- CatBoost
- Matplotlib
- Seaborn

---

## Conclusion
Ensemble-based methods (Random Forest, CatBoost) demonstrated improved predictive performance compared to a single Decision Tree model.  

The findings suggest that clinical features such as metastasis indicators and leukemia subtype play a significant role in predicting survival outcomes.

---

## Author
Mehrdad Hassanzadeh  
M.Sc. Medical Informatics
