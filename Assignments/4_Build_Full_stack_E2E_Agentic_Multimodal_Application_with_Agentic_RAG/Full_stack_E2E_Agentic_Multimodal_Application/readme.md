# 🧾 Personal Expense Assistant – Going Multimodal with Gemini 2.5, Firestore & Cloud Run

### 🚀 Overview

The **Personal Expense Assistant** is an end-to-end multimodal web app built using Google’s **Agent Development Kit (ADK)** and **Gemini 2.5**.
It lets users upload receipt images, automatically extracts and stores expense details in **Firestore**, performs both **metadata** and **vector-based contextual searches**, and displays results through an interactive **Gradio chat interface** served by a **FastAPI backend**.
Both services run seamlessly on **Google Cloud Run**.

---

### 📽️ YouTube Walkthrough

🎥 **Full Video Tutorial:** [Watch the complete build and deployment walkthrough on YouTube](https://youtu.be/SRLYwLynx4s)

---

### 🧠 Key Features

* **Multimodal Gemini 2.5 integration** via the Google ADK.
* **Automatic receipt parsing** — extract store name, date, total, and items from images.
* **Firestore Vector Search** for contextual queries (RAG-style retrieval).
* **FastAPI Backend** with session & artifact management.
* **Gradio Frontend** providing chat + image upload interface.
* **Cloud Run Deployment** in one container using supervisord.
* **Environment-based config** via YAML and Pydantic-Settings.
* **ADK Callbacks** to manage conversation context and image placeholders.

---

### ⚙️ Architecture Overview

| Layer             | Technology                       | Purpose                                   |
| :---------------- | :------------------------------- | :---------------------------------------- |
| **LLM Agent**     | Gemini 2.5 Flash (via Vertex AI) | Reasoning, extraction, RAG search         |
| **ADK Framework** | Google ADK v1.18                 | Agent orchestration & tool integration    |
| **Database**      | Firestore (Native Mode)          | Store metadata + vector embeddings        |
| **Storage**       | Cloud Storage (GCS bucket)       | Persist uploaded receipt images           |
| **Backend**       | FastAPI + ADK Runner             | Session handling, tool execution          |
| **Frontend**      | Gradio 5.x                       | Chat UI for text + image interaction      |
| **Deployment**    | Cloud Run + Supervisord          | Serve frontend + backend in one container |

---

### 🧩 What You’ll Learn

* How to build multimodal agents with Gemini 2.5 and the ADK.
* How to integrate Firestore as a **vector database**.
* How to develop a simple full-stack prototype with FastAPI + Gradio.
* How to deploy agentic apps to Cloud Run with environment variables.
* How to debug ADK agents locally using the development UI.

---

### 🧰 Technologies Used

* **Python 3.12 + uv**
* **Google ADK v1.18**
* **Gemini 2.5 Flash (through Vertex AI)**
* **Firestore (Native Mode)**
* **Google Cloud Storage**
* **Gradio 5.x**
* **FastAPI + Uvicorn**
* **Docker + Supervisord**
* **Cloud Run**

---

### 🧾 Project Flow Summary

1. **Setup Cloud Project** – enable APIs & create Firestore + Storage bucket.
2. **Prepare Environment** – clone repo, configure `settings.yaml`.
3. **Build Agent** – use ADK CLI to scaffold, then add tools, callbacks, prompt.
4. **Test Locally** – run `adk web` UI, interact, and store sample receipts.
5. **Add Frontend & Backend** – Gradio chat interface + FastAPI server.
6. **Integrate & Debug** – confirm storage, queries, and vector retrieval.
7. **Deploy to Cloud Run** – one-click deployment using `gcloud run deploy`.
8. **Demo** – upload receipts, ask for summaries, totals, and images.

---

### 🔍 Sample Interactions

* “Store this receipt.” *(after uploading a photo)*
* “Show all expenses from January 2024.”
* “Find my coffee receipts.”
* “Give me the image for the Yakiniku Like receipt.”
* “What’s my total spending between 2023–2024?”
---

### 💡 Possible Extensions

* Add spending categories or budget limits.
* Integrate Google Sheets export.
* Add speech input or mobile view with Gradio Blocks.
* Visualize monthly spending with Plotly charts.

---

### 🙌 Acknowledgements

* Google Cloud Codelab: *Going Multimodal with Agent Development Kit*
* Alvin Prayuda Juniarta Dwiyantoro (original lab author)
* Gemini 2.5 team & ADK contributors
