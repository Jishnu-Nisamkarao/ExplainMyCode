# ExplainMyCode
An Al-Powered System for Generating Explanations of Source Code in a Local Indian Language

* **Project Title:** NLP Code Explainer — English & Telugu
* **Domain:** Natural Language Processing
* **Platform:** Google Colab
* **Language:** Python

# 🧠 NLP Code Explainer — English & Telugu
![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)


## 📌 Project Overview

**NLP Code Explainer — English & Telugu** is an AI-powered web application designed to help beginners understand programming code by converting it into **simple natural-language explanations**.
The system provides explanations in **English and Telugu**, making programming education more accessible to regional-language learners.

This project combines **Natural Language Processing (NLP)**, **Large Language Models (LLMs)**, and an **interactive web interface** to bridge the gap between source code and human understanding.

---

## 🎯 Problem Statement

Many students struggle to learn programming due to:

* Complex technical explanations
* Lack of learning tools in regional languages
* Overly verbose or code-repeating explanations
* Limited accessibility for non-English speakers

Traditional code documentation and tutorials are often **English-only**, which creates a learning barrier for Telugu-medium and regional-language students.

---

## 💡 Proposed Solution

This project solves the above problem by:

* Automatically analyzing programming code
* Generating **clear, beginner-friendly English explanations**
* Translating and explaining the same content in **Telugu**
* Presenting the results through a **simple web-based interface**

The system avoids repeating code and focuses purely on **conceptual understanding**.

---

## 🏗️ System Architecture

```
User Input (Code)
        ↓
English Explanation Model (FLAN-T5)
        ↓
Cleaned English Explanation
        ↓
Telugu Explanation Model (LLaMA-3 API)
        ↓
Gradio Web Interface (Output)
```

---

## 🧠 Models Used

### 🔹 English Explanation Model

* **Model Name:** `google/flan-t5-base`
* **Type:** Encoder–Decoder Transformer
* **Purpose:**

  * Convert code into clear English explanations
  * Follow instructions strictly
  * Avoid repeating code or symbols

**Why FLAN-T5?**

* Excellent instruction-following capability
* CPU-friendly
* Produces clean, readable explanations

---

### 🔹 Telugu Explanation Model

* **Model Name:** `meta-llama/Meta-Llama-3-70B-Instruct`
* **Access Method:** Hugging Face Inference API
* **Purpose:**

  * Convert English explanations into natural Telugu
  * Preserve meaning and clarity

**Why LLaMA-3?**

* High-quality multilingual generation
* Natural sentence structure in Telugu
* Accurate translation and explanation ability

---

## 🛠️ Technologies Used

| Technology       | Purpose                     |
| ---------------- | --------------------------- |
| Python           | Core programming language   |
| Transformers     | Model loading and inference |
| Hugging Face Hub | API-based model access      |
| Gradio           | Web interface               |
| Google Colab     | Development & execution     |
| SentencePiece    | Tokenization support        |
| WebSockets       | API communication           |

---

## ⚙️ Installation & Setup

### 1️⃣ Install Required Libraries

```bash
pip install transformers==4.41.2 \
huggingface_hub==0.34.1 \
gradio==4.44.1 \
sentencepiece \
websockets>=13,<15
```

---

### 2️⃣ Hugging Face Token Setup

1. Go to **Hugging Face → Settings → Access Tokens**
2. Create a token with **Read** permission
3. In **Google Colab**:

   * Open **Tools → Secrets**
   * Add:

     * **Name:** `HF_TOKEN`
     * **Value:** your Hugging Face token

---

## ▶️ How to Run the Project

1. Open the notebook in Google Colab
2. Run all cells sequentially
3. Wait for model loading to complete
4. A Gradio web interface will launch
5. Paste your code
6. Select output language:

   * English
   * Telugu
   * Both
7. Click **Submit**

---

## 🖥️ User Interface Features

* Code input textbox
* Language selection radio button
* Explanation output panel
* Public shareable URL
* Clean dark-themed UI

---

## ✨ Example

### Input Code

```python
for i in range(3):
    print(i)
```

### English Explanation

This code runs a loop three times.
The range function generates values from zero to two.
During each iteration, the current value is printed.

### Telugu Explanation

ఈ కోడ్‌లో for లూప్‌ను ఉపయోగించారు.
range(3) ద్వారా 0, 1, 2 విలువలు వస్తాయి.
ప్రతి సారి లూప్ నడిచినప్పుడు ఆ విలువను ప్రింట్ చేస్తుంది.

<img width="1337" height="492" alt="Screenshot 2026-02-24 235550" src="https://github.com/user-attachments/assets/0a5019b0-0528-46c4-b80c-64ebe7d01444" />

---

## 📈 Advantages

* Helps beginners understand code easily
* Supports Telugu language learners
* Reduces fear of programming
* Simple and interactive UI
* No need for local GPU

---

## ⚠️ Limitations

* Telugu explanation requires internet connection
* API-based model may have slight latency
* Best suited for small to medium code snippets

---

## 🔮 Future Enhancements

* Support for more Indian languages
* Voice-based explanations
* Mobile-friendly UI
* Syntax highlighting
* Support for more programming languages

---

## 🎓 Educational Impact

This project:

* Promotes inclusive learning
* Encourages regional-language education
* Demonstrates real-world NLP application
* Bridges the gap between AI and education

---

## 🧾 Conclusion

The **NLP Code Explainer — English & Telugu** project successfully demonstrates how modern NLP models can be applied to make programming education more accessible and inclusive.
By combining AI, multilingual support, and an interactive interface, the system empowers learners to understand code conceptually rather than memorizing syntax.

---






