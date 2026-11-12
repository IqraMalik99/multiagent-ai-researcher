# Multi-Agent AI Researcher


Give it a topic.

A team of AI agents will search the web, read the pages, write a report, and then review it.


---


## What does it do?


You type a topic, for example:

`Impact of AI agents on customer support`


The project then:

1. Searches the web for good sources
2. Reads and scrapes those web pages
3. Writes a detailed research report
4. Reviews the report and points out weak parts


---


## The 4 agents


**1. Search Agent**

Finds up-to-date sources on the web using Tavily.


**2. Reader Agent**

Opens the web pages and extracts the text.


**3. Writer Agent**

Uses the collected text to write the research report.


**4. Critic Agent**

Checks the report and suggests improvements.


---


## How the flow works


```text
Topic
  |
  v
Search Agent   -->  finds sources
  |
  v
Reader Agent   -->  scrapes pages
  |
  v
Writer Agent   -->  writes report
  |
  v
Critic Agent   -->  reviews report
  |
  v
Final report + feedback
```


Each agent passes its result to the next one.

This keeps every step simple and focused.


---


## Features


- Real-time web search (Tavily)

- Automatic web page reading and scraping

- Detailed research reports

- Built-in review of every report

- Google Gemini as the AI model

- Built with LangChain


---


## Tech stack


- Python

- LangChain

- Google Gemini

- Tavily Search API

- uv (for the virtual environment)


---


## Project structure


```text
multiagent-ai-researcher/
|
|-- agents.py          -> the agents and chains
|-- tools.py           -> search and scraping tools
|-- pipeline.py        -> runs everything in order
|-- requirements.txt   -> dependencies
|-- .env.example       -> template for API keys
|-- .gitignore
|-- README.md
```


---


## How to run it


**Step 1: Clone the project**

```bash
git clone https://github.com/IqraMalik99/multiagent-ai-researcher.git
cd multiagent-ai-researcher
```


**Step 2: Create a virtual environment**

```bash
uv venv
```


**Step 3: Activate it**

Windows:

```bash
.venv\Scripts\activate
```

Mac / Linux:

```bash
source .venv/bin/activate
```


**Step 4: Install the packages**

```bash
uv pip install -r requirements.txt
```


**Step 5: Add your API keys**

Copy `.env.example` to a new file named `.env`.

Then add your keys:

```env
GOOGLE_API_KEY=your_gemini_key
TAVILY_API_KEY=your_tavily_key
```

Get the keys here:

- Gemini: https://aistudio.google.com/app/apikey
- Tavily: https://tavily.com


**Step 6: Run it**

```bash
python pipeline.py
```

Enter a topic and wait for the final report.


---


## Future improvements


- Save reports as PDF or Markdown

- Add source links to the report

- Let the critic send the report back to the writer for a rewrite

- Add a web interface


---


## Author


**Iqra Malik**

AI and Full-Stack Engineer

GitHub: https://github.com/IqraMalik99

Email: iqra.aatzaz.malik@gmail.com
