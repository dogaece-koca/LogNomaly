LogNomaly: Hybrid Log Anomaly Detection with Machine Learning
LogNomaly is an advanced, multi-layered system designed to detect operational anomalies and cyber threats in modern software logs. As systems grow more complex, manual tracing of logs becomes impossible; LogNomaly addresses this by providing an automated, intelligent analysis pipeline.




The Hybrid Architecture
Unlike traditional systems that rely on a single detection method, LogNomaly utilizes a three-layer hybrid architecture to balance speed and accuracy:



Layer 1 - Rule-Based Filtering: Rapidly detects known attack patterns (e.g., brute force) to reduce computational overhead.


Layer 2 - Unsupervised Detection (Isolation Forest): Identifies unknown "zero-day" anomalies by flagging outliers in behavioral data.



Layer 3 - Supervised Classification (Random Forest): Categorizes detected anomalies (e.g., SQL Injection) and assigns a probabilistic Risk Score (0.0 - 1.0).

Key Innovations

Actionable Risk Scoring: Moves beyond binary "Normal/Abnormal" labels by providing a specific risk priority (Low, Medium, High) and threat classification.



Explainable AI (XAI): Integrates SHAP (Shapley Additive Explanations) to visualize which features (e.g., source IP, time) most influenced the model's decision, solving the "black box" problem of traditional ML.




Integrated Web Interface: Features a real-time interactive dashboard for monitoring system health and reviewing incident reports.


System Design & Modeling
The project is built on rigorous Software Engineering principles, featuring a modular and scalable design:



Architectural View: Decoupled frontend and backend using a REST API architecture.



Design Patterns: Utilizes the Strategy Pattern for switching ML algorithms and the Facade Pattern to simplify the analysis pipeline for the interface.


Technology Stack

Machine Learning Engine: Python (Pandas, NumPy, Scikit-learn, SHAP).




Backend API: Flask / FastAPI.


Web Frontend: C# and ASP.NET Core MVC.



Deployment: Containerized with Docker for cross-platform interoperability.
