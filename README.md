# PartORG/ds-diabetes-challenge

Analyze and predict diabetes outcomes using machine learning models.

## Overview

This repository contains a Jupyter Notebook challenge for implementing classification algorithms on new data, comparing their performance, and understanding pipelines in scikit-learn. The dataset is included in `data/diabetes_data.csv`, and the challenge details are provided in `2_Diabetes_Challenge.ipynb`.

## Requirements

To run this project, you need the following dependencies with specified versions:

- jupyterlab==3.6.3
- Pillow==9.5.0
- matplotlib==3.7.1
- seaborn==0.12.2
- numpy==1.24.3
- pandas==2.0.1
- scikit-learn==1.2.2
- python-dotenv==1.0.0
- psycopg2-binary
- SQLAlchemy==2.0.15
- imbalanced-learn

## Installation

### macOS

To set up your environment on macOS, use the following commands:

```bash
make setup
```

After that, activate your environment with:

```bash
source .venv/bin/activate
```

### WindowsOS

For WindowsOS, follow these steps:

#### PowerShell CLI

```powershell
pyenv local 3.11.3
python -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
```

#### Git-bash CLI

```bash
pyenv local 3.11.3
python -m venv .venv
source .venv/Scripts/activate
python -m pip install --upgrade pip
pip install -r requirements.txt
```

If you encounter an error when trying to run `pip install --upgrade pip`, use:

```bash
python.exe -m pip install --upgrade pip
```

## Usage

To run the project, execute the following commands:

1. Activate your virtual environment.
2. Open the Jupyter Notebook by running:

   ```bash
   jupyter lab 2_Diabetes_Challenge.ipynb
   ```

This will open the Diabetes Challenge notebook in JupyterLab where you can follow along with the instructions and complete the challenge.