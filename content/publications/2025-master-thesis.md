---
title: "Research on Highly Robust and High-Order Gas-Kinetic Schemes Based on Discontinuity Feedback Factor"
date: 2025-05-01
# 学位论文通常只写你自己，但为了索引，我们保持格式
authors: ["Hong Zhang"]
tags: ["Master Thesis", "XJTU", "GKS", "Robustness"]
# 建议：可以用论文封面的截图，或者西安交大的校徽/校门照片做封面
featureImage: "" 
summary: "𝗛 𝗭𝗵𝗮𝗻𝗴 [ 🎓 𝙈𝙖𝙨𝙩𝙚𝙧'𝙨 𝙏𝙝𝙚𝙨𝙞𝙨 (XJTU, 2025) ]"
---

<div style="display: flex; flex-wrap: wrap; gap: 10px; margin-bottom: 20px;">
  <a href="/files/ms-thesis.pdf" target="_blank" style="text-decoration: none;">
    <img src="https://img.shields.io/badge/Thesis-Master's_Degree-FFD700?style=flat&logo=googlescholar&logoColor=white" alt="Master Thesis">
  </a>
  
  <a href="http://www.xjtu.edu.cn/" target="_blank" style="text-decoration: none;">
    <img src="https://img.shields.io/badge/University-Xi'an%20Jiaotong%20University-003366?style=flat&logo=school&logoColor=white" alt="XJTU">
  </a>

  <span style="text-decoration: none;">
    <img src="https://img.shields.io/badge/Language-Chinese%20%2F%20English%20Abs-4CAF50?style=flat" alt="Language">
  </span>
</div>

**Author:** **Hong Zhang** 

**Supervisor:** Prof. Xing Ji

---

## Abstract

This thesis addresses the critical bottleneck in high-order Computational Fluid Dynamics (CFD): the conflict between **spectral-like resolution** and **shock-capturing robustness**. 

By introducing the **Discontinuity Feedback (DF)** factor, a novel sensor for local flow smoothness, this work constructs a unified framework for robust high-order schemes. The thesis covers theoretical derivation, algorithm design, and validation across varying flow regimes.

---

## 🔑 Key Contributions

1.  **Hybrid Reconstruction with DF**: 
    Proposed a mechanism to automatically switch between high-order WENO and robust low-order schemes based on the DF sensor, significantly enhancing stability in hypersonic flows.

2.  **Adaptive Stencil Extension (ASE)**:
    Developed a "bottom-up" reconstruction strategy that achieves arbitrary high-order accuracy (up to 9th order) without expensive smoothness indicators, reducing computational cost.

3.  **Multi-Component GKS**:
    Extended the DF framework to multi-component flows, designing a new density reconstruction method to eliminate numerical oscillations at material interfaces.

---

{{< katex >}}

## 📝 Citation

```bibtex
@mastersthesis{zhang2025master,
  title={Research on Highly Robust and High-Order Gas-Kinetic Schemes Based on Discontinuity Feedback Factor},
  author={Zhang, Hong},
  school={Xi'an Jiaotong University},
  year={2025},
  month={May},
  address={Xi'an, China}
}