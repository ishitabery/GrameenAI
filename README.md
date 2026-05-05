# GrameenAI
Multilingual AI Chatbot for Financial Literacy and Rural Empowerment
```markdown
# Grameen-AI: Multi-Lingual Conversational Financial Assistant for Rural India

## Overview
Grameen-AI is an intelligent conversational AI system designed to assist rural users in India, particularly in the Punjab region, with financial information and government schemes. It leverages speech recognition, multi-lingual translation, intent detection, and a rule-based backend to provide accurate and context-aware responses, explained in a simple and understandable manner by a large language model.

## Features

*   **Multi-Lingual Support:** Interacts with users in their native language (e.g., Punjabi, Hindi) and provides explanations in the chosen language.
*   **Speech-to-Text:** Converts spoken audio input into text using Google's Web Speech API.
*   **Audio Format Flexibility:** Handles various audio formats (.mp3, .m4a, .flac, .ogg) and converts them to WAV for processing.
*   **Intent Detection:** Utilizes a priority-based, regex-driven intent classification system to accurately identify user needs (e.g., Scam Check, Scheme Eligibility, Loan Education).
*   **Rule-Based Flow Management:** Guides users through structured question-and-answer flows based on detected intent, collecting necessary information.
*   **Deterministic Backend Logic:** Processes collected user data against predefined rules to determine eligibility for schemes, provide application steps, or deliver specific information.
*   **LLM-Powered Explanations:** Employs the Gemini API to generate simplified, culturally relevant explanations of backend decisions, ensuring clarity for rural users.
*   **Content Localization:** Translates LLM-generated explanations back into the user's chosen target language.

## How It Works

1.  **Language Selection:** The user specifies their source and target languages.
2.  **Audio Input:** The user uploads an audio file containing their query.
3.  **Speech Recognition:** The audio is converted to text in the source language.
4.  **Translation to English:** The recognized text is translated into English for intent detection.
5.  **Intent Identification:** A regex-based system identifies the user's intent (e.g., asking about a loan, eligibility for a scheme).
6.  **Flow Binding & Questioning:** Based on the intent, the system enters a specific conversational flow, asking follow-up questions to gather more details.
7.  **Backend Processing:** Once all necessary information is collected, a deterministic rule engine processes the answers to generate a factual result (e.g., a list of eligible schemes, loan education topic).
8.  **LLM Explanation:** The backend result is fed to the Gemini LLM, which generates a simple, easy-to-understand explanation tailored for rural users.
9.  **Final Translation:** The LLM's explanation is translated back into the user's chosen target language (e.g., Punjabi) and presented to the user.

## Setup and Dependencies

This project requires Python 3 and several libraries, including `SpeechRecognition`, `pydub`, `googletrans`, and `google-generativeai`. `ffmpeg` is also required for audio processing. An API key for the Google Gemini API is necessary and should be configured in Colab's secrets manager.

## Usage

Users interact with the system by providing audio input in their preferred language. The system then guides them through a series of questions and provides relevant information and explanations in their chosen language.
```
