# Telecom-Churn_Analysis-Prediction
## Churn Prediction Model

This repository contains a Jupyter Notebook for building a customer churn prediction model using a Random Forest Classifier. The model is designed to help businesses identify customers who are likely to churn based on historical data.

**Features**

- Reads customer data from an Excel file (`Prediction Analysis.xlsx`, sheet: `vw_ChurnData`)
- Preprocesses data (label encoding of categorical features, dropping irrelevant columns)
- Trains a Random Forest Classifier to predict customer churn
- Evaluates model performance using classification metrics

**Requirements**

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- joblib
- openpyxl (for reading Excel files)

**Usage**

1. Clone the repository and open `Churn_Prediction_Model.ipynb` in Jupyter Notebook or Google Colab.
2. Ensure the Excel file (`Prediction Analysis.xlsx`) is in the same directory.
3. Run the notebook cells to:
   - Load and preview the data
   - Preprocess features and encode categorical variables
   - Train a Random Forest model
   - Evaluate model predictions

**Data**

The model expects the following columns in the Excel data (among others):

- Demographics: `Gender`, `Age`, `Married`, `State`
- Service usage: `Phone_Service`, `Internet_Service`, `Streaming_TV`, etc.
- Financials: `Monthly_Charge`, `Total_Charges`, `Payment_Method`
- Target: `Customer_Status` (encoded as 0 for Stayed, 1 for Churned)

**Model Training**

The notebook splits the data into training and testing sets, fits a Random Forest Classifier, and provides evaluation metrics such as classification report and confusion matrix.

**Customization**

- You can adjust the list of features or try different models by modifying the notebook.
- Update the file path or sheet name as needed for your data.

**License**

This project is open-source and free to use for educational and non-commercial purposes.

---
