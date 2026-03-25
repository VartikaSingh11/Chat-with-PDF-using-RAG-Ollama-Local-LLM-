# Chat-with-PDF-using-RAG-Ollama-Local-LLM-
This project demonstrates a complete end-to-end RAG pipeline using local LLMs without external APIs.

#Project Overview

This project implements a Retrieval-Augmented Generation (RAG) pipeline that allows users to ask questions from a PDF document using a local LLM (phi3 via Ollama).

#The system ensures:
Answers are based only on the document
No hallucinations (controlled output)
Fully runs locally (no API needed)

#Tech Stack
Python
LangChain
Ollama (phi3 + Nomic Embeddings)
ChromaDB (Vector Database)
PyPDF

#How It Works
Load PDF
Split into chunks
Convert text → embeddings
Store in vector database
Retrieve relevant chunks
Generate answer using LLM

#Setup Instructions
1. Install Ollama

Download from: https://ollama.com

Run:

ollama run llama2
2. Pull Embedding Model
ollama pull nomic-embed-text
3. Install Dependencies
pip install -r requirements.txt
4. Run Notebook
jupyter notebook

Open:

notebooks/rag.ipynb
