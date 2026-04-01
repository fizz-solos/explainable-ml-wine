# 🍷 Explainable ML - UCI Wine Classification

![Python](https://img.shields.io/badge/Python-3.8+-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![sklearn](https://img.shields.io/badge/scikit--learn-latest-green)
![License](https://img.shields.io/badge/License-MIT-yellow)

## What is this?
This project applies two explainable machine learning techniques to classify wines using the UCI Wine dataset. The goal was not just to get good accuracy but to actually understand **why** the model makes each prediction.

---

## Models Used
| Model | Accuracy | F1-Score |
|---|---|---|
| Logistic Regression (L1) | 98.2% | 0.983 |
| Logistic Regression (L2) | 98.2% | 0.983 |
| Decision Tree | 96.3% | 0.964 |

---

## Explainability Outputs
| Technique | Explainability Method |
|---|---|
| Logistic Regression L1 | Coefficient Heatmap |
| Logistic Regression L1 | Regularization Path |
| Decision Tree | If-Then Rules |
| Decision Tree | Tree Visualization |
| Decision Tree | Feature Importance |

---

## Project Structure
```
📦 explainable-ml-wine
 ┣ 📓 Wine Classification.ipynb
 ┣ 📁 outputs/
 ┃ ┣ 🖼️ eda_class_distribution.png
 ┃ ┣ 🖼️ eda_feature_distributions.png
 ┃ ┣ 🖼️ lr_l1_coefficients_heatmap.png
 ┃ ┣ 🖼️ lr_l1_regularization_path.png
 ┃ ┣ 🖼️ decision_tree_plot.png
 ┃ ┣ 🖼️ decision_tree_feature_importance.png
 ┃ ┣ 🖼️ confusion_matrices.png
 ┃ ┣ 🖼️ model_comparison.png
 ┃ ┣ 📄 decision_tree_rules.txt
 ┃ ┗ 📄 metrics_summary.csv
 ┣ 📄 README.md
 ┗ 📄 LICENSE
```

---

## How to Run

### 1. Clone the repo
```bash
git clone https://github.com/fizz-solos/explainable-ml-wine.git
cd explainable-ml-wine
```

### 2. Install dependencies
```bash
pip install numpy pandas matplotlib scikit-learn jupyter
```

### 3. Open the notebook
```bash
jupyter notebook "Wine Classification.ipynb"
```

### 4. Run all cells top to bottom ✅
All outputs save automatically to the `outputs/` folder

---

## Dataset
- **Name:** UCI Wine Dataset
- **Source:** [UCI ML Repository](https://archive.ics.uci.edu/ml/datasets/wine)
- **Samples:** 178 wines
- **Features:** 13 chemical properties
- **Classes:** 3 wine types

---

## Key Finding
Both models agreed that **Flavanoids** and **Proline** are the most important features for classifying wine types

---

## Dependencies
```
numpy
pandas
matplotlib
scikit-learn
jupyter
```

---

## License
MIT License - see [LICENSE](LICENSE) for details