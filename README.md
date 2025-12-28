# Real-Time IoT Intrusion Detection Using a Hybrid Machine and Deep Learning Framework  
### Comprehensive Evaluation on CIC-IoT-2025

## 📄 Associated Paper
**Title:** Real-Time IoT Intrusion Detection Using a Hybrid Machine and Deep Learning Framework: Comprehensive Evaluation on CIC-IoT-2025  

**Authors:**  
- **Zineb ADAMMICHE**, National Institute of Posts and Telecommunications (INPT), Rabat, Morocco  
- **Prof. Iyad LAHSEN-CHERIF**, National Institute of Posts and Telecommunications (INPT), Rabat, Morocco  

📧 adammiche.zineb@master.inpt.ac.ma  
📧 iyad.lahsencherif@inpt.ac.ma  

---

## 📌 Overview
This repository provides the **implementation notebooks** accompanying the research paper *“Real-Time IoT Intrusion Detection Using a Hybrid Machine and Deep Learning Framework”*.  

The work presents a **rigorous, fair, and unified comparison** between:
- **Classical Machine Learning (ML)** models  
- **Advanced Deep Learning (DL)** architectures  

for **intrusion detection in IoT networks**, using the **CIC-IoT-2025 dataset**.

The study evaluates **binary (benign vs attack)** and **multiclass (8 attack types)** intrusion detection under **identical preprocessing, feature engineering, and evaluation protocols**.

---

## 🎯 Research Objectives
- Perform a **head-to-head comparison** of ML and DL paradigms for IoT IDS
- Analyze the **accuracy–efficiency trade-off** in resource-constrained IoT environments
- Evaluate models under **binary and multiclass classification**
- Investigate the impact of **feature engineering vs automatic feature learning**
- Provide **practical deployment recommendations** for real-world IoT systems

---

## 🚀 Main Contributions
- ✅ Unified experimental framework for ML and DL on CIC-IoT-2025  
- ✅ Correlation-based feature selection (71 → 48 features)  
- ✅ Evaluation of **6 ML configurations** and **4 DL architectures**  
- ✅ Detailed per-class analysis across **8 attack categories**  
- ✅ Computational efficiency benchmarking (training time, inference latency, memory)  
- ✅ Actionable deployment guidance (edge, cloud, critical infrastructure)

---

## 📊 Dataset
- **Dataset:** CIC-IoT-2025  
- **Source:** Canadian Institute for Cybersecurity (UNB)  
- **Records:** 685,671 network flows  
- **Features:** 71 numerical flow-based features  
- **Classes:**  
  - Binary: Benign / Attack  
  - Multiclass (8): Benign, BruteForce, DDoS, DoS, Malware, MITM, Reconnaissance, Web  

⚠️ **Dataset not included** due to size constraints.  
📎 Download: CIC-IoT-2025 (official UNB website)

---

## 🧠 Methodology Summary
The framework adopts a **dual-track evaluation pipeline**:

### 1️⃣ Data Processing
- Cleaning NaN and infinite values  
- Standardization (StandardScaler)  
- Class imbalance analysis  
- Correlation-based feature selection  
- Dimensionality reduction (PCA for ML)

### 2️⃣ Machine Learning Track
Algorithms:
- Random Forest  
- XGBoost  
- LightGBM  
- Ensemble models (RF + XGB + LGB)

Key strengths:
- High accuracy with low computational cost  
- Strong performance on rare attack classes  
- High interpretability

### 3️⃣ Deep Learning Track
Architectures:
- CNN  
- CNN + BiLSTM  
- Transformer  
- Hybrid CNN + BiLSTM + Transformer  

Key strengths:
- Automatic feature learning  
- Temporal and sequential pattern modeling  

---

## 🧪 Experimental Scenarios
- **Binary Classification:** Benign vs Attack  
- **Multiclass Classification:** 8 attack categories  

Metrics:
- Accuracy  
- Precision  
- Recall  
- F1-score  
- ROC-AUC  
- Training time, inference latency, memory usage  

---

## 📈 Key Results (From the Paper)

### 🔹 Best Machine Learning Models
- **Binary:** XGBoost + LightGBM  
  - Accuracy: **96%**
  - ROC-AUC: **0.9844**
- **Multiclass:** LightGBM  
  - Accuracy: **96%**
  - Strong performance on rare classes (Bruteforce, Recon)

### 🔹 Best Deep Learning Models
- **Binary:** Hybrid CNN + BiLSTM + Transformer  
  - Accuracy: **96%**
- **Multiclass:** CNN + BiLSTM  
  - Accuracy: **94.4%**

### 🔹 Efficiency Comparison
| Approach | Training Time | Inference | Memory |
|--------|---------------|-----------|--------|
| ML     | 2–4 min       | 1.8–3.2 ms | 52–145 MB |
| DL     | 9–19 min      | 8.5–15 ms  | 12–35 MB |

---
Hybrid-ML-DL-IDS-for-IoT-CIC-IoT-2025/
│
├── Notebook_Machine Learning Approach for IDS.ipynb
│ └─ Classical ML models and ensemble evaluation
│
├── Notebook_Deep Learning Approach for IDS.ipynb
│ └─ CNN, BiLSTM, Transformer, Hybrid architectures
│
└── README.md

---

## ⚙️ Technologies
- Python  
- Jupyter Notebook  
- Scikit-learn  
- XGBoost  
- LightGBM  
- TensorFlow / Keras  
- NumPy, Pandas, Matplotlib, Seaborn  

---

## ▶️ How to Run
```bash
git clone https://github.com/zinebadammiche/Hybrid-ML-DL-IDS-for-IoT-CIC-IoT-2025-.git
cd Hybrid-ML-DL-IDS-for-IoT-CIC-IoT-2025-
jupyter notebook


## 📂 Repository Structure
