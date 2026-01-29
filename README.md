# ClickAware 🔐  
### Malicious URL Detection using Machine Learning

ClickAware is a simple **Application Security project** that detects whether a given URL is **Benign, Phishing, Malware, or Defacement** using machine-learning techniques.  
The project focuses on **URL-based threat detection**, a common real-world security problem.

---

## 📌 Problem Statement
Malicious URLs are widely used in:
- Phishing attacks
- Malware distribution
- Website defacement
- Credential theft

Manually identifying such URLs is unreliable.  
This project demonstrates how **machine learning + security feature engineering** can help classify malicious URLs automatically.

---

## 🛠️ Technologies Used
- **Python**
- **Google Colab**
- **Pandas, NumPy**
- **Scikit-learn**
- **Matplotlib, Seaborn**
- **tld (Top Level Domain extraction)**

---

## 📂 Dataset
- **Dataset Name:** Malicious URLs Dataset  
- **Source:** Kaggle  
- **Classes:**
  - Benign
  - Phishing
  - Malware
  - Defacement

> ⚠️ Dataset is not included in this repository.  
> Please download it manually from Kaggle and place it in Google Drive.

---

## ⚙️ Features Extracted
The model does **URL-based feature engineering**, including:

- URL length
- Count of special characters (`@`, `?`, `-`, `=`, `//`, etc.)
- Presence of IP address in URL
- HTTPS usage
- Abnormal URL structure
- URL shortening services detection
- Number of digits and letters
- Domain extraction using TLD

These features are commonly used in **Application Security and Web Security analysis**.

---

## 🧠 Machine Learning Model
- **Algorithm:** Random Forest Classifier
- **Train/Test Split:** 80/20
- **Evaluation Metrics:**
  - Accuracy
  - Confusion Matrix
  - Classification Report

The trained model is saved using **pickle** for reuse during prediction.

---

## ▶️ How to Run the Project

### 1️⃣ Download the dataset
Download `malicious_phish.csv` from Kaggle.

### 2️⃣ Upload to Google Drive
Upload the file to:
MyDrive/

### 3️⃣ Open the Notebook
Open `ClickAware.ipynb` in **Google Colab**.

### 4️⃣ Update dataset path (if needed)
python
data = pd.read_csv('/content/drive/MyDrive/malicious_phish.csv')

###5️⃣ Run all cells

Train the model and test URL classification.

---

## 🔍 URL Prediction Example
The user can input a URL, and the system outputs:
Predicted Category (Benign / Phishing / Malware / Defacement)
Safety Status (Safe / Unsafe)

Example:
Enter URL: http://secure-login-update.net
Predicted Category: Phishing
URL Safety: Unsafe

---

## 📊 Output

1. Accuracy score of the model
2. Confusion matrix visualization
3. Classification report
4. Real-time URL classification

---
