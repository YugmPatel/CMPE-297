# 🧳 Build a Travel Agent using MCP Toolbox for Databases and Agent Development Kit (ADK)

### 📘 Overview

This project demonstrates how to build an **AI-powered Travel Agent** capable of answering user queries about hotels using **Google’s Agent Development Kit (ADK)** and the **MCP Toolbox for Databases**.
It connects a **PostgreSQL Cloud SQL database** to an **AI Agent**, allowing natural-language hotel searches by city or hotel name.

The implementation follows Google’s official codelab:
**[Build a Travel Agent using MCP Toolbox for Databases and ADK](https://codelabs.developers.google.com/travel-agent-mcp-toolbox-adk#0)**

---

## 🎯 Objectives

By completing this project, you’ll learn how to:

* Provision and populate a **Cloud SQL for PostgreSQL** instance with hotel data.
* Set up the **MCP Toolbox for Databases** to securely expose SQL queries as reusable tools.
* Build and configure an **AI Agent using the Agent Development Kit (ADK)**.
* Connect the MCP Toolbox tools with your ADK agent.
* Test the entire setup locally using **ADK CLI** and **MCP Toolbox UI**.
* (Optional) Deploy the agent and toolbox to **Google Cloud Run** for production use.

---

## 🧠 How It Works

The Travel Agent follows this workflow:

1. **Database Layer**
   A Cloud SQL (PostgreSQL) database stores hotel information such as name, location, price tier, and availability.

2. **MCP Toolbox Layer**
   The MCP Toolbox acts as a bridge between the database and the AI agent.
   It defines tools such as “Search hotels by name” and “Search hotels by location” that the agent can call via API.

3. **Agent Layer (ADK)**
   Using the Agent Development Kit, an AI agent (powered by the Gemini model) is configured to utilize the MCP Toolbox tools.
   When users ask hotel-related questions, the agent dynamically selects and executes the appropriate tool to retrieve real data.

4. **Testing & Interaction**
   The project can be tested through:

   * **ADK Web UI** – a local browser interface for interacting with the agent.
   * **MCP Toolbox UI** – a web dashboard to test and monitor your database tools.
   * **Command Line** – via `adk run` or `gemini` CLI.

---

## 🧩 Tech Stack

| Component                         | Description                                           |
| --------------------------------- | ----------------------------------------------------- |
| **Google Cloud SQL (PostgreSQL)** | Managed relational database for hotel data            |
| **MCP Toolbox for Databases**     | Middleware to manage and expose SQL tools securely    |
| **Agent Development Kit (ADK)**   | Framework for building and deploying AI agents        |
| **Gemini (Vertex AI)**            | Underlying LLM model used by the agent                |
| **Python (ADK environment)**      | Primary language for building the agent               |
| **Cloud Shell / Cloud Run**       | Cloud environments for setup, testing, and deployment |

---

## 🧪 Testing Options

* **Local Testing**

  * Run the MCP Toolbox server locally and connect the agent through ADK CLI.
  * Access the Toolbox UI at `http://localhost:5000/ui` for visual testing.
  * Use `adk web` or `adk run` to interact with the agent directly.

* **Cloud Deployment (Optional)**

  * Deploy both the MCP Toolbox server and the ADK agent to **Google Cloud Run** for scalable, managed access.

---

## 🎥 YouTube Walkthrough

A complete **video walkthrough** is available on YouTube, covering every step from setup to testing.
Watch it here:
👉 [**Travel Agent with MCP Toolbox & ADK — Full Tutorial**](https://youtu.be/WPpXRu8HXrA)

---

## 📚 Credits

* **Authors of Original Codelab:** Romin Irani & Jack Wotherspoon
* **Codelab Source:** [Google Developers — Build a Travel Agent using MCP Toolbox for Databases and ADK](https://codelabs.developers.google.com/travel-agent-mcp-toolbox-adk#0)

---

## 🏁 Outcome

By the end of this project, you’ll have:

* A fully functional **AI Travel Agent** integrated with real hotel data.
* Hands-on experience with **ADK**, **MCP Toolbox**, and **Gemini**.
* A reusable setup you can extend for other datasets like flights, restaurants, or travel packages.
