# Machine Failure Prediction using ML & Deep Learning
![License](https://img.shields.io/badge/license-MIT-green)
![Language](https://img.shields.io/badge/language-Python-blue)
![Framework](https://img.shields.io/badge/framework-TensorFlow-orange)
![ML](https://img.shields.io/badge/ML-ScikitLearn-yellowgreen)

Predictive maintenance project for the UC course on Computational Learning. Implements data preprocessing, classification (binary and multi-class), and evaluation using Neural Networks, SVM, and Random Forest to predict machine failures.

---

## Overview
This repository contains the final project for the **Computational Learning (AC)** course.  
The main goals are:
1. Predict if a machine will fail (**binary classification**)  
2. Identify the type of failure (**multi-class classification**)  

The project includes preprocessing, model training, and evaluation with clear metrics.

---

## Repository Structure
```plaintext
.
├── Project/
│   └── AC_Project.ipynb      # Main notebook with all code (preprocessing, training, evaluation)
├── predictive_maintenance.csv # Dataset used in the project
├── LICENSE                   # MIT license
└── README.md                 # This file
```

---

## Dataset
The project expects a dataset with:

**IDs / Metadata:**  
- UDI, Product_ID, Type  

**Sensors / Process:**  
- Air_temperature, Process_temperature, Rotational_speed, Torque, Tool_wear  

**Targets:**  
- `Target` → failure vs no failure (binary)  
- `Failure_Type` → type of failure (multi-class)  

*(column names may change depending on the dataset)*

---

## Requirements
- Python ≥ 3.10  

Main packages:
- numpy, pandas  
- scikit-learn  
- imbalanced-learn  
- matplotlib, seaborn  
- tensorflow (Keras)  

Install with:
```bash
pip install -r requirements.txt
```

---

## 🚀 How to Run

### Option A) Run locally (Jupyter)
1) Create and activate a virtual environment (optional)
   python -m venv .venv
   source .venv/bin/activate    # Windows: .venv\Scripts\activate

2) Install packages
   pip install numpy pandas scikit-learn imbalanced-learn matplotlib seaborn tensorflow notebook

3) Start Jupyter
   jupyter notebook

4) Open and run:
   Project/AC_Project.ipynb

### Option B) Google Colab
1) Open the notebook `Project/AC_Project.ipynb` in Colab
2) Upload `predictive_maintenance.csv`
3) Run all cells


---

## Methodology
**Models used:**
- Neural Networks (Keras/TensorFlow)  
- Support Vector Machine (SVM)  
- Random Forest  

**Preprocessing:**
- Drop irrelevant columns (Type, UDI, Product_ID)  
- Normalize numerical values  
- Oversampling to reduce class imbalance  

**Evaluation:**
- Main metrics: F1-score and confusion matrix  
- Check trade-off between False Negatives (FN) and False Positives (FP)  

Full details in the report

---

## Results
- **Binary task** → failure vs no failure  
- **Multi-class task** → classify failure type  
- Metrics and confusion matrices are saved in `reports/`  

---

## Notes
- The folder `data/` is ignored in git (`.gitignore`) → datasets are not included.  
- Do not upload personal or sensitive data.  
- For Neural Networks, GPU support is recommended but optional.  

---

## Report
The final report can be accessed at the following link (Dropbox):  
[Report.pdf](https://www.dropbox.com/scl/fi/6hl6vi5mtxefozfoofra9/Report.pdf?rlkey=t094k5x0mdp9k7njh39l717xu&st=8xa68wkz&dl=0)

Access is restricted → please request access if needed.

--- 

## Authors
- Miguel Cruz
- Rúben Castanheira

---

## License
This project is licensed under the MIT License. See LICENSE for details.
