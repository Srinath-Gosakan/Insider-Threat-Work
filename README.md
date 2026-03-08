# Insider Threat Detection Using Machine Learning

## Overview

Insider threats are one of the most difficult cybersecurity risks to detect because malicious activities often resemble legitimate user behavior. Traditional rule-based monitoring systems struggle to identify subtle behavioral anomalies.

This project builds a **machine learning based behavioral analytics system** to detect potential insider threats by analyzing user activity logs such as logins, file access, device usage, and web activity.

The objective is to identify **suspicious behavioral patterns** that may indicate data exfiltration, privilege misuse, or other insider threats.

---

## Dataset

This project uses the **CERT Insider Threat Dataset (Release 6.2)**.

The dataset contains simulated enterprise user activity logs including:

* Logon events
* File access activity
* Email communications
* HTTP browsing logs
* Device usage events

Dataset Source:

https://www.kaggle.com/datasets/goseh11/r6-2-dataset

Note:
The dataset is **not included in this repository** because it exceeds GitHub's file size limits.

### How to Download

1. Visit the Kaggle dataset page.
2. Download the dataset.
3. Extract the files.
4. Place them inside the `data/` directory.


## Project Structure

```
Insider-Threat-Work
│
├── notebooks
│   ├── Self Attention Neural Networks.ipynb
│   ├── SPCAGAN.ipynb
│   ├── chebyshev-graph-laplacian.ipynb
│
├── data
│   └── (downloaded dataset files)
│
└── README.md
```

---

## Methodology

The workflow followed in this project:

1. **Data Collection**

   * Import activity logs from the CERT dataset.

2. **Data Preprocessing**

   * Cleaning missing values
   * Converting timestamps
   * Encoding categorical features

3. **Feature Engineering**

   * Login frequency
   * File access counts
   * Device usage patterns
   * Data transfer activity

4. **Model Training**
   Machine learning models are trained to identify anomalous behavior patterns.

5. **Evaluation**
   Models are evaluated using classification metrics to determine how well insider threats can be detected.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## Example Features Used

Examples of behavioral features extracted from logs:

* Number of logins per day
* Failed login attempts
* File download activity
* USB device usage
* Unusual working hours
* Email volume

These features help identify deviations from normal user behavior.

---

## Results

The trained model identifies **anomalous user activity patterns** that could indicate insider threats.

Outputs include:

* Suspicious user detection
* Anomaly scores
* Behavioral pattern analysis

---

## Future Improvements

Potential improvements for this project:

* Implement real-time anomaly detection
* Use deep learning models such as LSTM for sequential activity analysis
* Build a monitoring dashboard
* Deploy the model as a security analytics API

---

## Disclaimer

The CERT dataset contains **synthetic enterprise activity logs** created for research purposes. This project is intended for **educational and research use only**.
