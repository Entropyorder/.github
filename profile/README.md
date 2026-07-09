# Entropyorder

**Post-training data infrastructure for frontier model labs.**

Entropyorder (熵基秩序) supplies high-quality RL / SFT / Eval data to base-model post-training labs. We exist to solve the bottleneck that defines the capability race: expert-grade training signal is scarce, expensive to produce, and too slow to keep pace with rapid base-model iteration.

## The shift

For years, post-training data meant PhD-level experts annotating by hand — high cost, capped throughput, slow turnaround. That model has hit its ceiling. Frontier models, multi-agent frameworks, tool calling, code-execution environments, VLMs, multimodal tooling, and automatic verifiers are now mature enough to automate expert-grade data production. We turn that opportunity into infrastructure.

## Light Infra, Heavy Harness

We don't build a bloated unified platform. Base-model data needs are highly variable, formats are fragmented, and model weaknesses migrate every training round — a fixed platform cannot absorb this market.

What we build instead is a **data-production Harness**: a layer that assembles models, tools, knowledge sources, expert roles, verification rules, and delivery formats on demand, then runs task understanding, sample generation, quality verification, batch delivery, and feedback iteration at speed.

## Expert-in-the-loop

Expert knowledge — distilled into Agent Orchestrators — acts as task designer, domain-knowledge provider, quality calibrator, and boundary judge. The Harness handles candidate generation, scaling, formatting, tool verification, trajectory logging, and first-pass QC. Expert credibility is preserved; the human-throughput, cost, and latency bottlenecks of traditional annotation are broken. A single OPC super-individual now covers the full pipeline that used to require a cross-functional team.

## Architecture

![Entropyorder Data Harness Architecture](assets/architecture.png)

## Four production Harnesses

Our repos are not demos — each is a working piece of one of the four production pipelines below. Together they trace the loop from raw asset to verifiable training signal.

### 1 · Multi-agent synthesis Harness

Science reasoning, math, AI for Science, complex QA, PhD-level eval. Drives HLE, SFE, hard-math, MicroVQA, MSEarth, SciCode-style products.

- [Math-Forge](https://github.com/Entropyorder/Math-Forge) & [MathForge_Mulitimodal](https://github.com/Entropyorder/MathForge_Mulitimodal) — hard-math problem generation, including multimodal variants
- [Stem-Video-QA-Studio](https://github.com/Entropyorder/Stem-Video-QA-Studio) — STEM video reasoning data studio
- [Paper-QA-Expert](https://github.com/Entropyorder/Paper-QA-Expert) · [Paper_QA_CLI](https://github.com/Entropyorder/Paper_QA_CLI) · [Paper-Filter](https://github.com/Entropyorder/Paper-Filter) — AI-for-Science paper search, filter, and expert QA pipeline

### 2 · Long-document extraction & matching Harness

Textbooks, PDFs, scans, long knowledge assets → structured QA, knowledge points, image problems, solutions, training samples.

- [Book-QA-Extract](https://github.com/Entropyorder/Book-QA-Extract) — textbook / long-document → structured QA extraction
- [pdf-exercise-crawler](https://github.com/Entropyorder/pdf-exercise-crawler) — PDF exercise crawling, async download, AI subject classification

### 3 · Agent synthesis, eval & toolchain Harness

Tool-use trajectories and long-horizon tasks for Agent SFT / RL — OpenClaw, AgentOS, SkillBench-shaped data.

- [Trajectory-Orchestrator](https://github.com/Entropyorder/Trajectory-Orchestrator) — tool-use trajectory generation toolkit
- [Openclaw-Syn](https://github.com/Entropyorder/Openclaw-Syn) — OpenClaw trajectory synthesis
- [Skills-QA-Expert](https://github.com/Entropyorder/Skills-QA-Expert) — SkillBench-style skill / tool evaluation data
- [MultiModels-Sample-Script](https://github.com/Entropyorder/MultiModels-Sample-Script) — multi-model candidate sampling for the generation stage

### 4 · Cross-modal alignment Harness

Video / audio / image / text understanding & alignment — streaming video response, fine-grained AV alignment, camera-movement data, art appreciation.

- [Worldengine-Data-Collector](https://github.com/Entropyorder/Worldengine-Data-Collector) — frame-aligned video + telemetry pipeline (camera-movement / kinematics data)
- [Mirror-Disdirection-QA](https://github.com/Entropyorder/Mirror-Disdirection-QA) — mirror / contour perception eval data
- [Art-Wiki-Expert](https://github.com/Entropyorder/Art-Wiki-Expert) — art appreciation expert data
- [Omni-Studio](https://github.com/Entropyorder/Omni-Studio) — multimodal alignment studio
- [Social-World-Model](https://github.com/Entropyorder/Social-World-Model) — social-scene world model data

## Information retrieval

Open-ended, long-chain real-world retrieval challenges.

- [Search-Align-Studio](https://github.com/Entropyorder/Search-Align-Studio) — long-chain retrieval & search-alignment data

## The signal that matters

The valuable part of post-training data isn't random volume — it's high-density, verifiable, correctable training signal aimed at a model's *marginal capability zone*. A sample that almost succeeds but fails at a key step is worth more than thousands of ordinary ones.

Our loop isn't "collect → label → QA → deliver." It's:

```
Seed Mining → Task Design → Candidate Generation → Tool/Model Verification
→ Expert Calibration → Dataset Packaging → Customer Feedback → Boundary Mining
```

Every eval round, every post-training failure mode becomes input for the next data cycle. The faster it spins, the deeper our grasp of model capability boundaries — and the closer our data lands to real post-training demand.

## Vision

Ordinary data will only get less scarce. What stays scarce is the ability to construct tasks, environments, trajectories, verifiers, and corrective feedback. The future of AI data converges on simulation + environment + data: a sample is no longer just a record, but a task environment, tool calls, execution traces, error feedback, and reward signal.

Entropyorder uses data as the entry point — connecting expert organization, AI Harness, and customer model feedback — to keep producing the post-training fuel that drives models toward self-evolution, and ultimately AGI.

---

> Self-evolved AI for AGI.
