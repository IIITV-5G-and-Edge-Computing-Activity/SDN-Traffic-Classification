# 🚀 5G Project: SDN Traffic Classification

## 🌟 Group Number: Gr37EC431

### Group Team Members:
- **AYUSH KUMAR AGARWAL** (202151037)  
- **PARMAR HET** (202151103)  
- **PATEL SHUBH UMESHKUMAR** (202151111)  
- **POPAT RITIK MANISH** (202151114)  
- **RAJ JIGNESHKUMAR SHAH** (202151127)  
- **JENNY KAMLESHBHAI BHUT** (202152314)  

---

## 📖 Overview
This project leverages **Software-Defined Networking (SDN)** for traffic classification in 5G networks using **supervised learning** and **unsupervised learning** techniques. By analyzing traffic patterns and characteristics, it aims to enhance:  
- 🛠 **Network Efficiency**  
- 🔒 **Security**  
- ⚡ **Resource Allocation**



## Installation

Follow these steps to set up and run the project locally:

### 1. Clone the Repository
First, clone the repository to your local machine:
```bash
git clone https://github.com/SDN-Traffic-Classification](https://github.com/IIITV-5G-and-Edge-Computing-Activity/SDN-Traffic-Classification.git

cd SDN-Traffic-Classification
```
### 2. Install dependencies:
```bash

pip install -r requirements.txt
```

## 🔍 Methodology

### **🧑‍🏫 A. Supervised Learning with Logistic Regression**
1. **🧹 Dataset Preparation:**
   - Cleaned and encoded the data.  
   - Split into features (independent variables) and labels (dependent variables).  
   - Used `train_test_split` for a 70-30 split between training and testing data.

2. **⚙️ Model Initialization:**
   - Chose Logistic Regression for its simplicity and effectiveness in multiclass problems.  
   - Configured parameters:
     - Penalty: L2 regularization.  
     - Solver: Liblinear.

3. **📊 Training Process:**
   - Trained the model using the **one-vs-rest** approach to handle multiclass classification.  

4. **🔄 Cross-Validation:**
   - Performed **5-fold cross-validation** for robust evaluation.  
   - Analyzed metrics across folds to detect overfitting or underfitting.  

5. **📈 Evaluation Metrics:**
   - Evaluated using Accuracy, Precision, Recall, and F1 Score for each traffic class.  
   - Generated a confusion matrix to highlight misclassifications.  

---

### **🤖 B. Unsupervised Learning with K-Means Clustering**
1. **📏 Dataset Standardization:**
   - Used `StandardScaler` to standardize feature values.  

2. **🛠 Clustering Initialization:**
   - Explored multiple cluster numbers (`k`) to uncover the data structure.  
   - Used `random_state` for reproducibility.  

3. **📉 Optimal Clusters:**
   - Applied the **Elbow Method** to find the ideal `k`.  

4. **🔗 Cluster Formation:**
   - Grouped data into clusters and assigned labels.  

5. **✔️ Cluster Validation:**
   - Evaluated clustering with the **Silhouette Score**.  

6. **🌈 Visualization:**
   - Reduced dimensions using **Principal Component Analysis (PCA)** for 2D scatter plots.  

---

## 📊 Results and Analysis

### **✅ Supervised Learning with Logistic Regression**
- **Confusion Matrix Highlights:**  
  - 🟢 **Ping Traffic:** 569 correctly classified.  
  - 🟢 **Voice Traffic:** 885 correctly classified (highest accuracy).  
  - 🟢 **DNS Traffic:** 574 correct, minor confusion observed.  
  - 🟢 **Telnet Traffic:** 571 correctly identified samples.  
  - **🟡 Misclassifications:** Minimal errors, primarily between closely related traffic types (e.g., Telnet and DNS).

### **📊 Unsupervised Learning with K-Means**
- Optimal clusters determined using the **Elbow Method**.  
- **Silhouette Scores** indicated strong cluster separation.  
- **PCA Visualization:** Clearly illustrated data separation.

---

## 🛠 Technologies and Tools Used
- 🐍 **Python**: Core programming language.  
- 📚 **Libraries**: NumPy, Pandas, Scikit-learn, Matplotlib, Seaborn, TensorFlow.  
- 🖧 **SDN Simulation**: Mininet and OpenFlow.  
- 🔍 **Dimensionality Reduction**: PCA.

---
