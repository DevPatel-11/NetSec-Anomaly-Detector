# NetSec Anomaly Detector

NetSec Anomaly Detector is a machine learning-driven system designed to detect anomalies and categorize different types of attacks in network traffic. Using the UNSW-NB15 dataset, this project evaluates various unsupervised and supervised models for effective intrusion detection and classification.

---

## 🧠 Models Implemented

### Unsupervised Learning
- **K-Means Clustering**
- **Gaussian Mixture Models (GMM)**
- **Self-Organizing Maps (SOM)**

### Supervised Learning
- **Random Forest Classifier**
- **XGBoost Classifier**
- **Support Vector Classifier (SVC)**
- **K-Nearest Neighbors Classifier (KNN)**

These models support **multiclass detection**, enabling classification of multiple attack categories as well as benign traffic.

---

## 📊 Performance Metrics

Model evaluation was performed using:
- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**
- **Confusion Matrix**

The metrics demonstrate the effectiveness of the classifiers, particularly in complex multiclass scenarios involving various attack types.

---

## 🧰 Tech Stack

- **Languages & Libraries**: Python, Pandas, NumPy, Matplotlib, Seaborn
- **Machine Learning**: Scikit-learn, XGBoost, Joblib
- **Development Tools**: Jupyter Notebook
- **Dataset**: UNSW-NB15
- **Monitoring Tool**: Zeek (planned integration)

---

## 🚀 Future Enhancements

Planned and suggested improvements for the system include:

1. **Real-Time Zeek Integration**  
   Connect the trained models with Zeek to monitor live network traffic and classify anomalies on the fly.

2. **Web-Based Security Dashboard**  
   Build an intuitive dashboard for real-time visualization of traffic patterns, alerts, and attack statistics.

3. **Cloud Deployment**  
   Deploy the solution to cloud platforms (e.g., AWS, GCP, Azure) to enable scalable, distributed network monitoring.

4. **Hyperparameter Optimization**  
   Use automated tuning techniques (e.g., GridSearchCV, Optuna) to improve model performance.

5. **Ensemble Learning**  
   Combine multiple models to increase detection robustness and reduce false positives.

6. **Threat Intelligence Integration**  
   Leverage external threat intelligence APIs to enrich detection and provide contextual threat analysis.

7. **SIEM Integration**  
   Connect the system with Security Information and Event Management (SIEM) platforms to support full-stack threat management.

