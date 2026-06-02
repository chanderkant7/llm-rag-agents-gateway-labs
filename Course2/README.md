# Course 2: RAG Basics

## Overview

This course introduces **Retrieval-Augmented Generation (RAG)**, a technique that combines document retrieval with language generation to create more accurate and contextual responses.

## Course Contents

### 1. **OpenAI_Connection.ipynb**
- Setting up OpenAI API with LiteLLM
- Authentication and configuration
- Testing basic completion requests
- Understanding API response structures

### 2. **Prompt_Engineering.ipynb**
- Crafting effective prompts
- Few-shot learning techniques
- Temperature and parameter tuning
- Prompt optimization strategies

### 3. **Sentiment_Analysis.ipynb**
- Building sentiment classifiers with LLMs
- Using Patient_Reviews.csv dataset
- Multi-class sentiment classification
- Real-world NLP application

### 4. **Text_Summarization.ipynb**
- Abstractive and extractive summarization
- Using conversation datasets
- Implementing RAG for context-aware summaries
- Quality metrics for summarization

## Data Files

- `Data/SentimentAnalysis/Patient_Reviews.csv` - Patient review dataset
- `Data/TextSummarization/conversation_*.txt` - Conversation samples for summarization

## Learning Objectives

- Understand RAG fundamentals and use cases
- Retrieve and rank relevant documents
- Integrate retrieval with LLM generation
- Handle different data formats (text, CSV)
- Evaluate RAG system performance

## Prerequisites

- Completion of Course 1
- Understanding of Langchain chains and prompts
- Basic familiarity with embeddings

## Running the Notebooks

1. Activate virtual environment
2. Ensure `.env` file has API keys
3. Open Jupyter:
```bash
jupyter notebook
```
4. Follow notebooks in order

## Key Concepts

- **Retrieval**: Finding relevant documents from a corpus
- **Context Window**: Using retrieved documents as context
- **Ranking**: Scoring document relevance
- **Generation**: Creating response using retrieved context

## Next Steps

Progress to **Course 3: Advanced RAG with ChromaDB** for production-ready vector databases and advanced retrieval techniques.
