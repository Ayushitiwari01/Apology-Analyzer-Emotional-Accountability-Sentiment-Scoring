# 🤖 Apology Analyzer – Emotional Accountability & Sentiment Scoring

A Python-based NLP tool that analyzes apology statements by scoring their **Emotional Accountability Score (EAS)** and classifying their **sentiment** and **interpretation**. This project helps determine how responsible or deflective an apology is using natural language understanding.

---

## 🚀 Features

* ✅ **Sentiment Analysis** using TextBlob
* ✅ **Emotional Accountability Score (EAS)** to quantify apology depth
* ✅ Classification into:

  * High Accountability
  * Medium Accountability
  * Low Accountability
  * Deflective / No Accountability
* ✅ Detection of key ownership, emotional, and deflective words
* ✅ Polarity adjustment using EAS to better reflect sincerity
* ✅ Easy to extend and customize for various contexts (e.g., corporate, public, personal)

---

## 📊 How It Works

1. **Input**: Any natural language apology (e.g., `"I take full responsibility for my mistake."`)
2. **Processing**:

   * Polarity via TextBlob
   * Word-level scan for predefined **ownership**, **emotional**, and **deflection** terms
   * Computes a normalized Emotional Accountability Score (EAS)
3. **Output**:

   * Adjusted Sentiment (`Positive`, `Weak Positive`, `Neutral`, `Negative`)
   * EAS Score (ranging -10 to +10)
   * Interpretation (`High Accountability` to `Deflective`)

---

## 📁 Example Output

```
📌 Apology: I am truly sorry for my actions. I deeply regret what I did and I take full responsibility.
   ➤ Sentiment: Positive (Polarity: 0.45)
   ➤ EAS (Emotional Accountability Score): 10
   ➤ Interpretation: High accountability
```

---

## 🛠️ Tech Stack

* **Python 3**
* **TextBlob** (for polarity and sentiment analysis)
* Custom logic for:

  * Ownership and emotional language parsing
  * Accountability scoring and categorization

---

## 📚 Use Cases

* HR & Conflict Resolution
* Public Relations Analysis
* Corporate Apology Evaluation
* Mental Health & Counseling Tools
* Social Media Sentiment Research

---

## 🌐 Future Scope

Here's what's planned next:

### 🔤 Multilingual & Mixed Language Support

* **Hindi-English (Hinglish)** hybrid apology detection
* Handle code-mixed language common on social media and informal communication
* Examples: `"Mujhe maaf karo, I really didn't mean to hurt you."`

### 🧠 ML-Based Classifier

* Use **supervised learning** (e.g., Logistic Regression or BERT) trained on apology datasets to:

  * Classify apology strength
  * Predict public acceptance likelihood

### 🧪 Dashboard & Visualization

* Develop a **web interface** or **dashboard** using Streamlit or Flask:

  * Upload/enter text
  * See sentiment charts
  * Export reports

### 📲 API Deployment

* Turn this into a microservice for plug-and-play integration in enterprise or research tools.

---

## 🧑‍💻 Author

**Ayushi Tiwari**
Aspiring Data Analyst | Machine Learning Enthusiast
GitHub: \[your-username]
Email: \[your-email]

---

## 📄 License

This project is open-source and available under the **MIT License**.

---

Would you like me to:

* Format this as a real `README.md` file for GitHub?
* Add sample `apologies.txt` and a `requirements.txt` for easier cloning and setup?

Let me know!
