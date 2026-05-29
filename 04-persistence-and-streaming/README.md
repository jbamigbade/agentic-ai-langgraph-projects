# Persistence and Streaming

This project demonstrates how to build production-ready AI agents using LangGraph persistence and streaming capabilities.

## Overview

The project focuses on allowing AI agents to:

- Remember previous interactions
- Resume interrupted workflows
- Stream outputs in real time
- Maintain conversational state
- Recover from failures

These capabilities are essential for long-running autonomous agents.

---

## Technologies Used

- Python
- LangGraph
- LangChain
- OpenAI GPT-4o
- Tavily Search
- MemorySaver
- SqliteSaver
- Jupyter Notebook

---

## Features Implemented

### Agent Memory

Implemented persistent agent memory using:

```python
MemorySaver()
```

This allows the agent to remember previous interactions and continue conversations.

---

### Checkpointing

Implemented workflow checkpointing using:

```python
SqliteSaver.from_conn_string(":memory:")
```

This enables:

- State recovery
- Workflow continuation
- Fault tolerance

---

### Thread Management

Used configurable thread IDs:

```python
thread = {
    "configurable": {
        "thread_id": "1"
    }
}
```

This allows:

- Multiple conversations
- Session tracking
- Agent persistence across interactions

---

### Streaming

Implemented LangGraph streaming:

```python
graph.stream(...)
```

Benefits include:

- Real-time visibility
- Progress monitoring
- Interactive workflows

---

### Search Tool Integration

Integrated Tavily Search for real-time information retrieval.

The agent can:

- Search the web
- Gather external information
- Use retrieved data in reasoning workflows

---

## Skills Demonstrated

- LangGraph
- Agent Memory
- Checkpointing
- State Persistence
- Streaming Workflows
- Thread Management
- Tool Calling
- OpenAI Integration
- Tavily Search
- Production Agent Design
- Python Development

---

## Key Learning Outcomes

This project demonstrates how modern AI agents can:

- Maintain memory across sessions
- Recover from interruptions
- Stream progress while working
- Manage long-running workflows
- Support production-scale deployments

These concepts are foundational for building enterprise-grade AI agent systems.

---

## Files

- persistence_and_streaming.ipynb
