
---

# **Stylized Motion – Python SDK Comparison (with VRAM requirements)**

| Stylized Motion Type             | AI / Non-AI | Python SDK / Library                     | Key Parameters                                       | GPU Required   | Min GPU / VRAM Requirement         | Feasibility to Standardization |
| -------------------------------- | ----------- | ---------------------------------------- | ---------------------------------------------------- | -------------- | ---------------------------------- | ------------------------------ |
| Morphing / Cross-Dissolve        | AI/Non-AI   | OpenCV, NumPy, DAIN, EbSynth             | blend\_ratio, speed, alignment                       | Optional / Yes | DAIN: 6–8 GB VRAM, EbSynth: CPU OK | Medium                         |
| Neural Style Transfer Animation  | AI          | PyTorch, TensorFlow, fast-style-transfer | style\_image, style\_strength, temporal\_consistency | Yes            | 6–8 GB VRAM (GTX 1660 / RTX 2060+) | Medium                         |
| Fractal / Recursive Zooms        | Non-AI      | OpenCV, PIL, NumPy                       | zoom\_factor, recursion\_depth, rotation             | No             | N/A                                | High                           |
| Glitch / Distortion Effects      | Non-AI      | OpenCV, MoviePy, NumPy                   | glitch\_intensity, frequency, region                 | No             | N/A                                | High                           |
| Transition Effects (Wipe, Slide) | Non-AI      | MoviePy, OpenCV                          | direction, speed, easing\_curve                      | No             | N/A                                | High                           |
| Particle / Procedural Motion     | Non-AI      | Pygame, Pyglet, Blender Python API       | particle\_count, velocity, lifespan                  | Optional / Yes | Blender smoke/fire: 6–8 GB VRAM    | Medium                         |
| Temporal Video Stylization       | AI          | Deforum SD, torchvideo, OpenCV           | style\_weight, temporal\_consistency                 | Yes            | 8–12 GB VRAM (RTX 3060–3090)       | Medium-Low                     |

---

⚡ **Quick notes**:

* **Non-AI methods**: run fine on CPU, scale with resolution.
* **AI-based methods**: VRAM is critical. Under 6 GB VRAM, most models (DAIN, style transfer, Deforum) will OOM on >720p video.
* **8–12 GB VRAM** (RTX 3060/3070/3090) is the sweet spot for smooth workflows.
* **24 GB VRAM+ (RTX 4090, A100)** → best for batching, long clips, and HD/4K.

---
