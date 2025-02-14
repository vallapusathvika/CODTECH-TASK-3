# CODTECH-TASK-3
COMPANY:CODTECH IT SOLUTIONS

NAME:VALLAPU SATHVIKA

INTERN ID:CT08RGJ

DOMAIN:PYTHON PROGRAMMING

DURATION:4 WEEKS

MENTOR:NEELA SANTOSH

**DESCRIPTION OF THE CODE***
This Python code implements a simple chatbot using the **Natural Language Toolkit (NLTK)** library. It is designed to interact with a user by recognizing specific patterns in user input and responding accordingly. The chatbot uses **regular expressions** to match patterns in the user's text and provides predefined responses. This implementation is performed in a **Jupyter Notebook**, providing an interactive and real-time environment for the chatbot's execution.

 **Step 1: Importing NLTK and Handling Missing Packages**
The code starts by importing the `nltk` library, which is a powerful tool for working with human language data in Python. NLTK provides easy-to-use interfaces to over 50 corpora and lexical resources, along with libraries for text processing tasks. The first step is to check whether the NLTK package for tokenization (`punkt`) is available on the system. If it is not found, a `LookupError` is raised, and the package is automatically downloaded using `nltk.download('punkt')`. This ensures that the necessary resources for tokenizing text (i.e., breaking down text into smaller units like words and sentences) are available for the chatbot's functionality. This download process is performed within the **Jupyter Notebook**, where the user can observe and interact with any errors or messages.

 **Step 2: Defining the Chatbot’s Patterns and Responses**
The core of the chatbot is the list `pairs`, which consists of **regular expressions** and their corresponding responses. The patterns represent different types of user inputs that the chatbot is designed to recognize. The regular expressions allow the chatbot to match various user queries such as greetings (`"hi|hello|hey"`), asking about the chatbot's name (`"what is your name?"`), and seeking help (`"(.*) (help|assist) (.*)"`). Each regular expression is associated with a list of potential responses. For example:
- If the user types a greeting like "hi" or "hello", the chatbot responds with a greeting.
- If the user asks about the chatbot’s name, it will respond with a predefined answer about its identity.
- If the user types "quit", the chatbot ends the conversation.

Additionally, the regular expression `(.*)` acts as a fallback to catch any user input that does not match any of the predefined patterns. In such cases, the chatbot responds with a message asking the user to rephrase their query.

 **Step 3: Creating the Chatbot Instance**
The chatbot is created using the `Chat` class from the `nltk.chat.util` module. The `Chat` class takes two arguments:
1. `pairs`: The list of patterns and responses that the chatbot will recognize.
2. `reflections`: A dictionary that maps common user pronouns (e.g., "I" to "you") for creating more natural responses. In this code, the `reflections` dictionary is imported from NLTK and used by default.

By initializing the `Chat` class with these parameters, the chatbot is ready to interact with the user based on the defined patterns.

 **Step 4: Running the Chatbot**
The `start_chat()` function is defined to initiate the interaction between the user and the chatbot. When called, the function prints an introductory message ("Hi! I'm your chatbot. Type 'quit' to exit.") and enters a loop where it continuously asks for user input. If the user types "quit", the chatbot responds with a goodbye message and terminates the conversation. Otherwise, the chatbot uses the `respond()` method from the `Chat` class to generate an appropriate response based on the user’s input. The response is then printed to the screen. The interaction continues until the user types "quit".

 **Step 5: Running the Program in Jupyter Notebook**
The `if __name__ == "__main__":` block ensures that the chatbot only starts when the script is executed directly. Since the code is implemented in a **Jupyter Notebook**, the function `start_chat()` can be called directly within a code cell to initiate the conversation. The user can interact with the chatbot in real-time, providing inputs and receiving responses within the notebook interface.

 **Conclusion**
This chatbot implementation in **Jupyter Notebook** demonstrates a simple way to create a conversational agent using the **NLTK** library and **regular expressions**. It is an interactive tool that responds to predefined patterns and can easily be extended with additional patterns and responses. The chatbot is suitable for educational purposes and basic conversational tasks and can be tested in the **Jupyter Notebook** environment, making it easy to modify and experiment with different inputs and patterns. The notebook environment provides an ideal platform for real-time interaction and debugging, allowing the user to observe and adjust the chatbot’s behavior instantly.
***OUTPUT***:![Image](https://github.com/user-attachments/assets/9011ba6b-f327-4827-95c9-9cf566141e36)
