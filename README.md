```
╔═══════════════════════════════════════════════════════════════╗
║  dhruv · AI engineer · security researcher                   ║
║  2nd year ISE @ NIE Mysore (2024–2028)                       ║
╚═══════════════════════════════════════════════════════════════╝
```

> building multi-agent systems, LLM infra, and multimodal deep learning  
> from a non-tier-1 college — because geography shouldn't cap ambition.

---

## ⬡ projects

### [AVRA — Agentic Vulnerability Research Assistant](https://github.com/Dhruv/avra) `WIP`
5-node LangGraph pipeline for automated code vulnerability analysis. Integrates Semgrep + Bandit for static analysis, Groq (`llama-3.3-70b`) for reasoning, and surfaces findings through a React dashboard + FastAPI backend.

`LangGraph` `FastAPI` `Groq` `Semgrep` `Bandit` `React` `Python`

---

### [ARIA — Multi-Agent Research Intelligence](https://github.com/Dhruv/aria) `live`
8-agent orchestration system with adversarial critique loops — Devil's Advocate triggers Analyst revision when weak claims exceed 30%. Full pipeline observability via `agent_logs` table (every agent's I/O + duration in ms). Parallel report generation in 3 formats.

`FastAPI` `Uvicorn` `asyncio` `Groq` `SQLite` `SSE` `Python`

---

### [Deepfake Detector — Multimodal Forensics](https://github.com/Dhruv/deepfake-detector) `in progress`
Cross-attention fusion classifier over three modalities: EfficientNet-B4 + SRM noise filters (image), LFCC/LCNN (audio), R3D-18 3D CNN (video). 512-dim embeddings per modality → single fake probability. `fake_weight=2.0` asymmetric loss because false negatives cost more. Grad-CAM heatmaps + ONNX export.

`PyTorch` `EfficientNet-B4` `MTCNN` `Gradio` `ONNX` `FastAPI`

---

### [StudyAI — Context-Aware Study Assistant](https://github.com/Dhruv/studyai) `live`
PDF-to-chat pipeline with SSE streaming, flashcard generation, multi-model selector (Llama 3.3-70b, Mixtral, Gemma). Auto-upgrades SQLite→PostgreSQL via `DATABASE_URL` — the scalability answer is in the architecture.

`Flask` `Groq` `PyPDF2` `SQLite` `Waitress` `SSE` `marked.js`

---

## ⬡ stack

| domain | tools |
|---|---|
| **AI / ML** | PyTorch · LangGraph · Groq · EfficientNet · ONNX · Grad-CAM |
| **backend** | FastAPI · Flask · asyncio · SSE · SQLite · PostgreSQL |
| **security** | Semgrep · Bandit · Burp Suite · subfinder · httpx · gau |
| **frontend / infra** | React · Gradio · Render · Docker |

---

## ⬡ security research

**Circle Bug Bounty Program — Report #3667751**  
Identified missing per-vote signature verification in the Malachite consensus protocol (`liveness.rs` — `on_round_certificate` vs `on_vote()` path). CWE-390. Severity conditional on host implementation quality.

Passive recon workflow: `subfinder → httpx → gau → waybackurls → Burp Suite`

---

## ⬡ reach me

[![HackerOne](https://img.shields.io/badge/HackerOne-grey?style=flat&logo=hackerone)](https://hackerone.com/toji_2712)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin)](https://www.linkedin.com/in/connectwdhruv/)
[![Instagram](https://img.shields.io/badge/Instagram-grey?style=flat&logo=instagram)](https://www.instagram.com/adonisdhruv/)


---

<sub>NIE Mysore · ISE · Batch 2024–2028 
