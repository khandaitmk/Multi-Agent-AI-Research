# 🔍 Multi-Agent AI Research System

An intelligent multi-agent research assistant that automates the complete research workflow using specialized AI agents. The system searches the web, extracts detailed information from trusted sources, generates a structured research report, and performs quality review using multiple collaborating AI agents.

---

# 🚀 Features

* 🌐 Web Search using Tavily Search API
* 📄 Content Extraction using BeautifulSoup
* 🤖 Specialized AI Agents for different tasks
* 📝 Automated Research Report Generation
* 🔍 Critical Review and Feedback Generation
* ⚡ Built using LangChain and Mistral AI
* 🧩 Modular Multi-Agent Architecture

---

# 🏗️ System Architecture

```text
                    ┌─────────────────┐
                    │     User        │
                    │  Research Query │
                    └────────┬────────┘
                             │
                             ▼
                ┌─────────────────────────┐
                │     Search Agent        │
                │      (Tavily API)       │
                └─────────┬───────────────┘
                          │
                          ▼
                ┌─────────────────────────┐
                │      Reader Agent       │
                │   (BeautifulSoup Tool)  │
                └─────────┬───────────────┘
                          │
                          ▼
                ┌─────────────────────────┐
                │      Writer Agent       │
                │  Research Report Draft  │
                └─────────┬───────────────┘
                          │
                          ▼
                ┌─────────────────────────┐
                │      Critic Agent       │
                │ Review & Improvements   │
                └─────────┬───────────────┘
                          │
                          ▼
                ┌─────────────────────────┐
                │      Final Report       │
                └─────────────────────────┘
```

---

# 🔄 Workflow

### Step 1: Search Agent

* Receives the user's research topic.
* Uses Tavily Search API to gather recent and reliable information.
* Collects relevant sources and summaries.

### Step 2: Reader Agent

* Analyzes search results.
* Selects the most relevant source.
* Scrapes webpage content using BeautifulSoup.
* Extracts detailed information from the article.

### Step 3: Writer Agent

* Combines search results and extracted content.
* Generates a structured research report.
* Organizes information into a readable format.

### Step 4: Critic Agent

* Reviews the generated report.
* Identifies weaknesses and missing information.
* Provides constructive feedback and suggestions.

---

# 🛠️ Tech Stack

### LLM

* Mistral AI

### Frameworks

* LangChain
* LangGraph

### Search

* Tavily Search API

### Web Scraping

* BeautifulSoup4
* Requests

### Utilities

* Python Dotenv
* Rich
* Pydantic

---

# 📊 Pipeline Overview

```text
Research Topic
      │
      ▼
Search Agent
      │
      ▼
Search Results
      │
      ▼
Reader Agent
      │
      ▼
Scraped Content
      │
      ▼
Writer Agent
      │
      ▼
Research Report
      │
      ▼
Critic Agent
      │
      ▼
Feedback + Improvements
```

---

# 🎯 Future Improvements

* Multi-source content aggregation
* Citation generation
* PDF report export
* Memory-enabled agents
* Advanced LangGraph workflows
* Streamlit/Web interface
* RAG-based knowledge storage
* Research report quality scoring
* Research history tracking

---

# 📜 License

This project is created for educational and research purposes.
