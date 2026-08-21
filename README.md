# ASK&ACT — Agentic AI Orchestration & Specialized Multi-Agent Engine

ASK&ACT brings multiple specialized AI capabilities together within one agentic AI platform. It supports code review, stock intelligence, market research, YouTube content analysis, and general AI conversation through modular AI workflows.

## What ASK&ACT Offers

### Code Review Through Multiple AI Checks

Submitted code is examined through specialized checks covering quality, correctness, security, performance, and testing.

### Natural-Language Stock Intelligence

The platform understands stock-related questions written in natural language and coordinates the relevant analysis to provide focused financial insights.

### Market Data and Trend Analysis

Market information for selected stocks is retrieved and analyzed across observable price, volume, and trend patterns.

### Web and Social Intelligence

Relevant online information is collected to identify current discussions, trends, and market-related signals.

### Recent News Intelligence

Company and market news is processed to produce concise summaries, sentiment, and important developments.

### YouTube Content Analysis

The content of YouTube videos is analyzed to generate topic-focused insights and summaries.

### General AI Conversation

A conversational AI interface handles general-purpose questions and interactions.

### Multi-Agent Graph Workflows

Graph-based orchestration connects specialized processing stages and coordinates complex AI tasks.

## Architecture Behind ASK&ACT

### Specialized Processing for Different Tasks

Each major task follows its own processing workflow, making the system more focused than relying on a single general-purpose AI agent.

### Modular Architecture

Independent agents, tools, and processing components can be extended without requiring changes throughout the entire application.

### Local AI and Privacy

The architecture can use local open-source models, reducing dependency on external models and keeping sensitive processing closer to the user.

### Separate Application Layers

A React frontend and FastAPI backend keep the user interface separated from the AI processing layer.

## How the System Works

### Step 1 — Submit the Request

The user provides a question, code, stock query, or YouTube URL through the web interface.

### Step 2 — Identify and Process the Required Workflow

The backend determines which workflow is needed and coordinates the appropriate AI agents, tools, and data sources.

### Step 3 — Combine the Analysis

The individual processing results are brought together by the workflow to create a unified response.

### Step 4 — Deliver the Result

The processed output is returned through the backend and displayed within the React interface.

## Specialized Agent Workflows

### Code Review Flow

`Code → Multiple Specialized Checks → Result Evaluation → Final Review`

The code-review process separates its evaluation responsibilities before combining the results into a consolidated review.

### Stock Intelligence Flow

`User Query → Query Understanding → Relevant Analysis → Information Synthesis → Stock Insights`

The workflow determines what information is needed for the user's financial question before producing the resulting stock insights.

### YouTube Analysis Flow

`YouTube URL → Content Retrieval → Topic Understanding → Analysis → Summary`

The system retrieves the underlying video content and uses it to generate information focused on the relevant topics.

### General AI Chat Flow

`User Message → AI Processing → Response`

A dedicated conversational workflow processes general-purpose user interactions.

## Technology Foundation

| Domain               | Technologies                                   |
| :------------------- | :--------------------------------------------- |
| **Frontend**         | React, JavaScript, Tailwind CSS, Vite          |
| **Backend**          | Python, FastAPI, Uvicorn                       |
| **AI Orchestration** | LangGraph, LangChain                           |
| **AI Models**        | Local LLMs through Ollama / Open-Source Models |
| **Market Data**      | yfinance                                       |
| **Video Content**    | YouTube Transcript Retrieval                   |
| **Development**      | Git, GitHub, VS Code                           |

## Environment Requirements

The platform requires:

* Python 3.10+
* Node.js 18+
* npm
* Git
* Local Ollama runtime for the recommended local AI architecture
* Sufficient system resources for the selected local model

