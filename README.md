# Chatbot_Automation
AI-powered automation project recommendation chatbot using NLP, RAG, FAISS vector search, and a fine-tuned Llama-3.2-3B-Instruct model. The system understands natural language, retrieves relevant automation projects from a custom dataset, and generates conversational, dataset-grounded recommendations using E5 embeddings and QLoRA fine-tuning.
AI-Powered Automation Project Recommendation Chatbot

This project is an intelligent conversational AI chatbot specialized in the automation and industrial automation domain. The system combines Natural Language Processing (NLP), Retrieval-Augmented Generation (RAG), semantic vector search, and a fine-tuned Large Language Model (LLM) to recommend automation projects based on user requirements such as budget, manpower, complexity, duration, ROI, automation level, and required components.

The chatbot was built using Python and developed in Visual Studio Code, while model training and experimentation were performed using Google Colab Pro and Modal AI with GPU acceleration. The project uses a custom dataset containing approximately 2500 automation project records with engineering and business-related attributes including project descriptions, budgets, skills required, risk levels, energy savings, and bill of materials.

To enable conversational AI capabilities, the system uses the meta-llama/Llama-3.2-3B-Instruct model fine-tuned using QLoRA (Quantized Low-Rank Adaptation) for efficient low-memory training. Semantic understanding and retrieval are handled using the intfloat/e5-base-v2 embedding model together with a FAISS vector database for fast similarity search and dataset-grounded responses.

The project architecture follows a modern RAG pipeline:

User Query → E5 Embeddings → FAISS Vector Retrieval → Fine-Tuned Llama-3.2-3B-Instruct → Conversational Response

The chatbot can:

Understand natural language automation requests
Recommend projects based on constraints
Retrieve relevant dataset records
Respond conversationally like an AI assistant
Reduce hallucinations through retrieval grounding
Reject unrelated domain questions politely

The repository includes:

Dataset preprocessing scripts
Excel-to-JSONL conversion tools
Fine-tuning scripts using QLoRA
Vector database generation
Retrieval validation tools
RAG chatbot implementation
4-bit quantized inference scripts

This project demonstrates the integration of NLP, vector databases, RAG, and fine-tuned open-source LLMs to build a scalable and GPU-efficient engineering recommendation assistant.
