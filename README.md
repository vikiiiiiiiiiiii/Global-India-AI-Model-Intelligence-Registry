# Global & India AI Model Intelligence Registry (Multi-Agent Control Center)

An autonomous, 4-node **LangGraph** multi-agent system built with **Gemini 2.5 Flash**, **Pydantic**, **SQLite**, and **Gradio** to discover frontier & open-weight LLMs, normalize **18% GST-inclusive INR pricing**, and audit **India DPDP Act & RBI cloud data residency (Mumbai/Pune)**.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vikiiiiiiiiiiii/Global-India-AI-Model-Intelligence-Registry/blob/main/Global_India_AI_Model_Intelligence_Registry.ipynb)

## Architecture: 4-Node Stateful LangGraph Pipeline
1. **Discovery Scout Agent:** Fetches live model catalogs, context windows, and token pricing from OpenRouter and Hugging Face Hub APIs while filtering out uncensored/abliterated weights.
2. **INR & 18% GST Normalizer:** Pulls live USD-to-INR exchange rates and computes deterministic 18% Indian enterprise GST-inclusive pricing per 1M tokens.
3. **India Sovereignty Auditor:** Uses **Gemini 2.5 Flash** enforced by **Pydantic** structured outputs to audit regional cloud availability (**GCP `asia-south1` Mumbai**, **Vertex AI India**, **AWS `ap-south-1` Mumbai**, **Azure Central India Pune**), deployment topologies (*VPC Dedicated* vs. *Serverless API*), and Indic language readiness.
4. **SQLite Registry Persister:** Stores normalized model records locally for deterministic SQL filtering and zero-latency TCO comparisons.

## Interactive Control Center (Gradio)
* **Compliance & Cost Filters:** Toggle strict India Data Residency (Mumbai/Pune) and 18% GST-inclusive INR pricing.
* **Enterprise TCO Engine:** Ranks models across 5 enterprise segments (**BFSI & Regulated Compliance**, **Agentic Coding & DevOps**, **Indic Multilingual Support**, **High-Volume Document Extraction**, and **Enterprise RAG & Legal Synthesis**).
* **Citation-Backed Reports:** Generates downloadable Markdown comparative architecture reports with direct links to cloud residency and statutory documentation.

## Tech Stack
* **Orchestration & LLMs:** Python, LangGraph, LangChain, Gemini 2.5 Flash, Pydantic v2
* **Data & Storage:** SQLite3, Pandas, OpenRouter API, Hugging Face Hub API
* **Frontend & Reporting:** Gradio, Automated Markdown TCO Report Generator

## Quickstart (Google Colab)
1. Click the **Open in Colab** badge above.
2. Open **Secrets** (🔑 icon in the left Colab sidebar) and add `GEMINI_API_KEY`.
3. Run all cells sequentially to initialize the SQLite database, execute an autonomous discovery scan, and launch the Gradio dashboard.
