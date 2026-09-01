# Jinho Lee

M.S. Bioinformatics @ University of Michigan | Computer Vision & Generative Modeling

I build systems that learn structured representations from high-dimensional data—medical imaging, sensor streams, and single-cell genomics. I care as much about whether a model's evaluation actually holds up as I do about the model itself.

**Currently:** Training a 3D diffusion foundation model on multimodal MRI volumes, solving a hard GPU memory constraint through a wavelet-domain representation, and distilling it down 10x with zero measured loss in downstream performance.

[LinkedIn](https://linkedin.com/in/jin-lee-l804) · [Email](mailto:jinhlee@umich.edu)

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/-PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/-React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Three.js](https://img.shields.io/badge/-Three.js-000000?style=flat-square&logo=three.js&logoColor=white)
![Spring Boot](https://img.shields.io/badge/-Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

---

## At a Glance

| Metric / Scale | Context & Implementation |
| :--- | :--- |
| **8x memory reduction** | Wavelet-domain compression for 3D diffusion training; exactly invertible with no information loss |
| **10x model compression** | Self-supervised knowledge distillation ($232\text{M} \to 20\text{M}$ parameters) with zero downstream accuracy drop |
| **60,000+ volumes** | Multimodal MRI cohorts (T1w, T2w, DWI, FLAIR) utilized in foundation model pretraining |
| **207k nuclei, 28 donors** | Single-nucleus and spatial transcriptomics pipeline for Parkinson's disease cohort analysis |
| **1,337 protein nodes** | Affinity-weighted graph attention network for cell-cell signaling perturbation prediction |

---

## Projects

**[LiDAR-OD](https://github.com/jinl33/LiDAR-OD)** — A 3D perception evaluation pipeline built from raw sensor data on the KITTI benchmark. Features camera-LiDAR calibration, a Three.js dashboard with 9 camera modes and split 3D/BEV views, and 6 scenario presets (sparse returns, dense traffic, long range, occlusion)—built to construct edge-case conditions deliberately rather than relying on random validation splits.

**[stock-news-agent](https://github.com/jinl33/stock-news-agent)** — An autonomous agent that fetches live news feeds, runs LLM-based inference to classify and analyze market-relevant stories by theme and importance, and independently dispatches formatted alerts with zero human intervention, orchestrated via GitHub Actions.

**[EZbooth](https://github.com/jinl33/EZbooth)** — A full-stack web-based 3D editor with mesh-level selection, an object hierarchy tree, and per-object material editing. Implemented with React and TypeScript on Three.js for the frontend, backed by Kotlin and Spring Boot on PostgreSQL with OAuth 2.0 authentication.

**[ISR-PD-SpatialNiche](https://github.com/jinl33/ISR-PD-SpatialNiche)** — A reproducible Nextflow pipeline integrating single-nucleus RNA-seq (207k nuclei, 28 donors) and spatial transcriptomics (10x Xenium and Visium, 10 PD and 8 control donors), mapping neuroinflammatory signaling niches through Harmony batch correction, AUCell ISR signature scoring, and CellChat/MISTy interaction modeling.

**[Cell-to-Cell-Communication](https://github.com/jinl33/Cell-to-Cell-Communication)** — An affinity-weighted graph attention network integrating CellPhoneDB, BindingDB, and BioGRID with TNBC single-cell data across 1,337 protein nodes to predict cell-cell signaling perturbation, recovering the PD-L1/PD-1 immune checkpoint axis as a top predicted driver.

---

## Skills

* **Generative & Deep Learning:** PyTorch · Diffusion Models · Self-Supervised Learning · Knowledge Distillation · U-Net Architectures
* **Computer Vision:** Object Detection · Semantic Segmentation · 3D Scene Understanding · Camera-LiDAR Calibration · Point Cloud Processing
* **Genomics & Bioinformatics:** Scanpy · Seurat · Nextflow · Single-Cell & Spatial Transcriptomics
* **Full-Stack & Systems:** React · TypeScript · Three.js · Spring Boot · PostgreSQL · Docker · FastAPI
* **Evaluation & Reliability:** Cross-Validation · Model Calibration · Structured Failure Analysis · Ablation Testing
