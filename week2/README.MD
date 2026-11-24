# Week 2 – Provider-Agnostic LLM Client

## Project Overview

This project implements a provider-agnostic Large Language
Model (LLM) client that supports both cloud-based and
local AI models through a common interface.

The application allows users to switch between Google
Gemini and Ollama without changing the main application logic.

## Objectives

- Understand cloud-based and local LLMs.
- Implement a common interface for multiple LLM providers.
- Integrate Google Gemini API.
- Run Llama 3.2 locally using Ollama.
- Understand abstraction and modular programming.
- Perform automated unit testing.

## Technologies Used

- Python
- Google Gemini API
- Ollama
- Llama 3.2
- Python-dotenv
- Requests
- Unittest
- Pytest
- Visual Studio Code

## Project Structure

```text
Week-2/
├── llm_client.py
├── main.py
├── test_client.py
├── requirements.txt
├── .env
├── .gitignore
└── README.md
```

## Features

- Supports multiple LLM providers.
- Cloud-based AI using Google Gemini.
- Local AI using Ollama and Llama 3.2.
- Common interface for generating responses.
- User-friendly provider selection.
- Secure API key configuration.
- Automated unit testing.
- Modular and reusable code.

## Installation

### Step 1: Install Dependencies

```bash
pip install -r requirements.txt
```

Required libraries:

```text
python-dotenv
pytest
google-genai
requests
```

### Step 2: Install Ollama

Download Ollama from:

https://ollama.com/download

Check the installation:

```bash
ollama --version
```

Download the Llama 3.2 model:

```bash
ollama pull llama3.2
```

### Step 3: Configure Environment Variables

Create a `.env` file and add your Gemini API key:

```env
GEMINI_API_KEY=your_api_key_here
```

## How to Run

Execute the following command:

```bash
python main.py
```

Choose an LLM provider:

```text
Choose provider (gemini/ollama): ollama
Enter your question: What is Artificial Intelligence?
```

## Sample Output

```text
LLM Response:

Artificial Intelligence is a technology that enables
machines to perform tasks that normally require
human intelligence.
```

The actual response may vary depending on the selected model.

## Working Process

1. The user selects Gemini or Ollama.
2. The application initializes the selected provider.
3. The user enters a question or prompt.
4. The common LLM client sends the prompt to the provider.
5. The selected AI model generates a response.
6. The response is displayed in the terminal.

## System Architecture

```text
             User Input
                 |
             LLM Client
                 |
          Common Interface
            /          \
     Gemini API       Ollama
     Cloud Model     Local Model
            \          /
            AI Response
```

## Automated Testing

Run the unit test using:

```bash
python -m unittest test_client.py
```

The test uses a fake provider to verify response generation
without making an actual API call.

## Advantages

- Easy switching between AI providers.
- Reduced dependency on a single provider.
- Supports local AI execution.
- Improved code reusability.
- Easy maintenance and future expansion.

## Applications

- AI chatbots
- Virtual assistants
- Generative AI applications
- Question-answering systems
- Multimodel AI platforms

## Security

Never upload API keys to GitHub.

Add the following entries to your `.gitignore` file:

```text
.env
.venv/
__pycache__/
```

## Conclusion

This project demonstrates how to build a flexible and
reusable LLM client that supports both cloud-based and
local AI models. It provides a common interface for
multiple providers, making AI applications easier to
develop, maintain and extend.

