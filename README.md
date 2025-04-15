# 🚀 NetSec Anomaly Detector

**NetSec Anomaly Detector** is a cybersecurity project that leverages machine learning to detect anomalies and categorize attacks in network traffic. With the growing frequency of cyber threats, early detection of suspicious behavior is vital to protect sensitive infrastructure.

This project explores both **unsupervised** and **supervised** machine learning techniques on benchmark datasets like **UNSW-NB15**, ultimately selecting **Random Forest** due to its superior classification performance.

---

## 🔥 Features

- ✅ **Data Preprocessing**  
  - Cleaning, encoding, and normalization of network traffic logs.

- ✅ **Model Evaluation & Selection**  
  - Models tested:
    - **Unsupervised**:  
      - **KMeans** – Clustering normal vs. anomalous data  
      - **GMM (Gaussian Mixture Model)** – Probabilistic clustering  
      - **MiniSom (Self-Organizing Maps)** – Neural network-based unsupervised learning  

    - **Supervised**:  
      - **Random Forest Classifier**  
      - **XGBoost Classifier**  
      - **SVC (Support Vector Classifier)**  
      - **KNN Classifier**

  - Final model: **Random Forest**, based on highest **F1-scores** (micro, macro, weighted)

- ✅ **Multiclass Attack Detection**  
  - Predicts the `attack_cat` column to identify the type of intrusion (e.g., DoS, Reconnaissance, etc.)

- ✅ **Performance Metrics**  
  - Evaluation using precision, recall, F1-score (micro, macro, weighted), ROC-AUC, and confusion matrix.

- ✅ **Real-Time Anomaly Simulation**  
  - Captures live packets using Python & Scapy and flags anomalies in real-time.

---

## 🔬 Datasets Used

- [UNSW-NB15](https://www.kaggle.com/datasets/mrwellsdavid/unsw-nb15)

---

## 📌 Tech Stack

- **Languages/Tools**:  
  - **Python**, **Zeek**

- **Libraries & Frameworks**:  
  - 🧠 Machine Learning: `Scikit-learn`, `XGBoost`, `MiniSom`, `SciPy`  
  - 📊 Data Processing: `Pandas`, `NumPy`  
  - 📈 Visualization: `Matplotlib`, `Seaborn`  
  - 🌐 Networking: `Scapy`, `Zeek`  
  - (Planned) Dashboard: `Flask` or `Streamlit` for web-based monitoring

---

## 📈 Model Performance

After comparing multiple models, **Random Forest** was selected for its high classification accuracy across:

- ✅ Micro F1-Score  
- ✅ Macro F1-Score  
- ✅ Weighted F1-Score  

This model demonstrated strong generalization to unseen network traffic and consistently outperformed others in multiclass classification tasks.

---

## 🔮 Future Enhancements

- 🤖 **Real-Time Prediction Pipeline**  
  Integrate the trained ML model with **Zeek** to continuously monitor live network traffic and classify anomalies in real-time.

- 🌐 **Web-Based Security Dashboard**  
  Build an intuitive web dashboard to:
  - Visualize detected anomalies and attack types
  - View real-time alerts from Zeek-integrated predictions
  - Track daily/weekly security trends and traffic stats

- ☁️ **Cloud-Ready Deployment**  
  Dockerize the solution and deploy it to the cloud (e.g., AWS, Azure) for scalable and continuous network monitoring.

---


