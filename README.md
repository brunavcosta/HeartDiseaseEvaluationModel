# Heart Disease Prediction Project

## Overview
This project focuses on predicting the risk of heart disease using the UCI Heart Disease dataset. The goal is to analyze how various clinical features such as age, cholesterol levels, resting blood pressure, and other factors influence the likelihood of developing heart-related conditions. The project leverages regression techniques, data preprocessing, and model evaluation to derive meaningful insights from real-world medical data.

## Dataset
The dataset used is the UCI Heart Disease dataset, which contains 920 entries with 16 features. Key features include:
- `age`: Age of the patient
- `sex`: Gender of the patient (Male/Female)
- `cp`: Type of chest pain
- `trestbps`: Resting blood pressure
- `chol`: Serum cholesterol level
- `fbs`: Fasting blood sugar
- `restecg`: Resting electrocardiographic results
- `thalch`: Maximum heart rate achieved
- `exang`: Exercise-induced angina
- `oldpeak`: ST depression induced by exercise relative to rest
- `slope`: The slope of the peak exercise ST segment
- `ca`: Number of major vessels colored by fluoroscopy
- `thal`: Thalassemia type
- `num`: Target variable indicating the presence of heart disease (0 = no disease, 1-4 = varying levels of disease)

## Project Structure
1. **Data Loading**: The dataset is loaded from Kaggle using the `kagglehub` library.
2. **Exploratory Data Analysis (EDA)**:
   - Basic statistics and data overview.
   - Visualizations of key features (e.g., age distribution, cholesterol levels, gender distribution).
   - Correlation analysis to understand relationships between features.
3. **Data Preprocessing**:
   - Handling missing values (if any).
   - Encoding categorical variables.
   - Normalizing or scaling numerical features.
4. **Model Building**:
   - Implementation of a linear regression model and non linear models to predict heart disease risk.
   - Evaluation using metrics such as accuracy, precision, recall, and F1-score.
5. **Visualizations**:
   - Histograms, boxplots, and pair plots to explore feature distributions and relationships.
   - Correlation heatmaps to identify significant predictors.

## Key Findings
- **Age Distribution**: The majority of patients are between 50-60 years old.
- **Gender Distribution**: The dataset is skewed toward male patients.
- **Cholesterol Levels**: Most patients have cholesterol levels between 200-300 mg/dL.
- **Correlation Analysis**: Features like `thalch` (maximum heart rate) and `oldpeak` (ST depression) show notable correlations with the target variable.

## Dependencies
- Python 3.x
- Libraries:
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `seaborn`
  - `scikit-learn`
  - `kagglehub`

## How to Run
1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
2. Open the Jupyter notebook:
   ```bash
   jupyter notebook HeartDiseasePrediction.ipynb
   ```
3. Execute the cells sequentially to reproduce the analysis and model.

## Future Work
- Experiment with other machine learning models (e.g., logistic regression, random forests, SVM).
- Perform hyperparameter tuning to improve model performance.
- Deploy the model as a web application for real-time predictions.

## Acknowledgments
- Dataset sourced from the UCI Machine Learning Repository via Kaggle.
- Special thanks to the open-source community for providing valuable tools and libraries.

## License
This project is open-source and available under the MIT License. Feel free to use, modify, and distribute it as needed.
