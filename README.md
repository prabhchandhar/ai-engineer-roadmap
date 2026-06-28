# AI Engineer Roadmap 🚀

> A structured 9-month, 4-book self-study plan for software engineers transitioning into AI engineering and ML — built and followed in public.

**Started:** 29 June 2026 &nbsp;|&nbsp; **Target completion:** 7 March 2027 &nbsp;|&nbsp; **Pace:** 10–12 hours/week

[![Progress](https://img.shields.io/badge/Progress-Week%201%20of%2036-8b7ef8?style=flat-square)](./progress)
[![Books](https://img.shields.io/badge/Books-4-2fd4a0?style=flat-square)](#the-four-books)
[![Portfolio Projects](https://img.shields.io/badge/Portfolio%20Projects-3-f5a623?style=flat-square)](#portfolio-projects)
[![License](https://img.shields.io/badge/License-MIT-f07050?style=flat-square)](./LICENSE)

---

## Why I Built This

I'm a software engineer. Not an ML researcher. Not a data scientist.

Just someone who builds systems for a living — and realised the entire industry is shifting under my feet.

Most "learn AI" content is designed for people who already know AI. The courses assume a PhD. The tutorials skip the parts that actually matter. The roadmaps are just lists of tools with no order, no context, no honest timeline.

So I built something different: a rigorous, week-by-week plan built around the four best technical books in the field, calibrated for a software engineer background, with real portfolio projects baked in.

This repo is where I'm doing it in public — weekly progress notes, code from exercises, and the three portfolio projects I'll build along the way.

---

## The Four Books

| # | Book | Author(s) | Weeks | Focus |
|---|------|-----------|-------|-------|
| 1 | **AI Engineering: Building Applications with Foundation Models** | Chip Huyen | 1–14 | Production LLM systems, RAG, evaluation, inference optimisation |
| 2 | **Hands-On Machine Learning with Scikit-Learn and PyTorch** *(2025 ed.)* | Aurélien Géron | 1–26 | Full ML + deep learning stack, transformers, diffusion models |
| 3 | **Designing Data-Intensive Applications** *(2nd ed.)* | Martin Kleppmann + Chris Riccomini | 13–28 | Data systems, replication, transactions, stream processing |
| 4 | **Patterns of Distributed Systems** | Unmesh Joshi | 27–36 | 29 concrete distributed systems patterns with Java implementations |

These four books cover the complete AI engineering stack:
- **Huyen** → the AI application layer (what to build and how to evaluate it)
- **Géron** → the ML and deep learning layer (how models actually work)
- **Kleppmann** → the data systems layer (what holds it all up)
- **Joshi** → the distributed implementation layer (how the pieces work internally)

---

## Study Schedule

**10.5 hours/week across 5 sessions (IST):**

| Day | Time | Duration |
|-----|------|----------|
| Monday | 8:00 PM – 9:30 PM | 1.5 hrs |
| Wednesday | 8:00 PM – 9:30 PM | 1.5 hrs |
| Friday | 8:00 PM – 9:30 PM | 1.5 hrs |
| Saturday | 9:00 AM – 12:00 PM | 3 hrs |
| Sunday | 9:00 AM – 12:00 PM | 3 hrs |

---

## 9-Month Overview

```
Month  1    2    3    4    5    6    7    8    9
Week   1----5----10---15---20---25---30---35-36

AI Engineering (Huyen)
       [====Primary=======][==Wrap-up==]

Hands-On ML (Géron)
       [====Part 1: Scikit-Learn====][====Part 2: Deep Learning + PyTorch=======]

DDIA 2nd Ed. (Kleppmann)
                          [==Foundations==][====Distributed====][=Derived=]

Patterns of Dist. Systems (Joshi)
                                              [====29 Patterns========]

Portfolio projects
       Week 6: RAG Pipeline    Week 14: Vision Model    Week 22-24: Capstone
```

---

## Week-by-Week Plan

<details>
<summary><strong>📘 Book 1 — AI Engineering (Huyen) · Weeks 1–14</strong></summary>

| Week | Chapter | Practice Task |
|------|---------|---------------|
| 1 | Ch 1 — The AI Engineering Landscape | Sign up for LLM API. Write 10 prompts manually. |
| 2 | Ch 2 — Understanding Foundation Models | Experiment with temperature + sampling params. Tokenise sentences with HuggingFace. |
| 3 | Ch 3 — Evaluation Methodology | Design an eval rubric for your Week 1 prompts. |
| 4 | Ch 4 — Evaluate AI Systems | **★ Build eval harness** — 20 test inputs, LLM-as-judge scoring. |
| 5 | Ch 5 — Prompt Engineering | Add 3 prompt variants to eval harness. Compare scores systematically. |
| 6 | Ch 6 — RAG and Agents | **★ Build RAG pipeline** — ChromaDB/FAISS + LLM. Run eval harness on it. |
| 7 | Ch 7 — Finetuning | Write personal fine-tune vs RAG vs prompt decision framework. |
| 8 | Ch 8 — Dataset Engineering | Audit RAG documents. Write data quality report. |
| 9 | Ch 9 — Inference Optimisation | Benchmark RAG pipeline: latency, tokens/sec, cost/query. |
| 10 | Ch 10 — Architecture + User Feedback | Sketch full production architecture of RAG app. |
| 11–14 | Wrap-up + buffer | Revisit gaps. Finalise RAG project. |

</details>

<details>
<summary><strong>📗 Book 2 — Hands-On ML (Géron) · Weeks 1–26</strong></summary>

**Part 1 — ML Fundamentals with Scikit-Learn (Weeks 1–9)**

| Week | Chapter | Practice Task |
|------|---------|---------------|
| 1 | Ch 1 — The ML Landscape | Set up environment. Run first notebook from `ageron/handson-mlp`. |
| 2 | Ch 2 — End-to-End ML Project | Full California housing pipeline — do every step manually first. |
| 3 | Ch 3 — Classification | MNIST binary + multiclass classifier. Observe precision-recall trade-offs. |
| 4 | Ch 4 — Training Models | Implement linear regression from scratch with NumPy before using Scikit-Learn. |
| 5 | Ch 5–6 — SVMs + Decision Trees + XGBoost | SVM on non-linear data. Visualise decision tree. |
| 6 | Ch 7 — Ensemble Learning + Random Forests | Stacking ensemble + XGBoost on housing dataset. |
| 7 | Ch 8 — Dimensionality Reduction | PCA on MNIST → 2D. Compare with t-SNE. |
| 8 | Ch 9 — Unsupervised Learning | K-Means on real dataset with elbow + silhouette score. |
| 9 | Part 1 review + exercises | **★ Portfolio Project 1** — full Scikit-Learn pipeline on Kaggle dataset. |

**Part 2 — Deep Learning + PyTorch (Weeks 10–26)**

| Week | Chapter | Practice Task |
|------|---------|---------------|
| 10 | Ch 10 — PyTorch Fundamentals | Linear regression 3 ways: NumPy → tensors+autograd → nn.Linear+Adam. |
| 11 | Ch 11 — Training Deep Neural Networks | Deep MLP on MNIST. Transfer learning to new dataset. |
| 12 | Ch 12–13 — Custom Models + HuggingFace | Write custom training loop from scratch. |
| 13 | Ch 14 — CNNs + Computer Vision | CNN on CIFAR-10. Fine-tune pretrained ResNet. |
| 14 | Ch 14 exercises | **★ Portfolio Project 2** — fine-tune pretrained model on custom image dataset. |
| 15 | Ch 15 — NLP + Transformers + HuggingFace | Fine-tune BERT for text classification end-to-end. |
| 16 | Advanced NLP + exercises | Fine-tune T5/BART for summarisation. Evaluate with ROUGE. |
| 17 | Ch 17 — Autoencoders + GANs | Train VAE on MNIST. Visualise latent space. |
| 18 | Ch 17 — Diffusion Models | HuggingFace Diffusers: generate + guide images. |
| 19 | Ch 18 — Reinforcement Learning | Train DQN agent on CartPole with Gymnasium. |
| 20 | Ch 19 — Training + Deploying at Scale | Quantise a model. Measure speedup vs accuracy trade-off. |
| 21 | Exercises + consolidation | Fill gaps. Deepdive on one shaky concept. |
| 22–24 | **★ Capstone Project** | Design → train → evaluate → deploy a full deep learning project. |
| 25 | Buffer / weak spots | Extra time on hardest chapters. |
| 26 | Retrospective | Learning retrospective. Forward plan for next 3 months. |

</details>

<details>
<summary><strong>📙 Book 3 — DDIA 2nd Ed. (Kleppmann + Riccomini) · Weeks 13–28</strong></summary>

**Part I — Foundations (Weeks 13–17)**

| Week | Chapter | Practice Task |
|------|---------|---------------|
| 13 | Ch 1 — Trade-offs in Data Systems *(new)* | Write 3 data system trade-offs from your own work experience. |
| 14 | Ch 2 — Nonfunctional Requirements *(new)* | Write 1-page NFR doc: p99 latency, failure rate, load growth, compliance. |
| 15 | Ch 3 — Data Models + Query Languages | Design same schema 3 ways: relational, document, graph. |
| 16 | Ch 4 — Storage and Retrieval | Trace a write + read through B-tree vs LSM-tree step by step. |
| 17 | Ch 5 — Encoding + Evolution | Map a past schema incident to Kleppmann's compatibility framework. |

**Part II — Distributed Data (Weeks 18–24)**

| Week | Chapter | Practice Task |
|------|---------|---------------|
| 18 | Ch 6 — Replication Part 1 | Draw replication topology of a DB you use. Label every arrow. |
| 19 | Ch 6 cont. + Ch 7 — Partitioning | Design partitioning for 100M ML training examples. |
| 20 | Ch 8 — Transactions Part 1 | Build race condition reference card — all 4 anomalies with real examples. |
| 21 | Ch 8 — Transactions Part 2 | Look up default isolation level of your main DB. Write what it means. |
| 22 | Ch 9 — The Trouble with Distributed Systems | Find a real clock-skew incident post-mortem. Map it to this framework. |
| 23 | Ch 10 — Consistency + Consensus Part 1 *(★ hardest)* | Read once. Write half-page summary without looking at the book. |
| 24 | Ch 10 — Consensus Part 2 | Watch raft.github.io. Sketch how etcd maps to what you learned. |

**Part III — Derived Data (Weeks 25–28)**

| Week | Chapter | Practice Task |
|------|---------|---------------|
| 25 | Ch 11 — Batch Processing | Map an ML training pipeline to Kleppmann's batch framework. |
| 26 | Ch 12 — Stream Processing | Design streaming pipeline for real-time ML inference. |
| 27 | Ch 13 — The Future of Data Systems | Write 1-page data architecture review of a system you know. |
| 28 | Full review + AI engineering synthesis | Build AI data architecture reference: DDIA concept per AI concern. |

</details>

<details>
<summary><strong>📕 Book 4 — Patterns of Distributed Systems (Joshi) · Weeks 27–36</strong></summary>

| Week | Patterns | Practice Task |
|------|---------|---------------|
| 27 | Ch 1–2 — Narratives + Pattern Overview | Draw pattern dependency graph from memory after Ch 2. |
| 28 | Ch 3–5 — Write-Ahead Log, Segmented Log, Low-Water Mark | Map WAL → Kafka partition log. Segmented Log → Kafka segments. |
| 29 | Ch 6–10 — Leader/Followers, HeartBeat, Majority Quorum, Generation Clock, High-Water Mark | Trace full write request through all 5 patterns as a sequence diagram. |
| 30 | Ch 11–12 — Paxos + Replicated Log | Compare Paxos vs Raft. Map Replicated Log → etcd internals. |
| 31 | Ch 13–16 — Singular Update Queue, Request Waiting List, Idempotent Receiver, Follower Reads | Design an idempotent LLM API endpoint. |
| 32 | Ch 17–20 — Versioned Value, Version Vector, Fixed Partitions, Key-Range Partitions | Compare Cassandra vs CockroachDB partitioning strategies. |
| 33 | Ch 21–24 — Two-Phase Commit, Lamport Clock, Hybrid Clock, Clock-Bound Wait | Read Spanner paper abstract. Connect to DDIA Ch 9. |
| 34 | Ch 25–29 — Consistent Core, Lease, State Watch, Gossip, Emergent Leader | Map ZooKeeper features to patterns. Then map to Kubernetes + etcd. |
| 35 | Ch 30–32 — Single-Socket Channel, Request Batch, Request Pipeline | Map Kafka producer config to all 3 patterns. |
| 36 | Final synthesis | Build the complete AI systems stack reference across all 4 books. |

</details>

---

## Portfolio Projects

### Project 1 — RAG Pipeline + Eval Harness *(Week 6–9)*
**Stack:** Python · LLM API · ChromaDB or FAISS · custom eval harness

An end-to-end retrieval-augmented generation application with a systematic evaluation framework.

- Ingests and chunks a document corpus
- Embeds and stores in a vector database
- Queries with an LLM and returns grounded answers
- Evaluates output quality using an LLM-as-judge harness across 20+ test cases

📁 [`/projects/01-rag-pipeline`](./projects/01-rag-pipeline)

---

### Project 2 — Fine-Tuned Vision Model *(Week 14)*
**Stack:** PyTorch · HuggingFace Transformers · TorchVision · Weights & Biases

A fine-tuned pretrained image classification model on a custom dataset.

- Pretrained backbone (ResNet / EfficientNet / ViT) fine-tuned on a domain-specific dataset
- Experiment tracking with W&B — loss curves, validation metrics, hyperparameter runs
- Error analysis — where the model fails and why
- Deployed to HuggingFace Spaces

📁 [`/projects/02-vision-model`](./projects/02-vision-model)

---

### Project 3 — End-to-End Capstone *(Weeks 22–24)*
**Stack:** PyTorch · HuggingFace · FastAPI or HuggingFace Spaces · chosen domain

A full deep learning project chosen based on a real problem — from raw data to deployed model.

- Problem definition and dataset curation
- Baseline model (Scikit-Learn) → deep learning model → fine-tuned pretrained model
- Systematic evaluation with domain-appropriate metrics
- Production-ready deployment with monitoring

📁 [`/projects/03-capstone`](./projects/03-capstone)

---

## How the Four Books Connect

Every major AI engineering concern has a layer in each book:

| AI Engineering Concern | Huyen (Ch) | Géron (Ch) | Kleppmann (Ch) | Joshi (Pattern) |
|------------------------|------------|------------|----------------|-----------------|
| RAG + retrieval | Ch 6 | Ch 9 (embeddings) | Ch 4 (storage) | Write-Ahead Log |
| Model serving | Ch 9–10 | Ch 19 | Ch 6 (replication) | Replicated Log |
| Inference optimisation | Ch 9 | Ch 19 | Ch 7 (partitioning) | Request Pipeline |
| Feature store | Ch 6 | Ch 12–13 | Ch 11 (batch) | Fixed Partitions |
| Real-time inference | Ch 10 | — | Ch 12 (stream) | Request Batch |
| Fine-tuning pipelines | Ch 7–8 | Ch 11–15 | Ch 11 (batch) | Segmented Log |
| Evaluation pipelines | Ch 3–4 | Ch 3 (metrics) | Ch 5 (encoding) | Idempotent Receiver |
| Schema evolution | Ch 8 | Ch 13 | Ch 5 | Versioned Value |

---

## Repository Structure

```
ai-engineer-roadmap/
│
├── README.md                          # This file
│
├── resources/
│   ├── ai_engineer_roadmap.html       # Full interactive infographic
│   ├── ai_engineer_roadmap.pdf        # Landscape PDF (6 pages, A3)
│   └── ai_engineer_roadmap_jun29.ics  # Google Calendar / Outlook import file
│
├── progress/
│   ├── week-01.md                     # Week 1 notes
│   ├── week-02.md                     # Week 2 notes
│   └── ...                            # Updated every week
│
├── notes/
│   ├── ai-engineering-huyen/          # Chapter notes — Huyen
│   ├── hands-on-ml-geron/             # Chapter notes — Géron
│   ├── ddia-kleppmann/                # Chapter notes — DDIA
│   └── patterns-joshi/                # Pattern summaries — Joshi
│
└── projects/
    ├── 01-rag-pipeline/               # Project 1
    ├── 02-vision-model/               # Project 2
    └── 03-capstone/                   # Project 3
```

---

## Weekly Progress Log

| Week | Dates | Books | Status | Notes |
|------|-------|-------|--------|-------|
| 1 | 29 Jun – 5 Jul 2026 | Huyen Ch 1 · Géron Ch 1 | 🟡 In progress | |
| 2 | 6 – 12 Jul 2026 | Huyen Ch 2 · Géron Ch 2 | ⬜ Not started | |
| 3 | 13 – 19 Jul 2026 | Huyen Ch 3 · Géron Ch 3 | ⬜ Not started | |
| 4 | 20 – 26 Jul 2026 | Huyen Ch 4 · Géron Ch 4 | ⬜ Not started | |
| 5 | 27 Jul – 2 Aug 2026 | Huyen Ch 5 · Géron Ch 5–6 | ⬜ Not started | |
| 6 | 3 – 9 Aug 2026 | Huyen Ch 6 · Géron Ch 7 | ⬜ Not started | |
| 7 | 10 – 16 Aug 2026 | Huyen Ch 7 · Géron Ch 8 | ⬜ Not started | |
| 8 | 17 – 23 Aug 2026 | Huyen Ch 8 · Géron Ch 9 | ⬜ Not started | |
| 9 | 24 – 30 Aug 2026 | Huyen Ch 9 · Géron Project 1 | ⬜ Not started | |
| 10 | 31 Aug – 6 Sep 2026 | Huyen Ch 10 · Géron Ch 10 | ⬜ Not started | |
| 11 | 7 – 13 Sep 2026 | Géron Ch 11 | ⬜ Not started | |
| 12 | 14 – 20 Sep 2026 | Géron Ch 12–13 | ⬜ Not started | |
| 13 | 21 – 27 Sep 2026 | Géron Ch 14 · DDIA Ch 1 | ⬜ Not started | |
| 14 | 28 Sep – 4 Oct 2026 | Géron Project 2 · DDIA Ch 2 | ⬜ Not started | |
| 15 | 5 – 11 Oct 2026 | Géron Ch 15 · DDIA Ch 3 | ⬜ Not started | |
| 16 | 12 – 18 Oct 2026 | Géron NLP · DDIA Ch 4 | ⬜ Not started | |
| 17 | 19 – 25 Oct 2026 | Géron Ch 17a · DDIA Ch 5 | ⬜ Not started | |
| 18 | 26 Oct – 1 Nov 2026 | Géron Ch 17b · DDIA Ch 6 | ⬜ Not started | |
| 19 | 2 – 8 Nov 2026 | Géron Ch 18 · DDIA Ch 6–7 | ⬜ Not started | |
| 20 | 9 – 15 Nov 2026 | Géron Ch 19 · DDIA Ch 8a | ⬜ Not started | |
| 21 | 16 – 22 Nov 2026 | Géron review · DDIA Ch 8b | ⬜ Not started | |
| 22 | 23 – 29 Nov 2026 | Géron Capstone Wk 1 · DDIA Ch 9 | ⬜ Not started | |
| 23 | 30 Nov – 6 Dec 2026 | Géron Capstone Wk 2 · DDIA Ch 10a | ⬜ Not started | |
| 24 | 7 – 13 Dec 2026 | Géron Capstone Wk 3 · DDIA Ch 10b | ⬜ Not started | |
| 25 | 14 – 20 Dec 2026 | Géron buffer · DDIA Ch 11 | ⬜ Not started | |
| 26 | 21 – 27 Dec 2026 | Géron retro · DDIA Ch 12 | ⬜ Not started | |
| 27 | 28 Dec – 3 Jan 2027 | DDIA Ch 13 · Joshi Ch 1–2 | ⬜ Not started | |
| 28 | 4 – 10 Jan 2027 | DDIA synthesis · Joshi Ch 3–5 | ⬜ Not started | |
| 29 | 11 – 17 Jan 2027 | Joshi Ch 6–10 | ⬜ Not started | |
| 30 | 18 – 24 Jan 2027 | Joshi Ch 11–12 | ⬜ Not started | |
| 31 | 25 – 31 Jan 2027 | Joshi Ch 13–16 | ⬜ Not started | |
| 32 | 1 – 7 Feb 2027 | Joshi Ch 17–20 | ⬜ Not started | |
| 33 | 8 – 14 Feb 2027 | Joshi Ch 21–24 | ⬜ Not started | |
| 34 | 15 – 21 Feb 2027 | Joshi Ch 25–29 | ⬜ Not started | |
| 35 | 22 – 28 Feb 2027 | Joshi Ch 30–32 | ⬜ Not started | |
| 36 | 1 – 7 Mar 2027 | Final synthesis — all 4 books | ⬜ Not started | |

---

## Who Can Follow This

This roadmap is designed for:

- **Software engineers** who want to transition into AI/ML roles
- **CS students** who want to stand out when they graduate
- **Backend or fullstack developers** seeing "AI experience required" in every job description
- **Career changers** with coding skills who want to enter the field properly

**You don't need:**
- A PhD or research background
- A statistics or data science degree
- Prior ML experience

**You do need:**
- Solid programming fundamentals (any language)
- 10–12 hours per week of consistent study time
- Willingness to code along, not just read

**Realistic expectations:**

By Week 6 you will have built a working RAG pipeline. By Week 9 you will have your first ML portfolio project on GitHub. By Week 14 you will have fine-tuned a deep learning model. By Week 36 you will not be a 10-year ML veteran — but you will be able to design a production AI system end-to-end, reason about the data infrastructure underneath it, and have a portfolio that demonstrates you can build, not just talk.

---

## Resources in This Repo

| File | Description |
|------|-------------|
| [`resources/ai_engineer_roadmap.html`](./resources/ai_engineer_roadmap.html) | Full interactive roadmap infographic — open in browser |
| [`resources/ai_engineer_roadmap.pdf`](./resources/ai_engineer_roadmap.pdf) | 6-page landscape PDF — print or share |
| [`resources/ai_engineer_roadmap_jun29.ics`](./resources/ai_engineer_roadmap_jun29.ics) | Calendar file — import into Google Calendar or Outlook (216 events, 29 Jun 2026 – 7 Mar 2027) |

---

## Following Along

I'm sharing weekly updates as I go — what I'm learning, what's hard, and what's actually useful.

- 🔔 **Watch this repo** to get notified when weekly progress notes are added
- ⭐ **Star it** if this is useful to you
- 🍴 **Fork it** if you want to follow the same plan — update the progress table with your own dates

If you're following this plan too, feel free to open an issue or a discussion. Happy to compare notes.

---

## Books Referenced

- Huyen, Chip. *AI Engineering: Building Applications with Foundation Models*. O'Reilly, 2025.
- Géron, Aurélien. *Hands-On Machine Learning with Scikit-Learn and PyTorch*. O'Reilly, 2025.
- Kleppmann, Martin and Chris Riccomini. *Designing Data-Intensive Applications*, 2nd ed. O'Reilly, 2026.
- Joshi, Unmesh. *Patterns of Distributed Systems*. Addison-Wesley, 2023.

---

## License

MIT — feel free to use, adapt, and share this roadmap.

---

*Built by [Prabhjot Singh Chandhar](https://github.com/prabhchandhar) · Started 29 June 2026*
 
