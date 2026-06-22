# Adult_Income_Predictive_Modeling 
End-to-End Predictive Modeling Pipeline for Socio-Economic Insights

## Project Overview & Strategic Impact
This project delivers a robust, binary classification pipeline designed to predict annual individual income (>50K vs. <=50K) using U.S. Census demographic and employment data. 

From a product management standpoint, this model serves as a foundational predictive framework for market segmentation, targeted consumer financing products, and economic resource allocation. The focus of this initiative was managing the end-to-end Machine Learning Lifecycle (MLLC) spanning data quality governance, pipeline optimization, and stakeholder-aligned model validation.

---

## AI Product Lifecycle & Methodology

### 1. Data Governance & Preprocessing
Managed data quality constraints by identifying and resolving structural anomalies in 48,000 records.
* **Data Quality Assurance:** Replaced missing values (`?`) with robust statistical imputations (mode for categorical, mean/median for numerical).
* **Feature Engineering Execution:** Orchestrated a scalable encoding strategy utilizing One-Hot Encoding for categorical features (`workclass`, `occupation`) and Label Encoding for binary targets.
* **Data Normalization:** Implemented `MinMaxScaler` on key numerical drivers (`age`, `capital gain/loss`) to prevent feature dominance and ensure uniform gradient descent during training.

### 2. Validation & Quality Gates
To ensure model generalizability and prevent data leakage, a strict **70/15/15 split** strategy was defined:
* **Training Set (70%):** Core model calibration.
* **Validation Set (15%):** Hyperparameter tuning and architecture optimization.
* **Testing Set (15%):** Final unbiased performance benchmarking before deployment scoping.

### 3. Model Evaluation & Benchmark Metrics
*Project performance was evaluated using standard industry KPIs to ensure alignment with business risk tolerances (balancing Precision vs. Recall to manage false positives in income targeting).*
* **Key Metrics Tracked:** ROC-AUC, Precision, Recall, and F1-Score.
* **Advanced Ensembling:** Evaluated advanced architectural configurations, including **Bayesian Stacking**, to optimize ensemble learning weights for maximum classification accuracy.

---

## Repository Structure
* `UnnatiShakya_CleanDataset_*.csv` — Managed and cleaned production-ready dataset.
* `UnnatiShakya_FinalExam_14406_Notebook.ipynb` — Core technical execution notebook.
* `UnnatiShakya_ModelComparison_*.pdf` — Comparative benchmarking analysis for executive leadership.
* `UnnatiShakya_FinalReport_*.pdf` — Comprehensive technical and strategic documentation.
