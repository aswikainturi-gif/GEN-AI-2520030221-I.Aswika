# Week 3 – LLM Monitoring with MongoDB

## Overview
This project monitors LLM requests from Google Gemini
and Ollama using MongoDB. It tracks token usage,
response latency, API costs, and request status.

## Technologies Used
- Python
- Google Gemini API
- Ollama (Llama 3.2)
- MongoDB Atlas
- PyMongo
- Python-dotenv

## Features
- Token usage tracking
- Response latency monitoring
- API cost estimation
- MongoDB usage logging
- Timeout and retry handling
- Automated unit testing

## Installation

```bash
pip install -r requirements.txt
```

## Configuration

Create a `.env` file:

```env
GEMINI_API_KEY=your_api_key
MONGODB_URI=your_connection_string
GEMINI_INPUT_PRICE_PER_MILLION=0
GEMINI_OUTPUT_PRICE_PER_MILLION=0
```

## How to Run

```bash
python main.py
```

## Testing

```bash
python -m unittest test_client.py
```

## Database
- Database: llm_monitoring
- Collection: api_usage

## Security
Do not upload the `.env` file or API credentials to GitHub.

## Conclusion
This project helps monitor LLM performance, token
consumption, API costs, and request reliability.

