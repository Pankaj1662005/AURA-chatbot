# AURA-chatbot
offline chatbot using advanced Machine Learning (ML) and Large Language Models (LLM)


Got it! Here's the actual `README.md` **file content** in proper format — you can copy-paste this directly into a `README.md` file:

---

```markdown
# 💬 AURA: Conversational AI with Falcon-7B

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
git clone https://github.com/your-username/aura-chatbot.git
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

---

## 🚀 Usage

Run the chatbot with:

```bash
python main.py
```

You will enter an interactive session like:

```
> Hello
AURA: Hi there! How can I assist you today?
```

To stop the conversation, simply use `Ctrl + C`.

---

## 🧾 Code Breakdown

```python
model = "tiiuae/falcon-7b-instruct"
tokenizer = AutoTokenizer.from_pretrained(model)
pipeline = pipeline(
    "text-generation",
    model=model,
    tokenizer=tokenizer,
    torch_dtype=torch.bfloat16,
    device_map="auto",
    trust_remote_code=True
)
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

---

Let me know if you want to turn this into a GitHub project with a `main.py` and everything organized, or if you want to make the README fancier with badges or screenshots!
