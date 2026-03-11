# LLM RAG Enterprise Search

Enterprise style Retrieval Augmented Generation system for document search and question answering.

## Features
Document ingestion  
Vector embeddings  
Semantic search  
LLM answer generation  
FastAPI service

## Tech Stack
Python  
FastAPI  
Transformers  
Sentence Transformers  
FAISS  
PyTorch

## Project Structure
app/api/main.py – API endpoints  
app/rag – embedding, retrieval, generation logic  
app/ingestion – document indexing pipeline  
data – sample documents

## Install

pip install -r requirements.txt

## Run

python app/ingestion/ingest_documents.py

uvicorn app.api.main:app --reload

## Endpoint

GET /query?q=question
