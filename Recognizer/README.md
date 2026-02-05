# Recognizer: Digits 3 vs 8

## Project Overview

This project solves a digit recognition task from a Kaggle-style competition.  
The goal is to build a machine learning model that classifies handwritten digits **3** and **8** based on their pixel representations.

The dataset contains transformed images of digits taken from different fonts. The images are distorted, scaled, rotated, and placed on random backgrounds, making the classification task more challenging.

Competition link:  
🔗 https://www.kaggle.com/competitions/25-hse-recognizer/overview


## Task Description

The objective is to train a classification model using the provided training dataset and generate predictions for the test dataset.

### Training dataset (`trainYX.csv`)
Each row contains:
- `id` — sample identifier
- `y` — digit label (`3` or `8`)
- 1024 feature columns representing pixel brightness intensities

### Test dataset (`testX.csv`)
Each row contains:
- `id`
- 1024 feature columns

The final output must be a CSV file containing predictions for the test dataset.


## Dataset

The dataset is provided as part of the Kaggle competition.

Due to size limitations, the dataset is not included in this repository.

### How to use the dataset

1. Download the competition dataset from Kaggle  
   https://www.kaggle.com/competitions/25-hse-recognizer/data

3. Extract dataset files

4. Place the following files in the project directory:
   - `trainYX.csv`
   - `testX.csv`


## Project Workflow

- Data loading and preprocessing
- Feature inspection
- Model training
- Model evaluation
- Prediction generation for submission


## Modeling Approach

The project applies machine learning classification techniques to distinguish between digits 3 and 8 based on pixel intensity features.


## How to Run

### 1) Clone repository
```bash
git clone https://github.com/ekaterinassss/ml_assignments.git
cd ml_assignments/digit_recognizer
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

Open `Recognizer_solution.ipynb` and run all cells to generate submission predictions.
