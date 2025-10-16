# cns_previlege_attack_cs22b1036

# AI-Based Real-Time Threat Analysis for Networks

## 📚 Project Overview
This project implements an AI-based real-time detection system for **Privilege Escalation Attempts** on honeypot-monitored networks. Using machine learning, the system analyzes process and system event logs in real time, identifying suspicious activity that could indicate unauthorized privilege escalation or malicious intrusion.

---

## 🚀 Features

- **Attack Detection Focus:**  
  Detects suspicious process activity, with a focus on identifying possible privilege escalation attempts.
- **Hybrid AI Approach:**  
  - Supervised learning (Random Forest)
  - Unsupervised anomaly detection (Isolation Forest)
- **Real-World Data:**  
  Based on authentic honeypot log data (over 760,000 records, 1,269 suspicious events)
- **End-to-End Pipeline:**  
  From data preprocessing and exploratory analysis to model evaluation and deployment-ready demo code.
- **Visualization:**  
  Classification metrics, confusion matrix, ROC curve, and process/event distributions.

---

## 📊 Dataset Description

- **Source:** Honeypot Collected Process Logs  
- **Rows:** 763,144  
- **Columns:** 16  
- **Attack Samples (Suspicious):** 1,269  
- **Normal Samples:** 761,875  
- **Attack Label:** Defined by `sus = 1` (suspicious event detected by honeypot system)

---

## 🧑‍💻 Installation & Usage

1. **Clone this repository and set up a virtual environment:**
    ```
    git clone <repo_url>
    cd <repo_folder>
    python3 -m venv myenv
    source myenv/bin/activate
    pip install -r requirements.txt
    ```
2. **Run the Jupyter notebook for full experimentation & demo:**
    ```
    jupyter notebook cnsproject.ipynb
    ```
    Make sure the dataset CSV is available in the working directory.

3. **Key files:**
    - `cnsproject.ipynb` — full code, analysis, and model training
    - `requirements.txt` — all dependencies

---

## 📈 Results

- **Random Forest:** Achieved high precision/recall for normal events; moderate recall for privilege escalation attempts.
- **Isolation Forest:** Detected a portion of anomalies, but with a higher false positive rate.
- **Visualization:** See notebook for plots (confusion, class balance, ROC).

---

## 📒 Deliverables

- Data preprocessing and cleaning
- Exploratory data analysis (EDA)
- Supervised/unsupervised modeling
- Evaluation metrics and visuals
- Simulated real-time detection demo

---

## 📝 License
Distributed for academic/non-commercial use only.

---

## 🤝 Credits
Developed by [Your Name].  
(Data, inspiration: public honeypot datasets and academic IDS references.)

---

## 🔗 Links
- [Project Report/Document](link_to_document)
- [Dataset Source](link_to_dataset)
