# 🧠 RAG Course Knowledge Assistant

A Retrieval-Augmented Generation (RAG) system built from scratch using **LangChain**, **ChromaDB**, and **OpenAI Embeddings**.  
This project was created as part of my learning journey through the *Ultimate RAG Bootcamp (LangChain, LangGraph, LangSmith)* — transforming course transcripts and notes into an **intelligent study assistant**.

---

## 📘 Overview

This project demonstrates how to build a complete **Conversational RAG pipeline** capable of:
- Loading and preprocessing educational PDFs  
- Extracting structured metadata (topics, video titles, difficulty, etc.)  
- Chunking content using recursive splitting  
- Generating embeddings with OpenAI’s API  
- Storing and retrieving context using **Chroma vector store**  
- Running contextual question-answering with memory-aware chat history  

---

## 🧩 Architecture

PDF Loader → Metadata Extractor → Recursive Chunker → Embeddings → ChromaDB → Conversational RAG Chain




Each stage of the pipeline is modular — allowing easy replacement of loaders, embedding models, or retrievers.

---

## ⚙️ Tech Stack

| Component | Library / Tool |
|------------|----------------|
| Language | Python 3.12 |
| Framework | LangChain |
| Vector Store | ChromaDB |
| Embeddings | OpenAI (text-embedding-3-small) |
| Environment | `.env` file with API key |
| Notebook | Jupyter Notebook (`study_buddy.ipynb`) |

---

## 📂 Project Structure

RAG-Course-Knowledge-Assistant/
│
├── pdf/ # Raw course PDFs
├── chroma_store/ # Vector store (ignored in Git)
├── study_buddy.ipynb # Main RAG pipeline notebook
├── .env # OpenAI API key (ignored in Git)
├── .gitignore
└── README.md



---

## 🚀 Getting Started

### 1️⃣ Clone the Repository

git clone https://github.com/AbdullahAbuShammala/RAG-Course-Knowledge-Assistant.git
cd RAG-Course-Knowledge-Assistant
2️⃣ Install Dependencies

pip install -r requirements.txt
3️⃣ Add Your API Key
Create a .env file:

ini
Copy code
OPENAI_API_KEY=your-key-here
4️⃣ Run the Notebook
Open Jupyter and execute:

Copy code
study_buddy.ipynb
💬 Example Query
Question:

What are the main phases of a RAG system?

Answer:

Document Ingestion Phase

Query Processing Phase

Generation Phase

The assistant automatically retrieves and summarizes answers from the most relevant course documents.

🧠 Key Learnings
How to parse and structure unstructured course PDFs

Using recursive text splitting for context preservation

Building embeddings and managing a local vector store

Implementing a conversational RAG chain with memory

Evaluating retrieval relevance and context quality

🏁 Next Steps
Add Hugging Face embeddings for local/offline mode

Deploy as a Streamlit or Gradio web app

Integrate LangSmith for trace visualization

👤 Author
Abdullah AbuShammala
Data Scientist • AI & LLM Enthusiast
📍 Riyadh, Saudi Arabia





 







