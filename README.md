# Diabetes Predictor with XGBoost

[![Python](https://img.shields.io/badge/python-3.8%2B-blue)](https://www.python.org/)  
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)  
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/your-username/diabetes-predictor/master?filepath=diabetes-prediction.ipynb)

---

## Table of Contents

1. [Project Overview](#project-overview)  
2. [Features](#features)  
3. [Installation](#installation)  
4. [Usage](#usage)  
5. [Notebook Walkthrough](#notebook-walkthrough)  
6. [File Structure](#file-structure)  
7. [Contributing](#contributing)  
8. [License](#license)  

---

## Project Overview

This repository contains a complete end-to-end machine learning pipeline for predicting diabetes based on routine clinical measurements using **XGBoost**. Key objectives:

- Explore and visualize patient data  
- Engineer clinically meaningful features  
- Handle class imbalance in this medical screening task  
- Train, evaluate, and tune an XGBoost classifier  
- Package results in a polished Jupyter notebook for reproducibility  

---

## Features

- **Data Preprocessing**  
  - Handling missing and unknown smoking history  
  - Binning age and BMI into clinically relevant categories  
  - Generating interaction and composite-risk features  
  - Scaling numeric variables for consistency  

- **Exploratory Data Analysis (EDA)**  
  - Class distribution plots  
  - Histogram & boxplot visualizations  
  - Correlation heatmap  

- **Modeling & Evaluation**  
  - Stratified train/test split  
  - XGBoost with `scale_pos_weight` for imbalance  
  - Confusion matrix, ROC-AUC, PR-AUC, Brier Score  
  - Hyperparameter tuning via RandomizedSearchCV  

- **Reproducibility**  
  - Single notebook (`diabetes-prediction.ipynb`) containing code, explanations, and visualizations  
  - Binder badge for one-click, cloud-based execution  

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Jin-yah/diabetes-predictor.git
   cd diabetes-predictor
   ```

2. (Optional) Create and activate a virtual environment:
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## Usage

1. **Launch Jupyter Notebook**  
   ```bash
   jupyter notebook diabetes-prediction.ipynb
   ```

2. **Follow the notebook sections**:  
   - Data loading & preprocessing  
   - Feature engineering  
   - EDA  
   - Model training & evaluation  
   - Hyperparameter tuning  
   - Conclusions & next steps  

---

## Notebook Walkthrough

The Jupyter notebook is organized into the following sections:

1. **Project Overview & Imports**  
2. **Preprocessing**  
3. **Feature Engineering**  
4. **Exploratory Data Analysis (EDA)**  
5. **Model Training**  
6. **Model Evaluation**  
7. **Hyperparameter Tuning**  
8. **Conclusion & Recommendations**  

Each section contains clear markdown explanations, code cells, and inline visualizations for a self-contained analysis.

---

## File Structure

```
diabetes-predictor/
├── diabetes-prediction.ipynb   ← Main analysis notebook
├── requirements.txt            ← Python dependencies
├── LICENSE                     ← MIT license file
└── README.md                   ← Project overview and instructions
```

---

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork this repository.  
2. Create a new branch: `git checkout -b feature/YourFeature`.  
3. Commit your changes: `git commit -m 'Add some feature'`.  
4. Push to the branch: `git push origin feature/YourFeature`.  
5. Open a Pull Request describing your changes.

Please ensure your code follows PEP8 conventions and includes appropriate tests or validations.

---

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use and modify the code for academic and non-commercial purposes, with attribution.

---
