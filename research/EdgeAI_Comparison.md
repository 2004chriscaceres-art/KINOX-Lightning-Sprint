# Edge AI Platform Comparison

| Feature | NVIDIA Jetson Nano | NVIDIA Jetson Orin Nano (8GB) | Raspberry Pi 5 (+ AI HAT+) | Intel NUC (Pro/Edge Series) |
| :--- | :--- | :--- | :--- | :--- |
| **Primary Use** | Prototyping (Legacy) | Edge AI/Robotics | Education/IoT/Light AI | Industrial/Desktop/GenAI |
| **GPU/NPU** | 128-core Maxwell | 1024-core Ampere | Hailo NPU (13-40 TOPS) | Integrated Iris Xe / Arc |
| **AI Performance** | ~0.47 TOPS | Up to 67 TOPS | 13–40 TOPS | Varies (up to 99+ TOPS) |
| **Power Draw** | 5W – 10W | 7W – 25W | 5W – 12W | 20W – 60W+ |
| **Best For** | Learning fundamentals | High-perf AI pipelines | Easy dev/affordable AI | Heavy, 24/7 reliability |

## Summary Recommendation
For uniarx's "KINOX" project, the **NVIDIA Jetson Orin Nano** is the recommended platform for high-performance edge AI, especially if the project involves real-time 3D reconstruction. The **Raspberry Pi 5** serves as an excellent, lower-cost alternative for prototyping initial computer vision pipelines.
