
```markdown

- Updated by Hassan 'zimkk' Nazir

This simple voice assistant application uses OpenAI's GPT-3 to respond to user queries. It can recognize speech, generate responses using GPT-3, and perform basic actions such as opening websites.

## Features

- Convert speech to text using Google's Speech Recognition API.
- Generate responses using OpenAI's GPT-3.
- Speak responses using pyttsx3.
- Open websites based on user commands.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/voice-assistant-application.git
   cd voice-assistant-application
   ```

2. Create a virtual environment and activate it:

   ```bash
   python3 -m venv env
   source env/bin/activate   # On Windows use `env\Scripts\activate`
   ```

3. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Set up your OpenAI API key:

   Create a file named `apikey.py` in the project directory and add your API key:

   ```python
   api_data = "your_openai_api_key"
   ```

## Usage

Run the main script:

```bash
python main.py
```

The voice assistant will start and listen for your commands.

## File Descriptions

- `main.py`: The main script that runs the voice assistant.
- `apikey.py`: Contains the OpenAI API key (not included in the repository for security reasons).

## Dependencies

- Python 3.6+
- `openai`
- `pyttsx3`
- `speech_recognition`
- `webbrowser`

## License

This project is licensed under the MIT License - see the LICENSE file for details.
```

---

## Documentation.md

```markdown
# Voice Assistant Application Documentation

## Overview

This document provides detailed information about the Voice Assistant Application, including installation instructions, usage guidelines, and a description of the functions and their roles.

## Installation

### Prerequisites

- Python 3.6+
- `pip` (Python package installer)

### Steps

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/voice-assistant-application.git
   cd voice-assistant-application
   ```

2. Create a virtual environment and activate it:

   ```bash
   python3 -m venv env
   source env/bin/activate   # On Windows use `env\Scripts\activate`
   ```

3. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Set up your OpenAI API key:

   Create a file named `apikey.py` in the project directory and add your API key:

   ```python
   api_data = "your_openai_api_key"
   ```

## Usage

To run the application, execute the following command:

```bash
python main.py
```

### User Interaction

The voice assistant will greet you and wait for your commands. You can ask it questions, and it will respond using GPT-3. It can also perform specific actions like opening websites. 

### Example Commands

- "Open YouTube"
- "Open Google"
- "Bye" (to exit the application)

## Function Descriptions

### `main.py`

- **`Reply(question)`**: Generates a response to the given question using GPT-3.
- **`speak(text)`**: Converts text to speech using pyttsx3.
- **`takeCommand()`**: Listens for and recognizes speech input using the microphone and Google's Speech Recognition API.
- **`if __name__ == '__main__':`**: The main loop that keeps the assistant running, processing commands, and performing actions based on recognized speech.

### `apikey.py`

This file should contain your OpenAI API key in the following format:

```python
api_data = "your_openai_api_key"
```

## Dependencies

- `openai`: OpenAI's API client for Python.
- `pyttsx3`: A text-to-speech conversion library in Python.
- `speech_recognition`: Library for performing speech recognition.
- `webbrowser`: Standard Python module for opening URLs in web browsers.
