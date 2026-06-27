# Generative-Ai-and-Agentic
# Enterprise Multi-Document RAG AI Assistant

An end-to-end **Retrieval-Augmented Generation (RAG)** application built using **LangChain**, **LangGraph**, **ChromaDB**, and **Groq/OpenAI**. The project enables users to query information from multiple document formats using natural language while leveraging vector embeddings and semantic search for accurate responses.

---

## Features

* Multi-document ingestion (PDF, TXT, CSV)
* Automatic document preprocessing
* Intelligent text chunking
* Vector embedding generation
* Persistent vector storage using ChromaDB
* Semantic similarity search
* Retrieval-Augmented Generation (RAG)
* AI Agents powered by LangGraph
* Custom Tool Calling
* Structured JSON Output
* Middleware support
* Chat message management
* Modular project architecture

---

## Project Architecture

```
Documents
    │
    ▼
Document Loaders
(PyPDFLoader, TextLoader, CSVLoader)
    │
    ▼
Text Splitter
(RecursiveCharacterTextSplitter)
    │
    ▼
Embedding Model
    │
    ▼
ChromaDB Vector Store
    │
User Query
    │
Similarity Search
    │
Relevant Context
    │
    ▼
LangGraph Agent
    │
LLM (Groq/OpenAI)
    │
    ▼
Generated Answer
```

---

## Technologies Used

### Programming Language

* Python

### Frameworks

* LangChain
* LangGraph

### Vector Database

* ChromaDB

### LLM Providers

* Groq
* OpenAI

### Document Loaders

* PyPDFLoader
* TextLoader
* CSVLoader

### Embedding Models

* OpenAI Embeddings
* HuggingFace Embeddings (Optional)

### Other Libraries

* python-dotenv
* pypdf
* chromadb
* langchain-community
* langchain-text-splitters

---

## Project Structure

```
.
├── data/
│   ├── pdf/
│   ├── text_files/
│   └── vector_store/
│
├── src/
│   ├── data_loader.py
│   ├── embedding.py
│   ├── vectorstore.py
│   ├── rag_pipeline.py
│   └── config.py
│
├── notebooks/
│   ├── 1-langchain.ipynb
│   ├── 2-modelintegration.ipynb
│   ├── 3-tools.ipynb
│   ├── 4-messages.ipynb
│   ├── 5-structuredoutput.ipynb
│   └── 6-middleware.ipynb
│
├── requirements.txt
└── README.md
```

---

## Installation

Clone the repository

```bash
git clone https://github.com/Ahatesham121/Generative-Ai-and-Agentic.git

cd Generative-Ai-and-Agentic
```

Create a virtual environment

```bash
python -m venv .venv
```

Activate

Windows

```bash
.venv\Scripts\activate
```

Linux / macOS

```bash
source .venv/bin/activate
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## Environment Variables

Create a `.env` file

```env
GROQ_API_KEY=your_groq_api_key

OPENAI_API_KEY=your_openai_api_key
```

---

## Workflow

### Step 1

Load documents

* PDF
* TXT
* CSV

### Step 2

Split documents into chunks

### Step 3

Generate vector embeddings

### Step 4

Store vectors in ChromaDB

### Step 5

Retrieve relevant chunks using semantic similarity

### Step 6

Pass retrieved context to the LLM

### Step 7

Generate context-aware responses

---

## Example Query

```
User:
What are the responsibilities of a Software Engineer?
```

```
Assistant:
Based on the uploaded documents, the primary responsibilities include designing software, writing efficient code, debugging applications, collaborating with teams, and maintaining software systems.
```

---

## Skills Demonstrated

* Retrieval-Augmented Generation (RAG)
* AI Agent Development
* LangGraph Workflows
* Prompt Engineering
* Vector Databases
* Semantic Search
* Embedding Models
* Document Processing
* Function Calling
* Structured Outputs
* Middleware Design
* LLM Integration
* Context Retrieval
* Conversational AI

---

## Future Enhancements

* Streamlit Web Interface
* FastAPI REST API
* Multi-user Authentication
* Redis Caching
* Hybrid Search (Keyword + Vector)
* Conversation Memory
* Citation-Based Responses
* Docker Deployment
* Kubernetes Deployment
* Azure/OpenAI Integration

---

## Author

**Ahatesham Mopagar**

* Python Developer
* GenAI Developer
* Cybersecurity Enthusiast
* LangChain & LangGraph Developer

---

## License

This project is licensed under the MIT License.
