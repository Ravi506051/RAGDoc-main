# RAGDoc — Document Question Answering

RAGDoc is a document-assistant project exploring Retrieval-Augmented Generation (RAG) for finding relevant information and answering questions grounded in uploaded or indexed documents.

## Core workflow
1. Load and parse supported documents.
2. Split extracted text into searchable chunks.
3. Generate embeddings for the chunks.
4. Retrieve relevant passages for a question.
5. Provide retrieved context to a language model.
6. Return a context-aware response.

## Technology areas
Python · Retrieval-Augmented Generation · Embeddings · Large Language Models · NLP

Check the dependency files and application source for the exact parser, vector store, model provider and user interface configured in this repository.

## Getting started
```bash
git clone https://github.com/Ravi506051/RAGDoc-main.git
cd RAGDoc-main
python -m venv .venv
# Windows: .venv\\Scripts\\activate
pip install -r requirements.txt
```
Run the entry point documented in the project after configuring any required model credentials.

## Evaluation
Measure retrieval relevance separately from answer quality. Test questions with no supporting passage, long documents, duplicate content and malformed files. Prefer answers that cite or identify their supporting source passages.

## Security
Treat uploaded documents as private data. Validate file types and sizes, isolate document processing and never expose credentials or document contents in logs.

## Future improvements
Add page-level citations, retrieval benchmarks, configurable chunking, persistent indexing and document-level access controls.

## Maintainer
**Ravi Kumar Rao** · [GitHub](https://github.com/Ravi506051)
