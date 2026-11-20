# multi-agent-ai-software-development
AI-powered multi-agent system for automated software development using LangGraph, LangChain, Python and FastAPI.
# 🤖 Multi-Agent AI System for Automated Software Development

An AI-powered web application that automates software development tasks using specialized AI agents. The system understands software requirements, generates a structured development plan, and produces Python code through coordinated AI workflows.

---

## 📌 Project Overview

The **Multi-Agent AI System for Automated Software Development** is an AI-based web application designed to simplify the software development process using multiple specialized AI agents.

The system uses a **Planner Agent** to understand user requirements and break them down into smaller, structured tasks. A **Coder Agent** then generates Python code based on the plan provided by the Planner Agent.

The agents are coordinated using **LangGraph**, while the backend is developed using FastAPI and the frontend provides a user-friendly interface for interacting with the system.

The main objective is to demonstrate how multiple AI agents can collaborate to automate important stages of software development.

## 🎯 Project Objectives

- Develop a user-friendly web application for automated software development.
- Understand software requirements using an AI-powered Planner Agent.
- Break complex development requirements into smaller, structured tasks.
- Generate Python code using a specialized Coder Agent.
- Coordinate multiple AI agents using LangGraph.
- Display generated plans and code through a web interface.
- Provide basic task history management using SQLite.

## ✨ Key Features

- **AI-Based Requirement Analysis:** Understands software development requirements.
- **Automated Task Planning:** Converts user requirements into structured development tasks.
- **AI Code Generation:** Generates Python code based on the development plan.
- **Multi-Agent Architecture:** Uses specialized agents for different responsibilities.
- **Workflow Orchestration:** Coordinates agents using LangGraph.
- **Web-Based Interface:** Allows users to submit requirements and view results.
- **Task History:** Optional storage of generated task history using SQLite.

## 🏗️ System Architecture

The system follows a multi-agent architecture in which the frontend communicates with the FastAPI backend, which invokes the AI workflow.

### Workflow

1. User enters a software development requirement.
2. Frontend sends the request to the FastAPI backend.
3. Backend validates the input.
4. Planner Agent analyzes the requirement.
5. Planner Agent generates a structured development plan.
6. Coder Agent receives the plan and generates Python code.
7. LangGraph manages the workflow and shared state between agents.
8. Backend returns the generated plan and code.
9. Frontend displays the final output to the user.
10. Task history can optionally be stored in SQLite.

## 🧩 Functional Modules

| Module | Description |
|---|---|
| M1 – Website UI & Frontend | User-friendly interface with requirement input, Generate button, loading indicator, and output section. |
| M2 – Backend & API | FastAPI backend for request handling, input validation, and AI workflow execution. |
| M3 – Planner Agent | Uses an LLM to understand requirements and divide them into smaller tasks. |
| M4 – Coder Agent | Generates Python code based on the Planner Agent's output. |
| M5 – Workflow Integration & Output | Connects agents using LangGraph, manages shared workflow state, and displays final results. |

## 🛠️ Technology Stack

### Programming Language
- Python

### AI & Agent Frameworks
- LangChain
- LangGraph
- Large Language Models (LLMs)

### Backend
- FastAPI

### Frontend
- Web Technologies (HTML, CSS, JavaScript)

### Database
- SQLite

### Development & Deployment Tools
- Docker
- Git
- GitHub

## 📂 Project Structure

```text
Multi-Agent-AI-System/
│
├── frontend/
│   ├── index.html
│   ├── style.css
│   └── script.js
│
├── backend/
│   ├── main.py
│   ├── api/
│   └── requirements.txt
│
├── agents/
│   ├── planner_agent.py
│   └── coder_agent.py
│
├── workflow/
│   └── graph.py
│
├── database/
│   └── database.py
│
├── .env.example
├── .gitignore
├── README.md
└── requirements.txt
```

*Note: This is a proposed directory structure. Update it according to the actual implementation.*

## ⚙️ Installation & Setup

### Prerequisites

Make sure you have the following installed:

- Python 3.10 or above
- Git
- Code Editor (VS Code recommended)

### Step 1: Clone the Repository

```bash
git clone https://github.com/avdhutgatkal17-avii/multi-agent-ai-software-development.git
```

### Step 2: Navigate to the Project Directory

```bash
cd Multi-Agent-AI-System
```

### Step 3: Create a Virtual Environment

```bash
python -m venv venv
```

Activate the environment:

**Windows:**
```bash
venv\Scripts\activate
```

**Linux / macOS:**
```bash
source venv/bin/activate
```

### Step 4: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 5: Configure Environment Variables

Create a `.env` file and add the required LLM provider credentials and configuration.

Do not upload API keys or sensitive credentials to GitHub.

### Step 6: Run the Application

Once the backend is implemented, start the FastAPI server:

```bash
uvicorn backend.main:app --reload
```

Open the API documentation at:

```text
http://127.0.0.1:8000/docs
```

*Update the commands according to your actual application entry point.*

## 💻 Expected System Output

The application is expected to:

1. Accept software development requirements from the user.
2. Generate a structured task plan using the Planner Agent.
3. Generate Python code using the Coder Agent.
4. Display the development plan and generated code on the website.

## 🔮 Future Scope

The following advanced capabilities are planned for future development:

- Automated code testing and validation.
- AI-based code review.
- Persistent semantic memory.
- Improved agent collaboration.
- Advanced error detection and debugging.
- Enhanced software development automation.

## 👨‍💻 Project Team

**Institute:** Institute of Management & Career Courses (IMCC), Pune

**Department:** Department of Computer Applications (MCA)

**Academic Year:** 2026–2028

| Name | Responsibility |
|---|---|
| Avdhut Gatkal | Lead Team Leader |
| Soham B. Pujari | Core Team Member |

**Project Guide:** Dr. Mukul Kulkarni

## 📚 Project Category

- MCA Capstone Team Project
- Artificial Intelligence & Machine Learning
- Multi-Agent Systems
- Automated Software Development

---

## 📌 Project Status

Currently under development as an MCA capstone project.

The initial prototype focuses on the frontend, FastAPI backend, Planner Agent, Coder Agent, and LangGraph workflow integration.

---

## 📄 License

This project is developed for academic purposes as part of the MCA Capstone Project at IMCC, Pune.
