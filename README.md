# Antimicrobial Resistance Prediction for UTIs (GEN-UTI)

This project aims to predict antimicrobial resistance (AMR) in urinary tract infections (UTIs) using a hybrid approach that combines machine learning and genomic profiling. The system, GEN-UTI, is designed to support clinicians by providing personalized treatment recommendations based on both patient clinical data and genomic resistance markers.

## 🔍 Overview

Urinary tract infections are one of the most common bacterial infections, with rising cases of multidrug-resistant (MDR) pathogens like *E. coli* and *Klebsiella pneumoniae*. Traditional culture-based diagnostics are slow and do not account for patient-specific factors. GEN-UTI bridges this gap by combining:
- Clinical metadata (age, gender, renal function, pregnancy status, etc.)
- Genomic markers (e.g., presence of resistance genes like `blaCTX-M`, `blaNDM`)
- Machine Learning (Random Forest, SVM, CatBoost)
- A rule-based engine for tailored treatment suggestions

## 📌 Features

- ✅ Predicts MDR risk using Random Forest with >92% accuracy  
- 🧬 Incorporates genomic data to identify resistance genes  
- 🧠 Provides interpretable model outputs for clinicians  
- ⚕️ Suggests empirical treatments based on standard clinical guidelines  
- 💡 Context-aware recommendations (e.g., avoids nephrotoxic drugs for renal patients)

## 🧪 Tech Stack

- Python (Pandas, Scikit-learn, NumPy, Flask)
- Machine Learning: Random Forest, SVM, CatBoost
- Genomic data simulation & resistance feature extraction
- Jupyter Notebooks for EDA & model training
- Web interface (Flask) for input & prediction display

## 🛠️ Setup Instructions

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/GEN-UTI-AMR.git
   cd GEN-UTI-AMR
   
2.Create a virtual environment:

bash
Copy
Edit
python -m venv env
source env/bin/activate  # or env\Scripts\activate on Windows

3.Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt

4.Run the app:

bash
Copy
Edit
python app.py
