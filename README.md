# Diabetes Prediction Model

## Overview
This project aims to predict the likelihood of diabetes in patients based on several health-related features, including glucose levels, body mass index (BMI), height, weight, and blood pressure. The model utilizes a dataset containing information gathered from patients, including clinical data and health measurements. The final goal is to classify patients into two categories: those likely to have diabetes and those who are not.

## Project Structure
- **Data Cleaning & Preprocessing**: The raw data contains several columns, including personal information (e.g., name, gender), health measurements (e.g., glucose, BMI), and other relevant details. The preprocessing steps include handling missing data, cleaning string-based values (e.g., removing "cm" or "kg" from height and weight), converting units, and generating new features like age.
- **Model Building & Evaluation**: After cleaning the dataset, different machine learning models (e.g., Logistic Regression, Random Forest, SVM, etc.) are trained and evaluated to predict diabetes. The performance of each model is evaluated using accuracy metrics.
- **Data Visualization**: A correlation matrix heatmap is generated to understand the relationships between the different features.

## Dataset
The dataset used for this project is a collection of patient data that includes the following features:
- **FULL_NAME**: Name of the patient
- **GENDER**: Gender of the patient (Male/Female)
- **Age**: Age of the patient (derived from year of birth)
- **GLUCOSE**: Glucose level of the patient
- **BMI**: Body Mass Index of the patient
- **Systolic**: Systolic blood pressure value
- **Diastolic**: Diastolic blood pressure value
- **HEIGHT**: Height of the patient in meters
- **WEIGHT**: Weight of the patient in kilograms

## Steps Taken
1. **Data Cleaning**:
   - Handled missing values in height, weight, BMI, glucose, and blood pressure columns.
   - Removed irrelevant columns (e.g., names, contact information).
   - Converted the height and weight columns to numeric values and handled unit conversions.
   - Filled missing height values using the mean height of the dataset.

2. **Feature Engineering**:
   - Created new features such as "Age" from the year of birth.
   - Handled encoding of categorical columns like gender.

3. **Modeling**:
   - Split the dataset into training and test sets.
   - Applied several machine learning models, including Logistic Regression, Decision Tree, Random Forest, and Support Vector Machine (SVM).
   - Evaluated model performance using accuracy and other metrics.

4. **Model Evaluation**:
   - The models were evaluated and compared to find the one with the best performance.
   - Used accuracy as the primary metric for evaluation.

5. **Visualization**:
   - Created a correlation matrix heatmap to visualize relationships between features.

## Results
After training and evaluating various machine learning models, the model with the highest accuracy will be selected to predict whether a patient has diabetes or not based on the input features.

## Example Output
Model Accuracy: 97.83%
Best Model: Random Forest Classifier
Based on model accuracy, performace and time

## Conclusion
The diabetes prediction model is a robust system that can predict the likelihood of diabetes in patients based on several health factors. The accuracy of the model can vary based on the choice of algorithm and the quality of the input data.
