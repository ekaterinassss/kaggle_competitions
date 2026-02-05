# Stellar Object Classification

## Project Overview

This project focuses on classifying astronomical objects based on their spectral and photometric features.

The goal is to predict the class of a stellar entity using observational data. The model distinguishes between three object types:

- Star
- Galaxy
- Quasar

The project is based on a Kaggle competition using astronomical survey data.

Competition link:  
https://www.kaggle.com/competitions/25-hse-stellar/data


## Context

Stellar classification is a fundamental task in astronomy. It allows scientists to distinguish between stars, galaxies, and quasars based on spectral characteristics.

The dataset originates from the Sloan Digital Sky Survey (SDSS), one of the largest astronomical surveys ever conducted.


## Dataset

The dataset is based on the **Stellar Classification Dataset (SDSS17)** and was augmented for the competition.

### Dataset Characteristics

- ~200,000 observations
- 14 spectral and observational features
- Multiclass classification task

### Features

- `alpha` — Right Ascension angle
- `delta` — Declination angle
- `u`, `g`, `r`, `i`, `z` — Photometric filters
- `run_ID` — Scan run identifier
- `cam_col` — Camera column identifier
- `field_ID` — Field identifier
- `redshift` — Wavelength shift measurement
- `plate` — Plate identifier
- `MJD` — Modified Julian Date
- `fiber_ID` — Fiber identifier

### Target Variable

- `Class` — Object type (Star, Galaxy, Quasar)



## Project Workflow

- Data loading and preprocessing
- Feature analysis and visualization
- Model training
- Model evaluation
- Prediction generation


## Modeling Approach

Machine learning classification algorithms are applied to predict stellar object classes based on spectral features.


## Evaluation

Model performance is evaluated using classification metrics such as:

- Accuracy
- Confusion matrix
- Classification report


## Tech Stack

- Python
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn


## How to Run

### 1) Clone repository
```bash
git clone https://github.com/ekaterinassss/ml_assignments.git
cd ml_assignments/stellar_classification
```

### 2) Create virtual environment
```bash
python -m venv .venv
source .venv/bin/activate  # macOS/Linux
# .venv\Scripts\activate   # Windows
```

### 3) Install dependencies
```bash
pip install -U pip
pip install -r requirements.txt
```

### 4) Run notebook
```bash
jupyter lab
```

Open `Stellar_solution.ipynb`.


## References

- Sloan Digital Sky Survey (SDSS)
- SDSS Data Release 17
- Stellar Classification Dataset (SDSS17)

