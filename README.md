# Hybrid Machine and Deep Learning Framework for Real-Time IoT Intrusion Detection  
### Comprehensive Evaluation on CIC-IoT-2025

---

## 📄 Associated Paper
**Title:** *Real-Time IoT Intrusion Detection Using a Hybrid Machine and Deep Learning Framework: Comprehensive Evaluation on CIC-IoT-2025*

**Authors:**  
- **Zineb ADAMMICHE**, National Institute of Posts and Telecommunications (INPT), Rabat, Morocco  
- **Prof. Iyad LAHSEN-CHERIF**, National Institute of Posts and Telecommunications (INPT), Rabat, Morocco  

📧 adammiche.zineb@master.inpt.ac.ma  
📧 iyad.lahsencherif@inpt.ac.ma  

---

## 📌 Abstract / Overview
This repository contains the **implementation notebooks** supporting the research paper on **real-time intrusion detection for IoT networks** using a **hybrid Machine Learning (ML) and Deep Learning (DL) framework**.

The study provides a **fair, unified, and reproducible comparison** between:
- Classical **Machine Learning models**
- Advanced **Deep Learning architectures**

Experiments are conducted on the **CIC-IoT-2025 dataset** under **identical preprocessing, feature engineering, and evaluation protocols**, considering:
- **Binary classification** (Benign vs. Attack)
- **Multiclass classification** (8 attack categories)

---

## 🎯 Research Objectives
- Perform a **head-to-head comparison** of ML and DL approaches for IoT IDS  
- Analyze the **accuracy–efficiency trade-off** in resource-constrained IoT environments  
- Evaluate **binary and multiclass classification** scenarios  
- Investigate **manual feature engineering vs. automatic feature learning**  
- Provide **practical deployment guidelines** for real-world IoT systems  

---

## 🚀 Main Contributions
- Unified experimental pipeline for ML and DL models  
- Correlation-based feature selection (**71 → 48 features**)  
- Evaluation of **6 ML models** and **4 DL architectures**  
- Detailed per-class analysis across **8 attack categories**  
- Computational efficiency benchmarking (training time, inference latency, memory usage)  
- Deployment-oriented recommendations (edge, cloud, critical infrastructure)  

---

## 📊 Dataset Description
- **Dataset:** CIC-IoT-2025  
- **Provider:** Canadian Institute for Cybersecurity (UNB)  
- **Records:** 685,671 network flows  
- **Features:** 71 numerical flow-based features  

**Classes:**
- **Binary:** Benign / Attack  
- **Multiclass (8):** Benign, BruteForce, DDoS, DoS, Malware, MITM, Reconnaissance, Web  

⚠️ Dataset not included due to size constraints.  
📎 Available via the official UNB website.

---

## 🧠 Methodology Overview

### 1️⃣ Data Preprocessing
- Removal of NaN and infinite values  
- Feature standardization (StandardScaler)  
- Class imbalance analysis  
- Correlation-based feature selection  
- PCA-based dimensionality reduction (ML track)  

### 2️⃣ Machine Learning Track
**Algorithms:**
- Random Forest  
- XGBoost  
- LightGBM  
- Ensemble models (RF + XGB + LGB)  

**Advantages:**
- High accuracy with low computational cost  
- Strong detection of rare attack classes  
- High interpretability  

### 3️⃣ Deep Learning Track
**Architectures:**
- CNN  
- CNN + BiLSTM  
- Transformer  
- Hybrid CNN + BiLSTM + Transformer  

**Advantages:**
- Automatic feature learning  
- Temporal and sequential pattern modeling  

---

## 🧪 Experimental Scenarios & Metrics
**Scenarios:**
- Binary classification  
- Multiclass classification (8 classes)  

**Metrics:**
- Accuracy  
- Precision  
- Recall  
- F1-score  
- ROC-AUC  
- Training time  
- Inference latency  
- Memory usage  

---

## 📈 Key Results (From the Paper)

### 🔹 Best Machine Learning Models
- **Binary:** XGBoost + LightGBM  
  - Accuracy: **96%**  
  - ROC-AUC: **0.9844**  
- **Multiclass:** LightGBM  
  - Accuracy: **96%**  
  - Strong performance on rare attacks  

### 🔹 Best Deep Learning Models
- **Binary:** Hybrid CNN + BiLSTM + Transformer  
  - Accuracy: **96%**  
- **Multiclass:** CNN + BiLSTM  
  - Accuracy: **94.4%**  

### 🔹 Computational Efficiency
| Approach | Training Time | Inference Latency | Memory Usage |
|--------|---------------|------------------|--------------|
| ML     | 2–4 min       | 1.8–3.2 ms       | 52–145 MB    |
| DL     | 9–19 min      | 8.5–15 ms        | 12–35 MB     |

---

## 📂 Repository Structure
```text
Hybrid-ML-DL-IDS-for-IoT-CIC-IoT-2025/
│
├── Notebook_Machine_Learning_Approach_for_IDS.ipynb
│   └─ Classical ML models and ensemble evaluation
│
├── Notebook_Deep_Learning_Approach_for_IDS.ipynb
│   └─ CNN, BiLSTM, Transformer, hybrid architectures
│
└── README.md

