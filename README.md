# IPL-Winner-Prediction

# 🏏 IPL Winner Prediction

Machine learning project that predicts the winner of an IPL match using team, toss, and venue features. It compares several classifiers and tunes the best performers with cross-validation.

> ⚠️ **Note:** The default run uses a **synthetic dataset** (`USE_SYNTHETIC = True`) so the notebook works out of the box. Results on synthetic data are for demonstration only. To use real data, set `USE_SYNTHETIC = False` and place the IPL `matches.csv` in the project folder.

## Highlights
- Exploratory analysis: match wins by team, and whether winning the toss helps
- Preprocessing with `LabelEncoder` and `StandardScaler`
- Model comparison across 6 classifiers:
  Logistic Regression, Decision Tree, Random Forest, Gradient Boosting, KNN, SVM, Gaussian Naive Bayes
- Hyperparameter tuning with `GridSearchCV` and `cross_val_score`
- Evaluation: accuracy, classification report, confusion matrix, ROC-AUC / ROC curve

## Teams Covered
Mumbai Indians, Chennai Super Kings, Royal Challengers Bangalore, Kolkata Knight Riders, Delhi Capitals, Sunrisers Hyderabad, Punjab Kings, Rajasthan Royals, Gujarat Titans, Lucknow Super Giants

## Tech Stack
Python · NumPy · Pandas · Matplotlib · Seaborn · scikit-learn

## Project Structure
```
├── IPL_Winner_Prediction.ipynb
├── matches.csv          # optional: real IPL data
└── README.md
```

## How to Run
```bash
git clone https://github.com/<your-username>/ipl-winner-prediction.git
cd ipl-winner-prediction
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
jupyter notebook IPL_Winner_Prediction.ipynb
```
Config at the top of the notebook:
```python
USE_SYNTHETIC = True      # False → use real matches.csv
DATA_PATH = "matches.csv"
RANDOM_STATE = 42
```

## Results
| Model | Accuracy | ROC-AUC |
|-------|----------|---------|
| _fill in_ | _–_ | _–_ |

Best model: **_fill in_**

## Key Insights
- _e.g., Toss winner also won the match in XX% of matches_
- _e.g., Top features driving predictions_

## Future Improvements
- Train on real historical data with season-wise splits
- Add features: team form, head-to-head record, venue stats, player-level data
- Try XGBoost / LightGBM
- Deploy as a Streamlit app

<img width="1428" height="947" alt="Screenshot 2026-10-09 114008" src="https://github.com/user-attachments/assets/a433abd0-5124-4c05-827c-2aad67a6aed3" />

<img width="1430" height="970" alt="Screenshot 2026-10-09 114046" src="https://github.com/user-attachments/assets/e7d04ffe-4c4f-4ad2-91f8-4b55c921fee0" />
