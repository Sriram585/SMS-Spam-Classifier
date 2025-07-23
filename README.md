#  SMS Spam Classifier

This is a simple, interactive **Spam Detection Web App** built using **Streamlit**. The app uses a **machine learning model** trained to classify SMS messages as either **Spam** or **Not Spam**.

---

##  How It Works

1. **Text Preprocessing**  
   Custom `transform_text()` function:
   - Converts text to lowercase
   - Tokenizes text using regex
   - Removes manually defined stopwords
   - Applies stemming using `PorterStemmer`

2. **Vectorization**  
   Uses **TF-IDF (Term Frequency–Inverse Document Frequency)** vectorization to convert text into numerical format.

3. **Prediction**  
   Uses a pre-trained **machine learning model** (loaded from `model.pkl`) to classify the message:
   - `1` → Spam  
   - `0` → Not Spam

---

## 🛠️ Technologies Used

- **Python**
- **Streamlit**
- **NLTK (PorterStemmer only)** – No downloads required
- **Scikit-learn** – For vectorization and model training
- **Pickle** – For loading the model and vectorizer

---

