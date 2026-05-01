🤖 AI Interviewer Pro
An intelligent AI-powered interview simulation platform built with React, Python, and integrated with OpenAI & Google Gemini APIs.

📌 About the Project
AI Interviewer Pro is a full-stack AI interview preparation platform developed by Yugantara Pathak. It simulates a real-world on-camera job interview experience using cutting-edge AI models. The application asks dynamic interview questions, listens to your answers via microphone, evaluates your responses in real-time, and generates a comprehensive performance report — all powered by OpenAI and Google Gemini.

Whether you're preparing for your first job or leveling up for a senior role, AI Interviewer Pro gives you a realistic, data-driven mock interview experience from the comfort of your browser.

👨‍💻 Developed By
Field	Details
Developer	Yugantara Pathak
Frontend	React.js
Backend	Python (FastAPI / Flask)
AI Models	OpenAI GPT, Google Gemini 2.0 Flash
Type	Full-Stack AI Web Application
<img width="748" height="527" alt="ai interview photo 2" src="https://github.com/user-attachments/assets/335513b2-411d-478d-9fa9-2b2b6dbaf6f1" />

✨ Key Features
🎯 On-Camera AI Interview — Real-time interview simulation with animated AI avatar

🤖 Gemini AI Feedback — Live response evaluation using Google Gemini 2.0 Flash API

🧠 OpenAI Integration — GPT-powered question generation and answer analysis

📊 Live Performance Scoring — Real-time scoring across Communication, Technical, Confidence, and Clarity

🎤 Voice Recognition — Speak your answers via Web Speech API

🔊 AI Voice Output — AI interviewer speaks questions aloud using Speech Synthesis

📄 Resume Upload — Upload your resume to get personalized, tailored interview questions

📈 Final Report — Comprehensive AI-generated report with strengths and improvement areas

💾 Transcript Export — Download the full Q&A session as a .txt file

🌗 Dark / Light Mode — Full theme toggle support

📹 Camera Integration — Live webcam feed with recording indicator

🛠️ Tech Stack
Frontend
text
React.js          → UI components and state management
HTML5 / CSS3      → Custom animations, responsive layout
Web Speech API    → Voice input and AI speech output
Fetch API         → REST calls to backend and AI APIs
Backend
text
Python            → Core backend logic
FastAPI / Flask   → REST API server
Uvicorn           → ASGI server for FastAPI
AI / APIs
text
Google Gemini 2.0 Flash   → Real-time answer evaluation, question generation
OpenAI GPT                → Intelligent question bank, response scoring
🚀 Getting Started
Prerequisites
Node.js >= 18

Python >= 3.10

OpenAI API Key

Google Gemini API Key

1. Clone the Repository
bash
git clone https://github.com/yugantarapathak/ai-interviewer-pro.git
cd ai-interviewer-pro
2. Backend Setup
bash
cd backend
pip install -r requirements.txt
cp .env.example .env
# Add your API keys in .env
uvicorn main:app --reload
3. Frontend Setup
bash
cd frontend
npm install
npm start
4. Environment Variables
Create a .env file in the backend directory:

text
OPENAI_API_KEY=your_openai_api_key_here
GEMINI_API_KEY=your_gemini_api_key_here
SECRET_KEY=your_secret_key
📂 Project Structure
text
ai-interviewer-pro/
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── AvatarOrb.jsx
│   │   │   ├── ChatFeed.jsx
│   │   │   ├── ScorePanel.jsx
│   │   │   ├── CameraFeed.jsx
│   │   │   └── ReportModal.jsx
│   │   ├── hooks/
│   │   │   ├── useSpeechRecognition.js
│   │   │   └── useGemini.js
│   │   ├── App.jsx
│   │   └── index.js
│   └── package.json
│
├── backend/
│   ├── main.py
│   ├── routes/
│   │   ├── interview.py
│   │   └── analysis.py
│   ├── services/
│   │   ├── gemini_service.py
│   │   └── openai_service.py
│   ├── requirements.txt
│   └── .env.example
│
└── README.md
🔌 API Integrations
Google Gemini 2.0 Flash
Used for:

Real-time answer evaluation and scoring

Resume-based personalized question generation

Final performance report generation

python
import google.generativeai as genai

genai.configure(api_key=GEMINI_API_KEY)
model = genai.GenerativeModel("gemini-2.0-flash")
response = model.generate_content(prompt)
OpenAI GPT
Used for:

Dynamic interview question generation

Deep semantic answer analysis

Constructive feedback generation

python
from openai import OpenAI

client = OpenAI(api_key=OPENAI_API_KEY)
response = client.chat.completions.create(
    model="gpt-4",
    messages=[{"role": "user", "content": prompt}]
)
📸 Screenshots
Coming Soon — UI screenshots will be added after deployment

🤝 Contributing
Contributions are welcome! Please follow these steps:

Fork the repository

Create a new branch: git checkout -b feature/your-feature

Commit your changes: git commit -m 'Add your feature'

Push to the branch: git push origin feature/your-feature

Open a Pull Request

📄 License
This project is licensed under the MIT License — see the LICENSE file for details.

🙌 Acknowledgements
Google Gemini API

OpenAI API

React.js

FastAPI

Web Speech API

<div align="center">

Made with ❤️ by Yugantara Pathak

⭐ Star this repo if you found it helpful!

</div>
