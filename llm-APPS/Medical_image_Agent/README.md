# 🩻 Medical Imaging Diagnosis Agent: Your AI-Powered Radiology Assistant ✨

[![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://your-streamlit-app-url-here)  <!-- Replace with your Streamlit sharing URL if you have one -->

This project brings to life a cutting-edge Medical Imaging Diagnosis Agent, built on the blazing-fast **Gemini 2.0 Flash** model (via `agno`)!  Think of it as your AI-powered radiology assistant, ready to provide insightful analysis of a wide range of medical images.  🚀

![Medical Imaging GIF](https://media.giphy.com/media/xUA7aUxCScDJLTwemA/giphy.gif) <!--  Replace with a relevant GIF.  This one is a general medical scan GIF. Find one specific to your supported modalities (X-ray, MRI, etc.) if possible. -->

## Features That Make It Awesome 🤩

This agent isn't just a simple image viewer; it's packed with features designed to provide a comprehensive and informative analysis:

*   **Comprehensive Image Analysis:**  We go deep, covering everything from basic identification to subtle abnormality detection.
*   **Image Type Identification:**  Instantly recognizes the imaging modality:
    *   🦴 **X-ray**
    *   🧠 **MRI**
    *   🫁 **CT Scan**
    *   🤰 **Ultrasound**
*   **Anatomical Region Detection:**  Pinpoints the specific body part being imaged (e.g., "Chest," "Left Knee," "Brain").
*   **Key Findings and Observations:**  Provides a clear, structured summary of what the AI sees, including:
    *   Systematic listing of visual observations.
    *   Detailed descriptions of image appearance.
    *   Highlights areas that *might* indicate abnormalities.  🚩
*   **Potential Abnormalities Detection:**  Identifies potential issues that warrant further investigation (but *always* consult a doctor!).
*   **Image Quality Assessment:**  Evaluates the quality of the image to ensure reliable analysis.  Is it blurry?  Is there artifact?  The agent will let you know! ✅
*   **Research and Reference:**  (Future Enhancement - Good to mention!)  We're planning to integrate links to relevant medical literature and resources. 📚

## How to Run 🏃‍♀️🏃‍♂️

Getting started is a breeze!  Follow these simple steps:

### Setup Environment

1.  **Clone the Repository:**  Get the code onto your machine.

    ```bash
    git clone https: *********
    cd ai_agent_tutorials/ai_medical_imaging_agent
    ```

2.  **Install Dependencies:**  Install the necessary Python packages.

    ```bash
    pip install -r requirements.txt
    ```

### Configure API Keys

1.  **Get Your Google API Key:**  Head over to [Google AI Studio](https://ai.google.dev/) and grab your API key.  It's like the secret handshake to access Gemini's power. 🔑

2.  **Set the API Key (Important!)**:  You'll need to set your API key as an environment variable or configure it within the application (the exact method depends on how `ai_medical_imaging.py` is structured). A common way is to add it to a `.env` file:

    ```
    GOOGLE_API_KEY=your_actual_api_key_here
    ```
    And then load it in your Python script:
    ```python
    import os
    from dotenv import load_dotenv

    load_dotenv()
    api_key = os.getenv("GOOGLE_API_KEY")
    ```
    Or, you might directly input it into a Streamlit text input field within the app.

### Run the Application

1.  **Launch the Streamlit App:**  Fire up the interactive interface!

    ```bash
    streamlit run ai_medical_imaging.py
    ```

    This will open a new tab in your web browser.  You're ready to upload images!

## Analysis Components (A Deeper Dive) 🕵️‍♀️

Here's a breakdown of what the agent analyzes and how it presents the information:

### Image Type and Region

*   **Identifies Imaging Modality:**  Determines whether it's an X-ray, MRI, CT scan, or ultrasound.
*   **Specifies Anatomical Region:**  Identifies the body part shown in the image.

### Key Findings

*   **Systematic Listing of Observations:**  Provides a structured list of what the AI "sees" in the image.
*   **Detailed Appearance Descriptions:**  Offers descriptions of the textures, shapes, and densities observed.
*   **Abnormality Highlighting:**  Flags areas that *potentially* deviate from the norm.

### Diagnostic Assessment

*   **Potential Diagnoses Ranking:**  Offers a list of possible diagnoses, ranked by likelihood (based on the AI's analysis).
*   **Differential Diagnoses:**  Considers alternative explanations for the findings.
*   **Severity Assessment:**  Provides an indication of the potential severity of any identified issues (e.g., "Mild," "Moderate," "Severe").  This is a *very* important area where you need to be extra cautious and emphasize that it's NOT a definitive diagnosis.

### Patient-Friendly Explanations 🗣️

*   **Simplified Terminology:**  Avoids complex medical jargon, making the information accessible to non-experts.
*   **Detailed First-Principles Explanations:**  Breaks down the findings in a step-by-step manner.
*   **Visual Reference Points:**  (Future Enhancement) Ideally, the app would eventually highlight areas on the image corresponding to the explanations.

## Important Notes ⚠️

*   **Powered by Gemini 2.0 Flash:**  This agent leverages the speed and efficiency of Google's Gemini 2.0 Flash model. ⚡
*   **Requires Stable Internet Connection:**  You'll need to be online to use the agent.
*   **Free API Usage (with Limits):**  You get 1,500 free requests per day thanks to Google!  🎉  Be mindful of usage.
*   **Educational and Development Purposes ONLY:**  This tool is intended for learning and experimentation.  It is **NOT** a substitute for professional medical advice.
*   **NOT a Replacement for Professional Medical Diagnosis:**  This cannot be stressed enough.  Always consult with a qualified healthcare professional.

## Disclaimer 📜

This tool is provided for educational and informational purposes only.  All analyses generated by this agent should be reviewed and interpreted by qualified healthcare professionals.  **Do not make any medical decisions based solely on the output of this tool.**  The developers are not responsible for any actions taken based on the information provided by this agent.
