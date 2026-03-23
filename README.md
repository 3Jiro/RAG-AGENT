# 🔍 RAG Agent: Intelligent Knowledge Retrieval (Pinecone + Gemini)
### 🌟 Overview
An end-to-end Retrieval-Augmented Generation (RAG) pipeline that transforms static documentation into a dynamic, queryable knowledge base. This project focuses on the Ingestion-to-Insight lifecycle, ensuring the AI only answers based on verified internal data.

### 🛠️ Technical Architecture
- **Vector Embeddings:** Uses text-embedding-004 to convert Google Drive documents into high-dimensional vectors stored in a Pinecone index.

- **Semantic Search Protocol:** Implemented a "Vector Store Tool" that performs similarity searches to retrieve the most relevant 1,000-character chunks for every query.

- **Recursive Character Splitting:** Optimized document chunking with a 100-character overlap to preserve semantic context across boundaries.

### 🚀 Key Challenges Overcome
- **Retrieval Noise:** Fine-tuned the Top-K retrieval parameters to balance between comprehensive context and LLM token limits.

- **Document Syncing:** Automated the pipeline to trigger a re-index whenever a new file is added to the linked Google Drive folder.

### ⚙️ Tech stack
- **Primary Engine:** n8n (self hosted) / Langchain
- **AI/LLM:** Gemini/OpenAI + Pinecone
- **Data & storage:** Google drive
- **Communication:** Chat UI
