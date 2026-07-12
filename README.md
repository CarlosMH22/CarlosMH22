## Hi, I'm Carlos 👋
### AI Engineer | LLM Applications & Multi-Agent Systems | Edge AI & IoT

I build AI systems end-to-end — from on-device LLMs optimized for NPU inference and LoRaWAN-connected industrial IoT gateways, to local multi-agent assistants with RAG, fine-tuned open models, and voice I/O. Currently focused on [TU_ESPECIALIDAD] at [EMPRESA_ACTUAL].

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white" />
  <img src="https://img.shields.io/badge/ONNX-005CED?style=for-the-badge&logo=onnx&logoColor=white" />
  <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white" />
  <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white" />
  <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" />
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
</p>

<p align="center"><em>Core AI/ML stack — keep only what's genuinely yours, remove the rest:</em></p>
<p align="center">
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" />
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" />
  <img src="https://img.shields.io/badge/Hugging%20Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black" />
</p>

---

### 🧠 What I'm working on
- 🤖 Building Jarvis, a local multi-agent AI assistant on consumer GPU hardware: hybrid retrieval, semantic routing, and reconciled long-term memory
- ⚡ Optimizing on-device LLM and vision inference for NPU/edge hardware (ONNX Runtime, quantized models)
- 📚 Running a self-directed LLM fine-tuning curriculum (Unsloth, QLoRA) from base models to instruction tuning

### 🚀 Featured Projects

> Most of my production work lives in private repositories. Here's a summary of what I've built:

**🏭 IQ9-Sentinel — On-Device Multi-Agent AI for Industrial Operations**
Multi-agent AI assistant for industrial field operators, running 100% locally on an edge gateway (QCS9075). Voice-controlled, with computer vision analytics and 5G connectivity.
- Deployed an end-to-end LoRaWAN sensor network (ChirpStack EU868, SX1302 concentrator, OTAA onboarding) with live vibration/temperature/pressure telemetry in Grafana
- Built an RTSP camera → GStreamer → anomaly-detection → push-to-talk alert pipeline (MCPTT)
- Debugged a Cat-1 cellular module (AT command sequencing, LTE band config, SIM registration) inside a multi-container Docker stack
`Python` `Multi-Agent Orchestration` `RAG` `Edge AI` `LoRaWAN` `Computer Vision`

**🍞 Smart Retail AI Kiosk**
Self-service ordering kiosk with an on-device LLM (Qwen2.5 via Ollama), a React/Vite frontend streaming responses over SSE from a FastAPI backend, a GStreamer camera pipeline, and an ONNX-based demographics inference module (age/gender) for retail analytics. Optimized inference for NPU execution (ONNX Runtime QNNExecutionProvider, HTP backend), resolving operator-compatibility constraints for on-device acceleration.
`React` `FastAPI` `Ollama` `ONNX Runtime` `GStreamer` `NPU Optimization`

**🧠 Jarvis — Local Multi-Agent AI Assistant**
A local multi-agent assistant running entirely on a consumer GPU (RX 570 8GB, Vulkan/RADV backend), serving Granite 4.1-8B through LM Studio with an optimized KV cache (Flash Attention, KV q8_0, 8192 ctx). A cosine-similarity SemanticRouter classifies incoming queries into five domains (personal assistant, dev, finance, music, general) at 92.7% accuracy in ~5ms per call. Retrieval is hybrid: BM25 + sentence embeddings + an ONNX reranker. Long-term semantic memory uses Mem0-style reconciliation (ADD/UPDATE/DELETE/NOOP via cosine similarity) on top of a layered session → semantic → core memory architecture, with tool-calling agents. Planned: Whisper STT, Piper TTS, an Arduino client, and a Meta Quest 3 WebXR HUD for physical deployment.
`Python` `FastAPI` `Granite 4.1-8B` `LM Studio` `Hybrid RAG (BM25 + Embeddings + ONNX Reranker)` `SemanticRouter` `Mem0`

**🤖 Multi-Agent Orchestration Framework**
The modular framework that emerged from building Jarvis: stateless agents running a ReACT loop, tools modeled as file=resource / function=operation, an orchestrator handling routing + context + gateway logic, and a dedicated LLM client layer. New agents are added by defining a system prompt and a tool set — no changes to the core loop required.
`Python` `Agentic AI` `ReACT` `LLM Orchestration`

**📈 AlphaTradingDesk — Quantitative Trading Dashboard**
A 4-tab desktop backtester for an Opening Range Breakout (ORB) strategy on US equities/options, built directly on the Interactive Brokers TWS API, with a paper-trading mode using regulatory market data snapshots.
`Python` `Tkinter` `Matplotlib` `Interactive Brokers API`

**⚙️ SecLang — DSL for Network Security Rules**
A compiler and rule-evaluation simulator for a custom domain-specific language for network security rules: lexer/parser (Flex & Bison), AST generation, JSON export, and priority-based packet simulation. Built as a team project at Universidad Panamericana.
`C++` `Flex` `Bison` `Compiler Design`

> Also built: a self-directed **LLM fine-tuning curriculum** (Unsloth, QLoRA, Qwen2.5-7B/Qwen3.5-4B) and a **3-stage course-scheduling optimizer** (JS scraper + Python backtracking solver) that processed 2,291+ university course sections.

### 🛠️ Skills

**LLM & GenAI:** Prompt engineering, hybrid RAG, semantic routing, agentic workflows, LLM fine-tuning (Unsloth, QLoRA)
**Edge AI & Embedded:** ONNX Runtime / QNNExecutionProvider (HTP backend), GStreamer pipelines, LM Studio, Edge Impulse
**IoT & Connectivity:** LoRaWAN / ChirpStack, cellular AT command interfaces, MCPTT
**Data & Storage:** SQLite, MongoDB
**Tools:** Docker, Flex/Bison, nmap, Git

### 🏆 Accomplishments
- 🥇 Kaggle Playground Series — Irrigation Prediction: Random Forest model achieved Macro F1 ~0.968, outperforming an XGBoost baseline
- 🔒 Home server security audit: penetration testing & hardening (nmap, UFW, fail2ban, Lynis)
- 🚩 Competitive ethical hacking CTFs (steganography & malware-classification tracks)

### 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=CarlosMH22&show_icons=true&theme=radical&hide_border=true" height="165"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=CarlosMH22&layout=compact&theme=radical&hide_border=true" height="165"/>
</p>
<p align="center">
  <img src="https://streak-stats.demolab.com/?user=CarlosMH22&theme=radical&hide_border=true" />
</p>

### 📫 Let's connect
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/TU_LINKEDIN)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=todoist&logoColor=white)](https://TU_PORTFOLIO_URL)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:TU_EMAIL@example.com)

---

<p align="center"><em>"Ship it local, ship it fast, ship it real."</em></p>
