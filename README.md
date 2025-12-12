# Breast Cancer Diagnosis Prediction  
### Using K-Nearest Neighbors (KNN) and K-Means Clustering  


## Dataset
The dataset contains numeric features extracted from images of breast tumors.  
It includes measurements such as radius, texture, perimeter, smoothness, etc.

---

## Steps Performed in This Project

### **1. Load Dataset**
Used pandas to read the CSV file.

### **2. Remove Unnecessary Columns**
Dropped:
- `id`
- `Unnamed: 32`

### **3. Encode the Target Column**
Mapped:
- **M → 1 (Malignant)**
- **B → 0 (Benign)**

### **4. Normalize Features**
Applied **Min-Max Scaling** to all feature columns except the target.

### **5. Split the Dataset**
Used `train_test_split()`:
- Training data → 80%
- Testing data → 20%
- `random_state = 42`

### **6. K-Means Clustering (k = 2)**
Performed unsupervised clustering to observe natural grouping.  
Created a crosstab to compare **cluster labels vs actual diagnosis**.

### **7. Train KNN Model (k = 5)**
KNN classifier was trained using normalized training data.

### **8. Evaluate Model**
Calculated performance using:
- Accuracy
- Precision
- Recall
- F1-score

These metrics show how well the model predicts tumor types.
Accuracy : 0.95
Precision : 0.94
Recall : 0.96
F1-score : 0.95

---

##  Libraries Used
- pandas  
- numpy  
- sklearn  
- matplotlib  
- seaborn  

---

##  Notebook Contents
The colab Notebook includes:
- Data preprocessing  
- Normalization  
- Clustering  
- KNN training  
- Evaluation  
- Visualizations  


---


## Conclusion
This project successfully demonstrates how:
- **K-Means** can discover natural clusters  
- **KNN** can accurately classify cancer diagnoses  

Both methods help in understanding and predicting tumor types using medical data.




