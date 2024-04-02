# vector-rerank-search-solution

## Overview

**vector-rerank-search-solution** is a state-of-the-art search optimization tool that elevates the standard of search results through the integration of vector search and AI-driven re-ranking. By harnessing the power of Weaviate's vector search engine alongside Cohere's natural language processing models, this project delivers unparalleled search precision and relevance. Ideal for developers and researchers, it's a pivotal tool for anyone aiming to implement or enhance search functionalities with advanced optimization techniques.

## Features

- **Vector Search**: Leverages Weaviate to perform semantic search, allowing for more accurate matching based on the meaning of queries and documents.
- **AI Re-Ranking**: Utilizes Cohere's re-ranking model to refine search results, ensuring the most relevant results are prioritized.
- **Language Understanding**: Employs advanced NLP models for a deeper understanding of query context and content semantics.
- **Customizable Parameters**: Offers flexibility in search settings, including language preference and result limits, to suit various needs.
- **Easy Integration**: Designed for straightforward implementation into existing projects, enhancing search capabilities with minimal setup.

## Getting Started

### Prerequisites

Ensure you have Python 3.8+ installed on your system. Additionally, you will need API keys for both Weaviate and Cohere. You can also use the API keys offered below for free.

### Installation

1. Clone the repository:

```bash
git clone https://github.com/Shining-in-galaxies/vector-rerank-search-solution.git
```

2. Navigate to the project directory:

```bash
cd vector-rerank-search-solution
```

3. Install the required dependencies:

```bash
pip install -r requirements.txt
```

### Usage

1. Start by setting up your `.env` file with your Weaviate and Cohere API keys:

```plaintext
COHERE_API_KEY=xVPzQWYsYel6CBukP0nPwPXsPWaFXYZDJCVXxIlP
WEAVIATE_API_KEY='76320a90-53d8-42bc-b41d-678647c6672e'
WEAVIATE_API_URL= 'https://cohere-demo.weaviate. network/'
```

2. Run the script with a query of your choice:

```python
from search_solution import dense_retrieval, rerank_responses

query = "Your search query"
results = dense_retrieval(query, client)
reranked_results = rerank_responses(query, [result['text'] for result in results])

print(reranked_results)
```

## Acknowledgments

- Weaviate, for the vector search engine.
- Cohere, for the natural language processing and re-ranking models.
