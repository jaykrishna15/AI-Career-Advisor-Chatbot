# 🎓 AI Career Advisor Chatbot  
### Production-Ready Domain-Specific Chatbot using Google Gemini API

---

## 📌 Project Overview

The **AI Career Advisor Chatbot** is a production-ready, domain-specific conversational AI application built using **Google Gemini GenAI API** and **Streamlit**.

The chatbot provides structured and professional career guidance including:

- Career path suggestions  
- Skill gap analysis  
- Learning roadmaps  
- Certification recommendations  
- Interview preparation tips  
- Industry insights  

This project follows clean architecture principles, modular backend design, logging, exception handling, and advanced token optimization.

---

## 🏗 System Architecture

The application follows a modular architecture:
 ```bash
User
↓
Streamlit UI
↓
Chatbot Layer (Orchestration)
↓
Prompt Engineering Module
↓
Gemini API Client
↓
Response Processing Layer
↓
UI Rendering
 ```

 
---

## 🧱 Architecture Breakdown

### 1️⃣ UI Layer (`app.py`)
- Chat-style interface  
- Session-based conversation  
- Displays history  
- Loading indicators  
- Avatar support  

---

### 2️⃣ Chatbot Layer (`backend/chatbot.py`)
- Handles user input  
- Applies token optimization  
- Controls conversation flow  
- Calls Gemini client  
- Stores conversation history  

---

### 3️⃣ Prompt Engineering Layer (`backend/prompt_manager.py`)
- Defines system prompt  
- Implements career-only guardrails  
- Structures contextual prompt  

---

### 4️⃣ Gemini API Layer (`backend/gemini_client.py`)
- Secure API integration  
- Configurable generation parameters  
- Response validation and cleanup  
- Exception handling  
- Logging  

---

### 5️⃣ Memory Manager (`backend/memory_manager.py`)
- Multi-turn conversation memory  
- History limiting  
- Prevents prompt overflow  

---

### 6️⃣ Logging System (`backend/logger.py`)
- API call logging  
- Error logging  
- System event tracking  
- Persistent log file (`logs/app.log`)  

---

### 7️⃣ Configuration (`config/settings.py`)
- Model configuration  
- Temperature control  
- Output token limits  
- No hardcoded secrets  

---

## 🚀 Key Features

- ✅ Domain-specific AI Career Advisor  
- ✅ Multi-turn conversation memory  
- ✅ Advanced token optimization  
- ✅ Prompt guardrails (career-only restriction)  
- ✅ Response processing layer  
- ✅ Exception handling  
- ✅ Logging system  
- ✅ Modular architecture  
- ✅ Secure API key handling  

---

## 🛠 Tech Stack

- Python  
- Streamlit  
- Google Gemini GenAI API  
- Python-dotenv  
- Logging module  

---

## 📂 Project Structure
```bash
career-advisor-chatbot/
│
├── assets/
│ ├── chatbot.png
│ └── user.png
│
├── backend/
│ ├── chatbot.py
│ ├── gemini_client.py
│ ├── memory_manager.py
│ ├── prompt_manager.py
│ └── logger.py
│
├── config/
│ └── settings.py
│
├── logs/
│ └── app.log
│
├── .env
├── .gitignore
├── app.py
└── README.md
```


---

## ⚙️ Setup Instructions

### 1️⃣ Clone Repository

```bash
git clone <your-repository-link>
cd career-advisor-chatbot
```

### 2️⃣ Create Virtual Environment
```bash
python -m venv myenv
```

#### Activate environment:

Windows
```bash
myenv\Scripts\activate
```
Mac/Linux
```bash
source myenv/bin/activate
```

### 3️⃣ Install Dependencies
```bash
pip install streamlit google-generativeai python-dotenv
```
(Optional: create a requirements.txt)

### 4️⃣ Add Gemini API Key

Create .env file in root directory:
```bash
GEMINI_API_KEY=your_api_key_here
```

### 5️⃣ Run Application
```bash
streamlit run app.py
```

## 🔐 Security Practices

* API keys stored in .env

* No hardcoded credentials

* Modular API handling

* Log-based debugging instead of console prints

## 📈 Production Enhancements Implemented

* Structured prompt engineering

* Guardrails for domain restriction

* Advanced token optimization

* Response validation and trimming

* Logging of API calls and errors

* Graceful exception handling

* Clean architecture design

## 🚧 Future Improvements

* AWS EC2 Deployment

* Docker containerization

* Authentication layer

* Monitoring dashboard

Usage analytics

## 📊 Project Status

✔ Production-structured
✔ Modular and scalable
✔ Technically complete
✔ Deployment-ready

## 👨‍💻 Author
* Jaya Krishna Golla
* AI Career Advisor Chatbot
* Built using Google Gemini API
