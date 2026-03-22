# 🤖 Digital Twin AI Agent — C Tejesh

> An AI-powered personal agent that talks like me, knows my background through RAG, and helps with real daily tasks using 6 custom tools.

Built at **RVITM Bengaluru** as part of a hackathon by **Team Titanic**.

---

## 🎯 What It Does

This project is a **Digital Twin** — an AI version of me (Tejesh) that:
- Answers questions about my background, skills, and projects using **RAG**
- Performs real-world tasks using **6 custom tools**
- Speaks in my personality via a custom system prompt
- Runs as an interactive chat UI built with **Gradio**

---

## 🏗️ Architecture

```
User Query
    │
    ▼
┌─────────────────────────────────┐
│        Digital Twin Agent       │
│                                 │
│  Personal Query → RAG Retrieve  │
│       ↓               ↓        │
│  ChromaDB         Resume Chunks │
│       ↓               ↓        │
│      LLM (Groq — LLaMA)        │
│       ↓                         │
│  Tool Call? → Execute Tool      │
│       ↓                         │
│   Final Answer                  │
└─────────────────────────────────┘
```

---

## 🔧 Tech Stack

| Component | Technology |
|---|---|
| Framework | LangChain |
| LLM | Groq (openai/gpt-oss-20b) |
| Embeddings | Google Gemini (gemini-embedding-001) |
| Vector Store | ChromaDB |
| Knowledge Base | Resume as RAG |
| UI | Gradio |

---

## 🛠️ Tools Built

| Tool | Description |
|---|---|
| 🧮 Scientific Calculator | Evaluates math — arithmetic, trig, log, factorial |
| 🌦️ Live Weather | Real-time weather via Open-Meteo API (free, no key needed) |
| 🔍 Wikipedia Search | Quick factual lookups for study and general knowledge |
| 📅 Study Planner | Daily plan based on my actual VTU Sem 4 subjects |
| 🎓 CGPA Calculator | VTU 10-point CGPA calculator + target grade planner |
| 💻 DSA Suggester | Daily DSA topic + problem for coding practice |

---

## 🚀 How to Run

### 1. Open in Google Colab
Upload `Team_Titanic_Digital_Twin.ipynb` to [Google Colab](https://colab.research.google.com)

### 2. Add API Keys
Go to 🔑 **Secrets** (left sidebar in Colab) and add:

| Secret Name | Where to Get |
|---|---|
| `GROQ_API_KEY` | [console.groq.com/keys](https://console.groq.com/keys) |
| `GEMINI_API_KEY` | [aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey) |

### 3. Run All Cells
`Runtime → Run All` — the Gradio UI launches automatically at the last cell.

---

## 💬 Demo Prompts

Try these in the chat:

```
"Roast me as my digital twin would 😂"
"If I were Batman, how would I approach my DBMS exam?"
"I have 8.4 CGPA after 21 subjects, I want 9.0 — is it even possible?"
"What should I study today and in what order?"
"Give me the hardest DSA problem for today."
"Calculate: sin(pi/4) * factorial(6) + log10(1000)"
"What is the weather in Bangalore right now?"
"Explain dynamic programming like I'm 10 years old."
```

---

## 📁 Project Structure

```
Digital-Twin-AI-Agent/
│
├── Team_Titanic_Digital_Twin.ipynb   # Main notebook — run this
└── README.md
```

---

## 👤 About Me

**C Tejesh** — 2nd year B.E. CSE student at RVITM Bengaluru (VTU), CGPA 8.4

- 🐍 Python | AI/ML | NLP
- 🔗 [LinkedIn](https://linkedin.com/in/tejesh-c)
- 🐙 [GitHub](https://github.com/Mr-C-Tejesh)

---

## 👥 Team Titanic

| Role | Member |
|---|---|
| Captain & Developer | C Tejesh |
| Member | Bhuvan |
| Member | Darshan BR |
| Member | Vinay |

---

*Built with ❤️ at RVITM Bengaluru*
