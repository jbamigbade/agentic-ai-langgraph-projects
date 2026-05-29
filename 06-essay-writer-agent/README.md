# Essay Writer Agent

First and foremost, I give all glory to God for His grace, wisdom, and faithfulness throughout this learning journey.

This project demonstrates a complete autonomous essay-writing agent built using LangGraph, LangChain, OpenAI, and Tavily Search.

## Overview

The agent follows a multi-step workflow:

1. Create an essay plan
2. Research the topic
3. Generate a draft
4. Critique the draft
5. Research improvements
6. Revise the essay
7. Repeat until the revision limit is reached

This workflow demonstrates how AI agents can iteratively improve their own work.

---

## Technologies Used

- Python
- LangGraph
- LangChain
- OpenAI GPT
- Tavily Search
- Pydantic
- SQLite Checkpointing
- Jupyter Notebook

---

## Architecture

```text
Planner
   ↓
Research Plan
   ↓
Generate Draft
   ↓
Should Continue?
   ↓
Reflect
   ↓
Research Critique
   ↓
Generate Revised Draft
   ↓
Final Essay
```

---

## Components Implemented

### Planning Agent

Creates a structured essay outline before writing begins.

```python
plan_node()
```

---

### Research Agent

Generates search queries and gathers information using Tavily Search.

```python
research_plan_node()
```

---

### Essay Generation Agent

Uses:

- User task
- Essay plan
- Research content

to generate a complete essay draft.

```python
generation_node()
```

---

### Reflection Agent

Reviews the essay and generates constructive critique.

```python
reflection_node()
```

---

### Critique Research Agent

Searches for additional information based on weaknesses identified during reflection.

```python
research_critique_node()
```

---

### Conditional Routing

Controls whether the workflow continues or ends.

```python
should_continue()
```

This allows iterative improvement until the maximum revision count is reached.

---

## LangGraph Concepts Demonstrated

- StateGraph
- Nodes
- Edges
- Conditional Edges
- Agent State
- Shared State Management
- Iterative Workflows
- Reflection Loops
- Agentic Search
- Memory
- Persistence

---

## Agent State

The workflow maintains:

```python
task
plan
draft
critique
content
revision_number
max_revisions
```

This shared state allows every node to collaborate on improving the essay.

---

## Skills Demonstrated

- Agentic AI
- LangGraph
- LangChain
- Multi-Step Workflows
- Reflection Loops
- Agentic Search
- Tool Calling
- Structured Outputs
- Pydantic Validation
- Tavily Integration
- State Management
- Workflow Orchestration
- Prompt Engineering
- Python Development

---

## Key Learning Outcomes

This project demonstrates how AI systems can:

- Plan before acting
- Research external information
- Generate content
- Critique their own work
- Improve through iteration
- Maintain state across multiple workflow steps

These concepts form the foundation of modern autonomous AI agents.

---

## Files

- essay_writer_agent.ipynb
