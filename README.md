<h1 align="center">Aditya Prasath Ravilla</h1>
<p align="center">
  <strong>I build the systems underneath machine learning.</strong><br>
  M.S. Computer Science, University of Illinois Urbana-Champaign · Expected May 2027
</p>
<p align="center">
  <a href="https://www.linkedin.com/in/adityaprasath">LinkedIn</a>
  &nbsp;·&nbsp;
  <a href="mailto:apr11@illinois.edu">apr11@illinois.edu</a>
  &nbsp;·&nbsp;
  <a href="https://github.com/adityaCS-UIUC">GitHub</a>
</p>

I am a computer science master's student at the Siebel School of Computing and Data Science. My work sits on the path from a model to a system that is fast, measurable, and correct: GPU kernels, speculative tool-use inference, retrieval indexes, and data infrastructure.

Before UIUC I worked in AI engineering at StitchStudio and in software engineering at Cognizant, including production 5G microservices and real-time pipelines for Verizon. I am looking for software engineering and ML systems roles.

<p align="center">
  <img src="output/bonsai.gif" width="320" alt="Bonsai grown from the public history of adityaCS-UIUC" />
</p>
<p align="center">
  <sub>
    One account, one tree. Grown from this history by
    <a href="https://www.egorthinks.com/bonsai/?u=adityaCS-UIUC">git-bonsai</a>.
    <a href="output/bonsai-growth.gif">Replay the growth</a>.
  </sub>
</p>

<p align="center">
  <img src="https://gitcard-studio.creativecode.com.co/api/languages?username=adityaCS-UIUC&theme=tokyonight&locale=en" alt="Language mix on this GitHub account: Python, CUDA, Jupyter, TypeScript" />
</p>

## What I work on

- **GPU inference.** Custom CUDA kernels for transformer forward passes, including memory pipelines and KV-cache decode.
- **Speculative agent inference.** A small model decides when a long tool-use trace is ready to hand off, then another small model emits the call.
- **Retrieval.** Embedding indexes tuned on recall, latency, and memory, not on a single quality number.
- **Data systems.** Approximate nearest-neighbor search, distributed storage, and contention under skewed OLTP load.

Coursework at UIUC includes Applied Parallel Programming, Systems for GenAI, Applied Machine Learning, Cloud Computing Applications, Database Systems, and Advanced Data Management.

## Open these first

| Project | Why it is here |
| --- | --- |
| [THINKER-GPT2-Inference](https://github.com/adityaCS-UIUC/THINKER-GPT2-Inference) | CUDA forward pass for GPT-2 124M: tiled GEMM, Tensor Cores, cuBLAS, Flash Attention, KV-cache decode, and `cp.async` pipelines. |
| [PACT](https://github.com/adityaCS-UIUC/PACT) | Speculative early exit for tool-use agents. A Phi-3 speculator truncates a QwQ-32B trace, and a second Phi-3 model emits the tool call. |
| [DenseRetrievalSystem_Contriever](https://github.com/adityaCS-UIUC/DenseRetrievalSystem_Contriever) | Contriever and FAISS, tuned on Recall@k, p50/p95 latency, throughput, and memory. |

## All repositories

| Repository | What it is | Stack |
| --- | --- | --- |
| [THINKER-GPT2-Inference](https://github.com/adityaCS-UIUC/THINKER-GPT2-Inference) | CUDA forward pass for GPT-2 124M: tiled GEMM, Tensor Cores, cuBLAS, Flash Attention, KV-cache decode, and `cp.async` pipelines. ECE 408 portfolio build, based on [llm.c](https://github.com/karpathy/llm.c). | CUDA |
| [PACT](https://github.com/adityaCS-UIUC/PACT) | Speculative early exit for tool-use agents. A Phi-3 speculator truncates a QwQ-32B reasoning trace at threshold τ, and a second Phi-3 model turns that prefix into the next tool call. CS 598. | Python, PyTorch, LoRA |
| [DenseRetrievalSystem_Contriever](https://github.com/adityaCS-UIUC/DenseRetrievalSystem_Contriever) | Dense retrieval with Contriever and FAISS. Index choices are driven by Recall@k, p50/p95 latency, throughput, and memory, including sub-300ms p95 retrieval on the evaluated sets. | Python, PyTorch, FAISS |
| [LegendSpot-LegendDB-Primary](https://github.com/adityaCS-UIUC/LegendSpot-LegendDB-Primary) | Research simulation of HotSpot-LegendDB: an LSM-augmented, multi-primary RDMA OLTP design for hot-spot contention. Companion to a CS 511 proposal on write buffering and ownership consolidation. | Python |
| [CS511-MP2-HNSW-DiskANN](https://github.com/adityaCS-UIUC/CS511-MP2-HNSW-DiskANN) | HNSW and DiskANN approximate nearest-neighbor search. Construction and search grids target Recall@1 of 0.95, with combined latency curves. | Python |
| [CS511-FA25-MP1-HDFS-Spark](https://github.com/adityaCS-UIUC/CS511-FA25-MP1-HDFS-Spark) | Cluster bring-up and deployment checks for HDFS and Spark. CS 511. | Shell |
| [mp2](https://github.com/adityaCS-UIUC/mp2) | [Aditya's Cosmic Atlas](https://adityacs-uiuc.github.io/mp2/): a React app over NASA's public image archive, with search, sort, a filterable Mars rover gallery, and routed detail pages. | TypeScript, React |
| [mp1](https://github.com/adityaCS-UIUC/mp1) | Responsive landing page for Yentha AI, a product concept for AI tools and subscription management. HTML, SCSS, and JavaScript only. | HTML, SCSS, JavaScript |
| [mp0](https://github.com/adityaCS-UIUC/mp0) | CS 409 setup exercise: one HTML/CSS profile card, deployed with GitHub Pages. | HTML, CSS |
| [MP5_FullStack_Template](https://github.com/adityaCS-UIUC/MP5_FullStack_Template) | Fork of the [UIUC CS 498 Cloud](https://github.com/UIUC-CS498-Cloud/MP5_FullStack_Template) full-stack starter. Course template, not an original application. | JavaScript |

The GPT-2 repository packages an ECE 408 team project for public review. Kernel work was collaborative. My focus on that project was KV-cache attention, `cp.async` GEMM, profiling, LayerNorm and softmax, and the verification harness.

PACT is a CS 598 team project. The public repository is the local project tree.

## Stack

<p align="center">
  <img alt="CUDA" src="https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white" />
  <img alt="C++" src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white" />
  <img alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img alt="Go" src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white" />
  <img alt="Java" src="https://img.shields.io/badge/Java-437291?style=flat-square&logo=openjdk&logoColor=white" />
  <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
  <img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" />
</p>
<p align="center">
  <img alt="Linux" src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" />
  <img alt="Docker" src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
  <img alt="Kubernetes" src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white" />
  <img alt="AWS" src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=FF9900" />
  <img alt="Kafka" src="https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white" />
  <img alt="PostgreSQL" src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
  <img alt="Redis" src="https://img.shields.io/badge/Redis-FF4438?style=flat-square&logo=redis&logoColor=white" />
</p>
<p align="center">
  <img alt="Spark" src="https://img.shields.io/badge/Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white" />
  <img alt="FastAPI" src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" />
  <img alt="React" src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" />
  <img alt="Next.js" src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" />
</p>

**Languages.** C++, Python, Go, Java, TypeScript, JavaScript, SQL, Bash

**GPU and ML.** CUDA, PyTorch, LoRA, FAISS, FlashAttention, vLLM, Nsight Compute

**Systems.** Linux, Docker, Kubernetes, AWS, Kafka, PostgreSQL, Redis, gRPC, Spark, HDFS

**Interfaces.** React, Next.js, FastAPI, WebSockets

Icons from [Simple Icons](https://github.com/simple-icons/simple-icons).
