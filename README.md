# Sarcasm-Detector-for-text
A sarcasm detection tool that uses NLP and logistic regression to classify tweets as sarcastic or not. Trained on labeled data and powered by TF-IDF vectorization with n-grams, it offers real-time predictions with confidence scores. Built with scikit-learn, this lightweight CLI tool is ideal for experimenting with sentiment nuance in text.


## 🧠 Model Details

- **Algorithm**: Logistic Regression (with class balancing)
- **Vectorizer**: TF-IDF with n-grams (unigram + bigram)
- **Text Preprocessing**: Lowercasing, removing URLs, mentions, hashtags, and punctuation
- **Target Labels**:
  - `1` → Sarcastic
  - `0` → Regular

---

## 🔧 Requirements

Install dependencies with:
pip install -r requirements.txt

If using only the Streamlit version, you may also just install:
pip install streamlit pandas scikit-learn

🌐 Streamlit Web App
Path: streamlit_app/app.py

This version runs a clean, interactive web interface using Streamlit. Enter a sentence and get a prediction with confidence levels for both sarcastic and regular.

▶️ Run it:
cd streamlit_app
streamlit run app.py
💡 Sample Output:
Prediction: Sarcastic 😏 or Regular 🙂

Confidence: Percentage bars for both classes

📊 Dataset
File: train.csv
Columns:
tweets: The text data
class: The label (sarcasm or something else)
Binary label conversion:
sarcasm → 1
all others → 0

"

🚀 Future Improvements
Add deep learning model (e.g., LSTM or BERT)

Deploy Streamlit app to Streamlit Cloud or Hugging Face

Add sarcasm explanation/rationale

Use a larger or more diverse dataset

🧑‍💻 Author
Developed by Aman Jain
Feel free to fork, improve, and share!

