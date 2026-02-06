🎯 Prompt Understanding Test
📌 Project Summary

This project is an interactive web application built on Hugging Face Spaces that helps users test whether a Large Language Model (LLM) truly understands a given prompt (instruction or question).

The user writes a prompt, the app sends it to a ready-made language model (Qwen 2.5-7B-Instruct), then automatically analyzes the response to check if the model understood the context and the required task correctly.

The goal is to teach students how prompt quality affects AI understanding and how to evaluate LLM responses in a simple, practical way.

📌 Overview

The Prompt Understanding Test is an interactive web application designed to demonstrate advanced Large Language Model (LLM) integration and evaluation techniques.

The primary goal of this project is to assess whether an LLM truly understands a given prompt (instruction or question), rather than simply generating text. The application allows users to input a prompt, sends it to a powerful LLM via an API, receives the generated response, and then automatically analyzes that response to evaluate the model’s level of understanding.

The application is deployed as a web app on Hugging Face Spaces and provides a clean, user-friendly interface for real-time interaction.

🛠️ Tech Stack & Tools

Programming Language: Python 3

UI Framework: Gradio (customized with CSS for a professional appearance)

Model Provider: Hugging Face Inference API

Model Used: Qwen/Qwen2.5-7B-Instruct

Chosen for its strong performance in both Arabic and English

High-quality instruction-following and contextual understanding

✨ Key Features

Interactive User Interface
A clean and professional UI featuring a White Window design with high-contrast text for clarity and readability.

Real-time Inference
Direct integration with the Qwen 2.5 model to generate instant responses from user-provided prompts.

Automatic Evaluation Logic
The application includes built-in logic to analyze the generated response and classify the model’s understanding:

✅ Understood: The response contains confirmation keywords or a meaningful, detailed explanation.

⚠️ Uncertain / Error: The response is empty, too short, or an API error occurs.

Bilingual Support
Fully supports prompt processing and evaluation in both Arabic and English.

⚙️ How It Works

Input
The user enters a prompt (instruction or question) into the text box.

Processing
The application sends the prompt securely to the Hugging Face Inference API using an environment secret token (HF_API_TOKEN).

Generation
The LLM generates a response based on the input prompt.

Analysis
A Python-based evaluation script analyzes the response length and checks for key indicators of understanding.

Display
The result is displayed in a styled output box (white background, black text) along with a clear status indicator.

🚀 Installation & Local Setup

Follow these steps to run the project locally:

1️⃣ Clone the Repository
git clone https://github.com/your-username/Task-5-Project.git
cd Task-5-Project

2️⃣ Install Dependencies
pip install gradio huggingface_hub

3️⃣ Set Up the API Token

You need a Hugging Face Access Token.

For local testing, set it as an environment variable:

export HF_API_TOKEN="your_huggingface_token_here"


⚠️ For security reasons, never hardcode your API token in public repositories.

4️⃣ Run the Application
python app.py
The app will launch locally and open in your browser.

📂 Project Structure
├── app.py              # Main application file (UI + logic)
├── requirements.txt    # Project dependencies
├── README.md           # Project documentation
└── assets/             # Screenshots and images

🌍 Deployment

This project is designed to be easily deployed on Hugging Face Spaces, using environment secrets to securely manage API tokens.
