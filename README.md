# Machine Learning & AI Projects

This page collects all of my ML/AI-focused projects in one place.  
Most of them live on GitHub and are linked directly from here.

---
## Quick Overview

| Project | What it is | Tech | Highlights |
|--------|------------|------|-----------|
| [AI Inference Microservice](https://github.com/mgorripa/AI_Inference_Microservice) | Production-style ML inference service with load testing and observability | Python, C++, Go, FastAPI, Docker, K8s, Prometheus | Custom C++ op via pybind11, HPA-based autoscaling, metrics-driven load tests |
| [Agent 1 – Customer Service Agent](https://github.com/mgorripa/agent1-customer-service-openai-llamaindex) | Customer support agent using LlamaIndex and OpenAI | Python, OpenAI API, LlamaIndex, Jupyter | Customer query handling, retrieval-augmented responses, clear notebook workflow |
| [Agent 2 – LlamaIndex Agentic Projects](https://github.com/mgorripa/agent2-llamaindex-projects) | Collection of multi-agent and REACT-style workflows | Python, LlamaIndex, Jupyter | Multi-agent hospital scenario, REACT workflows, reflection and scheduling patterns |
| [AsteroidInsight (Asterostellar)](https://github.com/mgorripa/AsteroidInsight) | Data analysis and Django-based structure for asteroid data | Python, Jupyter, Django | EDA notebook, reports, and a web backend scaffold for analytics |
| [Multicast Market Data Lab](https://github.com/mgorripa/multicast-market-data-lab) | Network lab producing time-series metrics for later ML/analysis | Python, iperf2, containerlab | Parses jitter/loss logs into CSV, good example of telemetry pre-processing for ML |

---

## Detailed Project Descriptions


## 1. Production-Flavored ML Systems

### 🔹 AI Inference Microservice  
**Repo:** https://github.com/mgorripa/AI_Inference_Microservice  

A tiny, production-flavored inference microservice that brings together model serving, load testing, and basic observability. :contentReference[oaicite:0]{index=0}  

**What I built:**
- A Python + FastAPI inference service backed by **PyTorch**.
- A **C++ / pybind11** custom op integrated into the inference path.
- A **Golang load generator** that sends requests and exports **Prometheus** metrics.
- Docker + Kubernetes deployment with **Horizontal Pod Autoscaling (HPA)** configured.
- A small roadmap documenting how to extend this to **CUDA / Triton / CUTLASS / vLLM**.

**Skills demonstrated:**
- End-to-end ML system design (from model to API to load testing).
- Combining Python, C++, and Go in a single production-style stack.
- Basic MLOps patterns: containers, K8s, metrics, and autoscaling.

---

## 2. Agentic AI & LLM Projects

### 🔹 Agent 1 – Customer Service Agent (OpenAI + LlamaIndex)  
**Repo:** https://github.com/mgorripa/agent1-customer-service-openai-llamaindex  

My first full agentic AI project: a **customer service agent** built using OpenAI models and LlamaIndex, implemented in a Jupyter Notebook. :contentReference[oaicite:1]{index=1}  

**What it does:**
- Automates customer support tasks like query triage and intent understanding.
- Uses **OpenAI API** as the LLM backbone for reasoning and response generation.
- Uses **LlamaIndex** for data ingestion, retrieval, and orchestration.
- Runs in Jupyter for easy experimentation and explanation.

**Skills demonstrated:**
- Prompt and agent design for realistic customer-service workflows.
- LLM + retrieval integration with LlamaIndex.
- Clear documentation of purpose, tech stack, and usage.

---

### 🔹 Agent 2 – Agentic AI Projects with LlamaIndex  
**Repo:** https://github.com/mgorripa/agent2-llamaindex-projects  

A curated collection of agentic-AI projects I built while taking the LinkedIn Learning course  
**“Hands-On Agentic AI: Building AI Agents with LlamaIndex.”** :contentReference[oaicite:2]{index=2}  

**What’s inside:**
- `01_basic_agent.ipynb` – minimal single-agent example.
- `02_healthcare_react.ipynb` – a REACT-style agent for a healthcare scenario.
- `03_summarization_reflection.ipynb` – summarization and reflection workflows.
- `04_simple_workflow.ipynb` – chaining multiple agent steps together.
- `05_react_workflows_scheduling.ipynb` – REACT workflows with scheduling / control flow.
- `06_multi_agent_hospital.ipynb` – multi-agent coordination in a hospital setting.

**Skills demonstrated:**
- Designing **multi-step and multi-agent** LLM workflows.
- Using LlamaIndex to orchestrate tools, memory, and data retrieval.
- Experimenting with different patterns like REACT, reflection, and scheduling.

---

## 3. Data & ML Exploration

### 🔹 AsteroidInsight (Asterostellar)  
**Repo:** https://github.com/mgorripa/AsteroidInsight  

A project around asteroid data (“Asterostellar”) with exploratory data analysis and a Django-based structure for further work. :contentReference[oaicite:3]{index=3}  

**What’s in the repo:**
- `EDA.ipynb` – Jupyter notebook for exploratory analysis of asteroid-related data.
- A Django project (`asterostellar/`) wired via Makefile commands:
  - `make venv`, `make install`, `make run`, `make migrate`, `make static`. :contentReference[oaicite:4]{index=4}  
- Phase 1 and Phase 2 project reports (PDFs).

**Skills demonstrated:**
- Jupyter-based data exploration and reporting.
- Structuring a data project with a **web backend (Django)**.
- Laying groundwork for turning analysis into a user-facing ML/analytics app.

---

## 4. (Bonus) Infra & Data Labs That Support ML Thinking

These are not strictly “ML models” but they are highly relevant to **data + systems for ML/AI**.

### 🔹 Multicast Trading Lab – Metrics & Log Parsing  
**Repo:** https://github.com/mgorripa/multicast-market-data-lab  

Lab focused on UDP multicast across a spine/leaf fabric with PIM-SM and BFD. It generates traffic via `iperf2`, logs per-interval jitter and loss, and parses those logs to CSV using a small Python script. :contentReference[oaicite:5]{index=5}  

**Why it’s relevant here:**
- Shows how I **collect, parse, and summarize time-series performance data**, which is exactly the kind of input real ML models use for network reliability and trading-latency analysis.

---

In the future, I may add:
- Time-series forecasting projects (XGBoost, LSTM/BiLSTM, transformers) for cloud resource prediction.
- Explainable AI (SHAP) experiments from my thesis work.
- More production-style deployments (Kubernetes, autoscaling, observability).
