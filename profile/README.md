# ⚛️ Entropyorder

**Post-training data infrastructure for frontier model labs.**

We feed high-quality RL / SFT / Eval data to base-model post-training labs. The bottleneck in the capability race isn't compute — it's expert-grade training signal: scarce, expensive, and too slow to keep up with rapid base-model iteration. We exist to fix that.

## 🔄 The shift

For years, post-training data meant PhD experts annotating by hand — costly, capped, slow. That model has hit its ceiling. Frontier models, multi-agent frameworks, tool calling, code-execution environments, VLMs, multimodal tooling, and automatic verifiers are now mature enough to automate expert-grade data production. We turn that opportunity into infrastructure.

## 🪶 Light Infra, Heavy Harness

We don't build a bloated unified platform. Base-model data needs are highly variable, formats are fragmented, and model weaknesses migrate every training round — a fixed platform can't absorb this market.

What we build instead is a **data-production Harness**: a layer that assembles models, tools, knowledge sources, expert roles, verification rules, and delivery formats on demand — then runs task understanding, sample generation, quality verification, batch delivery, and feedback iteration at speed.

## 🧑‍🔬 Expert-in-the-loop

Expert knowledge — distilled into Agent Orchestrators — acts as task designer, domain-knowledge provider, quality calibrator, and boundary judge. The Harness handles candidate generation, scaling, formatting, tool verification, trajectory logging, and first-pass QC. Expert credibility is preserved; the human-throughput, cost, and latency bottlenecks of traditional annotation are broken. A single OPC super-individual now covers the full pipeline that used to need a cross-functional team.

## 🏗️ Architecture

![Entropyorder Data Harness Architecture](assets/architecture.png)

## 🧱 Four production Harnesses

Our repos aren't demos — each is a working piece of one of the pipelines below. Together they trace the loop from raw asset to verifiable training signal.

### 1️⃣ Multi-agent synthesis
Science reasoning, math, AI for Science, complex QA, PhD-level eval — drives HLE, SFE, hard-math, MicroVQA, MSEarth, SciCode-style products.

- [Math-Forge](https://github.com/Entropyorder/Math-Forge) & [MathForge_Mulitimodal](https://github.com/Entropyorder/MathForge_Mulitimodal) — hard-math generation, incl. multimodal variants
- [Stem-Video-QA-Studio](https://github.com/Entropyorder/Stem-Video-QA-Studio) — STEM video reasoning
- [Paper-QA-Expert](https://github.com/Entropyorder/Paper-QA-Expert) · [Paper_QA_CLI](https://github.com/Entropyorder/Paper_QA_CLI) · [Paper-Filter](https://github.com/Entropyorder/Paper-Filter) — AI-for-Science paper search, filter & expert QA

### 2️⃣ Long-document extraction & matching
Textbooks, PDFs, scans, long knowledge assets → structured QA, knowledge points, image problems, solutions, training samples.

- [Book-QA-Extract](https://github.com/Entropyorder/Book-QA-Extract) — textbook / long-doc → structured QA
- [pdf-exercise-crawler](https://github.com/Entropyorder/pdf-exercise-crawler) — PDF exercise crawling + AI subject classification

### 3️⃣ Agent synthesis, eval & toolchain
Tool-use trajectories and long-horizon tasks for Agent SFT / RL — OpenClaw, AgentOS, SkillBench-shaped data.

- [Trajectory-Orchestrator](https://github.com/Entropyorder/Trajectory-Orchestrator) — tool-use trajectory generation toolkit
- [Openclaw-Syn](https://github.com/Entropyorder/Openclaw-Syn) — OpenClaw trajectory synthesis
- [Skills-QA-Expert](https://github.com/Entropyorder/Skills-QA-Expert) — SkillBench-style skill / tool eval
- [MultiModels-Sample-Script](https://github.com/Entropyorder/MultiModels-Sample-Script) — multi-model candidate sampling for generation

### 4️⃣ Cross-modal alignment
Video / audio / image / text understanding & alignment — streaming video response, fine-grained AV alignment, camera-movement data, art appreciation.

- [Worldengine-Data-Collector](https://github.com/Entropyorder/Worldengine-Data-Collector) — frame-aligned video + telemetry (camera-movement / kinematics)
- [Mirror-Disdirection-QA](https://github.com/Entropyorder/Mirror-Disdirection-QA) — mirror / contour perception eval
- [Art-Wiki-Expert](https://github.com/Entropyorder/Art-Wiki-Expert) — art appreciation expert data
- [Omni-Studio](https://github.com/Entropyorder/Omni-Studio) — multimodal alignment studio
- [Social-World-Model](https://github.com/Entropyorder/Social-World-Model) — social-scene world model data

### 🔎 Information retrieval
Open-ended, long-chain real-world retrieval challenges.

- [Search-Align-Studio](https://github.com/Entropyorder/Search-Align-Studio) — long-chain retrieval & search-alignment data

## 🎯 The signal that matters

The valuable part of post-training data isn't random volume — it's high-density, verifiable, correctable training signal aimed at a model's *marginal capability zone*. A sample that almost succeeds but fails at a key step is worth more than thousands of ordinary ones.

Our loop isn't "collect → label → QA → deliver":

```
Seed Mining → Task Design → Candidate Generation → Tool/Model Verification
→ Expert Calibration → Dataset Packaging → Customer Feedback → Boundary Mining
```

Every eval round, every post-training failure mode becomes input for the next cycle. The faster it spins, the deeper our grasp of model capability boundaries — and the closer our data lands to real post-training demand.

## 🚀 Vision

Ordinary data will only get less scarce. What stays scarce is the ability to construct tasks, environments, trajectories, verifiers, and corrective feedback. The future of AI data converges on simulation + environment + data: a sample is no longer just a record, but a task environment, tool calls, execution traces, error feedback, and reward signal.

Entropyorder uses data as the entry point — connecting expert organization, AI Harness, and customer model feedback — to keep producing the post-training fuel that drives models toward self-evolution, and ultimately AGI.

---

> 🧬 Self-evolved AI for AGI.
