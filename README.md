# 🤖 Apology Analyzer – Accountability & Sentiment Scoring

A Python-based **NLP tool** that evaluates apology statements by measuring their **Emotional Accountability Score (EAS)**, **sentiment polarity**, and **interpretation level**. It also provides **visual insights** with **word clouds, pie charts, and bar charts**.

---

## 🚀 Features

* ✅ **Sentiment Analysis** (Positive / Weak Positive / Neutral / Negative) using **TextBlob**
* ✅ **Emotional Accountability Score (EAS)** → Quantifies apology depth by checking ownership, emotions, and deflection
* ✅ **Interpretation** → Categorizes accountability into High, Medium, Low, or Deflective
* ✅ **Word Cloud Visualization** → Highlights frequent terms in apologies
* ✅ **Pie & Bar Charts** → Show accountability distribution and sentiment spread

---

## 📊 Example Output

### 🔹 Word Cloud

Shows the most frequent words across all apologies.

### 🔹 Pie Chart

Distribution of **accountability levels (EAS-based)**

### 🔹 Bar Chart

Comparison of **sentiment categories**

---

## 📌 Usage

```python
from analyzer import analyze_apology

# Example
text = "I take full responsibility and sincerely apologize for my mistake."
result = analyze_apology(text)
print(result)
```

### Example Output:

```json
{
  "text": "I take full responsibility and sincerely apologize for my mistake.",
  "sentiment": "Positive",
  "polarity": 0.75,
  "EAS": 8,
  "interpretation": "High accountability"
}
```

---

## 📈 Visualizations

Run the script to generate **Word Cloud, Pie Chart, and Sentiment Bar Chart**:

```bash
python visualize.py
```

---


## 🧠 Scoring Logic

**EAS = (2 × Ownership + 2 × Emotion – 3 × Deflection)** (normalized by text length)

* **≥ +7** → High accountability
* **+4 to +6** → Medium accountability
* **+1 to +3** → Low accountability
* **≤ 0** → Deflective / No accountability

---

## 💡 Applications

* Analyzing **politician/corporate apologies**
* Detecting **sincere vs. insincere apologies**
* Text mining for **PR crisis management**
* Sentiment & accountability research

---

