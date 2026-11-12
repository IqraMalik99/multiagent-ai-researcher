# 🤖 Multi-Agent Researcher

### An AI-powered research system where specialized agents collaborate to search, analyze, write, and critically review research reports.

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-blue?logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/LangChain-Framework-green?logo=chainlink&logoColor=white" />
  <img src="https://img.shields.io/badge/Google-Gemini-4285F4?logo=google&logoColor=white" />
  <img src="https://img.shields.io/badge/Tavily-Web_Search-orange" />
  <img src="https://img.shields.io/badge/Status-Active-success" />
</p>

---

## 📌 Overview

**Multi-Agent Researcher** is an AI-powered research pipeline built with LangChain, Google Gemini, and Tavily Search API.

Instead of relying on a single AI model to perform every task, the system uses multiple specialized agents that collaborate through a structured workflow.

Each agent has a dedicated responsibility — from discovering relevant information across the web to analyzing sources, writing comprehensive reports, and evaluating the final output.

The goal is to simulate a collaborative research team powered by AI.

## ✨ Key Features

| Feature | Description |
|---|---|
| 🔍 Web Search Agent | Finds relevant and up-to-date information using Tavily Search API. |
| 📖 Reader Agent | Scrapes and extracts useful content from web pages. |
| ✍️ Research Writer | Synthesizes collected information into structured research reports. |
| 🧪 Critic Agent | Evaluates reports for accuracy, clarity, completeness, and quality. |
| 🌐 Real-Time Search | Retrieves information from the web rather than relying only on model knowledge. |
| 🤖 Gemini Integration | Uses Google Gemini for AI-powered reasoning and content generation. |
| 🧠 Multi-Agent Architecture | Separates research responsibilities into specialized agents. |

## 🏗️ System Architecture

The pipeline follows a sequential multi-agent workflow.

```mermaid
flowchart TD
    A([User Research Query]) --> B[Research Pipeline]
    B --> C[🔍 Search Agent]
    C --> D[📖 Reader Agent]
    D --> E[✍️ Research Writer]
    E --> F[🧪 Critic Agent]
    F --> G[Final Research Report]

    C -.-> H[(Tavily Search API)]
    D -.-> I[Web Pages]
    E -.-> J[Google Gemini]
    F -.-> J

    style A fill:#1d4ed8,color:#fff
    style G fill:#15803d,color:#fff
```

### 🔄 How It Works

1. **User Input:** The user submits a research topic or question.
2. **Web Research:** The Search Agent discovers relevant sources using Tavily.
3. **Content Extraction:** The Reader Agent visits relevant pages and extracts useful information.
4. **Report Generation:** The Research Writer analyzes the collected information and creates a structured report.
5. **Critical Evaluation:** The Critic Agent reviews the generated report and identifies weaknesses.
6. **Final Output:** The pipeline returns the reviewed research report.

## 🧰 Tech Stack

| Technology | Purpose |
|---|---|
| Python | Core application development |
| LangChain | Agent and LLM orchestration |
| Google Gemini | AI reasoning and text generation |
| Tavily Search API | Real-time web research |
| Web Scraping Tools | Extracting webpage content |
| Python-dotenv | Environment variable management |

## 📂 Project Structure

```text
multiagent-researcher/
│
├── agents.py           # Specialized AI agents and chains
├── tools.py            # Web search and scraping tools
├── pipeline.py         # Main multi-agent research workflow
│
├── requirements.txt    # Python dependencies
├── .env.example        # Environment variable template
├── .gitignore          # Git ignored files
└── README.md           # Project documentation
```

## 🚀 Getting Started

Follow these steps to run the project locally.

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/multiagent-researcher.git

cd multiagent-researcher
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

Activate it:

**Windows (PowerShell)**

```powershell
.\venv\Scripts\Activate.ps1
```

**Linux / macOS**

```bash
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure Environment Variables

Create a `.env` file in the project root:

```env
GOOGLE_API_KEY=your_gemini_api_key
TAVILY_API_KEY=your_tavily_api_key
```

Get your API keys:

- [Google AI Studio – Gemini API](https://aistudio.google.com/apikey)
- [Tavily – Search API](https://tavily.com/)

### 5. Run the Project

```bash
python pipeline.py
```

## 💡 Example Use Cases

The Multi-Agent Researcher can be used for:

- **Technical Research:** Investigating emerging technologies, frameworks, and tools.
- **Market Research:** Exploring industry trends and competitor information.
- **Academic Research:** Gathering and organizing information around research topics.
- **Technology Comparisons:** Comparing tools, platforms, and technical approaches.
- **Industry Analysis:** Generating structured insights from multiple online sources.

## 🔮 Future Improvements

- [ ] Add iterative research and review loops.
- [ ] Implement source credibility scoring.
- [ ] Add citation and reference generation.
- [ ] Introduce parallel agent execution.
- [ ] Build an interactive Streamlit or Next.js interface.
- [ ] Add report export to PDF and Markdown.
- [ ] Implement LangGraph for more advanced agent orchestration.
- [ ] Add persistent research memory.

## 🎯 Project Goals

This project explores how multiple specialized AI agents can work together to solve complex information-gathering tasks.

It focuses on:

- Agent specialization and collaboration.
- LLM-powered research automation.
- Tool integration with external APIs.
- Structured information extraction.
- AI-generated content evaluation.

## 👩‍💻 Author

**Iqra Malik**

Full Stack Developer | Exploring Agentic AI

- GitHub: [Your GitHub Profile](https://github.com/YOUR_USERNAME)
- LinkedIn: [Connect with me](https://www.linkedin.com/in/iqra-malik-937a502a0/)

---

<p align="center">
  ⭐ If you find this project interesting, consider giving it a star!
  <br/>
  Built with curiosity and a passion for Agentic AI.
</p>
