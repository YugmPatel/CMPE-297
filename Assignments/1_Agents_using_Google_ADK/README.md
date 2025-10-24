# 🧠 Agents using Google ADK

## 📘 Overview

This project focuses on developing and deploying **AI agents using Google’s Agent Development Kit (ADK)**.
The assignment consists of two main parts:

1. **Implementing Google ADK Codelabs**
2. **Developing a Full Agent Application from the Hackathon Repository**

Each part includes:

* A **README file** documenting the implementation
* The **working agent code** (hosted on GitHub or Colab)
* A **YouTube video walkthrough** demonstrating setup, code execution, and final outputs

---

## 🧩 Part A — Codelabs Implementation

### 1️⃣ From Prototypes to Agents with ADK

**Codelab:** [Google ADK Codelab – From Prototypes to Agents](https://share.google/SedY3WmkMRCEkJrrA)

**Summary:**
Introduced the fundamentals of Google’s Agent Development Kit (ADK) — creating a simple conversational agent, defining its prompts, and running it locally using the ADK Web UI.
The project demonstrated how an LLM-based agent can respond intelligently to user inputs through ADK’s orchestration layer.

**Deliverables:**

* README documentation
* Local ADK agent code and environment files
* YouTube walkthrough showing creation and testing of the prototype agent

---

### 2️⃣ Building AI Agents with ADK: Empowering with Tools

**Codelab:** [Google ADK Codelab – Empowering with Tools](https://share.google/2PaSC2sdeHuNqENjq)

**Summary:**
Extended the agent functionality by integrating **external tools** using ADK.
Implemented an agent capable of performing structured tasks like retrieving data, processing user queries, and performing simple computations through ADK’s tool integration framework.

**Deliverables:**

* README with explanation of ADK tool integration
* Executable ADK agent code and setup instructions
* YouTube video walkthrough demonstrating the agent executing tasks using custom tools

---

### 3️⃣ Build a Travel Agent using MCP Toolbox and ADK

**Codelab:** [Google ADK + MCP Toolbox Codelab](https://share.google/aTibSpbyEDvVPhIqD)

**Summary:**
Developed a **Travel Agent** that integrates **Google Cloud SQL** with the **MCP Toolbox for Databases** through ADK.
The agent responds to user queries about hotel availability, locations, and price tiers using structured SQL queries executed via the MCP Toolbox.
It demonstrates a real-world use case of ADK agents working with cloud databases to answer user questions dynamically.

**Deliverables:**

* README documentation describing cloud setup, database configuration, and ADK integration
* Functional code archive or Colab workspace
* YouTube video showing database provisioning, MCP configuration, and live query responses from the agent

---

## 🤖 Part B — Hackathon Agent Implementation

### Academic Research Assistant (from [awesome-adk-agents](https://github.com/Sri-Krishna-V/awesome-adk-agents))

**Summary:**
Developed an **AI-powered Academic Research Assistant** capable of analyzing researcher profiles, extracting keywords, finding relevant academic papers, and generating comparative research reports.
Built using **Google ADK** and **Vertex AI (Gemini 2.0 Flash)**, the agent automates the early stages of academic literature review.

**Key Capabilities:**

* Extracts research areas and keywords from user profiles
* Searches and summarizes relevant publications
* Performs multi-step reasoning via analysis–critique loops
* Generates a professional markdown report with insights and gaps

**System Workflow:**

1. **Profiler Agent** → Extracts research keywords
2. **Searcher Agent** → Finds relevant papers
3. **Comparison Root Agent** → Analyzes and refines output
4. **Formatter Agent** → Produces final structured report

**Deliverables:**

* Detailed README documentation
* Source code archived on GitHub
* YouTube video demonstrating full code walkthrough, execution, and final report generation
  
---

## 💡 Learning Outcomes

Through these implementations, the following concepts were demonstrated:

* Understanding of **multi-agent architecture** in ADK
* Integration of **external tools** like MCP and databases
* Use of **Gemini models on Vertex AI** for intelligent task execution
* Application of **prompt engineering** and **workflow orchestration**
* Hands-on deployment and testing of agents in **Google Cloud Shell and Cloud Run**

---

## 🌐 Submission Components

* ✅ GitHub repository containing all agent folders and documentation
* ✅ Four YouTube videos (one per implemented agent)
* ✅ Each project accompanied by an independent README file
* ✅ Fully functional ADK Web Interface demonstration

---

## 🏁 Conclusion

This project showcases how **Google’s Agent Development Kit (ADK)** can transform prototype conversational models into fully capable, tool-empowered AI agents.
The implementations bridge the gap between **research concepts and real-world AI workflows**, using modular, composable agents that can reason, interact, and act — powered by **Vertex AI**.

Would you like me to format this README for your GitHub (with emojis, section dividers, and clean typography like a professional submission page)?
