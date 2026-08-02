# Basic RAG System

A basic Retrieval-Augmented Generation (RAG) system built using Google Gemini that answers questions from PDF documents using text embeddings and semantic search.

## Features

- Upload any text-based PDF document
- Extract text from the PDF
- Split the document into overlapping chunks
- Generate embeddings using Gemini Embedding API
- Retrieve the most relevant chunks using cosine similarity
- Answer questions using only the retrieved document context
- Returns "I could not find this in the document." for questions outside the document

## Technologies Used

- Python
- Google Gemini API
- Google Colab
- PyPDF
- NumPy

## How It Works

1. Upload a PDF document.
2. Extract text from the PDF.
3. Split the text into chunks with overlap.
4. Generate embeddings for each chunk.
5. Convert the user's question into an embedding.
6. Retrieve the top matching chunks using cosine similarity.
7. Send the retrieved context to Gemini.
8. Generate an answer based only on the retrieved context.

## Project Structure

```
Basic-RAG-System/
│
├── RAG_system.ipynb
└── README.md
```

## Example Workflow

```
PDF
   │
   ▼
Text Extraction
   │
   ▼
Chunking
   │
   ▼
Embeddings
   │
   ▼
Semantic Search
   │
   ▼
Top Matching Chunks
   │
   ▼
Google Gemini
   │
   ▼
Answer
```

## Requirements

Install the required library:

```bash
pip install pypdf
```

You will also need:

- Google Gemini API Key
- Google Colab Secrets (`GEMINI_API_KEY`)

## Future Improvements

- Support multiple PDF documents
- Use a vector database (FAISS/ChromaDB)
- Interactive chat interface
- Citation of retrieved chunks
- Support for different embedding models

## License

This project is intended for learning and educational purposes.
