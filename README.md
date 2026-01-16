# 🩺 Kidney Stone Prediction Web App

## 📌 Overview
This project is a **Streamlit-based web application** that predicts the risk of kidney stones using **machine learning models**.  
It leverages **Random Forest** and **Logistic Regression** classifiers trained on a dataset of urine parameters.  

The app allows users to:
- Input their urine test values interactively.
- Get predictions from both models (High Risk / Low Risk).
- Evaluate model performance with accuracy, classification reports, confusion matrices, and ROC curves.

---

## ⚙️ Features
- **Interactive Input Page**: Users enter values for urine parameters via sliders.
- **Prediction Results Page**: Displays model predictions side by side.
- **Evaluation Page**: Shows performance metrics, confusion matrices, and ROC curves.
- **Automatic Dataset Handling**: Detects target column and validates required features.

---

## 📂 Dataset
The app expects a CSV file named **`kidney-stone-dataset.csv`** with the following columns:

- `gravity` – Urine specific gravity  
- `ph` – Urine pH  
- `osmo` – Osmolality  
- `cond` – Conductivity  
- `urea` – Urea (mg/dL)  
- `calc` – Calcium (mg/dL)  
- `target` – Binary outcome (1 = High Risk, 0 = Low Risk)

> ⚠️ If the dataset does not contain `target`, the app assumes the last column is the target.

---

## 🚀 Installation & Setup

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/kidney-stone-prediction.git
   cd kidney-stone-prediction
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Ensure the dataset file `kidney-stone-dataset.csv` is in the project folder.

---

## ▶️ Usage

Run the Streamlit app:
```bash
streamlit run app.py
```

Navigate to the local URL shown in the terminal (usually `http://localhost:8501`).

---

## 📊 Example Workflow

1. **Input Page**  
   - Enter urine test values using sliders.  
   - Click **Predict** to see results.  
   - Click **Evaluate Models** to view performance metrics.

2. **Results Page**  
   - Displays entered values in a table.  
   - Shows predictions from Random Forest and Logistic Regression.  

3. **Evaluation Page**  
   - Accuracy scores for both models.  
   - Classification reports.  
   - Confusion matrices (visualized with heatmaps).  
   - ROC curves with AUC values.

---

## 🛠️ Technologies Used
- **Python 3**
- **Streamlit** – Web app framework
- **pandas / numpy** – Data handling
- **scikit-learn** – Machine learning models & metrics
- **matplotlib / seaborn** – Visualization

---

## 📈 Future Improvements
- Add more models (e.g., SVM, XGBoost) for comparison.
- Allow users to upload their own datasets.
- Deploy the app online (Heroku, Streamlit Cloud).
- Add feature importance visualization for Random Forest.

---

## 👨‍💻 Author
Developed by **Chandrasekaran S & Team**  
Passionate about building real-world AI solutions for healthcare.

