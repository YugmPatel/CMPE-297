# Agent B: Advanced Tool Agent with Gemini CLI

Based on: https://medium.com/@derrickchwong/combine-adk-gemini-cli-and-cloud-run-c5dea5118853

## Overview

This agent demonstrates advanced tool integration by combining Google ADK with Gemini CLI. It creates a pipeline where the ADK agent can invoke Gemini CLI as a tool for specialized code generation and analysis tasks.

## Features

- ADK + Gemini CLI integration
- Tool-based architecture
- Code generation pipeline
- Cloud Run deployment ready
- Streaming responses

## Setup

1. Install dependencies:
```bash
cd agent-b-gemini-cli
pip install -r requirements.txt
```

2. Install Gemini CLI:
```bash
pip install google-generativeai
```

3. Set up environment:
```bash
export GOOGLE_CLOUD_PROJECT="your-project-id"
export GOOGLE_API_KEY="your-api-key"  # For Gemini CLI
export GOOGLE_GENAI_USE_VERTEXAI="true"
```

## Usage

Run the tool agent:
```bash
python tool_agent.py
```

Interactive mode:
```bash
python tool_agent.py --interactive
```

## Architecture

```
User Request → ADK Agent → Tool Selection → Gemini CLI Execution → Response
```

The agent decides when to use Gemini CLI as a specialized tool for tasks like:
- Complex code generation
- Multi-file refactoring
- Advanced analysis

## Output

- Generated code files
- Execution logs
- Tool invocation traces
