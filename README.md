# March Matchup Inference Pipeline

This repository contains exploratory notebooks and a lightweight pipeline for
analyzing NCAA men’s basketball results and preparing matchup features for the
March Machine Learning Mania 2026 competition.

## Repository Structure

- `data_science/EDA.ipynb` — exploratory data analysis and dataset walkthroughs
- `data_science/notebook.ipynb` — feature engineering and season filtering
- `requirements.txt` — Python dependencies used by the notebooks

## Data

The notebooks expect the Kaggle competition data to be available in a local
`data/` directory (this folder is ignored by git). At minimum, the following
CSV files are referenced:

- `MNCAATourneyCompactResults.csv`
- `MRegularSeasonDetailedResults.csv`
- `MNCAATourneySeeds.csv`
- `MMasseyOrdinals.csv`
- `MNCAATourneyDetailedResults.csv`

Download the competition dataset from Kaggle and place the files under
`data/` so the notebooks can load them.

## Setup

1. Create and activate a virtual environment.
2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

Open the notebooks in Jupyter or VS Code:

```bash
jupyter notebook data_science/EDA.ipynb
```

The notebooks read CSVs from `../data/` relative to the `data_science/` folder.
If you store data elsewhere, update the file paths in the notebook cells.

## Notes

- Data files are ignored by `.gitignore`, so keep them local.
- The notebooks are designed for iterative exploration and can be extended with
  modeling, validation, and submission generation logic.
