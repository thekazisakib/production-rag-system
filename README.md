# Smart Chatbot (LLM + Vector DB)

A simple RAG-based chatbot that answers questions using a custom knowledge base.

It uses a vector database for retrieval and an LLM for generating context-aware responses.

---

## What it does

- answers questions from your data (PDF / text / docs)  
- retrieves relevant chunks using embeddings  
- generates responses using an LLM  
- reduces hallucination with retrieval  

---

## How it works

1. Load and process documents  
2. Convert text → embeddings  
3. Store embeddings in vector DB  
4. Retrieve relevant context for a query  
5. Pass context + query to LLM  
6. Generate final response  

---

## Tech stack

- Python  
- LangChain  
- Vector DB (Qdrant)  
- HuggingFace
- FastAPI (for API layer)  

---

## Run locally

```bash
git clone https://github.com/thekazisakib/Smart-Chatbot-LLM-VectorDB.git
cd Smart-Chatbot-LLM-VectorDB

pip install -r requirements.txt
python app.py
