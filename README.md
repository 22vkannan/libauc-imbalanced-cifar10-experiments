# libauc-imbalanced-cifar10-experiments
Comparative experiments on CIFAR-10 using LibAUC loss functions to optimize AUROC, AUPRC, and a combined objective. Includes grid search over weighted loss combinations and robust handling of imbalanced data with DualSampler.

# CIFAR-10 AUROC vs AUPRC Optimization using LibAUC

This project compares different loss functions for learning on an imbalanced version of CIFAR-10 using [LibAUC](https://github.com/Optimization-AI/LibAUC). We focus on optimizing AUROC, AUPRC, and a combined objective.

## 📌 Experiments

- ✅ **Experiment 1:** Optimize AUROC with `AUCMLoss`
- ✅ **Experiment 2:** Optimize AUPRC with `APLoss`
- ✅ **Experiment 3:** Combine AUCMLoss + APLoss using different `r` values (`r ∈ {0.2, 0.5, 0.8}`)

## 🧪 Dataset

- **CIFAR-10**
- Artificially imbalanced to simulate real-world scenarios
- DualSampler used to ensure each batch has at least one positive sample

## 📈 Results Summary

| r value | Best AUPRC |
|--------|-------------|
| 0.2    | TBD         |
| 0.5    | 0.6484      |
| 0.8    | TBD         |

*(Update after grid search)*

## 🛠️ Setup

```bash
pip install -r requirements.txt
