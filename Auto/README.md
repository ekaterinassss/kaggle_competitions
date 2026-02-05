# Vehicle MPG and Price Prediction

## Project Overview

This project focuses on predicting vehicle fuel efficiency and price based on automobile characteristics.

The goal is to build machine learning models that predict:

- City fuel efficiency (city MPG)
- Highway fuel efficiency (highway MPG)
- Vehicle price

The project is based on a Kaggle competition involving real-world automotive data.

Competition link:  
https://www.kaggle.com/competitions/25-hse-auto/overview


##  Task Description

The task is a **multi-target regression problem** where models must simultaneously predict multiple numerical targets describing vehicle performance and cost.

### Target Variables

- `city-mpg` — fuel efficiency in city driving
- `highway-mpg` — fuel efficiency in highway driving
- `price` — vehicle market price


## 📊 Dataset

The dataset was derived from a larger automobile dataset available on OpenML.

Original dataset source:  
🔗 https://www.openml.org/search?type=data&sort=runs&id=1189&status=active

The competition dataset contains vehicle characteristics such as engine parameters, body specifications, and performance features.



## 🔍 Project Workflow

- Data loading and preprocessing
- Feature analysis
- Handling missing values
- Model training
- Multi-target prediction
- Submission file generation


## Modeling Approach

Machine learning regression algorithms are applied to predict multiple vehicle characteristics based on automobile attributes.


## Evaluation

Model performance is evaluated using regression metrics such as:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)


## Tech Stack

- Python
- NumPy
- Pandas
- Scikit-learn
- Matplotlib / Seaborn


## How to Run

### 1) Clone repository
```bash
git clone https://github.com/ekaterinassss/kaggle_competitions.git
cd kaggle_competitions/Auto
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

Open `Auto_solution.ipynb`.


