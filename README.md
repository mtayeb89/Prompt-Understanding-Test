📌 Project Overview
This project is a Prompt Understanding Test application developed to demonstrate advanced Large Language Model (LLM) integration and evaluation capabilities.
The main goal is to create an interactive web application hosted on Hugging Face Spaces that allows users to input a specific prompt (instruction or question). 
The app sends this prompt to a powerful Large Language Model (LLM) via an API, receives the response, and automatically analyzes it to determine if the model understood the context.

🛠️ Tech Stack & Tools

Language: Python 3

UI Framework: Gradio (Customized with CSS for a professional look)

Model Provider: Hugging Face Inference API

Model Used: Qwen/Qwen2.5-7B-Instruct (Selected for its high performance in both Arabic and English)

✨ Key Features

Interactive UI: A clean, professional user interface featuring a "White Window" design with high-contrast text.

Real-time Inference: Connects directly to the Qwen 2.5 model to generate instant responses.

Auto-Evaluation Algorithm: A built-in logic system that analyzes the model's output quality:

✅ Understood: If the response contains positive confirmation keywords or a detailed explanation.

⚠️ Uncertain/Error: If the response is too short, empty, or an API error occurs.

Bilingual Support: Capable of processing and evaluating prompts in both Arabic and English.

⚙️ How It Works

Input: The user enters a prompt in the text box.

Processing: The app sends the request to the Hugging Face API securely using an environment secret token (HF_API_TOKEN).

Generation: The LLM generates a response based on the input.

Analysis: The Python script evaluates the response length and keywords.

Display: The result is shown in a styled box (White background, Black text) with a specific status indicator.
🚀 Installation & Local Setup
To run this project locally, follow these steps:
Clone the repository:
cd Task-5-Project

Install dependencies:
pip install gradio huggingface_hub

Set up your API Token:
You need a Hugging Face Access Token. Set it as an environment variable or paste it directly in the code (for local testing only).

export HF_API_TOKEN="your_huggingface_token_here"

Run the App:

python app.py

📂 Project Structure

├── app.py              # Main application file containing UI and Logic
├── requirements.txt    # List of dependencies
├── README.md           # Project Documentation
└── assets/             # Screenshots and images

