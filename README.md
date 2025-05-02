<div align="center">

# Garment-Diffusion: 3D Garment Sewing Pattern Generation with Multimodal Diffusion Transformers

**IJCAI 2025**

**[Xinyu Li](https://scholar.google.com/citations?hl=zh-CN&user=haWm-DoAAAAJ),
[Qi Yao](xxx),
[Yuanda Wang](xxx)**

**[[Project Page]](https://shenfu-research.github.io/Garment-Diffusion/)**, **[[Paper Link]](https://arxiv.org/abs/2504.21476)**

</div>

## Introduction
This repository is the official implementation of **GarmentDiffusion**, a generative model for 3D sewing pattern generation.

The key features of our model are:
- **Multimodal Inputs**: Our model takes in text, image, and incomplete sewing pattern as input modalities.
- **Efficient Edge Encoding Scheme**: We use an edge-oriented encoding method to encode the 3D sewing pattern parameters into compact edge token representations. This significantly reduces the sequence length of the edge tokens, allowing for faster training and generation.
- **Diffusion Transformer**: Our model uses a diffusion transformer to denoise all edge tokens along the temporal axis, maintaining a constant number of denoising steps regardless of dataset-specific edge and panel statistics.

We evaluate our model thoroughly on the [DressCodeData](https://github.com/IHe-KaiI/DressCode), [SewFactory](https://github.com/sail-sg/sewformer) and [GarmentCodeData](https://github.com/maria-korosteleva/GarmentCode) to validate the effectiveness of our method.

## Acknowledgment
This project takes the following works ([[BRepGen]](https://github.com/samxuxiang/BrepGen), [[DressCode]](https://github.com/IHe-KaiI/DressCode), [[PyGarment]](https://github.com/maria-korosteleva/GarmentCode), [[SewFormer]](https://github.com/sail-sg/sewformer)) as reference. We thank the authors of above projects for their great works.

We especially thank the authors of ([[Garment-Pattern-Generator]](https://github.com/maria-korosteleva/Garment-Pattern-Generator), [[GarmentCodeData]](https://github.com/maria-korosteleva/GarmentCode)) for providing the great garment sewing pattern datasets.

## Citation
```
@inproceedings{li2025garmentdiffusion,
  author    = {Li, Xinyu and Yao, Qi and Wang, Yuanda},
  title     = {GarmentDiffusion: 3D Garment Sewing Pattern Generation with Multimodal Diffusion Transformers},
  booktitle = {Proceedings of the 34th International Joint Conference on Artificial Intelligence (IJCAI)},
  year      = {2025},
  url       = {https://arxiv.org/abs/xxx}
}
```
