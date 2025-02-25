Certainly! Below is the README.md formatted for your GitHub repository:

markdown
Copy
# 📠 RAG Agent with Database Routing

This is a Streamlit application that demonstrates an advanced implementation of the Retrieval-Augmented Generation (RAG) Agent with intelligent query routing. The system combines multiple specialized databases with smart fallback mechanisms to ensure reliable and accurate responses to user queries.

## ✨ Features

- **Document Upload**: Users can upload multiple PDF documents related to a particular company. These documents are processed and stored in one of the three databases:
  - Product Information
  - Customer Support & FAQ
  - Financial Information
- **Natural Language Querying**: Users can ask questions in natural language. The system automatically routes the query to the most relevant database using a `phidata` agent as the router.
- **RAG Orchestration**: Utilizes Langchain for orchestrating the retrieval-augmented generation process, ensuring that the most relevant information is retrieved and presented to the user.
- **Fallback Mechanism**: If no relevant documents are found in the databases, a LangGraph agent with a DuckDuckGo search tool is used to perform web research and provide an answer.

## 🚀 How to Run?

### 1. Clone the Repository:
```bash
git clone ******
cd rag_tutorials/rag_database_routing
```
2. Install Dependencies:
```bash
pip install -r requirements.txt
```
3. Run the Application:
```bash
streamlit run rag_database_routing.py
```

# 4. Get OpenAI API Key:
Obtain an OpenAI API key and set it in the application. This is required for initializing the language models used in the application.

## 5. Setup Qdrant Cloud:
- Visit Qdrant Cloud
- Create an account or sign in.
- Create a new cluster.
- Get your credentials:
- Qdrant API Key: Found in the API Keys section.
- Qdrant URL: Your cluster URL (format: https://xxx-xxx.aws.cloud.qdrant.io).
  
# 6. Upload Documents:
Use the document upload section in the app to add PDF documents to the desired database.

# 7. Ask Questions:
Enter your questions in the query section. The application will route your question to the appropriate database and provide an answer.

# 🛠️ Technologies Used
**Langchain**: For RAG orchestration, ensuring efficient retrieval and generation of information.
**Phidata Agent**: Used as the router agent to determine the most relevant database for a given query.
**LangGraph Agent**: Acts as a fallback mechanism, utilizing DuckDuckGo for web research when necessary.
**Streamlit**: Provides a user-friendly interface for document upload and querying.
**Qdrant**: Used for managing the databases, storing, and retrieving document embeddings efficiently.

# 🔍 How It Works?
# Query Routing:
The system uses a three-stage routing approach:

- 1. **Vector Similarity Search**: Queries are checked against embeddings in all databases.
- 2. **LLM-based Routing**: For ambiguous queries, a language model is used to route to the correct database.
- 3. **Web Search Fallback**: If the query cannot be answered from the databases, a web search is performed via DuckDuckGo.
     
# Document Processing:
- Text Extraction: Automatic text extraction from PDFs.
- Text Chunking: Smart text chunking with overlap to maintain context.
- Vector Embedding Generation: Embeddings are generated for efficient document retrieval.
- Database Storage: Efficient storage and retrieval of embeddings in Qdrant.

# Answer Generation:
- Context-Aware Retrieval: Ensures relevant context is used for answering queries.
- Smart Document Combination: Combines information from relevant documents to form a complete answer.
- Confidence-Based Responses: Provides answers based on confidence scores.
- Web Research Integration: If needed, integrates information from the web to enhance the answer.

