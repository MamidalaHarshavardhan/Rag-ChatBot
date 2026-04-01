🧠 RAG Chatbot

A lightweight and efficient **Retrieval-Augmented Generation (RAG) Chatbot** built using **Streamlit** and **Sentence Transformers**. This project demonstrates how semantic search can be combined with a simple knowledge base to deliver intelligent responses to user queries about AI concepts.

---

## 🚀 Overview

This chatbot leverages **embedding-based similarity search** to retrieve the most relevant answer from a predefined knowledge base. Instead of generating responses from scratch, it selects the best-matching context using cosine similarity.

It is designed to be:

* ⚡ Fast and lightweight
* 🧩 Easy to understand and extend
* 🎯 Focused on core RAG principles

---

## 🛠️ Tech Stack

* **Frontend/UI:** Streamlit
* **Embedding Model:** Sentence Transformers (`all-MiniLM-L6-v2`)
* **Similarity Search:** Scikit-learn (Cosine Similarity)
* **Numerical Processing:** NumPy
* **Transformer Utilities:** Hugging Face Transformers

---

## 📂 Project Structure

```
📦 RAG-Chatbot
 ┣ 📜 rag_chatbot.py        # Main Streamlit application
 ┣ 📜 requirements.txt      # Dependencies
 ┗ 📜 README.md             # Project documentation
```

---

## ⚙️ How It Works

### 1. Knowledge Base

A small set of AI-related documents is stored in memory.

👉 Defined in: 

---

### 2. Embedding Generation

* Documents are converted into vector embeddings using a pre-trained model.
* Cached for performance optimization.

---

### 3. Query Processing

* User input is converted into an embedding.
* Cosine similarity is calculated against stored document embeddings.

---

### 4. Retrieval

* The system selects the most relevant document.
* Returns it as the chatbot response.

---

## 🖥️ Installation & Setup

### Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/rag-chatbot.git
cd rag-chatbot
```

### Step 2: Install Dependencies

```bash
pip install -r requirements.txt
```

Dependencies used: 

---

### Step 3: Run the Application

```bash
streamlit run rag_chatbot.py
```

---

## 🎯 Features

* ✅ Simple and intuitive UI
* ⚡ Fast response using cached embeddings
* 🧠 Semantic search-based retrieval
* 🔁 Efficient model loading with caching
* 📦 Minimal dependencies

---

## 📸 User Interface

* Input box to ask questions
* Button-triggered response system
* Clean and minimal design

---

## 🧪 Example Queries

Try asking:

* “What is Machine Learning?”
* “Explain Deep Learning”
* “What are Large Language Models?”
* “What is RAG?”

---

## ⚡ Optimization Techniques Used

* `@st.cache_resource` → Prevents reloading the model
* `@st.cache_data` → Avoids recomputing embeddings
* Disabled tokenizer parallelism for stability

---

## ⚠️ Limitations

* 📉 Limited knowledge base (static documents)
* ❌ No generative LLM (retrieval only)
* 🔒 Not connected to external data sources

---

## 🔮 Future Improvements

* 🔗 Integrate with real LLMs (e.g., OpenAI / Hugging Face APIs)
* 📚 Add dynamic document ingestion (PDF, web scraping)
* 💬 Multi-turn conversational memory
* 🌐 Deploy on cloud (Streamlit Cloud / AWS / GCP)
* 🧠 Use vector databases (FAISS, Pinecone)

---

## 🤝 Contributing

Contributions are welcome!
Feel free to fork the repo and submit a pull request.

---

## 📜 License

This project is open-source and available under the **MIT License**.

---

## 👨‍💻 Author

**Harshavardhan Mamidala**
AI & ML Enthusiast | Developer | Innovator

---
