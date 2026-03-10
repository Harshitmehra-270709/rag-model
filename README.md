# RAG Model

This repository contains the codebase for a Retrieval-Augmented Generation (RAG) model. It focuses on taking transcripts, chunking them, creating vector embeddings, and performing semantic queries to generate informed responses.

## Key Features

- **Speech-to-Text (`Speech_to_text.py`)**: Generates text transcripts from audio inputs.
- **Transcript Chunking (`chunk_transcripts.py`, `overlap_chunks.py`)**: Breaks down large text passages into smaller, manageable chunks (optionally with overlap) to maintain context.
- **Embedding Creation (`create_embeddings.py`)**: Generates mathematical vector representations of the text chunks.
- **Vector Database**: Saves embeddings to a local SQLite-backed vector database for rapid semantic retrieval.
- **RAG Querying (`rag_query.py`)**: The main interface that searches the vector database for relevant chunks and uses them as context to answer user queries.

## Getting Started

1. Set up a virtual environment: `python -m venv venv`
2. Activate the environment: `.\venv\Scripts\Activate.ps1`
3. Install dependencies (make sure `requirements.txt` is populated if not already).
4. Configure your API keys in the `.env` file (DO NOT commit this file to version control).

## Usage

*Ensure all sensitive `.env` files and large generated artifacts output to `data/`, `vector_db/`, or `.mp3`/`.wav` files remain ignored in your `.gitignore`.*
