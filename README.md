# ✨ Mood-Based Motivational Quote Generator

The **Motivational Quote Generator** is a simple AI-based command-line app that generates personalized motivational quotes based on the user’s mood. Designed as an offline tool using Hugging Face’s `falcon-rw-1b` model, it provides fast, private, and uplifting quotes — without requiring internet access or external APIs.

> 🧘 “Let your mood guide your motivation.”

---

## 🎯 Project Objective

To help users — especially students and working professionals — get instant, mood-specific encouragement using an efficient local LLM model. Whether you're feeling anxious, tired, or unfocused, this tool generates a motivational quote designed to uplift your mindset.

---

## 💡 Features

- 🧠 Mood-based quote generation with 9+ emotion categories
- 🤖 Uses Falcon-RW-1B, a lightweight Transformer model for text generation
- 📦 Fully local execution — no OpenAI API, no data leakage
- 📝 Saves all generated quotes in a `quotes.txt` file for later reference
- 🧑‍💻 Simple, interactive command-line interface

---

## 🧠 How It Works

1. Loads the `tiiuae/falcon-rw-1b` model from Hugging Face Transformers.
2. Prompts the user to select their current emotional state.
3. Generates a motivational quote tailored to that emotion.
4. Logs the quote into `quotes.txt` for future inspiration.

---

## 🔧 Technologies Used

| Component     | Tech Used                      |
|---------------|-------------------------------|
| Model         | Falcon-RW-1B (`tiiuae/falcon-rw-1b`) |
| Text Gen      | Hugging Face Transformers     |
| Backend       | PyTorch                       |
| UI            | Python CLI (Terminal)         |
| Logging       | Built-in file I/O             |

---

## 🚀 How to Run It Locally

### 1. 📦 Install Requirements

pip install transformers torch

### 2. ▶️ Run the Script

Run all or press Shift + Enter to run cells step by step.

---

📁 File Structure
motivational-quote-generator/
├── Untitled2.ipynb         # Main Jupyter Notebook with full logic
├── quotes.txt              # Auto-saved generated quotes
├── README.md               # You're reading it!

---

✅ Sample Interaction
🌟 Select your current mood:
1. Anxious
2. Stressed
3. Unmotivated
...

Enter your choice: 3

###💬 Motivational Quote:
"Even on your lowest days, your effort matters and your journey counts."

---

###📌 Mood Categories Supported
#Anxious

#Stressed

#Unmotivated

#Tired

#Excited

#Confused

#Focused

#Sad

#Lonely

---

###🧪 Testing Summary

✅ Generated relevant quotes for each mood

✅ Model loads correctly and runs offline

✅ Handled invalid input without crashing

✅ Saved quotes accurately to a file

---

###✨ Why This Project Matters

This project shows how local LLMs like Falcon can create meaningful, real-world applications even on standard hardware. It’s a reminder that AI isn’t just for tech giants — it can be used for wellness, learning, and inspiration right from your terminal.

---
###🚧 Model Choice & Limitations

Initially, I considered using larger models such as GPT-4 or LLaMA derivatives to enhance the quality and creativity of generated quotes. However, several practical constraints influenced my final choice:

Resource Efficiency: Large-scale models required more RAM and GPU power than a typical laptop can offer.

Latency & Privacy: Online APIs introduce delays and privacy concerns. Offline models provide faster responses and complete control.

Local Compatibility: Falcon-RW-1B was chosen for its balance of performance and hardware-friendliness. It runs locally using Hugging Face Transformers with PyTorch backend, making it ideal for personal or educational use.

Creative Limitations: While Falcon-RW-1B generates coherent, relevant content, its creativity and depth are naturally limited compared to larger models like GPT-4 or Claude 3.

⚠️ Note: The model may occasionally produce generic or repetitive phrases due to its smaller size and limited context awareness.

---

###🙋 Author

Anwika Mothukuri
Student | Builder | Founder Motivational quote generator

---
###🏁 Final Note
This project is more than just an AI demo — it’s a personal tool for reflection and encouragement. By integrating local LLMs with emotion-aware prompts, it proves that even small models can have a big emotional impact.

Whether you're starting your day, facing challenges, or just need a moment of motivation, this quote generator is a reminder that the right words, at the right time, can truly uplift your spirit.

“Not every AI needs to be massive — sometimes, meaningful is enough.” 💡
