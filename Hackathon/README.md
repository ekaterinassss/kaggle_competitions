# Particle Entry Position Reconstruction in Electromagnetic Calorimeter

## Project Overview

This project focuses on reconstructing the entry position of particles in an electromagnetic calorimeter using machine learning techniques.

The goal is to predict the spatial coordinates **(x, y)** of particle entry based on energy deposits recorded in calorimeter detector cells.

The project was completed as part of a Kaggle competition focused on particle detector data analysis.

Competition link:  
https://www.kaggle.com/competitions/ml-1-hackathon/overview


## Physical Background

Particles passing through matter lose energy via electromagnetic interactions.  
An electromagnetic calorimeter measures this energy by recording energy deposits in detector cells.

When a particle enters the calorimeter:

- High-energy particles affect multiple cells
- Low-energy particles affect fewer cells
- The set of activated cells forms a **calorimetric cluster**

By analyzing the spatial distribution of energy deposits, it is possible to reconstruct particle entry coordinates with precision exceeding individual cell size.


## Calorimeter Structure

- Total size: **60.6 cm × 60.6 cm**
- Grid: **15 × 15 cells**
- Total cells: **225**
- Cell size: **4.04 cm × 4.04 cm**
- Coordinate origin located at central cell


## Dataset

The dataset contains simulated particle interactions in the calorimeter.

### Input Features

- Energy deposits recorded in each calorimeter cell
- Each observation corresponds to a calorimetric cluster

### Target Variables

- `x` — particle entry coordinate
- `y` — particle entry coordinate


## Dataset Access

The dataset is provided as part of the Kaggle competition and is not included in this repository due to size limitations.

Download dataset from Kaggle:
https://www.kaggle.com/competitions/ml-1-hackathon/data


## Project Workflow

- Data loading and preprocessing
- Feature exploration
- Spatial energy distribution analysis
- Model training
- Multi-output regression
- Submission prediction generation


## Modeling Approach

Machine learning regression algorithms are used to reconstruct particle entry coordinates based on energy deposit patterns across calorimeter cells.


## Evaluation

Model performance is evaluated using:

### Mean Columnwise Root Mean Squared Error (MCRMSE)

The metric averages prediction errors across spatial coordinates:

- RMSE_x — error for x coordinate
- RMSE_y — error for y coordinate

Lower MCRMSE indicates better spatial reconstruction accuracy.


## How to Run

### 1) Clone repository
```bash
git clone https://github.com/ekaterinassss/kaggle_competitions.git
cd kaggle_competitions/Hackathon_solution
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

Open `Hackathon_solution.ipynb`.


## Scientific Context

Particle position reconstruction using calorimetric data is a fundamental task in high-energy physics experiments.

This project demonstrates how machine learning can achieve spatial resolution exceeding detector cell size by analyzing energy distribution patterns.

