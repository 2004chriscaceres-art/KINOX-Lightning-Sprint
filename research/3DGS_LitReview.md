# 3D Gaussian Splatting (3DGS) Literature Review

**Author:** [Chris Caceres]
**Date:** 2026-06-18
**Project:** KINOX Lightning Sprint - uniarx

## Introduction
This report summarizes three key papers foundational to 3D Gaussian Splatting. The goal is to understand the transition from traditional radiance fields to Gaussian-based real-time rendering.

---

## 1. 3D Gaussian Splatting for Real-Time Radiance Field Rendering (Kerbl et al., 2023)
* **Problem Statement:** Existing methods (like NeRF) are often too slow for real-time rendering and struggle with training efficiency.
* **Methodology:** Uses 3D Gaussians as a scene representation, optimized through a differentiable tile-based rasterizer.
* **Key Contributions:** Achieves high-quality, real-time rendering (1080p) while maintaining fast training times.
* **Limitations/Future Work:** Memory consumption can be high for complex, large-scale scenes.

## 2. DreamGaussian: Generative Gaussian Splatting (Tang et al., 2024)
* **Problem Statement:** Creating 3D assets from scratch (generative 3D) is traditionally slow and computationally expensive.
* **Methodology:** Combines a 2D diffusion model with a 3D Gaussian representation to "generate" 3D objects from text or single images.
* **Key Contributions:** Drastically accelerates 3D generation, making it practical for game asset pipelines.
* **Limitations/Future Work:** Texture and geometry consistency can still vary depending on the input prompt/image quality.

## 3. LightGaussian: Unbounded 3D Gaussian Compression with 16x Reduction (Fan et al., 2024)
* **Problem Statement:** Standard 3D Gaussian Splatting models produce massive files that are difficult to store and render on memory-constrained hardware.
* **Methodology:** Introduces a geometry-aware pruning and quantization method to compress the Gaussian representation while maintaining visual quality.
* **Key Contributions:** Achieves up to 16x reduction in model size, making it much more feasible to deploy 3DGS on edge or mobile devices.
* **Limitations/Future Work:** Requires a pre-trained model for compression; future work focuses on real-time on-device training capabilities.

---

## Synthesis for uniarx
3DGS offers a significant shift for game architecture, potentially replacing slower mesh-based workflows or complex NeRF pipelines. For future internships, exploring how to optimize these for mobile/edge platforms will be critical.
