# Bacteria DNA Sequence Classification

## Project Overview

This project focuses on classifying bacterial species based on DNA sequence data.

The goal is to build a machine learning model that distinguishes between two bacteria classes using genomic sequences composed of nucleotide symbols.

The project was completed as part of an in-class Kaggle competition.

Competition link:  
🔗 https://www.kaggle.com/competitions/25-hse-genomics/overview


## Context

DNA sequences contain biological information that can be used to distinguish between organisms. Sequence classification is widely used in genomics, microbiology, and medical research.

This project applies machine learning techniques to classify bacterial species based on DNA sequences.


## Dataset

The dataset is based on the **Genomics OOD dataset** provided by TensorFlow.

Dataset source:  
🔗 https://www.tensorflow.org/datasets/catalog/genomics_ood

Each observation represents a DNA sequence consisting of nucleotide symbols:

- A — Adenine  
- C — Cytosine  
- G — Guanine  
- T — Thymine  

The task is a **binary classification problem**.


## Dataset Access

The dataset is not included in this repository due to size limitations.

### How to use the dataset

1. Download dataset from Kaggle or TensorFlow Datasets
2. Extract dataset files
3. Place dataset files in the project directory



## Project Workflow

- DNA sequence loading
- Sequence preprocessing
- Sequence encoding
- Feature matrix construction
- Model training
- Model evaluation
- Submission prediction generation


## Feature Engineering

DNA sequences are converted into numerical representations using sequence encoding techniques, allowing classical machine learning algorithms to process genomic data.


##  Modeling Approach

Machine learning classification algorithms are applied to encoded DNA sequence features to distinguish between bacterial species.


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
- Matplotlib / Seaborn


## How to Run

### 1) Clone repository
```bash
git clone https://github.com/ekaterinassss/kaggle_competitions.git
cd kaggle_competitions/Genomics
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

Open `Genomics_solution.ipynb`.


