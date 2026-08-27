# Botanical Plant Species Classification & Thriving Predictor 📊🤖

[![CI/CD Pipeline](https://github.com/Yuossef-Ashraf/ML_Plant_Species_Classification/actions/workflows/tests.yml/badge.svg)](https://github.com/Yuossef-Ashraf/ML_Plant_Species_Classification/actions)
[![Python Version](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 🎯 What This Does

Multi-class ecological classification model identifying plant species and predicting thriving viability under varying soil, sunlight, water, and pH conditions.

---

## ✨ Key Features

- 🔬 **Comprehensive Pipeline:** Automated data cleaning, one-hot encoding, feature scaling, and model persistence.
- 📈 **High-Performance Models:** Evaluates and tunes `XGBoost Classifier, Random Forest, K-Nearest Neighbors, Multi-Layer Perceptron`.
- 💻 **CLI & API Inference:** Modular `pipeline.py` CLI supporting immediate prediction and validation on unseen data.
- 🛡️ **Senior-Grade Engineering:** Includes automated pytest testing, GitHub Actions CI/CD workflows, and flake8 compliance.

---

## 📊 Performance Benchmarks

| Evaluation Metric | Benchmark Result |
| :--- | :---: |
| **Accuracy** | **96.0%** |
| **Macro Precision** | **0.95** |
| **Macro Recall** | **0.96** |
| **F1-Score** | **0.955** |

---

## 🚀 Quick Start

```bash
git clone https://github.com/Yuossef-Ashraf/ML_Plant_Species_Classification.git
cd ML_Plant_Species_Classification

# Virtual environment
python -m venv .venv
.\.venv\Scripts\activate   # Windows
source .venv/bin/activate  # Linux/macOS

# Install dependencies
pip install -r requirements.txt

# Run Model Training & Evaluation
python pipeline.py --data "plants_dataset_euhm_itai_07.csv"
```

---

## 🧪 Testing & CI/CD

```bash
pytest tests/ -v
flake8 . --max-line-length=120 --exclude=.venv,__pycache__
```

---

## 👨‍💻 Author
**Yuossef Ashraf** - [@Yuossef-Ashraf](https://github.com/Yuossef-Ashraf)

## 📄 License
MIT License
