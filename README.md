## 🚨 Anomaly Detection for Fraud Detection using Isolation Forest

This project implements an **unsupervised anomaly detection** approach using the **Isolation Forest** algorithm to identify fraudulent transactions in a highly imbalanced dataset.

---

### ✅ Model Summary

* **Algorithm**: Isolation Forest
* **Goal**: Detect anomalies (fraudulent activities) within a dataset dominated by legitimate transactions.
* **Label Convention**:

  * `0` → Fraud (Anomalous)
  * `1` → Legitimate (Normal)

---

### 📊 Classification Report

| Metric        | Class 0 (Fraud) | Class 1 (Legit) |
| ------------- | --------------- | --------------- |
| **Precision** | 0.54            | 1.00            |
| **Recall**    | 0.93            | 0.96            |
| **F1-score**  | 0.69            | 0.98            |
| **Support**   | 2,510           | 48,490          |

**Overall Accuracy**: **0.96**
**Macro Average F1-Score**: **0.83**
**Weighted Average F1-Score**: **0.96**

---

### 🔍 Insights

* The model achieves **high recall (0.93)** for fraudulent cases, which is crucial in fraud detection where missing a fraud is costlier than raising a false alarm.
* **Precision for fraud (0.54)** shows some false positives (i.e., misclassifying legit transactions as fraud), which is expected in anomaly detection.
* The **F1-score of 0.69** for fraud indicates a solid balance between precision and recall for the minority class.
* The classifier performs **exceptionally well on legitimate transactions** with nearly perfect scores across all metrics.
* Overall **96% accuracy** demonstrates strong model generalization, especially given the class imbalance.

---

### ⚖️ Conclusion

The Isolation Forest model proves to be a valuable tool for unsupervised fraud detection. Its ability to correctly identify a high proportion of fraud cases with minimal training supervision makes it suitable for real-world financial systems, where labeled data may be scarce or unreliable.

---
