# 🌾 Grameen-AI  
### Multi-Lingual Conversational Financial Assistant for Rural India

---

## 📌 Overview
**Grameen-AI** is an intelligent conversational AI system designed to assist rural users in India—especially in regions like Punjab—with financial awareness and access to government schemes.

It combines:
- Speech recognition  
- Multi-lingual translation  
- Intent detection  
- Rule-based decision logic  
- Large Language Model (LLM) explanations  

to deliver **accurate, simple, and context-aware responses** in the user’s native language.

---

## 🚀 Features

### 🌐 Multi-Lingual Support
- Supports native languages such as **Punjabi** and **Hindi**
- Provides responses in the user’s chosen language

### 🎤 Speech-to-Text
- Converts spoken audio into text using **Google Web Speech API**

### 🎧 Audio Format Flexibility
- Accepts multiple formats: `.mp3`, `.m4a`, `.flac`, `.ogg`
- Automatically converts audio to **WAV** for processing

### 🧠 Intent Detection
- Uses **priority-based regex classification**
- Detects intents like:
  - Scam Check  
  - Scheme Eligibility  
  - Loan Education  

### 🔄 Rule-Based Flow Management
- Guides users through structured Q&A flows
- Dynamically collects required information

### ⚙️ Deterministic Backend Logic
- Applies predefined rules to:
  - Check eligibility  
  - Suggest schemes  
  - Provide actionable steps  

### 🤖 LLM-Powered Explanations
- Uses **Gemini API** to:
  - Simplify technical results  
  - Provide culturally relevant explanations  
  - Improve user understanding  

### 🌍 Content Localization
- Translates final responses back to the user’s preferred language

---

## ⚙️ How It Works

1. **Language Selection**  
   User selects source and target languages  

2. **Audio Input**  
   User uploads a voice query  

3. **Speech Recognition**  
   Audio → Text (source language)  

4. **Translation to English**  
   For consistent processing  

5. **Intent Identification**  
   Regex-based classification determines user intent  

6. **Flow-Based Interaction**  
   System asks follow-up questions  

7. **Backend Processing**  
   Rule engine generates factual results  

8. **LLM Explanation**  
   Gemini API converts results into simple explanations  

9. **Final Translation**  
   Output is translated back to user’s language  

---

## 🛠️ Setup & Dependencies

### Requirements
- Python 3.x  
- `SpeechRecognition`  
- `pydub`  
- `googletrans`  
- `google-generativeai`  

### Additional Tools
- **ffmpeg** (required for audio processing)

### API Configuration
- A **Google Gemini API Key** is required  
- Configure it using **Colab Secrets Manager** or environment variables  

---

## ▶️ Usage

1. Provide an audio query in your preferred language  
2. The system processes and understands your request  
3. Answer follow-up questions (if any)  
4. Receive:
   - Financial guidance  
   - Scheme eligibility  
   - Simple explanations  

All responses are delivered in your chosen language for easy understanding.

---

## 🎯 Goal

To bridge the financial knowledge gap in rural India by making:
- Government schemes accessible  
- Financial education understandable  
- Technology usable in local languages  

---
