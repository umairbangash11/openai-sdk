# 📘 OpenAI Agents SDK Notes

## Main: Overview

The **OpenAI Agents SDK** is a production-grade toolkit for developing *agentic AI applications* in Python. It offers a minimal and intuitive interface for orchestrating agents, tools, and control flows with traceability and extensibility.

Originally built as a successor to the Swarm experimental framework, this SDK simplifies the process of building complex AI applications by offering only a few powerful primitives.

---

## Main: Key Components

### 🔹 Agents
- Core logic units powered by LLMs.
- Defined with instructions and an optional toolset.
- Can perform tasks autonomously or as part of a system.

### 🔹 Handoffs
- Delegate subtasks from one agent to another.
- Allows complex workflows to be modular and maintainable.

### 🔹 Guardrails
- Validate and filter inputs before they're passed to agents.
- Ensure only safe or relevant inputs are processed.

---

## Main: Why Use the Agents SDK?

The SDK is guided by two main principles:

- **Minimal yet powerful**: Just a few constructs, but expressive enough for real-world complexity.
- **Highly customizable**: Sensible defaults that can be overridden when necessary.

### Subheading: Core Features

- ✅ **Agent Loop**  
  Built-in loop to automatically handle tool invocations and LLM outputs until task completion.

- 🐍 **Python-first Design**  
  Leverages standard Python features instead of introducing new abstractions.

- 🧠 **Handoffs**  
  Coordinate multiple agents to delegate work intelligently.

- 🛡️ **Guardrails**  
  Run validations in parallel; abort early if inputs fail checks.

- 🔧 **Function Tools**  
  Any Python function can be turned into a tool, with automatic schema and input validation using Pydantic.

- 📊 **Tracing & Evaluation**  
  Includes tools for debugging, monitoring, evaluating workflows, and fine-tuning models.

---

## Main: Installation

Install the OpenAI Agents SDK via pip:

```bash
pip install openai-agents
from agents import Agent, Runner

agent = Agent(name="Assistant", instructions="You are a helpful assistant")

result = Runner.run_sync(agent, "Write a haiku about recursion in programming.")
print(result.final_output)

