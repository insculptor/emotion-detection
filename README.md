# Emotion Detection

This repository contains an end-to-end machine learning project for emotion detection using XGBoost. The project demonstrates a complete MLOps workflow, including data preprocessing, feature engineering, model training, evaluation, and deployment. It uses DVC for data version control and GitHub Actions for continuous integration and deployment.

## Table of Contents

- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [MLOps Workflow](#mlops-workflow)
- [License](#license)

## Project Structure
Emotion-Detection/
│
├── data/
│ ├── raw/
│ ├── processed/
│ └── features/
├── models/
│ └── model.pkl
├── scripts/
│ ├── data_preprocessing.py
│ ├── feature_engineering.py
│ ├── model_training.py
│ ├── model_evaluation.py
│ └── requirements.txt
├── .github/
│ └── workflows/
│ └── ci.yml
├── params.yaml
├── dvc.yaml
├── dvc.lock
├── README.md
├── .gitignore
└── .env

## Installation

1. **Clone the repository:**

```bash
git clone https://github.com/yourusername/Emotion-Detection.git
cd Emotion-Detection

2. **Create a new conda environment and install dependencies:**

```bash
conda create --name emotion_detection python=3.12
conda activate emotion_detection
pip install -r scripts/requirements.txt

3. **Set up environment variables:**
Create a .env file in the root directory and add the following variables:

```bash
BASE_DATA_DIR=./data
BASE_MODEL_DIR=./models

4. **Download NLTK resources:**

```bash
python -m nltk.downloader wordnet stopwords4


## Usage

**Data Preprocessing**
Run the data preprocessing script to clean and prepare the data:

```bash
python scripts/data_preprocessing.py


**Feature Engineering**
Run the feature engineering script to extract features:

```bash
python scripts/feature_engineering.py

**Model Training**
Run the model training script to train the XGBoost model:

```bash
python scripts/model_training.py

**Model Evaluation**
Run the model evaluation script to evaluate the model's performance:

```bash
python scripts/model_evaluation.py