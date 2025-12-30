---
title: "Adaptive High-Order Compact/Non-Compact Gas-Kinetic Schemes Based on Discontinuity Feedback Factor"
date: 2025-08-08
# A catchy summary for the list view
summary: "🎤 Presented at the **21st NMFD Conference**. Introducing the **Discontinuity Feedback (DF)** factor to achieve spectral-like resolution for hypersonic flows."

# Tags for filtering
tags: ["Conference", "Oral", "CFD", "Hypersonic", "High-Order Methods"]

# You need to export the first page of the PDF as an image and put it in assets/img/
featureImage: "img/2025-cfd-numericals.png"

# Enable the cool background effect
article:
  showHero: true
  heroStyle: "background"
---

### 📅 Event Details

* [cite_start]**Conference:** 21st Conference on Numerical Methods in Fluid Dynamics (第二十一届流体力学数值方法研讨会) [cite: 4]
* **Location:** Xi'an, China
* [cite_start]**Date:** August 8, 2025 [cite: 10]
* [cite_start]**Presenter:** **Hong Zhang** (Xi'an Jiaotong University) [cite: 7, 8]

---

### 💡 Abstract

[cite_start]High-order numerical schemes often struggle to balance **spectral-like resolution** with **shock-capturing robustness**, especially in hypersonic flows[cite: 91].

[cite_start]In this talk, I introduced a novel **Discontinuity Feedback (DF) Factor**[cite: 174]. [cite_start]Unlike traditional limiters that only rely on current time-step data, the DF factor utilizes interfacial discontinuity information from the previous step to guide the reconstruction of the next step, forming a closed-loop feedback system[cite: 268].

**Key Highlights:**
* [cite_start]**Mechanism:** The DF factor acts as a sensor ($\sigma_{i+1/2}$) to detect shocks, rarefaction waves, and shear layers[cite: 170, 283].
* [cite_start]**Efficiency:** It requires minimal computational cost ($O(k)$ complexity) compared to traditional WENO-Z or smoothness indicators[cite: 302, 309].
* [cite_start]**Extreme Robustness:** Successfully simulated **Mach 80** and **Mach 2000** astrophysical jets and hypersonic boundary layer interactions[cite: 439, 452].

---

### 📊 Key Results

The method was validated against complex benchmarks, demonstrating superior performance compared to standard WENO schemes:

1.  [cite_start]**Hypersonic Astrophysical Jet:** Stable simulations up to **Mach 2000**, capturing fine turbulent structures[cite: 452].
2.  [cite_start]**Two-Component Flows:** Accurately resolved Rayleigh-Taylor instability and shock-interface interactions[cite: 476].
3.  [cite_start]**Spectral Resolution:** The method achieves arbitrary high-order accuracy automatically for smooth flows[cite: 294].

---

### 📝 Related Publications

This presentation is based on the following research:

1.  **Zhang, H.**, Ji, X., & Xu, K. (2024). *A robustness-enhanced reconstruction based on discontinuity feedback factor for high-order finite volume scheme*. [cite_start]**Journal of Scientific Computing**, 101(1): 20. [cite: 513, 514]
2.  **Zhang, H.**, Ji, X., & Xu, K. (2024). *An Adaptive Reconstruction Method for Arbitrary High-Order Accuracy Using Discontinuity Feedback*. [cite_start]**arXiv preprint**. [cite: 523, 525]

---

### 📥 Download Slides

{{< button href="/files/2025-cfd-numericals.pdf" target="_blank" >}}
  Download PDF Slides
{{< /button >}}