## 🧬 Multimodal AI Agent

A Streamlit application that combines video analysis and web search capabilities using Google's Gemini 1.5 pro/flash model. This agent can analyze uploaded videos and answer questions by combining visual understanding with web-search.

### Features

*   Video analysis using Gemini 1.5 pro/flash
*   Web research integration via DuckDuckGo
*   Support for multiple video formats (MP4, MOV, AVI)
*   Real-time video processing
*   Combined visual and textual analysis

### How to get Started?

1.  **Clone the GitHub repository**

    ```bash
    git clone https://github.com/Shubhamsaboo/awesome-llm-apps.git
    cd ai_agent_tutorials/multimodal_ai_agent
    ```

2.  **Install the required dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

3.  **Get your Google Gemini API Key**

    *   Sign up for an [Google AI Studio account](https://ai.google.dev/) and obtain your API key.  **(Important: I've added a direct link to Google AI Studio here.  This is best practice.)**

4.  **Set up your Gemini API Key as the environment variable**

    ```bash
    GOOGLE_API_KEY=your_api_key_here
    ```
    **(Note: Best practice is to use a `.env` file for environment variables, but the image shows it directly in the command line.  I've kept it consistent with the image.  Consider adding a note about using `.env` files for better security.)**

5.  **Run the Streamlit App**

    ```bash
    streamlit run multimodal_agent.py
    ```
