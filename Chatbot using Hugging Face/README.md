# Chatbot using Hugging Face

A simple chatbot GUI application powered by Hugging Face's DialoGPT model. Chat naturally with an AI through a clean Tkinter interface.

## Features

- Clean, responsive GUI built with Tkinter
- Powered by Microsoft's DialoGPT-medium model
- Maintains conversation context for natural dialogue
- Intelligent response filtering and cleaning
- Supports both GPU and CPU inference
- Real-time status updates and error handling

## Requirements

- Python 3.x
- Jupyter Notebook
- PyTorch
- Transformers library
- Tkinter (usually included with Python)

Install dependencies:
```bash
pip install torch transformers
pip install huggingface_hub[hf_xet]  # optional, for better model loading
```

## Usage

1. Open `huggingface_chatbot.ipynb` in Jupyter Notebook.
2. Run the notebook cells to launch the chat window.
3. Wait for the model to load (status shown at bottom).
4. Start chatting! Type messages and press Enter or click Send.
5. Use the Clear button to reset the conversation.

## How It Works

- Uses Microsoft's DialoGPT-medium for natural language generation
- Maintains conversation history for contextual responses
- Implements smart response filtering to avoid gibberish
- Uses threading to keep UI responsive during generation
- Carefully tuned generation parameters for quality responses

---

Chat with an AI in a simple, clean interface!