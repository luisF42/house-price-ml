# House Price Prediction (Beginner-Friendly ML)

A step-by-step Jupyter notebook that predicts house prices with **Linear Regression** and **Random Forest**, written for people who are new to machine learning. Every step explains what it does and why it matters.

![Predicted vs actual](https://img.shields.io/badge/R²-0.95-brightgreen) ![Python](https://img.shields.io/badge/Python-3.10+-blue) ![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange)

## What's inside

| Step | Topic |
|---|---|
| 1 | Setup and imports |
| 2 | Generating a reproducible synthetic dataset (500 houses) |
| 3 | Exploratory analysis with plain-language takeaways |
| 4 | Train/test split and why it matters |
| 5 | Linear Regression and how to read its weights |
| 6 | Evaluation with R², MAE and RMSE |
| 7 | Random Forest and model comparison |
| 8 | Predicting the price of a new house |
| 9 | Ideas to experiment with |

## Results

| Model | R² | MAE (k$) | RMSE (k$) |
|---|---|---|---|
| Linear Regression | 0.952 | 21.4 | 27.0 |
| Random Forest | 0.941 | 24.7 | 30.0 |

The simple model wins because the data follows a mostly linear pattern, a useful reminder that more complex is not always better.

## How to run it

1. Install [Python 3.10+](https://www.python.org/downloads/).
2. Open a terminal in this folder and create a virtual environment (optional but recommended):
   ```bash
   python -m venv .venv
   # Windows
   .venv\Scripts\activate
   # macOS / Linux
   source .venv/bin/activate
   ```
3. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Start Jupyter and open `house_price_prediction.ipynb`:
   ```bash
   jupyter notebook
   ```
5. Run all cells (**Kernel → Restart & Run All**).

The notebook creates `houses.csv`, so you can also open the data in Excel.

## Things to tweak

- `test_size` in the train/test split
- The amount of random noise when generating the data
- Which features are used by the model
- `n_estimators` in the Random Forest

## Author

Luis Fernando · [fernan9997.itch.io](https://fernan9997.itch.io)
