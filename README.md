# RAG_FROM_SCRATCH..EPISODE-1

RAG From Scratch: Episode 1 - Overview & Quickstart
This notebook serves as the first entry in a series dedicated to building Retrieval-Augmented Generation (RAG) systems from the ground up without relying on high-level "magic" abstractions. It covers the core architectural flow: Indexing, Retrieval, and Generation.
<img width="1568" height="769" alt="image" src="https://github.com/user-attachments/assets/b6d09fc8-b293-464e-b1b9-a046c40d82c3" />




🚀 Overview
Standard LLMs are limited by their training data "cutoff" and may hallucinate when asked about private or recent information. This project implements a basic RAG pipeline to bridge that gap by connecting an LLM to external data sources.

🛠️ Tech Stack
Framework: LangChain

Vector Store: ChromaDB

Embeddings: OpenAI Embeddings

LLM: OpenAI (ChatOpenAI)

Environment: Python, Tiktoken (for tokenization), and LangSmith (for tracing)

📖 Key Components
Environment Setup: Configuration for API keys (OpenAI, LangSmith) and necessary package installations.

Indexing:

Loading: Fetching content using WebBaseLoader.

Splitting: Breaking documents into manageable chunks using RecursiveCharacterTextSplitter.

Storing: Converting chunks into vector embeddings and storing them in a local vector database.

Retrieval: Using semantic similarity to find the most relevant document chunks based on a user's question.

Generation: Crafting a prompt that combines the retrieved context with the user's question to generate a grounded response.

🏃 How to Run
Open the notebook in Google Colab or a local Jupyter environment.

Install dependencies:

Bash
pip install langchain langchain_community tiktoken langchain-openai chromadb
Set your OPENAI_API_KEY in the environment variables section.

Execute the cells to walk through the basic "Quickstart" RAG pipeline.

Created by: John Mwendwa
