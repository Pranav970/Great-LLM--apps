# 📠 RAG Agent with Database Routing

A Streamlit application that demonstrates an advanced implementation of RAG Agent with intelligent query routing. The system combines multiple specialized databases with smart fallback mechanisms to ensure reliable and accurate responses to user queries.

## ✨ Features

- **Document Upload**: Users can upload multiple PDF documents related to a particular company. These documents are processed and stored in one of the three databases: Product Information, Customer Support & FAQ, or Financial Information.
- **Natural Language Querying**: Users can ask questions in natural language. The system automatically routes the query to the most relevant database using a phidata agent as the router.
- **RAG Orchestration**: Utilizes Langchain for orchestrating the retrieval augmented generation process, ensuring that the most relevant information is retrieved and presented to the user.
- **Fallback Mechanism**: If no relevant documents are found in the databases, a LangGraph agent with a DuckDuckGo search tool is used to perform web research and provide an answer.

## 🚀 How to Run?

1. **Clone the Repository:**
   ```bash
   git clone 
   cd rag_tutorials/rag_database_routing
```
