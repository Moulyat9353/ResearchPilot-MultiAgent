# ResearchPilot
This project demonstrates a **multi-agent system** built using LangGraph.  

# **Key Features:**
- Web search via Tavily API
- Web scraping to extract text from URLs
- LLM-driven routing of agents (supervisor logic)
- Document outlining and writing
- Saving outputs as Markdown or text files

## 🚀 Overview

The pipeline consists of multiple specialized **agents**, each responsible for a piece of the task:

- **Search Agent**  
  Finds relevant web pages for a user query using Tavily API.

- **Web Scraper Agent**  
  Downloads and extracts text from web pages.

- **Supervisor**  
  An LLM-driven node that decides which agent should act next based on context and progress.

- **Writing Team**  
  - **Note Taker Agent** — generates an outline for the document.
  - **Doc Writer Agent** — writes detailed content to disk in `.txt` or `.md` format.

All agents communicate via a stateful graph architecture, allowing complex multi-step reasoning.

## 🔐 API Keys  

The pipeline requires:

- OpenAI API Key

- Tavily API Key

## 📚 Technologies Used  

- LangGraph – graph-based orchestration for LLM agents

- LangChain – tooling and agent interfaces

- OpenAI GPT-4o – LLM backbone for agent logic

- Tavily API – web search integration

- BeautifulSoup – HTML parsing for scraping

- tiktoken – token counting to manage LLM context limits
