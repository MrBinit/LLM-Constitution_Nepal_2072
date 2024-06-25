# Legal LLM for the Constitution of Nepal

## Overview

This project introduces a specialized Legal Language Model (LLM) designed to provide accurate and insightful responses to queries related to the Constitution of Nepal. By harnessing the power of Retrieval Augmented Generation (RAG), we combine the vast knowledge of the Nepalese Constitution with the advanced language understanding of the LLAMA 3 70B model. This enables users to interact with the constitution in a natural, conversational manner.

## Key Features

- **Legal Expertise:**  Fine-tuned on the entire Constitution of Nepal for domain-specific understanding.
- **RAG-Powered:**  Employs Retrieval Augmented Generation to provide contextually relevant and legally sound answers.
- **State-of-the-Art:** Utilizes cutting-edge technologies like LLAMA 3, sentence transformers, and vector databases.
- **User-Friendly:** Accessible through an intuitive ChatGroq interface.

## Technical Implementation

1. **Data Preparation:**
   - The Constitution of Nepal is parsed and structured using `llama parse`.

2. **Embedding Model:**
   - `BAAI/bge-base-en-v1.5` is used to generate high-quality embeddings for both constitutional text and user queries.

3. **Vector Database:**
   - `Qdrant` stores the embeddings and facilitates efficient similarity searches.

4. **Reranking and Compression:**
   - `FlashrankRerank` with the `ms-marco-MiniLM-L-12-v2` model improves relevance ranking.
   - Compression techniques optimize storage and retrieval.

5. **Chat Interface:**
   - `ChatGroq` provides a seamless conversational experience.

