# Student Performance Prediction

A beginner-level machine learning project that predicts students' final Mathematics grades using Python and student performance data.

## Overview

This project explores how machine learning regression algorithms can be used to predict students' final Mathematics grades based on selected student attributes.

The workflow includes data loading, preprocessing, model training, evaluation, comparison of regression models, and visualization of actual versus predicted grades.

## Objectives

- Explore and prepare student performance data.
- Apply regression algorithms to predict final grades.
- Compare Linear Regression and Random Forest Regression.
- Evaluate predictions using standard regression metrics.
- Visualize actual and predicted grades.
- Save the trained model for potential reuse.

## Technologies Used

| Technology | Purpose |
|---|---|
| Python | Implementation |
| Pandas | Data handling |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Scikit-learn | Model training and evaluation |
| Jupyter Notebook | Development environment |
| Joblib | Saving the trained model |

## Dataset

The project uses the Student Performance dataset, including the Mathematics student data file `student-mat.csv`.

The dataset contains student attributes and academic information. The notebook uses selected attributes to predict the final Mathematics grade.

## Methodology

1. **Data loading:** Load the dataset and inspect its structure.
2. **Data preprocessing:** Prepare the selected input features and target variable.
3. **Train-test split:** Divide the data into training and testing sets.
4. **Model training:** Train Linear Regression and Random Forest Regression models.
5. **Evaluation:** Compare predictions using MAE, RMSE, and R².
6. **Visualization:** Plot actual versus predicted final grades.
7. **Model saving:** Save the trained model using Joblib.

## Model Performance

The following results were obtained on the test set.

| Model | MAE | RMSE | R² |
|---|---:|---:|---:|
| Random Forest Regressor | 2.966 | 3.754 | 0.313 |
| Linear Regression | 3.395 | 4.196 | 0.141 |

Random Forest Regression performed better than Linear Regression on this test set, with lower MAE and RMSE and a higher R² score.

However, the R² value of 0.313 indicates that the model has limited predictive power. Predictions should therefore be treated as estimates rather than exact grades.

### Evaluation Metrics

- **MAE (Mean Absolute Error):** Measures the average absolute difference between actual and predicted grades. Lower is better.
- **RMSE (Root Mean Squared Error):** Measures prediction error while penalizing larger errors more heavily. Lower is better.
- **R² (Coefficient of Determination):** Measures how much variation in the target is explained by the model. Values closer to 1 generally indicate better performance.

## Visualizations

The notebook includes a scatter plot comparing actual and predicted final Mathematics grades. This visualization helps examine prediction errors and the relationship between actual and predicted values.

## Repository Structure

```text
student-performance-prediction/
├── README.md
├── student_prediction.ipynb
├── student-mat.csv
├── student_performance_model.pkl
└── student.txt
```

## How to Run

### 1. Clone the repository

```bash
git clone https://github.com/NamrataSingh-615/student-performance-prediction.git
cd student-performance-prediction
```

### 2. Install the dependencies

```bash
python -m pip install pandas numpy matplotlib scikit-learn joblib jupyter
```

### 3. Open the notebook

```bash
jupyter notebook student_prediction.ipynb
```

Alternatively, open the notebook in Visual Studio Code with the Jupyter extension installed.

Run the notebook cells in order. Keep `student-mat.csv` in the expected location used by the notebook.

## Limitations

- The dataset is relatively small.
- Model performance is limited on the test set.
- Predictions depend on the selected features and the quality of the dataset.
- The model does not establish causal relationships between student attributes and grades.
- Results on this dataset may not generalize to other student populations.

## Future Improvements

- Experiment with additional regression algorithms.
- Tune model hyperparameters using cross-validation.
- Analyze feature importance and prediction errors.
- Improve the model through careful feature selection and evaluation.
- Develop a simple interface for entering student attributes and obtaining predictions.

## Conclusion

This project demonstrates a basic machine learning regression workflow, from data preparation and model training to evaluation, visualization, and model saving. It also illustrates why comparing multiple models and examining evaluation metrics are important when assessing predictive performance.

## Author

**Namrata Singh**

GitHub: [NamrataSingh-615](https://github.com/NamrataSingh-615)
