# Sales-Prediction

This repository contains a machine learning project focused on predicting retail sales using various regression models. The dataset used in this project is synthetic, generated for the purpose of this exercise.

## Project Overview

The goal of this project is to build and compare different machine learning models to predict retail sales based on features such as location, section, footfall, and other relevant factors. The models are trained and evaluated using cross-validation to identify the best-performing model.

### Models Used
- **Random Forest Regressor**
- **Gradient Boosting Regressor**
- **Ridge Regression**
- **XGBoost Regressor**

### Data Overview

The dataset consists of two CSV files: `train.csv` and `test.csv`. Each dataset contains the following features:
- `ID`: Unique identifier for each record.
- `Date`: Timestamp of the record.
- `Location`: Location of the retail store.
- `Section`: Section of the store.
- `Footfall`: Category indicating the level of foot traffic.
- `Size`: Size of the store section.
- `Humidity`: Humidity level at the time of the record.
- `Normalised Buying Power`: A normalized measure of buying power.
- `Normalised Rating`: A normalized customer rating of the store.
- `Labour Index`: A measure of labor intensity.
- `Sales`: The target variable, representing sales in the store section.

### Workflow

1. **Data Preprocessing**: The data is preprocessed using pipelines. Numerical features are scaled and imputed, and categorical features are encoded using one-hot encoding.
2. **Feature Engineering**: Features are extracted from the `Date` column, including year, month, and day.
3. **Model Training**: Various regression models are trained using cross-validation to tune hyperparameters and identify the best model.
4. **Model Evaluation**: The performance of each model is evaluated using the R-squared score.

### Results

The best model was determined using cross-validation. The XGBoost Regressor performed the best with an R-squared score of -0.2228 on the validation set.

### Installation

To run this project, you need to have Python installed. Clone this repository and install the required dependencies using:

```bash
pip install -r requirements.txt
```
### Usage

1. **Training the Model**: Run the `code_file.ipynb` script to train the model.
2. **Making Predictions**: After training, the model will generate predictions for the test set.
3. **Saving the Model**: The trained model is saved as `trained_model.pkl`.

### Dependencies

See the `requirements.txt` file for a list of required packages.

### Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request.

### License

This project is licensed under the MIT License.


