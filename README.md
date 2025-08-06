# Word2Vec with t-SNE Visualization

A comprehensive implementation for training Word2Vec embeddings and visualizing them using both custom and scikit-learn t-SNE algorithms. This project demonstrates natural language processing, word embeddings, and dimensionality reduction techniques.

## Overview

This project combines word embedding generation with advanced visualization techniques to understand semantic relationships between words in text data. It includes both a custom implementation of t-SNE and comparison with scikit-learn's implementation.

## Features

### 1. Text Preprocessing Pipeline
- **Data Loading**: Extracts and processes text from ZIP archives
- **Text Cleaning**: Removes punctuation, converts to lowercase, and filters stopwords
- **Tokenization**: Breaks text into individual words using NLTK
- **Corpus Building**: Structures text into sentences for Word2Vec training

### 2. Word2Vec Embedding Training
- **Custom Training**: Trains Word2Vec models on preprocessed text corpus
- **Configurable Parameters**: Adjustable vector dimensions, window size, and minimum word count
- **Semantic Learning**: Captures semantic relationships between words in vector space

### 3. Custom t-SNE Implementation
- **From-Scratch Algorithm**: Complete implementation of t-SNE dimensionality reduction
- **Batch Processing**: Efficient processing of large datasets using batch operations
- **Customizable Parameters**: Adjustable perplexity, learning rate, and iterations
- **Gradient Computation**: Implements the core t-SNE gradient descent algorithm

### 4. Visualization System
- **2D Plotting**: Creates scatter plots of word embeddings in reduced dimensions
- **Interactive Labels**: Annotates points with corresponding words
- **Comparison Views**: Side-by-side visualization of custom vs scikit-learn results
- **Semantic Clustering**: Reveals semantic clusters and relationships visually

### 5. Word Similarity Analysis
- **Semantic Search**: Finds most similar words based on vector similarity
- **Relationship Discovery**: Explores word associations and contexts
- **Model Validation**: Verifies embedding quality through similarity queries

## Prerequisites

Ensure you have the following packages installed:

- Python 3.7 or higher
- numpy
- matplotlib
- gensim
- scikit-learn
- nltk
- zipfile (built-in)

## Installation

Install required dependencies:

```bash
pip install numpy matplotlib gensim scikit-learn nltk
```

The project automatically downloads necessary NLTK data:
- punkt tokenizer
- stopwords corpus

## Dataset Requirements

The project expects:
- A ZIP file named 'train.zip' containing text data
- Text file should be UTF-8 encoded
- Sufficient text volume for meaningful word embeddings

## Output and Results

The project generates:
- **Word Embedding Visualizations**: 2D scatter plots showing word relationships
- **Similarity Analysis**: Lists of most similar words for query terms
- **Comparative Results**: Custom vs scikit-learn t-SNE visualizations
- **Interactive Plots**: Matplotlib figures with word annotations

