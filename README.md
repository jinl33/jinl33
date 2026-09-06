# Jinho Lee

Machine Learning Engineer & Computational Scientist | 3D Perception, Generative Modeling & Complex Networks

I build systems that learn structured representations from high-dimensional data, volumetric biological imaging, sensor streams, and single-cell genomics. I care as much about whether a model's evaluation holds up under distribution shifts as I do about the architecture itself.

**Currently:** Pretraining 3D generative diffusion foundation models across 300,000+ multimodal volumes, solving hardware VRAM limits via an 8x invertible wavelet transform, and distilling backbones by 11.6x with zero measured accuracy degradation.

[LinkedIn](https://linkedin.com/in/jin-lee-l804) · [Email](mailto:jinhlee@umich.edu)

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/-PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![C++](https://img.shields.io/badge/-C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white)
![PyTorch Geometric](https://img.shields.io/badge/-PyTorch%20Geometric-3C2179?style=flat-square)
![CUDA](https://img.shields.io/badge/-CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Nextflow](https://img.shields.io/badge/-Nextflow-000000?style=flat-square)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)

---

## At a Glance

| Metric / Scale | Context & Implementation |
| :--- | :--- |
| **8x memory reduction** | Invertible 3D wavelet-domain compression for volumetric diffusion; lossless spatial recovery |
| **11.6x model distillation** | Self-supervised knowledge distillation ($232\text{M} \to 20\text{M}$ parameters) with zero downstream accuracy loss |
| **300,000+ volumes** | Multimodal clinical volumes (T1w, T2w, DWI, FLAIR) processed in distributed SLURM HPC pipelines |
| **< 0.8 px mean error** | Sub-pixel camera-LiDAR extrinsic calibration optimization with robust Huber loss outlier rejection |
| **207k nuclei, 28 donors** | Containerized Nextflow pipeline for Parkinson's disease single-nucleus and spatial transcriptomics |
| **1,337 protein nodes** | Affinity-weighted graph attention network for single-cell signaling perturbation modeling |

---

## Featured Repositories

**[tensor-kernel-engine](https://github.com/jinl33/tensor-kernel-engine)** — High-performance fused GPU kernels implemented in OpenAI Triton alongside a zero-overhead C++17 inference runtime. Fuses edge-affinity attention with FlashAttention-style online softmax directly in SRAM registers, eliminating $O(N^2)$ global memory round-trips and moving memory-bandwidth-bound operations toward hardware compute ceilings. Includes a full Roofline analysis suite and a native LibTorch C++ driver.

**[Cell-to-Cell-Communication](https://github.com/jinl33/Cell-to-Cell-Communication)** — Interpretable affinity-weighted Graph Attention Network (PyG) integrating multi-source biological prior graphs with single-cell transcriptomics to prioritize checkpoint signaling axes.

**[LiDAR-OD](https://github.com/jinl33/LiDAR-OD)** — A modular 3D perception and camera-LiDAR calibration evaluation harness benchmarked on KITTI. Implements $SE(3)$ rigid-body transformations, intrinsic pinhole projection, frustum clipping, 3D oriented bounding boxes, and BEV IoU estimation. Features an automated Levenberg-Marquardt solver reaching $<0.8\text{ px}$ sub-pixel reprojection accuracy, an interactive Three.js scene viewer, and deterministic scenario presets for occlusion and range falloff.

**[ISR-PD-SpatialNiche](https://github.com/jinl33/ISR-PD-SpatialNiche)** — An audit-ready, containerized Nextflow batch pipeline integrating single-nucleus RNA-seq (207k nuclei, 28 donors) and spatial transcriptomics (10x Xenium and Visium). Automates quality control, Harmony batch correction, AUCell integrated stress response scoring, and CellChat/MISTy spatial interaction modeling with end-to-end data provenance.

**[stock-news-agent](https://github.com/jinl33/stock-news-agent)** — An autonomous event-intelligence pipeline that ingests streaming live feeds, executes LLM-based Retrieval-Augmented Generation (RAG) for thematic classification and significance scoring, and automatically dispatches structured operational alerts via scheduled GitHub Actions CI/CD workflows.

**[EZbooth](https://github.com/jinl33/EZbooth)** — A full-stack web-based 3D editor with mesh-level selection, scene hierarchy trees, and material editing. Implemented in React, TypeScript, and Three.js, backed by a Spring Boot and PostgreSQL REST service with OAuth 2.0 authentication.

---

## Core Technical Stack

* **Deep Learning & Foundation Models:** PyTorch · Distributed Data Parallel (DDP) · 3D Diffusion Models · Self-Supervised Learning · Knowledge Distillation · Graph Neural Networks (PyG)
* **Computer Vision & Perception:** 3D Point Cloud Processing · Camera-LiDAR Calibration · $SE(3)$ Rigid Transforms · Bounding Box Regression · Open3D · OpenCV
* **Data Engineering & HPC:** Nextflow (DSL2) · SLURM Clusters · Docker Containerization · Automated ETL · PostgreSQL · Linux/Bash · CI/CD
* **Statistical Rigor & Reliability:** Nested Cross-Validation · Sub-Group Failure Diagnostics · Paired Hypothesis Testing · Calibration Analysis · FAIR Data Lineage
