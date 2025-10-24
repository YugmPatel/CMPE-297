# 🧠 From Prototypes to Agents with ADK

**Author:** Abirami Sukumaran
**Based on:** [Google Codelab – From Prototypes to Agents with ADK](https://codelabs.developers.google.com/your-first-agent-with-adk#0)
**Walkthrough Video:** [Watch on YouTube 🎥](https://youtu.be/ZUDjU5IL0UI)

---

## 📘 Overview

This project demonstrates how to move from a **Gemini prototype prompt** in Google AI Studio to a fully functional **AI Agent** built using Google’s **Agent Development Kit (ADK)**.

The agent automatically generates a **Kitchen Renovation Proposal Document**, formats it into a professional PDF, and uploads it to a **Google Cloud Storage Bucket** — showcasing how you can transform an idea into an autonomous agent application.

---

## 🧩 What You’ll Learn

* Create and configure your first **AI Agent** using ADK.
* Connect your agent to **Gemini 2.5 Flash** through Google AI Studio.
* Generate and store documents in **Google Cloud Storage**.
* Test and visualize your agent in both **Cloud Shell Terminal** and **ADK Web UI**.

---

## ⚙️ Requirements

* A Google Cloud project with **billing enabled**
* Access to **Google Cloud Console** and **Cloud Shell**
* Python **3.9+**
* A **Google AI Studio API key** or **Vertex AI credentials**
* Browser: Chrome or Firefox

---

## 🪜 Step-by-Step Setup

### **1. Create and Configure Your Google Cloud Project**

Set up or select a Google Cloud project, ensure billing is active, and authenticate in Cloud Shell.
This prepares your environment for ADK development.

---

### **2. Prototype in Google AI Studio**

Use **Gemini 2.5 Pro** in Google AI Studio to design a detailed renovation plan prompt.
Experiment with the “Thinking” model for long, structured outputs and try **Gemini 2.0 Flash Image Generation** to visualize design concepts.

This prototype becomes the foundation for your ADK agent.

---

### **3. Set Up ADK**

In Cloud Shell, create a virtual environment and install the **Agent Development Kit (ADK)**.
This enables you to build modular, autonomous agents directly within your Google Cloud workspace.

---

### **4. Build the Renovation Agent**

Within your project workspace, structure your files and define the **root agent**, which:

* Accepts user renovation requests.
* Uses Gemini to generate structured proposal content.
* Calls a tool to format and store the proposal as a PDF in **Google Cloud Storage**.

---

### **5. Configure Google Cloud Storage**

Create a storage bucket (e.g., `next-demo-store`) to store proposal PDFs.
Grant the **Storage Object User** role to `allUsers` for demonstration purposes (or restrict access in production).

---

### **6. Connect Everything with Environment Variables**

Store your configuration in a `.env` file, including:

* Google AI Studio API key or Vertex credentials
* Project ID and region
* Cloud Storage bucket name

This ensures your agent has secure access to all required services.

---

### **7. Run and Test Your Agent**

Execute your agent in Cloud Shell (`adk run .`) or through the ADK Web UI (`adk web`).
Use natural prompts like:

> “Generate a kitchen renovation proposal document in a professional format.”

The agent generates a polished PDF and uploads it to your Google Cloud Storage bucket.

---

### **8. Validate the Output**

Open your Cloud Storage bucket and confirm the newly created **Renovation Proposal PDF**.
You can preview or download it directly via its public URL.

---

### **9. Clean Up**

After testing, delete your project or bucket to avoid future billing charges.

---

## 🧠 Key Concepts

* **Agents:** Autonomous programs capable of reasoning and executing goal-based tasks.
* **ADK (Agent Development Kit):** Framework for creating modular, scalable, and multi-agent systems.
* **LLMs (Large Language Models):** Gemini 2.5 Flash powers understanding and text generation.
* **Tools:** Extend agent functionality, e.g., generating PDFs or accessing APIs.
* **Root Agent:** Central orchestrator that routes user requests to appropriate tools.
* **Cloud Storage:** Persists the generated documents.
* **Environment File (.env):** Stores API keys and configuration securely.

---

## 🎥 Video Walkthrough

A complete step-by-step demonstration is available on YouTube.
It covers everything from project setup to viewing the generated PDF in Cloud Storage.

👉 **Watch the full tutorial here:** [https://youtu.be/ZUDjU5IL0UI](https://youtu.be/ZUDjU5IL0UI)

---

## 🧰 Technologies Used

* **Google AI Studio (Gemini 2.5 Pro)**
* **Google Agent Development Kit (ADK)**
* **Google Cloud Storage**
* **Vertex AI / Generative Language API**
* **Python 3.9+**

---

## 🏁 Outcome

By completing this codelab, you’ll learn how to:

* Turn a simple AI Studio prototype into a working agent.
* Automate document creation and cloud storage using ADK.
* Build the foundation for more complex, multi-agent applications.

---

## 📄 License

This project is provided for **educational and demonstration purposes only**, following Google’s Agent Development Kit (ADK) guidelines.
