# FIFA World Cup 2026 Predictor

A machine-learning and statistical modelling pipeline for predicting FIFA World Cup 2026 knockout outcomes and potential semifinalists.

## Highlights

- Combines historical international match data with current tournament information
- Builds Elo-based team-strength features
- Uses Poisson score modelling to estimate scoreline and match probabilities
- Includes historical knockout backtesting and calibration analysis
- Produces semifinal predictions and an interactive HTML report
- Achieved 67.86% outcome accuracy in the historical knockout evaluation recorded in the notebook

## Repository contents

- `wc2026_semifinal_predictor_pipeline.ipynb` — data preparation, feature engineering, modelling, evaluation, and predictions
- `semifinal_predictions.csv` — exported prediction results
- `wc2026_semifinal_predictor.html` — interactive output report

## Technology

- Python
- Pandas and NumPy
- SciPy
- Matplotlib and Seaborn
- Elo ratings
- Poisson scoreline modelling

## Run in Google Colab

1. Open `wc2026_semifinal_predictor_pipeline.ipynb` in Google Colab.
2. Install any missing packages from the first setup cells.
3. Configure Kaggle credentials as environment variables or Colab secrets.
4. Run the notebook from top to bottom.

Never commit `kaggle.json`, API keys, or account credentials to the repository.

## Local setup

```bash
git clone https://github.com/IRTAZA-110/fifa-world-cup-2026-predictor.git
cd fifa-world-cup-2026-predictor
python -m venv .venv
pip install -r requirements.txt
jupyter notebook
```

## Modelling notes

The project uses independent Poisson goal distributions and simplified handling of draws in knockout matches. Future improvements could include Dixon-Coles adjustments, explicit extra-time and penalty models, rolling form features, and stricter time-based validation.

## Author

Irtaza Iftikhar Choudry

