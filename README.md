# player_performance_prediction

This project analyzes cricket match data to predict player performance using machine learning techniques.

## Project Structure

- `deliveries.csv`: Ball-by-ball delivery data for matches.
- `matches.csv`: Match-level metadata.
- `points_table.csv`: Points table for teams.
- `player_pred.ipynb`: Jupyter notebook containing data analysis, feature engineering, model training, and prediction code.
- `README.md`: Project documentation.

## Features

- Cleans and processes cricket match data.
- Extracts player-level statistics (runs, wickets, strike rate, economy rate, etc.).
- Builds predictive models for batting and bowling performance.
- Supports custom predictions for new player data.

## Usage

1. Open `player_pred.ipynb` in Jupyter or VS Code.
2. Run all cells to process data and train models.
3. Modify the prediction section to input new player stats for predictions.

## Requirements

- Python 3.x
- pandas
- scikit-learn
- Jupyter Notebook

Install dependencies with:

```sh
pip install pandas scikit-learn notebook# player_performance_prediction

Data Sources:

- All data files (deliveries.csv, matches.csv, points_table.csv) are required for analysis and predictions.

Example:
To predict if a player had a "good batting" performance:
new_data = pd.DataFrame({
    "ball_faced": [30],
    "strike_rate": [(45/30)*100],
    "wickets": [1],
    "economy_rate": [40/6],
    "run_scored": [45],
    "ball_bowled": [36],
    "over": [36/6]
})
# after using the model i predict good batting and bowling