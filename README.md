# Article Retrieval System (ARS)

## Introduction
This Article Retrieval System (ARS) leverages advanced NLP techniques and efficient similarity search algorithms to find and recommend articles based on textual queries. Using BERT for embeddings, PCA for dimensionality reduction, and FAISS for quick nearest neighbor searching, ARS provides an efficient and scalable solution for navigating large datasets of articles.

## Features
1. **Text Embedding**: Converts article titles and texts into dense vector representations.
2. **Dimensionality Reduction**: Uses PCA to reduce the dimensionality of the embeddings, enhancing search efficiency.
3. **Efficient Search**: Utilizes FAISS, an efficient library for similarity search, to quickly find the most relevant articles.
4. **Customizable Querying**: Allows querying with adjustable number of results (k-nearest articles).

## Prerequisites
- Python 3.9+
- Libraries: `transformers`, `safetensors`, `langchain`, `chromadb`, `faiss-cpu`, `nltk`, `bitsandbytes`, `pandas`, `sklearn`, `tiktoken`, `sentence-transformers`, `torch`, `accelerate`


> **Warning:** After installing the `accelerate` library, you may need to restart your kernel to ensure that all changes are properly applied. This is necessary to load the newly installed packages into the working environment.

## Usage

### Prepare your dataset:
Ensure your dataset is in a CSV format with at least the columns `Title` and `Text`. At the start of the code, add the path to the CSV file and offload path.

### Set up the environment:
Load the necessary models and preprocess your data.

### Run the embedding and PCA setup:
Execute the initial scripts to transform your article data into a searchable index.

### Query articles:
Use the `search_articles` function to find articles similar to a given query.


### RAG
Use the `generate_responce` function to get respnse using RAG implementation



