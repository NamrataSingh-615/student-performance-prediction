# Student Performance Prediction

A machine learning project that predicts students' final Mathematics grades using Python.

## Technologies Used
- Python
- Pandas and NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook
- Joblib

## Models
- Linear Regression
- Random Forest Regressor

## Results
The Random Forest model achieved these test-set results:
- MAE: 2.966
- RMSE: 3.754
- R²: 0.313

The model showed modest predictive performance.

## How to Run
1. Install the required libraries:

   `python -m pip install pandas numpy matplotlib seaborn scikit-learn joblib jupyter`

2. Open `student_prediction.ipynb` in VS Code.
3. Select a Python kernel and run the notebook cells in order.

Keep `student-mat.csv` in the same folder as the notebook.

## Dataset
The project uses the Student Performance dataset. See `student.txt` for documentation.

## Limitations
Predictions have limited accuracy and should not be treated as definitive assessments of individual students.