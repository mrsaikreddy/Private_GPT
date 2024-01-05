# PrivateGPT

## Project Motivation
PrivateGPT was inspired by the need for privacy in AI interactions. Recognizing the growing concern for data confidentiality, it aims to provide a secure environment for AI communication.

## Core Features and Benefits
PrivateGPT stands out with its advanced data protection features and user-friendly interface, making AI interactions safe and accessible.

## Examples of Use
Ideal for secure business communications and personal data protection, PrivateGPT can be integrated into various scenarios requiring confidentiality.

### Architecture
![Architecture](/static/arch.png)

### Private GPT vs OpenAI ChatGPT
![Private GPT vs OpenAI ChatGPT](/static/privategpt_vs_chatgpt.png)

## Redaction and Anonymization in Private GPT
![Redaction and Anonymization in Private GPT](/static/demo2.png)

## How it Works
Private GPT works in two steps:
1. Local Data Redaction: The user prompt is first redacted locally on your PC using a language model, such as Vicuna or any other good performance open-source LLM, to remove any personal information. The redacted prompt is then sent to the AI model.
Enterprises can use this models on their own servers instead of running on the user's PC.

2. AI Response Redaction: The sanitized Prompt is then sent to ChatGPT or Bard which generates a response. This is processed and sent back to the user after filtering out any unintended information.


## Tech Stack
- Python
- Streamlit: Python library for building user interfaces.Streamlit is a free and open-source framework to rapidly build and share beautiful machine learning and data science web apps.
- Sqlite: Database for using storing all chat queries.
- HTML/CSS: Markup and styling for the web application.
- Vicuna: Vicuna is a LLaMA - based language Model. It performs data redaction and anonymization.
- AI Models (e.g., ChatGPT, Bard): Deep learning models used to generate AI responses.
- FastAPI: FastAPI is a modern, fast (high-performance), web framework for building APIs with Python 3.6+ based on standard Python type hints.
- llama-cpp-python: A library for using LLaMA models in Python and C++.
## Future Enhancements
We plan to expand PrivateGPT's capabilities with more AI models and enhanced privacy features.

## Acknowledgments
Special thanks to everyone who contributed to PrivateGPT's development.


