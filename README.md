# Semantic File Search Using Sentence Transformers and FAISS
This project implements a semantic search system that reads PDF files (such as resumes), generates embeddings using a sentence transformer, stores them in a FAISS vector index, and allows fast semantic search to filter relevant files based on a query.

## What It Does
✅ Reads all PDF files from a specified folder (e.g., resumes).

✅ Extracts text content from each PDF.

✅ Splits the extracted text into smaller chunks to maintain semantic context.

✅ Converts text chunks into dense vector embeddings using a pre-trained SentenceTransformer model.

✅ Builds a FAISS index using the embeddings for efficient similarity search.

✅ Saves the FAISS index to disk.

✅ Supports semantic search queries to find and return filenames of the most relevant PDFs based on a given keyword or phrase.

## Tech Stack
pdfminer.six – for extracting text from PDF files

sentence-transformers – for generating vector embeddings

FAISS – for fast similarity search

langchain – used here only for text splitting
