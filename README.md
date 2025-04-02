# 🧠 FileSage

FileSage is an intelligent file analysis and query engine that ingests text documents, code files, markdown, PDFs, presentations, Word docs, and images. It uses OCR and language models to extract and index content, enabling natural language search with output as rich Word and PDF reports — including referenced images. 

## ✨ Features

- 🔍 Query any content using natural language
- 📁 Supports `.txt`, `.md`, `.py`, `.js`, `.pdf`, `.pptx`, `.docx`, `.png`, `.jpg`, `.jpeg`
- 🧾 Extracts text from scanned images using OCR
- 📄 Generates well-formatted `.docx` and `.pdf` reports with embedded images
- 📚 Uses FAISS vector store + OpenAI embeddings for semantic search

## 🚀 Usage

.env

OPENAI_API_KEY=your-key-here

put all files in DATA folder.

```bash

pip install -r requirements.txt

# Ingest all supported files from the data/ folder
python ingest.py

# Query the project using natural language
python query.py "Show all Hello World implementations"
