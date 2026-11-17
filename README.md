# Advanced Agentic RAG System

An Agentic Retrieval-Augmented Generation (RAG) system built using Python, Groq LLM, and ChromaDB. The project combines document retrieval, LLM-based chunk enrichment, and agent tool calling to answer questions using a company policy document.

## Project Overview

This project demonstrates how an AI agent can retrieve relevant information from documents before generating an answer.

The system uses both original and enriched document chunks to improve retrieval and combines the results using Reciprocal Rank Fusion (RRF).

## Key Features

- Document loading and chunking
- LLM-based chunk enrichment
- Vector storage and retrieval using ChromaDB
- Original and enriched document retrieval
- Reciprocal Rank Fusion (RRF)
- Tool calling using Groq LLM
- Agentic RAG workflow
- Source-aware answers based on retrieved context
- Clear handling of questions not covered by the document

## Project Workflow

1. Load the company policy document.
2. Split the document into smaller chunks.
3. Enrich chunks using an LLM by generating summaries, keywords, and topics.
4. Store original and enriched chunks in separate ChromaDB collections.
5. Retrieve relevant chunks from both collections.
6. Combine retrieval results using Reciprocal Rank Fusion (RRF).
7. Expose retrieval functionality through a search tool.
8. Allow the AI agent to call the search tool and generate responses.

## Technology Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Groq API | LLM inference |
| GPT-OSS-20B | Language model |
| ChromaDB | Vector database |
| Reciprocal Rank Fusion | Combining retrieval results |
| Google Colab | Development environment |

## Dataset

The project uses a fictional employee company policy handbook:

`sample_company_policy_for_rag.txt`

The document is created for testing and demonstration purposes.

## How to Run

1. Clone or download this repository.
2. Open `Advanced_Agentic_RAG_System.ipynb` using Google Colab.
3. Upload `sample_company_policy_for_rag.txt` to the Colab Files panel.
4. Add your Groq API key to Google Colab Secrets using the name `Groq`.
5. Run the notebook from the beginning.

**Important:** Never hardcode your API key or upload it to GitHub.

## Example Use Cases

- Ask questions about company policies.
- Retrieve relevant information from employee documents.
- Identify information that is not available in the source document.
- Answer general questions separately from company-specific information.

## Learning Outcomes

Through this project, I explored:

- Retrieval-Augmented Generation (RAG)
- Vector databases and embeddings
- LLM-based document enrichment
- Hybrid retrieval techniques
- Reciprocal Rank Fusion
- LLM tool calling
- Agentic AI workflows

## Future Improvements

- Add support for multiple documents.
- Improve retrieval accuracy through evaluation.
- Add a user-friendly interface.
- Implement conversation memory and additional agent capabilities.

---

**Note:** This is a learning and demonstration project built to explore Agentic RAG concepts and practical LLM applications.
