# Voice Assistant — Whisper + Llama + TTS 🎙️

An experiment notebook where I built a **voice chatbot pipeline** end to end and tried several speech and LLM APIs:

```text
🎤 speech ──▶ Whisper large-v3 (Groq) ──▶ text ──▶ Llama 3.1 70B (Groq) ──▶ reply ──▶ gTTS / Deepgram Aura ──▶ 🔊 speech
```

> This is a prototype and learning notebook with Gradio and Streamlit UIs, not a production app.

## 🧪 What's inside

| Section | What it does |
|---|---|
| **Gemini** | Text and multi-turn chat with Gemini, plus Streamlit chat UIs |
| **Deepgram** | Text-to-speech with the Deepgram Aura voice API |
| **Whisper** | Speech-to-text with `whisper-large-v3` on Groq, connected to Llama 3.1 replies and gTTS speech output |
| **Gradio UIs** | Microphone/audio input → transcription → chatbot reply → spoken answer |
| **Groq chat** | Llama chat with short conversation memory (last 5 turns) |
| **Hugging Face** | Text generation through Hugging Face Hub, served with a small FastAPI endpoint |

## 💻 Stack

Python · Groq API (Whisper large-v3, Llama 3.1) · Google Gemini · Deepgram · gTTS · Gradio · Streamlit · FastAPI · Hugging Face Hub

## 🔑 Setup

API keys are read from environment variables, so none are stored in the notebook:

```bash
export GROQ_API_KEY=...
export GOOGLE_API_KEY=...
export DEEPGRAM_API_KEY=...
export HUGGINGFACEHUB_API_TOKEN=...
```

Then open `voice_assistant_whisper_llama.ipynb` in Jupyter or Colab and run the section you want.
