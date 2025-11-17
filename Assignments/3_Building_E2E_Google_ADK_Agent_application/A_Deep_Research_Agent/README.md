# Agent A: Deep Research Agent for Lead Generation

Based on: https://cloud.google.com/blog/products/ai-machine-learning/build-a-deep-research-agent-with-google-adk

## Overview

This agent performs deep research on companies to generate qualified leads. It searches the web, analyzes company information, and produces structured reports with contact details and insights.

## Features

- Multi-step research workflow
- Web search integration using Google Search
- Structured data extraction
- CSV and JSON report generation
- Configurable research depth

## Setup

1. Install dependencies:
```bash
cd agent-a-deep-research
pip install -r requirements.txt
```

2. Set up environment variables:
```bash
export GOOGLE_CLOUD_PROJECT="your-project-id"
export GOOGLE_GENAI_USE_VERTEXAI="true"
export GOOGLE_CLOUD_LOCATION="us-central1"
```

3. Authenticate with Google Cloud:
```bash
gcloud auth application-default login
```

## Usage

Run the research agent:
```bash
python research_agent.py
```

Or use the interactive mode:
```bash
python research_agent.py --interactive
```

## Output

The agent generates:
- `outputs/leads_report.csv` - Structured lead data
- `outputs/research_summary.json` - Detailed research findings
- `outputs/agent_log.txt` - Execution trace
