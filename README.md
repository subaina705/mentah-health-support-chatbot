# 🧠 Mental Health Support Chatbot (Fine-Tuned LLM)

A fine-tuned language model chatbot that provides supportive and empathetic
responses for stress, anxiety, and emotional wellness.
Built as part of an AI/NLP internship task using Hugging Face Transformers.

---

## 📌 Project Overview

This project fine-tunes **DistilGPT2** on the **EmpatheticDialogues dataset**
to create a chatbot that responds to emotional situations with a gentle,
supportive tone. The model is trained to understand the user's emotion and
situation and reply in a compassionate way.

---

## 🛠️ Technologies Used

| Tool | Purpose |
|------|---------|
| Python 3.12 | Programming language |
| HuggingFace Transformers | Model loading & fine-tuning |
| HuggingFace Datasets | Dataset loading |
| DistilGPT2 | Base language model |
| PyTorch | Deep learning backend |
| Google Colab (T4 GPU) | Training environment |

---

## 📂 Dataset

- **Name:** EmpatheticDialogues (Facebook AI)
- **Source:** `bdotloh/empathetic-dialogues-contexts` on HuggingFace
- **Size:** 19,209 training examples
- **Content:** Real emotional situations labeled with emotions like
  sentimental, anxious, sad, joyful, etc.

> **Note:** The original `empathetic_dialogues` dataset script is no longer
> supported by newer versions of the HuggingFace `datasets` library.
> An equivalent mirror dataset was used with the same underlying data.

---

## 🔄 Project Pipeline
Install Libraries → Load Dataset → Format & Tokenize
→ Load Model → Fine-Tune → Save Model → Run Chatbot
---

## 🚀 How to Run

### Option 1: Google Colab (Recommended)
1. Open `mental_health_chatbot.ipynb` in Google Colab
2. Go to **Runtime → Change runtime type → T4 GPU**
3. Run all cells from top to bottom

### Option 2: Local Machine
```bash
pip install transformers datasets accelerate torch
jupyter notebook mental_health_chatbot.ipynb
```

---

## 💬 Sample Interaction
👤 You: I have been feeling really anxious about my exams
🤖 Bot: I hear you. That sounds really anxious.
It's completely okay to feel this way.
👤 You: I feel so lonely and dont know what to do
🤖 Bot: I hear you. That sounds really sad.
It's completely okay to feel this way.

## 📋 Requirements
transformers
datasets
accelerate
torch
---

## 📁 File Structure
mental-health-chatbot/
│
├── mental_health_chatbot.ipynb   # Main notebook
├── requirements.txt              # Dependencies
└── README.md                     # Project documentation
---

## ⚠️ Disclaimer

This chatbot is built for educational purposes only.
It is not a substitute for professional mental health advice,
diagnosis, or treatment. If you are struggling, please reach
out to a licensed mental health professional.

---

## 👨‍💻 Author

Built as part of an AI/NLP Internship Program
Task 5 — Mental Health Support Chatbot (Fine-Tuned)
