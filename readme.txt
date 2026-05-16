# Multi-Agent Researcher

A multi-agent AI research pipeline built using LangChain, Gemini, and Tavily Search API.

This project demonstrates how multiple AI agents can collaborate to:
- Search the web
- Read and scrape webpages
- Generate detailed research reports
- Critically review the generated reports

---

# Features

- 🔍 AI Web Search Agent
- 📖 AI Reader/Scraper Agent
- ✍️ AI Research Writer
- 🧪 AI Critic/Reviewer
- 🌐 Real-time web search using Tavily
- 🤖 Google Gemini LLM integration
- 🧠 Multi-agent workflow architecture

---

# Project Structure

```text
multiagent-researcher/
│
├── agents.py          # AI agents and chains
├── tools.py           # Search and scraping tools
├── pipeline.py        # Main research pipeline
├── requirements.txt   # Project dependencies
├── README.md
├── .env.example
└── .gitignore
