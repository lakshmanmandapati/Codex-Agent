# Codex Agent

**Codex Agent** is an AI-powered coding assistant built with [LangGraph](https://github.com/langchain-ai/langgraph).
It works like your personal multi-agent development team — you describe what you want in natural language, and it generates a complete working project file by file.

It follows a structured developer workflow: planning, designing, and implementing your project.

---

## Architecture

Codex Agent is powered by three specialized agents:

* **Planner Agent** – Understands your request and creates a high-level project plan.
* **Architect Agent** – Breaks the plan into engineering tasks with clear context for each file.
* **Coder Agent** – Implements the tasks, writes code into files, and ensures the project runs.

---

## Getting Started

### Prerequisites

* [uv](https://docs.astral.sh/uv/getting-started/installation/) installed for managing Python environments.
* A [Groq](https://console.groq.com/keys) account with a valid API key.

---

### Installation & Setup

1. **Create a virtual environment**

   ```bash
   uv venv
   source .venv/bin/activate
   ```

2. **Install dependencies**

   ```bash
   uv pip install -r pyproject.toml
   ```

3. **Configure environment variables**

   * Copy `.sample_env` to `.env`
   * Add your Groq API key and any other required values

4. **Run the application**

   ```bash
   python main.py
   ```

If everything is set up correctly, you can start giving Codex Agent natural language prompts.

---

## Example Prompts

You can ask Codex Agent to build complete projects. Some examples:

* Create a to-do list application using HTML, CSS, and JavaScript.
* Build a simple calculator web application.
* Develop a blog API in FastAPI with a SQLite database.
* Generate a REST API for managing student records with CRUD functionality.

---

