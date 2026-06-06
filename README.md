# 🚀 RAG (Retrieval-Augmented Generation) Application
Import Theses Two Flows Inside Your Langflow Container and add the api Key's and MonogDB Connection String and You are Ready to go.... 🚀
## 📖 Overview
This repository contains a **Retrieval-Augmented Generation (RAG)** application built in LangFlow to dynamically enhance large language models (LLMs) by allowing them to access and retrieve external data sources in real-time [1]. 

This project was developed as the final implementation for the **Advanced Gen-AI Development** course at the **Information Technology Institute (ITI)**, instructed by Eng.

By utilizing a RAG architecture, this application avoids the limitations of static foundation models and ensures that the generated responses are highly context-aware, accurate, and up-to-date without the need for extensive model fine-tuning [3].

## ✨ Key Features & Data Pipeline
The application follows a robust data pipeline flow to supply grounding data for the AI:

1. **Document Processing & Chunking:** Breaks down large, unstructured documents into smaller, semantically relevant parts that represent single ideas or concepts [4, 5].
2. **Metadata Enrichment:** Adds metadata fields (such as titles, summaries, and keywords) to the categorized chunks to improve searchability [5].
3. **Vector Embeddings:** Utilizes mathematical embedding models to convert text chunks and metadata into dense high-dimensional vectors, capturing their semantic meaning [5-7].
4. **Vector Storage:** Persists the generated embeddings in a vector database for extremely fast similarity searches [5, 6, 8].
5. **Query Processing & Generation:** Upon receiving a user query, the application calculates the embedding similarity, fetches the nearest neighbor text from the database, and augments the LLM prompt to generate a factual, context-based answer [4, 6, 7].

## 🛠️ Technology Stack
* **Language/Framework:** Python [9, 10] 
* **AI Orchestration:** LangChain  - utilized to build modular chains of operations and seamlessly connect LLMs to external tools .
* **Embeddings & LLM:**  Hugging Face Open-Source Models .
* **Vector Database:** MongoDB - used to store unstructured data as vector embeddings .

🎓 Acknowledgments
Institution: Information Technology Institute (ITI)
Course: Developing Gen-AI based software engineering

