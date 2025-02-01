# chat_assistant

# Importing required library
import random

# List of responses
responses = [
    "Hello! How can I help you today?",
    "I'm here to assist you with anything you need.",
    "Feel free to ask me any questions.",
    "I can help you with Python programming and much more!"
]

# Define the chat assistant function
def chat_assistant(user_input):
    if 'hello' in user_input.lower():
        return random.choice(responses)
    else:
        return "Sorry, I didn't understand that. Please ask something else."

# Simulate a chat session
print("Chat Assistant: Hello! Type 'exit' to end the conversation.")
while True:
    user_input = input("You: ")
    if user_input.lower() == "exit":
        print("Chat Assistant: Goodbye!")
        break
    response = chat_assistant(user_input)
    print(f"Chat Assistant: {response}")
