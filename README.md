# 🌱 Weed Detection Using Deep Learning  
### Classification of Broadleaf, Grass, Soil & Soybean Classes

This project implements **three deep learning models**—a Tuned CNN, EfficientNetB0, and MobileNetV2—for automated weed detection in soybean crop images.  
The goal is to classify cropped RGB image patches into one of four categories:

- **Broadleaf weed**
- **Grass weed**
- **Soil / Background**
- **Soybean crop**

**Dataset used:** *Weed Detection in Soybean Crops (Kaggle)*

---

## 🚀 Project Features

### ✔ Data Preprocessing
- Images resized to **32 × 32 RGB**
- Normalized pixel values  
- Label encoding + one-hot encoding  
- Train–test split with **stratified sampling**
- `tf.data` pipeline for faster training  

---

## ✔ Deep Learning Models Implemented

### **1. Tuned CNN (Keras Tuner)**
Hyperparameters tuned:
- Filters  
- Kernel sizes  
- Dense units  
- Dropout rate  

**Highest Accuracy:** **95.63%**

---

### **2. EfficientNetB0**
- Trained from scratch  
- Custom dense classification head  
**Accuracy:** *81.77%*

---

### **3. MobileNetV2**
- Lightweight architecture  
- Custom classification head  
**Accuracy:** *48.10%*

---

## 📊 Results Summary

| Model           | Accuracy | Loss   |
|----------------|----------|--------|
| **Tuned CNN**  | **0.9563** | 0.1354 |
| EfficientNetB0 | 0.8178   | 0.5276 |
| MobileNetV2    | 0.4810   | 1.9914 |

---

## 📌 Why Tuned CNN Performs Best
- Architecture optimized for small **32×32** images  
- Hyperparameter tuning significantly reduces overfitting  
- Achieved **AUC = 0.994**, indicating near-perfect class separability  

---

## 📚 Confusion Matrices
Visual confusion matrices for all models are included in the project report:

**Report_WeedProtection.pdf**

---

## 🧠 Model Workflow

1. Load Dataset  
2. Preprocess Images  
3. Build Models (CNN, EfficientNetB0, MobileNetV2)  
4. Train on **80%** of the data  
5. Evaluate on **20%** test split  
6. Plot accuracy, loss, confusion matrices, ROC-AUC curves  

---

---

## 🛠 Technologies & Libraries

- TensorFlow / Keras  
- Keras Tuner  
- Scikit-learn  
- NumPy  
- Matplotlib & Seaborn  

---

## 📈 ROC-AUC Highlights  
(From ROC curves in Report_WeedProtection.pdf)

- **CNN:** 0.994  
- **EfficientNetB0:** 0.950  
- **MobileNetV2:** 0.694  

---

## 📚 References  
Detailed references are available in **Report_WeedProtection.pdf (Page 17)**.

---

## 🙌 Authors

- **Rashi Toteja**  
- **Saksham Kumar Jha**  
- **Diya**  
- **Kshitiz Arora**  
- **Shambhavi Rajshree**


