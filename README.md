# TGA3D: Texture-Geometry Admixture with Explicit 3D for Single-Image Novel View Synthesis
## Accepted by IEEE Trans on Multi Media (CCF-A, SCI TOP)

## Abstract
Single-image Novel View Synthesis (NVS) aims to generate photorealistic multi-view renderings of objects from a single image based on image-generative frameworks or implicit 3D neural representations. However, a fundamental trade-off persists. Image-based methods often sacrifice geometric fidelity due to insufficient 3D consistency, whereas implicit 3D representations of complex point clouds exhibit limited capacity to recover high-fidelity textures. We formulate this challenge as a dual-objective optimization problem, where preserving fine-grained textures conflicts with reconstructing precise 3D geometry. To reconcile this imbalance, we propose TGA3D, a Texture-Geometry Admixture framework that admixtures explicit 3D geometry reconstruction and detail-preserving texture alignment through frequency-aware disentanglement. Image contents are decomposed based on a frequency edge into low-frequency structural priors and high-frequency texture details via Pixel-Conditioned Prompts. In the Geometry-Aware Module, to iteratively refine geometric reconstructions and colour adjustments conditioned on structure information from low-frequency prompts, 3D-consistent geometric reconstructions integrate two-phase cross-attention layers. In the Texture-Align Module, to align fine surface details across synthesized views, multi-level feature mixtures fuse image features with high-frequency prompts guidance. A fusion module then amalgamates outputs from both branches, balancing geometric precision and textural fidelity. During training, to mimic the hierarchical integration of geometric priors and textural statistics observed in human cognition, TGA3D integrates pixel-level MSE optimization with geometric-aware KL divergence loss. 
Extensive experiments demonstrate that TGA3D achieves state-of-the-art performance.

Demo Video (Click to watch)
<div align="center">
  <a href="https://www.youtube.com/watch?v=eQSrY7SjrTQ" target="_blank">
    <img src="https://img.youtube.com/vi/eQSrY7SjrTQ/maxresdefault.jpg" alt="视频封面" width="80%">
  </a>
</div>
