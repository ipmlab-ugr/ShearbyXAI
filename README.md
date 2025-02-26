
#XAI-GP: Explainable AI-Genetic Programming for Shear Strength Prediction
========================================================
This script is designed to run in **Google Colab** and implements **Explainable AI (XAI) for shear strength prediction** using **H2O.ai models**.

### **Overview**
Shear strength is a critical parameter in **structural engineering**, particularly for designing **concrete beams**. This script leverages **machine learning models** to predict shear strength based on various beam properties, such as:
- **Effective depth of the beam**
- **Shear span**
- **Maximum aggregate size**
- **Compressive strength of concrete**
- **Percentage of tension reinforcement**
- **Beam width**

The script applies **H2O.ai’s powerful AutoML framework** to train and evaluate multiple models while integrating **explainability tools** using **DALEXtra** to interpret the results.

---
### **Key Features:**
 **Loads & preprocesses data** from an Excel file
 **Trains multiple machine learning models**, including:
   - **Multi-layers Perceptron (MLP)**
   - **Gradient Boosted Machines (GBM)**
   - **Random Forest (RF)**
   - **Stacked Ensembles** (combining multiple models for better predictions)
 **Uses DALEXtra** to explain model predictions
 **Visualizes SHAP and Breakdown**

---
### **How It Works:**
- The dataset (`M1cylinderical.xlsx`) is uploaded to **Google Colab**.
- The script preprocesses the data and splits it into **training and test sets**.
- Several machine learning models are trained using **H2O.ai’s AutoML framework**.
- The **DALEXtra library** is used to explain predictions and understand model behavior.
- **SHAP and Breadown plots** provide insights into key influencing parameters.

---
### **Code Structure:**
**Install dependencies** (H2O, DALEX, R libraries)
**Load dataset & preprocess** (split into training & testing)
**Train models** (DL, GBM, GLM, RF, and Stacked Ensembles)
**Explain models** using **DALEXtra**
**Evaluate performance**
**Visualize results** (feature importance, SHAP, break-down plots)


To perform an explainability analysis, please use xai-shear.py. Make sure to uncomment the necessary sections, as the code is designed to run in both an R environment and Google Colab.
![Alt Text](https://github.com/ipmlab-ugr/ShearbyXAI/blob/main/uml_diagram_final.png)

---
## **Implemntation of Genetic Programming:**
For Genetic Programming (GP), use data-for-gp.csv and execute gp-main-for-eq-that-reported.py. For verification, use data-for-verification.

---
## **Cite the code:**

To cite this code, please use the following reference: @misc{iPMLab2025,
  author = {{iPMLab}},
  title = {Codes Repository},
  year = {2025},
  url = {https://github.com/ipmlab-ugr/ShearbyXAI},  % Update if the repo name has changed
  note = {GitHub repository}
}
 }
