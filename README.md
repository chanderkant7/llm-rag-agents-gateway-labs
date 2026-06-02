# RAG and Agentic AI using Langchain & LiteLLM Gateway

This repository contains comprehensive examples and implementations of RAG systems, Agentic AI, and multi-agent workflows using Langchain and LiteLLM.

## Quick Setup

### Prerequisites
- Python 3.8+
- API keys for LiteLLM providers (OpenAI, Anthropic, etc.)

### Install `uv` and Setup Environment

**Linux/macOS:**
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
uv venv .venv
source .venv/bin/activate
uv pip install -r requirements.txt
```

**Windows:**
```bash
powershell -c "irm https://astral.sh/uv/install.ps1 | iex"
uv venv .venv
.venv\Scripts\activate
uv pip install -r requirements.txt
```

### Configure API Keys

Create `.env` file in project root:
```env
OPENAI_API_KEY=your_openai_api_key
ANTHROPIC_API_KEY=your_anthropic_api_key
AZURE_API_KEY=your_azure_api_key
COHERE_API_KEY=your_cohere_api_key
```

## LiteLLM Quick Start

```python
from litellm import completion

response = completion(
    model="gpt-4",
    messages=[{"role": "user", "content": "Hello!"}],
)
print(response.choices[0].message.content)
```

Supports OpenAI, Claude, Azure, Cohere, HuggingFace, and more.

## Courses & Content

### **Course 1: Foundations**
Introductory examples covering basic LLM concepts and Langchain fundamentals.

### **Course 2: RAG Basics**
Retrieve documents and generate answers with:
- OpenAI Connection setup
- Prompt Engineering
- Sentiment Analysis on Patient Reviews
- Text Summarization on conversation datasets

### **Course 3: Advanced RAG with ChromaDB**
- Document embedding and chunking strategies
- ChromaDB data retrieval and re-ranking
- PDF processing and RAG evaluation
- Single and multi-PDF RAG systems

### **Course 4: Agentic AI**
Building intelligent agents with tools:
- React Agents (with/without built-in tools)
- Multi-user Conversational AI
- Multi-Agent Systems
- Tool implementation for agents

## Project: Insurance Agent Validation

End-to-end project implementing an intelligent insurance validation agent:
- **Data**: Insurance policies, reference codes, test records
- **Features**:
  - Multi-agent validation workflow
  - Human vs Agent performance comparison
  - Comprehensive test result analysis
  - Validation accuracy metrics

**Key Files**:
- `code.ipynb` - Complete implementation
- `validation_records.json` - Test dataset
- `agent_validation_records_results.csv` - Agent results
- `human_vs_agent_comparison.csv` - Performance comparison

## Resources

- [LiteLLM Docs](https://docs.litellm.ai/)
- [Langchain Docs](https://python.langchain.com/)
- [uv Package Manager](https://github.com/astral-sh/uv)

## License

Educational purposes