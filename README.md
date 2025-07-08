# Cybersecurity Threat Detection Using Machine Learning

This project uses machine learning to identify potential cybersecurity threats by analyzing network session data. It predicts whether network activity is safe or suspicious.

## Why This Project Matters

Cyberattacks are hard to detect manually. This project automates detection using patterns like failed logins, unknown browsers, or unusual access times. It helps security teams take action early.

## Dataset Information

The dataset includes ~9,000 records with features:
- Network Packet Size
- Protocol Type (e.g., HTTP, HTTPS)
- Login Attempts
- Session Duration
- Encryption Used (AES, DES)
- IP Reputation Score (0 to 1)
- Failed Logins
- Browser Type (Chrome, Firefox, etc.)
- Unusual Access Time (0 or 1)

## ML Models Used

Tested models:
- Logistic Regression
- SVC
- **Random Forest** (best performance)
- XGBoost

## Tools and Technologies

- Python
- Scikit-learn
- Pandas, NumPy, matplotlib, seaborn
- Pickle (for model saving)
- Gradio (for user interface)

## Project Structure

```
├── dataset/
│   └── cybersecurity.csv
├── app/
│   └── Cybersecurity Intrusion Detection.ipynb
├── model/
│   ├── cybersecurity.sav
│   ├── protocol_type.pkl
│   ├── encryption_used.pkl
│   └── browser_type.pkl
├── requirements.txt
├── describtion/
│    └── Cybersecurity Intrusion Detection.pptx
├── README.md
```

## Instructions for Beginners: How to Use This Notebook

This project includes a Jupyter Notebook file (`Cybersecurity-Intrusion-Detection.ipynb`) that can be downloaded and run locally using **Jupyter Notebook** or **JupyterLab**.

---

### Step 1: Download the Notebook File

1. Click on the notebook file (`Cybersecurity-Intrusion-Detection.ipynb`) in this repository.
2. Click the **“Download raw”** or **“Download”** button to save it to your computer.

---

### Step 2: Open the Notebook in Jupyter

#### If You Already Have Jupyter Installed:

1. Open a **Terminal** (Mac/Linux) or **Command Prompt** (Windows).
2. Navigate to the folder where the notebook was saved:

```bash
cd path/to/your/folder
```

3. Launch Jupyter Notebook:

```bash
jupyter notebook
```

4. Your browser will open with the Jupyter interface. Click on `Cybersecurity-Intrusion-Detection.ipynb` to open and run it.

---

### If Jupyter is Not Installed Yet:

#### Option 1: Install via pip (if Python is installed)

```bash
pip install notebook
```

Then launch it with:

```bash
jupyter notebook
```

#### Option 2: Use Anaconda (Recommended for Beginners)

1. Download and install **Anaconda** from:\
   https://www.anaconda.com/products/distribution
2. Open **Anaconda Navigator**
3. Click **Launch** under **Jupyter Notebook**
4. Navigate to the downloaded `.ipynb` file and open it

---

## How to Run the App Inside the Notebook

Once you've opened the notebook (`Cybersecurity-Intrusion-Detection.ipynb`) in **Jupyter Notebook** or **JupyterLab**, follow these steps:

### Step-by-Step Instructions

1. **Open the Notebook**\
   Launch Jupyter Notebook and click on the file `Cybersecurity-Intrusion-Detection.ipynb` to open it.

2. **Run the Cells Sequentially**

   - Click inside each code cell and press:
     - `Shift + Enter` to run the current cell and move to the next one
     - Or click the **Run (▶️)** button in the toolbar


3. **View the App in Your BrowserGradio will automatically open a browser tab with a local link like:**

   If your notebook uses Gradio, a simple UI will launch locally when you run the final code cell.

   Running on local URL:  http://127.0.0.1:7860 (Press CTRL+C to quit)

   Open this link in your browser to interact with the app.

### Sample Prediction Output
The model outputs:
    • Attack detected
    • No Attack detected


## 📚 What I Learned

- Data cleaning and preprocessing
- Model training and evaluation
- Label encoding for text data
- Web app deployment using Gradio

## About Me

Created by Dhanya Varghese 
Email: dhanya030697@gmail.com  
LinkedIn: https://www.linkedin.com/in/dhanya-varghese