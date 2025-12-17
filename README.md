# Applied Computer Vision: Explainable & Edge AI Portfolio

This repository contains a two-part portfolio exploring critical frontiers in Applied AI: **Medical Interpretability** and **Industrial Edge Optimization**.

**Project Contributors:** Prahas Hegde, Rohan Sanjay Patil, Vidya Padmanabha.

**Academic Context:** Portfolio 2, Computer Vision.

---

## 🏥 Part I: Explainable AI in Medical Imaging

**The Challenge:** Bridging the "Trust Gap" in life-or-death medical decisions by making opaque deep learning models transparent for clinicians.

### Technical Overview

* **Model:** Fine-tuned **ResNet50** for binary classification (Normal vs. Pneumonia).


* **Performance:** Achieved **87% overall accuracy** with a high **Recall (94%)**, ensuring critical pneumonia cases are not missed.


* **Explainability Pipeline:** Integrated and compared two distinct XAI methods to justify predictions:


* **Grad-CAM:** A "white-box" approach using internal gradients to produce high-resolution, reproducible attention maps.


* **LIME:** A "black-box" approach that perturbs image regions to highlight intuitive, superpixel-level features.



---

## 🏭 Part II: Edge AI for Industry 4.0

**The Challenge:** Developing a high-speed, reliable vehicle verification system that performs local inference on the factory floor without cloud dependency.

### Technical Overview

* **Objective:** Optimize a **MobileNetV2** model to achieve **50% sparsity** while maintaining **>95% accuracy**.


* **Optimization Strategy:** Compared One-Shot vs. Iterative Pruning (L2 and Taylor methods).


* **Edge Hardware:** Designed for deployment on the **NVIDIA Jetson Nano**.




### Performance Results

* **Best Method:** Iterative Taylor Pruning maintained **95.2% accuracy** (only -0.2% drop).


* **Compression:** Successfully reduced model size from **8.9 MB to 6.1 MB**.


* **Latency:** Achieved inference speeds of **~60ms** using quantization, comfortably exceeding the factory requirement of >10 FPS.



System Architecture 

1. **Sensing Layer:** GigE Vision overhead cameras and position sensors.


2. **Edge Computing Layer:** NVIDIA Jetson Nano running a **TensorRT** inference engine.


3. **Decision Layer:** Industrial Ethernet triggers for pneumatic sorting gates (Gate A/B).



---

## 💡 Key Takeaways

* **Transparency:** A dual-method XAI approach (Grad-CAM + LIME) provides the most robust path to clinical trust.


* **Efficiency:** Iterative pruning is superior to one-shot methods for maintaining high accuracy in resource-constrained environments.



---
