# 🔗 Prompt Chaining Workflow using LangGraph + Groq

This project demonstrates how to build a multi-step LLM pipeline using **LangGraph** and **Groq LLM models**.

The notebook showcases how to chain multiple prompts together, where the output of one LLM call becomes the input for the next step in a structured state-driven workflow.

---

## 📌 Project Overview

This workflow implements:

- LangGraph `StateGraph`
- Structured state using `TypedDict`
- Multi-step LLM reasoning
- Prompt chaining architecture
- Controlled state transitions

The graph structure:

START → Step 1 (Initial Prompt) → Step 2 (Refinement/Analysis) → END

---

## 🧠 What is Prompt Chaining?

Prompt chaining is a technique where:

1. An LLM generates an initial response.
2. That response is passed into a second prompt.
3. The second LLM call refines, analyzes, or transforms the output.
4. The final result is returned.

Instead of relying on a single prompt, the reasoning is broken into structured steps.

---

## 🏗 Workflow Architecture

<img width="107" height="432" alt="image" src="https://github.com/user-attachments/assets/aacd45dc-6d52-4923-9db7-981389302096" />


## 🛠 Technologies Used

- Python
- LangGraph
- LangChain Groq Integration
- Groq Llama Model
- TypedDict (for structured state)
- dotenv (for environment variables)
