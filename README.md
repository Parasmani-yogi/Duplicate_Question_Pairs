# Duplicate Question Pairs Detection

## Overview
This project focuses on detecting whether two questions are **semantically duplicate** or not.

Using Natural Language Processing (NLP) techniques and Machine Learning, the system extracts multiple similarity features from question pairs and predicts duplication using a trained Scikit-Learn model.

A **Streamlit web application** has been developed to provide a simple and interactive interface for real-time predictions.

---

## Features
- Text preprocessing and normalization (cleaning, decontracting, symbol handling)  
- Handcrafted similarity feature extraction  
- TF-IDF vectorization for text representation  
- Fuzzy string matching techniques  
- Real-time prediction using Streamlit interface  
- Lightweight and fast ML-based solution  

---

## Tech Stack
- **Language:** Python  
- **Libraries:** Pandas, NumPy, Scikit-learn, NLTK, FuzzyWuzzy, BeautifulSoup, Distance  
- **Framework:** Streamlit  
- **Modeling:** TF-IDF + Machine Learning Classifier  

---

## How to Run

### Install Required Packages
Ensure you have Python 3.8 or higher installed. Then install dependencies:

```bash
pip install -r requirements.txt
```

(Optional – improves fuzzy matching performance)
```bash
pip install python-Levenshtein
```

---

### Run the Application Locally
If Streamlit is not installed, run:
```bash
pip install streamlit
```
Download or clone the repository, then open the terminal inside the project folder and run:

```bash
streamlit run app.py
```

- Once the command runs, Streamlit will automatically open the app in your default browser.

---

## Required Files
Make sure the following files are present in the root directory:

- model.pkl  
- tfidf.pkl  
- stopwords.pkl  

Without these files, the application will not run.

## Dataset
The dataset used in this project is sourced from Kaggle's **Quora Question Pairs** competition:

Dataset link : [https://www.kaggle.com/c/quora-question-pairs](https://www.kaggle.com/c/quora-question-pairs)
