# Brain Stroke Prediction

This project applies exploratory data analysis (EDA) and machine learning models to predict the likelihood of stroke occurrence using patient demographic and medical history data.  
The aim is to identify high-risk individuals early and guide preventive healthcare strategies. 

---

##  Project Workflow

We evaluated model performance under three dataset conditions:
- **Case 1:** Imbalanced dataset (original)
- **Case 2:** Fully balanced dataset using SMOTE
- **Case 3:** Partially balanced dataset
- 
### 1. Data Loading & Cleaning
- Imported the dataset and handled missing values.
- Converted categorical variables into numerical form.
- Removed duplicates and corrected inconsistent data entries.

### 2. Exploratory Data Analysis (EDA)
- **Age Distribution**: Most patients were aged between 40–70 years.
- **Class Distribution**: Stroke cases were imbalanced, with fewer positive stroke cases.
- **Correlation Heatmap**: Found strong correlations between certain features (e.g., age, hypertension, heart disease).

### 3. Feature Engineering
- Created additional features like BMI categories and age groups.
- Normalized continuous variables for better model performance.

### 4. Model Building & Evaluation
- Tested multiple classification algorithms: Logistic Regression, Random Forest, Gradient Boosting, and XGBoost.
- Used metrics like Accuracy, Precision, Recall, F1-score, and ROC-AUC.
- **Feature Importance**: Identified key predictors such as age, average glucose level, and BMI.
- **Model Comparison**: Random Forest and XGBoost performed the best.

---

Key Visualizations & Insights

### 1️⃣ Case 1 – Class Distribution (Imbalanced Dataset)
![Class Distribution](./images/class_distribution.png)  
**Insight:** Stroke cases represent <1% of the dataset, leading to severe class imbalance and potential bias towards predicting non-stroke cases.

---

### 2️⃣ Case 1 – Age Distribution by Stroke Outcome
![Age Distribution](./images/AgeDistribution.png)  
**Insight:** Stroke cases are concentrated in the **40–80 age range**, while non-stroke cases dominate the younger range.  
This highlights the importance of age as a risk factor.

---

### 3️⃣ Case 1 – Correlation Heatmap
![Correlation Heatmap](./images/correlationheatmap.png)  
**Insight:**  
- Age, hypertension, and heart disease show the strongest positive correlation with stroke occurrence.
- Average glucose level and BMI also contribute moderately.

---

### 4️⃣ Case 1 – ROC AUC Curves (Model Comparison)
![Model Comparison](./images/modelcomparison.png)  
**Insight:**  
- Logistic Regression, Random Forest, and SVM were evaluated on the imbalanced dataset.
- ROC AUC scores were relatively low, reinforcing the need for balancing techniques.

---

### 5️⃣ Case 2 – Feature Importance (Best Model)
![Feature Importance](./images/featureimportance.png)  
**Insight:**  
- Age, average glucose level, and hypertension emerged as the top three predictive features.
- This information can directly guide healthcare monitoring priorities.

---

### 6️⃣ Case 3 – Class Distribution (Partially Balanced Dataset)
![Class Distribution Case 3](./images/classdistributioncase3.png)  
**Insight:**  
- Positive (stroke) cases increased significantly compared to Case 1, resulting in a better learning balance.
- Logistic Regression achieved the highest AUC score of **0.89**, the best across all experiments.

---

## 📈 Key Impacts
- Improved **stroke prediction accuracy** by addressing extreme class imbalance.
- Identified **critical health factors** for early detection (age, glucose level, hypertension).
- Achieved **AUC score improvement from ~0.63 to 0.89** through strategic data balancing.
- Delivered interpretable insights to guide healthcare interventions.


---

## ⚙️ How to Run

### 1️Clone the Repository
```bash
git clone https://github.com/your-username/brain-stroke-prediction.git
cd brain-stroke-prediction
vvvvv
