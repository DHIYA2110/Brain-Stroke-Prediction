🧠 Brain Stroke Prediction using Classification Models

This project focuses on predicting the likelihood of brain strokes using machine learning models. The dataset is imbalanced, requiring careful handling to achieve reliable predictions.

## 🎯 Project Goals
- Predict stroke occurrence using patient health indicators.
- Compare performance of multiple classification algorithms.
- Handle class imbalance using oversampling and undersampling techniques.
- Provide model evaluation with accuracy, precision, recall, and F1-score.

## 🔧 Tech Stack
- Python
- Pandas, Matplotlib, Seaborn
- Scikit-learn (Logistic Regression, Random Forest, Gradient Boosting)
- Jupyter Notebook

## 📂 Folder Structure
brain-stroke-prediction/
├── data/ # Stroke dataset (ignored in Git)
├── notebooks/ # Jupyter notebooks
├── visuals/ # EDA and model evaluation plots
├── README.md # Project overview
├── .gitignore # Files ignored by Git

markdown
Copy
Edit

## 📁 Dataset
- The stroke prediction dataset contains patient demographics, medical history, and stroke occurrence labels.
- Dataset is stored in:
data/

bash
Copy
Edit

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/brain-stroke-prediction.git
   cd brain-stroke-prediction
Open the notebook:

bash
Copy
Edit
notebooks/stroke_prediction.ipynb
Ensure your CSV dataset is in:

kotlin
Copy
Edit
data/
Run the notebook top-to-bottom to:

Perform EDA

Handle imbalance

Train classification models

Evaluate performance

View result graphs inside:

Copy
Edit
visuals/
📦 Dependencies
This project uses standard data science libraries:

pandas

numpy

matplotlib

seaborn

sklearn
