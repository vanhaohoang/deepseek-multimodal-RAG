# 🚀 Multimodal RAG with DeepSeek & Qdrant

Welcome to **Multimodal RAG**, a powerful **Retrieval-Augmented Generation (RAG) system** that combines text and image embeddings with **DeepSeek** and **Qdrant** to provide rich contextual responses! 🎯📚🔍

## 🌟 Features

✅ **Multimodal Embeddings**: Leverages `ColPali` for text and image embeddings 🖼️📖  
✅ **Efficient Retrieval**: Uses `Qdrant` for fast, high-dimensional vector search ⚡  
✅ **Seamless LLM Integration**: Works with `DeepSeek AI` for advanced response generation 🤖💡  
✅ **Streamlit UI**: A simple and interactive web interface for document indexing and querying 🎨🖥️  

---

## 🔧 Installation

Make sure you have the required dependencies installed:
```bash
pip install torch qdrant-client colpali-engine Janus transformers streamlit pdf2image tqdm
```

---

## 🚀 How It Works

1️⃣ **Embed Images & Text**:
   - Uses `ColPali` to generate embeddings for images and text chunks.  
   - Stores them in `Qdrant`, a fast, scalable vector database.  

2️⃣ **Efficient Search & Retrieval**:
   - Queries are transformed into embeddings and matched against stored vectors.
   - `Qdrant` returns the most relevant images/texts.  

3️⃣ **Augmented Generation with LLM**:
   - The retrieved data is used to **enhance** LLM responses.  
   - **DeepSeek AI** generates a context-aware response.  

4️⃣ **User-Friendly UI**:
   - Upload PDFs 📄, view indexed images 🖼️, and chat 💬 with the AI!

---

## 🏗️ Code Overview

### 1️⃣ **`ragcode.py`** (Core RAG Logic)
- `EmbedData`: Converts images & text into embeddings using `ColPali` 📷📖
- `QdrantVDB_QB`: Manages the `Qdrant` vector database 🔎
- `Retriever`: Searches for the most relevant context 🔥
- `RAG`: Generates responses using `DeepSeek AI` 🧠💬

### 2️⃣ **`app.py`** (Streamlit UI)
- Upload PDFs 📂 and extract images 🔍
- Index and query documents with a **simple chat interface** 🤖
- Render results in a friendly web UI 🏡

---

## 🎯 Quick Start

Run the Streamlit app and start querying!
```bash
streamlit run app.py
```

🔍 **Upload PDFs, index them, and get AI-powered answers instantly!**

---

## 🤝 Contributing

We welcome contributions! Feel free to fork, improve, and submit a pull request. 🚀

📧 **Have questions?** Reach out anytime! ✨

---

## 🏆 Credits
- Built with ❤️ using `DeepSeek`, `Qdrant`, `ColPali`, and `Streamlit` 🎉
- Inspired by **state-of-the-art RAG techniques** 🔥

---

🔹 **Star this repo ⭐ if you find it useful!**  
🔹 **Happy coding & exploring AI! 🤖💡**

