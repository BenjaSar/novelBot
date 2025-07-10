# 📚 Literary Corpus NLP Project  --  NovelBot

###### Author: FS


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

3. Add your environment variables
Create a .env file or export the following:

```
OPENAI_API_KEY=your_openai_key_here
PINECONE_API_KEY=your_pinecone_key
PINECONE_ENV=your_pinecone_environment
Or you can pass api_key directly in code if you're testing.
```

4. 🧹 **Run your preprocessing notebook** to clean and tokenize:

    ```bash
    EDA.ipynb
    ```

**Run your RAG notebook**:

    ```bash
    RAG.ipynb
    ```

5. 💾 **Check your results** in `outputs/` and `corpus_list_token.json`.

6. 🤖 **Use the corpus** with your RAG chatbot pipeline.

📋 Features

    AgentState structured management (task, context, content)

    LangGraph to define multi-step reasoning workflows (plan → retrieve → generate)

    RetrievalQA pipeline for grounding LLM responses with vector search

    Modular nodes: easy to plug in smarter planning, retrieval, or generation modules

**Run your RAG notebook**:

    ```bash
    RAG.ipynb
    ```
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



