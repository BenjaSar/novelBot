# 📚 Literary Corpus NLP Project

This project builds a high-quality text corpus from literary works (novels, short stories, etc.) for downstream **NLP** tasks like **TF-IDF analysis** and a **Retrieval-Augmented Generation (RAG)** chatbot.

---

## 🚀 Project Overview

**Features:**
- Preprocess and clean literary texts.
- Tokenize text into sentences and words.
- Remove low-content words (e.g., stopwords, pronouns, generic verbs, titles like *Mr.*, *Mrs.*).
- Compute word frequencies and TF-IDF scores.
- Find shared keywords across multiple corpora.
- Save tokenized corpus and TF-IDF scores to JSON for later use.
- Prepare the dataset for a RAG-based chatbot.

---

## 🛠️ Project Structure

---

## 📌 Key Files

- **`process_text.py`** — Tokenizes and cleans the text corpus with spaCy.
- **`find_shared_tfidf_words.py`** — Computes TF-IDF and finds shared keywords.
- **`corpus_list_token.json`** — Example saved tokenized corpus for your RAG pipeline.
- **`.gitignore`** — Keeps your repo clean (ignores venvs, logs, data files).

---

## ⚙️ How to Run

1. 📥 **Install dependencies:**

    ```bash
    python -m venv .venv
    source .venv/bin/activate   # On Windows: .venv\Scripts\activate
    pip install -r requirements.txt
    ```

2. 📚 **Download your literary texts** into `data/` (e.g., from Project Gutenberg).

3. 🧹 **Run your preprocessing script** to clean and tokenize:

    ```bash
    python scripts/preprocess.py
    ```

4. 🧮 **Run your TF-IDF analysis**:

    ```bash
    python scripts/tfidf_analysis.py
    ```

5. 💾 **Check your results** in `outputs/` and `corpus_list_token.json`.

6. 🤖 **Use the corpus** with your RAG chatbot pipeline.

---

## 🤝 Contributing
Feel free to fork, open issues, or submit pull requests!
This is an evolving project for NLP and literature lovers 📚✨

## License
MIT License

## ✨ Credits
* Python

* spaCy

* scikit-learn

* Matplotlib / Seaborn



