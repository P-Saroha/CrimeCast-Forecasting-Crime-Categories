# Crime Category Prediction

## Overview

This project is aimed at predicting crime categories based on a comprehensive dataset of crime incidents within a city. The dataset provides various attributes of each incident, including location, time, victim demographics, modus operandi, and more. By leveraging machine learning techniques, the goal is to predict the crime category for each incident. This can potentially aid law enforcement agencies in predicting crime trends and improving public safety strategies.

## Objective

The objective of this project is to develop a predictive model capable of accurately forecasting the **Crime_Category** based on other features available in the dataset.

## Dataset

The dataset used in this project consists of the following files:

- **train.csv**: The training dataset, which includes the target variable `crime_category` along with the relevant feature attributes.
- **test.csv**: The test dataset, containing the same feature attributes as the training dataset but excluding the target variable (`crime_category`), which needs to be predicted.
- **sample_submission.csv**: A sample submission file in the correct format for competition submissions.

### Columns Description:

1. **Location**: Street address of the crime incident.
2. **Cross_Street**: Cross street of the rounded address.
3. **Latitude**: Latitude coordinates of the crime incident.
4. **Longitude**: Longitude coordinates of the crime incident.
5. **Date_Reported**: Date when the incident was reported.
6. **Date_Occurred**: Date when the incident occurred.
7. **Time_Occurred**: Time the incident occurred (24-hour format).
8. **Area_ID**: LAPD's geographic area number.
9. **Area_Name**: Name of the LAPD geographic area.
10. **Reporting_District_no**: Reporting district number.
11. **Part 1-2**: Crime classification.
12. **Modus_Operandi**: Activities associated with the suspect.
13. **Victim_Age**: Age of the victim.
14. **Victim_Sex**: Gender of the victim.
15. **Victim_Descent**: Descent code of the victim.
16. **Premise_Code**: Premise code indicating the location of the crime.
17. **Premise_Description**: Description of the premise code.
18. **Weapon_Used_Code**: Weapon code indicating the type of weapon used.
19. **Weapon_Description**: Description of the weapon code.
20. **Status**: Status of the case.
21. **Status_Description**: Description of the status code.
22. **Crime_Category**: The target variable, which indicates the category of the crime.



## Methodology

1. **Data Preprocessing**: Clean and preprocess the data, handle missing values, and transform variables to be suitable for model building.
2. **Feature Engineering**: Create new features, such as time-related variables from `Date_Occurred` and `Time_Occurred`, and encode categorical variables like `Location` and `Modus_Operandi`.
3. **Modeling**: Train machine learning models (e.g., Random Forest, XGBoost, etc.) to predict the `crime_category` based on the available features.
4. **Model Evaluation**: Evaluate the model using performance metrics such as accuracy, precision, recall, F1-score, and confusion matrix.
5. **Hyperparameter Tuning**: Use techniques such as grid search or random search to optimize the model's hyperparameters.

## Requirements

- Python 3.x
- pandas
- numpy
- scikit-learn
- xgboost
- matplotlib
- seaborn
- Jupyter Notebook (for exploratory analysis)

Install the required dependencies using:

## Usage

1. Clone this repository.
2. Install the required dependencies.
3. Open the Jupyter notebook `crime_category_prediction.ipynb` to explore the data, build models, and make predictions.
4. Use the `predict()` function to generate predictions on the test set.
5. Submit your predictions in the required format as `submission.csv`.

## Acknowledgments

- Dataset: [Crime Data Source]
- Libraries: [Pandas](https://pandas.pydata.org/), [Scikit-learn](https://scikit-learn.org/), [XGBoost](https://xgboost.ai/), [Matplotlib](https://matplotlib.org/), [Seaborn](https://seaborn.pydata.org/)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

