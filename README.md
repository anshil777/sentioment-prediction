# 🧠 Sentiment Analysis with Machine Learning

A machine learning project focused on building a sentiment classifier using Natural Language Processing (NLP) techniques and an XGBoost model. The project includes data exploration, preprocessing, model training, evaluation, and a lightweight web interface (Flask API + Streamlit) for interactive predictions.

---

## 📌 Objective

To analyze and model sentiment in textual data (Positive/Negative) using a supervised ML pipeline. The final model is served via a web interface for both individual and bulk predictions.

---

## 🔍 Project Highlights

- 📊 Exploratory Data Analysis (EDA) on text data
- 🧹 Text cleaning, stopword removal, stemming
- 🔠 Feature extraction using CountVectorizer
- ⚖️ Data scaling using StandardScaler
- 🤖 Model training with XGBoost Classifier
- 🧪 Evaluation metrics (accuracy, precision, recall, ROC-AUC)
- 🖥️ Web app interface with Streamlit and Flask

---



---

## 📊 Data Analysis & Modeling

Performed in the Jupyter Notebook `Data Exploration & Modelling.ipynb`:

### 🔹 Steps Covered:

- Initial data exploration and visualization
- Class imbalance check
- Text preprocessing:
  - Lowercasing
  - Regex-based cleaning
  - Stopword removal
  - Stemming with PorterStemmer
- Feature Engineering:
  - CountVectorizer
  - StandardScaler
- Model Training:
  - XGBoost Classifier
  - Cross-validation
- Evaluation:
  - Confusion matrix
  - Classification report
  - ROC-AUC curve

---

## 🧪 Model Summary

- **Model**: XGBoost Classifier
- **Input features**: Vectorized and scaled text
- **Preprocessing**: NLP cleaning → vectorization → scaling
- **Output**: Sentiment label — *Positive* or *Negative*

---

## 🌐 Web App Interface (Optional)

- **Flask API** serves the model
- **Streamlit frontend** for easy interaction

### 🖥 Run the Web App:

1. **Start API**

```bash
python api.py
