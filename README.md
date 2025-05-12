# 🔐 DDoS Attack Detection using Machine Learning

This project presents a comparative analysis of multiple machine learning models for detecting DDoS (Distributed Denial of Service) attacks, using the CICDDoS2019 dataset. The objective is to evaluate each model's ability to accurately classify normal and malicious network traffic.

---

## 📊 Models Evaluated

We trained and evaluated the following models:

- **CNN** – Convolutional Neural Network  
- **DNN** – Deep Neural Network  
- **GRU** – Gated Recurrent Unit  
- **KNN** – K-Nearest Neighbors  
- **LR** – Logistic Regression  
- **LSTM** – Long Short-Term Memory  

---

## 📊 Evaluation Metrics

Each model was assessed using the following metrics:

- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**
- **Normal Detection Rate**
- **Attack Detection Rate**
- **ROC AUC**

---

## 📁 Dataset

- **Source**: [CICDDoS2019](https://www.unb.ca/cic/datasets/ddos-2019.html) — provided by the Canadian Institute for Cybersecurity  
- **Preprocessing**:
  - Removed missing values and redundant features
  - Encoded categorical labels
  - Scaled features using StandardScaler
  - Balanced dataset if required (e.g., using undersampling or oversampling)

---

## 📊 Visualizations

- 🧠 **Model & Hyperparameter Grid**  
  For each model, visualize the relationship between key hyperparameters and performance  
  *(e.g., accuracy vs. number of layers, batch size, units, etc.)*

- 📈 **Performance Comparison Charts**  
  Compare **Accuracy**, **Precision**, **Recall**, **F1-Score**, and **Average** across all models.

- 📉 **Detection Rate Chart**  
  Visualize the difference between **Normal** and **Attack Detection Rates**.

- 🏆 **Best Model per Grid**  
  For each model, select the best-performing configuration and plot its  
  **ROC Curve** and **Confusion Matrix**.

---

## 📌 Conclusion 
Through extensive evaluation on the CICDDoS2019 dataset, all six models demonstrated high performance in detecting DDoS attacks. **DNN** shows the best overall result (0.999498), followed by **CNN** and **GRU**. **LSTM** has the lowest accuracy but still performs well (0.998328). All models detect attacks and normal behavior effectively.
