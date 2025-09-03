# Detection of Breast Cancer  

This project builds a **predictive machine learning model** to classify **breast tissue samples** as either **benign** or **malignant** using the **Wisconsin Breast Cancer Diagnostic dataset**.  

By analyzing features extracted from **cell nuclei** in breast tissue samples, the model aims to assist medical professionals in **early diagnosis of breast cancer** and in identifying cases that require further investigation or treatment.  

---

## 🎯 Project Objective  

- Develop a classification model to distinguish between **benign (2)** and **malignant (4)** tumors.  
- Explore relationships between **cell nuclei features** and cancer outcomes.  
- Support medical decision-making by reducing unnecessary biopsies.  

---

## 📂 Dataset  

- **Name**: Wisconsin Breast Cancer Diagnostic Dataset  
- **Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/breast-cancer-wisconsin.data)  
- **Instances**: 699 (collected between Jan 1989 – Nov 1991)  
- **Attributes**: 11 total (10 features + 1 target)  

### Features  

| Attribute                  | Range | Description |
|----------------------------|-------|-------------|
| Sample code number         | ID    | Unique identifier |
| Clump Thickness            | 1–10  | Thickness of clump |
| Uniformity of Cell Size    | 1–10  | Cell size uniformity |
| Uniformity of Cell Shape   | 1–10  | Cell shape uniformity |
| Marginal Adhesion          | 1–10  | Cell adhesion |
| Single Epithelial Cell Size| 1–10  | Size of epithelial cells |
| Bare Nuclei                | 1–10  | Nuclei visibility |
| Bland Chromatin            | 1–10  | Chromatin texture |
| Normal Nucleoli            | 1–10  | Presence of nucleoli |
| Mitoses                    | 1–10  | Rate of mitosis |
| **Class (Target)**         | {2,4} | 2 = Benign, 4 = Malignant |

---

## 🧭 Workflow  

### 1. Data Preprocessing  
- Handle missing values (e.g., in **Bare Nuclei**)  
- Convert categorical target variable into **binary labels (0 = benign, 1 = malignant)**  
- Normalize feature values for consistency  

### 2. Exploratory Data Analysis (EDA)  
- Distribution of benign vs malignant cases  
- Feature correlations with diagnosis  
- Boxplots and histograms of feature values  

### 3. Modeling  
- Machine learning models for binary classification (examples):  
  - Logistic Regression  
  - Support Vector Machine (SVM)  
  - Random Forest  
  - K-Nearest Neighbors (KNN)  
- Cross-validation to ensure robustness  

### 4. Evaluation  
- Metrics: Accuracy, Precision, Recall, F1-score, ROC-AUC  
- Confusion matrix to evaluate false positives/negatives  

---

## 📂 Repository Structure  

- `data/` – Wisconsin Breast Cancer dataset  
- `notebooks/` – Jupyter notebooks for preprocessing, EDA, and modeling  
- `models/` – Trained machine learning models  
- `results/` – Evaluation metrics and plots  

---

## 🚀 How to Run  

1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/breast-cancer-detection.git
   cd breast-cancer-detection
