# LangGraph Components

This project demonstrates how to build an AI agent using LangGraph core components.

## Overview

The project builds a research assistant agent that uses a language model and a search tool to answer user questions.

The agent workflow includes:

1. User sends a question
2. LLM decides whether a tool is needed
3. Agent calls Tavily Search
4. Search results are returned as observations
5. LLM generates the final answer

## LangGraph Concepts Used

- StateGraph
- AgentState
- Nodes
- Edges
- Conditional Edges
- Tool Messages
- Tool Calling
- Graph Compilation
- Mermaid Graph Visualization

## Main Components

### AgentState

Stores the conversation messages and allows the graph to keep track of the agent workflow.

### LLM Node

Calls the OpenAI chat model and decides the next action.

### Action Node

Executes tool calls requested by the model.

### Conditional Edge

Routes the workflow:

- If tool call exists → go to action node
- If no tool call exists → end

## Tools Used

- Tavily Search
- OpenAI Chat Model
- LangGraph
- LangChain

## Skills Demonstrated

- LangGraph workflow design
- Tool-enabled agents
- Conditional routing
- Search tool integration
- State management
- Agent orchestration
- Python development
- Jupyter Notebook development

## Example Questions Tested

- What is the weather in San Francisco?
- What is the weather in San Francisco and Los Angeles?
- Who won the Super Bowl in 2024?
- What state is the winning team headquartered in?
- What is the GDP of that state?

## Key Learning Outcome

This project helped me understand how LangGraph structures agent behavior through nodes, edges, conditional routing, and state management. It also demonstrated how an AI agent can decide when to use external tools and continue reasoning after receiving tool results.
