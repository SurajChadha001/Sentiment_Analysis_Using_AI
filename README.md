
# Sentiment Analysis with TextBlob (Python)

This is a simple Python script that performs **sentiment analysis** using the `TextBlob` library. It evaluates whether a given text is **positive**, **negative**, or **neutral**.

---

## 🧠 How It Works

- The `TextBlob` library processes the input text.
- The `sentiment.polarity` value is used:
  - `> 0` → Positive
  - `< 0` → Negative
  - `== 0` → Neutral

---

## 📄 Example Code

```python
from textblob import TextBlob

def analyze_sentiment(text):
    blob = TextBlob(text)
    sentiment_score = blob.sentiment.polarity
    if sentiment_score > 0:
        return "Positive"
    elif sentiment_score < 0:
        return "Negative"
    else:
        return "Neutral"

post = "I love python! It's amazing."
print("Sentiment:", analyze_sentiment(post))

---
🧪 Output
makefile
Always show details

Copy
Sentiment: Positive
⚙️ Requirements
Python 3.6+

Install TextBlob:

bash
Always show details

Copy
pip install textblob
python -m textblob.download_corpora


Sentiment: Positive
⚙️ Requirements
Python 3.6+

Install TextBlob:
---
