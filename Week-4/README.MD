# Week 4 – Tokenizer Comparison Lab

## Project Overview

This project demonstrates and compares three subword tokenization techniques used in Natural Language Processing (NLP) and Generative AI. It analyzes how different tokenizers process English, Telugu and Hindi text.

## Objectives

- Understand the concept of tokenization.
- Compare BPE, WordPiece and SentencePiece tokenizers.
- Analyze token pieces, token IDs and token counts.
- Understand multilingual text processing in Large Language Models (LLMs).

## Tokenizers Used

| Tokenizer | Pretrained Model |
|---|---|
| Byte Pair Encoding (BPE) | GPT-2 |
| WordPiece | Multilingual BERT |
| SentencePiece | XLM-RoBERTa |

## Technologies Used

- Python
- Hugging Face Transformers
- SentencePiece
- Visual Studio Code
- Natural Language Processing (NLP)

## Supported Languages

- English
- Telugu
- Hindi

## Project Structure

```text
Week4/
├── tokenizer_comparison.py
├── requirements.txt
└── README.md
```

## Installation

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Required libraries:

```text
transformers
sentencepiece
```

Python 3.10 or later is recommended. Internet access is required during the first execution to download the pretrained tokenizers.

## How to Run

Execute the following command in the terminal:

```bash
python tokenizer_comparison.py
```

## Working Process

1. Load the three pretrained tokenizers.
2. Provide English, Telugu and Hindi input sentences.
3. Convert the sentences into tokens.
4. Generate corresponding token IDs.
5. Calculate and compare token counts.
6. Display the results in the terminal.

## Expected Output

The program displays:

- Input language
- Input sentence
- Tokenizer name
- Generated tokens
- Token IDs
- Total token count

## Conclusion

This project helps in understanding how different tokenizers process multilingual text. Token counts vary depending on the tokenization method, vocabulary and training data. XLM-R uses SentencePiece with BPE, so this experiment compares pretrained tokenizers rather than three independently trained algorithms.

## Author

Aswika Inturi

B.Tech – Computer Science and Engineering

Generative AI – Week 4 Lab
