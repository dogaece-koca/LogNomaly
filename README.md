# LogNomaly: Hybrid Log Anomaly Detection with Machine Learning

[cite_start]LogNomaly is an advanced, multi-layered system designed to detect operational anomalies and cyber threats in modern software logs[cite: 4, 33]. As systems grow more complex, manual tracing of logs becomes impossible; [cite_start]LogNomaly addresses this by providing an automated, intelligent analysis pipeline[cite: 35, 36, 60].

## 🏗 The Hybrid Architecture
[cite_start]Unlike traditional systems that rely on a single detection method, LogNomaly utilizes a three-layer hybrid architecture to balance speed and accuracy[cite: 88, 92]:

1. [cite_start]**Layer 1 - Rule-Based Filtering:** Rapidly detects known attack patterns (e.g., brute force) to reduce computational overhead[cite: 93, 108].
2. [cite_start]**Layer 2 - Unsupervised Detection (Isolation Forest):** Identifies unknown "zero-day" anomalies by flagging outliers in behavioral data[cite: 95, 109].
3. [cite_start]**Layer 3 - Supervised Classification (Random Forest):** Categorizes detected anomalies (e.g., SQL Injection) and assigns a probabilistic **Risk Score** (0.0 - 1.0)[cite: 96, 97, 110].

---

## 🚀 Key Innovations
* [cite_start]**Actionable Risk Scoring:** Moves beyond binary "Normal/Abnormal" labels by providing a specific risk priority (Low, Medium, High) and threat classification[cite: 99, 281].
* [cite_start]**Explainable AI (XAI):** Integrates **SHAP (Shapley Additive Explanations)** to visualize which features most influenced the model's decision, solving the "black box" problem of traditional ML[cite: 276, 442, 446].
* [cite_start]**Integrated Web Interface:** Features a real-time interactive dashboard for monitoring system health and reviewing incident reports[cite: 112, 673, 674].

---

## 📐 System Design & Modeling
[cite_start]The project is built on rigorous Software Engineering principles, featuring a modular and scalable design[cite: 130, 598]:

* [cite_start]**Architectural View:** Decoupled frontend and backend using a REST API architecture[cite: 519, 528].
* [cite_start]**Design Patterns:** Utilizes the **Strategy Pattern** for switching ML algorithms and the **Facade Pattern** to simplify the analysis pipeline for the interface[cite: 669, 671].

---

## 🛠 Technology Stack
* [cite_start]**Machine Learning Engine:** Python (Pandas, NumPy, Scikit-learn, SHAP)[cite: 114, 124, 450].
* [cite_start]**Backend API:** Flask / FastAPI[cite: 115, 124].
* [cite_start]**Web Frontend:** C# and ASP.NET Core MVC[cite: 113, 125].
* [cite_start]**Deployment:** Containerized with **Docker** for cross-platform interoperability[cite: 127, 504].

---

## 📂 Documentation
[cite_start]The full technical design report, including detailed UML diagrams (Class, Sequence, Activity, and Deployment), is available in the repository as a PDF[cite: 25, 28].
