# 🛫 AI Travel Agent: Your Personalized Trip Planner! ✨

[![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](your-streamlit-app-url-here) <!-- Replace with your Streamlit sharing URL if you deploy -->

Tired of endless travel planning tabs and overwhelming options?  Say hello to your new AI-powered travel companion!  This Streamlit app, fueled by the incredible **GPT-4o** from OpenAI, crafts personalized travel itineraries, turning your dream vacation into a reality with minimal effort.  🚀

![Travel GIF](https://media.giphy.com/media/3o6Zt481isNVuQIc8g/giphy.gif) <!-- Replace with a fun, relevant travel GIF! -->

## Features That Will Make You Wanderlust 🤩

*   **Research & Discovery:**  Unearth hidden gems and popular hotspots!  The agent researches destinations, activities, and accommodations tailored to your interests. 🏖️🏞️🏛️
*   **Customizable Itineraries:**  Tell us how long you're traveling, and we'll create a plan that fits your schedule perfectly.  From weekend getaways to epic adventures! 🗓️
*   **GPT-4o Powered Intelligence:**  Experience the magic of cutting-edge AI!  Our agent generates smart, personalized travel plans that go beyond basic recommendations. 🤔
*   **Effortless Planning:**  Ditch the spreadsheets and endless research.  Let the AI Travel Agent handle the heavy lifting, so you can focus on the fun! ✈️

## How to Get Started 🗺️

Getting your AI travel assistant up and running is a breeze:

1.  **Clone the Repository:** Grab the code!

    ```bash
    git clone :- **********
    cd awesome-llm-apps/ai_agent_tutorials/ai_travel_agent
    ```

2.  **Install Dependencies:**  Get the necessary Python packages.

    ```bash
    pip install -r requirements.txt
    ```

3.  **API Keys - Your Passport to AI Power! 🔑**

    *   **OpenAI API Key:**
        *   Sign up for an [OpenAI account](https://platform.openai.com/).
        *   Obtain your API key from your account dashboard.
        *   Set the key. You'll likely want to set it as an environment variable. A common method is:
            ```
            OPENAI_API_KEY=your_actual_openai_api_key
            ```
             Or add to .env file

    *   **SerpAPI Key:**
        *   Sign up for a [SerpAPI account](https://serpapi.com/).
        *   Get your API key from your SerpAPI dashboard.
        *    Set the key. Similar to the OpenAI key, use an environment variable:
            ```
            SERPAPI_API_KEY=your_actual_serpapi_key
            ```
            Or add to .env file

    *Important*: These keys are like your digital passport – keep them secure and don't share them publicly!

4.  **Launch the Streamlit App:**  Start planning your adventure!

    ```bash
    streamlit run travel_agent.py
    ```

    This will open the app in your web browser.

## How It Works - Behind the Scenes 🕵️‍♀️

The AI Travel Agent is a dynamic duo of two powerful components:

*   **The Researcher 🧳:**  This diligent agent acts as your personal travel researcher.
    *   **Generates Search Terms:** Based on your destination and trip duration, it crafts intelligent search queries to find the best activities and places to stay.
    *   **Searches the Web:**  Using the SerpAPI, it scours the internet for relevant information, gathering a wealth of travel possibilities.

*   **The Planner 🗓️:** This is the brains behind your itinerary.
    *   **Processes Research:** It takes the results from the Researcher and filters them based on your preferences.
    *   **Generates Draft Itinerary:** It crafts a personalized, draft itinerary, suggesting activities, timings, and potentially even estimated costs (future enhancement!).

##  Technologies Used 💻

* **Streamlit:**  For building the interactive web application.
* **OpenAI GPT-4o:** For generating text, creating itineraries, and personalizing recommendations.
* **SerpAPI:** For performing web searches and retrieving information.
* **Python:** The core programming language.

## Contributing 🤝
Contributions are welcome! If you have ideas for improvements or new features, please feel free to submit a pull request.
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the branch (`git push origin feature/AmazingFeature`).
5. Open a pull request.

## License

This project is licensed under the [MIT License](LICENSE) - see the LICENSE file for details.(Add the License file in the directory.)

## Need help? 🤔

If you encounter any issues or have questions, don't hesitate to open an issue on the GitHub repository.

Have an awesome trip! 🌎✈️
