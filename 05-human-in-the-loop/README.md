# Human in the Loop

This project demonstrates how to build a human-in-the-loop AI agent using LangGraph.

## Overview

The agent is designed to pause before executing tool actions, allowing a human user to inspect, approve, modify, or stop the workflow before the agent continues.

This is important for building safe and controllable AI systems.

## Technologies Used

- Python
- LangGraph
- LangChain
- OpenAI
- Tavily Search
- MemorySaver
- SqliteSaver
- Jupyter Notebook

## Features Implemented

### Human Approval Before Tool Execution

The graph is compiled with:

```python
interrupt_before=["action"]
