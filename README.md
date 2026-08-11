# Rohan — AI Engineer
Building production-oriented AI systems across Machine Learning, Computer Vision, Generative AI, and AI backend engineering.
**Machine Learning · Computer Vision · Generative AI · MLOps · AI Systems**
<!-- TODO: Add portfolio URL once deployed --> <!-- [![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=flat&logo=vercel&logoColor=white)](YOUR_PORTFOLIO_URL) --> <!-- TODO: Add LinkedIn profile URL --> <!-- [![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](YOUR_LINKEDIN_URL) --> [![Email](https://img.shields.io/badge/Email-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:rohanprajapati7970@gmail.com) [![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/rohanxlabs)
---
## About
I build end-to-end AI systems — from training pipelines and computer vision backends to agentic applications and self-healing MLOps platforms. My work combines ML engineering with software engineering: clean architecture, real test coverage, and systems that behave predictably under real conditions.
Currently focused on multi-model AI pipelines, agentic systems with tool use, production CV with pose estimation, and autonomous MLOps.
---
## What I Build
| Area | Focus | |---|---| | **AI Products** | Full-stack applications powered by LLMs, vision pipelines, RAG, and agentic loops | | **Agentic AI** | Multi-agent systems with planning, tool use, memory, and iterative refinement | | **Computer Vision** | Pose estimation, object detection, multi-person tracking, temporal analysis | | **MLOps** | Drift detection, auto-retraining, experiment tracking, CI/CD for ML | | **AI Backend** | FastAPI and Express services for ML inference, structured AI output, and data pipelines |
---
## Featured Projects
### 🌾 FarmLens AI Full-stack crop disease diagnostic tool for smallholder farmers. A user photographs a crop leaf — the system runs a structured-output vision pipeline through a multi-model fallback chain (paid → gemma-4-26b → gemma-4-31b → nemotron-nano), applies a domain-specific safety filter against 29 banned/restricted pesticide ingredients, augments the diagnosis with retrieved treatment literature via pgvector RAG, and returns a confidence-calibrated result. An agentic chat interface (Groq tool-calling, max 3 iterations) provides access to field health data, weather forecasts, and the same knowledge base through four validated tools. A deterministic rule engine generates an AI Insights feed, with LLM narration grounded strictly in measured values.
`React 18` `Express` `TypeScript` `Groq` `OpenRouter` `pgvector` `PostgreSQL` `JWT` `Pino` · 199 server tests · eval harness with published accuracy results
[→ Repository](https://github.com/rohanxlabs/farmlens-ai) <!-- TODO: Add live deployment URL once available --> <!-- [→ Live](YOUR_FARMLENS_DEPLOYMENT_URL) -->
---
### ⚙️ Sentinel ML Self-healing MLOps platform for credit card fraud detection. When data drift or model degradation is detected, an autonomous SRE Agent triggers retraining, evaluates the new model against quality thresholds, promotes it to Production in MLflow, hot-reloads the serving layer without downtime, and generates a Claude-powered natural language incident report — without human intervention.
`FastAPI` `MLflow` `Evidently AI` `Anthropic Claude API` `Prometheus` `Streamlit` `scikit-learn` `Docker`
[→ Repository](https://github.com/rohanxlabs/sentinel-ml) · [→ Live](https://sentinel-ml-ov0d.onrender.com)
---
### 📚 LearnPath AI Personalised AI study agent that turns a single learning goal into a structured multi-phase curriculum. Generates roadmaps via Groq Llama 3.3 70B with SSE streaming, a quality gate (score ≥ 60/100), and corrective retry before persistence. Lesson content is lazily generated on first access and permanently cached in PostgreSQL. Includes an AI Mentor with conversation history and prompt injection neutralisation, XP/streak/quiz tracking, and a fallback curriculum for provider outages.
`React 19` `Express` `TypeScript` `Groq` `Supabase Auth` `Drizzle ORM` `PostgreSQL` `Upstash Redis` · CI/CD via GitHub Actions · deployed on Render
[→ Repository](https://github.com/rohanxlabs/LearnPath-AI-v3) <!-- TODO: Add live deployment URL once available --> <!-- [→ Live](YOUR_LEARNPATH_DEPLOYMENT_URL) -->
---
### 🤖 Agentic AI System Multi-agent autonomous system that decomposes a user goal into executable steps, acts using verified tools (calculator, DuckDuckGo web search), and critiques its own outputs before deciding to continue or stop. Built around a Manager → Planner → Executor → Critic loop with Groq function-calling, short-term ring-buffer memory, and persistent long-term memory with semantic search via sentence-transformers.
`Python` `Groq` `LLM Function Calling` `sentence-transformers` `FastAPI` · 122 passing tests
[→ Repository](https://github.com/rohanxlabs/Agentic-AI-system) <!-- TODO: Add live deployment URL once available --> <!-- [→ Live](YOUR_AGENTIC_DEPLOYMENT_URL) -->
---
### 🦾 PoseGuard Computer vision pipeline for biomechanical risk-signal detection from sports video. Combines YOLOv8-Pose keypoint detection, IoU-based multi-person tracking, temporal motion smoothing, joint angle and limb asymmetry analysis, and a configurable rule-based risk classifier (8 thresholds, HIGH / MEDIUM / LOW scoring). Outputs annotated video and JSON/CSV event logs.
*Risk signals are heuristic outputs from configurable thresholds — not clinically validated and not intended for medical use.*
`YOLOv8-Pose` `OpenCV` `Python` `IoU Tracker` `Temporal Analysis`
[→ Repository](https://github.com/rohanxlabs/PoseGuard) <!-- TODO: Add live deployment URL once available --> <!-- [→ Live](YOUR_POSEGUARD_DEPLOYMENT_URL) -->
---
### 👁️ PerceptAgent Perception-to-memory-to-action pipeline for live video monitoring. YOLOv8 detection with ByteTrack IDs feeds a compact scene state (ENTER/EXIT events), an in-process episodic memory store, and a Groq function-calling agent loop that selects validated tools whose results feed the next decision cycle. Five tools implemented: log_event, trigger_alert, query_object_history, annotate_frame, and a safe simulated actuator adapter.
`YOLOv8` `ByteTrack` `Groq` `Python` `Streamlit`
[→ Repository](https://github.com/rohanxlabs/PercerptAgent) <!-- TODO: Add live deployment URL once available --> <!-- [→ Live](YOUR_PERCEPTAGENT_DEPLOYMENT_URL) -->
---
### 🔁 MLOps Complete ML Pipeline End-to-end MLOps pipeline for SMS spam detection — raw data to deployed REST API. DVC tracks the full pipeline (ingestion → validation → preprocessing → training → evaluation). MLflow logs experiments. A MultinomialNB + TF-IDF model is served via FastAPI and deployed on Render. GitHub Actions runs lint + pipeline + tests on every push.
`Python` `DVC` `MLflow` `FastAPI` `scikit-learn` `Docker` `GitHub Actions` · live deploy on Render
[→ Repository](https://github.com/rohanxlabs/mlops-complete-ml-pipeline) · [→ Live](https://mlops-complete-ml-pipeline.onrender.com)
---
## Also in the Portfolio
| Project | What it is | |---|---| | [churn-ml-system](https://github.com/rohanxlabs/churn-ml-system) | End-to-end churn prediction — scikit-learn pipeline + FastAPI inference API. ROC-AUC 0.84 on held-out test set. | | [Recommendation-system](https://github.com/rohanxlabs/Recommendation-system) | SVD matrix factorization recommendation engine with FastAPI. Precision@K, Recall@K, NDCG@K evaluation. 45 tests. | | [rag-based-qa-system](https://github.com/rohanxlabs/rag-based-qa-system) | RAG pipeline — document ingestion, FAISS vector search, LLM generation, FastAPI serving. | | [AI-Video-Generator](https://github.com/rohanxlabs/AI-Video-Generator) | Multimodal generative pipeline: LLM script → SDXL image synthesis → TTS → video composition via MoviePy. | | [6-DOF-Robotic-Arm-MuJoCo](https://github.com/rohanxlabs/6-DOF-Robotic-Arm-MuJoCo-) | 6-DOF robotic arm simulation in MuJoCo with motion planning and kinematics. |
---
## Technical Stack
**Languages** Python · TypeScript · JavaScript
**ML / AI** PyTorch · scikit-learn · YOLOv8 · OpenCV · sentence-transformers
**Generative AI** Groq · OpenRouter · LLM function-calling · RAG · pgvector · Anthropic Claude API
**Backend** FastAPI · Express · Node.js · Pydantic · Zod · JWT · Supabase Auth
**Data / Databases** PostgreSQL · pgvector · Drizzle ORM · DVC · MLflow
**MLOps / Infrastructure** Evidently AI · Prometheus · Docker · GitHub Actions · Render · Vercel · Upstash Redis
---
## Engineering Approach
``` Problem → Design → Implementation → Evaluation → Deployment ```
- Solve real problems with systems that behave predictably - Architecture decisions made explicitly and documented (see FarmLens AI / LearnPath AI engineering decision logs) - Real test coverage over mocked assertions - Reproducible ML workflows (DVC, MLflow, eval harnesses) - Safety constraints built in, not added after — domain filters, input validation, prompt injection neutralisation
---
## Current Focus
Building and refining production-oriented AI systems with a focus on: - Multi-model and multi-agent architectures - Computer Vision with temporal reasoning - Autonomous MLOps and self-healing systems - Full-stack AI products with real users in mind
---
## Connect
<!-- TODO: Uncomment and update these links once available --> <!-- - Portfolio: [YOUR_PORTFOLIO_URL](YOUR_PORTFOLIO_URL) --> <!-- - LinkedIn: [linkedin.com/in/YOUR_LINKEDIN](https://linkedin.com/in/YOUR_LINKEDIN) --> - Email: [rohanprajapati7970@gmail.com](mailto:rohanprajapati7970@gmail.com) - GitHub: [github.com/rohanxlabs](https://github.com/rohanxlabs)
---
<p align="center">   <img src="https://github-readme-stats.vercel.app/api?username=rohanxlabs&show_icons=true&theme=github_dark&hide_border=true&hide=stars&count_private=true" height="150"/>   <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=rohanxlabs&layout=compact&theme=github_dark&hide_border=true&langs_count=6" height="150"/> </p>
<!-- 🐍 SNAKE -->🐍 Contribution Graph

<p align="center">
  <img src="https://github.com/rohanxlabs/rohanxlabs/blob/output/github-contribution-grid-snake.svg" />
</p>---

<!-- 🌐 CONNECT -->🌐 Connect

<p align="center">
  <a href="https://github.com/rohanxlabs">
    <img src="https://skillicons.dev/icons?i=github" height="40"/>
  </a>
  <a href="https://linkedin.com/in/YOUR_LINKEDIN">
    <img src="https://skillicons.dev/icons?i=linkedin" height="40"/>
  </a>
  <a href="https://instagram.com/YOUR_INSTAGRAM">
    <img src="https://skillicons.dev/icons?i=instagram" height="40"/>
  </a>
</p>---

<!-- ⚡ CLOSING -->⚡ Philosophy

«"Execution beats knowledge. Systems beat ideas."»

---

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=rohanxlabs&label=Profile%20Views&color=0e75b6&style=flat" />
</p>

![snake gif](https://github.com/rohanxlabs/rohanxlabs/blob/output/github-snake-dark.svg)
