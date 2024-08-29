# MiniAlexa - Alexa Voice Assistant

This project is a simple Alexa-like voice assistant implemented in Python. It uses various libraries to recognize speech, convert text to speech, perform internet searches, fetch current time, tell jokes, and more. The assistant listens for voice commands and responds accordingly, offering basic functionalities such as playing songs on YouTube, telling the current time, fetching information from Wikipedia, and telling jokes.

# Features

- **Speech Recognition**: Listens to voice commands using the microphone.
- **Text-to-Speech**: Converts the assistant's responses to audible speech.
- **Play YouTube Videos**: Plays songs on YouTube based on voice commands.
- **Time Inquiry**: Provides the current time.
- **Wikipedia Search**: Fetches brief information about a person from Wikipedia.
- **Jokes**: Tells jokes when prompted.

# Requirements

- Python 3.x
- Required Libraries:
  - 'speech_recognition'
  - 'pyttsx3'
  - 'pywhatkit'
  - 'datetime' (comes pre-installed with Python)
  - 'wikipedia'
  - 'pyjokes'

# Installation

1. Clone the repository or download the source code.
2. Navigate to the project directory.
3. Install the required libraries using pip:
   pip install speechrecognition pyttsx3 pywhatkit wikipedia pyjokes

# Usage

1.Ensure your microphone is set up correctly and is working.
2.Run the main program:
  python main.py

# How it Works

1. Speech Recognition: The assistant listens to the user's voice through the microphone using the speech_recognition library.
2. Text-to-Speech: The recognized command is converted to text using Google's speech recognition service, and the assistant responds using the pyttsx3 text-to-speech engine.
3. Commands Execution:
   - Play Command: Uses pywhatkit to search and play songs on YouTube.
   - Time Command: Fetches the current time using the datetime module.
   - Wikipedia Command: Fetches information using wikipedia based on the command.
   - Joke Command: Tells a random joke using the pyjokes library.
4. Continuous Listening: The program runs in an infinite loop, continuously waiting for commands.

# Algorithm

1. Import Modules: Import required libraries (speech_recognition, pyttsx3, pywhatkit, datetime, wikipedia, and pyjokes).
2. Initialize the Listener: Create a listener object using speech_recognition for voice input.
3. Text-to-Speech Setup: Initialize the speech engine (pyttsx3) and configure the voice settings.
4. Talk Function: Define talk(text) to convert given text into speech and play it.
5. Get Command Function: Define get_command() to listen and recognize commands from the user. It uses recognize_google for speech-to-text conversion.
6. Take Command Function: Define takeCommand() to listen for input with a pause threshold and recognize it as a string output.
7. Run Alexa Function: Define run_alexa() which executes the appropriate command based on recognized speech:
   - Play Music: Plays a song on YouTube using pywhatkit.
   - Tell Time: Announces the current time.
   - Who is: Fetches information about a person from Wikipedia.
   - Joke: Tells a random joke.
   - Unrecognized Commands: Asks the user to repeat.
8. Main Loop: Continuously runs the run_alexa() function, making the assistant responsive to new commands.

# Troubleshooting

1. No Python Found Error: Ensure Python is installed correctly and the environment variables are set up properly.
2. Microphone Issues: Check if the microphone is correctly configured and accessible by the program.
3. Speech Recognition Errors: If the assistant is unable to recognize commands, check the microphone sensitivity and ensure proper internet access.

# Contributing

Feel free to fork the repository and submit pull requests for additional features or bug fixes.

# License

This project is open-source and free to use for educational and personal purposes.

This README file provides an overview of what the code does, how to set it up, and what commands it can respond to. Let me know if you need any further modifications!
