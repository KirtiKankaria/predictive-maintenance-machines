# Predictive Maintenance for Machines

## 📌 Overview
This project analyzes sensor data from manufacturing machines to predict potential failures.  
The goal is to leverage machine learning models to forecast when a machine is likely to fail,  
helping prevent costly downtime and optimize maintenance operations.  

The analysis compares **Logistic Regression, Random Forest, and Gradient Boosting Models (GBM)**,  
as well as Recurrent Neural Networks (RNN). It evaluates performance based on **accuracy, precision,  
recall, F1-score, and ROC-AUC**.  

An additional dashboard is developed for visualizing machine health status and maintenance schedules.  

---

## 🛠️ Tools & Technologies
- Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, TensorFlow/Keras)
- Machine Learning Models: Logistic Regression, Random Forest, Gradient Boosting, RNN
- Data Source: [UCI AI4I 2020 Predictive Maintenance Dataset](https://archive.ics.uci.edu/dataset/601/ai4i+2020+predictive+maintenance+dataset)
- Streamlit (for potential interactive deployment)

---

## 📊 Key Results
- **Logistic Regression:**  
  - Accuracy: 97% | ROC AUC: 0.63  
  - Weak recall for failures (0.26) → not effective for minority class  

- **Random Forest:**  
  - Accuracy: 98% | ROC AUC: 0.79  
  - Balanced performance across classes | F1-score: 0.69 for failures  

- **Gradient Boosting (Neural Network):**  
  - Accuracy: 98% | ROC AUC: 0.82  
  - Best recall for failures (0.66) and strongest balance between precision and recall  

📌 **Conclusion:**  
Gradient Boosting offers the best overall balance, but Random Forest is recommended for production due to robustness.  

---

## 📂 Repository Structure
- `notebooks/` – Jupyter/Colab notebooks with full model training & evaluation  
- `report/` – Project PDF and documentation
- `images/` – Visualizations (EDA plots, model performance, training curves)  

---

## 🔗 Links
- 📄 [Project Report (PDF)](https://github.com/KirtiKankaria/predictive-maintenance-machines/blob/main/Predictive_Maintenance_for_Machines.ipynb%20-%20Colab.pdf)  
- 📊 [Dataset](https://archive.ics.uci.edu/dataset/601/ai4i+2020+predictive+maintenance+dataset)  

---

## 🚀 Future Work
- Deploy interactive predictive maintenance dashboard with Streamlit  
- Optimize ensemble methods with hyperparameter tuning  
- Expand dataset with real-world IoT sensor data for production testing  
