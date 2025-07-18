# Day 19 — LLaMA 3 Chat (via Ollama)

**Date:** July 17, 2025

---

## Overview

On **Day 19**, I built a **simple web-based chat interface** that connects to a local **LLaMA 3** large language model using **Ollama**.  
This project demonstrates how to interact with an AI API in real-time through a browser.

---

## What is LLaMA 3 with Ollama?

- **LLaMA 3:** A large language model capable of generating human-like text.
- **Ollama:** A local API server that serves the LLaMA 3 model on your machine.

---

## How It Works

**1️ Create an HTML file**

- Use a text editor to create `i.html`.

**2️ Add HTML & JavaScript**

- Basic structure includes:
  - Text input for your message.
  - Send button.
  - JavaScript to send requests using `fetch()` with `stream: true`.
  - Live updates: incoming message chunks stream in real-time.

**3️ Run a Local Server**

```bash
# In the same folder as i.html
python3 -m http.server 8000
```

- Open your browser at http://localhost:8000/
- Type a message → click Send → watch the conversation appear!

## Files
- i.html — The chat page with HTML + JavaScript.
- Day19.pdf — Notes on project steps & explanation.

> “Talking to AI locally — fast, private, and entirely under your control.”

