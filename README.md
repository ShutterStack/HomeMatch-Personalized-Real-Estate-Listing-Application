# HomeMatch: Personalized Real Estate Listing Application

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen.svg)

## Overview

**HomeMatch** is an innovative Python application designed to enhance the real estate search experience by delivering personalized property listings tailored to individual buyer preferences. Built for "Future Homes Realty" (a simulated forward-thinking real estate company), this project leverages advanced AI technologies to transform standard listings into engaging, buyer-specific narratives. It integrates large language models (LLMs), vector databases, and semantic search to match properties with user needs seamlessly.

### Key Features
- **Listing Generation**: Generates 10 diverse real estate listings with unique attributes, saved as JSON and CSV files.
- **Vector Storage**: Stores listings in ChromaDB for efficient semantic search using embeddings.
- **Preference Processing**: Interprets buyer preferences in natural language and converts them into concise search queries.
- **Personalized Descriptions**: Rewrites listing descriptions to highlight features matching buyer preferences, maintaining factual accuracy.

### Tech Stack
- **Language**: Python 3.9+
- **LLM**: Groq API (llama3-70b-8192 model)
- **Framework**: LangChain (prompt chaining and output parsing)
- **Embeddings**: HuggingFace (all-MiniLM-L6-v2)
- **Vector Database**: ChromaDB
- **Dependencies**: `langchain`, `langchain-groq`, `langchain-chroma`, `chromadb`, `huggingface-hub`, `sentence-transformers`, `pandas`

## Project Structure

The application is implemented in a Google Colab notebook (`HomeMatch.ipynb`) with a modular, five-part workflow:
1. **Setup and Dependencies**: Configures the environment and installs required packages.
2. **Generate Listings**: Creates and saves a dataset of 10 listings.
3. **Initialize Vector Database**: Loads listings into ChromaDB for search functionality.
4. **Collect and Process Preferences**: Gathers buyer preferences and generates a search query.
5. **Search and Personalize**: Performs semantic search and outputs personalized listings.

Each part is preceded by a detailed description in the notebook, explaining its purpose and actions.

## Prerequisites

- **Python**: Version 3.9 or higher (Colab provides this by default).
- **Groq API Key**: Obtain from [Groq Console](https://console.groq.com/) for LLM access.
- **Google Colab**: Recommended for execution, though adaptable to local environments with modifications.

