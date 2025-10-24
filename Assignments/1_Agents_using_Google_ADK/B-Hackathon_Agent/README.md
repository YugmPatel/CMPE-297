# 🎓 Academic Research Assistant

An **AI-powered academic research assistant** built using **Google’s Agent Development Kit (ADK)** and **Vertex AI (Gemini 2.5 Flash)**.
This system helps researchers accelerate their literature review process by analyzing academic profiles, discovering relevant papers, and generating a comparative research report with thematic and methodological insights.

---

## 🚀 Features

### 🧩 Multi-Agent Architecture

* **Root Agent** – Orchestrates the full workflow.
* **Profiler Agent** – Extracts keywords and research interests from a user’s academic profile.
* **Searcher Agent** – Finds recent and relevant academic papers based on extracted keywords.
* **Comparison Root Agent** – Compares and analyzes the papers in a multi-step refinement loop:

  * Generates initial analysis
  * Critiques and improves it
  * Produces a structured, readable report

### 📄 Report Output Includes

* Annotated bibliography with summaries
* Thematic and methodological analysis
* Identified research gaps and future directions
* Concise concluding insights tailored to the researcher’s focus

---

## 🧠 System Architecture

```
academic_research_assistant/
│
├── agent.py                     # Root orchestrator agent
├── prompts.py                   # Root workflow prompt logic
├── sub_agents/
│   ├── profiler_agent/          # Profile extraction and keyword analysis
│   ├── searcher_agent/          # Paper search and retrieval
│   └── comparison_root_agent/   # Multi-stage paper comparison and formatting
│
├── tools/                       # Utility functions and data access tools
├── shared_libraries/            # Global constants and shared configs
└── .env                         # Environment configuration
```

---

## 🧰 Tech Stack

| Component                              | Description                               |
| -------------------------------------- | ----------------------------------------- |
| **Google ADK (Agent Development Kit)** | Multi-agent orchestration framework       |
| **Gemini 2.5 Flash (Vertex AI)**       | Core reasoning and text generation model  |
| **Python 3.12**                        | Core language for ADK agents              |
| **FastAPI (via ADK)**                  | Provides the interactive web interface    |
| **Cloud Shell / Cloud Run**            | Deployment and runtime environment        |
| **SerpAPI (Optional)**                 | API integration for academic paper search |

---

## 🧾 Prerequisites

* Google Cloud Project (with billing enabled)
* Vertex AI API access
* Python 3.10 or newer
* ADK and its dependencies installed
* Optional: [SerpAPI key](https://serpapi.com) for expanded paper search

---

## ⚙️ Environment Setup

1. **Clone the repository**

   ```bash
   git clone https://github.com/<your-username>/academic-research-assistant.git
   cd academic-research-assistant
   ```

2. **Create and activate a virtual environment**

   ```bash
   python -m venv .venv
   source .venv/bin/activate
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Create a `.env` file**

   ```bash
   GOOGLE_GENAI_USE_VERTEXAI=1
   GOOGLE_CLOUD_PROJECT=your_project_id
   GOOGLE_CLOUD_LOCATION=us-central1
   MODEL=gemini-2.0-flash
   DISABLE_WEB_DRIVER=1
   ```

   *(You can optionally include `SERPAPI_KEY` if you want to enable web-based paper search.)*

---

## ▶️ Running the Agent

1. **Start the ADK Web Interface**

   ```bash
   adk web --host 0.0.0.0 --port 8002
   ```

2. **Open in Browser**

   * In Google Cloud Shell:
     Click **Web Preview → Change Port → 8002**
   * Visit:
     `https://<your-cloud-shell-url>-8002.googleusercontent.com/dev-ui/`

3. **Create a new session**
   Make sure *Token Streaming* is **OFF** to avoid SSE errors.

---

## 🧩 Expected Output

After running the above prompt, the assistant:

1. Analyzes the research profile
2. Extracts major keywords
3. Searches for related papers
4. Generates a full **comparison report** with:

   * Annotated bibliography
   * Research connections
   * Thematic analysis
   * Final summary of insights

---

## 🧠 System Workflow

1. **Input:** Topic + Research Profile
2. **Profiler Agent:** Extracts key themes and concepts
3. **Searcher Agent:** Retrieves relevant publications
4. **Comparison Loop:** Iteratively refines analysis and critique
5. **Formatter Agent:** Produces the final structured report

---

## 🎥 YouTube Walkthrough

📺 **Watch the complete video tutorial here:**
👉 [Academic Research Assistant using Google ADK](https://youtu.be/90ooj1W8mAc)

**Includes:**

* Full setup in Google Cloud Shell
* Step-by-step agent explanation
* Live run and report generation
* Output review and architecture recap

---

## 🧾 License

This project is released under the [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0).

---

## ✨ Credits

* **Authors:** [Sri-Krishna-V](https://github.com/Sri-Krishna-V)
* **Base Repository:** [awesome-adk-agents](https://github.com/Sri-Krishna-V/awesome-adk-agents)
* **Powered by:** Google Agent Development Kit (ADK) + Gemini 2.5 Flash
