---
title: "Adaptive High-Order Finite Volume Schemes based on Discontinuity Feedback Factor"
date: 2025-07-09
# 摘要已修正为讲习班背景
summary: "🎤 Presentation for the **2025 Summer School on Turbulence, Aeroacoustics, and CFD Methods**. Discussing the balance between high-order accuracy and robustness using the DF factor."

tags: ["Summer School", "CFD", "Turbulence", "Aeroacoustics", "CGKS"]

# 请确保有一张名为 2025-summer-cover.jpg 的封面图在 assets/img/
featureImage: "img/2025-datong.png"

article:
  showHero: true
  heroStyle: "background"
---

### 📅 Event Details

* [cite_start]**Event:** 2025 Summer School on Turbulence, Aeroacoustics, and CFD Methods (2025湍流、气动噪声及计算流体力学方法暑期高级讲习班) 
* [cite_start]**Location:** Datong, Shanxi, China [cite: 505]
* [cite_start]**Date:** August 8, 2025 [cite: 509]
* [cite_start]**Presenter:** **Hong Zhang** (Xi'an Jiaotong University) [cite: 510, 511]

---

### 💡 Abstract

[cite_start]As the order of numerical schemes increases, the conflict between **accuracy** and **robustness** becomes more prominent[cite: 91]. [cite_start]This talk explores the application of the **Discontinuity Feedback (DF) factor** to adaptively manage this trade-off in complex flow simulations[cite: 5].

**Core Topics Covered:**
* [cite_start]**Research Background:** Why high-order schemes (Order > 2) are essential for resolving fine turbulent structures and aeroacoustics[cite: 58, 59].
* [cite_start]**Methodology:** A reconstruction method based on the DF factor that accurately limits discontinuities within cells, which traditional cell-averaged methods often fail to do[cite: 104, 137].
* [cite_start]**Validation:** Robust performance on extreme cases, including **Mach 80** and **Mach 2000** astrophysical jets[cite: 439, 452].

---

### 📊 Results & Applications

[cite_start]The presentation demonstrates that the DF factor automatically satisfies the accuracy requirements of arbitrary high-order reconstruction while maintaining low computational and storage overhead[cite: 294, 299]. [cite_start]It forms a complete feedback loop within the algorithm, making parameters less sensitive and physical meanings clearer[cite: 259, 281].

---

### 📥 Download Slides

{{< button href="/files/2025-datong.pdf" target="_blank" >}}
  Download PDF Slides
{{< /button >}}