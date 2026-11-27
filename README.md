#  AI Fake News Detection System using RAG

##  Project Overview

The **AI Fake News Detection System** is an AI-powered application designed to analyze news content and identify whether it is likely to be **Real or Fake** using Retrieval-Augmented Generation (RAG) architecture.

The system combines Natural Language Processing (NLP), Transformer-based embeddings, FAISS vector search, and Large Language Models (LLMs) to analyze news articles, retrieve relevant information, and generate explanations along with confidence scores.

##  Features

- **News Analysis:** Analyze user-provided news content.
- **NLP Preprocessing:** Clean and process text for better analysis.
- **Text Chunking:** Split text into manageable chunks for retrieval.
- **Transformer Embeddings:** Convert text into vector representations using transformer models.
- **FAISS Vector Database:** Store and search embeddings efficiently.
- **Retrieval-Augmented Generation (RAG):** Retrieve relevant information to support the analysis.
- **AI Classification:** Classify news content as Real or Fake.
- **Explainable Results:** Generate explanations for the classification.
- **Confidence Score:** Provide an AI-generated confidence estimate.

##  System Architecture

```text
User Input (News Article)
        |
        v
   NLP Preprocessing
        |
        v
     Text Chunking
        |
        v
 Transformer Embeddings
        |
        v
 FAISS Vector Database
        |
        v
 Relevant Information Retrieval
        |
        v
       LLM
        |
        v
  News Classification
        |
        v
 Real / Fake + Explanation + Confidence
```

##  Technologies Used

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Streamlit | User interface |
| LangChain | RAG pipeline orchestration |
| Hugging Face / Sentence Transformers | Text embeddings |
| FAISS | Vector storage and similarity search |
| Ollama | Local LLM integration |
| NLP | Text preprocessing and analysis |
| PyPDF2 | PDF text extraction (if applicable) |

##  Workflow

1. **User Input:** The user submits a news article or news content.
2. **Text Preprocessing:** The input text is cleaned and prepared using NLP techniques.
3. **Text Chunking:** The text is divided into smaller chunks.
4. **Embedding Generation:** Transformer models convert text chunks into vector embeddings.
5. **Vector Storage:** The embeddings are stored in a FAISS vector database.
6. **Information Retrieval:** The retriever searches for relevant information from the indexed knowledge base.
7. **LLM Analysis:** The LLM analyzes the input news alongside the retrieved information.
8. **Result Generation:** The system generates a classification, explanation, and confidence estimate.

##  Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/AI-Fake-News-Detection-RAG.git
```

```bash
cd AI-Fake-News-Detection-RAG
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

Activate it on
