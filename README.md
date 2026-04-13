# Production RAG System

A simple retrieval-augmented generation (RAG) system for answering questions from custom data.

It uses a vector database for retrieval and an LLM to generate context-aware responses.

---

## What it does

- answers questions from your data (PDF / text / docs)  
- retrieves relevant context using embeddings  
- generates responses grounded in retrieved data  
- reduces hallucination using RAG  

---

## How it works

1. Load and process documents  
2. Convert text → embeddings  
3. Store embeddings in vector DB (Qdrant)  
4. Retrieve relevant context for a query  
5. Pass context + query to LLM  
6. Generate final response  

---

## Tech stack

Python • LangChain • Qdrant • HuggingFace • FastAPI  

---

## Run locally

```bash
git clone https://github.com/thekazisakib/production-rag-system.git
cd production-rag-system

pip install -r requirements.txt
python app.py
