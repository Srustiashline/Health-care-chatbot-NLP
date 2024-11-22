# HealthCare Chatbot Using NLP

## Overview

This is an AI-powered healthcare chatbot designed to assist users by diagnosing potential health issues based on their symptoms. Using Natural Language Processing (NLP), the chatbot is capable of understanding and processing user input to provide relevant responses, including suggesting possible causes for symptoms like fever and providing general advice.

The chatbot utilizes pre-trained models and a TF-IDF vectorizer to match user inputs with known symptom data, offering personalized responses.

## Features

- **Symptom Detection**: The chatbot identifies common health issues like fever and asks for more details to provide possible diagnoses.
- **Greeting Responses**: It can respond to greetings like "hello" or "hi" and inquire about health status.
- **General Health Advice**: Based on symptoms, the chatbot can give a response, providing suggestions or asking for further information.
- **Interactive**: The bot can keep the conversation flowing and is able to detect when the user is saying goodbye.

## Technologies Used

- **Python**: Primary programming language.
- **NLTK (Natural Language Toolkit)**: For text processing and tokenization.
- **Scikit-learn**: Used for vectorization (TF-IDF) and cosine similarity to match user input with predefined responses.
- **TensorFlow** (commented out for now): Placeholder for future integration with more advanced AI models if needed.
  
## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/healthcare-chatbot-nlp.git
   cd healthcare-chatbot-nlp
   ```
2. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```
3. Download the necessary NLTK datasets:
   ```bash
   import nltk
   nltk.download('punkt')
   nltk.download('wordnet')
   ```
4. Ensure that you have the symptom.txt and pincodes.txt files in the project directory as they are used for identifying symptoms and location-based responses.

## Usage
- Run the chatbot by executing the following command in the terminal:
   ```bash
   python serve.py
   ```
- The bot will greet you and ask if you are experiencing any health issues. If you respond with "yes", it will proceed to ask for symptoms and provide responses based on the information it has.

- You can ask about health-related concerns, and the bot will provide a relevant response based on predefined data. For example, if you mention symptoms like "fever", it will ask further questions about the type of fever and its symptoms.

- To exit the chatbot, simply type "bye" and it will end the conversation.

## How It Works
-  **Greeting**: The chatbot checks if the input matches any greeting keywords.
-  **Basic Query**: If the user responds positively to a health-related query, the bot asks for symptoms.
-  **Symptom Matching**: The chatbot matches the symptoms entered by the user with predefined symptoms to suggest potential health issues.
-  **Cosine Similarity**: It uses cosine similarity to match user inputs with the closest symptom text and provide appropriate responses.
## Snapshot
[HealthCare Chatbot Using NLP]![![Screenshot 2024-11-22 224850](https://github.com/user-attachments/assets/6e5f2959-2cf0-450a-9536-4501186217d3)
](https://github.com/user-attachments/assets/4f22c6bd-6042-47b9-923c-6fa72aff7f3f)
## License
This project is licensed under the MIT License - see the LICENSE file for details.
You can copy and paste this content directly into your `README.md` file for your GitHub repository.
