---
title: "Very High-Order Compact Gas-Kinetic Scheme With Discontinuity Feedback Factor"
date: 2025-09-03
# 【关键点】保持纯文本，方便系统索引
tags: ["arXiv", "Compact Scheme", "CGKS", "Spectral-Like"]
# 建议：找一张展示 "Spectral-like resolution" 的频谱对比图，或者精细的旋涡结构图做封面
featureImage: "" 
summary: "J Mu, 𝗛 𝗭𝗵𝗮𝗻𝗴, X Ji†, Y Zhang, G Chen, K Xu  [ 📖 𝙖𝙧𝙓𝙞𝙫 𝙋𝙧𝙚𝙥𝙧𝙞𝙣𝙩 (2025) ] "
---

<div style="display: flex; flex-wrap: wrap; gap: 10px; margin-bottom: 20px;">
  <a href="#" target="_blank" style="text-decoration: none;">
    <img src="https://img.shields.io/badge/arXiv-2508.13705-007EC6?style=flat&logo=arxiv&logoColor=white" alt="arXiv PDF">
  </a>
  
  <a href="https://github.com/zhanghong24" target="_blank" style="text-decoration: none;">
    <img src="https://img.shields.io/badge/Code-GitHub-181717?style=flat&logo=github&logoColor=white" alt="Code">
  </a>
</div>

**Authors:** Junlei Mu, **Hong Zhang**, Xing Ji*, Yang Zhang, Gang Chen, Kun Xu

---

## Abstract

This paper presents a robust and efficient **Very High-Order** scheme for compressible flow simulation. By integrating the **Compact Gas-Kinetic Scheme (CGKS)** with the **Adaptive Stencil Extension with Discontinuity Feedback Factor (ASE-DFF)**, we achieve significant improvements in both robustness and computational efficiency.

Unlike traditional WENO schemes that suffer from large stencils and reduced robustness at very high orders, our proposed method maintains **spectral-like resolution** while effectively capturing strong shock waves without characteristic decomposition.

---

## 💡 The "Best of Both Worlds" Strategy

This work fuses two powerful technologies:

1.  **Compact GKS (CGKS)**: Provides **Spectral-like Resolution**. It evolves both cell averages ($W$) and cell slopes ($W_x$) simultaneously, achieving higher accuracy on smaller stencils.
    $$
    \frac{\partial W}{\partial t} + \nabla \cdot \mathbf{F} = 0, \quad \frac{\partial W_x}{\partial t} + \dots
    $$

2.  **ASE-DFF Reconstruction**: Provides **Extreme Robustness**. It uses the Discontinuity Feedback factor to adaptively control the interpolation order.

### Key Advantages:
* **Smaller Stencil**: 8th-order accuracy on a compact stencil (much smaller than WENO-9).
* **Lower Cost**: Bypasses the expensive smoothness indicators ($\beta_k$) calculation.
* [cite_start]**High Robustness**: Validated on challenging cases like double Mach reflection and viscous shock tubes[cite: 44, 45].

---

## 📊 Results Verification

The scheme demonstrates superior capability in capturing high-frequency waves (small vortices) compared to standard methods:

| Method | Resolution | Robustness | Cost |
| :--- | :--- | :--- | :--- |
| **Traditional WENO** | Good | Moderate | High |
| **Standard DG** | Excellent | Low (Fragile) | Very High |
| **Our CGKS+ASE** | **Spectral-like** | **High** | **Low** |

*(Benchmarks include Lax problem, Shu-Osher, and Blast Wave problems)*

---
{{< katex >}}
## 📝 Citation

```bibtex
@article{mu2025very,
  title={Very High-order Compact Gas-kinetic Scheme With Discontinuity Feedback Factor},
  author={Mu, Junlei and Zhang, Hong and Ji, Xing and Zhang, Yang and Chen, Gang and Xu, Kun},
  journal={arXiv preprint arXiv:2508.13705},
  year={2025}
}