# 🧠 Context-Aware QA System Using LangChain

This project demonstrates the creation of a **question-answering chatbot** that provides answers related to **dental health** using a **retrieval-based QA system** built with **LangChain**, **OpenAI's GPT model**, and a **vector database**.

📎 [Click here to open the project notebook in Google Colab](https://colab.research.google.com/drive/1j5t3BYuRCFiUZVO_G1X3sTY8EuBfyRIO?usp=sharing)

---

## 📌 Project Overview

The chatbot is designed to **answer user queries about dental care and health** by retrieving relevant context from a set of documents. This is achieved through the use of:
- **LangChain’s RetrievalQA** chain
- **OpenAI’s `gpt-3.5-turbo` model**
- **FAISS vector database** for semantic search

Users can input natural language queries like _"How can I prevent cavities?"_ and the system provides accurate, context-aware answers.


## 🔧 Key Components

### 1. **Document Loading & Splitting**
- Text documents related to dental health are loaded into memory.
- Content is split into manageable chunks for efficient embedding and retrieval.

### 2. **Embedding Creation**
- Text chunks are embedded using **OpenAIEmbeddings**, transforming text into numerical vectors that represent meaning.

### 3. **Vector Store (FAISS)**
- A **FAISS** index is used to store and search embeddings.
- Allows fast similarity-based retrieval of relevant chunks.

### 4. **LLM Integration (OpenAI)**
- Uses `ChatOpenAI` from LangChain with the `gpt-3.5-turbo` model.
- Requires a valid OpenAI API key for execution.

### 5. **RetrievalQA Chain**
- Combines the retriever with the language model.
- Automatically fetches relevant content and generates an answer to the user’s query.


