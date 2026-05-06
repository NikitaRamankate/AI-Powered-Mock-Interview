# AI-Powered-Mock-Interview
# 🎤 AI-Powered Mock Interview Platform

<div align="center">

🚀 An AI-powered full-stack mock interview platform that simulates real technical interviews with voice interaction, live coding, AI evaluation, and performance analytics.

<img src="https://img.shields.io/badge/Frontend-React-blue?style=for-the-badge&logo=react" />
<img src="https://img.shields.io/badge/Backend-Node.js-green?style=for-the-badge&logo=node.js" />
<img src="https://img.shields.io/badge/Database-MongoDB-darkgreen?style=for-the-badge&logo=mongodb" />
<img src="https://img.shields.io/badge/AI-Gemini-orange?style=for-the-badge&logo=google" />
<img src="https://img.shields.io/badge/Voice-MurfAI-purple?style=for-the-badge" />
<img src="https://img.shields.io/badge/STT-AssemblyAI-red?style=for-the-badge" />

</div>

---

# 🧠 Overview

The **AI-Powered Mock Interview Platform** helps students and job seekers practice technical interviews in a realistic AI environment.

It generates personalized interview questions from resumes, conducts voice-based interviews, evaluates coding submissions, and provides intelligent AI feedback with scoring and analytics.

---
# 🏗 System Architecture

```bash
┌───────────────────────────────────────────────────────────────┐
│                      ⚛ React Frontend                         │
│                                                               │
│   ┌────────────┐  ┌────────────┐  ┌────────────┐             │
│   │ Setup Page │→ │ Interview  │→ │ Feedback   │             │
│   │            │  │   Page     │  │   Page     │             │
│   └────────────┘  └────────────┘  └────────────┘             │
│            ↓                ↓                 ↓               │
│   ┌───────────────────────────────────────────────┐          │
│   │         📡 Axios API Service Layer             │          │
│   └───────────────────────────────────────────────┘          │
└───────────────────────────┬───────────────────────────────────┘
                            │
                     🌐 HTTP REST API
                            │
┌───────────────────────────┴───────────────────────────────────┐
│                     🚂 Express Backend                         │
│                                                               │
│   ┌──────────┐   ┌────────────┐   ┌──────────┐               │
│   │  Routes  │ → │ Controllers│ → │ Services │               │
│   └──────────┘   └────────────┘   └──────────┘               │
│                                              ↓                │
│                                      ┌────────────┐           │
│                                      │  Models    │           │
│                                      └────────────┘           │
│                                                               │
│   ┌───────────────────────────────────────────────────────┐   │
│   │              🤖 External AI Services                  │   │
│   │                                                       │   │
│   │   ┌─────────┐   ┌──────────┐   ┌──────────────┐      │   │
│   │   │ Gemini  │   │ Murf AI  │   │ AssemblyAI  │      │   │
│   │   │   LLM   │   │   TTS    │   │    STT      │      │   │
│   │   └─────────┘   └──────────┘   └──────────────┘      │   │
│   └───────────────────────────────────────────────────────┘   │
│                                                               │
│                            ↓                                  │
│   ┌───────────────────────────────────────────────────────┐   │
│   │                🍃 MongoDB Atlas                       │   │
│   │                                                       │   │
│   │   ┌──────────┐  ┌──────────────┐  ┌────────────┐     │   │
│   │   │  Users   │  │ Interviews   │  │  Resumes   │     │   │
│   │   └──────────┘  └──────────────┘  └────────────┘     │   │
│   └───────────────────────────────────────────────────────┘   │
└───────────────────────────────────────────────────────────────┘
```

## 🧠 Architecture Flow

1️⃣ User uploads resume from React frontend  
2️⃣ Backend parses resume and stores data in MongoDB  
3️⃣ Gemini AI generates interview questions  
4️⃣ Murf AI converts questions into voice  
5️⃣ User answers through voice or code editor  
6️⃣ AssemblyAI converts voice to text  
7️⃣ Gemini evaluates answers and generates feedback  
8️⃣ Interview history and analytics are stored in MongoDB  


# ✨ Features

## 📄 Resume-Based Question Generation
- Upload PDF resumes
- AI analyzes resume content
- Personalized interview flow generation

## 🎙 AI Voice Interviewer
- Realistic AI interviewer voice
- Voice-based interaction
- Natural interview experience

## 🗣 Speech-to-Text
- Convert spoken answers into text
- Powered by AssemblyAI
- Real-time transcription support

## 💻 Live Coding Interview
- Monaco code editor integration
- Solve coding problems live
- AI evaluates submitted code

## 🤖 AI Evaluation & Feedback
- Detailed interview analysis
- Performance scoring
- Strengths & improvement areas

## 📊 Dashboard & History
- Interview analytics
- Previous interview history
- Resume incomplete interviews

## 🔐 Authentication System
- Secure login/signup
- JWT authentication
- Protected routes

---

# 📸 Screenshots

## 🏠 Home Dashboard
<## 🏠 Home Dashboard
<img width="100%" alt="Home Dashboard" src=""C:\Users\nikit\OneDrive\Pictures\Screenshots\Records interview.png"">

---

## 🎤 AI Interview Page
<img width="100%" alt="Interview" src="https://via.placeholder.com/1200x600.png?text=AI+Interview+Page">

---

## 📊 Feedback & Analytics
<img width="100%" alt="Feedback" src="https://via.placeholder.com/1200x600.png?text=Feedback+Analytics">

---

# 🛠 Tech Stack

## 🎨 Frontend
- ⚛ React.js
- 🛣 React Router
- 📡 Axios
- 💻 Monaco Editor
- 🎨 CSS3

## ⚙ Backend
- 🟢 Node.js
- 🚂 Express.js
- 🍃 MongoDB
- 📦 Mongoose

## 🤖 AI Services
- 🧠 Google Gemini API
- 🎤 Murf AI (Text-to-Speech)
- 🗣 AssemblyAI (Speech-to-Text)

---

# 📂 Project Structure

```bash
AI-Mock-Interview-Platform/
│
├── client/                 # Frontend React Application
│
├── server/                 # Backend Express Server
│
├── screenshots/            # Project screenshots
│
├── README.md
│
└── package.json
```

---

# ⚙️ Installation

## 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/ai-mock-interview-platform.git
```

---

## 2️⃣ Navigate to Project

```bash
cd ai-mock-interview-platform
```

---

# 🔧 Backend Setup

## Install Dependencies

```bash
cd server
npm install
```

---

## Create `.env` File

```env
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
GEMINI_API_KEY=your_gemini_api_key
ASSEMBLYAI_API_KEY=your_assemblyai_api_key
MURF_API_KEY=your_murf_api_key
```

---

## ▶ Run Backend Server

```bash
npm run dev
```

---

# 💻 Frontend Setup

## Install Dependencies

```bash
cd client
npm install
```

---

## ▶ Run Frontend

```bash
npm run dev
```

---

# 🚀 Workflow

## 📄 Resume Upload
Upload your resume in PDF format.

## 🧠 AI Generates Questions
Gemini AI creates personalized interview questions.

## 🎤 Voice Interview
AI interviewer asks questions using realistic voice.

## 💻 Coding Round
Solve coding problems using Monaco Editor.

## 📊 Feedback Generation
Receive detailed AI-generated interview analysis.

---

# 📡 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/auth/login` | User login |
| POST | `/api/auth/register` | User registration |
| POST | `/api/resume/upload` | Upload resume |
| POST | `/api/interview/start` | Start interview |
| POST | `/api/interview/:id/answer` | Submit answer |
| POST | `/api/interview/:id/code` | Submit code |
| GET | `/api/history` | Interview history |

---

# 🌟 Key Functionalities

✅ Resume Parsing  
✅ AI Interview Questions  
✅ Voice Recording  
✅ Speech-to-Text  
✅ AI Voice Responses  
✅ Live Coding Challenges  
✅ AI Code Evaluation  
✅ Feedback Analytics  
✅ Interview History Tracking  

---

# 🔐 Privacy & Security

- 🔒 Secure JWT authentication
- 📁 User data protection
- ☁ No unnecessary data sharing
- 🛡 Protected backend routes

---

# 🔮 Future Enhancements

- 🎥 Video interview support
- 😊 Emotion detection
- 🌍 Multi-language interviews
- 🧠 AI interviewer avatar
- 📈 Advanced analytics
- 🏆 Leaderboards

---

# 🧪 Tested On

✅ Windows 11  
✅ Ubuntu  
✅ macOS  

---

# 👩‍💻 Author

## Nikita Ramankate

💡 B.Tech CSE (Computer Science & Business Systems)  
🚀 Full Stack Developer  
🤖 AI & Web Development Enthusiast  

---

# 🤝 Contributing

Contributions are welcome!

```bash
Fork the repository
Create your feature branch
Commit your changes
Push to the branch
Create a Pull Request
```

---

# ⭐ Support

If you like this project, give it a ⭐ on GitHub!

---

# 📜 License

This project is developed for educational and learning purposes.

---

<div align="center">

### 🚀 Built with AI + Full Stack Development

</div>
