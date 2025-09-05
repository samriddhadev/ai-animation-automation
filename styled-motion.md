| Stylized Motion Type             | AI / Non-AI | Python SDK / Library                     | Key Parameters                                       | GPU Required   | Feasibility to Standardization |
| -------------------------------- | ----------- | ---------------------------------------- | ---------------------------------------------------- | -------------- | ------------------------------ |
| Morphing / Cross-Dissolve        | AI/Non-AI   | OpenCV, NumPy, DAIN, EbSynth             | blend\_ratio, speed, alignment                       | Optional / Yes | Medium                         |
| Neural Style Transfer Animation  | AI          | PyTorch, TensorFlow, fast-style-transfer | style\_image, style\_strength, temporal\_consistency | Yes            | Medium                         |
| Fractal / Recursive Zooms        | Non-AI      | OpenCV, PIL, NumPy                       | zoom\_factor, recursion\_depth, rotation             | No             | High                           |
| Glitch / Distortion Effects      | Non-AI      | OpenCV, MoviePy, NumPy                   | glitch\_intensity, frequency, region                 | No             | High                           |
| Transition Effects (Wipe, Slide) | Non-AI      | MoviePy, OpenCV                          | direction, speed, easing\_curve                      | No             | High                           |
| Particle / Procedural Motion     | Non-AI      | Pygame, Pyglet, Blender Python API       | particle\_count, velocity, lifespan                  | Optional / Yes | Medium                         |
| Temporal Video Stylization       | AI          | Deforum SD, torchvideo, OpenCV           | style\_weight, temporal\_consistency                 | Yes            | Medium-Low                     |
