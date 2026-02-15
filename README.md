# DAPASS: Denoise and Align: Towards Source-Free UDA for Robust Panoramic Semantic Segmentation

This is the official PyTorch implementation of the following publication:

> **DAPASS: Denoise and Align: Towards Source-Free UDA for Robust Panoramic Semantic Segmentation**<br/>
> [Yaowen Chang](https://pz0826.github.io/), [Zhen Cao](https://hpwang-whu.github.io/), [Zhen Dong](https://dongzhenwhu.github.io/index.html)
> *arXiv 2026*<br/>
> [**Full Paper**]() | [**Webpage**]() | [**Dataset**]()

## Introduction

<p align="center">
<strong>TL;DR: DAPASS achieves state-of-the-art performances on outdoor (Cityscapes-to-DensePASS) and indoor (Stanford2D3D) benchmarks, yielding 55.04\% (+2.05\%) and 70.38\% (+1.54\%) mIoU, respectively.</strong>
</p>

![Teaser image](assets/teaser_DAPASS.pdf)

<p align="justify">
  <strong>Abstract:</strong> Panoramic semantic segmentation is pivotal for comprehensive 360° scene understanding in critical applications like autonomous driving and virtual reality. However, progress in this domain is constrained by two key challenges: the severe geometric distortions inherent in panoramic projections and the prohibitive cost of dense annotation. While Unsupervised Domain Adaptation (UDA) from label-rich pinhole-camera datasets offers a viable alternative, many real-world tasks impose a stricter source-free (SFUDA) constraint where source data is inaccessible for privacy or proprietary reasons. This constraint significantly amplifies the core problems of domain shift, leading to unreliable pseudo-labels and dramatic performance degradation, particularly for minority classes. To overcome these limitations, we propose the DAPASS framework. DAPASS introduces two synergistic modules to robustly transfer knowledge without source data. First, our Panoramic Confidence-Guided Denoising (PCGD) module generates high-fidelity, class-balanced pseudo-labels by enforcing perturbation consistency and incorporating neighborhood-level confidence to filter noise. Second, a Cross-Resolution Attention Module (CRAM) explicitly addresses scale variance and distortion by adversarially aligning fine-grained details from high-resolution crops with global semantics from low-resolution contexts. DAPASS achieves state-of-the-art performances on outdoor (Cityscapes-to-DensePASS) and indoor (Stanford2D3D) benchmarks, yielding 55.04\% (+2.05\%) and 70.38\% (+1.54\%) mIoU, respectively.
</p>
