# Phoneme Classification


This project is based on the Kaggle competition:

https://www.kaggle.com/competitions/hse-phoneme-5/overview


## Project Overview

This project focuses on phoneme classification using acoustic spectral features extracted from speech signals.

The goal is to predict phoneme class **g** based on its spectral representation.  
This task is based on an example from *The Elements of Statistical Learning* (Hastie, Tibshirani, Friedman).


## Dataset

The dataset originates from the **TIMIT Acoustic-Phonetic Continuous Speech Corpus**, a widely used benchmark in speech recognition research.

The data were prepared in collaboration between Andreas Buja, Werner Stuetzle, and Martin Maechler and were used in the paper:

> Hastie, Buja, Tibshirani (1995) – Penalized Discriminant Analysis


https://www.kaggle.com/competitions/hse-phoneme-5/data

Due to file size limitations, the dataset is not included in this repository.


### Dataset Characteristics

- 4509 speech frames
- 5 phoneme classes:
  - `aa`
  - `ao`
  - `dcl`
  - `iy`
  - `sh`
- Each frame:
  - Duration: 32 ms
  - 512 raw signal samples
  - Converted into log-periodogram representation
  - 256 spectral features (`x.1 – x.256`)

Additional columns:
- `g` — phoneme label
- `speaker` — speaker ID


## Project Workflow

- Data preprocessing
- Feature analysis
- Model training
- Model evaluation
- Classification performance comparison


## Models

The project implements classification algorithms for phoneme recognition using acoustic spectral features.


## Evaluation

Model performance is evaluated using classification metrics such as:

- Accuracy
- Confusion matrix
- Classification error analysis


## Tech Stack

- Python
- NumPy
- Pandas
- Scikit-learn
- Matplotlib / Seaborn



## How to Run

### 1) Clone repository
```bash
git clone https://github.com/YOUR_USERNAME/ml_assignments.git
cd ml_assignments/phoneme_classification
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

Open `Phonemes_solution.ipynb`.
