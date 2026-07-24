# 🧠 Kenny AI

A personal local AI assistant built with Python, Ollama and MCP architecture.

---

## ✨ About

Kenny is a modular local AI assistant designed to become a complete personal operating system powered by artificial intelligence.

Unlike ordinary chatbots, Kenny is built around a Brain, Memory, AI Router, and an MCP (Model Context Protocol) architecture that allows the assistant to use tools, remember information, and make decisions.

Everything runs locally through Ollama.

---

## 🚀 Current Features

### 🧠 Brain
* AI decision system
* AI Router
* Intent Engine (fallback)
* Task Manager

### 💾 Memory
* Conversation history
* Long-term memory
* User profile
* Goals
* Diary
* State storage

### 👤 User Profile
* Name
* Age
* Interests
* Preferences
* Memory-based responses

### 🖥 System MCP
* CPU usage
* RAM usage
* Disk information
* Date & Time
* Windows information
* Local IP
* Hostname
* Battery status
* Running processes

### 📁 Files MCP
* List files
* Search files
* Read files
* Create files
* Write files
* Append files
* Rename files
* Copy files
* Move files
* Delete files
* File size

### 🌍 Internet MCP
* Internet status
* Page loading
* Provider architecture
* Tavily support (optional)

---

## 📂 Project Structure

```text
KENNY/
│
├── main.py                 # Точка входа
├── kenny.py                # Основной класс Kenny
├── brain.py                # Логика принятия решений
├── llm.py                  # Работа с Ollama/Qwen
├── config.py               # Настройки
├── task_manager.py         # Выполнение инструментов
├── intent_engine.py        # Резервный Intent Engine
├── tool_registry.py        # Реестр инструментов
├── register_tools.py       # Регистрация всех MCP
│
├── core/
│   ├── ai_router.py        # AI Router
│   ├── planner.py          # Планировщик (заготовка)
│   ├── executor.py         # Исполнитель планов
│   ├── profile_manager.py  # Сохранение информации о пользователе
│   └── profile_reader.py   # Ответы по профилю
│
├── memory/
│   ├── memory.py
│   ├── diary.py
│   ├── profile.py
│   ├── goals.py
│   └── state.py
│
├── mcp/
│   ├── mcp_client.py
│   ├── router.py
│   │
│   ├── files/
│   │   └── files.py
│   │
│   ├── system/
│   │   └── system.py
│   │
│   ├── internet/
│   │   ├── internet.py
│   │   └── providers.py
│   │
│   ├── server/
│   │   └── server.py
│   │
│   └── robots/
│       └── robots.py
│
├── personality/
│   ├── personality.py
│   ├── emotions.py
│   └── thoughts.py
│
├── data/
│   ├── memory.json
│   ├── diary.json
│   ├── profile.json
│   ├── goals.json
│   ├── personality.json
│   └── state.json
│
├── logs/
│   └── kenny.log
│
├── README.md
├── LICENSE
├── requirements.txt
└── .gitignore
```

🏗 Architecture
```text
User
 │
 ▼
Brain
 │
 ├───────────────┐
 │               │
 ▼               ▼
AI Router      Profile
 │
 ▼
Task Manager
 │
 ▼
MCP Router
 │
 ├──────── Files
 ├──────── System
 ├──────── Internet
 ├──────── Robots
 └──────── Server
```

🛠 Technologies
Python

Ollama

Qwen

JSON

psutil

requests

📈 Roadmap
✅ v2 
Brain

AI Router

Memory

Profile

Files MCP

System MCP

Internet MCP (base)

Tool Registry

🔜 Next Version
Better AI Router

Planner

Executor

Voice

Vision

Smart Memory

Scheduler

Plugin System

🎯 Goal
The long-term goal is to build a fully autonomous local AI assistant capable of reasoning, planning, remembering, using tools, and interacting naturally with the user.

📜 License
MIT License. Made with ❤️ using Python & Ollama.
