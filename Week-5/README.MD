# Week 5 – Token Economics: Cost and Rate-Limit Budgeting

## Project Overview

This project focuses on estimating token usage, API costs,
and rate limits before developing an LLM-based application.
It uses a Python-based budget planner to calculate daily
and monthly expenses and determine whether the application
operates within the configured budget and rate limits.

## Objectives

- Understand input and output tokens.
- Calculate daily and monthly token consumption.
- Estimate LLM API costs.
- Understand Requests Per Minute (RPM).
- Understand Tokens Per Minute (TPM).
- Apply a safety margin to usage estimates.
- Perform automated testing and what-if analysis.

## Technologies Used

- Python
- Python-dotenv
- Unittest
- Visual Studio Code
- Generative AI
- Large Language Models (LLMs)

## Project Structure

```text
TokenEconomics/
├── .env
├── .gitignore
├── budget.py
├── test_budget.py
├── requirements.txt
└── README.md
```

## Features

- Token usage estimation
- Daily and monthly cost calculation
- RPM and TPM capacity checking
- Configurable budget limits
- Safety margin calculation
- Automated unit testing
- Budget recommendations

## Installation

Install the required library:

```bash
pip install -r requirements.txt
```

## Environment Configuration

Create a `.env` file with the following sample values:

```env
INPUT_PRICE_PER_MILLION=0.30
OUTPUT_PRICE_PER_MILLION=1.20
REQUESTS_PER_DAY=2000
AVG_INPUT_TOKENS=1200
AVG_OUTPUT_TOKENS=300
PEAK_REQUESTS_PER_MINUTE=30
RPM_LIMIT=60
TPM_LIMIT=100000
MONTHLY_BUDGET_USD=50
DAILY_BUDGET_USD=2
SAFETY_MARGIN_PERCENT=20
```

These prices and limits are illustrative planning values.

## How to Run

Execute the following command:

```bash
python budget.py
```

## Expected Output

| Parameter | Expected Result |
|---|---|
| Input tokens per day | 2,400,000 |
| Output tokens per day | 600,000 |
| Total tokens per day | 3,000,000 |
| Estimated daily cost | $1.44 |
| Estimated monthly cost | $43.20 |
| Peak RPM with margin | 36 |
| Peak TPM with margin | 54,000 |
| RPM capacity | PASS |
| TPM capacity | PASS |
| Daily budget | PASS |
| Monthly budget | REVIEW |

The monthly budget requires review because the estimated
monthly cost with a 20% safety margin is $51.84, which
exceeds the configured $50 budget.

## Automated Testing

Run the unit tests using:

```bash
python -m unittest test_budget.py
```

The tests verify:

- Cost estimation
- Capacity validation
- RPM limit failure
- Monthly budget failure

## What-If Analysis

The program allows users to analyze different scenarios:

- Increase the number of users.
- Increase input or output tokens.
- Increase peak traffic.
- Change model pricing.
- Reduce prompt size.
- Adjust budget limits.

## Security

Do not upload API keys or sensitive environment variables
to GitHub. Add `.env` and `.venv/` to the `.gitignore` file.

## Applications

- LLM application development
- AI chatbot cost estimation
- API budget management
- Resource optimization
- Generative AI project planning

## Conclusion

This project demonstrates how token economics helps
developers estimate API costs, manage rate limits, and
optimize resource usage before building LLM applications.
It supports cost-effective and efficient AI development.
