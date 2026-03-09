# Media-GenAI---Real-time-Speech-to-Speech

Real-time Speech-to-Speech Translator — AI-powered system for transcribing, translating, and vocalizing multilingual audio using Whisper, Google Translate, and gTTS. 

🎧 Media-Gen AI Speech Translator — Real-time Speech & Video Translation App


🌍 Translate spoken words from audio, video, or microphone input into 12 Indian languages — all powered by OpenAI Whisper, Google Translate, and Flask + ngrok for a seamless web experience.

🚀 Project Overview

Whisper Translator is an end-to-end multilingual audio and video translation web app.
It lets you:

🎙 Record audio directly from your mic
🎬 Upload video or audio files
🌐 Transcribe & translate speech into multiple Indian languages
🗣 Listen to the translated output with Text-to-Speech (TTS)
💻 Access it instantly via a secure ngrok public URL

This project combines AI speech recognition, machine translation, and speech synthesis — creating a complete real-time translation pipeline.

🧠 Tech Stack
Component	Description
🧩 Whisper (OpenAI)	Speech recognition & transcription
🌐 Google Translate	Text translation to 12+ Indian languages
🔊 gTTS	Text-to-Speech synthesis
🎬 MoviePy	Audio extraction from videos
🧱 Flask	Lightweight web backend
⚡ Ngrok	Public URL tunneling for Flask server

🔹 Supported Languages
| Language | Code | Language  | Code |
| -------- | ---- | --------- | ---- |
| English  | en   | Marathi   | mr   |
| Hindi    | hi   | Gujarati  | gu   |
| Bengali  | bn   | Punjabi   | pa   |
| Tamil    | ta   | Nepali    | ne   |
| Telugu   | te   | Assamese  | as   |
| Kannada  | kn   | Malayalam | ml   |

📦 Installation Guide

🧰 1. Clone the Repository
cd whisper-translator

⚙️ 2. Install Dependencies

Create a requirements.txt file (or use the one below 👇):

SpeechRecognition
googletrans==4.0.0-rc1
gTTS
pydub
moviepy
soundfile
openai-whisper
flask
flask-ngrok
pyngrok


Then install:

pip install -r requirements.txt

🔑 3. Set Ngrok Auth Token

Replace the placeholder in your code:

NGROK_AUTH_TOKEN = "your_own_token_here"


💡 Get your free token from https://dashboard.ngrok.com

🧠 How It Works
flowchart LR
A[🎙 Audio / 🎬 Video / 🎧 Mic Input] --> B[🎛 Whisper Transcription]
B --> C[🌐 Google Translate]
C --> D[🔊 gTTS Speech Generation]
D --> E[💻 Flask Web App Interface]
E --> F[🌍 ngrok Public Access]

💻 Running the App
python app.py


After running, you’ll see something like:

🌐 Public URL: https://abcd1234.ngrok.io
✅ Whisper model loaded!


Open the given URL in your browser to access the Whisper Translator UI.

🎨 Web Interface Preview

✨ Features:

Glassmorphism UI with gradient backgrounds

File uploads for audio & video

Live microphone recording

Real-time translation and playback

Example UI
(auto-generated HTML in index.html)

🔍 Example Usage
🎬 Translate a Video

Upload a .mp4 or .mkv file

The app extracts audio → transcribes → translates → plays TTS

🎙 Live Mic Recording

Click Start Recording

Speak in any language

Wait for automatic translation and TTS playback

⚡ Output Example
Step	Description	Example
🗣️ Transcription	Detected speech text	“Hello, how are you?”
🌐 Translation (Hindi)	Translated text	“नमस्ते, आप कैसे हैं?”
🔊 TTS Output	Spoken translation	Audio playback in Hindi
📁 Project Structure
whisper-translator/
├── app.py                # Main Flask application
├── MIT-license           # LIcense
├── index.html            # Web frontend
├── requirements.txt      # Python dependencies
└── README.md             # Documentation

🧩 Future Enhancements

🎤 Add real-time streaming transcription

🧠 Integrate speaker diarization

📱 Deploy as a mobile app (Flutter or React Native)

📈 Add voice emotion detection

🛡 License

This project is licensed under the MIT License — feel free to use and modify it.

 Acknowledgements

OpenAI Whisper

Google Translate API

gTTS – Google Text-to-Speech

Flask

MoviePy

✨ Developed with love using Whisper + Flask + Google Translate ✨
