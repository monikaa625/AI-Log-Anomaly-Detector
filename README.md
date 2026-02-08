# AI-Log-Anomaly-Detector
An unsupervised machine learning system using Isolation Forest to detect cyber threats in network logs (UNSW-NB15 dataset).
AI-Powered Log Anomaly Detector
🛡️ Project Overview
This project implements an unsupervised machine learning system designed to detect cyber threats within network logs. Unlike traditional signature-based systems, this model utilizes the Isolation Forest algorithm to identify "Zero-Day" attacks and anomalous behaviors without requiring prior labeling of attack signatures.

By focusing on anomalies (outliers), the system can detect sophisticated threats like DDoS, Backdoors, and Fuzzers that deviate from normal network patterns.

📊 Core Features
Unsupervised Learning: Employs Isolation Forest to detect unknown threats by isolating outliers in high-dimensional data.

Feature Engineering: Processes raw network telemetry (Protocols, Services, States) into numerical vectors using Label Encoding.

Threat Scoring: Calculates a decision score for every log entry; negative scores indicate a high probability of malicious activity.

Visual Analytics: Generates a real-time "Threat Detection Dashboard" to visualize the separation between normal traffic and anomalies.

🛠️ Tech Stack
Language: Python 3.x

Libraries: scikit-learn, pandas, numpy, matplotlib

Dataset: UNSW-NB15 (A modern benchmark for network intrusion detection).

🚀 Installation & Usage
Clone the repository:

Bash
git clone https://github.com/YOUR_USERNAME/AI-Log-Anomaly-Detector.git
Install dependencies:

Bash
pip install -r requirements.txt
Run the detection model:
Open the .ipynb file in Google Colab or Jupyter Notebook and execute the cells to train the model and generate the threat graph.

📈 Results
The model successfully separates normal traffic (clustered "Inliers") from potential threats (isolated "Outliers").

Blue Points: Normal system activity.

Red Points: Detected anomalies/potential intrusions.

X-Axis: Log Entry Index.

Y-Axis: Threat Level (Scores below 0 are categorized as critical threats).

📝 Future Enhancements
Integration with a SQL database for historical incident logging and forensic analysis.

Transitioning from batch processing to a real-time streaming pipeline using Flask or FastAPI.

Implementing Feature Importance analysis to explain why a specific log was flagged as a threat.

How to use this:
Go to your GitHub repository.

Click on the pencil icon to edit the README.md.

Delete everything currently in the file and paste the content above.

Important: Replace YOUR_USERNAME in the clone command with your actual GitHub username.

Upload your image_c348c2.jpg to the repository so the "Results" section has the visual proof!
AI-Log-Anomaly-Detector
