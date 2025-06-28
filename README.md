# AI Text Completion App

This project is a Python-based terminal application that uses Cohere's Generative AI API to perform real-time text completions. The goal was to explore how input prompts and model parameters influence the quality and tone of generated responses.

## ⚙️ Project Setup

For this project, I chose **Cohere** as the Generative AI provider due to its free-tier access and straightforward API integration. The application was built and tested using a **Jupyter Notebook and the macOS terminal**. I used the `cohere` Python library to interact with the API, and stored my API key securely within the script during testing.

The app was designed to run in a loop, allowing multiple prompts in a single session. Before each session, the user is asked to set a creativity level (`temperature`) between 0 and 1. The app also includes basic input validation for empty or overly long prompts and error handling for failed API calls.

## 🧪 Usage

During testing, I used various types of prompts—creative (e.g., continuing a story or song), instructional (e.g., explaining a concept to a child), and informational (e.g., summarizing an article). I experimented with different temperature values to evaluate how model behavior changes. Lower values (0.0–0.3) produced factual, structured responses, while higher values (0.8–1.0) led to more expressive and imaginative outputs.

Each session logged the prompt and response, enabling comparison across different creativity settings. This helped me analyze the model's strengths (e.g., creativity, instructional clarity) and limitations (e.g., occasional repetition or vague logic at higher temperatures).

## 📦 Dependencies

- `cohere` – Python client for Cohere's API, used for sending prompts and receiving completions.
- Python 3.x – Compatible with standard Python environments; no additional frameworks required.

## 📝 Notes

This project helped me better understand how generative models like Cohere's respond to prompt structure and parameter tuning. It also highlighted the importance of managing input validation and error handling in API-based applications.
