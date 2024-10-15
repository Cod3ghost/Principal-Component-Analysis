Breast Cancer Dataset Analysis

Overview

This project involves the analysis of the Breast Cancer dataset from the sklearn library. The main goal of the project is to implement Principal Component Analysis (PCA) for dimensionality reduction, followed by a logistic regression model to classify cancer as benign or malignant. Additionally, cross-validation is used for model evaluation, and proper data cleaning is performed to ensure quality analysis.

Project Structure

The project is organized into several sections:

1. Data Loading and Exploration
	- The breast cancer dataset is loaded and basic exploratory data analysis (EDA) is performed.
	- Initial summary statistics and pairplots provide insights into the dataset.
2. Data Cleaning
	- Missing values are handled by replacing them with the mean value of the corresponding feature.
	- Duplicate rows are identified and removed.
	- Outliers are detected based on z-scores (values beyond 3 standard deviations) and capped at 3 standard deviations.
	- Data types are checked and corrected.
3. Data Scaling
	- The features are standardized using `StandardScaler` to ensure they are on the same scale before applying PCA.
4. PCA Implementation
	- PCA is applied to reduce the dataset to 2 components.
	- The explained variance ratio is visualized to show how much variance is retained by each component.
5. PCA Visualization
	- A scatter plot is used to visualize how well the two principal components separate the data, based on the target labels (benign vs malignant).
6. Logistic Regression
	- Logistic regression is applied on the PCA-reduced dataset, with cross-validation used to evaluate model performance.
7. Model Evaluation
	- The logistic regression model is evaluated using a classification report (precision, recall, F1-score) and the ROC-AUC score.


How to Run the Code
To run the code, ensure you have the following libraries installed:
- `pandas`
- `seaborn`
- `matplotlib`
- `sklearn`

You can install these libraries using the following command:
```
pip install pandas seaborn matplotlib scikit-learn
```
Once the libraries are installed, you can run the script in a Python environment or Jupyter Notebook.

Acknowledgments
- The dataset used in this analysis is provided by the `sklearn` library.
- This project demonstrates the power of PCA for dimensionality reduction and the application of logistic regression for classification tasks.

