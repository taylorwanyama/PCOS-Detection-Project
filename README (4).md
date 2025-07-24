
# Detecting PCOS using Machine Learning

## Overview

Polycystic Ovary Syndrome (PCOS) is a hormonal condition affecting 5-10% of women of reproductive age. It is characterized by symptoms such as irregular periods, excessive hair growth, and ovarian cysts, which can significantly impact a woman's health and quality of life. Early detection is crucial for timely medical intervention.

In this project, I aim to build and evaluate three machine learning models—Logistic Regression, Decision Tree Classifier, and Random Forest Classifier—to predict PCOS diagnosis (binary target: 0 for no PCOS and 1 for PCOS). These models were chosen for their suitability in binary classification tasks and their ability to provide interpretable and accurate predictions.

The project will include hyperparameter tuning to optimize the models and identify the best-performing one. I will begin by importing the necessary libraries for data preprocessing, model building, and evaluation. This project holds real-world significance, as improving PCOS detection could help affected women receive timely medical care and support.

## Dataset

The dataset used is **pcos_dataset.csv**, which contains the following features:

- `Age`: The age of patients.
- `BMI`: Body Mass Index of each Patient.
- `Menstrual_Irregularity`: Show if a patient has menstrual irregularity or not.
- `Testosterone_Level(ng/dL)`: The patients' level of Testosterone.
- `Antral_Follicle_Count`: The number of antral follicles.
- `PCOS_Diagnosis`: Shows if a patient has PCOS or not.

## Steps in the Project

1. **Data Preprocessing**
   - Checked for missing values and data types.
2. **Exploratory Data Analysis (EDA)**
   - Visualized the target variable, PCOS_diagnosis.
   - Checked for correlations between the explanatory variables and the target variable to identify key influencing factors.
   - Plotted the correlation using a heatmap.
3. **Data Standardization**
   - Standardized all features in the dataset except the PCOS_diagnosis feature     
4. **Model Selection & Training**
   - Implemented **Logistic Regression** as the baseline model.
   - Also implemented a **Decision Tree Classifier** and a **Random Forest Classifier**. 
   - Performed **Hyperparameter tuning** on the tree trained models using **GridSearchCV** .
   - Evaluated models using metrics like **accuracy_score,Precision, recall, confusion matrix, and F1-score**.
5. **Results & Conclusion**
   - The best-performing models were found to be **Decision Tree Classifier** and **Random Forest Classifier**.
   - Both the **Decision Tree Classifier** and **Random Forest Classifier** had an **accuracy score** of 0.995 after tuning.
   - The models, **Decision Tree Classifier** and **Random Forest Classifier**, also had a recall of 1.00 for no PCOS and 0.97 for with PCOS.  
## Dependencies

To run this project, install the following libraries:

```bash
pip install pandas numpy seaborn matplotlib scikit-learn
```

## Running the Notebook

1. Clone this repository:
   ```bash
   git clone https://github.com/taylorwanyama/PCOS-Detection-Project/blob/main/Predicting%20if%20a%20Patient%20has%20PCOS_final_1%20%20(1).ipynb
   ```
2. Open the Jupyter Notebook and run the cells sequentially.
3. Modify parameters and visualize results for deeper analysis.

## Author

**Taylor Wanyama**  
[LinkedIn Profile](https://www.linkedin.com/in/taylor-wanyama-421920271/)

