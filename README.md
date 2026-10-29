# MLflow Experiment Tracking and Data Drift Detection

## Overview
This project demonstrates machine learning experiment tracking using MLflow and data drift detection using the Kolmogorov-Smirnov (KS) test.

## Features
- Iris dataset classification using Random Forest.
- Experiment tracking with MLflow.
- Logging model parameters and evaluation metrics.
- Comparison of Random Forest models.
- Data drift detection using the KS test.
- Tracking experiment results in MLflow.

## Technologies Used
- Python
- MLflow
- Scikit-learn
- Pandas
- NumPy
- SciPy

## Project Files
- `mlflow_exp.py` — Model training, evaluation, and MLflow tracking.
- `drift_analysis.py` — Data drift detection using the KS test.
- `requirements.txt` — Python dependencies.
- `.gitignore` — Files excluded from Git tracking.

## Setup

Create and activate a virtual environment, then install dependencies:

```bash
python -m venv venv
```

Windows:

```cmd
venv\Scripts\activate
```

Install the packages:

```bash
pip install -r requirements.txt
```

## Run the Experiment

```bash
python mlflow_exp.py
```

## Run the MLflow UI

```bash
mlflow ui --backend-store-uri sqlite:///mlflow.db --host 127.0.0.1 --port 5000
```

Open http://127.0.0.1:5000 in your browser.

## Data Drift Detection

Run the drift analysis script:

```bash
python drift_analysis.py
```

## Note
The local MLflow database and run artifacts are excluded from Git. Run the experiment locally to generate tracking data.
