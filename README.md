# OpenAI Agents SDK Notes

## 🧠 What is the OpenAI Agents SDK?

The **OpenAI Agents SDK** is a lightweight, production-ready framework to build **agentic AI apps** using a small set of powerful primitives. It's designed to be simple, flexible, and easy to use — while still enabling the construction of complex multi-agent systems.

> It’s a polished successor to the experimental *Swarm* framework.

---

## 🔧 Core Primitives

The SDK is centered around **three main primitives**:

- **Agents**: LLMs with instructions and tools.
- **Handoffs**: Mechanism for delegating tasks between agents.
- **Guardrails**: Input validation logic for safer and more controlled interactions.

These primitives, when combined with Python, let you model complex workflows with minimal overhead.

---

## 🎯 Why Use the Agents SDK?

The SDK is built on two core design principles:

1. **Minimalist, but powerful** – Just enough features to be productive without overcomplication.
2. **Works out of the box** – Easy to use, but highly customizable.

---

## 🌟 Main Features

- **🌀 Agent Loop**  
  Auto-manages tool execution, result flow, and iteration until the LLM finishes the task.

- **🐍 Python-First Design**  
  Chain and orchestrate agents using native Python syntax—no need to learn new DSLs or frameworks.

- **🤝 Handoffs**  
  Agents can pass tasks to other agents seamlessly.

- **🛡️ Guardrails**  
  Run validations alongside agent logic to catch bad inputs early.

- **🧰 Function Tools**  
  Turn any Python function into a tool. Schemas are auto-generated and validated using Pydantic.

- **🔍 Tracing**  
  Debug, visualize, and monitor agent workflows. Built-in support for OpenAI's eval/fine-tune/distill tools.

---

## 🚀 Installation

```bash
pip install openai-agents

