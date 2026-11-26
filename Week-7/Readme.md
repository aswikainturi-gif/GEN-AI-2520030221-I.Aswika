# Week 7 – Next Token Probability Analysis Using GPT-2

## Objective
To understand how Large Language Models (LLMs) predict the next token using logits, softmax, and probability distribution.

## Description
This project uses the GPT-2 model to predict the top 5 possible next tokens for different input prompts. It calculates token probabilities using the softmax function and stores the results in a CSV file.

## Technologies Used
- Python
- PyTorch
- Hugging Face Transformers
- GPT-2
- CSV

## Project Files
- `main.py` – Main Python program.
- `requirements.txt` – Required Python libraries.
- `week7_probability_results.csv` – Generated prediction results.
- `README.md` – Project documentation.

## Installation

Install the required libraries:

```bash
pip install -r requirements.txt
```

## Execution

Run the Python program:

```bash
python main.py
```

## Features
- Loads the pretrained GPT-2 model.
- Tokenizes input prompts.
- Converts logits into probabilities using softmax.
- Displays the top 5 predicted tokens for each prompt.
- Automatically saves results into a CSV file.

## Output
The program generates 20 predictions for 4 input prompts, including:
- Prompt
- Rank
- Candidate Token
- Token ID
- Probability

## Conclusion
This experiment demonstrates how GPT-2 predicts the next token and helps in understanding tokenization, logits, softmax, and probability distribution in Generative AI.
