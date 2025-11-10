# 🤖 Full Stack E2E Agentic Multimodal Application with Agentic RAG

This repository contains the complete implementation of a **Full Stack End-to-End (E2E) Agentic Multimodal Application** built using the **Google Agent Development Kit (ADK)** with integrated **Retrieval-Augmented Generation (RAG)** capabilities.
The project demonstrates a real-world **multimodal agent** that interacts with users through text and images, performs reasoning with RAG pipelines, and uses a **fully connected backend and database** to persist and retrieve contextual information.

---

## 🧠 Project Overview

This project is inspired by Google Cloud’s **Personal Expense Assistant** multimodal agent example.
It showcases how to build, integrate, and deploy an intelligent multimodal assistant that can understand both **text and visual inputs**, process contextual data using **Agentic RAG**, and provide meaningful, personalized responses through a modern **frontend–backend architecture**.

The application includes:

* A **React/Streamlit-based frontend** for multimodal interaction (text + images).
* A **Python-based backend** using ADK pipelines and APIs.
* **RAG integration** for contextual memory and retrieval.
* A **database layer** (AlloyDB / PostgreSQL / Firestore) for persistent storage.
* A **video walkthrough** demonstrating the full setup, code explanation, and execution.

---

## 🧩 Key Components

| Component                    | Description                                                                                                         |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| **Frontend (UI Layer)**      | Interactive multimodal interface allowing users to upload images, input text, and visualize outputs from the agent. |
| **Backend (Agentic Logic)**  | Built using Google ADK, handling request routing, multimodal reasoning, and tool orchestration.                     |
| **RAG Pipeline**             | Enables knowledge retrieval and contextual response generation by combining vector search and Gemini reasoning.     |
| **Database Integration**     | Stores user profiles, expense records, context data, and retrieval documents for RAG.                               |
| **Gemini Model Integration** | Uses Gemini 2.5 for multimodal understanding and inference (text + vision).                                         |
| **Deployment**               | Cloud-based deployment using Cloud Run or a local container setup for demonstration.                                |

---

## 📚 Reference Material

* **Codelab:** [Personal Expense Assistant with Multimodal ADK](https://codelabs.developers.google.com/personal-expense-assistant-multimodal-adk?hl=en)
* **Google Cloud Blog:**

  * [Going Multimodal with ADK (Part 1)](https://medium.com/google-cloud/going-multimodal-with-agent-development-kit-personal-expense-assistant-with-gemini-2-5-17626aaee9a2)
  * [Going Multimodal with ADK (Part 2)](https://medium.com/google-cloud/going-multimodal-with-agent-development-kit-personal-expense-assistant-with-gemini-2-5-480b031c7d5a)

---

## 🧱 Repository Structure

The repository is organized into modular sections for clarity and scalability.

**Top-level structure:**

* frontend/ — React or Streamlit-based multimodal UI
* backend/ — ADK agent logic, API services, and RAG integration
* database/ — schema definitions and setup scripts
* assets/ — screenshots, diagrams, and sample input data
* video_walkthrough/ — complete video demonstrating code and execution
* README.md — documentation (this file)

Each folder includes its own README file explaining configurations, dependencies, and execution steps.

---

## ⚙️ Features Implemented

* End-to-end **full stack architecture** using ADK and Gemini 2.5
* **Multimodal support** for text and image inputs
* **Retrieval-Augmented Generation (RAG)** with database and vector store
* Persistent **context memory** for personalized responses
* Seamless **frontend–backend communication** through REST APIs
* Cloud and local **deployment-ready setup**
* Comprehensive **video walkthrough** of code and app execution

---

## 🧠 Functional Workflow

1. **User Interaction:** The user inputs queries or uploads receipts/images via the frontend.
2. **Backend Processing:** The backend routes input to the ADK-based agent pipeline.
3. **Multimodal Understanding:** The Gemini model processes text and image inputs.
4. **RAG Retrieval:** Relevant context is retrieved from the database/vector store.
5. **Response Generation:** The agent produces a contextually aware, multimodal output.
6. **Frontend Display:** The response and analytics are rendered back to the user.

---

## 🎥 Video Demonstration

The **video walkthrough** includes:

* Detailed explanation of folder structure and architecture
* Code walkthrough of frontend, backend, and RAG pipeline
* Database connection setup and testing
* Real-time execution demo of the working multimodal agent
* End-to-end demonstration showing how data flows from user to agent and back

All videos are available in the **video_walkthrough/** directory and uploaded to YouTube for reference.

