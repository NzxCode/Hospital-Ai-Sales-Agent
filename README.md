# 🏥 Hospital AI Sales Agent

An AI-powered WhatsApp sales and patient engagement agent designed for hospitals and healthcare providers.

This system automates patient communication, lead qualification, appointment scheduling, and follow-up processes using Large Language Models (LLMs), memory management, and healthcare-specific conversation workflows.

---

## 📋 Overview

Hospital AI Sales Agent helps healthcare organizations improve patient acquisition and operational efficiency by providing an intelligent conversational assistant available 24/7.

The agent can:

- Respond to patient inquiries automatically
- Qualify potential patients based on predefined criteria
- Schedule appointments
- Maintain conversation context using memory
- Handle WhatsApp interactions through Evolution API
- Provide personalized responses using AI

---

## 🚀 Key Features

### 🤖 AI-Powered Patient Engagement

- Natural language conversations
- Context-aware responses
- Personalized patient interactions
- Healthcare-focused communication

### 📅 Appointment Scheduling

- Schedule consultation requests
- Collect patient information
- Manage booking workflows
- Reduce manual administrative work

### 🎯 Lead Qualification

- Identify potential patients
- Gather required information
- Prioritize high-value inquiries
- Improve conversion rates

### 🧠 Long-Term Memory

- Store conversation history
- Maintain patient context
- Deliver personalized follow-ups

### 💬 WhatsApp Integration

- Receive incoming messages
- Send automated responses
- Real-time communication via Evolution API

### 📊 Data Persistence

- SQLite database integration
- Conversation tracking
- Appointment storage

---

## 🏗️ System Architecture

```text
Patient
   │
   ▼
WhatsApp
   │
   ▼
Evolution API
   │
   ▼
FastAPI Webhook
   │
   ├── AI Agent
   ├── Memory Engine
   ├── Scheduling Engine
   └── Database Layer
   │
   ▼
Response to Patient
```

---

## 🛠️ Tech Stack

### Backend

- Python
- FastAPI

### AI

- OpenAI API
- LLM-based conversational workflows

### Database

- SQLite

### Integration

- Evolution API (WhatsApp)

### Development Tools

- Git
- GitHub
- VS Code

---

## 📁 Project Structure

```text
Hospital-AI-Sales-Agent/
│
├── agent.py
├── database.py
├── memory.py
├── whatsapp.py
├── tools.py
├── main.py
│
├── prompts/
│   └── system.md
│
├── requirements.txt
├── .env.example
└── README.md
```

---

## ⚙️ Installation

Clone repository:

```bash
git clone https://github.com/NzxCode/Hospital-Ai-Sales-Agent.git
cd Hospital-Ai-Sales-Agent
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Configure environment variables:

```env
OPENAI_API_KEY=your_api_key
EVOLUTION_API_URL=your_url
EVOLUTION_API_TOKEN=your_token
```

Run application:

```bash
python main.py
```

or

```bash
uvicorn main:app --reload
```

---

## 🔄 Workflow

1. Patient sends WhatsApp message
2. Evolution API forwards event to FastAPI webhook
3. AI Agent processes the message
4. Memory system retrieves previous context
5. Agent generates personalized response
6. Response is sent back through WhatsApp
7. Conversation is stored in database

---

## 🎯 Business Impact

This solution helps hospitals:

- Reduce response times
- Increase patient engagement
- Automate repetitive administrative tasks
- Improve lead conversion
- Provide 24/7 patient support
- Scale patient communication efficiently

---

## 🔒 Security Considerations

- Environment variables stored outside source code
- Sensitive credentials excluded using `.gitignore`
- Database files excluded from repository

---

## 📈 Future Improvements

- CRM Integration
- Multi-agent architecture
- Analytics dashboard
- Voice assistant support
- Multi-language support
- PostgreSQL migration
- Docker deployment

---

## 👨‍💻 Author

Developed by **NzxCode**

AI Solutions • Automation • Healthcare Technology

---

## 📄 License

MIT License
