# Building AI Agents with Google ADK — Foundation + Tools

Create your own **AI Personal Assistant** using Google’s **Agent Development Kit (ADK)** — and then empower it with real-time tools, Google Search, and LangChain integrations.

This project follows Google’s official codelab series:

1. **Building AI Agents with ADK: The Foundation**
2. **Building AI Agents with ADK: Empowering with Tools**

---

## ✨ Overview

This project demonstrates how to build, configure, and enhance an AI agent capable of:

* Conversational reasoning with **Gemini 2.5 Flash**
* Fetching **real-time currency exchange rates**
* Getting **live weather and event data** via Google Search
* Retrieving **cultural and historical knowledge** from Wikipedia
* Operating in a **multi-agent architecture** for modular task delegation

---

## 📹 YouTube Walkthrough

🎥 **Watch the full video tutorial here:**
*([https://youtu.be/W3IfrEmkvQI](https://youtu.be/W3IfrEmkvQI))*

In the video, I’ll walk you through:

* Setting up the ADK environment on Google Cloud
* Creating your first conversational agent
* Adding custom, built-in, and third-party tools
* Running and testing your agent in the ADK Web UI
* Understanding how multi-agent systems work

Make sure to like 👍 and subscribe 🔔 for more AI & developer tutorials!

---

## 🧠 Part 1 — The Foundation

In the first part, you’ll learn how to:

* Set up a **Google Cloud project** with Vertex AI enabled
* Use **Cloud Shell** and **Python 3.12** for your environment
* Install **Google ADK** and create your first agent
* Understand the structure and purpose of generated files
* Run your agent in the **terminal** or the **ADK Web UI**

By the end of Part 1, you’ll have a working personal assistant agent ready for customization.

---

## ⚙️ Part 2 — Empowering with Tools

In the second part, you’ll transform your agent from basic to powerful using ADK’s modular tool system.

### Custom Function Tool

Adds a function that retrieves **real-time currency exchange rates** using an external API.

### Built-in Google Search Tool

Integrates ADK’s built-in **Google Search** capability for **weather forecasts, news, and live updates**.

### Multi-Agent Pattern

Introduces a **specialized search agent** that handles real-time queries, while the root agent routes user requests intelligently.

### LangChain Wikipedia Integration

Connects the agent with **LangChain’s Wikipedia Tool** to fetch **historical and cultural** context about locations, people, and concepts.

---

## 🧩 Architecture Overview

This project uses a **multi-agent modular architecture**:

* **Root Agent (Orchestrator):** Routes user queries and chooses the correct tool.
* **Custom Function Tool:** Handles currency-related queries.
* **Search Agent (Sub-Agent):** Fetches real-time data using Google Search.
* **LangChain Wikipedia Tool:** Provides deeper historical and cultural context.

This decentralized structure makes it easy to extend your agent with new capabilities in the future.

---

## 🧱 Project Structure

The folder structure follows a clean, modular pattern:

```
ai-agents-adk/
└── personal_assistant/
    ├── .env
    ├── __init__.py
    ├── agent.py
    ├── custom_functions.py
    ├── custom_agents.py
    └── third_party_tools.py
```

Each file serves a distinct purpose:

* **agent.py:** Defines your main AI agent
* **custom_functions.py:** Contains user-defined tools
* **custom_agents.py:** Houses sub-agents for modular behavior
* **third_party_tools.py:** Integrates external AI frameworks like LangChain
* **.env:** Stores Google Cloud project configurations

---

## 🧰 Tools & Technologies Used

* **Google ADK (Agent Development Kit)**
* **Gemini 2.5 Flash (Vertex AI Model)**
* **Google Cloud Console / Shell**
* **Python 3.12**
* **uv (Python environment manager)**
* **LangChain & Wikipedia API**

---

## ▶️ Running the Agent

Once your environment and tools are configured, launch the agent in **Development Web UI** mode.

This gives you:

* A clean chat interface
* Proper Markdown rendering
* Live event inspection (see which tool the agent used)
* Easy debugging and monitoring of responses

You can test prompts like:

* “What’s the exchange rate from Singapore dollars to Japanese yen?”
* “What’s the weather forecast in Tokyo next month?”
* “Tell me about the history of Kyoto.”

---

## 🛡️ Troubleshooting Guide

**1. Billing or API Access Error**

* Make sure your Google Cloud billing account is active.
* Confirm that Vertex AI API is enabled in your project.

**2. Project Configuration Issues**

* Check that `.env` contains your correct Project ID and Region.
* Ensure Cloud Shell or terminal is set to the same project.

**3. Environment Activation**

* If running locally, activate your virtual environment before executing commands.

**4. Restart Required**

* After modifying files, stop the agent (Ctrl + C) and restart it to apply changes.

---

## 📊 Expected Output

When everything is working correctly:

* Your agent responds conversationally
* It provides accurate, real-time exchange rates
* It can answer current event and weather questions
* It retrieves reliable cultural or historical data from Wikipedia

---

## 📜 License

Released under the **MIT License**.
You are free to use, modify, and share this project for educational or personal use.

---

## 🙌 Acknowledgments

* **Google Developers Codelabs:** Building AI Agents with ADK
* **LangChain Community:** Open-source AI tools
* **Google Cloud Team:** Vertex AI and ADK integrations
