# Shallow Neural Network Optimisation for MNIST

This project investigates how to optimise the architecture of **shallow neural networks** for the **MNIST image classification task**, using three different hyperparameter search strategies:

- **Grid Search**
- **Random Search**
- **Bayesian Optimisation** (via Optuna)

In addition to accuracy, the project evaluates models based on computational cost, including parameter count and FLOPs.

---

## 📁 Files

| Filename                          | Description |
|----------------------------------|-------------|
| `Grid search.ipynb`              | Explores combinations of network parameters using a structured grid approach. |
| `Random Search.ipynb`            | Randomly samples hyperparameter configurations for comparison. |
| `Bayesian Optimisation.ipynb` | Implements Bayesian optimisation using Optuna; collects model metrics like accuracy, precision, recall, F1-score, FLOPs, and parameter count. |
| `optimisation_results_with_metrics.xlsx` | Spreadsheet of results for each trial, including performance and model size. |

---

## 🧪 Techniques

Each approach optimises:
- Number of layers
- Units per layer
- Activation function
- Dropout rate

Evaluation is performed on the **MNIST** dataset (grayscale handwritten digits).

---

## 📊 Metrics Collected

- **Accuracy**
- **Precision / Recall / F1-score**
- **Training Time (seconds)**
- **Number of Parameters**
- **FLOPs (Floating Point Operations)**

These metrics help assess the trade-off between **accuracy** and **efficiency**.

---

## 📦 Requirements

To run the notebooks, you’ll need:

```bash
python >= 3.8
tensorflow
optuna
numpy
pandas
scikit-learn
openpyxl   # for Excel export
