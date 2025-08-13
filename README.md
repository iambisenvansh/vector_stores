# vector_stores
LangChain IPL Vector Store with Gemini
Description
This repository provides a hands-on example of how to build a simple Vector Store using LangChain, Google's Gemini embeddings, and ChromaDB. The project demonstrates the core concepts of a Retrieval-Augmented Generation (RAG) pipeline by creating a vector database of IPL player data. It covers document loading, embedding generation, similarity search, and metadata filtering.

The code is presented in a Jupyter Notebook, making it easy to follow and experiment with each step of the process.

Features
Document Creation: Learn how to create LangChain Document objects with content and metadata.

Gemini Embeddings: Uses the GoogleGenerativeAIEmbeddings model to convert text data into vector embeddings.

ChromaDB Integration: Demonstrates how to initialize and use Chroma as an in-memory or persistent vector store.

Similarity Search: Perform semantic searches to find documents most relevant to a given query.

Metadata Filtering: Shows how to use metadata to filter search results, enabling more specific queries.

Document Updates: Includes an example of how to update a document within the vector store.

Getting Started
Follow these steps to set up the project and run the code on your local machine.

Prerequisites
Python 3.8+

A Google Gemini AI API key.

A Jupyter Notebook environment (e.g., JupyterLab or VS Code).

Installation
Clone the repository to your local machine:

Bash

git clone https://github.com/iambisenvansh/langchain_document_loader.git
cd langchain_document_loader
Install the required Python packages using pip. You can see the list of packages in the pip install command from the notebook:

Bash

pip install langchain langchain-google-genai chromadb pypdf langchain-community
Set your Google API Key. This is crucial for using the Gemini embedding model. In a Jupyter Notebook, you can set it directly as an environment variable in the first code cell:

Python

import os
os.environ["GOOGLE_API_KEY"] = "YOUR_API_KEY"
Replace "YOUR_API_KEY" with your actual Gemini API key.

Usage
Open the vector_stores.ipynb notebook in your Jupyter environment.

Run the cells sequentially to see each step of the RAG pipeline in action:

The notebook starts with setting the API key and installing dependencies.

It then creates sample documents for IPL players.

It initializes the Gemini embeddings and a persistent ChromaDB instance.

Finally, it demonstrates various search and filtering operations on the vector store.

Contributing
Contributions are welcome! If you have suggestions or improvements, please feel free to open an issue or submit a pull request.

License
This project is licensed under the MIT License.
