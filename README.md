Industrial Sensor Anomaly Detection & Machine Status Monitoring

Overview

This project is an advanced real-time industrial sensor anomaly detection system that continuously monitors sensor data from an SQLite database and detects potential faults in machine operations. By analyzing sensor values, detecting anomalies, and identifying correlations between different sensors, the system helps prevent failures, optimize performance, and increase equipment reliability.

Key Features

✅ Real-time Sensor Data Monitoring – Reads live sensor data from an SQLite database.
✅ Anomaly Detection – Uses statistical thresholds and machine learning techniques to detect anomalies.
✅ Machine Status Detection – Determines the operational state of machines based on sensor readings.
✅ Correlation Analysis – Identifies relationships between different sensors to pinpoint root causes of anomalies.
✅ Automated Reports & Alerts – Generates detailed reports (Excel) with affected sensors, correlated sensors, and timeline plots.
✅ Visualization – Saves sensor trend plots to track anomalies over time.
✅ Scalability & Flexibility – Can be adapted to different industrial setups.

Project Alignment with Jaaji Technologies

Jaaji Technologies specializes in IoT, AI-based industrial automation, and predictive maintenance solutions. This project aligns with their focus by providing:

AI-driven industrial monitoring & predictive analytics.

Automated anomaly detection for preventive maintenance.

Real-time machine health tracking with IoT-enabled sensor data processing.

This system can enhance Jaaji Technologies' existing solutions by integrating with their industrial automation tools, optimizing machine performance, and reducing downtime.

Installation Guide

Prerequisites

Ensure you have the following installed:

Python 3.x

SQLite (Pre-installed with Python)

Required Python Libraries (Install using requirements.txt)

Setup Instructions

1. Clone the Repository

git clone https://github.com/Abhishakth007/AI-Powered-Sensor-Anomaly-Detection-Reporting-System.git
cd industrial-anomaly-detection

2. Install Dependencies

pip install -r requirements.txt

3. Prepare the Database

Ensure your SQLite database contains real-time sensor data. The system reads from the database and updates at regular intervals.

4. Run the Anomaly Detection System

python main.py

5. View Reports & Alerts

Anomaly reports are generated as Excel files.

Sensor variation plots are saved in the sensor_variations/ folder.

Logs provide insights into detected anomalies and correlated sensors.

Project Structure

📂 industrial-anomaly-detection
├── 📄 Testing.ipynb                 # Entry point for real-time monitoring
├── 📄 Model_Development.ipynb       # Anomaly detection logic and ML Model Dev
├── 📄 correlation_data              # Sensor correlation computation
├── 📂 Data                          # SQLite data retrieval , Processed_Data , Raw Sensor Data
├── 📂 sensor_variations             # Stores timeline plots for sensors
├── 📄 requirements.txt              # Required dependencies
├── 📄 README.md                     # Project documentation

Troubleshooting

1. Database Connection Issues

Ensure the SQLite database is accessible and contains valid sensor data.

Verify the database path in database_handler.py.

2. No Anomalies Detected

Check if the sensor values exceed the defined anomaly threshold.

Adjust threshold values in anomaly_detection.py.

3. Missing Reports or Plots

Ensure sensor_variations/ folder exists for saving plots.

Verify report_generator.py runs without errors.

Future Enhancements

🔹 Integration with MQTT or Kafka for Streaming Data
🔹 Dashboard for Real-time Visualization
🔹 Machine Learning-based Predictive Maintenance
🔹 Support for Multiple Database Backends (PostgreSQL, MySQL)

Contributors

Name : D . Abhishakth

Open for contributions! Feel free to submit a PR.

License

This project is open-source and licensed under the MIT License.
