# ECG-Project-2025

---

### 📦 Libraries Used

| Library                   | Purpose                                             |
| ------------------------- | --------------------------------------------------- |
| `pandas`                  | Data manipulation and preprocessing                 |
| `numpy`                   | Numerical computations                              |
| `matplotlib.pyplot`       | Data visualization                                  |
| `seaborn`                 | Statistical data visualization                      |
| `neurokit2`               | ECG signal cleaning and feature extraction          |
| `scipy.stats`             | Box-Cox transformation for normalization            |
| `sklearn.model_selection` | Dataset splitting (train/val/test)                  |
| `sklearn.metrics`         | Model evaluation (accuracy, confusion matrix, etc.) |
| `tensorflow.keras`        | Neural network model building                       |
| `tabulate`                | Pretty-printing tables in console output            |

* Python version: **3.12.1**

---

### 🔍 Variables Used in Prediction

| Variable Name | Description                                                       | Type                    | Role            |
| ------------- | ----------------------------------------------------------------- | ----------------------- | --------------- |
| `age`         | Patient's age (transformed with Box-Cox)                          | Numerical               | Feature (input) |
| `sex`         | Biological sex (0 = Female, 1 = Male)                             | Categorical             | Feature (input) |
| `ecg_signals` | 12-lead ECG time-series signals                                   | Signal (2D NumPy array) | Feature (input) |
| `obstruction` | Simulated label for coronary artery obstruction (1 = Yes, 0 = No) | Binary                  | Target (output) |

> 💡 Note: Variables like `scp_code`, `scp_weight`, `AHA code`, and `ecg_id` were explored but not retained in the final input feature set. `ecg_signals` were processed to extract features (e.g., `HR_mean`, `QRS_amp`) or used directly in deep learning.

---
