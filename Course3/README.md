# Course 3: Advanced RAG with ChromaDB

## Overview

This advanced course covers production-ready RAG systems using ChromaDB for vector storage and retrieval. Learn document chunking, embeddings, retrieval ranking, and comprehensive RAG evaluation.

## Course Structure

### Module 2: Document Processing & Embeddings

#### **DataChunking.ipynb**
- Chunking strategies (fixed-size, recursive, semantic)
- Handling overlapping chunks
- Optimizing chunk size for retrieval
- Preserving context in chunks

#### **DocumentEmbeddings.ipynb**
- Generating embeddings with various models
- Embedding quality and dimensionality
- Storing embeddings in ChromaDB
- Vector similarity search

#### **Read Pdf File.ipynb**
- PDF parsing and extraction
- Handling different PDF formats
- Text extraction and cleaning
- Metadata preservation

#### **TalkToData.ipynb**
- Interactive chat with document data
- Real-time retrieval and generation
- Conversation history management
- Context-aware responses

#### **ChromaDB Data Retrieval and Re-ranking in RAG.ipynb**
- ChromaDB setup and configuration
- Advanced retrieval techniques
- Re-ranking retrieved documents
- Filtering and hybrid search
- Performance optimization

### Module 5: RAG Evaluation

#### **RAG_Evaluation_SinglePDF.ipynb**
- Evaluating RAG with single document
- Retrieval precision and recall
- Generation quality metrics
- Consistency checks

#### **RAG_Evaluation_MultiplePDF.ipynb**
- Handling multiple document sources
- Cross-document retrieval accuracy
- Handling conflicting information
- Scalability testing

#### **LLMTestcases.py**
- Automated test frameworks
- Performance benchmarking
- Regression testing
- Quality assurance

## Key Technologies

- **ChromaDB**: Vector database for embeddings
- **Langchain**: RAG orchestration
- **Various Embedding Models**: OpenAI, HuggingFace, etc.
- **PDF Processing**: PyPDF, pdfplumber

## Learning Objectives

- Implement production-ready RAG systems
- Master vector database operations
- Optimize retrieval performance
- Evaluate RAG system quality
- Handle multi-document scenarios
- Scale RAG to large datasets

## Running the Notebooks

1. Activate virtual environment
2. Install ChromaDB and dependencies:
```bash
uv pip install chromadb langchain pdf2image pdfplumber
```
3. Open Jupyter and follow Module 2 before Module 5

## Data

- `Data/` - Contains sample PDFs and documents for processing
- NLTK data for text processing

## Evaluation Metrics

- **Retrieval Metrics**: MRR, NDCG, Hit Rate
- **Generation Metrics**: BLEU, ROUGE, Exact Match
- **Latency**: Response time and throughput
- **Cost**: Token usage and API calls

## Next Steps

Complete Course 4 to learn how to build intelligent agents using tools and RAG systems together.
