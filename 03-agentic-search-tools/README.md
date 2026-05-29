# Agentic Search Tools

This project demonstrates how AI agents can search the web, retrieve information, and extract relevant data to answer user questions.

## Overview

The project integrates Tavily Search and DuckDuckGo Search to allow an AI workflow to gather real-time information from external sources.

The workflow includes:

1. User submits a query
2. Search engine retrieves relevant webpages
3. Agent extracts website content
4. Agent processes retrieved information
5. Agent generates useful responses

## Technologies Used

- Python
- Tavily Search API
- DuckDuckGo Search
- BeautifulSoup
- Requests
- OpenAI
- Jupyter Notebook

## Features Implemented

### Tavily Search

Used Tavily's AI-native search engine to:

- Search the web
- Retrieve current information
- Return summarized answers

Example:

```python
result = client.search(
    "What is in Nvidia's new Blackwell GPU?",
    include_answer=True
)
```

### DuckDuckGo Search

Used DuckDuckGo to:

- Find relevant websites
- Retrieve URLs
- Gather sources for further analysis

### Web Scraping

Implemented webpage scraping using:

- Requests
- BeautifulSoup

The workflow:

1. Retrieve webpage
2. Parse HTML
3. Extract useful text
4. Prepare content for AI processing

### Weather Information Retrieval

Built a simple search workflow that:

- Searches weather websites
- Retrieves weather information
- Extracts useful content for decision-making

## Skills Demonstrated

- Agentic Search
- Information Retrieval
- Web Scraping
- API Integration
- Search Tool Development
- Data Extraction
- External Knowledge Retrieval
- Python Development

## Key Learning Outcomes

This project demonstrates how AI agents can move beyond static model knowledge by retrieving and processing real-time information from the web.

The techniques used here form the foundation for:

- Research Agents
- Retrieval-Augmented Generation (RAG)
- Search Assistants
- AI Research Workflows
- Knowledge Agents

## Files

- agentic_search_tools.ipynb
