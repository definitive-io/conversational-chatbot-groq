# Groq Conversational Chatbot

This repository contains a Streamlit application that allows users to interact with a conversational chatbot powered by the Groq API. The application uses a list of starter prompts to initiate the conversation and maintains a history of the conversation to provide context for the chatbot's responses.

## Features

- **Conversational Interface**: The application provides a conversational interface where users can ask questions or make statements, and the chatbot responds accordingly.

- **Contextual Responses**: The application maintains a history of the conversation, which is used to provide context for the chatbot's responses.

- **Customization**: Users can customize the Groq model used for generating responses and the length of the conversational memory.

## Starter Prompts

The starter prompts are stored in a text file located in the root directory:

- `starter_prompts.txt`: Contains a list of prompts that users can use to start the conversation with the chatbot.

## Functions

- `chat_with_groq(client, prompt, model)`: Sends a chat message to the Groq API and returns the content of the response.

- `get_conversational_history(user_question_history, chatbot_answer_history, conversational_memory_length)`: Generates a full prompt for the chatbot based on the history of the conversation.

- `get_random_prompt(file_path)`: Reads a file of prompts and returns a random prompt.

- `main()`: The main function of the application, which initializes the Groq client, sets up the Streamlit interface, and handles the chat interaction.

## Usage

To use this application, you need to have Streamlit and the other required Python libraries installed. You also need to have a Groq API key, which you can obtain by signing up on the Groq website.

Once you have the necessary requirements, you can run the application by executing the script with Streamlit:

```shell
streamlit run app.py
```

This will start the Streamlit server and open the application in your web browser. You can then interact with the chatbot, and the application will generate responses based on the history of the conversation.
