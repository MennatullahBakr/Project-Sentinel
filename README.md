# Project Sentinel: Adaptive Cardiac Monitoring Engine

## About the Project

Project Sentinel started with a simple question: how can continuous cardiac monitoring become more accessible, dependable, and energy-efficient?

As cardiovascular diseases continue to be one of the leading health challenges worldwide, many monitoring solutions face limitations related to battery consumption and the large volume of data they need to process. Sentinel is a prototype designed to address these challenges through an adaptive monitoring approach.

Rather than analyzing every signal at maximum intensity all the time, the system adjusts its behavior based on the detected physiological state. This allows it to focus computational resources when they are most needed while reducing unnecessary processing during normal conditions.

## Why This Approach?

The project was built with a strong emphasis on practical design choices and explainable system behavior.

* **Efficient Resource Utilization:** The adaptive sampling mechanism enables the system to increase analysis depth only when potential abnormalities are detected, while remaining in a lower-power monitoring mode during stable periods. This approach can significantly reduce computational workload and energy consumption in wearable devices.

* **Data-Driven Development:** The detection framework was developed and evaluated using the MIT-BIH Arrhythmia Database, one of the most widely used benchmark datasets in cardiac signal research.

* **Privacy-Oriented Design:** The system focuses on physiological signal analysis and does not require personally identifiable information for its core functionality.

* **Machine Learning Integration:** CatBoost was selected as the primary classification model due to its strong performance, stability, and ability to handle complex physiological features effectively.

## How It Works

Project Sentinel follows a modular architecture that can be adapted to different hardware environments.

The workflow begins with cardiac signal acquisition and preprocessing. Relevant physiological features are then extracted and compared against an individualized baseline profile. When meaningful deviations are detected, the system generates alerts and adjusts its monitoring behavior accordingly.

Key project components include:

* `sentinel_engine.py` – Core engine responsible for signal processing, feature extraction, adaptive monitoring, and anomaly detection.
* `logs/alerts.csv` – Sample output demonstrating how the system classifies and reports cardiac events.
* `Prototype.ipynb` – Interactive notebook containing the complete simulation workflow and implementation details.

## Project Objective

The goal of Project Sentinel is to explore how intelligent monitoring strategies can improve the efficiency of cardiac surveillance systems without sacrificing analytical capability.

This prototype represents an effort to combine signal processing, machine learning, and adaptive decision-making into a practical framework that could support future wearable and remote health-monitoring applications.

## Getting Started

To explore the project results, review the `logs/alerts.csv` file, which contains sample monitoring outputs and alert classifications.

For a full walkthrough of the implementation and simulation process, open the `Prototype.ipynb` notebook in Google Colab and run the cells sequentially.

---

Project Sentinel is an ongoing prototype developed to investigate adaptive approaches to cardiac monitoring. Feedback, suggestions, and technical discussions are always welcome, as continuous improvement is an important part of the development process.
