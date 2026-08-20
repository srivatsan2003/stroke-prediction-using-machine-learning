# Stroke Prediction Using Machine Learning

This is a student machine learning project where I explored a healthcare dataset and built different classification models to predict stroke occurrence.

The main purpose of the project was to practice the complete machine learning workflow, including data exploration, preprocessing, class imbalance handling, model training, and evaluation.

## Dataset

The notebook uses the file:

`healthcare-dataset-stroke-data.csv`

Place the CSV file in the same folder as the notebook before running it.

## What I Did

- Explored the dataset and checked missing values
- Visualized age distribution and stroke class imbalance
- Removed the `id` column from the prediction features
- Handled missing numerical and categorical values
- Standardized numerical features
- One-hot encoded categorical features
- Split the data into training and testing sets
- Used SMOTE to handle class imbalance
- Compared five machine learning models
- Evaluated models using accuracy, precision, recall, F1-score, classification reports, and confusion matrices
- Used 5-fold stratified cross-validation
- Added a small K-Means clustering experiment

## Models Used

- Logistic Regression
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)
- Neural Network using `MLPClassifier`

## Important Improvement

SMOTE and preprocessing are applied inside the training pipeline rather than before the train/test split. This avoids data leakage from the test set.

## Project Structure

```text
stroke-prediction-project/
│
├── stroke_prediction.ipynb
├── healthcare-dataset-stroke-data.csv
├── requirements.txt
├── .gitignore
└── README.md
```

## How to Run

1. Clone or download this repository.
2. Put `healthcare-dataset-stroke-data.csv` inside the project folder.
3. Install the required packages:

```bash
pip install -r requirements.txt
```

4. Open `stroke_prediction.ipynb` in Jupyter Notebook, JupyterLab, or VS Code.
5. Run the notebook from top to bottom.

## Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn

## What I Learned

This project helped me understand how to work with an imbalanced classification dataset. I also learned why accuracy can be misleading when one class is much more common than another, and why metrics such as recall and F1-score are important.

I also learned the importance of avoiding data leakage by fitting preprocessing steps and SMOTE only on training data.

## Future Improvements

Some improvements I would like to try later are:

- hyperparameter tuning
- ROC-AUC comparison
- feature importance analysis
- testing other imbalance-handling techniques
- trying boosting models such as XGBoost

## Disclaimer

This project was created for learning and academic practice. It is not intended to be used for real medical diagnosis or clinical decision-making.
