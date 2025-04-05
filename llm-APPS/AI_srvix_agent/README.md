# 📚 AI Research Agent with Memory 🧠✨ <img src="https://img.shields.io/badge/AI%20Powered-GPT--4o--mini-blueviolet.svg" alt="AI Powered Badge"/> <img src="https://img.shields.io/badge/Memory-Mem0%20%26%20Qdrant-orange.svg" alt="Memory Badge"/>

Tired of endless searches and losing track of relevant academic papers? 🤯 Meet your new **AI Research Assistant!** 🚀

This intelligent Streamlit application transforms how you interact with arXiv. It doesn't just *find* papers; it **learns your interests**, remembers your past searches, and presents information in a way that's easy to digest. Think of it as your personal librarian with a super-powered AI brain! 🤖💡

Powered by **OpenAI's GPT-4o-mini**, enhanced with **Mem0 & Qdrant** for persistent memory, this agent makes academic research faster, smarter, and more personalized. 📈

---

## ✨ Features That Will Revolutionize Your Research Workflow ✨

*   **🔍 Smart arXiv Search:** Go beyond simple keywords. Query arXiv intelligently and get relevant results faster.
*   **📄 AI-Enhanced Readability:** Say goodbye to dense abstracts! GPT-4o-mini processes search results, summarizing and highlighting key points for quick understanding. ✨
*   **🧠 Persistent Memory:** This is the magic! The agent remembers your interests and past searches using Mem0 & Qdrant, making future searches increasingly relevant and personalized. It *knows* what you're looking for! 🤯
*   **💡 Powered by GPT-4o-mini:** Leverages OpenAI's cutting-edge model for sophisticated natural language understanding and processing.
*   **💾 Memory Magic with Mem0 & Qdrant:** Seamlessly integrates advanced memory storage and retrieval, ensuring your research context is never lost. 🪄
*   *(Optional: MultiOn Integration for advanced web interactions related to research - if implemented)*

---

## ⚙️ Requirements: What You Need to Get Started ⚙️

Before unleashing your AI research partner, make sure you have the following:

### 🐍 Python & Libraries:

*   Python 3.x installed
*   The following Python libraries (install via `requirements.txt`):
    *   `streamlit` 🎈 (For the interactive UI)
    *   `openai` 🤖
    *   `mem0ai` 🧠
    *   `qdrant-client` 💾
    *   `arxiv` 📄
    *   *(Add any other specific libraries from requirements.txt)*

### 🐳 Services:

*   **Qdrant:** A running instance of the Qdrant vector database. Docker is the easiest way! (See instructions below). The app expects it at `localhost:6333` by default.

### 🔑 API Keys:

*   **OpenAI API Key:** To power the GPT-4o-mini model. Get yours from [OpenAI Platform](https://platform.openai.com/api-keys).
*   *(Optional: MultiOn API Key if MultiOn features are used)*
*   **Tip:** For security, it's best to set these as environment variables or use Streamlit's secrets management (`.streamlit/secrets.toml`).

---

## 🚀 Get Started: Unleash the Agent! 🚀

Follow these steps to set up and run your AI Research Agent:

1.  **Clone the Repository:** Get the code onto your machine. 💾
    ```bash
    git clone https://github.com/Shubhamsaboo/awesome-llm-apps.git
    ```

2.  **Navigate to the Directory:** Enter the project folder. 📂
    ```bash
    cd awesome-llm-apps/llm_apps_with_memory_tutorials/ai_arxiv_agent_memory
    ```

3.  **Install Dependencies:** Let pip handle the library installations. ⚙️
    ```bash
    pip install -r requirements.txt
    ```

4.  **Run Qdrant with Docker:** Get your vector database running! 🐳
    *   **Pull the image:**
        ```bash
        docker pull qdrant/qdrant
        ```
    *   **Run the container (with persistent storage):**
        ```bash
        docker run -p 6333:6333 -p 6334:6334 \
            -v $(pwd)/qdrant_storage:/qdrant/storage:z \
            qdrant/qdrant
        ```
        *(This creates a `qdrant_storage` directory in your current folder to save data. Ensure Docker has permissions to write here. Adjust the path if needed.)*
    *   **Verify:** Check if Qdrant is accessible at `http://localhost:6333`.

5.  **Set Up API Keys:** Make sure your OpenAI (and potentially MultiOn) API key is accessible to the application (e.g., environment variable `OPENAI_API_KEY` or via Streamlit secrets). 🔑

6.  **Run the Streamlit App:** Launch the research agent! ✨ ▶️
    ```bash
    streamlit run ai_arxiv_agent_memory.py
    ```

    Your browser should automatically open the Streamlit interface. Start searching and watch the AI learn! 🎉

---

Happy Researching! 🧑‍🔬🔬💡
