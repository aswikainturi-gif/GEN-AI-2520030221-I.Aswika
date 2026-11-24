
# Week 6 – Golden Question Set and Baseline Evaluation

## Objective
To evaluate the performance of the Llama 3.2 model using a golden question set containing 30 questions, expected answers, keywords, and reference sources.

## Technologies Used
- Python
- Ollama
- Llama 3.2
- JSON
- Requests
- CSV

## Features
- Golden question dataset with 30 questions.
- Automatic response generation using Llama 3.2.
- Keyword-based evaluation and scoring.
- PASS and REVIEW classification.
- Automatic CSV report generation.
- Baseline evaluation summary.

## Project Structure

    Week6/
    ├── main.py
    ├── golden_set.json
    ├── requirements.txt
    ├── baseline_results.csv
    └── README.md

## Installation and Execution

1. Install Ollama.
2. Download the Llama 3.2 model:

       ollama pull llama3.2

3. Install dependencies:

       pip install -r requirements.txt

4. Ensure Ollama is running.
5. Run the program:

       python main.py

## Output
The program generates a baseline_results.csv file containing model responses, expected answers, matched keywords, scores, and evaluation status.

## Release Version
v0.1 – First Baseline Evaluation.

## Conclusion
This practical demonstrates how to evaluate LLM responses using a golden question set and keyword-based scoring.
