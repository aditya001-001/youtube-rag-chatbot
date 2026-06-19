# YouTube RAG Chatbot

A Retrieval-Augmented Generation (RAG) based Question Answering system that allows users to ask questions about a YouTube video and receive context-aware answers generated using Google's Gemini model.

## Overview

This project extracts transcripts from YouTube videos, converts the text into vector embeddings, stores them in a FAISS vector database, retrieves the most relevant chunks for a user query, and generates accurate responses using Gemini.

The system demonstrates the complete RAG pipeline, including data ingestion, text chunking, vector storage, retrieval, and LLM-powered answer generation.

## Features

* Extract transcripts directly from YouTube videos
* Split long transcripts into semantic chunks
* Generate embeddings using HuggingFace models
* Store and retrieve vectors using FAISS
* Context-aware question answering
* Powered by Google Gemini
* Built using LangChain components

## Tech Stack

* Python
* LangChain
* FAISS
* HuggingFace Embeddings
* Google Gemini
* YouTube Transcript API
* Python Dotenv

## Workflow

YouTube Video
→ Transcript Extraction
→ Text Chunking
→ Embedding Generation
→ FAISS Vector Store
→ Context Retrieval
→ Gemini LLM
→ Final Answer

## Installation

```bash
pip install -r requirements.txt
```

Create a `.env` file:

```env
GOOGLE_API_KEY=your_google_api_key
```

## Usage

1. Provide a YouTube video ID.
2. Extract the transcript.
3. Create embeddings and build the FAISS index.
4. Ask questions related to the video.
5. Receive context-aware answers generated using Gemini.

## Project Structure

```text
youtube-rag-chatbot/
│
├── rag_using_langchain.ipynb
├── requirements.txt
├── README.md
├── .gitignore
└── .env
```

## Future Improvements

* Streamlit Web Interface
* Multi-video support
* Persistent vector database
* Conversation memory
* Source citations for retrieved chunks

## Author

Aditya Sarapure
AI & Data Science Engineering
KLE College of Engineering & Technology, Chikodi
