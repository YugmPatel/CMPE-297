# Agent C: MCP Tools-based Bug Assistant

Based on: https://cloud.google.com/blog/topics/developers-practitioners/tools-make-an-agent-from-zero-to-assistant-with-adk

## Overview

This agent uses Model Context Protocol (MCP) tools to provide intelligent bug assistance. It can analyze code, identify bugs, suggest fixes, and even apply patches automatically.

## Features

- Code analysis with MCP tools
- Bug detection and classification
- Automated fix suggestions
- Patch generation and application
- Integration with version control

## Setup

1. Install dependencies:
```bash
cd agent-c-mcp-bug-assistant
pip install -r requirements.txt
```

2. Configure environment:
```bash
cp .env.example .env
# Edit with your project details
```

## Usage

Analyze a file for bugs:
```bash
python bug_assistant.py --file path/to/code.py
```

Interactive debugging session:
```bash
python bug_assistant.py --interactive
```

Analyze entire directory:
```bash
python bug_assistant.py --directory ./src
```

## MCP Tools

The agent uses these MCP tools:
- `analyze_code`: Static code analysis
- `detect_bugs`: Bug pattern detection
- `suggest_fix`: Generate fix suggestions
- `apply_patch`: Apply code patches

## Output

- Bug reports with severity levels
- Fix suggestions with explanations
- Patch files (`.patch`)
- Analysis logs
