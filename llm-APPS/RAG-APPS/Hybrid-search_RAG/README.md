# 👀 RAG App with Hybrid Search
## A powerful document Q&A application that leverages Hybrid Search (RAG) and Claude's advanced language capabilities to provide comprehensive answers. Built with RAGLite for robust document processing and retrieval, and Streamlit for an intuitive chat interface, this system seamlessly combines document-specific knowledge with Claude's general intelligence to deliver accurate and contextual responses.

# Features
- Hybrid Search Question Answering

- RAG-based answers for document-specific queries
- Fallback to Claude for general knowledge questions
- Document Processing:

## PDF document upload and processing
- Automatic text chunking and embedding
- Hybrid search combining semantic and keyword matching
- Reranking for better context selection
- Multi-Model Integration:

# Claude for text generation - tested with Claude 3 Opus
- OpenAI for embeddings - tested with text-embedding-3-large
- Cohere for reranking - tested with Cohere 3.5 reranker
# Prerequisites
- You'll need the following API keys and database setup:

Database: Create a free PostgreSQL database at Neon:

Sign up/Login at Neon
Create a new project
Copy the connection string (looks like: postgresql://user:pass@ep-xyz.region.aws.neon.tech/dbname)
API Keys:

OpenAI API key for embeddings
Anthropic API key for Claude
Cohere API key for reranking
How to get Started?
Clone the Repository:

git clone https://github.com/Shubhamsaboo/awesome-llm-apps.git
cd awesome-llm-apps/rag_tutorials/hybrid_search_rag
Install Dependencies:

pip install -r requirements.txt
Install spaCy Model:

pip install https://github.com/explosion/spacy-models/releases/download/xx_sent_ud_sm-3.7.0/xx_sent_ud_sm-3.7.0-py3-none-any.whl
Run the Application:

streamlit run main.py
Usage
Start the application
Enter your API keys in the sidebar:
OpenAI API key
Anthropic API key
Cohere API key
Database URL (optional, defaults to SQLite)
Click "Save Configuration"
Upload PDF documents
Start asking questions!
Document-specific questions will use RAG
General questions will use Claude directly
Database Options
The application supports multiple database backends:

PostgreSQL (Recommended):

Create a free serverless PostgreSQL database at Neon
Get instant provisioning and scale-to-zero capability
Connection string format: postgresql://user:pass@ep-xyz.region.aws.neon.tech/dbname
MySQL:

mysql://user:pass@host:port/db
SQLite (Local development):

sqlite:///path/to/db.sqlite
Contributing
Contributions are welcome! Please feel free to submit a Pull Request.
