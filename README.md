# Diabetes Challenge

**Analyze and classify diabetes data using machine learning algorithms with Jupyter Notebooks**

[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/PartORG/ds-diabetes-challenge/workflow-02.yml?branch=main)](https://github.com/PartORG/ds-diabetes-challenge/actions/workflows/workflow-02.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Introduction

The Diabetes Challenge is a dataset-driven project focused on diabetes classification using machine learning algorithms. This repository provides Jupyter Notebooks for understanding pipelines and applying various machine learning techniques to the diabetes dataset. The project includes detailed documentation, a paper explaining the dataset, and a Makefile for setting up the development environment.

This project aims to help data scientists and machine learning enthusiasts understand how to build and evaluate classification models using Python and popular libraries such as scikit-learn, pandas, and seaborn.

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

### Jupyter Notebook for Interactive Data Analysis and Visualization

The project uses Jupyter Notebooks to provide an interactive environment for data analysis, visualization, and machine learning model development.

- **Why It Exists:** Jupyter Notebooks allow users to combine code, visualizations, and narrative text in a single document.
- **Why It Is Useful:** They facilitate experimentation, collaboration, and reproducibility in data science projects.

## How It Works

The Diabetes Challenge project follows these steps:

1. **Data Preparation:** Load and preprocess the diabetes dataset using pandas.
2. **Feature Engineering:** Select relevant features for model training.
3. **Model Selection:** Choose appropriate machine learning algorithms from scikit-learn.
4. **Training and Evaluation:** Train models on the training data and evaluate their performance on the test set.
5. **Visualization:** Use matplotlib, seaborn, and other libraries to visualize results.

## Technology Stack

| Technology | Purpose |
|------------|---------|
| Jupyter Notebook | Interactive environment for data analysis and visualization |
| Python | Programming language for machine learning and data science |
| scikit-learn | Machine learning library for building models |
| pandas | Data manipulation and analysis library |
| matplotlib & seaborn | Libraries for data visualization |
| numpy | Numerical computing library |
| psycopg2-binary, SQLAlchemy | Database connectivity libraries |
| imbalanced-learn | Library for handling imbalanced datasets |

## Requirements

The project requires the following Python version:

- **Python 3.11.3**

Ensure you have `pyenv` installed to manage different Python versions.

## Installation

### macOS

To set up your environment on macOS, use the following commands:

```bash
make setup
```

After running the Makefile, activate the virtual environment:

```bash
source .venv/bin/activate
```

### WindowsOS

For Windows, you can set up the environment using PowerShell or Git-bash. Follow these steps:

**PowerShell:**

```powershell
pyenv local 3.11.3
python -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
```

**Git-bash:**

```bash
pyenv local 3.11.3
python -m venv .venv
source .venv/Scripts/activate
python -m pip install --upgrade pip
pip install -r requirements.txt
```

If you encounter an error during the installation of `pip`, try using:

```bash
python.exe -m pip install --upgrade pip
```

## Configuration

No specific configuration files or environment variables are required for this project.

## Quick Start

To get started with the Diabetes Challenge, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/PartORG/ds-diabetes-challenge.git
   cd ds-diabetes-challenge
   ```

2. Set up your environment as described in the [Installation](#installation) section.

3. Open the Jupyter Notebooks:
   - `1_Pipelines.ipynb` for understanding pipelines.
   - `2_Diabetes_Challenge.ipynb` for applying machine learning algorithms to the diabetes dataset.

## Usage

To run the notebooks, activate your virtual environment and start Jupyter Notebook:

```bash
source .venv/bin/activate  # macOS/Linux
.venv\Scripts\Activate.ps1  # Windows PowerShell
jupyter notebook
```

Navigate to the notebooks in your browser and follow along with the instructions.

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

- **Notebooks:** `1_Pipelines.ipynb` and `2_Diabetes_Challenge.ipynb`
- **Data Files:** `data/diabetes_data.csv`, `data/titanic.csv`
- **Images:** `images/sk_pipeline.png`
- **Makefile:** For setting up the development environment
- **Paper:** `Paper_on_Diabetes_Mellitus_Data_Set.pdf`

## Development

The project uses GitHub Actions for continuous integration and testing. The workflows are defined in `.github/workflows/`.

## Testing

No specific tests are included in this repository.

## Limitations

This project assumes that the diabetes dataset is available and correctly formatted. It does not handle data preprocessing or feature engineering steps, which should be done before running the notebooks.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.