# Always-On AI Agent

## Project Overview

The **Always-On AI Agent** is an autonomous AI-powered system developed using Python, LangChain, LangGraph, and Ollama. It demonstrates the practical implementation of Agentic AI concepts, including intelligent task planning, long-term memory management, human-in-the-loop approval, tool execution, workflow orchestration, and scheduled automation.

The agent uses the Llama 3.2 model to generate structured action plans, retrieve stored user preferences, and execute approved tasks through custom Python tools. SQLite provides persistent memory, while LangGraph manages the agent's workflow and execution process.

## Key Features

- **AI-Powered Planning:** Generates structured, step-by-step execution plans using the Llama 3.2 language model.
- **Long-Term Memory:** Stores and retrieves user preferences and contextual information using SQLite.
- **Human-in-the-Loop Approval:** Requests user confirmation before executing planned actions, ensuring controlled task execution.
- **Custom Tool Integration:** Uses Python-based tools to perform tasks such as saving task details and creating notes.
- **Workflow Orchestration:** Implements LangGraph to manage agent states, decision-making, and execution workflows.
- **Scheduled Automation:** Uses APScheduler to automatically trigger the agent every Monday at 9:00 AM IST.
- **Error Handling:** Implements Python's try-except mechanism to manage runtime errors and improve system reliability.

## Technology Stack

- **Programming Language:** Python 3.12
- **AI Frameworks:** LangChain, LangGraph
- **LLM Integration:** Ollama, Llama 3.2
- **Database:** SQLite
- **Task Scheduling:** APScheduler
- **Core Concepts:** Agentic AI, AI Planning, Long-Term Memory, Human-in-the-Loop, Tool Calling, Workflow Automation

## Project Structure

```text
always-on-ai-agent/
│
├── agent.py
├── memory.py
├── tools.py
├── scheduler.py
├── agent_memory.db
├── agent_notes/
└── README.md
```

## Installation and Setup

**1. Clone the Repository**

```bash
git clone <repository-url>
cd always-on-ai-agent
```

**2. Create a Virtual Environment**

```bash
python -m venv venv
```

Activate the environment:

Windows:
```bash
venv\Scripts\activate
```

Linux / macOS:
```bash
source venv/bin/activate
```

**3. Install Dependencies**

```bash
pip install langchain langgraph langchain-ollama apscheduler
```

**4. Install and Configure Ollama**

Install Ollama and ensure that the Ollama service is running.

Download the Llama 3.2 model:

```bash
ollama pull llama3.2
```

## Running the Application

**Start the AI Agent**

```bash
python agent.py
```

**Start the Automated Scheduler**

```bash
python scheduler.py
```

The scheduler is configured to execute the AI agent automatically every Monday at 9:00 AM IST.

## Learning Outcomes

This project provides hands-on experience with modern Agentic AI development and demonstrates how to:

- Build autonomous AI agents using Python.
- Integrate Large Language Models (LLMs) using Ollama.
- Develop intelligent planning and decision-making workflows.
- Implement persistent memory using SQLite.
- Design human-in-the-loop approval mechanisms.
- Integrate custom Python tools into AI agents.
- Orchestrate multi-step workflows using LangGraph.
- Automate recurring tasks using APScheduler.
- Implement error handling for reliable application execution.

## Author

**Rohit Biradar**

Data Scientist | AI/ML & Generative AI Enthusiast
