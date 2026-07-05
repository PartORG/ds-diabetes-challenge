# Diabetes Challenge

**"Empower Your Data Science Journey with Our Comprehensive Guide and Codebase"**

[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/PartORG/ds-diabetes-challenge/workflow-02.yml?branch=main&event=push)](https://github.com/PartORG/ds-diabetes-challenge/actions/workflows/workflow-02.yml)
[![GitHub license](https://img.shields.io/github/license/PartORG/ds-diabetes-challenge)](https://github.com/PartORG/ds-diabetes-challenge/blob/main/LICENSE)
[![Python version](https://img.shields.io/badge/python-3.11.3-blue.svg)](https://www.python.org/downloads/release/python-3113/)
[![Jupyter Notebook](https://img.shields.io/badge/jupyter-notebook-3.6.3-green.svg)](https://jupyter.org/)

Welcome to the Diabetes Challenge! This project is designed to help data scientists and machine learning enthusiasts apply their knowledge of classification algorithms on real-world datasets. By participating in this challenge, you'll gain hands-on experience with pipelines, model evaluation, and feature engineering.

## Table of Contents
1. [Features](#features)
2. [How It Works](#how-it-works)
3. [Technology Stack](#technology-stack)
4. [Requirements](#requirements)
5. [Installation](#installation)
6. [Configuration](#configuration)
7. [Quick Start](#quick-start)
8. [Usage](#usage)
9. [Project Structure](#project-structure)
10. [Development](#development)
11. [Testing](#testing)
12. [Limitations](#limitations)
13. [License](#license)

## Features
### Pipelines
**What it does:**  
Pipelines allow you to chain multiple data processing steps and machine learning models together in a sequential manner.

**Why it exists:**  
Pipelines help streamline the workflow, ensuring that each step is applied correctly and efficiently.

**Why it is useful:**  
They simplify model development and deployment, reducing the risk of errors and improving reproducibility.

### Model Evaluation
**What it does:**  
Evaluate the performance of machine learning models using various metrics.

**Why it exists:**  
Understanding how well your models are performing is crucial for making informed decisions.

**Why it is useful:**  
It helps in selecting the best model and tuning hyperparameters effectively.

## How It Works
The project follows a structured workflow:
1. **Data Preparation:** Load and preprocess the dataset.
2. **Feature Engineering:** Extract relevant features from the data.
3. **Model Training:** Train multiple classification models using pipelines.
4. **Evaluation:** Assess the performance of each model using appropriate metrics.

## Technology Stack

| Technology | Purpose |
|------------|---------|
| Jupyter Notebook | Interactive environment for data analysis and visualization. |
| scikit-learn | Machine learning library for building and evaluating models. |
| pandas | Data manipulation and analysis library. |
| numpy | Numerical computing library. |
| matplotlib & seaborn | Libraries for data visualization. |
| psycopg2-binary, SQLAlchemy | Database interaction libraries. |
| imbalanced-learn | Library for handling imbalanced datasets. |

## Requirements
- Python 3.11.3
- Jupyter Notebook

## Installation
### macOS
```bash
make setup
source .venv/bin/activate
```

### WindowsOS (PowerShell)
```powershell
pyenv local 3.11.3
python -m venv .venv
.venv\Scripts\Activate.ps1
pip install --upgrade pip
pip install -r requirements.txt
```

### WindowsOS (Git-bash)
```bash
pyenv local 3.11.3
python -m venv .venv
source .venv/Scripts/activate
python -m pip install --upgrade pip
pip install -r requirements.txt
```

## Configuration
No specific configuration files are required.

## Quick Start
To get started, run the following commands:
```bash
make setup
source .venv/bin/activate
jupyter notebook 2_Diabetes_Challenge.ipynb
```

## Usage
Open the `2_Diabetes_Challenge.ipynb` notebook in Jupyter and follow the instructions.

## Project Structure
```
ds-diabetes-challenge/
├── .github/workflows/
│   ├── REGX_test_import_libraries.sh
│   ├── discord-webhook-notify.yml
│   ├── replacement.yml
│   └── workflow-02.yml
├── .gitignore
├── 1_Pipelines.ipynb
├── 2_Diabetes_Challenge.ipynb
├── Diabete_Challenge_DG.ipynb
├── Makefile
├── Paper_on_Diabetes_Mellitus_Data_Set.pdf
├── README.md
├── data/
│   ├── diabetes_data.csv
│   └── titanic.csv
├── images/
│   └── sk_pipeline.png
└── requirements.txt
```

## Development
The project uses a Makefile for environment setup. Contributions are welcome!

## Testing
No tests are included in this repository.

## Limitations
- The dataset is relatively small, which may limit the performance of some models.
- The project does not include advanced feature engineering techniques.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.