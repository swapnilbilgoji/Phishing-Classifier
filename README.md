# 🛡️ Phishing Classifier using Machine Learning

A Python-based machine learning project to detect phishing websites using a variety of classification algorithms. This tool helps in improving web security by flagging potentially malicious URLs.

---

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Dataset Description](#dataset-description)
- [Features Used](#features-used)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Modeling Techniques](#modeling-techniques)
- [Results](#results)
- [Dependencies](#dependencies)
- [License](#license)

---

## 📌 Project Overview

Phishing websites are crafted to trick users into revealing sensitive data. This project uses machine learning to build a classifier that distinguishes between legitimate and phishing websites based on extracted features.

The classifier helps:

- Detect phishing URLs
- Prevent online fraud
- Increase awareness in cybersecurity practices

---

## 📊 Dataset Description

The dataset used contains labeled URLs classified as **legitimate (0)** or **phishing (1)** along with multiple features derived from their structure, content, and metadata.

Features include:

- Presence of IP address
- HTTPS status
- URL length
- Presence of special characters
- Domain age and registration

---

## 📌 Features Used

Some common features extracted:

- URL-based: `Having_IP_Address`, `URL_Length`, `Having_At_Symbol`
- Domain-based: `DNS_Record`, `Web_Traffic`, `Age_of_Domain`
- Technical: `SSLfinal_State`, `Popup_Window`, `Iframe`

These features are fed into classifiers to distinguish between phishing and legitimate sites.

---

## 🛠 Installation

1. Clone this repository:

```bash
git clone https://github.com/<swapnil bilgoji>/phishing-classifier.git
cd phishing-classifier
```

2. (Optional) Create and activate a virtual environment:

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install required libraries:

```bash
pip install -r requirements.txt
```

---

## ▶️ Usage

Run the Jupyter Notebook to:

1. Load the dataset
2. Preprocess the features
3. Train and test multiple classifiers
4. Evaluate model performance

Launch notebook:

```bash
jupyter notebook Phishing_Classfier_using_Machine_learning.ipynb
```

---

## 🧠 Modeling Techniques

The notebook tests multiple models:

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Support Vector Machine
- K-Nearest Neighbors

Evaluation metrics used:

- Accuracy
- Confusion Matrix
- Precision, Recall, F1-score

---

## 🏆 Results

- **Random Forest Classifier** yielded the best performance with over **95% accuracy**.
- Top features contributing to phishing detection were **SSLfinal\_State**, **Web\_Traffic**, and **Having\_IP\_Address**.

---

## 📦 Dependencies

- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- Jupyter Notebook

(Include these in `requirements.txt`)

---

## 📝 License

This project is licensed under the **MIT License**.


