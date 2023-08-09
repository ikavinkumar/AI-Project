# Machine Learning Regression Models for Concrete Strength Prediction

This repository contains Python code that demonstrates the use of different regression models to predict the compressive strength of concrete based on various input features.

## Prerequisites

Before running the code, make sure you have the following installed:

- Python 3.x
- Required Python packages: pandas, scikit-learn

## Usage

1. **Mounting Google Drive:**
   The code begins by mounting your Google Drive to access the dataset and save trained models.

2. **Loading and Preprocessing Data:**
   - The dataset named `Concrete_Dataset.csv` is loaded from the specified Google Drive location.
   - The dataset is split into independent features (`independent`) and the dependent target variable (`dependent`).
   - Data is split into training and testing sets using `train_test_split`.

3. **Linear Regression:**
   - A Linear Regression model is created and trained using the training data.
   - Model weights and bias are obtained.
   - Predictions are made on the test data.
   - The R-squared score is calculated as a measure of model performance.

4. **Saving and Loading Linear Regression Model:**
   - The trained Linear Regression model is saved using pickle.
   - The saved model is loaded and used to make predictions on new data.

5. **One-Hot Encoding:**
   - The dataset is one-hot encoded using `pd.get_dummies` to convert categorical features into numerical format.

6. **Random Forest Regression:**
   - A Random Forest Regression model is created with specified hyperparameters.
   - The model is trained and predictions are made.
   - The R-squared score for the Random Forest model is calculated and displayed.

7. **Standard Scaling and Support Vector Regression:**
   - Features are standardized using `StandardScaler`.
   - A Support Vector Regression (SVR) model with a polynomial kernel is trained.
   - Predictions are made and the R-squared score is calculated.

8. **Loading Saved Random Forest Model:**
   - A previously saved Random Forest model is loaded using pickle.
   - The loaded model is used to make predictions on new data.

## File Structure

- `Concrete_Dataset.csv`: Input dataset containing concrete properties and compressive strength.
- `README.md`: This documentation file.
- `ML_Concrete_Regression.ipynb`: Jupyter Notebook containing the code for regression models.

## How to Run

1. Make sure you have the required packages installed.
2. Open the `ML_Concrete_Regression.ipynb` notebook.
3. Run each cell sequentially to execute the code step by step.
4. Review the results and analysis for each regression model.

## Note

- This code is intended for educational purposes and may require adjustments for specific use cases.
- Make sure to provide the correct file paths when reading and saving data/models.

---

Feel free to modify the content as needed, and don't forget to update the file paths, comments, and descriptions according to your actual project structure and requirements.
