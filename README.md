# AURA-chatbot
offline chatbot using advanced Machine Learning (ML) and Large Language Models (LLM)

AURA is a simple interactive chatbot built using the [Falcon-7B-Instruct](https://huggingface.co/tiiuae/falcon-7b-instruct) model via Hugging Face's Transformers library. This chatbot keeps track of the conversation and responds contextually.

---

## 📌 Features

- 🤖 Based on Falcon-7B-Instruct LLM
- 💬 Multi-turn conversation support
- ⚡ Optimized with `bfloat16` for faster inference (if supported)
- 🔧 Automatic device mapping (GPU/CPU)
- 🧠 Simple, readable codebase

---

## 🛠️ Installation

### 1. Clone this repository

```bash
git clone https://github.com/Pankaj1662005/AURA-chatbot/.git
cd aura-chatbot
```

### 2. Set up a virtual environment (optional but recommended)

```bash
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install torch transformers accelerate
```


- Loads Falcon-7B-Instruct with tokenizer
- Sets up generation pipeline with device auto-mapping and bf16 precision
- Maintains a conversation history in a list and feeds it as a prompt

---

## 👨‍💻 Author

**Pankaj Sheokand**  
Student at Thapar Institute of Engineering & Technology (COE)  
📧 pankajsheokand2005@gmail.com  

---

## 🤖 Model Credits

- Model: [tiiuae/falcon-7b-instruct](https://huggingface.co/tiiuae/falcon-7b-instruct)  
- Framework: [Hugging Face Transformers](https://huggingface.co/docs/transformers)

---

## ⚠️ Disclaimer

This is an educational project. The chatbot may generate unpredictable or incorrect outputs. Use responsibly.

```

