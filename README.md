# Forecasting Crime Categories

## Project Overview
This project was part of a Kaggle competition aimed at predicting crime categories based on various features, including time, location, victim demographics, and more. The goal was to build machine learning models that can accurately classify crime categories using historical crime data.

**Competition Name**: [CrimeCast - Forecasting Crime Categories](https://www.kaggle.com/competitions/crime-cast-forecasting-crime-categories)  
**Objective**: Predict the category of crime based on given incident data.

## Dataset Description
The dataset provides a detailed record of criminal activities, encompassing multiple attributes like:

- **Location**: Street address of the crime incident.
- **Cross_Street**: Cross street of the rounded address.
- **Latitude**: Latitude coordinates of the crime incident.
- **Longitude**: Longitude coordinates of the crime incident.
- **Date_Reported**: Date the incident was reported.
- **Date_Occurred**: Date the incident occurred.
- **Time_Occurred**: Time the incident occurred in 24-hour military time.
- **Area_ID**: LAPD's Geographic Area number.
- **Area_Name**: Name designation of the LAPD Geographic Area.
- **Reporting_District_no**: Reporting district number.
- **Part 1-2**: Crime classification.
- **Modus_Operandi**: Activities associated with the suspect.
- **Victim_Age**: Age of the victim.
- **Victim_Sex**: Gender of the victim.
- **Victim_Descent**: Descent code of the victim.
- **Premise_Code**: Premise code indicating the location of the crime.
- **Premise_Description**: Description of the premise code.
- **Weapon_Used_Code**: Weapon code indicating the type of weapon used.
- **Weapon_Description**: Description of the weapon code.
- **Status**: Status of the case.
- **Status_Description**: Description of the status code.
- **Crime_Category**: The category of the crime **(Target Variable)**


## Project Pipeline
### 1. Exploratory Data Analysis (EDA)
- Analyzed key patterns and relationships within the data.
- Visualized crime frequency based on time, location, and demographic factors.

### 2. Feature Engineering
- Created new features to better capture crime trends.
- Encoded categorical variables and handled missing values.
- Engineered features like time-based attributes and victim profiling.

### 3. Data Preprocessing
- Utilized **Pipeline** and **Column Transformer** for efficient preprocessing.
- Standardized numerical features and applied Different **Encoding**, **Scaling** and **Imputation** methods to categorical variables.

### 4. Model Training
- Trained multiple classifiers including:
  - **XGBoost Classifier**
  - **LightGBM Classifier**
  - **RandomForest Classifier**

### 5. Hyperparameter Tuning
- Performed hyperparameter tuning using **RandomizedSearchCV** to optimize model performance.
- Focused on maximizing accuracy, precision, recall, and F1-score.

### 6. Model Evaluation
- Compared model performance .
- Achieved the highest accuracy of **0.95520**.

## Technologies Used
- **Programming Language**: Python
- **Libraries**: Pandas, NumPy, Scikit-learn, XGBoost, LightGBM, Seaborn, Matplotlib
- **Preprocessing**: Pipeline, ColumnTransformer
- **Modeling**: XGBoost, LightGBM, RandomForest
- **Hyperparameter Tuning**: RandomizedSearchCV

## How to Run the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/crimecast-forecasting.git
2. Install the necessary dependencies:
    ```bash
    pip install -r requirements.txt

3. Run the notebook to train the models:
    ```bash
    crimecast_forecasting.ipynb
