# RAG_ChatBot-
A Retrieval-Augmented Generation (RAG) chatbot designed to provide context-aware answers by grounding responses in real website data. Scrapes website data, generates semantic embeddings with HuggingFace Sentence Transformers, stores vectors in ChromaDB, and delivers context-grounded, low-hallucination responses using Groq LLM and prompt engineering.

**RAG Chatbot for Retrieval of Data from Website** 

This project implements a Retrieval-Augmented Generation (RAG) chatbot designed to provide accurate, context-aware answers by grounding responses in data collected from websites. The system combines semantic search with large language models to reduce hallucinations and improve reliability.

**Overview** 
Traditional large language models may generate responses that are incorrect or not supported by verified sources. This project addresses that limitation by retrieving relevant information from trusted website data before generating responses.
The chatbot scrapes website content, processes it into vector embeddings, retrieves the most relevant information for a given query, and generates structured answers using a large language model.

**System Architecture** 
-> Data Ingestion
   Website content is loaded using LangChain web loaders and split into manageable text chunks.
-> Embedding Generation
   Text chunks are converted into semantic embeddings using HuggingFace Sentence Transformers.
-> Vector Storage
   Embeddings are stored in ChromaDB to enable efficient similarity-based retrieval.
-> Retrieval
   Relevant document chunks are retrieved from the vector database based on semantic similarity to the user query.
-> Answer Generation
   Retrieved context is passed to a Groq-powered large language model using controlled prompts to generate accurate and readable responses.

**Technology Stack** 
-> Programming Language: Python
-> Framework: LangChain
-> Vector Database: ChromaDB
-> Embeddings: HuggingFace Sentence Transformers
-> Large Language Model: Groq (LLaMA-based models)
-> Core Concepts: RAG, NLP, Vector Search, Prompt Engineering

**Features** 
Retrieval-Augmented Generation pipeline
Semantic search over website content
Context-grounded responses to minimize hallucinations
Structured and readable outputs using prompt engineering
Modular and extensible design

**Getting Started** 

Prerequisites
Python 3.10 or 3.11

Virtual environment (recommended)

Installation
pip install -r requirements.txt

Run the Application
python main.py

**Use Cases** 
1. Website-based question answering systems
2. Healthcare information assistants
3. Domain-specific knowledge retrieval
4. Enterprise and educational chatbots
5. Why Retrieval-Augmented Generation
6. By grounding responses in retrieved website data, the system:
7. Improves factual accuracy
8. Reduces hallucinations
9. Ensures transparency and trust
10. Future Enhancements
11. Support for multiple websites and document formats
12. Web-based user interface
13. Metadata-based and hybrid retrieval
14. Evaluation metrics for retrieval performance

**Author** 
Saanvi M S
Computer Science and Business Systems Undergraduate
