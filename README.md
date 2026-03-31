# 🚀 Day 7: Building a Two-Way Interactive AI Agent

## 📌 Project Overview
Transitioning from simple one-way notifications (Day 6), today's mission was to build a fully interactive, conversational AI Agent. I architected a system where a user can send dynamic text inputs, have those inputs processed by an LLM (Llama-3), and receive real-time, context-aware responses back in a chat interface.

## ⚙️ Tech Stack & Architecture
* **Interface:** n8n Built-in Chat Trigger
* **Brain (LLM):** Llama-3 (via OpenRouter API)
* **Framework:** n8n Advanced AI Agent Node

## 🧠 What I Learned Today
* **Architectural Pivoting:** Encountered localhost limitations with Telegram webhooks and successfully pivoted to utilizing n8n's native Chat Trigger to test and validate the AI logic first.
* **Agentic Frameworks:** Shifted from standard programmatic nodes to "Agent" nodes, which dynamically handle context and routing rather than relying on hardcoded JSON paths.
* **Token Management:** Troubleshooted API credit limitations by dynamically restricting the `Max Tokens` parameter for the LLM output, ensuring efficient and cost-effective API calls.
* **Dynamic Prompting:** Successfully mapped live user inputs into the LLM's prompt window without relying on static strings.
