# Retrieval-Augmented-Generation_Chatbot
*Domain: EdTech | NLP | RAG | Streamlit UI | Vector DB | LLM Integration*
 
This project implements an **AI-powered Retrieval-Augmented Generation (RAG) chatbot** designed for the **GUVI Learning Platform**.  
It provides **accurate, contextual and explainable answers** to learner queries by retrieving information from **course materials, FAQs, notes, and blogs**, and then generating responses using a **fine-tuned LLM**.
 
---
 
## 🚀 Features
 
| Feature | Description |
|--------|-------------|
| **RAG Pipeline** | Combines semantic retrieval + LLM generation |
| **Vector Embeddings Search** | Uses FAISS/Chroma for efficient chunk search |
| **Context-Aware Answering** | Retrieves top-k relevant text chunks for correct answers |
| **Streamlit Chat UI** | Modern, clean, real-time interactive chat interface |
| **Chat Memory** | Maintains conversation context |
| **Auto Document Indexing** | Converts documents into embeddings with `memory_builder.py` |
| **Supports Local LLaMA / Mistral / Falcon Models** | Works offline using llama-cpp-python |
 
---
 
## 🎯 Problem Statement
 
Learners face difficulty in getting **quick and accurate answers** from lengthy course content.  
This chatbot acts as a **24/7 intelligent tutor**, capable of answering:
 
- Technical doubts from course notes  
- Common FAQ queries  
- Concept explanations  
- Career and learning path guidance  
 
---
 
---
 
## 📂 Project Structure
 
/project-root
│── chatbot_app.py # Normal chatbot interface (no retrieval)
│── rag_chatbot_app.py # RAG-based chatbot interface
│── memory_builder.py # Builds vector index from documents
│── models/ # GGUF LLaMA / Mistral model files
│── docs/ # Knowledge base (markdown files)
│── vector_store/ # FAISS / Chroma embeddings directory
│── chatbot/
│ │── bot/
│ │── conversation/
│ │── client/
│ │── model/
│ │── memory/
│ │── helpers/
 
 
---
 
## 🛠️ Tech Stack
 
| Component | Technology Used |
|----------|----------------|
| Language Model | **LLaMA / Mistral / Falcon (GGUF)** via llama-cpp-python |
| Embeddings | **sentence-transformers / all-MiniLM-L6-v2** |
| Vector Store | **Chroma / FAISS** |
| Frontend UI | **Streamlit Chat Interface** |
| Document Loader | Markdown Loader + Recursive Chunking |
| Deployment | Local / Streamlit Cloud / HuggingFace Spaces |
 
---
