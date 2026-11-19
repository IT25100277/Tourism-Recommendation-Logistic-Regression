# Tourism Recommendation System — Data Scaling & Logistic Regression

**Year 2, Semester 1 | Artificial Intelligence & Machine Learning (AIML) group project**

This repository presents my individual contributions to a collaborative tourism recommendation system project: numerical feature scaling and a Logistic Regression classification model. It is a **portfolio extract**, not a complete standalone recommendation application.

## My contributions

- **Numerical preprocessing:** Applied `MinMaxScaler` to `ticket_price`, `spend_amount`, and `visit_duration_hours`, creating features scaled to [0, 1]. Visualized the resulting distributions.
- **Classification:** Trained a Logistic Regression classifier to predict `recommendation_level` from numerical features in the team's cleaned tourism dataset.
- **Evaluation:** Computed accuracy, weighted precision, recall and F1 score, and plotted a confusion matrix.
- **Exploration and tuning:** Used PCA for feature reduction and a two-dimensional decision-boundary visualization, and `GridSearchCV` to compare regularization strengths and solvers.

## Files

| File | Description |
| --- | --- |
| `notebooks/IT25100277_Scaling.ipynb` | Min-max scaling and distribution plots |
| `notebooks/IT25100277_Model_LogisticRegression.ipynb` | Classification, evaluation, PCA visualization and parameter search |
| `images/IT25100277.jpeg` | Scaling distribution visualization provided with the project |

## Requirements

Python 3, Jupyter Notebook, `pandas`, `numpy`, `scikit-learn`, `matplotlib`, and `seaborn`.

```bash
pip install notebook pandas numpy scikit-learn matplotlib seaborn
```

## Data dependencies

The scaling notebook reads `tourism_recommendation_dataset_en.csv`. The classification notebook reads `clean_tourism_data.csv` and expects a `recommendation_level` target column. **These CSV files are not included in this portfolio extract.** To execute the notebooks, supply the appropriate datasets in the working directory and verify their columns.

The classifier notebook uses a **75%/25% train/test split** (`test_size=0.25`). It also uses `max_iter=2` in its Logistic Regression experiments; this is a very low iteration limit and may prevent convergence. Its notebook outputs are historical experiment results, not verified performance on a newly run dataset.

## Project attribution

The original Tourism Recommendation System was developed collaboratively as a university AIML group project. This repository highlights the data-scaling and Logistic Regression notebooks identified with my student ID, `IT25100277`. Other project modules and team contributions are not represented as my individual work.
