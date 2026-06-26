# Open-Source Ecosystem Exploration

## 1. Nerfstudio
* **Core Function:** A collaborative framework for NeRFs and 3D Gaussian Splatting. It provides high-level APIs for training, visualization, and evaluation.
* **Relevance to uniarx:** Serves as the primary sandbox for developing 3D reconstruction pipelines.
* **Recommendation:** Production-ready for research and prototyping; highly recommended for the initial development phase.

## 2. Open3D
* **Core Function:** A modern library for 3D data processing, including point cloud registration, visualization, and geometric deep learning.
* **Relevance to uniarx:** Necessary for preprocessing input datasets and performing quantitative analysis on reconstructed meshes/splats.
* **Recommendation:** Industry standard for 3D data manipulation.

## 3. NVIDIA TensorRT
* **Core Function:** A high-performance deep learning inference optimizer and runtime.
* **Relevance to uniarx:** Critical for meeting the real-time performance requirements of the KINOX project when deploying on Jetson hardware.
* **Recommendation:** Mandatory for any edge deployment scenarios involving NVIDIA hardware.
