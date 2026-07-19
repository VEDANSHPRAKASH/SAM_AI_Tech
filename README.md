# Machine Learning Internship – SAM AI Technologies

![Status](https://img.shields.io/badge/status-completed-brightgreen)
![Python](https://img.shields.io/badge/python-3.10%2B-blue)
![License](https://img.shields.io/badge/license-MIT-lightgrey)

This repository contains my project submissions for the **Machine Learning Internship** at
**[SAM AI Technologies](https://sites.google.com/view/sam-ai-technologies/home)** — *"Your dream
your passion."*

The internship focuses on real-world, NLP-driven machine learning projects, giving hands-on
practice with text preprocessing, feature engineering, model training, and evaluation.

---


## ✅ Task List — Machine Learning Track

As part of the internship, **any 3 of the following 5 tasks** must be completed for successful
completion of the program. This repository includes working solutions for **all 5 tasks**.

| # | Project | Notebook | Status |
|---|---------|----------|--------|
| 1 | [Fake News Detection](#1-fake-news-detection) | `Fake_News_Detection.ipynb` | ✅ Complete |
| 2 | [Email Spam Classifier](#2-email-spam-classifier) | `Email_Spam_Classification.ipynb` | ✅ Complete |
| 3 | [Text Summarization](#3-text-summarization) | `Text_Summarization.ipynb` | ✅ Complete |
| 4 | [Named Entity Recognition (NER)](#4-named-entity-recognition-ner) | `Named_Entity_Recognition.ipynb` | ✅ Complete |
| 5 | [AI Chatbot using NLP](#5-ai-chatbot-using-nlp) | `AI_Chatbot_NLP.ipynb` | ✅ Complete |

---

### 1. Fake News Detection

Classifies news articles as **Real** or **Fake**.

- Preprocesses article text using NLP techniques (cleaning, stopword removal, stemming)
- Converts text into numerical features using **TF-IDF**
- Trains **Naive Bayes** and **Logistic Regression** classifiers
- Evaluates performance using **Accuracy** and **F1-Score**, with confusion matrices and
  cross-validation

**Notebook:** [`Fake_News_Detection.ipynb`](./Fake_News_Detection.ipynb)

---

### 2. Email Spam Classifier

Detects whether an email is **spam** or **ham** (legitimate).

- Cleans and preprocesses raw email text (URLs, HTML, punctuation, stopwords, stemming)
- Applies **TF-IDF vectorization** (unigrams + bigrams)
- Trains **Naive Bayes** and **SVM** classification models
- Displays the **predicted category** for new, unseen emails with confidence scores
- Evaluates with Accuracy, F1-Score, and ROC-AUC

**Notebook:** [`Email_Spam_Classification.ipynb`](./Email_Spam_Classification.ipynb)

---

### 3. Text Summarization

Generates concise summaries from long-form articles using **extractive summarization**.

- Cleans and preprocesses text (sentence splitting, tokenization, stopword removal)
- Implements three extractive techniques: **Word-Frequency scoring**, **TF-IDF scoring**, and
  **TextRank** (graph-based PageRank)
- Compares original text against generated summaries (compression ratio)
- Evaluates summary quality using **ROUGE scores** and a content-preservation similarity metric

**Notebook:** [`Text_Summarization.ipynb`](./Text_Summarization.ipynb)

---

### 4. Named Entity Recognition (NER)

Identifies and classifies entities in text — **names, locations, organizations, and dates**.

- Uses **spaCy** (`en_core_web_sm`) for entity recognition, compared against **NLTK**'s `ne_chunk`
- Visualizes detected entities inline using spaCy's `displacy` renderer
- Evaluates model performance (Precision, Recall, F1-Score) against a hand-labeled gold-standard set

**Notebook:** [`Named_Entity_Recognition.ipynb`](./Named_Entity_Recognition.ipynb)

---

### 5. AI Chatbot using NLP

A simple rule-assisted, ML-powered chatbot that understands user intent and generates responses.

- Preprocesses user input using NLP techniques (cleaning, stopword removal, stemming)
- Implements **intent recognition** (TF-IDF + Logistic Regression) and templated **response
  generation** with confidence-based fallback handling
- Handles **multiple conversation flows**, including a multi-turn appointment-booking flow with
  slot filling (name, date, time)
- Evaluates chatbot accuracy (intent classifier metrics) and simulated user-interaction quality

**Notebook:** [`AI_Chatbot_NLP.ipynb`](./AI_Chatbot_NLP.ipynb)

---

## 🛠️ Tech Stack

- **Language:** Python 3.10+
- **Core Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`
- **NLP:** `nltk`, `spaCy`, `rouge-score`
- **Machine Learning:** `scikit-learn` (TF-IDF, Naive Bayes, Logistic Regression, SVM)
- **Graph Algorithms:** `networkx` (TextRank)
- **Environment:** Jupyter Notebook

---

## 📂 Repository Structure

```
├── Fake_News_Detection.ipynb
├── Email_Spam_Classification.ipynb
├── Text_Summarization.ipynb
├── Named_Entity_Recognition.ipynb
├── AI_Chatbot_NLP.ipynb
└── README.md
```

---

## 🚀 Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/<your-username>/<your-repo-name>.git
   cd <your-repo-name>
   ```

2. **Install dependencies**
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn nltk spacy rouge-score networkx jupyter
   python -m spacy download en_core_web_sm
   ```

3. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook
   ```

4. Open any of the `.ipynb` files and run all cells (`Cell → Run All`).

> Each notebook is self-contained — if a real dataset isn't present in the folder, a synthetic
> sample dataset is generated automatically so every notebook runs end-to-end out of the box.

---

## 📄 License

This project is submitted as part of the SAM AI Technologies Machine Learning Internship Program
and is shared for educational and portfolio purposes.
