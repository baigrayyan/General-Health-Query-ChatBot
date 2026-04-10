# General-Health-Query-ChatBot

## Objective
This project demonstrates how to build a simple chatbot using OpenAI's GPT-3.5 model. The chatbot is designed to provide general, factual information about health-related questions in a friendly and clear manner, while strictly avoiding medical advice, diagnoses, or treatment recommendations.

### Features
-   **Prompt Engineering:** Utilizes prompt engineering to establish a persona for the chatbot as a helpful medical assistant.
-   **Safety Filters:** Incorporates explicit instructions within the prompt to prevent the chatbot from offering medical advice and to always recommend consulting a qualified healthcare professional.
-   **Interactive Console:** Provides a simple command-line interface for users to interact with the chatbot.

### Setup Instructions
To run this chatbot, you'll need an OpenAI API key and access to Google Colab.

1.  **Obtain an OpenAI API Key:**
    *   Go to [OpenAI API Keys](https://platform.openai.com/account/api-keys).
    *   Create a new secret key.

2.  **Add API Key to Colab Secrets:**
    *   In your Google Colab notebook, locate the '🔑' icon (Secrets) in the left-hand panel.
    *   Click on it and add a new secret.
    *   Name the secret `OPENAI_API_KEY` (this name is crucial as the code specifically looks for it).
    *   Paste your OpenAI API key as the value for this secret.

3.  **Install Dependencies:**
    *   Ensure the `openai` library is installed. The first code cell in this notebook (`pip install openai`) handles this.

### How to Run
1.  **Execute the cells sequentially:** Run the `pip install openai` cell first.
2.  **Run the main chatbot code:** Execute the code cell that imports `openai` and defines the `get_health_response` function, followed by the `while True` loop.
3.  **Interact with the Chatbot:** Once the code is running, you will see a prompt "Your question: ". Type your health-related questions there. To exit the chatbot, type `quit`.

### Example Queries
*   "What are the symptoms of the common cold?"
*   "How can I improve my sleep hygiene?"
*   "What is a balanced diet?"

### Important Disclaimer
This chatbot is for informational purposes only and *does not* provide medical advice. Always consult a qualified healthcare professional for any medical concerns, diagnoses, or treatment.
