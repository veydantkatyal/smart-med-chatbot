# Smart Medical Chatbot

**Smart Med Chatbot** is an AI-powered medical assistant designed to handle basic health-related queries using voice, vision, and intelligent reasoning. It leverages natural language processing (NLP), speech recognition, and machine learning to provide a multi-modal, interactive healthcare support experience. This project is ideal for early triage, general medical awareness, and patient engagement.

---

## Installation Guide of FFmpeg and PortAudio

- Check out the step-by-step installation guide to install required dependencies to run this chatbot locally on your system on gradio and check live working end to end implementation of this chatbot.
- Link to guide: [Link](https://github.com/AIwithhassan/ai-doctor-2.0-voice-and-vision)

---

## Features

- **AI Medical Brain** – Uses NLP to interpret and respond to user symptoms intelligently.
- **Voice Input/Output** – Converts voice to text and text back to voice using TTS/STT engines.
- **Vision Capability** – Supports image-based symptom identification (e.g., skin conditions).
- **Gradio Web Interface** – Simple and interactive frontend powered by Gradio.
- **Text-to-Speech Playback** – Audio feedback to enhance accessibility and UX.
- **Offline Ready** – Works without cloud dependencies for improved privacy.

---

## Project Structure
<pre lang="markdown"> 
  smart-med-chatbot/ 
  ├── doctor_brain.py # Core logic for medical response generation 
  ├── doctor_voice.py # Text-to-speech conversion logic 
  ├── patient_voice.py # Speech-to-text input processing 
  ├── gradio_app.py # Gradio frontend implementation 
  ├── elevenlabs_testing.mp3 # Audio test for ElevenLabs API (TTS) 
  ├── elevenlabs_testing_autoplay.mp3 
  ├── gtts_testing.mp3 # Audio test for Google TTS 
  ├── gtts_testing_autoplay.mp3 
  └── README.md # Project documentation </pre>

---

## Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/veydantkatyal/smart-med-chatbot.git
cd smart-med-chatbot
```

### 2. Set Up Environment with Pipenv (Recommended)

```bash
pip install pipenv
pipenv install
pipenv shell
```
or use pip directly:
```bash
pip install -r requirements.txt 
```

### 3. Run the Application

```bash
python gradio_app.py
```
---

## How It Works

- **User Input**: User speaks or types their medical query.
- **Speech Recognition**: patient_voice.py processes the voice input to text.
- **NLP Processing**: doctor_brain.py analyzes the text and forms a response.
- **TTS Output**: doctor_voice.py reads out the reply using a TTS engine.
- **Gradio Interface**: gradio_app.py binds all components into a user interface.

---

## Example Use Case
- User: "I have a sore throat and fever."
- Bot: "You may be experiencing a viral infection. Please stay hydrated and monitor your symptoms. If it persists, consult a doctor."
- Bot speaks the response

---

## Future Improvements

1. GPT-based diagnosis reasoning
2. Wearable health device integration
3. Multilingual voice support
4. Real-time skin image classification (CNNs)
5. Symptom tracking and exportable reports

---
### This project is licensed under [MIT License](https://github.com/veydantkatyal/smart-med-chatbot/blob/main/LICENSE)
