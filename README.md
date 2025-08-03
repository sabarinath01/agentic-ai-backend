# agentic-ai-backend
Tool-augmented LLM agent using Groq and Python
A simple LLM-powered agentic system built in Python and Colab using Groq's LLaMA-3 model. The agent can:
- Generate and execute code from natural language prompts
- Monitor stock prices and trigger alerts
- Perform tool-based reasoning

## How It Works

1. User provides a task (e.g., "Calculate sum of exponential of Fibonacci numbers")
2. The system queries Groq LLM → returns Python code
3. The code is executed securely in Colab
4. Supports API integration, email alerts, and agentic extensions

## Tech Stack

- Python, Google Colab
- Groq API (LLaMA-3 70B)
- Requests, smtplib, yfinance, etc.

## Example

```python
prompt = "Calculate sum of exponential of first 6 Fibonacci numbers"
# Groq will return:
# import math
# fib = [0, 1, 1, 2, 3, 5]
# print(sum([math.exp(x) for x in fib]))
