
Text Sentiment Prediction App
🧠 Overview
This project is a web-based sentiment analysis tool that allows users to predict the sentiment (Positive/Negative) of input text or a CSV file of sentences. It combines a Flask API backend for model inference with a Streamlit frontend for user interaction.

🚀 Features
Predict sentiment for individual sentences.

Upload a CSV file for bulk sentiment analysis.

Download prediction results as a CSV.

Displays a sentiment distribution chart for bulk predictions.

Interactive and user-friendly interface.

📁 Project Structure
bash
Copy
Edit
.
├── main.py                # Streamlit frontend
├── api.py                 # Flask API backend
├── Models/                # Trained ML models (XGBoost, Scaler, CountVectorizer)
├── templates/
│   └── landing.html       # Flask homepage (optional use)
└── Data Exploration & Modelling.ipynb  # Exploratory Data Analysis and model training
🧰 Setup Instructions
Clone the repository and navigate into it:

bash
Copy
Edit
git clone https://github.com/your-username/sentiment-predictor.git
cd sentiment-predictor
Install required packages:

bash
Copy
Edit
pip install -r requirements.txt
Example requirements:

txt
Copy
Edit
streamlit
flask
flask-cors
pandas
matplotlib
nltk
scikit-learn
xgboost
Download NLTK stopwords (if not already downloaded):

python
Copy
Edit
import nltk
nltk.download('stopwords')
⚙️ Run the Application
1. Start the Flask API
bash
Copy
Edit
python api.py
It runs on http://127.0.0.1:5000

2. Launch the Streamlit Frontend
In a new terminal:

bash
Copy
Edit
streamlit run main.py
Access at: http://localhost:8501

📄 Input Format
For Single Prediction
Type directly into the text box.

For Bulk Prediction (CSV)
Upload a .csv file with the following format:

Sentence
I love this!
This was terrible

📤 Output
Sentiment predictions: Positive or Negative

Downloadable CSV with results

Pie chart of sentiment distribution

🛠 Model Information
Model: XGBoost Classifier

Vectorizer: CountVectorizer

Scaler: StandardScaler

Preprocessing: Lowercasing, stemming, stopword removal

📌 Notes
Ensure all files in Models/ folder (model_xgb.pkl, scaler.pkl, countVectorizer.pkl) exist and are correctly referenced.

The app uses Flask CORS to allow communication between Streamlit and Flask.
