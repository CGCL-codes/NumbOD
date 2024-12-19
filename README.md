# NumbOD
The implementation of our AAAI 2025 paper "NumbOD: A Spatial-Frequency Fusion Attack Against Object Detectors"

![Python 3.8](https://img.shields.io/badge/python-3.8-green.svg?style=plastic)
![Pytorch 1.8.0](https://img.shields.io/badge/pytorch-1.8.0-red.svg?style=plastic)

## Abstract
With the advancement of deep learning, object detectors (ODs) with various architectures have achieved significant success in complex scenarios like autonomous driving. Previous adversarial attacks against ODs have been focused on designing customized attacks targeting their specific structures (\eg, NMS and RPN), yielding some results but simultaneously constraining their scalability.
Moreover, most efforts against ODs stem from image-level attacks originally designed for classification tasks, resulting in redundant computations and disturbances in object-irrelevant areas (e.g., background). Consequently, how to design a model-agnostic efficient attack to comprehensively evaluate the vulnerabilities of ODs remains challenging and unresolved.
In this paper, we propose NumbOD, a brand-new spatial-frequency fusion attack against various ODs, aimed at disrupting object detection within images. We directly leverage the features output by the OD without relying on its internal structures to craft adversarial examples. Specifically, we first design a dual-track attack target selection strategy to select high-quality bounding boxes from OD outputs for targeting. Subsequently, we employ directional perturbations to shift and compress  predicted boxes and change classification results to deceive ODs. Additionally, we focus on manipulating the high-frequency components of images to confuse ODs' attention on critical objects, thereby enhancing the attack efficiency.
Our extensive experiments on nine ODs and two datasets show that NumbOD achieves powerful attack performance and high stealthiness.


We're currently putting the code in order and it will be coming shortly.


## BibTeX 
If you find NumbOD both interesting and helpful, please consider citing us in your research or publications:
```bibtex
@inproceedings{zhou2025numbod,
  title={NumbOD: A Spatial-Frequency Fusion Attack Against Object Detectors},
  author={Zhou, Ziqi and Li, Bowen and Song, Yufei and Hu, Shengshan and Wan, Wei and Zhang, Leo Yu and Yao, Dezhong and Jin, Hai},
  booktitle={Proceedings of the 39th Annual AAAI Conference on Artificial Intelligence (AAAI'25)},
  year={2025}
}
```
