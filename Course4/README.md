# Course 4: Agentic AI

## Overview

This course covers building intelligent agents that can reason, plan, and use tools to solve complex problems. Learn ReAct agents, multi-agent systems, and conversational AI with tool use.

## Course Contents

### 1. **1_ImplementingToolsForAgenticAI.ipynb**
- Understanding tool/function definitions
- Tool schema and signatures
- Tool validation and error handling
- Integrating custom tools with LLMs

### 2. **2_BuildingToolsReactAgenticAIBuiltin.ipynb**
- ReAct (Reasoning + Acting) pattern
- Using built-in Langchain tools
- Tool selection strategies
- Observation and refinement loops

### 3. **03_BuildingToolsReactAgenticAIScratch.ipynb**
- Building custom tools from scratch
- Tool composition and chaining
- Creating domain-specific toolsets
- Advanced tool orchestration

### 4. **04_BuildingMultiUserConversationalAgenticAI.ipynb**
- Multi-user conversation management
- Session and context handling
- User-specific tool access controls
- Conversation persistence

### 5. **05_BuildingMultiAgentSystem.ipynb**
- Multi-agent coordination
- Agent specialization and roles
- Inter-agent communication
- Consensus and conflict resolution

## Core Concepts

### ReAct Framework
```
Thought → Action → Observation → Thought → ... → Final Answer
```

### Agent Loop
1. **Input**: User query or task
2. **Thought**: Agent reasons about the problem
3. **Action**: Agent selects and executes tools
4. **Observation**: Agent processes tool output
5. **Repeat** until task is complete
6. **Output**: Final response

## Key Technologies

- **Langchain Agents**: Agent framework and execution
- **LiteLLM**: Multi-model LLM access
- **Tool Definitions**: Structured tool specifications
- **Memory Systems**: Conversation and context management

## Learning Objectives

- Understand agent reasoning and planning
- Design and implement effective tools
- Build ReAct agents for complex tasks
- Create multi-agent systems
- Handle multi-user scenarios
- Debug and optimize agent behavior

## Running the Notebooks

1. Activate virtual environment
2. Install agent dependencies:
```bash
uv pip install langchain-community langgraph
```
3. Configure API keys in `.env`
4. Follow notebooks sequentially

## Data

`Data/search_data.json` - Sample data for search operations
`Data/sop_documents.json` - Standard Operating Procedures for agent reference

## Agent Design Patterns

- **ReAct**: Reasoning + Action
- **Tool-Use**: Function calling with structured outputs
- **Chain of Thought**: Explicit reasoning steps
- **Self-Reflection**: Agent evaluation and correction
- **Hierarchical**: Master agent coordinating sub-agents

## Best Practices

- Design tools with clear, focused purposes
- Provide detailed tool descriptions
- Handle edge cases and errors gracefully
- Log agent decisions for debugging
- Test with diverse inputs
- Monitor cost and latency

## Next Steps

Apply these concepts in the **Project: Insurance Agent Validation** to build a production system that validates insurance policies using an intelligent agent.
