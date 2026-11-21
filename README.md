# Air Quality Insights

**Project 4 | Python, NumPy and Pandas**

This project uses the air-quality dataset supplied for the training assignment. I am using Pandas and NumPy to inspect and clean the readings for four cities.

## Project structure

```text
air-quality-analysis/
├── data/
│   ├── raw/
│   │   └── 04_air_quality.csv
│   └── processed/
│       └── 04_air_quality_cleaned.csv
├── notebooks/
│   └── air_quality_data_cleaning.ipynb
├── SRS/
│   └── Project_4_Air_Quality_SRS.docx
├── requirements.txt
├── .gitignore
└── README.md
```

## Setup

Python 3 is required. From the project folder, install the libraries with:

```bash
python -m pip install -r requirements.txt
```

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open `notebooks/air_quality_data_cleaning.ipynb` and run the cells from top to bottom.

## What the current notebook covers

- Loads and inspects the original CSV.
- Checks missing values and duplicate records.
- Fills missing `PM25` values using the median for the same city.
- Keeps a column showing which `PM25` values were filled.
- Converts `Date` to datetime and adds `Year`, `Month` and `YearMonth`.
- Flags selected values for checking instead of deleting those rows.
- Saves the cleaned dataset in `data/processed/`.

The original dataset in `data/raw/` is not changed. The current notebook is the data-cleaning part of Project 4; the remaining analysis tasks will be added separately.

## Dataset note

The dataset is provided for the course assignment. The flags are only used to identify records that may need a closer look. They do not automatically mean that a measurement is wrong.
